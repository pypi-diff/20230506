# Comparing `tmp/framelink-0.2.0.tar.gz` & `tmp/framelink-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "framelink-0.2.0.tar", last modified: Fri Apr 21 02:45:32 2023, max compression
+gzip compressed data, was "framelink-0.2.1.tar", last modified: Sat May  6 05:03:59 2023, max compression
```

## Comparing `framelink-0.2.0.tar` & `framelink-0.2.1.tar`

### file list

```diff
@@ -1,42 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 02:45:32.235062 framelink-0.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 02:45:32.227062 framelink-0.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 02:45:32.227062 framelink-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-04-21 02:44:18.000000 framelink-0.2.0/.github/workflows/lint_test_build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-21 02:44:18.000000 framelink-0.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-04-21 02:44:18.000000 framelink-0.2.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-04-21 02:45:32.235062 framelink-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-04-21 02:44:18.000000 framelink-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 02:45:32.227062 framelink-0.2.0/data/
--rw-r--r--   0 runner    (1001) docker     (123)    19808 2023-04-21 02:44:18.000000 framelink-0.2.0/data/divy_trips_limited.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 02:45:32.227062 framelink-0.2.0/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 02:45:32.227062 framelink-0.2.0/examples/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)    52351 2023-04-21 02:44:18.000000 framelink-0.2.0/examples/notebooks/basic_pandas.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   336847 2023-04-21 02:44:18.000000 framelink-0.2.0/pdm.lock
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-04-21 02:44:18.000000 framelink-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 02:45:32.235062 framelink-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 02:45:32.227062 framelink-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 02:45:32.231062 framelink-0.2.0/src/framelink/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 02:44:18.000000 framelink-0.2.0/src/framelink/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-21 02:45:32.000000 framelink-0.2.0/src/framelink/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-04-21 02:44:18.000000 framelink-0.2.0/src/framelink/_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    12820 2023-04-21 02:44:18.000000 framelink-0.2.0/src/framelink/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 02:45:32.231062 framelink-0.2.0/src/framelink.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-04-21 02:45:32.000000 framelink-0.2.0/src/framelink.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-04-21 02:45:32.000000 framelink-0.2.0/src/framelink.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 02:45:32.000000 framelink-0.2.0/src/framelink.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-21 02:45:32.000000 framelink-0.2.0/src/framelink.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-21 02:45:32.000000 framelink-0.2.0/src/framelink.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 02:45:32.231062 framelink-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 02:44:18.000000 framelink-0.2.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-04-21 02:44:18.000000 framelink-0.2.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 02:45:32.235062 framelink-0.2.0/tests/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 02:44:18.000000 framelink-0.2.0/tests/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-21 02:44:18.000000 framelink-0.2.0/tests/core/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-04-21 02:44:18.000000 framelink-0.2.0/tests/core/test_dag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-04-21 02:44:18.000000 framelink-0.2.0/tests/core/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     5608 2023-04-21 02:44:18.000000 framelink-0.2.0/tests/core/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-04-21 02:44:18.000000 framelink-0.2.0/tests/core/test_model_parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-21 02:44:18.000000 framelink-0.2.0/tests/core/test_persistance.py
--rw-r--r--   0 runner    (1001) docker     (123)     3845 2023-04-21 02:44:18.000000 framelink-0.2.0/tests/core/test_pipeline_metas.py
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-04-21 02:44:18.000000 framelink-0.2.0/tests/core/test_run.py
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-21 02:44:18.000000 framelink-0.2.0/tests/readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 05:03:59.362071 framelink-0.2.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 05:03:59.350071 framelink-0.2.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 05:03:59.354071 framelink-0.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-05-06 05:02:59.000000 framelink-0.2.1/.github/workflows/lint_test_build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-06 05:02:59.000000 framelink-0.2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-06 05:02:59.000000 framelink-0.2.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4660 2023-05-06 05:03:59.358071 framelink-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-05-06 05:02:59.000000 framelink-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 05:03:59.354071 framelink-0.2.1/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    19808 2023-05-06 05:02:59.000000 framelink-0.2.1/data/divy_trips_limited.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 05:03:59.350071 framelink-0.2.1/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 05:03:59.354071 framelink-0.2.1/examples/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)    52351 2023-05-06 05:02:59.000000 framelink-0.2.1/examples/notebooks/basic_pandas.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   309258 2023-05-06 05:02:59.000000 framelink-0.2.1/pdm.lock
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-05-06 05:02:59.000000 framelink-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 05:03:59.362071 framelink-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 05:03:59.350071 framelink-0.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 05:03:59.354071 framelink-0.2.1/src/framelink/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 05:02:59.000000 framelink-0.2.1/src/framelink/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 05:02:59.000000 framelink-0.2.1/src/framelink/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-06 05:03:59.000000 framelink-0.2.1/src/framelink/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-05-06 05:02:59.000000 framelink-0.2.1/src/framelink/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-05-06 05:02:59.000000 framelink-0.2.1/src/framelink/_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12870 2023-05-06 05:02:59.000000 framelink-0.2.1/src/framelink/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 05:03:59.358071 framelink-0.2.1/src/framelink/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 05:02:59.000000 framelink-0.2.1/src/framelink/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-05-06 05:02:59.000000 framelink-0.2.1/src/framelink/storage/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-05-06 05:02:59.000000 framelink-0.2.1/src/framelink/storage/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-06 05:02:59.000000 framelink-0.2.1/src/framelink/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 05:03:59.358071 framelink-0.2.1/src/framelink.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4660 2023-05-06 05:03:59.000000 framelink-0.2.1/src/framelink.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-06 05:03:59.000000 framelink-0.2.1/src/framelink.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 05:03:59.000000 framelink-0.2.1/src/framelink.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-06 05:03:59.000000 framelink-0.2.1/src/framelink.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-06 05:03:59.000000 framelink-0.2.1/src/framelink.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-06 05:03:59.000000 framelink-0.2.1/src/framelink.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 05:03:59.358071 framelink-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 05:02:59.000000 framelink-0.2.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-06 05:02:59.000000 framelink-0.2.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 05:03:59.358071 framelink-0.2.1/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 05:02:59.000000 framelink-0.2.1/tests/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-05-06 05:02:59.000000 framelink-0.2.1/tests/core/test_dag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-05-06 05:02:59.000000 framelink-0.2.1/tests/core/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-05-06 05:02:59.000000 framelink-0.2.1/tests/core/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-06 05:02:59.000000 framelink-0.2.1/tests/core/test_model_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3845 2023-05-06 05:02:59.000000 framelink-0.2.1/tests/core/test_pipeline_metas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-06 05:02:59.000000 framelink-0.2.1/tests/core/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-05-06 05:02:59.000000 framelink-0.2.1/tests/core/test_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-06 05:02:59.000000 framelink-0.2.1/tests/readme.md
```

### Comparing `framelink-0.2.0/.github/workflows/lint_test_build.yml` & `framelink-0.2.1/.github/workflows/lint_test_build.yml`

 * *Files identical despite different names*

### Comparing `framelink-0.2.0/.pre-commit-config.yaml` & `framelink-0.2.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `framelink-0.2.0/PKG-INFO` & `framelink-0.2.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: framelink
-Version: 0.2.0
+Version: 0.2.1
 Author-email: Toby Devlin <toby@tobydevlin.com>
 Project-URL: github, https://github.com/GitToby/framelink
 Requires-Python: <4.0,>=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: viz
 Provides-Extra: dev
 
 ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/gittoby/framelink/lint_test_build.yml)
 ![GitHub Release Date](https://img.shields.io/github/release-date/GitToby/framelink)
 
-Famelink is a simple wrapper that will provide context into pandas, polars and other Dataframe engines. See roadmap
+Framelink is a simple wrapper that will provide context into pandas, polars and other Dataframe engines. See roadmap
 below for future goals of the project.
 
 **This project is still in prerelease, consider the API unstable. Any usage should be pinned.**
 
 ```bash
 pip install framelink
 ```
@@ -33,55 +33,63 @@
 
 ## Concepts
 
 - A **Pipeline** is a DAG of _models_ that can be executed in a particular way.
 - A **Model** is a definition of sourcing data and, potentially, a transform. It's an ETL in its most basic form.
 - A **Frame** is a result of a _model_ run.
 
+## Features
+- [x] Model links & DAG + diagramming
+- [x] Context logging per model
+- [x] Diagramming and tracking of the model DAG
+- [x] Caches and auto-persistence
+- [ ] Dynamic sourcing for models
+- [x] Cli to run a project
+
 ## Example
 
 ```python
-import os
 from pathlib import Path
 
 import pandas as pd
 import polars as pl
 
 from framelink.core import FramelinkPipeline, FramelinkSettings
+from framelink.storage.core import PickleStorage, NoStorage
 
 settings = FramelinkSettings(
-    persist_models_dir=Path(os.getcwd()) / "data"
+  default_storage=PickleStorage(Path(__file__).parent / "data")
 )
 
 pipeline = FramelinkPipeline(settings=settings)
 
 
 @pipeline.model()
 def src_frame_1(_: FramelinkPipeline) -> pd.DataFrame:
-    return pd.DataFrame(data={
-        "name": ["amy", "peter"],
-        "age": [31, 12],
-    })
+  return pd.DataFrame(data={
+    "name": ["amy", "peter"],
+    "age": [31, 12],
+  })
 
 
-@pipeline.model()
+@pipeline.model(storage=NoStorage())
 def src_frame_2(_: FramelinkPipeline) -> pd.DataFrame:
-    return pd.DataFrame(data={
-        "name": ["amy", "peter", "helen"],
-        "fave_food": ["oranges", "chocolate", "water"],
-    })
+  return pd.DataFrame(data={
+    "name": ["amy", "peter", "helen"],
+    "fave_food": ["oranges", "chocolate", "water"],
+  })
 
 
 @pipeline.model()
 def merge_model(ctx: FramelinkPipeline) -> pl.DataFrame:
-    res_1 = ctx.ref(src_frame_1)
-    res_2 = ctx.ref(src_frame_2)
-    key = "name"
-    ctx.log.info(f"Merging both sources on {key}")
-    return pl.from_pandas(res_1).join(pl.from_pandas(res_2), on=key)
+  res_1 = ctx.ref(src_frame_1)
+  res_2 = ctx.ref(src_frame_2)
+  key = "name"
+  ctx.log.info(f"Merging both sources on {key}")
+  return pl.from_pandas(res_1).join(pl.from_pandas(res_2), on=key)
 
 
 # build with implicit context
 r_1 = pipeline.build(merge_model)
 print(r_1)
 # shape: (2, 3)
 # ┌───────┬─────┬───────────┐
@@ -121,18 +129,16 @@
 - [x] Diagramming and tracking of the model DAG
 
 ### v0.3.0
 
 - [ ] Cleaner graph results
 - [ ] Merging of multiple framelink pipelines enabling
 - [ ] Orchestration passthrough and local execution.
+- [x] Caches and auto-persistence
+- [x] Dynamic sourcing for models
+- [ ] model overrides for CLI and python runtimes.
+- [x] Cli to run a project
 
 ### v0.4.0
 
-- [ ] Caches and auto-persistence
-- [ ] Dynamic sourcing for models
-- [ ] Cli to run a project
-
-### v0.5.0
-
 - [ ] SQL models & dbt, sqlmesh compatability
 - [ ] Open Tracing integration
