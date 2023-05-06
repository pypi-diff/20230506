# Comparing `tmp/framelink-0.2.1.tar.gz` & `tmp/framelink-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "framelink-0.2.1.tar", last modified: Sat May  6 05:03:59 2023, max compression
+gzip compressed data, was "framelink-0.2.2.tar", last modified: Sat May  6 06:11:13 2023, max compression
```

## Comparing `framelink-0.2.1.tar` & `framelink-0.2.2.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 05:03:59.362071 framelink-0.2.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 05:03:59.350071 framelink-0.2.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 05:03:59.354071 framelink-0.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-05-06 05:02:59.000000 framelink-0.2.1/.github/workflows/lint_test_build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-06 05:02:59.000000 framelink-0.2.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-06 05:02:59.000000 framelink-0.2.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4660 2023-05-06 05:03:59.358071 framelink-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-05-06 05:02:59.000000 framelink-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 05:03:59.354071 framelink-0.2.1/data/
--rw-r--r--   0 runner    (1001) docker     (123)    19808 2023-05-06 05:02:59.000000 framelink-0.2.1/data/divy_trips_limited.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 05:03:59.350071 framelink-0.2.1/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 05:03:59.354071 framelink-0.2.1/examples/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)    52351 2023-05-06 05:02:59.000000 framelink-0.2.1/examples/notebooks/basic_pandas.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   309258 2023-05-06 05:02:59.000000 framelink-0.2.1/pdm.lock
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-05-06 05:02:59.000000 framelink-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 05:03:59.362071 framelink-0.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 05:03:59.350071 framelink-0.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 05:03:59.354071 framelink-0.2.1/src/framelink/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 05:02:59.000000 framelink-0.2.1/src/framelink/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 05:02:59.000000 framelink-0.2.1/src/framelink/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-06 05:03:59.000000 framelink-0.2.1/src/framelink/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-05-06 05:02:59.000000 framelink-0.2.1/src/framelink/_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-05-06 05:02:59.000000 framelink-0.2.1/src/framelink/_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    12870 2023-05-06 05:02:59.000000 framelink-0.2.1/src/framelink/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 05:03:59.358071 framelink-0.2.1/src/framelink/storage/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 05:02:59.000000 framelink-0.2.1/src/framelink/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-05-06 05:02:59.000000 framelink-0.2.1/src/framelink/storage/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-05-06 05:02:59.000000 framelink-0.2.1/src/framelink/storage/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-06 05:02:59.000000 framelink-0.2.1/src/framelink/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 05:03:59.358071 framelink-0.2.1/src/framelink.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4660 2023-05-06 05:03:59.000000 framelink-0.2.1/src/framelink.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-06 05:03:59.000000 framelink-0.2.1/src/framelink.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 05:03:59.000000 framelink-0.2.1/src/framelink.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-06 05:03:59.000000 framelink-0.2.1/src/framelink.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-06 05:03:59.000000 framelink-0.2.1/src/framelink.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-06 05:03:59.000000 framelink-0.2.1/src/framelink.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 05:03:59.358071 framelink-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 05:02:59.000000 framelink-0.2.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-06 05:02:59.000000 framelink-0.2.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 05:03:59.358071 framelink-0.2.1/tests/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 05:02:59.000000 framelink-0.2.1/tests/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-05-06 05:02:59.000000 framelink-0.2.1/tests/core/test_dag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-05-06 05:02:59.000000 framelink-0.2.1/tests/core/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-05-06 05:02:59.000000 framelink-0.2.1/tests/core/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-06 05:02:59.000000 framelink-0.2.1/tests/core/test_model_parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3845 2023-05-06 05:02:59.000000 framelink-0.2.1/tests/core/test_pipeline_metas.py
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-06 05:02:59.000000 framelink-0.2.1/tests/core/test_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-05-06 05:02:59.000000 framelink-0.2.1/tests/core/test_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-06 05:02:59.000000 framelink-0.2.1/tests/readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 06:11:13.583670 framelink-0.2.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 06:11:13.575670 framelink-0.2.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 06:11:13.579670 framelink-0.2.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-05-06 06:10:11.000000 framelink-0.2.2/.github/workflows/lint_test_build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-06 06:10:11.000000 framelink-0.2.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-06 06:10:11.000000 framelink-0.2.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-05-06 06:11:13.583670 framelink-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4899 2023-05-06 06:10:11.000000 framelink-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 06:11:13.579670 framelink-0.2.2/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    19808 2023-05-06 06:10:11.000000 framelink-0.2.2/data/divy_trips_limited.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 06:11:13.575670 framelink-0.2.2/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 06:11:13.579670 framelink-0.2.2/examples/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)    52351 2023-05-06 06:10:11.000000 framelink-0.2.2/examples/notebooks/basic_pandas.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   309258 2023-05-06 06:10:11.000000 framelink-0.2.2/pdm.lock
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-05-06 06:10:11.000000 framelink-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 06:11:13.583670 framelink-0.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 06:11:13.575670 framelink-0.2.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 06:11:13.579670 framelink-0.2.2/src/framelink/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 06:10:11.000000 framelink-0.2.2/src/framelink/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 06:10:11.000000 framelink-0.2.2/src/framelink/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-06 06:11:13.000000 framelink-0.2.2/src/framelink/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-05-06 06:10:11.000000 framelink-0.2.2/src/framelink/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-05-06 06:10:11.000000 framelink-0.2.2/src/framelink/_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12870 2023-05-06 06:10:11.000000 framelink-0.2.2/src/framelink/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 06:11:13.583670 framelink-0.2.2/src/framelink/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 06:10:11.000000 framelink-0.2.2/src/framelink/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-05-06 06:10:11.000000 framelink-0.2.2/src/framelink/storage/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-05-06 06:10:11.000000 framelink-0.2.2/src/framelink/storage/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-06 06:10:11.000000 framelink-0.2.2/src/framelink/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 06:11:13.583670 framelink-0.2.2/src/framelink.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-05-06 06:11:13.000000 framelink-0.2.2/src/framelink.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-06 06:11:13.000000 framelink-0.2.2/src/framelink.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 06:11:13.000000 framelink-0.2.2/src/framelink.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-06 06:11:13.000000 framelink-0.2.2/src/framelink.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-06 06:11:13.000000 framelink-0.2.2/src/framelink.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-06 06:11:13.000000 framelink-0.2.2/src/framelink.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 06:11:13.583670 framelink-0.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 06:10:11.000000 framelink-0.2.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-06 06:10:11.000000 framelink-0.2.2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 06:11:13.583670 framelink-0.2.2/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 06:10:11.000000 framelink-0.2.2/tests/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-05-06 06:10:11.000000 framelink-0.2.2/tests/core/test_dag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-05-06 06:10:11.000000 framelink-0.2.2/tests/core/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-05-06 06:10:11.000000 framelink-0.2.2/tests/core/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-06 06:10:11.000000 framelink-0.2.2/tests/core/test_model_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3845 2023-05-06 06:10:11.000000 framelink-0.2.2/tests/core/test_pipeline_metas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-06 06:10:11.000000 framelink-0.2.2/tests/core/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-05-06 06:10:11.000000 framelink-0.2.2/tests/core/test_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-06 06:10:11.000000 framelink-0.2.2/tests/readme.md
```

### Comparing `framelink-0.2.1/.github/workflows/lint_test_build.yml` & `framelink-0.2.2/.github/workflows/lint_test_build.yml`

 * *Files identical despite different names*

### Comparing `framelink-0.2.1/.pre-commit-config.yaml` & `framelink-0.2.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `framelink-0.2.1/PKG-INFO` & `framelink-0.2.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 Metadata-Version: 2.1
 Name: framelink
-Version: 0.2.1
+Version: 0.2.2
 Author-email: Toby Devlin <toby@tobydevlin.com>
 Project-URL: github, https://github.com/GitToby/framelink
+Keywords: data,DAG,orchastration,dataframe
+Classifier: Development Status :: 4 - Beta
 Requires-Python: <4.0,>=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: viz
 Provides-Extra: dev
 
-![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/gittoby/framelink/lint_test_build.yml)
-![GitHub Release Date](https://img.shields.io/github/release-date/GitToby/framelink)
+[![Version](https://img.shields.io/pypi/v/framelink)](https://pypi.org/project/framelink/)
+[![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/gittoby/framelink/lint_test_build.yml)](https://github.com/GitToby/framelink)
+[![GitHub Release Date](https://img.shields.io/github/release-date/GitToby/framelink)](https://github.com/GitToby/framelink)
+[![codecov](https://codecov.io/gh/GitToby/framelink/branch/master/graph/badge.svg?token=Uh8viFPyOG)](https://codecov.io/gh/GitToby/framelink)
+[![PyPi downloads](https://img.shields.io/pypi/dm/framelink)](https://pypi.org/project/framelink/)
 
-Framelink is a simple wrapper that will provide context into pandas, polars and other Dataframe engines. See roadmap
-below for future goals of the project.
+Framelink is a simple wrapper thats designed to provide context into pandas, polars and other Dataframe engines. See
+roadmap below for future of the project.
 
 **This project is still in prerelease, consider the API unstable. Any usage should be pinned.**
 
 ```bash
 pip install framelink
 ```
 
@@ -34,62 +39,64 @@
 ## Concepts
 
 - A **Pipeline** is a DAG of _models_ that can be executed in a particular way.
 - A **Model** is a definition of sourcing data and, potentially, a transform. It's an ETL in its most basic form.
 - A **Frame** is a result of a _model_ run.
 
 ## Features
+
 - [x] Model links & DAG + diagramming
 - [x] Context logging per model
 - [x] Diagramming and tracking of the model DAG
 - [x] Caches and auto-persistence
 - [ ] Dynamic sourcing for models
 - [x] Cli to run a project
+- [ ] Transpiler for popular DAG execution environments
 
 ## Example
 
 ```python
 from pathlib import Path
 
 import pandas as pd
 import polars as pl
 
 from framelink.core import FramelinkPipeline, FramelinkSettings
 from framelink.storage.core import PickleStorage, NoStorage
 
 settings = FramelinkSettings(
-  default_storage=PickleStorage(Path(__file__).parent / "data")
+    default_storage=PickleStorage(Path(__file__).parent / "data")
 )
 
 pipeline = FramelinkPipeline(settings=settings)
 
 
 @pipeline.model()
 def src_frame_1(_: FramelinkPipeline) -> pd.DataFrame:
-  return pd.DataFrame(data={
-    "name": ["amy", "peter"],
-    "age": [31, 12],
-  })
+    return pd.DataFrame(data={
+        "name": ["amy", "peter"],
+        "age": [31, 12],
+    })
 
 
 @pipeline.model(storage=NoStorage())
 def src_frame_2(_: FramelinkPipeline) -> pd.DataFrame:
-  return pd.DataFrame(data={
-    "name": ["amy", "peter", "helen"],
-    "fave_food": ["oranges", "chocolate", "water"],
-  })
+    return pd.DataFrame(data={
+        "name": ["amy", "peter", "helen"],
+        "fave_food": ["oranges", "chocolate", "water"],
+    })
 
 
 @pipeline.model()
 def merge_model(ctx: FramelinkPipeline) -> pl.DataFrame:
-  res_1 = ctx.ref(src_frame_1)
-  res_2 = ctx.ref(src_frame_2)
-  key = "name"
-  ctx.log.info(f"Merging both sources on {key}")
-  return pl.from_pandas(res_1).join(pl.from_pandas(res_2), on=key)
+    res_1 = ctx.ref(src_frame_1)
+    res_2 = ctx.ref(src_frame_2)
+    key = "name"
+    ctx.log.info(f"Merging both sources on {key}")
+    return pl.from_pandas(res_1).join(pl.from_pandas(res_2), on=key)
 
 
 # build with implicit context
 r_1 = pipeline.build(merge_model)
 print(r_1)
 # shape: (2, 3)
 # ┌───────┬─────┬───────────┐