```

### Comparing `framelink-0.2.0/README.md` & `framelink-0.2.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/gittoby/framelink/lint_test_build.yml)
 ![GitHub Release Date](https://img.shields.io/github/release-date/GitToby/framelink)
 
-Famelink is a simple wrapper that will provide context into pandas, polars and other Dataframe engines. See roadmap
+Framelink is a simple wrapper that will provide context into pandas, polars and other Dataframe engines. See roadmap
 below for future goals of the project.
 
 **This project is still in prerelease, consider the API unstable. Any usage should be pinned.**
 
 ```bash
 pip install framelink
 ```
@@ -23,55 +23,63 @@
 
 ## Concepts
 
 - A **Pipeline** is a DAG of _models_ that can be executed in a particular way.
 - A **Model** is a definition of sourcing data and, potentially, a transform. It's an ETL in its most basic form.
 - A **Frame** is a result of a _model_ run.
 
+## Features
+- [x] Model links & DAG + diagramming
+- [x] Context logging per model
+- [x] Diagramming and tracking of the model DAG
+- [x] Caches and auto-persistence
+- [ ] Dynamic sourcing for models
+- [x] Cli to run a project
+
 ## Example
 
 ```python
-import os
 from pathlib import Path
 
 import pandas as pd
 import polars as pl
 
 from framelink.core import FramelinkPipeline, FramelinkSettings
+from framelink.storage.core import PickleStorage, NoStorage
 
 settings = FramelinkSettings(
-    persist_models_dir=Path(os.getcwd()) / "data"
+  default_storage=PickleStorage(Path(__file__).parent / "data")
 )
 
 pipeline = FramelinkPipeline(settings=settings)
 
 
 @pipeline.model()
 def src_frame_1(_: FramelinkPipeline) -> pd.DataFrame:
-    return pd.DataFrame(data={
-        "name": ["amy", "peter"],
-        "age": [31, 12],
-    })
+  return pd.DataFrame(data={
+    "name": ["amy", "peter"],
+    "age": [31, 12],
+  })
 
 
-@pipeline.model()
+@pipeline.model(storage=NoStorage())
 def src_frame_2(_: FramelinkPipeline) -> pd.DataFrame:
-    return pd.DataFrame(data={
-        "name": ["amy", "peter", "helen"],
-        "fave_food": ["oranges", "chocolate", "water"],
-    })
+  return pd.DataFrame(data={
+    "name": ["amy", "peter", "helen"],
+    "fave_food": ["oranges", "chocolate", "water"],
+  })
 
 
 @pipeline.model()
 def merge_model(ctx: FramelinkPipeline) -> pl.DataFrame:
-    res_1 = ctx.ref(src_frame_1)
-    res_2 = ctx.ref(src_frame_2)
-    key = "name"
-    ctx.log.info(f"Merging both sources on {key}")
-    return pl.from_pandas(res_1).join(pl.from_pandas(res_2), on=key)
+  res_1 = ctx.ref(src_frame_1)
+  res_2 = ctx.ref(src_frame_2)
+  key = "name"
+  ctx.log.info(f"Merging both sources on {key}")
+  return pl.from_pandas(res_1).join(pl.from_pandas(res_2), on=key)
 
 
 # build with implicit context
 r_1 = pipeline.build(merge_model)
 print(r_1)
 # shape: (2, 3)
 # ┌───────┬─────┬───────────┐
@@ -111,18 +119,16 @@
 - [x] Diagramming and tracking of the model DAG
 
 ### v0.3.0
 
 - [ ] Cleaner graph results
 - [ ] Merging of multiple framelink pipelines enabling
 - [ ] Orchestration passthrough and local execution.
+- [x] Caches and auto-persistence
+- [x] Dynamic sourcing for models
+- [ ] model overrides for CLI and python runtimes.
+- [x] Cli to run a project
 
 ### v0.4.0
 
-- [ ] Caches and auto-persistence
-- [ ] Dynamic sourcing for models
-- [ ] Cli to run a project
-
-### v0.5.0
-
 - [ ] SQL models & dbt, sqlmesh compatability
 - [ ] Open Tracing integration
```

### Comparing `framelink-0.2.0/data/divy_trips_limited.csv` & `framelink-0.2.1/data/divy_trips_limited.csv`

 * *Files identical despite different names*

### Comparing `framelink-0.2.0/examples/notebooks/basic_pandas.ipynb` & `framelink-0.2.1/examples/notebooks/basic_pandas.ipynb`

 * *Files identical despite different names*

### Comparing `framelink-0.2.0/pdm.lock` & `framelink-0.2.1/pdm.lock`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,11 @@
 # This file is @generated by PDM.
 # It is not intended for manual editing.
 
 [[package]]
-name = "altair"
-version = "4.2.2"
-requires_python = ">=3.7"
-summary = "Altair: A declarative statistical visualization library for Python."
-dependencies = [
-    "entrypoints",
-    "jinja2",
-    "jsonschema>=3.0",
-    "numpy",
-    "pandas>=0.18",
-    "toolz",
-]
-
-[[package]]
 name = "anyio"
 version = "3.6.2"
 requires_python = ">=3.6.2"
 summary = "High level compatibility layer for multiple asynchronous event loop implementations"
 dependencies = [
     "idna>=2.8",
     "sniffio>=1.1",
@@ -73,20 +59,14 @@
 
 [[package]]
 name = "backcall"
 version = "0.2.0"
 summary = "Specifications for callback functions passed in to an API"
 
 [[package]]
-name = "backports-zoneinfo"
-version = "0.2.1"
-requires_python = ">=3.6"
-summary = "Backport of the standard library zoneinfo module"
-
-[[package]]
 name = "beautifulsoup4"
 version = "4.12.2"
 requires_python = ">=3.6.0"
 summary = "Screen-scraping library"
 dependencies = [
     "soupsieve>1.2",
 ]
@@ -113,41 +93,26 @@
 summary = "An easy safelist-based HTML-sanitizing tool."
 dependencies = [
     "six>=1.9.0",
     "webencodings",
 ]
 
 [[package]]
-name = "blinker"
-version = "1.6.1"
-requires_python = ">=3.7"
-summary = "Fast, simple object-to-object and broadcast signaling"
-dependencies = [
-    "typing-extensions>=4.2",
-]
-
-[[package]]
 name = "build"
 version = "0.10.0"
 requires_python = ">= 3.7"
 summary = "A simple, correct Python build frontend"
 dependencies = [
     "colorama; os_name == \"nt\"",
     "packaging>=19.0",
     "pyproject-hooks",
     "tomli>=1.1.0; python_version < \"3.11\"",
 ]
 
 [[package]]
-name = "cachetools"
-version = "5.3.0"
-requires_python = "~=3.7"
-summary = "Extensible memoizing collections and decorators"
-
-[[package]]
 name = "certifi"
 version = "2022.12.7"
 requires_python = ">=3.6"
 summary = "Python package for providing Mozilla's CA Bundle."
 
 [[package]]
 name = "cffi"
@@ -190,14 +155,19 @@
 requires_python = ">=3.6"
 summary = "Jupyter Python Comm implementation, for usage in ipykernel, xeus-python etc."
 dependencies = [
     "traitlets>=5.3",
 ]
 
 [[package]]
+name = "commonmark"
+version = "0.9.1"
+summary = "Python parser for the CommonMark Markdown spec"
+
+[[package]]
 name = "contourpy"
 version = "1.0.7"
 requires_python = ">=3.8"
 summary = "Python library for calculating contours of 2D quadrilateral grids"
 dependencies = [
     "numpy>=1.16",
 ]
@@ -245,20 +215,14 @@
 
 [[package]]
 name = "distlib"
 version = "0.3.6"
 summary = "Distribution utilities"
 
 [[package]]
-name = "entrypoints"
-version = "0.4"
-requires_python = ">=3.6"
-summary = "Discover and load entry points from installed packages."
-
-[[package]]
 name = "exceptiongroup"
 version = "1.1.1"
 requires_python = ">=3.7"
 summary = "Backport of PEP 654 (exception groups)"
 
 [[package]]
 name = "executing"
@@ -285,32 +249,14 @@
 [[package]]
 name = "fqdn"
 version = "1.5.1"
 requires_python = ">=2.7, !=3.0, !=3.1, !=3.2, !=3.3, !=3.4, <4"
 summary = "Validates fully-qualified domain names against RFC 1123, so that they are acceptable to modern bowsers"
 
 [[package]]
-name = "gitdb"
-version = "4.0.10"
-requires_python = ">=3.7"
-summary = "Git Object Database"
-dependencies = [
-    "smmap<6,>=3.0.1",
-]
-
-[[package]]
-name = "gitpython"
-version = "3.1.31"
-requires_python = ">=3.7"
-summary = "GitPython is a Python library used to interact with Git repositories"
-dependencies = [
-    "gitdb<5,>=4.0.1",
-]
-
-[[package]]
 name = "graphviz"
 version = "0.20.1"
 requires_python = ">=3.7"
 summary = "Simple Python interface for Graphviz"
 
 [[package]]
 name = "identify"
@@ -590,23 +536,14 @@
 [[package]]
 name = "kiwisolver"
 version = "1.4.4"
 requires_python = ">=3.7"
 summary = "A fast implementation of the Cassowary constraint solver"
 
 [[package]]
-name = "markdown-it-py"
-version = "2.2.0"
-requires_python = ">=3.7"
-summary = "Python port of markdown-it. Markdown parsing, done right!"
-dependencies = [
-    "mdurl~=0.1",
-]
-
-[[package]]
 name = "markupsafe"
 version = "2.1.2"
 requires_python = ">=3.7"
 summary = "Safely add untrusted strings to HTML/XML markup."
 
 [[package]]
 name = "matplotlib"
@@ -632,20 +569,14 @@
 requires_python = ">=3.5"
 summary = "Inline Matplotlib backend for Jupyter"
 dependencies = [
     "traitlets",
 ]
 
 [[package]]
-name = "mdurl"
-version = "0.1.2"
-requires_python = ">=3.7"
-summary = "Markdown URL utilities"
-
-[[package]]
 name = "mistune"
 version = "2.0.5"
 summary = "A sane Markdown parser with useful plugins and renderers"
 
 [[package]]
 name = "mypy"
 version = "1.2.0"
@@ -916,20 +847,14 @@
 requires_python = ">=3.7.0"
 summary = "Library for building powerful interactive command lines in Python"
 dependencies = [
     "wcwidth",
 ]
 
 [[package]]
-name = "protobuf"
-version = "3.20.3"
-requires_python = ">=3.7"
-summary = "Protocol Buffers"
-
-[[package]]
 name = "psutil"
 version = "5.9.4"
 requires_python = ">=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*"
 summary = "Cross-platform lib for process and system monitoring in Python."
 
 [[package]]
 name = "ptyprocess"
@@ -953,24 +878,14 @@
 [[package]]
 name = "pycparser"
 version = "2.21"
 requires_python = ">=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*"
 summary = "C parser in Python"
 
 [[package]]
-name = "pydeck"
-version = "0.8.0"
-requires_python = ">=3.7"
-summary = "Widget for deck.gl maps"
-dependencies = [
-    "jinja2>=2.10.1",
-    "numpy>=1.16.4",
-]
-
-[[package]]
 name = "pydot"
 version = "1.4.2"
 requires_python = ">=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*"
 summary = "Python interface to Graphviz's Dot"
 dependencies = [
     "pyparsing>=2.1.4",
 ]
@@ -983,20 +898,14 @@
 
 [[package]]
 name = "pyment"
 version = "0.3.3"
 summary = "Generate/convert automatically the docstrings from code signature"
 
 [[package]]
-name = "pympler"
-version = "1.0.1"
-requires_python = ">=3.6"
-summary = "A development tool to measure, monitor and analyze the memory behavior of Python objects."
-
-[[package]]
 name = "pyparsing"
 version = "3.0.9"
 requires_python = ">=3.6.8"
 summary = "pyparsing module - Classes and methods to define and execute parsing grammars"
 
 [[package]]
 name = "pyproject-hooks"
@@ -1054,24 +963,14 @@
 
 [[package]]
 name = "pytz"
 version = "2023.3"
 summary = "World timezone definitions, modern and historical"
 
 [[package]]
-name = "pytz-deprecation-shim"
-version = "0.1.0.post0"
-requires_python = "!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*,!=3.5.*,>=2.7"
-summary = "Shims to make deprecation of pytz easier"
-dependencies = [
-    "backports-zoneinfo; python_version >= \"3.6\" and python_version < \"3.9\"",
-    "tzdata; python_version >= \"3.6\"",
-]
-
-[[package]]
 name = "pywin32"
 version = "306"
 summary = "Python for Window Extensions"
 
 [[package]]
 name = "pywinpty"
 version = "2.0.10"
@@ -1144,36 +1043,30 @@
 name = "rfc3986-validator"
 version = "0.1.1"
 requires_python = ">=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*"
 summary = "Pure python rfc3986 validator"
 
 [[package]]
 name = "rich"
-version = "13.3.3"
-requires_python = ">=3.7.0"
+version = "12.6.0"
+requires_python = ">=3.6.3,<4.0.0"
 summary = "Render rich text, tables, progress bars, syntax highlighting, markdown and more to the terminal"
 dependencies = [
-    "markdown-it-py<3.0.0,>=2.2.0",
-    "pygments<3.0.0,>=2.13.0",
+    "commonmark<0.10.0,>=0.9.0",
+    "pygments<3.0.0,>=2.6.0",
     "typing-extensions<5.0,>=4.0.0; python_version < \"3.9\"",
 ]
 
 [[package]]
 name = "ruff"
 version = "0.0.261"
 requires_python = ">=3.7"
 summary = "An extremely fast Python linter, written in Rust."
 
 [[package]]
-name = "semver"
-version = "3.0.0"
-requires_python = ">=3.7"
-summary = "Python helper for Semantic Versioning (https://semver.org)"
-
-[[package]]
 name = "send2trash"
 version = "1.8.0"
 summary = "Send file to trash natively under Mac OS X, Windows and Linux."
 
 [[package]]
 name = "setuptools"
 version = "67.6.1"
@@ -1189,26 +1082,26 @@
     "packaging>=20.0",
     "setuptools",
     "tomli>=1.0.0; python_version < \"3.11\"",
     "typing-extensions",
 ]
 
 [[package]]
+name = "shellingham"
+version = "1.5.0.post1"
+requires_python = ">=3.7"
+summary = "Tool to Detect Surrounding Shell"
+
+[[package]]
 name = "six"
 version = "1.16.0"
 requires_python = ">=2.7, !=3.0.*, !=3.1.*, !=3.2.*"
 summary = "Python 2 and 3 compatibility utilities"
 
 [[package]]
-name = "smmap"
-version = "5.0.0"
-requires_python = ">=3.6"
-summary = "A pure Python implementation of a sliding window memory map manager"
-
-[[package]]
 name = "sniffio"
 version = "1.3.0"
 requires_python = ">=3.7"
 summary = "Sniff out which async library your code is running under"
 
 [[package]]
 name = "soupsieve"
@@ -1223,46 +1116,14 @@
 dependencies = [
     "asttokens>=2.1.0",
     "executing>=1.2.0",
     "pure-eval",
 ]
 
 [[package]]
-name = "streamlit"
-version = "1.12.0"
-requires_python = ">=3.7"
-summary = "The fastest way to build data apps in Python"
-dependencies = [
-    "altair>=3.2.0",
-    "blinker>=1.0.0",
-    "cachetools>=4.0",
-    "click>=7.0",
-    "gitpython!=3.1.19",
-    "importlib-metadata>=1.4",
-    "numpy",
-    "packaging>=14.1",
-    "pandas>=0.21.0",
-    "pillow>=6.2.0",
-    "protobuf<4,>=3.12",
-    "pyarrow>=4.0",
-    "pydeck>=0.1.dev5",
-    "pympler>=0.9",
-    "python-dateutil",
-    "requests>=2.4",
-    "rich>=10.11.0",
-    "semver",
-    "toml",
-    "tornado>=5.0",
-    "typing-extensions>=3.10.0.0",
-    "tzlocal>=1.1",
-    "validators>=0.2",
-    "watchdog; platform_system != \"Darwin\"",
-]
-
-[[package]]
 name = "terminado"
 version = "0.17.1"
 requires_python = ">=3.7"
 summary = "Tornado websocket backend for the Xterm.js Javascript terminal emulator library."
 dependencies = [
     "ptyprocess; os_name != \"nt\"",
     "pywinpty>=1.1.0; os_name == \"nt\"",
@@ -1275,105 +1136,83 @@
 requires_python = ">=3.7"
 summary = "A tiny CSS parser"
 dependencies = [
     "webencodings>=0.4",
 ]
 
 [[package]]
-name = "toml"
-version = "0.10.2"
-requires_python = ">=2.6, !=3.0.*, !=3.1.*, !=3.2.*"
-summary = "Python Library for Tom's Obvious, Minimal Language"
-
-[[package]]
 name = "tomli"
 version = "2.0.1"
 requires_python = ">=3.7"
 summary = "A lil' TOML parser"
 
 [[package]]
-name = "toolz"
-version = "0.12.0"
-requires_python = ">=3.5"
-summary = "List processing tools and functional utilities"
-
-[[package]]
 name = "tornado"
 version = "6.2"
 requires_python = ">= 3.7"
 summary = "Tornado is a Python web framework and asynchronous networking library, originally developed at FriendFeed."
 
 [[package]]
 name = "traitlets"
 version = "5.9.0"
 requires_python = ">=3.7"
 summary = "Traitlets Python configuration system"
 
 [[package]]
-name = "typing-extensions"
-version = "4.5.0"
-requires_python = ">=3.7"
-summary = "Backported and Experimental Type Hints for Python 3.7+"
+name = "typer"
+version = "0.7.0"
+requires_python = ">=3.6"
+summary = "Typer, build great CLIs. Easy to code. Based on Python type hints."
+dependencies = [
+    "click<9.0.0,>=7.1.1",
+]
 
 [[package]]
-name = "tzdata"
-version = "2023.3"
-requires_python = ">=2"
-summary = "Provider of IANA time zone data"
+name = "typer"
+version = "0.7.0"
+extras = ["all"]
+requires_python = ">=3.6"
+summary = "Typer, build great CLIs. Easy to code. Based on Python type hints."
+dependencies = [
+    "colorama<0.5.0,>=0.4.3",
+    "rich<13.0.0,>=10.11.0",
+    "shellingham<2.0.0,>=1.3.0",
+    "typer==0.7.0",
+]
 
 [[package]]
-name = "tzlocal"
-version = "4.3"
+name = "typing-extensions"
+version = "4.5.0"
 requires_python = ">=3.7"
-summary = "tzinfo object for the local timezone"
-dependencies = [
-    "backports-zoneinfo; python_version < \"3.9\"",
-    "pytz-deprecation-shim",
-    "tzdata; platform_system == \"Windows\"",
-]
+summary = "Backported and Experimental Type Hints for Python 3.7+"
 
 [[package]]
 name = "uri-template"
 version = "1.2.0"
 requires_python = ">=3.6"
 summary = "RFC 6570 URI Template Processor"
 
 [[package]]
 name = "urllib3"
 version = "1.26.15"
 requires_python = ">=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*"
 summary = "HTTP library with thread-safe connection pooling, file post, and more."
 
 [[package]]
-name = "validators"
-version = "0.20.0"
-requires_python = ">=3.4"
-summary = "Python Data Validation for Humans™."
-dependencies = [
-    "decorator>=3.4.0",
-]
-
-[[package]]
 name = "virtualenv"
 version = "20.21.0"
 requires_python = ">=3.7"
 summary = "Virtual Python Environment builder"
 dependencies = [
     "distlib<1,>=0.3.6",
     "filelock<4,>=3.4.1",
     "platformdirs<4,>=2.4",
 ]
 
 [[package]]
-name = "watchdog"
-version = "3.0.0"
-requires_python = ">=3.7"
-summary = "Filesystem events monitoring"
-
-[[package]]
 name = "wcwidth"
 version = "0.2.6"
 summary = "Measures the displayed width of unicode strings in a terminal"
 
 [[package]]
 name = "webcolors"
 version = "1.13"
@@ -1400,22 +1239,19 @@
 [[package]]
 name = "zipp"
 version = "3.15.0"
 requires_python = ">=3.7"
 summary = "Backport of pathlib-compatible object wrapper for zip files"
 
 [metadata]
-lock_version = "4.1"
-content_hash = "sha256:d3b5b0c87286dae5fc49f6752b736227d19e17612febda9879f525d6bbd9d189"
+lock_version = "4.2"
+groups = ["default", "dev", "viz"]
+content_hash = "sha256:6d9b353eec9db3436a4b6bda9ae9aeb8a2f045fb0085ef17a642da4f4d3a3b2b"
 
 [metadata.files]
-"altair 4.2.2" = [
-    {url = "https://files.pythonhosted.org/packages/18/62/47452306e84d4d2e67f9c559380aeb230f5e6ca84fafb428dd36b96a99ba/altair-4.2.2-py3-none-any.whl", hash = "sha256:8b45ebeaf8557f2d760c5c77b79f02ae12aee7c46c27c06014febab6f849bc87"},
-    {url = "https://files.pythonhosted.org/packages/ec/bf/781b607da4c1a2a7211cd570bd7e22e0accd4deaf1074c32ac7344a09339/altair-4.2.2.tar.gz", hash = "sha256:39399a267c49b30d102c10411e67ab26374156a84b1aeb9fcd15140429ba49c5"},
-]
 "anyio 3.6.2" = [
     {url = "https://files.pythonhosted.org/packages/77/2b/b4c0b7a3f3d61adb1a1e0b78f90a94e2b6162a043880704b7437ef297cad/anyio-3.6.2-py3-none-any.whl", hash = "sha256:fbbe32bd270d2a2ef3ed1c5d45041250284e31fc0a4df4a5a6071842051a51e3"},
     {url = "https://files.pythonhosted.org/packages/8b/94/6928d4345f2bc1beecbff03325cad43d320717f51ab74ab5a571324f4f5a/anyio-3.6.2.tar.gz", hash = "sha256:25ea0d673ae30af41a0c442f81cf3b38c7e79fdc7b60335a4c14e05eb0947421"},
 ]
 "appnope 0.1.3" = [
     {url = "https://files.pythonhosted.org/packages/41/4a/381783f26df413dde4c70c734163d88ca0550a1361cb74a1c68f47550619/appnope-0.1.3-py2.py3-none-any.whl", hash = "sha256:265a455292d0bd8a72453494fa24df5a11eb18373a60c7c0430889f22548605e"},
     {url = "https://files.pythonhosted.org/packages/6a/cd/355842c0db33192ac0fc822e2dcae835669ef317fe56c795fb55fcddb26f/appnope-0.1.3.tar.gz", hash = "sha256:02bd91c4de869fbb1e1c50aafc4098827a7a54ab2f39d9dcba6c9547ed920e24"},
@@ -1459,32 +1295,14 @@
     {url = "https://files.pythonhosted.org/packages/21/31/3f468da74c7de4fcf9b25591e682856389b3400b4b62f201e65f15ea3e07/attrs-22.2.0.tar.gz", hash = "sha256:c9227bfc2f01993c03f68db37d1d15c9690188323c067c641f1a35ca58185f99"},
     {url = "https://files.pythonhosted.org/packages/fb/6e/6f83bf616d2becdf333a1640f1d463fef3150e2e926b7010cb0f81c95e88/attrs-22.2.0-py3-none-any.whl", hash = "sha256:29e95c7f6778868dbd49170f98f8818f78f3dc5e0e37c0b1f474e3561b240836"},
 ]
 "backcall 0.2.0" = [
     {url = "https://files.pythonhosted.org/packages/4c/1c/ff6546b6c12603d8dd1070aa3c3d273ad4c07f5771689a7b69a550e8c951/backcall-0.2.0-py2.py3-none-any.whl", hash = "sha256:fbbce6a29f263178a1f7915c1940bde0ec2b2a967566fe1c65c1dfb7422bd255"},
     {url = "https://files.pythonhosted.org/packages/a2/40/764a663805d84deee23043e1426a9175567db89c8b3287b5c2ad9f71aa93/backcall-0.2.0.tar.gz", hash = "sha256:5cbdbf27be5e7cfadb448baf0aa95508f91f2bbc6c6437cd9cd06e2a4c215e1e"},
 ]
-"backports-zoneinfo 0.2.1" = [
-    {url = "https://files.pythonhosted.org/packages/1a/ab/3e941e3fcf1b7d3ab3d0233194d99d6a0ed6b24f8f956fc81e47edc8c079/backports.zoneinfo-0.2.1-cp38-cp38-manylinux1_x86_64.whl", hash = "sha256:7b0a64cda4145548fed9efc10322770f929b944ce5cee6c0dfe0c87bf4c0c8c9"},
-    {url = "https://files.pythonhosted.org/packages/1c/96/baaca3ad1b06d97138d42a225e4d4d27cd1586b646740f771706cd2d812c/backports.zoneinfo-0.2.1-cp37-cp37m-win32.whl", hash = "sha256:e55b384612d93be96506932a786bbcde5a2db7a9e6a4bb4bffe8b733f5b9036b"},
-    {url = "https://files.pythonhosted.org/packages/28/d5/e2f3d6a52870045afd8c37b2681c47fd0b98679cd4851e349bfd7e19cfd7/backports.zoneinfo-0.2.1-cp36-cp36m-win_amd64.whl", hash = "sha256:8439c030a11780786a2002261569bdf362264f605dfa4d65090b64b05c9f79a7"},
-    {url = "https://files.pythonhosted.org/packages/33/1c/9357061860f5d3a09e1877aa4cf7c004c55eec40a1036761144ef24d8a1d/backports.zoneinfo-0.2.1-cp36-cp36m-macosx_10_14_x86_64.whl", hash = "sha256:da6013fd84a690242c310d77ddb8441a559e9cb3d3d59ebac9aca1a57b2e18bc"},
-    {url = "https://files.pythonhosted.org/packages/4a/6d/eca004eeadcbf8bd64cc96feb9e355536147f0577420b44d80c7cac70767/backports.zoneinfo-0.2.1-cp38-cp38-macosx_10_14_x86_64.whl", hash = "sha256:8961c0f32cd0336fb8e8ead11a1f8cd99ec07145ec2931122faaac1c8f7fd987"},
-    {url = "https://files.pythonhosted.org/packages/4c/7e/ed8af95bed90eeccfb4a4fe6ec424bc7a79e1aa983e54dd1d9062d9fa20b/backports.zoneinfo-0.2.1-cp37-cp37m-manylinux1_x86_64.whl", hash = "sha256:5c144945a7752ca544b4b78c8c41544cdfaf9786f25fe5ffb10e838e19a27570"},
-    {url = "https://files.pythonhosted.org/packages/6c/99/513f2c4dd41522eefc42feb86854f6cf3b1add9c175c14d90c070775e484/backports.zoneinfo-0.2.1-cp37-cp37m-win_amd64.whl", hash = "sha256:a76b38c52400b762e48131494ba26be363491ac4f9a04c1b7e92483d169f6582"},
-    {url = "https://files.pythonhosted.org/packages/74/a1/323f86a5ca5a559d452affb879512365a0473529398bfcf2d712a40ae088/backports.zoneinfo-0.2.1-cp37-cp37m-macosx_10_14_x86_64.whl", hash = "sha256:f04e857b59d9d1ccc39ce2da1021d196e47234873820cbeaad210724b1ee28ac"},
-    {url = "https://files.pythonhosted.org/packages/78/cc/e27fd6493bbce8dbea7e6c1bc861fe3d3bc22c4f7c81f4c3befb8ff5bfaf/backports.zoneinfo-0.2.1-cp38-cp38-win_amd64.whl", hash = "sha256:4a0f800587060bf8880f954dbef70de6c11bbe59c673c3d818921f042f9954a6"},
-    {url = "https://files.pythonhosted.org/packages/ad/85/475e514c3140937cf435954f78dedea1861aeab7662d11de232bdaa90655/backports.zoneinfo-0.2.1.tar.gz", hash = "sha256:fadbfe37f74051d024037f223b8e001611eac868b5c5b06144ef4d8b799862f2"},
-    {url = "https://files.pythonhosted.org/packages/c0/34/5fdb0a3a28841d215c255be8fc60b8666257bb6632193c86fd04b63d4a31/backports.zoneinfo-0.2.1-cp38-cp38-win32.whl", hash = "sha256:1b13e654a55cd45672cb54ed12148cd33628f672548f373963b0bff67b217328"},
-    {url = "https://files.pythonhosted.org/packages/c1/8f/9b1b920a6a95652463143943fa3b8c000cb0b932ab463764a6f2a2416560/backports.zoneinfo-0.2.1-cp38-cp38-manylinux1_i686.whl", hash = "sha256:e81b76cace8eda1fca50e345242ba977f9be6ae3945af8d46326d776b4cf78d1"},
-    {url = "https://files.pythonhosted.org/packages/d1/04/8f2fed9c0cb9c88442fc8d6372cb0f5738fb05a65b45e2d371fbc8a15087/backports.zoneinfo-0.2.1-cp37-cp37m-manylinux1_i686.whl", hash = "sha256:17746bd546106fa389c51dbea67c8b7c8f0d14b5526a579ca6ccf5ed72c526cf"},
-    {url = "https://files.pythonhosted.org/packages/d4/79/249bd3c4f794741f04f1e0ff33ad3cca9b2d1f4299b73f78d0d9bc9ec8dc/backports.zoneinfo-0.2.1-cp36-cp36m-win32.whl", hash = "sha256:e8236383a20872c0cdf5a62b554b27538db7fa1bbec52429d8d106effbaeca08"},
-    {url = "https://files.pythonhosted.org/packages/ef/9a/8de8f379d5b3961a517762cc051b366de3f7d4d3a2250120e7a71e25fab4/backports.zoneinfo-0.2.1-cp36-cp36m-manylinux1_i686.whl", hash = "sha256:89a48c0d158a3cc3f654da4c2de1ceba85263fafb861b98b59040a5086259722"},
-    {url = "https://files.pythonhosted.org/packages/f9/04/33e910faffe91a5680d68a064162525779259ae5de3b0c0c5bd9c4e900e0/backports.zoneinfo-0.2.1-cp36-cp36m-manylinux1_x86_64.whl", hash = "sha256:1c5742112073a563c81f786e77514969acb58649bcdf6cdf0b4ed31a348d4546"},
-]
 "beautifulsoup4 4.12.2" = [
     {url = "https://files.pythonhosted.org/packages/57/f4/a69c20ee4f660081a7dedb1ac57f29be9378e04edfcb90c526b923d4bebc/beautifulsoup4-4.12.2-py3-none-any.whl", hash = "sha256:bd2520ca0d9d7d12694a53d44ac482d181b4ec1888909b035a3dbf40d0f57d4a"},
     {url = "https://files.pythonhosted.org/packages/af/0b/44c39cf3b18a9280950ad63a579ce395dda4c32193ee9da7ff0aed547094/beautifulsoup4-4.12.2.tar.gz", hash = "sha256:492bbc69dca35d12daac71c4db1bfff0c876c00ef4a2ffacce226d4638eb72da"},
 ]
 "black 23.3.0" = [
     {url = "https://files.pythonhosted.org/packages/06/1e/273d610249f0335afb1ddb03664a03223f4826e3d1a95170a0142cb19fb4/black-23.3.0-cp39-cp39-win_amd64.whl", hash = "sha256:6b39abdfb402002b8a7d030ccc85cf5afff64ee90fa4c5aebc531e3ad0175ddb"},
     {url = "https://files.pythonhosted.org/packages/12/4b/99c71d1cf1353edd5aff2700b8960f92e9b805c9dab72639b67dbb449d3a/black-23.3.0-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:562bd3a70495facf56814293149e51aa1be9931567474993c7942ff7d3533961"},
@@ -1512,26 +1330,18 @@
     {url = "https://files.pythonhosted.org/packages/eb/a5/17b40bfd9b607b69fa726b0b3a473d14b093dcd5191ea1a1dd664eccfee3/black-23.3.0-cp311-cp311-macosx_10_16_universal2.whl", hash = "sha256:c7ab5790333c448903c4b721b59c0d80b11fe5e9803d8703e84dcb8da56fec1b"},
     {url = "https://files.pythonhosted.org/packages/fd/5b/fc2d7922c1a6bb49458d424b5be71d251f2d0dc97be9534e35d171bdc653/black-23.3.0-cp39-cp39-macosx_10_16_universal2.whl", hash = "sha256:f0bd2f4a58d6666500542b26354978218a9babcdc972722f4bf90779524515f3"},
 ]
 "bleach 6.0.0" = [
     {url = "https://files.pythonhosted.org/packages/7e/e6/d5f220ca638f6a25557a611860482cb6e54b2d97f0332966b1b005742e1f/bleach-6.0.0.tar.gz", hash = "sha256:1a1a85c1595e07d8db14c5f09f09e6433502c51c595970edc090551f0db99414"},
     {url = "https://files.pythonhosted.org/packages/ac/e2/dfcab68c9b2e7800c8f06b85c76e5f978d05b195a958daa9b1dda54a1db6/bleach-6.0.0-py3-none-any.whl", hash = "sha256:33c16e3353dbd13028ab4799a0f89a83f113405c766e9c122df8a06f5b85b3f4"},
 ]
-"blinker 1.6.1" = [
-    {url = "https://files.pythonhosted.org/packages/a8/42/29714f0b9d6296a099d881b300ef76a04040b68ac70d73ddc18d74218ce5/blinker-1.6.1-py3-none-any.whl", hash = "sha256:8fa2dc7c28c15c8ddfd8b3a21834790984c7e4a89b336dc3f45eeb70e0c5a407"},
-    {url = "https://files.pythonhosted.org/packages/b2/83/418c03eaeed9f87eab0d5430f7e9d5248d8a7dd64d12b5ab9e5f674e7aa3/blinker-1.6.1.tar.gz", hash = "sha256:2ddfa223483ce8f24ecd2723e0e27cd4388ef19bef1d76b09a3dae93033db231"},
-]
 "build 0.10.0" = [
     {url = "https://files.pythonhosted.org/packages/58/91/17b00d5fac63d3dca605f1b8269ba3c65e98059e1fd99d00283e42a454f0/build-0.10.0-py3-none-any.whl", hash = "sha256:af266720050a66c893a6096a2f410989eeac74ff9a68ba194b3f6473e8e26171"},
     {url = "https://files.pythonhosted.org/packages/de/1c/fb62f81952f0e74c3fbf411261d1adbdd2d615c89a24b42d0fe44eb4bcf3/build-0.10.0.tar.gz", hash = "sha256:d5b71264afdb5951d6704482aac78de887c80691c52b88a9ad195983ca2c9269"},
 ]
-"cachetools 5.3.0" = [
-    {url = "https://files.pythonhosted.org/packages/4d/91/5837e9f9e77342bb4f3ffac19ba216eef2cd9b77d67456af420e7bafe51d/cachetools-5.3.0.tar.gz", hash = "sha256:13dfddc7b8df938c21a940dfa6557ce6e94a2f1cdfa58eb90c805721d58f2c14"},
-    {url = "https://files.pythonhosted.org/packages/db/14/2b48a834d349eee94677e8702ea2ef98b7c674b090153ea8d3f6a788584e/cachetools-5.3.0-py3-none-any.whl", hash = "sha256:429e1a1e845c008ea6c85aa35d4b98b65d6a9763eeef3e37e92728a12d1de9d4"},
-]
 "certifi 2022.12.7" = [
     {url = "https://files.pythonhosted.org/packages/37/f7/2b1b0ec44fdc30a3d31dfebe52226be9ddc40cd6c0f34ffc8923ba423b69/certifi-2022.12.7.tar.gz", hash = "sha256:35824b4c3a97115964b408844d64aa14db1cc518f6562e8d7261699d1350a9e3"},
     {url = "https://files.pythonhosted.org/packages/71/4c/3db2b8021bd6f2f0ceb0e088d6b2d49147671f25832fb17970e9b583d742/certifi-2022.12.7-py3-none-any.whl", hash = "sha256:4ad3232f5e926d6718ec31cfc1fcadfde020920e278684144551c91769c7bc18"},
 ]
 "cffi 1.15.1" = [
     {url = "https://files.pythonhosted.org/packages/00/05/23a265a3db411b0bfb721bf7a116c7cecaf3eb37ebd48a6ea4dfb0a3244d/cffi-1.15.1-cp27-cp27m-win_amd64.whl", hash = "sha256:e00b098126fd45523dd056d2efba6c5a63b71ffe9f2bbe1a4fe1716e1d0c331e"},
     {url = "https://files.pythonhosted.org/packages/03/7b/259d6e01a6083acef9d3c8c88990c97d313632bb28fa84d6ab2bb201140a/cffi-1.15.1-cp36-cp36m-manylinux_2_5_i686.manylinux1_i686.whl", hash = "sha256:173379135477dc8cac4bc58f45db08ab45d228b3363adb7af79436135d028405"},
@@ -1687,14 +1497,18 @@
     {url = "https://files.pythonhosted.org/packages/d1/d6/3965ed04c63042e047cb6a3e6ed1a63a35087b6a609aa3a15ed8ac56c221/colorama-0.4.6-py2.py3-none-any.whl", hash = "sha256:4f1d9991f5acc0ca119f9d443620b77f9d6b33703e51011c16baf57afb285fc6"},
     {url = "https://files.pythonhosted.org/packages/d8/53/6f443c9a4a8358a93a6792e2acffb9d9d5cb0a5cfd8802644b7b1c9a02e4/colorama-0.4.6.tar.gz", hash = "sha256:08695f5cb7ed6e0531a20572697297273c47b8cae5a63ffc6d6ed5c201be6e44"},
 ]
 "comm 0.1.3" = [
     {url = "https://files.pythonhosted.org/packages/74/f3/b88d7e1dadf741550c56b70d7ce62673354fddb68e143d193ceb80224208/comm-0.1.3-py3-none-any.whl", hash = "sha256:16613c6211e20223f215fc6d3b266a247b6e2641bf4e0a3ad34cb1aff2aa3f37"},
     {url = "https://files.pythonhosted.org/packages/d6/1a/9937a10f8fd6d9f0f72fa0ab520cec7e50c534b215f8fd2d28e0f0a7f9a7/comm-0.1.3.tar.gz", hash = "sha256:a61efa9daffcfbe66fd643ba966f846a624e4e6d6767eda9cf6e993aadaab93e"},
 ]
+"commonmark 0.9.1" = [
+    {url = "https://files.pythonhosted.org/packages/60/48/a60f593447e8f0894ebb7f6e6c1f25dafc5e89c5879fdc9360ae93ff83f0/commonmark-0.9.1.tar.gz", hash = "sha256:452f9dc859be7f06631ddcb328b6919c67984aca654e5fefb3914d54691aed60"},
+    {url = "https://files.pythonhosted.org/packages/b1/92/dfd892312d822f36c55366118b95d914e5f16de11044a27cf10a7d71bbbf/commonmark-0.9.1-py2.py3-none-any.whl", hash = "sha256:da2f38c92590f83de410ba1a3cbceafbc74fee9def35f9251ba9a971d6d66fd9"},
+]
 "contourpy 1.0.7" = [
     {url = "https://files.pythonhosted.org/packages/02/4d/009c25f6a3f27dab8fabd5e0f9eeb2bc2697bfcf533e9d07ee825d7fae22/contourpy-1.0.7-cp310-cp310-manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:f99e9486bf1bb979d95d5cffed40689cb595abb2b841f2991fc894b3452290e8"},
     {url = "https://files.pythonhosted.org/packages/03/a4/0119e530f7926377d283ed742b120ef5cf3f37f7c5aef5e77cfc59ebabfc/contourpy-1.0.7-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:130230b7e49825c98edf0b428b7aa1125503d91732735ef897786fe5452b1ec2"},
     {url = "https://files.pythonhosted.org/packages/08/ce/9bfe9f028cb5a8ee97898da52f4905e0e2d9ca8203ffdcdbe80e1769b549/contourpy-1.0.7-cp38-cp38-win_amd64.whl", hash = "sha256:57119b0116e3f408acbdccf9eb6ef19d7fe7baf0d1e9aaa5381489bc1aa56556"},
     {url = "https://files.pythonhosted.org/packages/09/c4/72ffdbea5f0f2a89e544b5e91793548488b892855c170f89f4b2d8d0597e/contourpy-1.0.7-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:a9d7587d2fdc820cc9177139b56795c39fb8560f540bba9ceea215f1f66e1566"},
     {url = "https://files.pythonhosted.org/packages/17/22/ae833bbd6ec6dc4b2134d095332dc9853d8ab81c9ced3ec18f1db1942134/contourpy-1.0.7-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:5dd34c1ae752515318224cba7fc62b53130c45ac6a1040c8b7c1a223c46e8967"},
     {url = "https://files.pythonhosted.org/packages/26/df/b5c53b350d9f8c8672fa96a756c12445854be430469a92ca081dfc0f3585/contourpy-1.0.7-cp38-cp38-musllinux_1_1_i686.whl", hash = "sha256:b8d587cc39057d0afd4166083d289bdeff221ac6d3ee5046aef2d480dc4b503c"},
@@ -1833,18 +1647,14 @@
     {url = "https://files.pythonhosted.org/packages/07/6c/aa3f2f849e01cb6a001cd8554a88d4c77c5c1a31c95bdf1cf9301e6d9ef4/defusedxml-0.7.1-py2.py3-none-any.whl", hash = "sha256:a352e7e428770286cc899e2542b6cdaedb2b4953ff269a210103ec58f6198a61"},
     {url = "https://files.pythonhosted.org/packages/0f/d5/c66da9b79e5bdb124974bfe172b4daf3c984ebd9c2a06e2b8a4dc7331c72/defusedxml-0.7.1.tar.gz", hash = "sha256:1bb3032db185915b62d7c6209c5a8792be6a32ab2fedacc84e01b52c51aa3e69"},
 ]
 "distlib 0.3.6" = [
     {url = "https://files.pythonhosted.org/packages/58/07/815476ae605bcc5f95c87a62b95e74a1bce0878bc7a3119bc2bf4178f175/distlib-0.3.6.tar.gz", hash = "sha256:14bad2d9b04d3a36127ac97f30b12a19268f211063d8f8ee4f47108896e11b46"},
     {url = "https://files.pythonhosted.org/packages/76/cb/6bbd2b10170ed991cf64e8c8b85e01f2fb38f95d1bc77617569e0b0b26ac/distlib-0.3.6-py2.py3-none-any.whl", hash = "sha256:f35c4b692542ca110de7ef0bea44d73981caeb34ca0b9b6b2e6d7790dda8f80e"},
 ]
-"entrypoints 0.4" = [
-    {url = "https://files.pythonhosted.org/packages/35/a8/365059bbcd4572cbc41de17fd5b682be5868b218c3c5479071865cab9078/entrypoints-0.4-py3-none-any.whl", hash = "sha256:f174b5ff827504fd3cd97cc3f8649f3693f51538c7e4bdf3ef002c8429d42f9f"},
-    {url = "https://files.pythonhosted.org/packages/ea/8d/a7121ffe5f402dc015277d2d31eb82d2187334503a011c18f2e78ecbb9b2/entrypoints-0.4.tar.gz", hash = "sha256:b706eddaa9218a19ebcd67b56818f05bb27589b1ca9e8d797b74affad4ccacd4"},
-]
 "exceptiongroup 1.1.1" = [
     {url = "https://files.pythonhosted.org/packages/61/97/17ed81b7a8d24d8f69b62c0db37abbd8c0042d4b3fc429c73dab986e7483/exceptiongroup-1.1.1-py3-none-any.whl", hash = "sha256:232c37c63e4f682982c8b6459f33a8981039e5fb8756b2074364e5055c498c9e"},
     {url = "https://files.pythonhosted.org/packages/cc/38/57f14ddc8e8baeddd8993a36fe57ce7b4ba174c35048b9a6d270bb01e833/exceptiongroup-1.1.1.tar.gz", hash = "sha256:d484c3090ba2889ae2928419117447a14daf3c1231d5e30d0aae34f354f01785"},
 ]
 "executing 1.2.0" = [
     {url = "https://files.pythonhosted.org/packages/28/3c/bc3819dd8b1a1588c9215a87271b6178cc5498acaa83885211f5d4d9e693/executing-1.2.0-py2.py3-none-any.whl", hash = "sha256:0314a69e37426e3608aada02473b4161d4caf5a4b244d1d0c48072b8fee7bacc"},
     {url = "https://files.pythonhosted.org/packages/8f/ac/89ff37d8594b0eef176b7cec742ac868fef853b8e18df0309e3def9f480b/executing-1.2.0.tar.gz", hash = "sha256:19da64c18d2d851112f09c287f8d3dbbdf725ab0e569077efb6cdcbd3497c107"},
@@ -1861,22 +1671,14 @@
     {url = "https://files.pythonhosted.org/packages/16/07/1c7547e27f559ec078801d522cc4d5127cdd4ef8e831c8ddcd9584668a07/fonttools-4.39.3-py3-none-any.whl", hash = "sha256:64c0c05c337f826183637570ac5ab49ee220eec66cf50248e8df527edfa95aeb"},
     {url = "https://files.pythonhosted.org/packages/39/d7/ab05ae34dd57dd657e492d95ce7ec6bfebfb3bfcdc7316660ac5a13fcfee/fonttools-4.39.3.zip", hash = "sha256:9234b9f57b74e31b192c3fc32ef1a40750a8fbc1cd9837a7b7bfc4ca4a5c51d7"},
 ]
 "fqdn 1.5.1" = [
     {url = "https://files.pythonhosted.org/packages/30/3e/a80a8c077fd798951169626cde3e239adeba7dab75deb3555716415bd9b0/fqdn-1.5.1.tar.gz", hash = "sha256:105ed3677e767fb5ca086a0c1f4bb66ebc3c100be518f0e0d755d9eae164d89f"},
     {url = "https://files.pythonhosted.org/packages/cf/58/8acf1b3e91c58313ce5cb67df61001fc9dcd21be4fadb76c1a2d540e09ed/fqdn-1.5.1-py3-none-any.whl", hash = "sha256:3a179af3761e4df6eb2e026ff9e1a3033d3587bf980a0b1b2e1e5d08d7358014"},
 ]
-"gitdb 4.0.10" = [
-    {url = "https://files.pythonhosted.org/packages/21/a6/35f83efec687615c711fe0a09b67e58f6d1254db27b1013119de46f450bd/gitdb-4.0.10-py3-none-any.whl", hash = "sha256:c286cf298426064079ed96a9e4a9d39e7f3e9bf15ba60701e95f5492f28415c7"},
-    {url = "https://files.pythonhosted.org/packages/4b/47/dc98f3d5d48aa815770e31490893b92c5f1cd6c6cf28dd3a8ae0efffac14/gitdb-4.0.10.tar.gz", hash = "sha256:6eb990b69df4e15bad899ea868dc46572c3f75339735663b81de79b06f17eb9a"},
-]
-"gitpython 3.1.31" = [
-    {url = "https://files.pythonhosted.org/packages/5f/11/2b0f60686dbda49028cec8c66bd18a5e82c96d92eef4bc34961e35bb3762/GitPython-3.1.31.tar.gz", hash = "sha256:8ce3bcf69adfdf7c7d503e78fd3b1c492af782d58893b650adb2ac8912ddd573"},
-    {url = "https://files.pythonhosted.org/packages/9e/8a/d1e02cc111d65b0346f70abb83c51f8593e7134bf694a4a56d1a470caaf7/GitPython-3.1.31-py3-none-any.whl", hash = "sha256:f04893614f6aa713a60cbbe1e6a97403ef633103cdd0ef5eb6efe0deb98dbe8d"},
-]
 "graphviz 0.20.1" = [
     {url = "https://files.pythonhosted.org/packages/a5/90/fb047ce95c1eadde6ae78b3fca6a598b4c307277d4f8175d12b18b8f7321/graphviz-0.20.1.zip", hash = "sha256:8c58f14adaa3b947daf26c19bc1e98c4e0702cdc31cf99153e6f06904d492bf8"},
     {url = "https://files.pythonhosted.org/packages/de/5e/fcbb22c68208d39edff467809d06c9d81d7d27426460ebc598e55130c1aa/graphviz-0.20.1-py3-none-any.whl", hash = "sha256:587c58a223b51611c0cf461132da386edd896a029524ca61a1462b880bf97977"},
 ]
 "identify 2.5.22" = [
     {url = "https://files.pythonhosted.org/packages/9c/85/2dad5866648c6b1772d5cb9b0ca1810f214e5d5e72f231dfb6891300358a/identify-2.5.22.tar.gz", hash = "sha256:f7a93d6cf98e29bd07663c60728e7a4057615068d7a639d132dc883b2d54d31e"},
     {url = "https://files.pythonhosted.org/packages/f0/be/8879e140d456886b377b27294671f527004b161bbd43da43a726a6d032c1/identify-2.5.22-py2.py3-none-any.whl", hash = "sha256:f0faad595a4687053669c112004178149f6c326db71ee999ae4636685753ad2f"},
@@ -2036,18 +1838,14 @@
     {url = "https://files.pythonhosted.org/packages/eb/db/b7ebaa2d35f9fb55f3ff8328b5e9dc049f6524dca737cea13e6235ab191d/kiwisolver-1.4.4-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:10ee06759482c78bdb864f4109886dff7b8a56529bc1609d4f1112b93fe6423c"},
     {url = "https://files.pythonhosted.org/packages/ed/bf/7994af5c838c761b4998044dfabecce8c9f428479e32fe77edc7336dcfd2/kiwisolver-1.4.4-cp311-cp311-macosx_10_9_universal2.whl", hash = "sha256:e0ea21f66820452a3f5d1655f8704a60d66ba1191359b96541eaf457710a5fc6"},
     {url = "https://files.pythonhosted.org/packages/ee/c2/99b2d61dc246844498e68571c589e37ed7a866a4914cb2da2d66d141b596/kiwisolver-1.4.4-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:c79ebe8f3676a4c6630fd3f777f3cfecf9289666c84e775a67d1d358578dc2e3"},
     {url = "https://files.pythonhosted.org/packages/f2/e2/7ed98290955aa83598d0e5672d88bbc193192cdcd23d3a9ed7e536cf8e55/kiwisolver-1.4.4-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:f0a71d85ecdd570ded8ac3d1c0f480842f49a40beb423bb8014539a9f32a5897"},
     {url = "https://files.pythonhosted.org/packages/f6/e8/194a4b4eee0990a648711bfb769a7110d10fd8d8b370a0464cb3d1060381/kiwisolver-1.4.4-pp38-pypy38_pp73-win_amd64.whl", hash = "sha256:70e7c2e7b750585569564e2e5ca9845acfaa5da56ac46df68414f29fea97be9f"},
     {url = "https://files.pythonhosted.org/packages/f8/f4/724d454e95c7e9be6a05f1da3fb85251b5dbb8c3b7d06bdc61d56b16035a/kiwisolver-1.4.4-pp39-pypy39_pp73-win_amd64.whl", hash = "sha256:36dafec3d6d6088d34e2de6b85f9d8e2324eb734162fba59d2ba9ed7a2043d5b"},
 ]
-"markdown-it-py 2.2.0" = [
-    {url = "https://files.pythonhosted.org/packages/bf/25/2d88e8feee8e055d015343f9b86e370a1ccbec546f2865c98397aaef24af/markdown_it_py-2.2.0-py3-none-any.whl", hash = "sha256:5a35f8d1870171d9acc47b99612dc146129b631baf04970128b568f190d0cc30"},
-    {url = "https://files.pythonhosted.org/packages/e4/c0/59bd6d0571986f72899288a95d9d6178d0eebd70b6650f1bb3f0da90f8f7/markdown-it-py-2.2.0.tar.gz", hash = "sha256:7c9a5e412688bc771c67432cbfebcdd686c93ce6484913dccf06cb5a0bea35a1"},
-]
 "markupsafe 2.1.2" = [
     {url = "https://files.pythonhosted.org/packages/02/2c/18d55e5df6a9ea33709d6c33e08cb2e07d39e20ad05d8c6fbf9c9bcafd54/MarkupSafe-2.1.2-cp310-cp310-win_amd64.whl", hash = "sha256:835fb5e38fd89328e9c81067fd642b3593c33e1e17e2fdbf77f5676abb14a156"},
     {url = "https://files.pythonhosted.org/packages/04/cf/9464c3c41b7cdb8df660cda75676697e7fb49ce1be7691a1162fc88da078/MarkupSafe-2.1.2-cp311-cp311-musllinux_1_1_i686.whl", hash = "sha256:085fd3201e7b12809f9e6e9bc1e5c96a368c8523fad5afb02afe3c051ae4afcc"},
     {url = "https://files.pythonhosted.org/packages/06/3b/d026c21cd1dbee89f41127e93113dcf5fa85c6660d108847760b59b3a66d/MarkupSafe-2.1.2-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:40dfd3fefbef579ee058f139733ac336312663c6706d1163b82b3003fb1925c4"},
     {url = "https://files.pythonhosted.org/packages/0a/88/78cb3d95afebd183d8b04442685ab4c70cfc1138b850ba20e2a07aff2f53/MarkupSafe-2.1.2-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:65608c35bfb8a76763f37036547f7adfd09270fbdbf96608be2bead319728fcd"},
     {url = "https://files.pythonhosted.org/packages/0d/15/82b108c697bec4c26c00aed6975b778cf0eac6cbb77598862b10550b7fcc/MarkupSafe-2.1.2-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:2298c859cfc5463f1b64bd55cb3e602528db6fa0f3cfd568d3605c50678f8f03"},
     {url = "https://files.pythonhosted.org/packages/19/00/3b8eb0093c885576a1ce7f2263e7b8c01e55b9977433f8246f57cd81b0be/MarkupSafe-2.1.2-cp311-cp311-win32.whl", hash = "sha256:7df70907e00c970c60b9ef2938d894a9381f38e6b9db73c5be35e59d92e06625"},
@@ -2139,18 +1937,14 @@
     {url = "https://files.pythonhosted.org/packages/f3/99/7010ae81984908cc655b7d24145aeed2784614957ed7f0cb5a72b17a63d3/matplotlib-3.7.1-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:46a561d23b91f30bccfd25429c3c706afe7d73a5cc64ef2dfaf2b2ac47c1a5dc"},
     {url = "https://files.pythonhosted.org/packages/fb/8c/391e3c105edb7e193bb163ed48988135228d0b5ce3143e1cbec2350e23c8/matplotlib-3.7.1-cp311-cp311-win_amd64.whl", hash = "sha256:c0bd19c72ae53e6ab979f0ac6a3fafceb02d2ecafa023c5cca47acd934d10be7"},
 ]
 "matplotlib-inline 0.1.6" = [
     {url = "https://files.pythonhosted.org/packages/d9/50/3af8c0362f26108e54d58c7f38784a3bdae6b9a450bab48ee8482d737f44/matplotlib-inline-0.1.6.tar.gz", hash = "sha256:f887e5f10ba98e8d2b150ddcf4702c1e5f8b3a20005eb0f74bfdbd360ee6f304"},
     {url = "https://files.pythonhosted.org/packages/f2/51/c34d7a1d528efaae3d8ddb18ef45a41f284eacf9e514523b191b7d0872cc/matplotlib_inline-0.1.6-py3-none-any.whl", hash = "sha256:f1f41aab5328aa5aaea9b16d083b128102f8712542f819fe7e6a420ff581b311"},
 ]
-"mdurl 0.1.2" = [
-    {url = "https://files.pythonhosted.org/packages/b3/38/89ba8ad64ae25be8de66a6d463314cf1eb366222074cfda9ee839c56a4b4/mdurl-0.1.2-py3-none-any.whl", hash = "sha256:84008a41e51615a49fc9966191ff91509e3c40b939176e643fd50a5c2196b8f8"},
-    {url = "https://files.pythonhosted.org/packages/d6/54/cfe61301667036ec958cb99bd3efefba235e65cdeb9c84d24a8293ba1d90/mdurl-0.1.2.tar.gz", hash = "sha256:bb413d29f5eea38f31dd4754dd7377d4465116fb207585f97bf925588687c1ba"},
-]
 "mistune 2.0.5" = [
     {url = "https://files.pythonhosted.org/packages/9f/e5/780d22d19543f339aad583304f58002975b586757aa590cbe7bea5cc6f13/mistune-2.0.5-py2.py3-none-any.whl", hash = "sha256:bad7f5d431886fcbaf5f758118ecff70d31f75231b34024a1341120340a65ce8"},
     {url = "https://files.pythonhosted.org/packages/fb/6b/d8013058fcdb0088b4130164fc961e15c50d30302f60a349c16bdfda9770/mistune-2.0.5.tar.gz", hash = "sha256:0246113cb2492db875c6be56974a7c893333bf26cd92891c85f63151cee09d34"},
 ]
 "mypy 1.2.0" = [
     {url = "https://files.pythonhosted.org/packages/17/81/62fb78abb9ae22a5eabf9d5b81b6b7ba89d65b9b190e10c685e4367183eb/mypy-1.2.0-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:fe91be1c51c90e2afe6827601ca14353bbf3953f343c2129fa1e247d55fd95ba"},
     {url = "https://files.pythonhosted.org/packages/1d/1a/8166959cf10a56218cf7a8eabd23d101050e38159ffee1868dd3e3a90ab1/mypy-1.2.0-cp39-cp39-win_amd64.whl", hash = "sha256:2de7babe398cb7a85ac7f1fd5c42f396c215ab3eff731b4d761d68d0f6a80f48"},
@@ -2402,38 +2196,14 @@
     {url = "https://files.pythonhosted.org/packages/5b/8e/6a546e439b4366ab9eab0a736876eb1e1916dd93b4a1fa560ef711d24f8c/prometheus_client-0.16.0-py3-none-any.whl", hash = "sha256:0836af6eb2c8f4fed712b2f279f6c0a8bbab29f9f4aa15276b91c7cb0d1616ab"},
     {url = "https://files.pythonhosted.org/packages/d0/55/9e34c73e1e490b105b4cd13d08497b1f7cb086a260e4161b7b7c2928b196/prometheus_client-0.16.0.tar.gz", hash = "sha256:a03e35b359f14dd1630898543e2120addfdeacd1a6069c1367ae90fd93ad3f48"},
 ]
 "prompt-toolkit 3.0.38" = [
     {url = "https://files.pythonhosted.org/packages/4b/bb/75cdcd356f57d17b295aba121494c2333d26bfff1a837e6199b8b83c415a/prompt_toolkit-3.0.38.tar.gz", hash = "sha256:23ac5d50538a9a38c8bde05fecb47d0b403ecd0662857a86f886f798563d5b9b"},
     {url = "https://files.pythonhosted.org/packages/87/3f/1f5a0ff475ae6481f4b0d45d4d911824d3218b94ee2a97a8cb84e5569836/prompt_toolkit-3.0.38-py3-none-any.whl", hash = "sha256:45ea77a2f7c60418850331366c81cf6b5b9cf4c7fd34616f733c5427e6abbb1f"},
 ]
-"protobuf 3.20.3" = [
-    {url = "https://files.pythonhosted.org/packages/00/e7/d23c439c55c90ae2e52184363162f7079ca3e7d86205b411d4e9dc266f81/protobuf-3.20.3-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:398a9e0c3eaceb34ec1aee71894ca3299605fa8e761544934378bbc6c97de23b"},
-    {url = "https://files.pythonhosted.org/packages/11/a5/e52b731415ad6ef3d841e9e6e337a690249e800cc7c06f0749afab26348c/protobuf-3.20.3-cp39-cp39-win_amd64.whl", hash = "sha256:03038ac1cfbc41aa21f6afcbcd357281d7521b4157926f30ebecc8d4ea59dcb7"},
-    {url = "https://files.pythonhosted.org/packages/28/55/b80e8567ec327c060fa39b242392e25690c8899c489ecd7bb65b46b7bb55/protobuf-3.20.3-cp310-cp310-manylinux2014_aarch64.whl", hash = "sha256:f4bd856d702e5b0d96a00ec6b307b0f51c1982c2bf9c0052cf9019e9a544ba99"},
-    {url = "https://files.pythonhosted.org/packages/2a/7c/e7091f0eea6eec70547d28c6c0d8c7335ee58f6b13456608beec8c94a62a/protobuf-3.20.3-cp37-cp37m-manylinux2014_aarch64.whl", hash = "sha256:d9e4432ff660d67d775c66ac42a67cf2453c27cb4d738fc22cb53b5d84c135d4"},
-    {url = "https://files.pythonhosted.org/packages/31/be/80a9c6f16dfa4d41be3edbe655349778ae30882407fa8275eb46b4d34854/protobuf-3.20.3-cp310-cp310-manylinux_2_12_x86_64.manylinux2010_x86_64.whl", hash = "sha256:9aae4406ea63d825636cc11ffb34ad3379335803216ee3a856787bcf5ccc751e"},
-    {url = "https://files.pythonhosted.org/packages/32/f8/52f598bceb16fe365f4ef8e957ac8890aeb56abf97d365ff5abd8c1250cf/protobuf-3.20.3-cp38-cp38-win_amd64.whl", hash = "sha256:447d43819997825d4e71bf5769d869b968ce96848b6479397e29fc24c4a5dfe9"},
-    {url = "https://files.pythonhosted.org/packages/36/8b/433071fed0058322090a55021bdc8da76d16c7bc9823f5795797803dd6d0/protobuf-3.20.3-cp39-cp39-win32.whl", hash = "sha256:819559cafa1a373b7096a482b504ae8a857c89593cf3a25af743ac9ecbd23480"},
-    {url = "https://files.pythonhosted.org/packages/3c/14/16ef7da61d30a519d84e6841d096fe446c4d8a2c39b083b0376b4785f1f3/protobuf-3.20.3-cp38-cp38-win32.whl", hash = "sha256:c02ce36ec760252242a33967d51c289fd0e1c0e6e5cc9397e2279177716add86"},
-    {url = "https://files.pythonhosted.org/packages/4c/12/62e1d5505c172e1a7f803d83b0b1693f7952c3c271eb2f155703012ae67a/protobuf-3.20.3-cp37-cp37m-manylinux_2_5_x86_64.manylinux1_x86_64.whl", hash = "sha256:74480f79a023f90dc6e18febbf7b8bac7508420f2006fabd512013c0c238f454"},
-    {url = "https://files.pythonhosted.org/packages/55/5b/e3d951e34f8356e5feecacd12a8e3b258a1da6d9a03ad1770f28925f29bc/protobuf-3.20.3.tar.gz", hash = "sha256:2e3427429c9cffebf259491be0af70189607f365c2f41c7c3764af6f337105f2"},
-    {url = "https://files.pythonhosted.org/packages/6f/5e/fc6feb366b0a9f28e0a2de3b062667c521cd9517d4ff55077b8f351ba2f3/protobuf-3.20.3-cp310-cp310-win_amd64.whl", hash = "sha256:67a3598f0a2dcbc58d02dd1928544e7d88f764b47d4a286202913f0b2801c2e7"},
-    {url = "https://files.pythonhosted.org/packages/8d/14/619e24a4c70df2901e1f4dbc50a6291eb63a759172558df326347dce1f0d/protobuf-3.20.3-py2.py3-none-any.whl", hash = "sha256:a7ca6d488aa8ff7f329d4c545b2dbad8ac31464f1d8b1c87ad1346717731e4db"},
-    {url = "https://files.pythonhosted.org/packages/98/07/4c75a689fa173c12b92c9a64a82efad44797b9b2b784c8562f36ab28b551/protobuf-3.20.3-cp37-cp37m-win_amd64.whl", hash = "sha256:8c0c984a1b8fef4086329ff8dd19ac77576b384079247c770f29cc8ce3afa06c"},
-    {url = "https://files.pythonhosted.org/packages/99/25/5825472ecd911f4ac2ac4e9ab039a48b6d03874e2add92fb633e080bf3eb/protobuf-3.20.3-cp39-cp39-manylinux2014_aarch64.whl", hash = "sha256:bf01b5720be110540be4286e791db73f84a2b721072a3711efff6c324cdf074b"},
-    {url = "https://files.pythonhosted.org/packages/9c/d8/dc6a9ee6ec43a1001e3d71cccda70cf50ac0098000fc455023dba3b46ebf/protobuf-3.20.3-cp36-cp36m-manylinux_2_5_x86_64.manylinux1_x86_64.whl", hash = "sha256:899dc660cd599d7352d6f10d83c95df430a38b410c1b66b407a6b29265d66469"},
-    {url = "https://files.pythonhosted.org/packages/9f/1a/6848ed1669a6c70bf947d25d64ce6dcc65ccec06e917072df516944fa17e/protobuf-3.20.3-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:de78575669dddf6099a8a0f46a27e82a1783c557ccc38ee620ed8cc96d3be7d7"},
-    {url = "https://files.pythonhosted.org/packages/b5/b6/ec87636b9381137f17292851461902ceac7632a00476c2afbcd864ed5447/protobuf-3.20.3-cp38-cp38-manylinux2014_aarch64.whl", hash = "sha256:f4c42102bc82a51108e449cbb32b19b180022941c727bac0cfd50170341f16ee"},
-    {url = "https://files.pythonhosted.org/packages/c7/df/ec3ecb8c940b36121c7b77c10acebf3d1c736498aa2f1fe3b6231ee44e76/protobuf-3.20.3-cp39-cp39-manylinux_2_5_x86_64.manylinux1_x86_64.whl", hash = "sha256:daa564862dd0d39c00f8086f88700fdbe8bc717e993a21e90711acfed02f2402"},
-    {url = "https://files.pythonhosted.org/packages/da/e4/4d62585593e9f962cb02614534f62f930de6a80a0a3784282094a01919b2/protobuf-3.20.3-cp38-cp38-manylinux_2_5_x86_64.manylinux1_x86_64.whl", hash = "sha256:44246bab5dd4b7fbd3c0c80b6f16686808fab0e4aca819ade6e8d294a29c7050"},
-    {url = "https://files.pythonhosted.org/packages/db/96/948d3fcc1fa816e7ae1d27af59b9d8c5c5e582f3994fd14394f31da95b99/protobuf-3.20.3-cp310-cp310-win32.whl", hash = "sha256:28545383d61f55b57cf4df63eebd9827754fd2dc25f80c5253f9184235db242c"},
-    {url = "https://files.pythonhosted.org/packages/ef/d4/765a106ca96d487f94f3c99e46b399218f53735628c3b2d759a832e2adab/protobuf-3.20.3-cp37-cp37m-win32.whl", hash = "sha256:b6cc7ba72a8850621bfec987cb72623e703b7fe2b9127a161ce61e61558ad905"},
-    {url = "https://files.pythonhosted.org/packages/fe/8f/d9db035740002d61b4140aaef53a8bac7e316b18ec8744eb6c1fcf83c310/protobuf-3.20.3-cp37-cp37m-macosx_10_9_x86_64.whl", hash = "sha256:e64857f395505ebf3d2569935506ae0dfc4a15cb80dc25261176c784662cdcc4"},
-]
 "psutil 5.9.4" = [
     {url = "https://files.pythonhosted.org/packages/1d/80/e1502ba4ff65390bd17b4612010762075f64f5a0e7c28e889c4820bd95a9/psutil-5.9.4-cp27-cp27m-manylinux2010_x86_64.whl", hash = "sha256:3ff89f9b835100a825b14c2808a106b6fdcc4b15483141482a12c725e7f78549"},
     {url = "https://files.pythonhosted.org/packages/25/6e/ba97809175c90cbdcd33b470e466ebf0854d15d1506e605cc0ddd284d5b6/psutil-5.9.4-cp36-abi3-win_amd64.whl", hash = "sha256:fd8522436a6ada7b4aad6638662966de0d61d241cb821239b2ae7013d41a43d4"},
     {url = "https://files.pythonhosted.org/packages/3d/7d/d05864a69e452f003c0d77e728e155a89a2a26b09e64860ddd70ad64fb26/psutil-5.9.4.tar.gz", hash = "sha256:3d7f9739eb435d4b1338944abe23f49584bde5395f27487d2ee25ad9a8774a62"},
     {url = "https://files.pythonhosted.org/packages/3e/af/fe14b984e8b0f778d502d387b789d846cb2fcc3989f63be942741266d8c8/psutil-5.9.4-cp36-abi3-win32.whl", hash = "sha256:149555f59a69b33f056ba1c4eb22bb7bf24332ce631c44a319cec09f876aaeff"},
     {url = "https://files.pythonhosted.org/packages/53/ae/536719016fe9399187dbf52cdc65aef942f82b75924495918a2f701bcb77/psutil-5.9.4-cp27-cp27m-win32.whl", hash = "sha256:852dd5d9f8a47169fe62fd4a971aa07859476c2ba22c2254d4a1baa4e10b95ad"},
     {url = "https://files.pythonhosted.org/packages/5a/37/ef88eed265d93bc28c681316f68762c5e04167519e5627a0187c8878b409/psutil-5.9.4-cp36-abi3-manylinux_2_12_i686.manylinux2010_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:16653106f3b59386ffe10e0bad3bb6299e169d5327d3f187614b1cb8f24cf2e1"},
@@ -2481,34 +2251,26 @@
     {url = "https://files.pythonhosted.org/packages/eb/25/694204296d1e2b8361cccc44bc2275c032e14be4f36c3b012e2906602296/pyarrow-11.0.0-cp37-cp37m-macosx_10_14_x86_64.whl", hash = "sha256:1cbcfcbb0e74b4d94f0b7dde447b835a01bc1d16510edb8bb7d6224b9bf5bafc"},
     {url = "https://files.pythonhosted.org/packages/ed/d2/9780501efdb77dbd3865375e9dc02d2b3963fc4d60b551f8d0ccec07e4de/pyarrow-11.0.0-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:a37bc81f6c9435da3c9c1e767324ac3064ffbe110c4e460660c43e144be4ed85"},
 ]
 "pycparser 2.21" = [
     {url = "https://files.pythonhosted.org/packages/5e/0b/95d387f5f4433cb0f53ff7ad859bd2c6051051cebbb564f139a999ab46de/pycparser-2.21.tar.gz", hash = "sha256:e644fdec12f7872f86c58ff790da456218b10f863970249516d60a5eaca77206"},
     {url = "https://files.pythonhosted.org/packages/62/d5/5f610ebe421e85889f2e55e33b7f9a6795bd982198517d912eb1c76e1a53/pycparser-2.21-py2.py3-none-any.whl", hash = "sha256:8ee45429555515e1f6b185e78100aea234072576aa43ab53aefcae078162fca9"},
 ]
-"pydeck 0.8.0" = [
-    {url = "https://files.pythonhosted.org/packages/a7/86/f7478f621e998b36afa4e668088c407b04182e1080d609f6b8d0b1396401/pydeck-0.8.0.tar.gz", hash = "sha256:07edde833f7cfcef6749124351195aa7dcd24663d4909fd7898dbd0b6fbc01ec"},
-    {url = "https://files.pythonhosted.org/packages/ac/1e/676ed6c028bfd39d6c7c75abd57bc482f7eaa813f3faa715d80431732a43/pydeck-0.8.0-py2.py3-none-any.whl", hash = "sha256:a8fa7757c6f24bba033af39db3147cb020eef44012ba7e60d954de187f9ed4d5"},
-]
 "pydot 1.4.2" = [
     {url = "https://files.pythonhosted.org/packages/13/6e/916cdf94f9b38ae0777b254c75c3bdddee49a54cc4014aac1460a7a172b3/pydot-1.4.2.tar.gz", hash = "sha256:248081a39bcb56784deb018977e428605c1c758f10897a339fce1dd728ff007d"},
     {url = "https://files.pythonhosted.org/packages/ea/76/75b1bb82e9bad3e3d656556eaa353d8cd17c4254393b08ec9786ac8ed273/pydot-1.4.2-py2.py3-none-any.whl", hash = "sha256:66c98190c65b8d2e2382a441b4c0edfdb4f4c025ef9cb9874de478fb0793a451"},
 ]
 "pygments 2.15.0" = [
     {url = "https://files.pythonhosted.org/packages/03/98/c7468f5a1b434cb15b1d240c5f3bd015962af8a822e89e7f10ee11e68928/Pygments-2.15.0.tar.gz", hash = "sha256:f7e36cffc4c517fbc252861b9a6e4644ca0e5abadf9a113c72d1358ad09b9500"},
     {url = "https://files.pythonhosted.org/packages/08/4c/c587fc05d6f15f4deff971cb1a5b624429d6187c19f7274a50670edf3ec8/Pygments-2.15.0-py3-none-any.whl", hash = "sha256:77a3299119af881904cd5ecd1ac6a66214b6e9bed1f2db16993b54adede64094"},
 ]
 "pyment 0.3.3" = [
     {url = "https://files.pythonhosted.org/packages/52/01/810e174c28a7dcf5f91c048faf69c84eafee60c9a844e4ce21671b2e99bb/Pyment-0.3.3-py2.py3-none-any.whl", hash = "sha256:a0c6ec59d06d24aeec3eaecb22115d0dc95d09e14209b2df838381fdf47a78cc"},
     {url = "https://files.pythonhosted.org/packages/dd/9e/c58a151c7020f6fdd48eea0085a9d1c91a57da19fa4e7bff0daf930c9900/Pyment-0.3.3.tar.gz", hash = "sha256:951a4c52d6791ccec55bc739811169eed69917d3874f5fe722866623a697f39d"},
 ]
-"pympler 1.0.1" = [
-    {url = "https://files.pythonhosted.org/packages/12/b7/9d17fbb2fde0b035dbd27e5d82dfbcd3fa990cf5a469cef8e89712d16113/Pympler-1.0.1.tar.gz", hash = "sha256:993f1a3599ca3f4fcd7160c7545ad06310c9e12f70174ae7ae8d4e25f6c5d3fa"},
-    {url = "https://files.pythonhosted.org/packages/2c/42/41e1469ed0b37b9c8532cb8074bea179f7d85ee7e82a59b5b6c289ed6045/Pympler-1.0.1-py3-none-any.whl", hash = "sha256:d260dda9ae781e1eab6ea15bacb84015849833ba5555f141d2d9b7b7473b307d"},
-]
 "pyparsing 3.0.9" = [
     {url = "https://files.pythonhosted.org/packages/6c/10/a7d0fa5baea8fe7b50f448ab742f26f52b80bfca85ac2be9d35cdd9a3246/pyparsing-3.0.9-py3-none-any.whl", hash = "sha256:5026bae9a10eeaefb61dab2f09052b9f4307d44aee4eda64b309723d8d206bbc"},
     {url = "https://files.pythonhosted.org/packages/71/22/207523d16464c40a0310d2d4d8926daffa00ac1f5b1576170a32db749636/pyparsing-3.0.9.tar.gz", hash = "sha256:2b020ecf7d21b687f219b71ecad3631f644a47f01403fa1d1036b0c6416d70fb"},
 ]
 "pyproject-hooks 1.0.0" = [
     {url = "https://files.pythonhosted.org/packages/25/c1/374304b8407d3818f7025457b7366c8e07768377ce12edfe2aa58aa0f64c/pyproject_hooks-1.0.0.tar.gz", hash = "sha256:f271b298b97f5955d53fb12b72c1fb1948c22c1a6b70b315c54cedaca0264ef5"},
     {url = "https://files.pythonhosted.org/packages/d5/ea/9ae603de7fbb3df820b23a70f6aff92bf8c7770043254ad8d2dc9d6bcba4/pyproject_hooks-1.0.0-py3-none-any.whl", hash = "sha256:283c11acd6b928d2f6a7c73fa0d01cb2bdc5f07c57a2eeb6e83d5e56b97976f8"},
@@ -2558,18 +2320,14 @@
     {url = "https://files.pythonhosted.org/packages/35/a6/145655273568ee78a581e734cf35beb9e33a370b29c5d3c8fee3744de29f/python_json_logger-2.0.7-py3-none-any.whl", hash = "sha256:f380b826a991ebbe3de4d897aeec42760035ac760345e57b812938dc8b35e2bd"},
     {url = "https://files.pythonhosted.org/packages/4f/da/95963cebfc578dabd323d7263958dfb68898617912bb09327dd30e9c8d13/python-json-logger-2.0.7.tar.gz", hash = "sha256:23e7ec02d34237c5aa1e29a070193a4ea87583bb4e7f8fd06d3de8264c4b2e1c"},
 ]
 "pytz 2023.3" = [
     {url = "https://files.pythonhosted.org/packages/5e/32/12032aa8c673ee16707a9b6cdda2b09c0089131f35af55d443b6a9c69c1d/pytz-2023.3.tar.gz", hash = "sha256:1d8ce29db189191fb55338ee6d0387d82ab59f3d00eac103412d64e0ebd0c588"},
     {url = "https://files.pythonhosted.org/packages/7f/99/ad6bd37e748257dd70d6f85d916cafe79c0b0f5e2e95b11f7fbc82bf3110/pytz-2023.3-py2.py3-none-any.whl", hash = "sha256:a151b3abb88eda1d4e34a9814df37de2a80e301e68ba0fd856fb9b46bfbbbffb"},
 ]
-"pytz-deprecation-shim 0.1.0.post0" = [
-    {url = "https://files.pythonhosted.org/packages/94/f0/909f94fea74759654390a3e1a9e4e185b6cd9aa810e533e3586f39da3097/pytz_deprecation_shim-0.1.0.post0.tar.gz", hash = "sha256:af097bae1b616dde5c5744441e2ddc69e74dfdcb0c263129610d85b87445a59d"},
-    {url = "https://files.pythonhosted.org/packages/eb/73/3eaab547ca809754e67e06871cff0fc962bafd4b604e15f31896a0f94431/pytz_deprecation_shim-0.1.0.post0-py2.py3-none-any.whl", hash = "sha256:8314c9692a636c8eb3bda879b9f119e350e93223ae83e70e80c31675a0fdc1a6"},
-]
 "pywin32 306" = [
     {url = "https://files.pythonhosted.org/packages/08/dc/28c668097edfaf4eac4617ef7adf081b9cf50d254672fcf399a70f5efc41/pywin32-306-cp310-cp310-win32.whl", hash = "sha256:06d3420a5155ba65f0b72f2699b5bacf3109f36acbe8923765c22938a69dfc8d"},
     {url = "https://files.pythonhosted.org/packages/0e/57/c3ec32b498f24a2392404d1f0fd29f47a3f7339d7d579df7a0560cff337c/pywin32-306-cp38-cp38-win32.whl", hash = "sha256:e4c092e2589b5cf0d365849e73e02c391c1349958c5ac3e9d5ccb9a28e017b3a"},
     {url = "https://files.pythonhosted.org/packages/14/91/17e016d5923e178346aabda3dfec6629d1a26efe587d19667542105cf0a6/pywin32-306-cp312-cp312-win32.whl", hash = "sha256:383229d515657f4e3ed1343da8be101000562bf514591ff383ae940cad65458b"},
     {url = "https://files.pythonhosted.org/packages/1c/43/e3444dc9a12f8365d9603c2145d16bf0a2f8180f343cf87be47f5579e547/pywin32-306-cp312-cp312-win_arm64.whl", hash = "sha256:5821ec52f6d321aa59e2db7e0a35b997de60c201943557d108af9d4ae1ec7040"},
     {url = "https://files.pythonhosted.org/packages/1c/f7/24d8ed4fd9c43b90354df7764f81f0dd5e623f9a50f1538f90fe085d6dff/pywin32-306-cp39-cp39-win_amd64.whl", hash = "sha256:39b61c15272833b5c329a2989999dcae836b1eed650252ab1b7bfbe1d59f30f4"},
     {url = "https://files.pythonhosted.org/packages/28/19/6b8f416ff02132c404042f251eb90a41d15abe677481fcff22077e943c6f/pywin32-306-cp37-cp37m-win32.whl", hash = "sha256:1c73ea9a0d2283d889001998059f5eaaba3b6238f767c9cf2833b13e6a685f65"},
@@ -2727,17 +2485,17 @@
     {url = "https://files.pythonhosted.org/packages/28/ea/a9387748e2d111c3c2b275ba970b735e04e15cdb1eb30693b6b5708c4dbd/rfc3339_validator-0.1.4.tar.gz", hash = "sha256:138a2abdf93304ad60530167e51d2dfb9549521a836871b88d7f4695d0022f6b"},
     {url = "https://files.pythonhosted.org/packages/7b/44/4e421b96b67b2daff264473f7465db72fbdf36a07e05494f50300cc7b0c6/rfc3339_validator-0.1.4-py2.py3-none-any.whl", hash = "sha256:24f6ec1eda14ef823da9e36ec7113124b39c04d50a4d3d3a3c2859577e7791fa"},
 ]
 "rfc3986-validator 0.1.1" = [
     {url = "https://files.pythonhosted.org/packages/9e/51/17023c0f8f1869d8806b979a2bffa3f861f26a3f1a66b094288323fba52f/rfc3986_validator-0.1.1-py2.py3-none-any.whl", hash = "sha256:2f235c432ef459970b4306369336b9d5dbdda31b510ca1e327636e01f528bfa9"},
     {url = "https://files.pythonhosted.org/packages/da/88/f270de456dd7d11dcc808abfa291ecdd3f45ff44e3b549ffa01b126464d0/rfc3986_validator-0.1.1.tar.gz", hash = "sha256:3d44bde7921b3b9ec3ae4e3adca370438eccebc676456449b145d533b240d055"},
 ]
-"rich 13.3.3" = [
-    {url = "https://files.pythonhosted.org/packages/42/5c/f44fc88bad850c4a20711a3349ec0e8bc50fece8d8b32c962d2aab70ea2b/rich-13.3.3-py3-none-any.whl", hash = "sha256:540c7d6d26a1178e8e8b37e9ba44573a3cd1464ff6348b99ee7061b95d1c6333"},
-    {url = "https://files.pythonhosted.org/packages/9a/50/672a8d347f92bc752b04c338bbf932fbd0104fbc416c82cc91aa5f7b4b0b/rich-13.3.3.tar.gz", hash = "sha256:dc84400a9d842b3a9c5ff74addd8eb798d155f36c1c91303888e0a66850d2a15"},
+"rich 12.6.0" = [
+    {url = "https://files.pythonhosted.org/packages/11/23/814edf09ec6470d52022b9e95c23c1bef77f0bc451761e1504ebd09606d3/rich-12.6.0.tar.gz", hash = "sha256:ba3a3775974105c221d31141f2c116f4fd65c5ceb0698657a11e9f295ec93fd0"},
+    {url = "https://files.pythonhosted.org/packages/32/60/81ac2e7d1e3b861ab478a72e3b20fc91c4302acd2274822e493758941829/rich-12.6.0-py3-none-any.whl", hash = "sha256:a4eb26484f2c82589bd9a17c73d32a010b1e29d89f1604cd9bf3a2097b81bb5e"},
 ]
 "ruff 0.0.261" = [
     {url = "https://files.pythonhosted.org/packages/0d/92/a8ca1c04dc47e7ac2667e445654590d689105fc106026df55cbcfcac0693/ruff-0.0.261-py3-none-manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:cc970f6ece0b4950e419f0252895ee42e9e8e5689c6494d18f5dc2c6ebb7f798"},
     {url = "https://files.pythonhosted.org/packages/14/40/96c3a8831a5fbac714ead0064ad6681526385908f2dd06f83391d6c7e08a/ruff-0.0.261-py3-none-musllinux_1_2_aarch64.whl", hash = "sha256:4bcec45abdf65c1328a269cf6cc193f7ff85b777fa2865c64cf2c96b80148a2c"},
     {url = "https://files.pythonhosted.org/packages/1b/a4/e89fbf5777404eb4b4532f5b06a709129eecdf6dcef0980688bec5f6b949/ruff-0.0.261-py3-none-win_amd64.whl", hash = "sha256:0fbc689c23609edda36169c8708bb91bab111d8f44cb4a88330541757770ab30"},
     {url = "https://files.pythonhosted.org/packages/2e/8b/5f6b7a8d4cc8dac3dcd2573180a7dbca839a73055df2e067272c543d997f/ruff-0.0.261-py3-none-musllinux_1_2_i686.whl", hash = "sha256:39abd02342cec0c131b2ddcaace08b2eae9700cab3ca7dba64ae5fd4f4881bd0"},
     {url = "https://files.pythonhosted.org/packages/2e/eb/8dfafe1ee789a495d85d679f5f788f275d9ea4f84add1668a05a749aadc1/ruff-0.0.261-py3-none-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:d1293acc64eba16a11109678dc4743df08c207ed2edbeaf38b3e10eb2597321b"},
@@ -2750,74 +2508,58 @@
     {url = "https://files.pythonhosted.org/packages/75/2c/3ecfee398c2608fb752caa19febab02381a4e55d7a18cae052df19cdc161/ruff-0.0.261-py3-none-manylinux_2_17_ppc64.manylinux2014_ppc64.whl", hash = "sha256:8fa98e747e0fe185d65a40b0ea13f55c492f3b5f9a032a1097e82edaddb9e52e"},
     {url = "https://files.pythonhosted.org/packages/97/7f/141919718fcacfec51ec23e6cb5c73bddf51be58f9549830951384470eb8/ruff-0.0.261-py3-none-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:8dbd0cee5a81b0785dc0feeb2640c1e31abe93f0d77c5233507ac59731a626f1"},
     {url = "https://files.pythonhosted.org/packages/9c/aa/da57cbfc20c854d339a65c082b26c4ca9b4fbc7c6496934b46c68163a3d6/ruff-0.0.261-py3-none-win_arm64.whl", hash = "sha256:d2eddc60ae75fc87f8bb8fd6e8d5339cf884cd6de81e82a50287424309c187ba"},
     {url = "https://files.pythonhosted.org/packages/d6/a2/0d5b08e9f27d0aa5369446a6146b5b4fe4ce4625732f49858dbed8768316/ruff-0.0.261-py3-none-win32.whl", hash = "sha256:daff64b4e86e42ce69e6367d63aab9562fc213cd4db0e146859df8abc283dba0"},
     {url = "https://files.pythonhosted.org/packages/dc/3a/209f1e016e6ed885e788b6021508aa257bd202ccbc72fae0a0f309e9e719/ruff-0.0.261-py3-none-macosx_10_7_x86_64.whl", hash = "sha256:6624a966c4a21110cee6780333e2216522a831364896f3d98f13120936eff40a"},
     {url = "https://files.pythonhosted.org/packages/e3/e9/717b326c9cfcf95461ea2b52a740de10da9abb0c8209a6fd29f1c946447c/ruff-0.0.261-py3-none-macosx_10_9_x86_64.macosx_11_0_arm64.macosx_10_9_universal2.whl", hash = "sha256:2dba68a9e558ab33e6dd5d280af798a2d9d3c80c913ad9c8b8e97d7b287f1cc9"},
 ]
-"semver 3.0.0" = [
-    {url = "https://files.pythonhosted.org/packages/5e/e2/699f6c2e9c4782694cd670a25806fa653e5fd065e9edf5dac33029dcb687/semver-3.0.0-py3-none-any.whl", hash = "sha256:ab4f69fb1d1ecfb5d81f96411403d7a611fa788c45d252cf5b408025df3ab6ce"},
-    {url = "https://files.pythonhosted.org/packages/9f/93/b7389cdd7e573e70cfbeb4b0bbe101af1050a6681342f5d2bc6f1bf2d150/semver-3.0.0.tar.gz", hash = "sha256:94df43924c4521ec7d307fc86da1531db6c2c33d9d5cdc3e64cca0eb68569269"},
-]
 "send2trash 1.8.0" = [
     {url = "https://files.pythonhosted.org/packages/47/26/3435896d757335ea53dce5abf8d658ca80757a7a06258451b358f10232be/Send2Trash-1.8.0-py3-none-any.whl", hash = "sha256:f20eaadfdb517eaca5ce077640cb261c7d2698385a6a0f072a4a5447fd49fa08"},
     {url = "https://files.pythonhosted.org/packages/49/2c/d990b8d5a7378dde856f5a82e36ed9d6061b5f2d00f39dc4317acd9538b4/Send2Trash-1.8.0.tar.gz", hash = "sha256:d2c24762fd3759860a0aff155e45871447ea58d2be6bdd39b5c8f966a0c99c2d"},
 ]
 "setuptools 67.6.1" = [
     {url = "https://files.pythonhosted.org/packages/0b/fc/8781442def77b0aa22f63f266d4dadd486ebc0c5371d6290caf4320da4b7/setuptools-67.6.1-py3-none-any.whl", hash = "sha256:e728ca814a823bf7bf60162daf9db95b93d532948c4c0bea762ce62f60189078"},
     {url = "https://files.pythonhosted.org/packages/cb/46/22ec35f286a77e6b94adf81b4f0d59f402ed981d4251df0ba7b992299146/setuptools-67.6.1.tar.gz", hash = "sha256:257de92a9d50a60b8e22abfcbb771571fde0dbf3ec234463212027a4eeecbe9a"},
 ]
 "setuptools-scm 7.1.0" = [
     {url = "https://files.pythonhosted.org/packages/1d/66/8f42c941be949ef2b22fe905d850c794e7c170a526023612aad5f3a121ad/setuptools_scm-7.1.0-py3-none-any.whl", hash = "sha256:73988b6d848709e2af142aa48c986ea29592bbcfca5375678064708205253d8e"},
     {url = "https://files.pythonhosted.org/packages/98/12/2c1e579bb968759fc512391473340d0661b1a8c96a59fb7c65b02eec1321/setuptools_scm-7.1.0.tar.gz", hash = "sha256:6c508345a771aad7d56ebff0e70628bf2b0ec7573762be9960214730de278f27"},
 ]
+"shellingham 1.5.0.post1" = [
+    {url = "https://files.pythonhosted.org/packages/1f/13/fab0a3f512478bc387b66c51557ee715ede8e9811c77ce952f9b9a4d8ac1/shellingham-1.5.0.post1.tar.gz", hash = "sha256:823bc5fb5c34d60f285b624e7264f4dda254bc803a3774a147bf99c0e3004a28"},
+    {url = "https://files.pythonhosted.org/packages/ae/2a/7ad62b2c56e71c6330fc35cfd5813376e788146ef7c884cc2fdf5fe77696/shellingham-1.5.0.post1-py2.py3-none-any.whl", hash = "sha256:368bf8c00754fd4f55afb7bbb86e272df77e4dc76ac29dbcbb81a59e9fc15744"},
+]
 "six 1.16.0" = [
     {url = "https://files.pythonhosted.org/packages/71/39/171f1c67cd00715f190ba0b100d606d440a28c93c7714febeca8b79af85e/six-1.16.0.tar.gz", hash = "sha256:1e61c37477a1626458e36f7b1d82aa5c9b094fa4802892072e49de9c60c4c926"},
     {url = "https://files.pythonhosted.org/packages/d9/5a/e7c31adbe875f2abbb91bd84cf2dc52d792b5a01506781dbcf25c91daf11/six-1.16.0-py2.py3-none-any.whl", hash = "sha256:8abb2f1d86890a2dfb989f9a77cfcfd3e47c2a354b01111771326f8aa26e0254"},
 ]
-"smmap 5.0.0" = [
-    {url = "https://files.pythonhosted.org/packages/21/2d/39c6c57032f786f1965022563eec60623bb3e1409ade6ad834ff703724f3/smmap-5.0.0.tar.gz", hash = "sha256:c840e62059cd3be204b0c9c9f74be2c09d5648eddd4580d9314c3ecde0b30936"},
-    {url = "https://files.pythonhosted.org/packages/6d/01/7caa71608bc29952ae09b0be63a539e50d2484bc37747797a66a60679856/smmap-5.0.0-py3-none-any.whl", hash = "sha256:2aba19d6a040e78d8b09de5c57e96207b09ed71d8e55ce0959eeee6c8e190d94"},
-]
 "sniffio 1.3.0" = [
     {url = "https://files.pythonhosted.org/packages/c3/a0/5dba8ed157b0136607c7f2151db695885606968d1fae123dc3391e0cfdbf/sniffio-1.3.0-py3-none-any.whl", hash = "sha256:eecefdce1e5bbfb7ad2eeaabf7c1eeb404d7757c379bd1f7e5cce9d8bf425384"},
     {url = "https://files.pythonhosted.org/packages/cd/50/d49c388cae4ec10e8109b1b833fd265511840706808576df3ada99ecb0ac/sniffio-1.3.0.tar.gz", hash = "sha256:e60305c5e5d314f5389259b7f22aaa33d8f7dee49763119234af3755c55b9101"},
 ]
 "soupsieve 2.4" = [
     {url = "https://files.pythonhosted.org/packages/1b/cb/34933ebdd6bf6a77daaa0bd04318d61591452eb90ecca4def947e3cb2165/soupsieve-2.4.tar.gz", hash = "sha256:e28dba9ca6c7c00173e34e4ba57448f0688bb681b7c5e8bf4971daafc093d69a"},
     {url = "https://files.pythonhosted.org/packages/d2/70/2c92d7bc961ba43b7b21032b7622144de5f97dec14b62226533f6940798e/soupsieve-2.4-py3-none-any.whl", hash = "sha256:49e5368c2cda80ee7e84da9dbe3e110b70a4575f196efb74e51b94549d921955"},
 ]
 "stack-data 0.6.2" = [
     {url = "https://files.pythonhosted.org/packages/6a/81/aa96c25c27f78cdc444fec27d80f4c05194c591465e491a1358d8a035bc1/stack_data-0.6.2-py3-none-any.whl", hash = "sha256:cbb2a53eb64e5785878201a97ed7c7b94883f48b87bfb0bbe8b623c74679e4a8"},
     {url = "https://files.pythonhosted.org/packages/db/18/aa7f2b111aeba2cd83503254d9133a912d7f61f459a0c8561858f0d72a56/stack_data-0.6.2.tar.gz", hash = "sha256:32d2dd0376772d01b6cb9fc996f3c8b57a357089dec328ed4b6553d037eaf815"},
 ]
-"streamlit 1.12.0" = [
-    {url = "https://files.pythonhosted.org/packages/28/7b/560c4e4f524c278e340e5ca2933c7ecdc36bb3646ed8e9581bd064d49e12/streamlit-1.12.0.tar.gz", hash = "sha256:1bbb406d4eee9acb055e72627212e9f04eea8ef0332f8dfeb6745bdf256c168b"},
-    {url = "https://files.pythonhosted.org/packages/a0/2b/b710d52297f733e703fecce3614d6cfa81e11d241c246354fb5b55aa9572/streamlit-1.12.0-py2.py3-none-any.whl", hash = "sha256:19f58ae723afaedbc85891c3a159e9576343609036713ecbb73b219a47dfe48d"},
-]
 "terminado 0.17.1" = [
     {url = "https://files.pythonhosted.org/packages/55/be/748034192602b9fd69ba94544c1675ff18b039ed8f346ad783478e31144f/terminado-0.17.1.tar.gz", hash = "sha256:6ccbbcd3a4f8a25a5ec04991f39a0b8db52dfcd487ea0e578d977e6752380333"},
     {url = "https://files.pythonhosted.org/packages/84/a7/c7628d79651b8c8c775d27b374315a825141b5783512e82026fb210dd639/terminado-0.17.1-py3-none-any.whl", hash = "sha256:8650d44334eba354dd591129ca3124a6ba42c3d5b70df5051b6921d506fdaeae"},
 ]
 "tinycss2 1.2.1" = [
     {url = "https://files.pythonhosted.org/packages/75/be/24179dfaa1d742c9365cbd0e3f0edc5d3aa3abad415a2327c5a6ff8ca077/tinycss2-1.2.1.tar.gz", hash = "sha256:8cff3a8f066c2ec677c06dbc7b45619804a6938478d9d73c284b29d14ecb0627"},
     {url = "https://files.pythonhosted.org/packages/da/99/fd23634d6962c2791fb8cb6ccae1f05dcbfc39bce36bba8b1c9a8d92eae8/tinycss2-1.2.1-py3-none-any.whl", hash = "sha256:2b80a96d41e7c3914b8cda8bc7f705a4d9c49275616e886103dd839dfc847847"},
 ]
-"toml 0.10.2" = [
-    {url = "https://files.pythonhosted.org/packages/44/6f/7120676b6d73228c96e17f1f794d8ab046fc910d781c8d151120c3f1569e/toml-0.10.2-py2.py3-none-any.whl", hash = "sha256:806143ae5bfb6a3c6e736a764057db0e6a0e05e338b5630894a5f779cabb4f9b"},
-    {url = "https://files.pythonhosted.org/packages/be/ba/1f744cdc819428fc6b5084ec34d9b30660f6f9daaf70eead706e3203ec3c/toml-0.10.2.tar.gz", hash = "sha256:b3bda1d108d5dd99f4a20d24d9c348e91c4db7ab1b749200bded2f839ccbe68f"},
-]
 "tomli 2.0.1" = [
     {url = "https://files.pythonhosted.org/packages/97/75/10a9ebee3fd790d20926a90a2547f0bf78f371b2f13aa822c759680ca7b9/tomli-2.0.1-py3-none-any.whl", hash = "sha256:939de3e7a6161af0c887ef91b7d41a53e7c5a1ca976325f429cb46ea9bc30ecc"},
     {url = "https://files.pythonhosted.org/packages/c0/3f/d7af728f075fb08564c5949a9c95e44352e23dee646869fa104a3b2060a3/tomli-2.0.1.tar.gz", hash = "sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f"},
 ]
-"toolz 0.12.0" = [
-    {url = "https://files.pythonhosted.org/packages/7f/5c/922a3508f5bda2892be3df86c74f9cf1e01217c2b1f8a0ac4841d903e3e9/toolz-0.12.0-py3-none-any.whl", hash = "sha256:2059bd4148deb1884bb0eb770a3cde70e7f954cfbbdc2285f1f2de01fd21eb6f"},
-    {url = "https://files.pythonhosted.org/packages/cf/05/2008534bbaa716b46a2d795d7b54b999d0f7638fbb9ed0b6e87bfa934f84/toolz-0.12.0.tar.gz", hash = "sha256:88c570861c440ee3f2f6037c4654613228ff40c93a6c25e0eba70d17282c6194"},
-]
 "tornado 6.2" = [
     {url = "https://files.pythonhosted.org/packages/11/30/ac70f5c5f03cf1cd0ae8199c80382387a9fe57e8f68853d5c9527c0219e5/tornado-6.2-cp37-abi3-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:b8150f721c101abdef99073bf66d3903e292d851bee51910839831caba341a75"},
     {url = "https://files.pythonhosted.org/packages/19/bb/b6c3d1668d2b10ad38a584f3a1ec9737984e274f8b708e09fcbb96427f5c/tornado-6.2-cp37-abi3-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:d3a2f5999215a3a06a4fc218026cd84c61b8b2b40ac5296a6db1f1451ef04c1e"},
     {url = "https://files.pythonhosted.org/packages/1c/26/cbfa1103e74a02e09dd53291e419da3ad4c5b948f52aea5800e6671b56e0/tornado-6.2-cp37-abi3-win_amd64.whl", hash = "sha256:e5f923aa6a47e133d1cf87d60700889d7eae68988704e20c75fb2d65677a8e4b"},
     {url = "https://files.pythonhosted.org/packages/5c/0c/cbc0a98f7b8ef833bcb13c58d35d09e2c288ae67a35af4c8960b88f99ae9/tornado-6.2-cp37-abi3-macosx_10_9_x86_64.whl", hash = "sha256:87dcafae3e884462f90c90ecc200defe5e580a7fbbb4365eda7c7c1eb809ebc9"},
     {url = "https://files.pythonhosted.org/packages/60/08/e630a348b34a9ddd640aed67dafc6f0df425d8ac07d2fa60288f38321c69/tornado-6.2-cp37-abi3-musllinux_1_1_i686.whl", hash = "sha256:6fdfabffd8dfcb6cf887428849d30cf19a3ea34c2c248461e1f7d718ad30b66b"},
     {url = "https://files.pythonhosted.org/packages/71/cc/c1342382484d0178a79029109c433e406a60095da1c3605ca966775a70e5/tornado-6.2-cp37-abi3-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:ba09ef14ca9893954244fd872798b4ccb2367c165946ce2dd7376aebdde8e3ac"},
@@ -2827,70 +2569,34 @@
     {url = "https://files.pythonhosted.org/packages/f9/51/6f63a166d9a3077be100cbb13dcbce434e5654daaaa7003b0a045b9f6edf/tornado-6.2-cp37-abi3-musllinux_1_1_x86_64.whl", hash = "sha256:1d54d13ab8414ed44de07efecb97d4ef7c39f7438cf5e976ccd356bebb1b5fca"},
     {url = "https://files.pythonhosted.org/packages/fb/bd/074254a55bfc82d7a1886abbd803600ef01cbd76ee66bc30307b2724130b/tornado-6.2-cp37-abi3-macosx_10_9_universal2.whl", hash = "sha256:20f638fd8cc85f3cbae3c732326e96addff0a15e22d80f049e00121651e82e72"},
 ]
 "traitlets 5.9.0" = [
     {url = "https://files.pythonhosted.org/packages/39/c3/205e88f02959712b62008502952707313640369144a7fded4cbc61f48321/traitlets-5.9.0.tar.gz", hash = "sha256:f6cde21a9c68cf756af02035f72d5a723bf607e862e7be33ece505abf4a3bad9"},
     {url = "https://files.pythonhosted.org/packages/77/75/c28e9ef7abec2b7e9ff35aea3e0be6c1aceaf7873c26c95ae1f0d594de71/traitlets-5.9.0-py3-none-any.whl", hash = "sha256:9e6ec080259b9a5940c797d58b613b5e31441c2257b87c2e795c5228ae80d2d8"},
 ]
+"typer 0.7.0" = [
+    {url = "https://files.pythonhosted.org/packages/0d/44/56c3f48d2bb83d76f5c970aef8e2c3ebd6a832f09e3621c5395371fe6999/typer-0.7.0-py3-none-any.whl", hash = "sha256:b5e704f4e48ec263de1c0b3a2387cd405a13767d2f907f44c1a08cbad96f606d"},
+    {url = "https://files.pythonhosted.org/packages/e1/45/bcbc581f87c8d8f2a56b513eb994d07ea4546322818d95dc6a3caf2c928b/typer-0.7.0.tar.gz", hash = "sha256:ff797846578a9f2a201b53442aedeb543319466870fbe1c701eab66dd7681165"},
+]
 "typing-extensions 4.5.0" = [
     {url = "https://files.pythonhosted.org/packages/31/25/5abcd82372d3d4a3932e1fa8c3dbf9efac10cc7c0d16e78467460571b404/typing_extensions-4.5.0-py3-none-any.whl", hash = "sha256:fb33085c39dd998ac16d1431ebc293a8b3eedd00fd4a32de0ff79002c19511b4"},
     {url = "https://files.pythonhosted.org/packages/d3/20/06270dac7316220643c32ae61694e451c98f8caf4c8eab3aa80a2bedf0df/typing_extensions-4.5.0.tar.gz", hash = "sha256:5cb5f4a79139d699607b3ef622a1dedafa84e115ab0024e0d9c044a9479ca7cb"},
 ]
-"tzdata 2023.3" = [
-    {url = "https://files.pythonhosted.org/packages/70/e5/81f99b9fced59624562ab62a33df639a11b26c582be78864b339dafa420d/tzdata-2023.3.tar.gz", hash = "sha256:11ef1e08e54acb0d4f95bdb1be05da659673de4acbd21bf9c69e94cc5e907a3a"},
-    {url = "https://files.pythonhosted.org/packages/d5/fb/a79efcab32b8a1f1ddca7f35109a50e4a80d42ac1c9187ab46522b2407d7/tzdata-2023.3-py2.py3-none-any.whl", hash = "sha256:7e65763eef3120314099b6939b5546db7adce1e7d6f2e179e3df563c70511eda"},
-]
-"tzlocal 4.3" = [
-    {url = "https://files.pythonhosted.org/packages/39/97/b15b711a10d0774390404bec9712b2647b0b53a4da50a08acf7d7e51e284/tzlocal-4.3.tar.gz", hash = "sha256:3f21d09e1b2aa9f2dacca12da240ca37de3ba5237a93addfd6d593afe9073355"},
-    {url = "https://files.pythonhosted.org/packages/d4/46/e8002faae3d1df7d7a0a3aa0cb4b2ccd805c3a71fb507b06446012b28790/tzlocal-4.3-py3-none-any.whl", hash = "sha256:b44c4388f3d34f25862cfbb387578a4d70fec417649da694a132f628a23367e2"},
-]
 "uri-template 1.2.0" = [
     {url = "https://files.pythonhosted.org/packages/40/55/9318f307d3b0a70ce5812fd2b9da286b0f58a2ffbdba5fa269d0c052ae89/uri_template-1.2.0.tar.gz", hash = "sha256:934e4d09d108b70eb8a24410af8615294d09d279ce0e7cbcdaef1bd21f932b06"},
     {url = "https://files.pythonhosted.org/packages/c0/db/d4f9c75b43541f7235daf4d13eb43f4491f9d5f5df45ce41daeed3a903f6/uri_template-1.2.0-py3-none-any.whl", hash = "sha256:f1699c77b73b925cf4937eae31ab282a86dc885c333f2e942513f08f691fc7db"},
 ]
 "urllib3 1.26.15" = [
     {url = "https://files.pythonhosted.org/packages/21/79/6372d8c0d0641b4072889f3ff84f279b738cd8595b64c8e0496d4e848122/urllib3-1.26.15.tar.gz", hash = "sha256:8a388717b9476f934a21484e8c8e61875ab60644d29b9b39e11e4b9dc1c6b305"},
     {url = "https://files.pythonhosted.org/packages/7b/f5/890a0baca17a61c1f92f72b81d3c31523c99bec609e60c292ea55b387ae8/urllib3-1.26.15-py2.py3-none-any.whl", hash = "sha256:aa751d169e23c7479ce47a0cb0da579e3ede798f994f5816a74e4f4500dcea42"},
 ]
-"validators 0.20.0" = [
-    {url = "https://files.pythonhosted.org/packages/95/14/ed0af6865d378cfc3c504aed0d278a890cbefb2f1934bf2dbe92ecf9d6b1/validators-0.20.0.tar.gz", hash = "sha256:24148ce4e64100a2d5e267233e23e7afeb55316b47d30faae7eb6e7292bc226a"},
-]
 "virtualenv 20.21.0" = [
     {url = "https://files.pythonhosted.org/packages/86/2f/35a79942c38d4ca89b444085d67900f713f1967446fdcefc8351619d7c65/virtualenv-20.21.0-py3-none-any.whl", hash = "sha256:31712f8f2a17bd06234fa97fdf19609e789dd4e3e4bf108c3da71d710651adbc"},
     {url = "https://files.pythonhosted.org/packages/87/14/ca9890d58cd33d9122eb87ffec2f3c6be0714785f992a0fd3b56a3b6c993/virtualenv-20.21.0.tar.gz", hash = "sha256:f50e3e60f990a0757c9b68333c9fdaa72d7188caa417f96af9e52407831a3b68"},
 ]
-"watchdog 3.0.0" = [
-    {url = "https://files.pythonhosted.org/packages/00/9e/a9711f35f1ad6571e92dc2e955e7de9dfac21a1b33e9cd212f066a60a387/watchdog-3.0.0-cp311-cp311-macosx_10_9_universal2.whl", hash = "sha256:2b57a1e730af3156d13b7fdddfc23dea6487fceca29fc75c5a868beed29177ae"},
-    {url = "https://files.pythonhosted.org/packages/06/fd/58b82550ebe4883bb2a5e1b6c14d8702b5ce0f36c58470bba51dc777df46/watchdog-3.0.0-cp310-cp310-macosx_10_9_universal2.whl", hash = "sha256:336adfc6f5cc4e037d52db31194f7581ff744b67382eb6021c868322e32eef41"},
-    {url = "https://files.pythonhosted.org/packages/21/72/46fd174352cd88b9157ade77e3b8835125d4b1e5186fc7f1e8c44664e029/watchdog-3.0.0-py3-none-manylinux2014_i686.whl", hash = "sha256:c07253088265c363d1ddf4b3cdb808d59a0468ecd017770ed716991620b8f77a"},
-    {url = "https://files.pythonhosted.org/packages/2b/f0/456948b865ab259784f774154e7d65844fa9757522fdb11533fbf8ae7aca/watchdog-3.0.0-py3-none-manylinux2014_x86_64.whl", hash = "sha256:d429c2430c93b7903914e4db9a966c7f2b068dd2ebdd2fa9b9ce094c7d459f33"},
-    {url = "https://files.pythonhosted.org/packages/2e/54/48527f3aea4f7ed331072352fee034a7f3d6ec7a2ed873681738b2586498/watchdog-3.0.0-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:25f70b4aa53bd743729c7475d7ec41093a580528b100e9a8c5b5efe8899592fc"},
-    {url = "https://files.pythonhosted.org/packages/30/65/9e36a3c821d47a22e54a8fc73681586b2d26e82d24ea3af63acf2ef78f97/watchdog-3.0.0-pp39-pypy39_pp73-macosx_10_9_x86_64.whl", hash = "sha256:c9d8c8ec7efb887333cf71e328e39cffbf771d8f8f95d308ea4125bf5f90ba64"},
-    {url = "https://files.pythonhosted.org/packages/3a/9d/d6586a065968f3e5d89a2565dffa6ea9151ce9d46c541340bfff27b41231/watchdog-3.0.0-cp37-cp37m-macosx_10_9_x86_64.whl", hash = "sha256:9fac43a7466eb73e64a9940ac9ed6369baa39b3bf221ae23493a9ec4d0022674"},
-    {url = "https://files.pythonhosted.org/packages/40/1b/4e6d3e0f587587931f590531b4ed08070d71a9efb35541d792a68d8ee593/watchdog-3.0.0-py3-none-manylinux2014_s390x.whl", hash = "sha256:ba07e92756c97e3aca0912b5cbc4e5ad802f4557212788e72a72a47ff376950d"},
-    {url = "https://files.pythonhosted.org/packages/51/b9/444a984b1667013bac41b31b45d9718e069cc7502a43a924896806605d83/watchdog-3.0.0-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:233b5817932685d39a7896b1090353fc8efc1ef99c9c054e46c8002561252fb8"},
-    {url = "https://files.pythonhosted.org/packages/55/0d/bfc2a0d425b12444a2dc245a934c065bbb7bd9833fff071cba79c21bb76e/watchdog-3.0.0-py3-none-win32.whl", hash = "sha256:3ed7c71a9dccfe838c2f0b6314ed0d9b22e77d268c67e015450a29036a81f60f"},
-    {url = "https://files.pythonhosted.org/packages/58/db/d419fdbd3051b42b0a8091ddf78f70540b6d9d277a84845f7c5955f9de92/watchdog-3.0.0-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:7e447d172af52ad204d19982739aa2346245cc5ba6f579d16dac4bfec226d2e7"},
-    {url = "https://files.pythonhosted.org/packages/67/e4/229144d23093436a21a8b84aa5931d70759b81743dc8c10d0e836dbfd752/watchdog-3.0.0-pp37-pypy37_pp73-macosx_10_9_x86_64.whl", hash = "sha256:13bbbb462ee42ec3c5723e1205be8ced776f05b100e4737518c67c8325cf6100"},
-    {url = "https://files.pythonhosted.org/packages/71/3a/b12740f4f60861240d57b42a2ac6ac0a2821db506c4435f7872c1fad867d/watchdog-3.0.0-py3-none-manylinux2014_ppc64le.whl", hash = "sha256:51f90f73b4697bac9c9a78394c3acbbd331ccd3655c11be1a15ae6fe289a8c83"},
-    {url = "https://files.pythonhosted.org/packages/74/3c/e4b77f4f069aca2b6e35925db7a1aa6cb600dcb52fc3e962284640ca37f3/watchdog-3.0.0-py3-none-manylinux2014_ppc64.whl", hash = "sha256:5113334cf8cf0ac8cd45e1f8309a603291b614191c9add34d33075727a967709"},
-    {url = "https://files.pythonhosted.org/packages/75/fe/d9a37d8df76878853f68dd665ec6d2c7a984645de460164cb880a93ffe6b/watchdog-3.0.0-cp39-cp39-macosx_10_9_universal2.whl", hash = "sha256:7c5f84b5194c24dd573fa6472685b2a27cc5a17fe5f7b6fd40345378ca6812e3"},
-    {url = "https://files.pythonhosted.org/packages/7f/6e/7ca8ed16928d7b11da69372f55c64a09dce649d2b24b03f7063cd8683c4b/watchdog-3.0.0-cp38-cp38-macosx_10_9_universal2.whl", hash = "sha256:8ae9cda41fa114e28faf86cb137d751a17ffd0316d1c34ccf2235e8a84365c7f"},
-    {url = "https://files.pythonhosted.org/packages/84/ab/67001e62603bf2ea35ace40023f7c74f61e8b047160d6bb078373cec1a67/watchdog-3.0.0-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:7ade88d0d778b1b222adebcc0927428f883db07017618a5e684fd03b83342bd9"},
-    {url = "https://files.pythonhosted.org/packages/92/28/631872d7fbc45527037060db8c838b47a129a6c09d2297d6dddcfa283cf2/watchdog-3.0.0-py3-none-manylinux2014_aarch64.whl", hash = "sha256:0e06ab8858a76e1219e68c7573dfeba9dd1c0219476c5a44d5333b01d7e1743a"},
-    {url = "https://files.pythonhosted.org/packages/92/dd/42f47ffdfadff4c41b89c54163f323f875eb963bf90088e477c43b8f7b15/watchdog-3.0.0-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:a70a8dcde91be523c35b2bf96196edc5730edb347e374c7de7cd20c43ed95397"},
-    {url = "https://files.pythonhosted.org/packages/94/ce/70c65a6c4b0330129c402624d42f67ce82d6a0ba2036de67628aeffda3c1/watchdog-3.0.0-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:3aa7f6a12e831ddfe78cdd4f8996af9cf334fd6346531b16cec61c3b3c0d8da0"},
-    {url = "https://files.pythonhosted.org/packages/95/a6/d6ef450393dac5734c63c40a131f66808d2e6f59f6165ab38c98fbe4e6ec/watchdog-3.0.0.tar.gz", hash = "sha256:4d98a320595da7a7c5a18fc48cb633c2e73cda78f93cac2ef42d42bf609a33f9"},
-    {url = "https://files.pythonhosted.org/packages/9b/39/30bb3c2e4f8e89b5c60e98589acf5c5a001cb0efde249aa05d748d1734a2/watchdog-3.0.0-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:adfdeab2da79ea2f76f87eb42a3ab1966a5313e5a69a0213a3cc06ef692b0e96"},
-    {url = "https://files.pythonhosted.org/packages/9b/6e/ce8d124d03cd3f2941365d9c81d62e3afe43f2dc7e6e86274fa9c2ec2d5b/watchdog-3.0.0-py3-none-win_amd64.whl", hash = "sha256:4c9956d27be0bb08fc5f30d9d0179a855436e655f046d288e2bcc11adfae893c"},
-    {url = "https://files.pythonhosted.org/packages/ba/0c/cd0337069c468f22ef256e768ece74c78b511092f1004ab260268e1af4a9/watchdog-3.0.0-py3-none-win_ia64.whl", hash = "sha256:5d9f3a10e02d7371cd929b5d8f11e87d4bad890212ed3901f9b4d68767bee759"},
-    {url = "https://files.pythonhosted.org/packages/c0/a2/4e3230bdc1fb878b152a2c66aa941732776f4545bd68135d490591d66713/watchdog-3.0.0-py3-none-manylinux2014_armv7l.whl", hash = "sha256:d00e6be486affb5781468457b21a6cbe848c33ef43f9ea4a73b4882e5f188a44"},
-    {url = "https://files.pythonhosted.org/packages/dc/89/3a3ce6dd01807ff918aec3bbcabc92ed1a7edc5bb2266c720bb39fec1bec/watchdog-3.0.0-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:4f94069eb16657d2c6faada4624c39464f65c05606af50bb7902e036e3219be3"},
-    {url = "https://files.pythonhosted.org/packages/ea/76/bef1c6f6ac18041234a9f3e8bc995d611e255c44f10433bfaf255968c269/watchdog-3.0.0-pp38-pypy38_pp73-macosx_10_9_x86_64.whl", hash = "sha256:8f3ceecd20d71067c7fd4c9e832d4e22584318983cabc013dbf3f70ea95de346"},
-]
 "wcwidth 0.2.6" = [
     {url = "https://files.pythonhosted.org/packages/20/f4/c0584a25144ce20bfcf1aecd041768b8c762c1eb0aa77502a3f0baa83f11/wcwidth-0.2.6-py2.py3-none-any.whl", hash = "sha256:795b138f6875577cd91bba52baf9e445cd5118fd32723b460e30a0af30ea230e"},
     {url = "https://files.pythonhosted.org/packages/5e/5f/1e4bd82a9cc1f17b2c2361a2d876d4c38973a997003ba5eb400e8a932b6c/wcwidth-0.2.6.tar.gz", hash = "sha256:a5220780a404dbe3353789870978e472cfe477761f06ee55077256e509b156d0"},
 ]
 "webcolors 1.13" = [
     {url = "https://files.pythonhosted.org/packages/a1/fb/f95560c6a5d4469d9c49e24cf1b5d4d21ffab5608251c6020a965fb7791c/webcolors-1.13.tar.gz", hash = "sha256:c225b674c83fa923be93d235330ce0300373d02885cef23238813b0d5668304a"},
     {url = "https://files.pythonhosted.org/packages/d5/e1/3e9013159b4cbb71df9bd7611cbf90dc2c621c8aeeb677fc41dad72f2261/webcolors-1.13-py3-none-any.whl", hash = "sha256:29bc7e8752c0a1bd4a1f03c14d6e6a72e93d82193738fa860cbff59d0fcc11bf"},
```

### Comparing `framelink-0.2.0/pyproject.toml` & `framelink-0.2.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 requires-python = ">=3.8,<4.0"
 name = "framelink"
 description = ""
 readme = "README.md"
 dynamic = ["version"]
 
 dependencies = [
-    "networkx>=3.0"
+    "networkx>=3.0",
+    "typer[all]>=0.7.0",
 ]
 
 [project.optional-dependencies]
 viz = [
     "matplotlib>=3.7.1",
     "graphviz>=0.20.1",
     "pydot>=1.4.2"
@@ -35,14 +36,17 @@
     "polars<1.0.0,>=0.16.7",
     "pre-commit>=3.2.0",
     "pyment>=0.3.3",
     "pyarrow>=11.0.0",
     "jupyter>=1.0.0",
 ]
 
+[project.scripts]
+framelink = "framelink._cli:_app"
+
 [project.urls]
 github = "https://github.com/GitToby/framelink"
 
 [build-system]
 requires = ["setuptools>=45", "setuptools_scm[toml]>=6.2"]
 
 [tool.setuptools_scm]
```

### Comparing `framelink-0.2.0/src/framelink/_util.py` & `framelink-0.2.1/src/framelink/_util.py`

 * *Files identical despite different names*

### Comparing `framelink-0.2.0/src/framelink/core.py` & `framelink-0.2.1/src/framelink/core.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,32 +1,34 @@
+import contextlib
 import inspect
 import logging
 import textwrap
 import time
 from dataclasses import dataclass
 from graphlib import TopologicalSorter
 from pathlib import Path
-from typing import Any, Callable, Collection, Generator, Generic, Iterator, Optional, Protocol, TypeVar, Union
+from typing import Any, Callable, Collection, Generator, Generic, Iterator, Optional, Protocol, Union
 
 import networkx as nx
 import pydot
 
+from framelink._cli import CLI_CONTEXT
 from framelink._util import parse_model_src_for_internal_refs
+from framelink.storage.core import NoStorage
+from framelink.storage.interfaces import FramelinkStorage
+from framelink.types import F, T
 
 
 @dataclass
 class FramelinkSettings:
     """Settings to be applied by the"""
 
     persist_models_dir: Path = Path(__file__).parent.parent / "data"
     default_log_level: int = logging.WARNING
-
-
-T = TypeVar("T")  # usually one of pl.DataFrame, pl.DataFrame, pl.LazyFrame.. etc
-F = Callable[["FramelinkPipeline"], T]  # the definition of one of the models users will write
+    default_storage: FramelinkStorage = NoStorage()
 
 
 class _FramelinkComponent(Protocol):
     _name: str
 
     @property
     def __name__(self):
@@ -55,33 +57,31 @@
     A wrapper around a callable model that enables:
      - visibility onto the model DAG
      - caching of the model run
      - monitoring of run performance
      - adapters to run the model on various engines
     """
 
-    _callable: F[T]
+    callable: F[T]
     _graph_ref: nx.DiGraph
     call_perf: tuple[float, ...] = tuple()
 
     def __init__(
         self,
         model_func: F[T],
         graph: nx.DiGraph,
         pipeline_settings: FramelinkSettings,
         *,
-        persist_after_run: bool = False,
-        cache_result: bool = True,
         logging_level: Optional[int] = None,
+        store: FramelinkStorage[T] = NoStorage(),
     ):
         # These are more "model settings"
-        self.persist_after_run = persist_after_run
-        self.cache_result = cache_result
-        self._callable = model_func
+        self.callable = model_func
         self._name = model_func.__name__
+        self._store = store
 
         # These are the core attributes of the Model
         self._graph_ref = graph
         self._log = logging.getLogger(self.name)
         self._log.setLevel(logging_level if logging_level else pipeline_settings.default_log_level)
 
     def __repr__(self):
@@ -102,61 +102,64 @@
         :return: a set of models that depend on this model.
         """
         return set(self._graph_ref.successors(self))
 
     @property
     def docstring(self) -> Optional[str]:
         """ """
-        doc__ = self._callable.__doc__
+        doc__ = self.callable.__doc__
         return textwrap.dedent(doc__).strip() if doc__ else None
 
     @property
     def source(self) -> str:
         """ """
-        source__ = inspect.getsource(self._callable)
+        source__ = inspect.getsource(self.callable)
         source__ = textwrap.dedent(source__).strip()
         return source__
 
     @property
     def call_count(self) -> int:
         """return the numer of times this model has been called"""
         return len(self.call_perf)
 
     @property
     def perf_stats(self) -> tuple[float, ...]:
         """ """
         return self.call_perf
 
+    @contextlib.contextmanager
+    def _own_logging(self, ctx: "FramelinkPipeline"):
+        old_log, ctx.log = ctx.log, self._log
+        yield
+        ctx.log = old_log
+
     def build(self, ctx: "FramelinkPipeline") -> T:
         """
         Build the current model with the context of the pipeline.
         :param ctx: "FramelinkPipeline": framelink pipeline context
         """
-        old_log, ctx.log = ctx.log, self._log
-        res = self(ctx)
-        ctx.log = old_log
-        return res
+        with self._own_logging(ctx):
+            ctx.log.info(f"Building {self.name}...")
 
-    # todo: make async?
-    def __call__(self, ctx: "FramelinkPipeline") -> T:
-        ctx.log.info(f"Building {self.name}")
-        start_time = time.perf_counter()
-        res = self._callable(ctx)
-        # question: this timer is the whole stream, how can we isolate just the build time for this model?
-        build_time = time.perf_counter() - start_time
-        ctx.log.info(f"Finished building {self.name} in {build_time:.3}s")
-        self.call_perf += (build_time,)
+            start_time = time.perf_counter()
+            res = self._store(self, ctx)
+            # question: this timer is the whole stream, how can we isolate just the build time for this model?
+            build_time = time.perf_counter() - start_time
+            ctx.log.info(f"Finished building {self.name} in {build_time:.3}s")
+
+            # post build steps
+            self.call_perf += (build_time,)
         return res
 
-    def __key(self) -> tuple[str, Optional[str], bool]:
+    def __key(self) -> tuple[str, Optional[str]]:
         """
         The uniqueness of a Model should be defined as its config and execution. This is used to determine the cache
         settings for the model when it is run
         """
-        return self.name, self.source, self.persist_after_run
+        return self.name, self.source
 
 
 class FramelinkPipeline(_FramelinkComponent):
     """The core class for building DAGs of models and producing links of the results.
 
     Each model linked to the pipeline will have context onto their upstream and downstream dependencies.
     """
@@ -171,14 +174,15 @@
         self._name = name
         self._models = dict()
         self.graph = nx.DiGraph()
         self.settings = settings
         self._log = logging.getLogger(self.name)
         self._log.setLevel(settings.default_log_level)
         self.log = self._log
+        CLI_CONTEXT.fl_pipelines[self._name] = self
 
     def __repr__(self):
         return f"<{self.name} with {len(self)} models at {self.__loc__}>"
 
     @property
     def model_names(self) -> list[str]:
         """Return a list of model names registered to this pipeline"""
@@ -200,39 +204,37 @@
         """
         # question: is there a better graph layout
         # pos = nx.multipartite_layout(self.graph)
         pos = nx.planar_layout(self.graph)
         return nx.draw_networkx(self.graph, pos)
 
     def model(
-        self, *, persist_after_run=False, cache_result=True, logging_level=None
+        self, *, logging_level=None, storage: Optional[FramelinkStorage[T]] = None
     ) -> Callable[[F[T]], FramelinkModel[T]]:
-        """Annotation to register a model to the pypeline.
+        """
+        Annotation to register a model to the framelink pipeline.
 
-        :param persist_after_run: Write the file to disk after running this model. The approach to writing the model is
-            defined in the :FramelinkSettings: (Default value = False)
-        :param cache_result:  (Default value = True)
         :param logging_level: Sets the logging level specifically for this model. If no level is passed it will default
             to the default level as per the pipelines settings.
+        :param storage: Sets the persistence approach used when storing the model.
         """
+        if storage:
+            model_store_unwrapped = storage
+        else:
+            model_store_unwrapped = self.settings.default_storage
 
         def _decorator(func: F[T]) -> FramelinkModel[T]:
             """Internal wrapping of the model function to produce the metadata about the model.
 
             :param func: "PYPE_MODEL": the callable function that defines the model
             :returns: the wrapped model with all the extra pieces
             """
 
             model_wrapper: FramelinkModel = FramelinkModel(
-                func,
-                self.graph,
-                self.settings,
-                persist_after_run=persist_after_run,
-                cache_result=cache_result,
-                logging_level=logging_level,
+                func, self.graph, self.settings, logging_level=logging_level, store=model_store_unwrapped
             )
             self._log.info(f"Registering model '{model_wrapper.name}'")
 
             # we need to keep a ref to the underlying graph to access the models when we ask for them via
             # `ref()` or `build()`
             assert model_wrapper.name not in self._models.keys(), f"Model already registered under {model_wrapper.name}"
             self._models[model_wrapper.name] = model_wrapper
@@ -280,20 +282,21 @@
         return model_wrapper.build(self)
 
     def build(self, model_name: Union[FramelinkModel[T], str]) -> T:
         """Building models is just proxied through to ref. Each build command should build only the given node in the
          graph up to the nearest cache or persisted cache.
 
         :param model_name: "PYPE_MODEL": the model to build in the context of this pipeline.
+        :param overrides: A mapping of models whos result should be overridden for this build.
         """
         return self.ref(model_name)
 
     def topological_sorted_nodes(self) -> Generator[tuple[FramelinkModel, ...], None, None]:
         """
-        This implementation is more parralel aware than the networkx implementation/
+        This implementation is more parallel aware than the networkx implementation/
 
         Basically a repeatable version of the example at https://docs.python.org/3/library/graphlib.html
         :return:
         """
         topological_sorter: TopologicalSorter = TopologicalSorter()
         for node in self._models.values():
             topological_sorter.add(node, *node.upstreams)
```

### Comparing `framelink-0.2.0/src/framelink.egg-info/PKG-INFO` & `framelink-0.2.1/src/framelink.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: framelink
-Version: 0.2.0
+Version: 0.2.1
 Author-email: Toby Devlin <toby@tobydevlin.com>
 Project-URL: github, https://github.com/GitToby/framelink
 Requires-Python: <4.0,>=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: viz
 Provides-Extra: dev
 
 ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/gittoby/framelink/lint_test_build.yml)
 ![GitHub Release Date](https://img.shields.io/github/release-date/GitToby/framelink)
 
-Famelink is a simple wrapper that will provide context into pandas, polars and other Dataframe engines. See roadmap
+Framelink is a simple wrapper that will provide context into pandas, polars and other Dataframe engines. See roadmap
 below for future goals of the project.
 
 **This project is still in prerelease, consider the API unstable. Any usage should be pinned.**
 
 ```bash
 pip install framelink
 ```
@@ -33,55 +33,63 @@
 
 ## Concepts
 
 - A **Pipeline** is a DAG of _models_ that can be executed in a particular way.
 - A **Model** is a definition of sourcing data and, potentially, a transform. It's an ETL in its most basic form.
 - A **Frame** is a result of a _model_ run.
 
+## Features
+- [x] Model links & DAG + diagramming
+- [x] Context logging per model
+- [x] Diagramming and tracking of the model DAG
+- [x] Caches and auto-persistence
+- [ ] Dynamic sourcing for models
+- [x] Cli to run a project
+
 ## Example
 
 ```python
-import os
 from pathlib import Path
 
 import pandas as pd
 import polars as pl
 
 from framelink.core import FramelinkPipeline, FramelinkSettings
+from framelink.storage.core import PickleStorage, NoStorage
 
 settings = FramelinkSettings(
-    persist_models_dir=Path(os.getcwd()) / "data"
+  default_storage=PickleStorage(Path(__file__).parent / "data")
 )
 
 pipeline = FramelinkPipeline(settings=settings)
 
 
 @pipeline.model()
 def src_frame_1(_: FramelinkPipeline) -> pd.DataFrame:
-    return pd.DataFrame(data={
-        "name": ["amy", "peter"],
-        "age": [31, 12],
-    })
+  return pd.DataFrame(data={
+    "name": ["amy", "peter"],
+    "age": [31, 12],
+  })
 
 
-@pipeline.model()
+@pipeline.model(storage=NoStorage())
 def src_frame_2(_: FramelinkPipeline) -> pd.DataFrame:
-    return pd.DataFrame(data={
-        "name": ["amy", "peter", "helen"],
-        "fave_food": ["oranges", "chocolate", "water"],
-    })
+  return pd.DataFrame(data={
+    "name": ["amy", "peter", "helen"],
+    "fave_food": ["oranges", "chocolate", "water"],
+  })
 
 
 @pipeline.model()
 def merge_model(ctx: FramelinkPipeline) -> pl.DataFrame:
-    res_1 = ctx.ref(src_frame_1)
-    res_2 = ctx.ref(src_frame_2)
-    key = "name"
-    ctx.log.info(f"Merging both sources on {key}")
-    return pl.from_pandas(res_1).join(pl.from_pandas(res_2), on=key)
+  res_1 = ctx.ref(src_frame_1)
+  res_2 = ctx.ref(src_frame_2)
+  key = "name"
+  ctx.log.info(f"Merging both sources on {key}")
+  return pl.from_pandas(res_1).join(pl.from_pandas(res_2), on=key)
 
 
 # build with implicit context
 r_1 = pipeline.build(merge_model)
 print(r_1)
 # shape: (2, 3)
 # ┌───────┬─────┬───────────┐
@@ -121,18 +129,16 @@
 - [x] Diagramming and tracking of the model DAG
 
 ### v0.3.0
 
 - [ ] Cleaner graph results
 - [ ] Merging of multiple framelink pipelines enabling
 - [ ] Orchestration passthrough and local execution.
+- [x] Caches and auto-persistence
+- [x] Dynamic sourcing for models
+- [ ] model overrides for CLI and python runtimes.
+- [x] Cli to run a project
 
 ### v0.4.0
 
-- [ ] Caches and auto-persistence
-- [ ] Dynamic sourcing for models
-- [ ] Cli to run a project
-
-### v0.5.0
-
 - [ ] SQL models & dbt, sqlmesh compatability
 - [ ] Open Tracing integration
```

### Comparing `framelink-0.2.0/tests/conftest.py` & `framelink-0.2.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `framelink-0.2.0/tests/core/test_dag.py` & `framelink-0.2.1/tests/core/test_dag.py`

 * *Files identical despite different names*

### Comparing `framelink-0.2.0/tests/core/test_logging.py` & `framelink-0.2.1/tests/core/test_logging.py`

 * *Files identical despite different names*

### Comparing `framelink-0.2.0/tests/core/test_model.py` & `framelink-0.2.1/tests/core/test_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,18 @@
-from typing import Callable
-
 import pandas as pd
 import polars as pl
 import pytest
 
 from framelink.core import FramelinkModel, FramelinkPipeline
 
 
 def test_model_registration(empty_framelink):
     pipeline = empty_framelink
 
-    @pipeline.model(persist_after_run=False, cache_result=True)
+    @pipeline.model()
     def src_frame(_: FramelinkPipeline) -> pl.LazyFrame:
         """
         Im a docstring!
         """
         return pl.LazyFrame()
 
     # naming things
@@ -23,16 +21,14 @@
 
     # metadata of model
     assert "Im a docstring!" in src_frame.docstring
     assert src_frame.call_count == 0
     assert src_frame.perf_stats == tuple()
 
     # model settings
-    assert src_frame.persist_after_run is False
-    assert src_frame.cache_result is True
     assert src_frame._log is not None
 
     # association to pipeline
     assert src_frame in pipeline
     assert src_frame.name in pipeline.model_names
 
 
@@ -136,25 +132,22 @@
     pipeline, src_frame = initial_framelink
 
     @pipeline.model()
     def head_model(ctx: FramelinkPipeline) -> pd.DataFrame:
         df_out = ctx.ref(src_frame).head()
         return df_out
 
-    assert isinstance(head_model, Callable)
     assert isinstance(head_model, FramelinkModel)
 
     def head_model_2(ctx: FramelinkPipeline) -> pd.DataFrame:
         df_out = ctx.ref(src_frame).head()
         return df_out
 
-    assert isinstance(head_model_2, Callable)
     assert not isinstance(head_model_2, FramelinkModel)
     head_model_2_wrapped = pipeline.model()(head_model_2)
-    assert isinstance(head_model_2, Callable)
     assert isinstance(head_model_2_wrapped, FramelinkModel)
 
 
 def test_get_lookups(initial_framelink):
     pipeline, src_frame = initial_framelink
 
     @pipeline.model()
```

### Comparing `framelink-0.2.0/tests/core/test_model_parsing.py` & `framelink-0.2.1/tests/core/test_model_parsing.py`

 * *Files identical despite different names*

### Comparing `framelink-0.2.0/tests/core/test_pipeline_metas.py` & `framelink-0.2.1/tests/core/test_pipeline_metas.py`

 * *Files identical despite different names*