```

### Comparing `framelink-0.2.1/README.md` & `framelink-0.2.2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,275 +1,307 @@
-00000000: 215b 4769 7448 7562 2057 6f72 6b66 6c6f  ![GitHub Workflo
-00000010: 7720 5374 6174 7573 5d28 6874 7470 733a  w Status](https:
-00000020: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
-00000030: 2f67 6974 6875 622f 6163 7469 6f6e 732f  /github/actions/
-00000040: 776f 726b 666c 6f77 2f73 7461 7475 732f  workflow/status/
-00000050: 6769 7474 6f62 792f 6672 616d 656c 696e  gittoby/framelin
-00000060: 6b2f 6c69 6e74 5f74 6573 745f 6275 696c  k/lint_test_buil
-00000070: 642e 796d 6c29 0a21 5b47 6974 4875 6220  d.yml).![GitHub 
-00000080: 5265 6c65 6173 6520 4461 7465 5d28 6874  Release Date](ht
-00000090: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
-000000a0: 732e 696f 2f67 6974 6875 622f 7265 6c65  s.io/github/rele
-000000b0: 6173 652d 6461 7465 2f47 6974 546f 6279  ase-date/GitToby
-000000c0: 2f66 7261 6d65 6c69 6e6b 290a 0a46 7261  /framelink)..Fra
-000000d0: 6d65 6c69 6e6b 2069 7320 6120 7369 6d70  melink is a simp
-000000e0: 6c65 2077 7261 7070 6572 2074 6861 7420  le wrapper that 
-000000f0: 7769 6c6c 2070 726f 7669 6465 2063 6f6e  will provide con
-00000100: 7465 7874 2069 6e74 6f20 7061 6e64 6173  text into pandas
-00000110: 2c20 706f 6c61 7273 2061 6e64 206f 7468  , polars and oth
-00000120: 6572 2044 6174 6166 7261 6d65 2065 6e67  er Dataframe eng
-00000130: 696e 6573 2e20 5365 6520 726f 6164 6d61  ines. See roadma
-00000140: 700a 6265 6c6f 7720 666f 7220 6675 7475  p.below for futu
-00000150: 7265 2067 6f61 6c73 206f 6620 7468 6520  re goals of the 
-00000160: 7072 6f6a 6563 742e 0a0a 2a2a 5468 6973  project...**This
-00000170: 2070 726f 6a65 6374 2069 7320 7374 696c   project is stil
-00000180: 6c20 696e 2070 7265 7265 6c65 6173 652c  l in prerelease,
-00000190: 2063 6f6e 7369 6465 7220 7468 6520 4150   consider the AP
-000001a0: 4920 756e 7374 6162 6c65 2e20 416e 7920  I unstable. Any 
-000001b0: 7573 6167 6520 7368 6f75 6c64 2062 6520  usage should be 
-000001c0: 7069 6e6e 6564 2e2a 2a0a 0a60 6060 6261  pinned.**..```ba
-000001d0: 7368 0a70 6970 2069 6e73 7461 6c6c 2066  sh.pip install f
-000001e0: 7261 6d65 6c69 6e6b 0a60 6060 0a0a 2323  ramelink.```..##
-000001f0: 2047 6f61 6c73 0a0a 4672 616d 656c 696e   Goals..Framelin
-00000200: 6b20 7368 6f75 6c64 2070 726f 7669 6465  k should provide
-00000210: 2061 2077 6179 2066 6f72 2063 6f6c 6c61   a way for colla
-00000220: 626f 7261 7469 6e67 2074 6561 6d73 2074  borating teams t
-00000230: 6f20 7772 6974 6520 7079 7468 6f6e 206f  o write python o
-00000240: 7220 5351 4c20 6d6f 6465 6c73 2074 6f20  r SQL models to 
-00000250: 7365 6520 7468 6569 7220 6461 7461 2066  see their data f
-00000260: 6c6f 7720 6561 7369 6c79 2061 6e64 2067  low easily and g
-00000270: 6574 2074 6865 2061 2077 686f 6c65 206c  et the a whole l
-00000280: 6f61 6420 6f66 2073 7475 6666 2066 6f72  oad of stuff for
-00000290: 2066 7265 6521 0a0a 2d20 2a2a 5369 6d70   free!..- **Simp
-000002a0: 6c65 2074 6f20 7772 6974 652a 2a20 2d20  le to write** - 
-000002b0: 7772 6974 696e 6720 6d6f 6465 6c73 2073  writing models s
-000002c0: 686f 756c 6420 6265 206e 6f20 6861 7264  hould be no hard
-000002d0: 6572 2074 6861 6e20 6120 6675 6e63 7469  er than a functi
-000002e0: 6f6e 2069 6d70 6c65 6d65 6e74 6174 696f  on implementatio
-000002f0: 6e20 6275 7420 7072 6f76 6964 6520 6120  n but provide a 
-00000300: 6465 7065 6e64 656e 6379 2074 7265 652c  dependency tree,
-00000310: 0a20 2073 6368 656d 6173 2026 206d 6f64  .  schemas & mod
-00000320: 656c 206d 6574 6164 6174 612e 0a2d 202a  el metadata..- *
-00000330: 2a53 696d 706c 6520 746f 2072 756e 2a2a  *Simple to run**
-00000340: 202d 2077 7269 7469 6e67 206d 6f64 656c   - writing model
-00000350: 7320 7368 6f75 6c64 2062 6520 6167 6e6f  s should be agno
-00000360: 7374 6963 206f 6620 7275 6e6e 696e 6720  stic of running 
-00000370: 6d6f 6465 6c73 2c20 6f6e 6365 2074 6865  models, once the
-00000380: 206d 6f64 656c 7320 6172 6520 7772 6974   models are writ
-00000390: 7465 6e20 6578 6563 7574 696f 6e0a 2020  ten execution.  
-000003a0: 7772 6170 7065 7273 2077 6974 6820 6469  wrappers with di
-000003b0: 6167 6e6f 7374 6963 732c 2074 7261 6369  agnostics, traci
-000003c0: 6e67 2026 206c 696e 6561 6765 2073 686f  ng & lineage sho
-000003d0: 756c 6420 6265 2065 6173 7920 746f 2064  uld be easy to d
-000003e0: 6572 6976 6520 666f 7220 7468 6520 6578  erive for the ex
-000003f0: 6563 7574 696f 6e20 706c 6174 666f 726d  ecution platform
-00000400: 2061 6e79 2074 6561 6d20 6973 2072 756e   any team is run
-00000410: 6e69 6e67 2077 6974 686f 7574 2068 6176  ning without hav
-00000420: 696e 6720 616e 7920 7370 6563 6961 6c20  ing any special 
-00000430: 7265 7175 6972 656d 656e 7473 2066 6f72  requirements for
-00000440: 2072 756e 6e69 6e67 206c 6f63 616c 6c79   running locally
-00000450: 2e0a 2d20 2a2a 5363 6865 6475 6c65 7220  ..- **Scheduler 
-00000460: 6167 6e6f 7374 6963 2a2a 202d 2077 6520  agnostic** - we 
-00000470: 6172 6520 6e6f 7420 6d61 6b69 6e67 2061  are not making a
-00000480: 206e 6577 2061 6972 666c 6f77 2c20 6461   new airflow, da
-00000490: 6773 7465 7220 6574 632e 2046 7261 6d65  gster etc. Frame
-000004a0: 6c69 6e6b 2073 6572 7665 7320 746f 2061  link serves to a
-000004b0: 6464 206d 6574 6164 6174 6120 746f 2061  dd metadata to a
-000004c0: 2070 726f 6a65 6374 0a20 2066 6f72 2066   project.  for f
-000004d0: 7265 652e 0a0a 2323 2043 6f6e 6365 7074  ree...## Concept
-000004e0: 730a 0a2d 2041 202a 2a50 6970 656c 696e  s..- A **Pipelin
-000004f0: 652a 2a20 6973 2061 2044 4147 206f 6620  e** is a DAG of 
-00000500: 5f6d 6f64 656c 735f 2074 6861 7420 6361  _models_ that ca
-00000510: 6e20 6265 2065 7865 6375 7465 6420 696e  n be executed in
-00000520: 2061 2070 6172 7469 6375 6c61 7220 7761   a particular wa
-00000530: 792e 0a2d 2041 202a 2a4d 6f64 656c 2a2a  y..- A **Model**
-00000540: 2069 7320 6120 6465 6669 6e69 7469 6f6e   is a definition
-00000550: 206f 6620 736f 7572 6369 6e67 2064 6174   of sourcing dat
-00000560: 6120 616e 642c 2070 6f74 656e 7469 616c  a and, potential
-00000570: 6c79 2c20 6120 7472 616e 7366 6f72 6d2e  ly, a transform.
-00000580: 2049 7427 7320 616e 2045 544c 2069 6e20   It's an ETL in 
-00000590: 6974 7320 6d6f 7374 2062 6173 6963 2066  its most basic f
-000005a0: 6f72 6d2e 0a2d 2041 202a 2a46 7261 6d65  orm..- A **Frame
-000005b0: 2a2a 2069 7320 6120 7265 7375 6c74 206f  ** is a result o
-000005c0: 6620 6120 5f6d 6f64 656c 5f20 7275 6e2e  f a _model_ run.
-000005d0: 0a0a 2323 2046 6561 7475 7265 730a 2d20  ..## Features.- 
-000005e0: 5b78 5d20 4d6f 6465 6c20 6c69 6e6b 7320  [x] Model links 
-000005f0: 2620 4441 4720 2b20 6469 6167 7261 6d6d  & DAG + diagramm
-00000600: 696e 670a 2d20 5b78 5d20 436f 6e74 6578  ing.- [x] Contex
-00000610: 7420 6c6f 6767 696e 6720 7065 7220 6d6f  t logging per mo
-00000620: 6465 6c0a 2d20 5b78 5d20 4469 6167 7261  del.- [x] Diagra
-00000630: 6d6d 696e 6720 616e 6420 7472 6163 6b69  mming and tracki
-00000640: 6e67 206f 6620 7468 6520 6d6f 6465 6c20  ng of the model 
-00000650: 4441 470a 2d20 5b78 5d20 4361 6368 6573  DAG.- [x] Caches
-00000660: 2061 6e64 2061 7574 6f2d 7065 7273 6973   and auto-persis
-00000670: 7465 6e63 650a 2d20 5b20 5d20 4479 6e61  tence.- [ ] Dyna
-00000680: 6d69 6320 736f 7572 6369 6e67 2066 6f72  mic sourcing for
-00000690: 206d 6f64 656c 730a 2d20 5b78 5d20 436c   models.- [x] Cl
-000006a0: 6920 746f 2072 756e 2061 2070 726f 6a65  i to run a proje
-000006b0: 6374 0a0a 2323 2045 7861 6d70 6c65 0a0a  ct..## Example..
-000006c0: 6060 6070 7974 686f 6e0a 6672 6f6d 2070  ```python.from p
-000006d0: 6174 686c 6962 2069 6d70 6f72 7420 5061  athlib import Pa
-000006e0: 7468 0a0a 696d 706f 7274 2070 616e 6461  th..import panda
-000006f0: 7320 6173 2070 640a 696d 706f 7274 2070  s as pd.import p
-00000700: 6f6c 6172 7320 6173 2070 6c0a 0a66 726f  olars as pl..fro
-00000710: 6d20 6672 616d 656c 696e 6b2e 636f 7265  m framelink.core
-00000720: 2069 6d70 6f72 7420 4672 616d 656c 696e   import Framelin
-00000730: 6b50 6970 656c 696e 652c 2046 7261 6d65  kPipeline, Frame
-00000740: 6c69 6e6b 5365 7474 696e 6773 0a66 726f  linkSettings.fro
-00000750: 6d20 6672 616d 656c 696e 6b2e 7374 6f72  m framelink.stor
-00000760: 6167 652e 636f 7265 2069 6d70 6f72 7420  age.core import 
-00000770: 5069 636b 6c65 5374 6f72 6167 652c 204e  PickleStorage, N
-00000780: 6f53 746f 7261 6765 0a0a 7365 7474 696e  oStorage..settin
-00000790: 6773 203d 2046 7261 6d65 6c69 6e6b 5365  gs = FramelinkSe
-000007a0: 7474 696e 6773 280a 2020 6465 6661 756c  ttings(.  defaul
-000007b0: 745f 7374 6f72 6167 653d 5069 636b 6c65  t_storage=Pickle
-000007c0: 5374 6f72 6167 6528 5061 7468 285f 5f66  Storage(Path(__f
-000007d0: 696c 655f 5f29 2e70 6172 656e 7420 2f20  ile__).parent / 
-000007e0: 2264 6174 6122 290a 290a 0a70 6970 656c  "data").)..pipel
-000007f0: 696e 6520 3d20 4672 616d 656c 696e 6b50  ine = FramelinkP
-00000800: 6970 656c 696e 6528 7365 7474 696e 6773  ipeline(settings
-00000810: 3d73 6574 7469 6e67 7329 0a0a 0a40 7069  =settings)...@pi
-00000820: 7065 6c69 6e65 2e6d 6f64 656c 2829 0a64  peline.model().d
-00000830: 6566 2073 7263 5f66 7261 6d65 5f31 285f  ef src_frame_1(_
-00000840: 3a20 4672 616d 656c 696e 6b50 6970 656c  : FramelinkPipel
-00000850: 696e 6529 202d 3e20 7064 2e44 6174 6146  ine) -> pd.DataF
-00000860: 7261 6d65 3a0a 2020 7265 7475 726e 2070  rame:.  return p
-00000870: 642e 4461 7461 4672 616d 6528 6461 7461  d.DataFrame(data
-00000880: 3d7b 0a20 2020 2022 6e61 6d65 223a 205b  ={.    "name": [
-00000890: 2261 6d79 222c 2022 7065 7465 7222 5d2c  "amy", "peter"],
-000008a0: 0a20 2020 2022 6167 6522 3a20 5b33 312c  .    "age": [31,
-000008b0: 2031 325d 2c0a 2020 7d29 0a0a 0a40 7069   12],.  })...@pi
-000008c0: 7065 6c69 6e65 2e6d 6f64 656c 2873 746f  peline.model(sto
-000008d0: 7261 6765 3d4e 6f53 746f 7261 6765 2829  rage=NoStorage()
-000008e0: 290a 6465 6620 7372 635f 6672 616d 655f  ).def src_frame_
-000008f0: 3228 5f3a 2046 7261 6d65 6c69 6e6b 5069  2(_: FramelinkPi
-00000900: 7065 6c69 6e65 2920 2d3e 2070 642e 4461  peline) -> pd.Da
-00000910: 7461 4672 616d 653a 0a20 2072 6574 7572  taFrame:.  retur
-00000920: 6e20 7064 2e44 6174 6146 7261 6d65 2864  n pd.DataFrame(d
-00000930: 6174 613d 7b0a 2020 2020 226e 616d 6522  ata={.    "name"
-00000940: 3a20 5b22 616d 7922 2c20 2270 6574 6572  : ["amy", "peter
-00000950: 222c 2022 6865 6c65 6e22 5d2c 0a20 2020  ", "helen"],.   
-00000960: 2022 6661 7665 5f66 6f6f 6422 3a20 5b22   "fave_food": ["
-00000970: 6f72 616e 6765 7322 2c20 2263 686f 636f  oranges", "choco
-00000980: 6c61 7465 222c 2022 7761 7465 7222 5d2c  late", "water"],
-00000990: 0a20 207d 290a 0a0a 4070 6970 656c 696e  .  })...@pipelin
-000009a0: 652e 6d6f 6465 6c28 290a 6465 6620 6d65  e.model().def me
-000009b0: 7267 655f 6d6f 6465 6c28 6374 783a 2046  rge_model(ctx: F
-000009c0: 7261 6d65 6c69 6e6b 5069 7065 6c69 6e65  ramelinkPipeline
-000009d0: 2920 2d3e 2070 6c2e 4461 7461 4672 616d  ) -> pl.DataFram
-000009e0: 653a 0a20 2072 6573 5f31 203d 2063 7478  e:.  res_1 = ctx
-000009f0: 2e72 6566 2873 7263 5f66 7261 6d65 5f31  .ref(src_frame_1
-00000a00: 290a 2020 7265 735f 3220 3d20 6374 782e  ).  res_2 = ctx.
-00000a10: 7265 6628 7372 635f 6672 616d 655f 3229  ref(src_frame_2)
-00000a20: 0a20 206b 6579 203d 2022 6e61 6d65 220a  .  key = "name".
-00000a30: 2020 6374 782e 6c6f 672e 696e 666f 2866    ctx.log.info(f
-00000a40: 224d 6572 6769 6e67 2062 6f74 6820 736f  "Merging both so
-00000a50: 7572 6365 7320 6f6e 207b 6b65 797d 2229  urces on {key}")
-00000a60: 0a20 2072 6574 7572 6e20 706c 2e66 726f  .  return pl.fro
-00000a70: 6d5f 7061 6e64 6173 2872 6573 5f31 292e  m_pandas(res_1).
-00000a80: 6a6f 696e 2870 6c2e 6672 6f6d 5f70 616e  join(pl.from_pan
-00000a90: 6461 7328 7265 735f 3229 2c20 6f6e 3d6b  das(res_2), on=k
-00000aa0: 6579 290a 0a0a 2320 6275 696c 6420 7769  ey)...# build wi
-00000ab0: 7468 2069 6d70 6c69 6369 7420 636f 6e74  th implicit cont
-00000ac0: 6578 740a 725f 3120 3d20 7069 7065 6c69  ext.r_1 = pipeli
-00000ad0: 6e65 2e62 7569 6c64 286d 6572 6765 5f6d  ne.build(merge_m
-00000ae0: 6f64 656c 290a 7072 696e 7428 725f 3129  odel).print(r_1)
-00000af0: 0a23 2073 6861 7065 3a20 2832 2c20 3329  .# shape: (2, 3)
-00000b00: 0a23 20e2 948c e294 80e2 9480 e294 80e2  .# .............
-00000b10: 9480 e294 80e2 9480 e294 80e2 94ac e294  ................
-00000b20: 80e2 9480 e294 80e2 9480 e294 80e2 94ac  ................
-00000b30: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00000b40: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00000b50: 80e2 9490 0a23 20e2 9482 206e 616d 6520  .....# ... name 
-00000b60: 20e2 9486 2061 6765 20e2 9486 2066 6176   ... age ... fav
-00000b70: 655f 666f 6f64 20e2 9482 0a23 20e2 9482  e_food ....# ...
-00000b80: 202d 2d2d 2020 20e2 9486 202d 2d2d 20e2   ---   ... --- .
-00000b90: 9486 202d 2d2d 2020 2020 2020 20e2 9482  .. ---       ...
-00000ba0: 0a23 20e2 9482 2073 7472 2020 20e2 9486  .# ... str   ...
-00000bb0: 2069 3634 20e2 9486 2073 7472 2020 2020   i64 ... str    
-00000bc0: 2020 20e2 9482 0a23 20e2 959e e295 90e2     ....# .......
-00000bd0: 9590 e295 90e2 9590 e295 90e2 9590 e295  ................
-00000be0: 90e2 95aa e295 90e2 9590 e295 90e2 9590  ................
-00000bf0: e295 90e2 95aa e295 90e2 9590 e295 90e2  ................
-00000c00: 9590 e295 90e2 9590 e295 90e2 9590 e295  ................
-00000c10: 90e2 9590 e295 90e2 95a1 0a23 20e2 9482  ...........# ...
-00000c20: 2061 6d79 2020 20e2 9486 2033 3120 20e2   amy   ... 31  .
-00000c30: 9486 206f 7261 6e67 6573 2020 20e2 9482  .. oranges   ...
-00000c40: 0a23 20e2 9482 2070 6574 6572 20e2 9486  .# ... peter ...
-00000c50: 2031 3220 20e2 9486 2063 686f 636f 6c61   12  ... chocola
-00000c60: 7465 20e2 9482 0a23 20e2 9494 e294 80e2  te ....# .......
-00000c70: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00000c80: 80e2 94b4 e294 80e2 9480 e294 80e2 9480  ................
-00000c90: e294 80e2 94b4 e294 80e2 9480 e294 80e2  ................
-00000ca0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00000cb0: 80e2 9480 e294 80e2 9498 0a0a 7072 696e  ............prin
-00000cc0: 7428 6d65 7267 655f 6d6f 6465 6c2e 7570  t(merge_model.up
-00000cd0: 7374 7265 616d 7329 0a23 207b 3c73 7263  streams).# {<src
-00000ce0: 5f66 7261 6d65 5f32 2061 7420 3078 3134  _frame_2 at 0x14
-00000cf0: 3737 6332 6339 303e 2c20 3c73 7263 5f66  77c2c90>, <src_f
-00000d00: 7261 6d65 5f31 2061 7420 3078 3134 3466  rame_1 at 0x144f
-00000d10: 3061 6235 303e 7d0a 0a70 7269 6e74 2873  0ab50>}..print(s
-00000d20: 7263 5f66 7261 6d65 5f31 2e64 6f77 6e73  rc_frame_1.downs
-00000d30: 7472 6561 6d73 290a 2320 7b3c 6d65 7267  treams).# {<merg
-00000d40: 655f 6d6f 6465 6c20 6174 2030 7831 3437  e_model at 0x147
-00000d50: 3763 3239 3130 3e7d 0a0a 7072 696e 7428  7c2910>}..print(
-00000d60: 7069 7065 6c69 6e65 2e6d 6f64 656c 5f6e  pipeline.model_n
-00000d70: 616d 6573 290a 2320 5b27 6d65 7267 655f  ames).# ['merge_
-00000d80: 6d6f 6465 6c27 2c20 2773 7263 5f66 7261  model', 'src_fra
-00000d90: 6d65 5f31 272c 2027 7372 635f 6672 616d  me_1', 'src_fram
-00000da0: 655f 3227 5d0a 0a70 7269 6e74 286c 6973  e_2']..print(lis
-00000db0: 7428 7069 7065 6c69 6e65 2e74 6f70 6f6c  t(pipeline.topol
-00000dc0: 6f67 6963 616c 5f73 6f72 7465 645f 6e6f  ogical_sorted_no
-00000dd0: 6465 7328 2929 290a 2320 5b28 3c73 7263  des())).# [(<src
-00000de0: 5f66 7261 6d65 5f31 2061 7420 3078 3134  _frame_1 at 0x14
-00000df0: 3466 3061 6235 303e 2c20 3c73 7263 5f66  4f0ab50>, <src_f
-00000e00: 7261 6d65 5f32 2061 7420 3078 3134 3737  rame_2 at 0x1477
-00000e10: 6332 6339 303e 292c 2028 3c6d 6572 6765  c2c90>), (<merge
-00000e20: 5f6d 6f64 656c 2061 7420 3078 3134 3737  _model at 0x1477
-00000e30: 6332 3931 303e 2c29 5d0a 0a23 2069 6620  c2910>,)]..# if 
-00000e40: 796f 7520 6861 7665 2074 6865 2067 7261  you have the gra
-00000e50: 7068 696e 6720 6f70 7469 6f6e 7320 656e  phing options en
-00000e60: 6761 6765 642e 0a70 6970 656c 696e 652e  gaged..pipeline.
-00000e70: 6772 6170 685f 706c 7428 2920 2023 2077  graph_plt()  # w
-00000e80: 696c 6c20 6472 6177 2079 6f75 2061 206d  ill draw you a m
-00000e90: 6174 706c 6f74 6c69 6220 6f66 2074 6865  atplotlib of the
-00000ea0: 2044 4147 0a64 6f74 203d 2070 6970 656c   DAG.dot = pipel
-00000eb0: 696e 652e 6772 6170 685f 646f 7428 2920  ine.graph_dot() 
-00000ec0: 2023 2077 696c 6c20 7072 6f76 6964 6520   # will provide 
-00000ed0: 6120 444f 5420 6c61 6e67 7561 6765 2072  a DOT language r
-00000ee0: 6570 7265 7365 6e74 6174 696f 6e20 6f66  epresentation of
-00000ef0: 2074 6865 2044 4147 0a60 6060 0a0a 2323   the DAG.```..##
-00000f00: 2046 6561 7475 7265 2052 6f61 646d 6170   Feature Roadmap
-00000f10: 0a0a 5468 6973 2063 6f75 6c64 2063 6861  ..This could cha
-00000f20: 6e67 652e 2e2e 0a0a 2323 2320 7630 2e32  nge.....### v0.2
-00000f30: 2e30 0a0a 2d20 5b78 5d20 4d6f 6465 6c20  .0..- [x] Model 
-00000f40: 6c69 6e6b 7320 2620 4441 4720 696d 706c  links & DAG impl
-00000f50: 656d 656e 7465 640a 2d20 5b78 5d20 436f  emented.- [x] Co
-00000f60: 6e74 6578 7420 6c6f 6767 6572 2061 7661  ntext logger ava
-00000f70: 696c 6162 6c65 0a2d 205b 785d 2044 6961  ilable.- [x] Dia
-00000f80: 6772 616d 6d69 6e67 2061 6e64 2074 7261  gramming and tra
-00000f90: 636b 696e 6720 6f66 2074 6865 206d 6f64  cking of the mod
-00000fa0: 656c 2044 4147 0a0a 2323 2320 7630 2e33  el DAG..### v0.3
-00000fb0: 2e30 0a0a 2d20 5b20 5d20 436c 6561 6e65  .0..- [ ] Cleane
-00000fc0: 7220 6772 6170 6820 7265 7375 6c74 730a  r graph results.
-00000fd0: 2d20 5b20 5d20 4d65 7267 696e 6720 6f66  - [ ] Merging of
-00000fe0: 206d 756c 7469 706c 6520 6672 616d 656c   multiple framel
-00000ff0: 696e 6b20 7069 7065 6c69 6e65 7320 656e  ink pipelines en
-00001000: 6162 6c69 6e67 0a2d 205b 205d 204f 7263  abling.- [ ] Orc
-00001010: 6865 7374 7261 7469 6f6e 2070 6173 7374  hestration passt
-00001020: 6872 6f75 6768 2061 6e64 206c 6f63 616c  hrough and local
-00001030: 2065 7865 6375 7469 6f6e 2e0a 2d20 5b78   execution..- [x
-00001040: 5d20 4361 6368 6573 2061 6e64 2061 7574  ] Caches and aut
-00001050: 6f2d 7065 7273 6973 7465 6e63 650a 2d20  o-persistence.- 
-00001060: 5b78 5d20 4479 6e61 6d69 6320 736f 7572  [x] Dynamic sour
-00001070: 6369 6e67 2066 6f72 206d 6f64 656c 730a  cing for models.
-00001080: 2d20 5b20 5d20 6d6f 6465 6c20 6f76 6572  - [ ] model over
-00001090: 7269 6465 7320 666f 7220 434c 4920 616e  rides for CLI an
-000010a0: 6420 7079 7468 6f6e 2072 756e 7469 6d65  d python runtime
-000010b0: 732e 0a2d 205b 785d 2043 6c69 2074 6f20  s..- [x] Cli to 
-000010c0: 7275 6e20 6120 7072 6f6a 6563 740a 0a23  run a project..#
-000010d0: 2323 2076 302e 342e 300a 0a2d 205b 205d  ## v0.4.0..- [ ]
-000010e0: 2053 514c 206d 6f64 656c 7320 2620 6462   SQL models & db
-000010f0: 742c 2073 716c 6d65 7368 2063 6f6d 7061  t, sqlmesh compa
-00001100: 7461 6269 6c69 7479 0a2d 205b 205d 204f  tability.- [ ] O
-00001110: 7065 6e20 5472 6163 696e 6720 696e 7465  pen Tracing inte
-00001120: 6772 6174 696f 6e0a                      gration.
+00000000: 5b21 5b56 6572 7369 6f6e 5d28 6874 7470  [![Version](http
+00000010: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
+00000020: 696f 2f70 7970 692f 762f 6672 616d 656c  io/pypi/v/framel
+00000030: 696e 6b29 5d28 6874 7470 733a 2f2f 7079  ink)](https://py
+00000040: 7069 2e6f 7267 2f70 726f 6a65 6374 2f66  pi.org/project/f
+00000050: 7261 6d65 6c69 6e6b 2f29 0a5b 215b 4769  ramelink/).[![Gi
+00000060: 7448 7562 2057 6f72 6b66 6c6f 7720 5374  tHub Workflow St
+00000070: 6174 7573 5d28 6874 7470 733a 2f2f 696d  atus](https://im
+00000080: 672e 7368 6965 6c64 732e 696f 2f67 6974  g.shields.io/git
+00000090: 6875 622f 6163 7469 6f6e 732f 776f 726b  hub/actions/work
+000000a0: 666c 6f77 2f73 7461 7475 732f 6769 7474  flow/status/gitt
+000000b0: 6f62 792f 6672 616d 656c 696e 6b2f 6c69  oby/framelink/li
+000000c0: 6e74 5f74 6573 745f 6275 696c 642e 796d  nt_test_build.ym
+000000d0: 6c29 5d28 6874 7470 733a 2f2f 6769 7468  l)](https://gith
+000000e0: 7562 2e63 6f6d 2f47 6974 546f 6279 2f66  ub.com/GitToby/f
+000000f0: 7261 6d65 6c69 6e6b 290a 5b21 5b47 6974  ramelink).[![Git
+00000100: 4875 6220 5265 6c65 6173 6520 4461 7465  Hub Release Date
+00000110: 5d28 6874 7470 733a 2f2f 696d 672e 7368  ](https://img.sh
+00000120: 6965 6c64 732e 696f 2f67 6974 6875 622f  ields.io/github/
+00000130: 7265 6c65 6173 652d 6461 7465 2f47 6974  release-date/Git
+00000140: 546f 6279 2f66 7261 6d65 6c69 6e6b 295d  Toby/framelink)]
+00000150: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00000160: 636f 6d2f 4769 7454 6f62 792f 6672 616d  com/GitToby/fram
+00000170: 656c 696e 6b29 0a5b 215b 636f 6465 636f  elink).[![codeco
+00000180: 765d 2868 7474 7073 3a2f 2f63 6f64 6563  v](https://codec
+00000190: 6f76 2e69 6f2f 6768 2f47 6974 546f 6279  ov.io/gh/GitToby
+000001a0: 2f66 7261 6d65 6c69 6e6b 2f62 7261 6e63  /framelink/branc
+000001b0: 682f 6d61 7374 6572 2f67 7261 7068 2f62  h/master/graph/b
+000001c0: 6164 6765 2e73 7667 3f74 6f6b 656e 3d55  adge.svg?token=U
+000001d0: 6838 7669 4650 794f 4729 5d28 6874 7470  h8viFPyOG)](http
+000001e0: 733a 2f2f 636f 6465 636f 762e 696f 2f67  s://codecov.io/g
+000001f0: 682f 4769 7454 6f62 792f 6672 616d 656c  h/GitToby/framel
+00000200: 696e 6b29 0a5b 215b 5079 5069 2064 6f77  ink).[![PyPi dow
+00000210: 6e6c 6f61 6473 5d28 6874 7470 733a 2f2f  nloads](https://
+00000220: 696d 672e 7368 6965 6c64 732e 696f 2f70  img.shields.io/p
+00000230: 7970 692f 646d 2f66 7261 6d65 6c69 6e6b  ypi/dm/framelink
+00000240: 295d 2868 7474 7073 3a2f 2f70 7970 692e  )](https://pypi.
+00000250: 6f72 672f 7072 6f6a 6563 742f 6672 616d  org/project/fram
+00000260: 656c 696e 6b2f 290a 0a46 7261 6d65 6c69  elink/)..Frameli
+00000270: 6e6b 2069 7320 6120 7369 6d70 6c65 2077  nk is a simple w
+00000280: 7261 7070 6572 2074 6861 7473 2064 6573  rapper thats des
+00000290: 6967 6e65 6420 746f 2070 726f 7669 6465  igned to provide
+000002a0: 2063 6f6e 7465 7874 2069 6e74 6f20 7061   context into pa
+000002b0: 6e64 6173 2c20 706f 6c61 7273 2061 6e64  ndas, polars and
+000002c0: 206f 7468 6572 2044 6174 6166 7261 6d65   other Dataframe
+000002d0: 2065 6e67 696e 6573 2e20 5365 650a 726f   engines. See.ro
+000002e0: 6164 6d61 7020 6265 6c6f 7720 666f 7220  admap below for 
+000002f0: 6675 7475 7265 206f 6620 7468 6520 7072  future of the pr
+00000300: 6f6a 6563 742e 0a0a 2a2a 5468 6973 2070  oject...**This p
+00000310: 726f 6a65 6374 2069 7320 7374 696c 6c20  roject is still 
+00000320: 696e 2070 7265 7265 6c65 6173 652c 2063  in prerelease, c
+00000330: 6f6e 7369 6465 7220 7468 6520 4150 4920  onsider the API 
+00000340: 756e 7374 6162 6c65 2e20 416e 7920 7573  unstable. Any us
+00000350: 6167 6520 7368 6f75 6c64 2062 6520 7069  age should be pi
+00000360: 6e6e 6564 2e2a 2a0a 0a60 6060 6261 7368  nned.**..```bash
+00000370: 0a70 6970 2069 6e73 7461 6c6c 2066 7261  .pip install fra
+00000380: 6d65 6c69 6e6b 0a60 6060 0a0a 2323 2047  melink.```..## G
+00000390: 6f61 6c73 0a0a 4672 616d 656c 696e 6b20  oals..Framelink 
+000003a0: 7368 6f75 6c64 2070 726f 7669 6465 2061  should provide a
+000003b0: 2077 6179 2066 6f72 2063 6f6c 6c61 626f   way for collabo
+000003c0: 7261 7469 6e67 2074 6561 6d73 2074 6f20  rating teams to 
+000003d0: 7772 6974 6520 7079 7468 6f6e 206f 7220  write python or 
+000003e0: 5351 4c20 6d6f 6465 6c73 2074 6f20 7365  SQL models to se
+000003f0: 6520 7468 6569 7220 6461 7461 2066 6c6f  e their data flo
+00000400: 7720 6561 7369 6c79 2061 6e64 2067 6574  w easily and get
+00000410: 2074 6865 2061 2077 686f 6c65 206c 6f61   the a whole loa
+00000420: 6420 6f66 2073 7475 6666 2066 6f72 2066  d of stuff for f
+00000430: 7265 6521 0a0a 2d20 2a2a 5369 6d70 6c65  ree!..- **Simple
+00000440: 2074 6f20 7772 6974 652a 2a20 2d20 7772   to write** - wr
+00000450: 6974 696e 6720 6d6f 6465 6c73 2073 686f  iting models sho
+00000460: 756c 6420 6265 206e 6f20 6861 7264 6572  uld be no harder
+00000470: 2074 6861 6e20 6120 6675 6e63 7469 6f6e   than a function
+00000480: 2069 6d70 6c65 6d65 6e74 6174 696f 6e20   implementation 
+00000490: 6275 7420 7072 6f76 6964 6520 6120 6465  but provide a de
+000004a0: 7065 6e64 656e 6379 2074 7265 652c 0a20  pendency tree,. 
+000004b0: 2073 6368 656d 6173 2026 206d 6f64 656c   schemas & model
+000004c0: 206d 6574 6164 6174 612e 0a2d 202a 2a53   metadata..- **S
+000004d0: 696d 706c 6520 746f 2072 756e 2a2a 202d  imple to run** -
+000004e0: 2077 7269 7469 6e67 206d 6f64 656c 7320   writing models 
+000004f0: 7368 6f75 6c64 2062 6520 6167 6e6f 7374  should be agnost
+00000500: 6963 206f 6620 7275 6e6e 696e 6720 6d6f  ic of running mo
+00000510: 6465 6c73 2c20 6f6e 6365 2074 6865 206d  dels, once the m
+00000520: 6f64 656c 7320 6172 6520 7772 6974 7465  odels are writte
+00000530: 6e20 6578 6563 7574 696f 6e0a 2020 7772  n execution.  wr
+00000540: 6170 7065 7273 2077 6974 6820 6469 6167  appers with diag
+00000550: 6e6f 7374 6963 732c 2074 7261 6369 6e67  nostics, tracing
+00000560: 2026 206c 696e 6561 6765 2073 686f 756c   & lineage shoul
+00000570: 6420 6265 2065 6173 7920 746f 2064 6572  d be easy to der
+00000580: 6976 6520 666f 7220 7468 6520 6578 6563  ive for the exec
+00000590: 7574 696f 6e20 706c 6174 666f 726d 2061  ution platform a
+000005a0: 6e79 2074 6561 6d20 6973 2072 756e 6e69  ny team is runni
+000005b0: 6e67 2077 6974 686f 7574 2068 6176 696e  ng without havin
+000005c0: 6720 616e 7920 7370 6563 6961 6c20 7265  g any special re
+000005d0: 7175 6972 656d 656e 7473 2066 6f72 2072  quirements for r
+000005e0: 756e 6e69 6e67 206c 6f63 616c 6c79 2e0a  unning locally..
+000005f0: 2d20 2a2a 5363 6865 6475 6c65 7220 6167  - **Scheduler ag
+00000600: 6e6f 7374 6963 2a2a 202d 2077 6520 6172  nostic** - we ar
+00000610: 6520 6e6f 7420 6d61 6b69 6e67 2061 206e  e not making a n
+00000620: 6577 2061 6972 666c 6f77 2c20 6461 6773  ew airflow, dags
+00000630: 7465 7220 6574 632e 2046 7261 6d65 6c69  ter etc. Frameli
+00000640: 6e6b 2073 6572 7665 7320 746f 2061 6464  nk serves to add
+00000650: 206d 6574 6164 6174 6120 746f 2061 2070   metadata to a p
+00000660: 726f 6a65 6374 0a20 2066 6f72 2066 7265  roject.  for fre
+00000670: 652e 0a0a 2323 2043 6f6e 6365 7074 730a  e...## Concepts.
+00000680: 0a2d 2041 202a 2a50 6970 656c 696e 652a  .- A **Pipeline*
+00000690: 2a20 6973 2061 2044 4147 206f 6620 5f6d  * is a DAG of _m
+000006a0: 6f64 656c 735f 2074 6861 7420 6361 6e20  odels_ that can 
+000006b0: 6265 2065 7865 6375 7465 6420 696e 2061  be executed in a
+000006c0: 2070 6172 7469 6375 6c61 7220 7761 792e   particular way.
+000006d0: 0a2d 2041 202a 2a4d 6f64 656c 2a2a 2069  .- A **Model** i
+000006e0: 7320 6120 6465 6669 6e69 7469 6f6e 206f  s a definition o
+000006f0: 6620 736f 7572 6369 6e67 2064 6174 6120  f sourcing data 
+00000700: 616e 642c 2070 6f74 656e 7469 616c 6c79  and, potentially
+00000710: 2c20 6120 7472 616e 7366 6f72 6d2e 2049  , a transform. I
+00000720: 7427 7320 616e 2045 544c 2069 6e20 6974  t's an ETL in it
+00000730: 7320 6d6f 7374 2062 6173 6963 2066 6f72  s most basic for
+00000740: 6d2e 0a2d 2041 202a 2a46 7261 6d65 2a2a  m..- A **Frame**
+00000750: 2069 7320 6120 7265 7375 6c74 206f 6620   is a result of 
+00000760: 6120 5f6d 6f64 656c 5f20 7275 6e2e 0a0a  a _model_ run...
+00000770: 2323 2046 6561 7475 7265 730a 0a2d 205b  ## Features..- [
+00000780: 785d 204d 6f64 656c 206c 696e 6b73 2026  x] Model links &
+00000790: 2044 4147 202b 2064 6961 6772 616d 6d69   DAG + diagrammi
+000007a0: 6e67 0a2d 205b 785d 2043 6f6e 7465 7874  ng.- [x] Context
+000007b0: 206c 6f67 6769 6e67 2070 6572 206d 6f64   logging per mod
+000007c0: 656c 0a2d 205b 785d 2044 6961 6772 616d  el.- [x] Diagram
+000007d0: 6d69 6e67 2061 6e64 2074 7261 636b 696e  ming and trackin
+000007e0: 6720 6f66 2074 6865 206d 6f64 656c 2044  g of the model D
+000007f0: 4147 0a2d 205b 785d 2043 6163 6865 7320  AG.- [x] Caches 
+00000800: 616e 6420 6175 746f 2d70 6572 7369 7374  and auto-persist
+00000810: 656e 6365 0a2d 205b 205d 2044 796e 616d  ence.- [ ] Dynam
+00000820: 6963 2073 6f75 7263 696e 6720 666f 7220  ic sourcing for 
+00000830: 6d6f 6465 6c73 0a2d 205b 785d 2043 6c69  models.- [x] Cli
+00000840: 2074 6f20 7275 6e20 6120 7072 6f6a 6563   to run a projec
+00000850: 740a 2d20 5b20 5d20 5472 616e 7370 696c  t.- [ ] Transpil
+00000860: 6572 2066 6f72 2070 6f70 756c 6172 2044  er for popular D
+00000870: 4147 2065 7865 6375 7469 6f6e 2065 6e76  AG execution env
+00000880: 6972 6f6e 6d65 6e74 730a 0a23 2320 4578  ironments..## Ex
+00000890: 616d 706c 650a 0a60 6060 7079 7468 6f6e  ample..```python
+000008a0: 0a66 726f 6d20 7061 7468 6c69 6220 696d  .from pathlib im
+000008b0: 706f 7274 2050 6174 680a 0a69 6d70 6f72  port Path..impor
+000008c0: 7420 7061 6e64 6173 2061 7320 7064 0a69  t pandas as pd.i
+000008d0: 6d70 6f72 7420 706f 6c61 7273 2061 7320  mport polars as 
+000008e0: 706c 0a0a 6672 6f6d 2066 7261 6d65 6c69  pl..from frameli
+000008f0: 6e6b 2e63 6f72 6520 696d 706f 7274 2046  nk.core import F
+00000900: 7261 6d65 6c69 6e6b 5069 7065 6c69 6e65  ramelinkPipeline
+00000910: 2c20 4672 616d 656c 696e 6b53 6574 7469  , FramelinkSetti
+00000920: 6e67 730a 6672 6f6d 2066 7261 6d65 6c69  ngs.from frameli
+00000930: 6e6b 2e73 746f 7261 6765 2e63 6f72 6520  nk.storage.core 
+00000940: 696d 706f 7274 2050 6963 6b6c 6553 746f  import PickleSto
+00000950: 7261 6765 2c20 4e6f 5374 6f72 6167 650a  rage, NoStorage.
+00000960: 0a73 6574 7469 6e67 7320 3d20 4672 616d  .settings = Fram
+00000970: 656c 696e 6b53 6574 7469 6e67 7328 0a20  elinkSettings(. 
+00000980: 2020 2064 6566 6175 6c74 5f73 746f 7261     default_stora
+00000990: 6765 3d50 6963 6b6c 6553 746f 7261 6765  ge=PickleStorage
+000009a0: 2850 6174 6828 5f5f 6669 6c65 5f5f 292e  (Path(__file__).
+000009b0: 7061 7265 6e74 202f 2022 6461 7461 2229  parent / "data")
+000009c0: 0a29 0a0a 7069 7065 6c69 6e65 203d 2046  .)..pipeline = F
+000009d0: 7261 6d65 6c69 6e6b 5069 7065 6c69 6e65  ramelinkPipeline
+000009e0: 2873 6574 7469 6e67 733d 7365 7474 696e  (settings=settin
+000009f0: 6773 290a 0a0a 4070 6970 656c 696e 652e  gs)...@pipeline.
+00000a00: 6d6f 6465 6c28 290a 6465 6620 7372 635f  model().def src_
+00000a10: 6672 616d 655f 3128 5f3a 2046 7261 6d65  frame_1(_: Frame
+00000a20: 6c69 6e6b 5069 7065 6c69 6e65 2920 2d3e  linkPipeline) ->
+00000a30: 2070 642e 4461 7461 4672 616d 653a 0a20   pd.DataFrame:. 
+00000a40: 2020 2072 6574 7572 6e20 7064 2e44 6174     return pd.Dat
+00000a50: 6146 7261 6d65 2864 6174 613d 7b0a 2020  aFrame(data={.  
+00000a60: 2020 2020 2020 226e 616d 6522 3a20 5b22        "name": ["
+00000a70: 616d 7922 2c20 2270 6574 6572 225d 2c0a  amy", "peter"],.
+00000a80: 2020 2020 2020 2020 2261 6765 223a 205b          "age": [
+00000a90: 3331 2c20 3132 5d2c 0a20 2020 207d 290a  31, 12],.    }).
+00000aa0: 0a0a 4070 6970 656c 696e 652e 6d6f 6465  ..@pipeline.mode
+00000ab0: 6c28 7374 6f72 6167 653d 4e6f 5374 6f72  l(storage=NoStor
+00000ac0: 6167 6528 2929 0a64 6566 2073 7263 5f66  age()).def src_f
+00000ad0: 7261 6d65 5f32 285f 3a20 4672 616d 656c  rame_2(_: Framel
+00000ae0: 696e 6b50 6970 656c 696e 6529 202d 3e20  inkPipeline) -> 
+00000af0: 7064 2e44 6174 6146 7261 6d65 3a0a 2020  pd.DataFrame:.  
+00000b00: 2020 7265 7475 726e 2070 642e 4461 7461    return pd.Data
+00000b10: 4672 616d 6528 6461 7461 3d7b 0a20 2020  Frame(data={.   
+00000b20: 2020 2020 2022 6e61 6d65 223a 205b 2261       "name": ["a
+00000b30: 6d79 222c 2022 7065 7465 7222 2c20 2268  my", "peter", "h
+00000b40: 656c 656e 225d 2c0a 2020 2020 2020 2020  elen"],.        
+00000b50: 2266 6176 655f 666f 6f64 223a 205b 226f  "fave_food": ["o
+00000b60: 7261 6e67 6573 222c 2022 6368 6f63 6f6c  ranges", "chocol
+00000b70: 6174 6522 2c20 2277 6174 6572 225d 2c0a  ate", "water"],.
+00000b80: 2020 2020 7d29 0a0a 0a40 7069 7065 6c69      })...@pipeli
+00000b90: 6e65 2e6d 6f64 656c 2829 0a64 6566 206d  ne.model().def m
+00000ba0: 6572 6765 5f6d 6f64 656c 2863 7478 3a20  erge_model(ctx: 
+00000bb0: 4672 616d 656c 696e 6b50 6970 656c 696e  FramelinkPipelin
+00000bc0: 6529 202d 3e20 706c 2e44 6174 6146 7261  e) -> pl.DataFra
+00000bd0: 6d65 3a0a 2020 2020 7265 735f 3120 3d20  me:.    res_1 = 
+00000be0: 6374 782e 7265 6628 7372 635f 6672 616d  ctx.ref(src_fram
+00000bf0: 655f 3129 0a20 2020 2072 6573 5f32 203d  e_1).    res_2 =
+00000c00: 2063 7478 2e72 6566 2873 7263 5f66 7261   ctx.ref(src_fra
+00000c10: 6d65 5f32 290a 2020 2020 6b65 7920 3d20  me_2).    key = 
+00000c20: 226e 616d 6522 0a20 2020 2063 7478 2e6c  "name".    ctx.l
+00000c30: 6f67 2e69 6e66 6f28 6622 4d65 7267 696e  og.info(f"Mergin
+00000c40: 6720 626f 7468 2073 6f75 7263 6573 206f  g both sources o
+00000c50: 6e20 7b6b 6579 7d22 290a 2020 2020 7265  n {key}").    re
+00000c60: 7475 726e 2070 6c2e 6672 6f6d 5f70 616e  turn pl.from_pan
+00000c70: 6461 7328 7265 735f 3129 2e6a 6f69 6e28  das(res_1).join(
+00000c80: 706c 2e66 726f 6d5f 7061 6e64 6173 2872  pl.from_pandas(r
+00000c90: 6573 5f32 292c 206f 6e3d 6b65 7929 0a0a  es_2), on=key)..
+00000ca0: 0a23 2062 7569 6c64 2077 6974 6820 696d  .# build with im
+00000cb0: 706c 6963 6974 2063 6f6e 7465 7874 0a72  plicit context.r
+00000cc0: 5f31 203d 2070 6970 656c 696e 652e 6275  _1 = pipeline.bu
+00000cd0: 696c 6428 6d65 7267 655f 6d6f 6465 6c29  ild(merge_model)
+00000ce0: 0a70 7269 6e74 2872 5f31 290a 2320 7368  .print(r_1).# sh
+00000cf0: 6170 653a 2028 322c 2033 290a 2320 e294  ape: (2, 3).# ..
+00000d00: 8ce2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00000d10: e294 80e2 9480 e294 ace2 9480 e294 80e2  ................
+00000d20: 9480 e294 80e2 9480 e294 ace2 9480 e294  ................
+00000d30: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00000d40: e294 80e2 9480 e294 80e2 9480 e294 900a  ................
+00000d50: 2320 e294 8220 6e61 6d65 2020 e294 8620  # ... name  ... 
+00000d60: 6167 6520 e294 8620 6661 7665 5f66 6f6f  age ... fave_foo
+00000d70: 6420 e294 820a 2320 e294 8220 2d2d 2d20  d ....# ... --- 
+00000d80: 2020 e294 8620 2d2d 2d20 e294 8620 2d2d    ... --- ... --
+00000d90: 2d20 2020 2020 2020 e294 820a 2320 e294  -       ....# ..
+00000da0: 8220 7374 7220 2020 e294 8620 6936 3420  . str   ... i64 
+00000db0: e294 8620 7374 7220 2020 2020 2020 e294  ... str       ..
+00000dc0: 820a 2320 e295 9ee2 9590 e295 90e2 9590  ..# ............
+00000dd0: e295 90e2 9590 e295 90e2 9590 e295 aae2  ................
+00000de0: 9590 e295 90e2 9590 e295 90e2 9590 e295  ................
+00000df0: aae2 9590 e295 90e2 9590 e295 90e2 9590  ................
+00000e00: e295 90e2 9590 e295 90e2 9590 e295 90e2  ................
+00000e10: 9590 e295 a10a 2320 e294 8220 616d 7920  ......# ... amy 
+00000e20: 2020 e294 8620 3331 2020 e294 8620 6f72    ... 31  ... or
+00000e30: 616e 6765 7320 2020 e294 820a 2320 e294  anges   ....# ..
+00000e40: 8220 7065 7465 7220 e294 8620 3132 2020  . peter ... 12  
+00000e50: e294 8620 6368 6f63 6f6c 6174 6520 e294  ... chocolate ..
+00000e60: 820a 2320 e294 94e2 9480 e294 80e2 9480  ..# ............
+00000e70: e294 80e2 9480 e294 80e2 9480 e294 b4e2  ................
+00000e80: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00000e90: b4e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00000ea0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00000eb0: 9480 e294 980a 0a70 7269 6e74 286d 6572  .......print(mer
+00000ec0: 6765 5f6d 6f64 656c 2e75 7073 7472 6561  ge_model.upstrea
+00000ed0: 6d73 290a 2320 7b3c 7372 635f 6672 616d  ms).# {<src_fram
+00000ee0: 655f 3220 6174 2030 7831 3437 3763 3263  e_2 at 0x1477c2c
+00000ef0: 3930 3e2c 203c 7372 635f 6672 616d 655f  90>, <src_frame_
+00000f00: 3120 6174 2030 7831 3434 6630 6162 3530  1 at 0x144f0ab50
+00000f10: 3e7d 0a0a 7072 696e 7428 7372 635f 6672  >}..print(src_fr
+00000f20: 616d 655f 312e 646f 776e 7374 7265 616d  ame_1.downstream
+00000f30: 7329 0a23 207b 3c6d 6572 6765 5f6d 6f64  s).# {<merge_mod
+00000f40: 656c 2061 7420 3078 3134 3737 6332 3931  el at 0x1477c291
+00000f50: 303e 7d0a 0a70 7269 6e74 2870 6970 656c  0>}..print(pipel
+00000f60: 696e 652e 6d6f 6465 6c5f 6e61 6d65 7329  ine.model_names)
+00000f70: 0a23 205b 276d 6572 6765 5f6d 6f64 656c  .# ['merge_model
+00000f80: 272c 2027 7372 635f 6672 616d 655f 3127  ', 'src_frame_1'
+00000f90: 2c20 2773 7263 5f66 7261 6d65 5f32 275d  , 'src_frame_2']
+00000fa0: 0a0a 7072 696e 7428 6c69 7374 2870 6970  ..print(list(pip
+00000fb0: 656c 696e 652e 746f 706f 6c6f 6769 6361  eline.topologica
+00000fc0: 6c5f 736f 7274 6564 5f6e 6f64 6573 2829  l_sorted_nodes()
+00000fd0: 2929 0a23 205b 283c 7372 635f 6672 616d  )).# [(<src_fram
+00000fe0: 655f 3120 6174 2030 7831 3434 6630 6162  e_1 at 0x144f0ab
+00000ff0: 3530 3e2c 203c 7372 635f 6672 616d 655f  50>, <src_frame_
+00001000: 3220 6174 2030 7831 3437 3763 3263 3930  2 at 0x1477c2c90
+00001010: 3e29 2c20 283c 6d65 7267 655f 6d6f 6465  >), (<merge_mode
+00001020: 6c20 6174 2030 7831 3437 3763 3239 3130  l at 0x1477c2910
+00001030: 3e2c 295d 0a0a 2320 6966 2079 6f75 2068  >,)]..# if you h
+00001040: 6176 6520 7468 6520 6772 6170 6869 6e67  ave the graphing
+00001050: 206f 7074 696f 6e73 2065 6e67 6167 6564   options engaged
+00001060: 2e0a 7069 7065 6c69 6e65 2e67 7261 7068  ..pipeline.graph
+00001070: 5f70 6c74 2829 2020 2320 7769 6c6c 2064  _plt()  # will d
+00001080: 7261 7720 796f 7520 6120 6d61 7470 6c6f  raw you a matplo
+00001090: 746c 6962 206f 6620 7468 6520 4441 470a  tlib of the DAG.
+000010a0: 646f 7420 3d20 7069 7065 6c69 6e65 2e67  dot = pipeline.g
+000010b0: 7261 7068 5f64 6f74 2829 2020 2320 7769  raph_dot()  # wi
+000010c0: 6c6c 2070 726f 7669 6465 2061 2044 4f54  ll provide a DOT
+000010d0: 206c 616e 6775 6167 6520 7265 7072 6573   language repres
+000010e0: 656e 7461 7469 6f6e 206f 6620 7468 6520  entation of the 
+000010f0: 4441 470a 6060 600a 0a23 2320 4665 6174  DAG.```..## Feat
+00001100: 7572 6520 526f 6164 6d61 700a 0a54 6869  ure Roadmap..Thi
+00001110: 7320 636f 756c 6420 6368 616e 6765 2e2e  s could change..
+00001120: 2e0a 0a23 2323 2076 302e 322e 300a 0a2d  ...### v0.2.0..-
+00001130: 205b 785d 204d 6f64 656c 206c 696e 6b73   [x] Model links
+00001140: 2026 2044 4147 2069 6d70 6c65 6d65 6e74   & DAG implement
+00001150: 6564 0a2d 205b 785d 2043 6f6e 7465 7874  ed.- [x] Context
+00001160: 206c 6f67 6765 7220 6176 6169 6c61 626c   logger availabl
+00001170: 650a 2d20 5b78 5d20 4469 6167 7261 6d6d  e.- [x] Diagramm
+00001180: 696e 6720 616e 6420 7472 6163 6b69 6e67  ing and tracking
+00001190: 206f 6620 7468 6520 6d6f 6465 6c20 4441   of the model DA
+000011a0: 470a 0a23 2323 2076 302e 332e 300a 0a2d  G..### v0.3.0..-
+000011b0: 205b 205d 2043 6c65 616e 6572 2067 7261   [ ] Cleaner gra
+000011c0: 7068 2072 6573 756c 7473 0a2d 205b 205d  ph results.- [ ]
+000011d0: 204d 6572 6769 6e67 206f 6620 6d75 6c74   Merging of mult
+000011e0: 6970 6c65 2066 7261 6d65 6c69 6e6b 2070  iple framelink p
+000011f0: 6970 656c 696e 6573 2065 6e61 626c 696e  ipelines enablin
+00001200: 670a 2d20 5b20 5d20 4f72 6368 6573 7472  g.- [ ] Orchestr
+00001210: 6174 696f 6e20 7061 7373 7468 726f 7567  ation passthroug
+00001220: 6820 616e 6420 6c6f 6361 6c20 6578 6563  h and local exec
+00001230: 7574 696f 6e2e 0a2d 205b 785d 2043 6163  ution..- [x] Cac
+00001240: 6865 7320 616e 6420 6175 746f 2d70 6572  hes and auto-per
+00001250: 7369 7374 656e 6365 0a2d 205b 785d 2044  sistence.- [x] D
+00001260: 796e 616d 6963 2073 6f75 7263 696e 6720  ynamic sourcing 
+00001270: 666f 7220 6d6f 6465 6c73 0a2d 205b 205d  for models.- [ ]
+00001280: 206d 6f64 656c 206f 7665 7272 6964 6573   model overrides
+00001290: 2066 6f72 2043 4c49 2061 6e64 2070 7974   for CLI and pyt
+000012a0: 686f 6e20 7275 6e74 696d 6573 2e0a 2d20  hon runtimes..- 
+000012b0: 5b78 5d20 436c 6920 746f 2072 756e 2061  [x] Cli to run a
+000012c0: 2070 726f 6a65 6374 0a0a 2323 2320 7630   project..### v0
+000012d0: 2e34 2e30 0a0a 2d20 5b20 5d20 5351 4c20  .4.0..- [ ] SQL 
+000012e0: 6d6f 6465 6c73 2026 2064 6274 2c20 7371  models & dbt, sq
+000012f0: 6c6d 6573 6820 636f 6d70 6174 6162 696c  lmesh compatabil
+00001300: 6974 790a 2d20 5b20 5d20 4f70 656e 2054  ity.- [ ] Open T
+00001310: 7261 6369 6e67 2069 6e74 6567 7261 7469  racing integrati
+00001320: 6f6e 0a                                  on.
```

### Comparing `framelink-0.2.1/data/divy_trips_limited.csv` & `framelink-0.2.2/data/divy_trips_limited.csv`

 * *Files identical despite different names*

### Comparing `framelink-0.2.1/examples/notebooks/basic_pandas.ipynb` & `framelink-0.2.2/examples/notebooks/basic_pandas.ipynb`

 * *Files identical despite different names*

### Comparing `framelink-0.2.1/pdm.lock` & `framelink-0.2.2/pdm.lock`

 * *Files identical despite different names*

### Comparing `framelink-0.2.1/pyproject.toml` & `framelink-0.2.2/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -3,14 +3,18 @@
     { name = "Toby Devlin", email = "toby@tobydevlin.com" },
 ]
 requires-python = ">=3.8,<4.0"
 name = "framelink"
 description = ""
 readme = "README.md"
 dynamic = ["version"]
+keywords = ["data", "DAG", "orchastration", "dataframe"]
+classifiers = [
+    "Development Status :: 4 - Beta",
+]
 
 dependencies = [
     "networkx>=3.0",
     "typer[all]>=0.7.0",
 ]
 
 [project.optional-dependencies]
```

### Comparing `framelink-0.2.1/src/framelink/_cli.py` & `framelink-0.2.2/src/framelink/_cli.py`

 * *Files identical despite different names*

### Comparing `framelink-0.2.1/src/framelink/_util.py` & `framelink-0.2.2/src/framelink/_util.py`

 * *Files identical despite different names*

### Comparing `framelink-0.2.1/src/framelink/core.py` & `framelink-0.2.2/src/framelink/core.py`

 * *Files identical despite different names*

### Comparing `framelink-0.2.1/src/framelink/storage/core.py` & `framelink-0.2.2/src/framelink/storage/core.py`

 * *Files identical despite different names*

### Comparing `framelink-0.2.1/src/framelink/storage/interfaces.py` & `framelink-0.2.2/src/framelink/storage/interfaces.py`

 * *Files identical despite different names*

### Comparing `framelink-0.2.1/src/framelink.egg-info/PKG-INFO` & `framelink-0.2.2/src/framelink.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 Metadata-Version: 2.1
 Name: framelink
-Version: 0.2.1
+Version: 0.2.2
 Author-email: Toby Devlin <toby@tobydevlin.com>
 Project-URL: github, https://github.com/GitToby/framelink
+Keywords: data,DAG,orchastration,dataframe
+Classifier: Development Status :: 4 - Beta
 Requires-Python: <4.0,>=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: viz
 Provides-Extra: dev
 
-![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/gittoby/framelink/lint_test_build.yml)
-![GitHub Release Date](https://img.shields.io/github/release-date/GitToby/framelink)
+[![Version](https://img.shields.io/pypi/v/framelink)](https://pypi.org/project/framelink/)
+[![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/gittoby/framelink/lint_test_build.yml)](https://github.com/GitToby/framelink)
+[![GitHub Release Date](https://img.shields.io/github/release-date/GitToby/framelink)](https://github.com/GitToby/framelink)
+[![codecov](https://codecov.io/gh/GitToby/framelink/branch/master/graph/badge.svg?token=Uh8viFPyOG)](https://codecov.io/gh/GitToby/framelink)
+[![PyPi downloads](https://img.shields.io/pypi/dm/framelink)](https://pypi.org/project/framelink/)
 
-Framelink is a simple wrapper that will provide context into pandas, polars and other Dataframe engines. See roadmap
-below for future goals of the project.
+Framelink is a simple wrapper thats designed to provide context into pandas, polars and other Dataframe engines. See
+roadmap below for future of the project.
 
 **This project is still in prerelease, consider the API unstable. Any usage should be pinned.**
 
 ```bash
 pip install framelink
 ```
 
@@ -34,62 +39,64 @@
 ## Concepts
 
 - A **Pipeline** is a DAG of _models_ that can be executed in a particular way.
 - A **Model** is a definition of sourcing data and, potentially, a transform. It's an ETL in its most basic form.
 - A **Frame** is a result of a _model_ run.
 
 ## Features
+
 - [x] Model links & DAG + diagramming
 - [x] Context logging per model
 - [x] Diagramming and tracking of the model DAG
 - [x] Caches and auto-persistence
 - [ ] Dynamic sourcing for models
 - [x] Cli to run a project
+- [ ] Transpiler for popular DAG execution environments
 
 ## Example
 
 ```python
 from pathlib import Path
 
 import pandas as pd
 import polars as pl
 
 from framelink.core import FramelinkPipeline, FramelinkSettings
 from framelink.storage.core import PickleStorage, NoStorage
 
 settings = FramelinkSettings(
-  default_storage=PickleStorage(Path(__file__).parent / "data")
+    default_storage=PickleStorage(Path(__file__).parent / "data")
 )
 
 pipeline = FramelinkPipeline(settings=settings)
 
 
 @pipeline.model()
 def src_frame_1(_: FramelinkPipeline) -> pd.DataFrame:
-  return pd.DataFrame(data={
-    "name": ["amy", "peter"],
-    "age": [31, 12],
-  })
+    return pd.DataFrame(data={
+        "name": ["amy", "peter"],
+        "age": [31, 12],
+    })
 
 
 @pipeline.model(storage=NoStorage())
 def src_frame_2(_: FramelinkPipeline) -> pd.DataFrame:
-  return pd.DataFrame(data={
-    "name": ["amy", "peter", "helen"],
-    "fave_food": ["oranges", "chocolate", "water"],
-  })
+    return pd.DataFrame(data={
+        "name": ["amy", "peter", "helen"],
+        "fave_food": ["oranges", "chocolate", "water"],
+    })
 
 
 @pipeline.model()
 def merge_model(ctx: FramelinkPipeline) -> pl.DataFrame:
-  res_1 = ctx.ref(src_frame_1)
-  res_2 = ctx.ref(src_frame_2)
-  key = "name"
-  ctx.log.info(f"Merging both sources on {key}")
-  return pl.from_pandas(res_1).join(pl.from_pandas(res_2), on=key)
+    res_1 = ctx.ref(src_frame_1)
+    res_2 = ctx.ref(src_frame_2)
+    key = "name"
+    ctx.log.info(f"Merging both sources on {key}")
+    return pl.from_pandas(res_1).join(pl.from_pandas(res_2), on=key)
 
 
 # build with implicit context
 r_1 = pipeline.build(merge_model)
 print(r_1)
 # shape: (2, 3)
 # ┌───────┬─────┬───────────┐
```

### Comparing `framelink-0.2.1/src/framelink.egg-info/SOURCES.txt` & `framelink-0.2.2/src/framelink.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `framelink-0.2.1/tests/conftest.py` & `framelink-0.2.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `framelink-0.2.1/tests/core/test_dag.py` & `framelink-0.2.2/tests/core/test_dag.py`

 * *Files identical despite different names*

### Comparing `framelink-0.2.1/tests/core/test_logging.py` & `framelink-0.2.2/tests/core/test_logging.py`

 * *Files identical despite different names*

### Comparing `framelink-0.2.1/tests/core/test_model.py` & `framelink-0.2.2/tests/core/test_model.py`

 * *Files identical despite different names*

### Comparing `framelink-0.2.1/tests/core/test_model_parsing.py` & `framelink-0.2.2/tests/core/test_model_parsing.py`

 * *Files identical despite different names*

### Comparing `framelink-0.2.1/tests/core/test_pipeline_metas.py` & `framelink-0.2.2/tests/core/test_pipeline_metas.py`

 * *Files identical despite different names*

### Comparing `framelink-0.2.1/tests/core/test_storage.py` & `framelink-0.2.2/tests/core/test_storage.py`

 * *Files identical despite different names*

