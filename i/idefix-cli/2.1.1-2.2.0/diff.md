# Comparing `tmp/idefix_cli-2.1.1.tar.gz` & `tmp/idefix_cli-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idefix_cli-2.1.1.tar", last modified: Thu May  4 16:24:17 2023, max compression
+gzip compressed data, was "idefix_cli-2.2.0.tar", last modified: Sat May  6 10:39:36 2023, max compression
```

## Comparing `idefix_cli-2.1.1.tar` & `idefix_cli-2.2.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:24:17.624853 idefix_cli-2.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-04 16:24:05.000000 idefix_cli-2.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-05-04 16:24:17.624853 idefix_cli-2.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-05-04 16:24:05.000000 idefix_cli-2.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:24:17.616853 idefix_cli-2.1.1/idefix_cli/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-04 16:24:05.000000 idefix_cli-2.1.1/idefix_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5593 2023-05-04 16:24:05.000000 idefix_cli-2.1.1/idefix_cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-05-04 16:24:05.000000 idefix_cli-2.1.1/idefix_cli/_backports.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:24:17.620853 idefix_cli-2.1.1/idefix_cli/_commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 16:24:05.000000 idefix_cli-2.1.1/idefix_cli/_commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-05-04 16:24:05.000000 idefix_cli-2.1.1/idefix_cli/_commands/clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-05-04 16:24:05.000000 idefix_cli-2.1.1/idefix_cli/_commands/clone.py
--rw-r--r--   0 runner    (1001) docker     (123)     9024 2023-05-04 16:24:05.000000 idefix_cli-2.1.1/idefix_cli/_commands/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-05-04 16:24:05.000000 idefix_cli-2.1.1/idefix_cli/_commands/read.py
--rw-r--r--   0 runner    (1001) docker     (123)    11781 2023-05-04 16:24:05.000000 idefix_cli-2.1.1/idefix_cli/_commands/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-05-04 16:24:05.000000 idefix_cli-2.1.1/idefix_cli/_commands/stamp.py
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-05-04 16:24:05.000000 idefix_cli-2.1.1/idefix_cli/_commands/switch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-05-04 16:24:05.000000 idefix_cli-2.1.1/idefix_cli/_commands/write.py
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-04 16:24:05.000000 idefix_cli-2.1.1/idefix_cli/_theme.py
--rw-r--r--   0 runner    (1001) docker     (123)    13406 2023-05-04 16:24:05.000000 idefix_cli-2.1.1/idefix_cli/lib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:24:17.616853 idefix_cli-2.1.1/idefix_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-05-04 16:24:17.000000 idefix_cli-2.1.1/idefix_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-05-04 16:24:17.000000 idefix_cli-2.1.1/idefix_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 16:24:17.000000 idefix_cli-2.1.1/idefix_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-04 16:24:17.000000 idefix_cli-2.1.1/idefix_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-04 16:24:17.000000 idefix_cli-2.1.1/idefix_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-04 16:24:17.000000 idefix_cli-2.1.1/idefix_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-05-04 16:24:05.000000 idefix_cli-2.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 16:24:17.624853 idefix_cli-2.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:24:17.620853 idefix_cli-2.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3724 2023-05-04 16:24:05.000000 idefix_cli-2.1.1/tests/test_app_structure.py
--rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-05-04 16:24:05.000000 idefix_cli-2.1.1/tests/test_clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-05-04 16:24:05.000000 idefix_cli-2.1.1/tests/test_clone.py
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-05-04 16:24:05.000000 idefix_cli-2.1.1/tests/test_commons.py
--rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-05-04 16:24:05.000000 idefix_cli-2.1.1/tests/test_conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-05-04 16:24:05.000000 idefix_cli-2.1.1/tests/test_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-05-04 16:24:05.000000 idefix_cli-2.1.1/tests/test_read.py
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-05-04 16:24:05.000000 idefix_cli-2.1.1/tests/test_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-05-04 16:24:05.000000 idefix_cli-2.1.1/tests/test_stamp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-05-04 16:24:05.000000 idefix_cli-2.1.1/tests/test_ux.py
--rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-05-04 16:24:05.000000 idefix_cli-2.1.1/tests/test_write.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 10:39:36.992097 idefix_cli-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-06 10:39:26.000000 idefix_cli-2.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-05-06 10:39:36.992097 idefix_cli-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-05-06 10:39:26.000000 idefix_cli-2.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 10:39:36.988097 idefix_cli-2.2.0/idefix_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-06 10:39:26.000000 idefix_cli-2.2.0/idefix_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5593 2023-05-06 10:39:26.000000 idefix_cli-2.2.0/idefix_cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-05-06 10:39:26.000000 idefix_cli-2.2.0/idefix_cli/_backports.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 10:39:36.988097 idefix_cli-2.2.0/idefix_cli/_commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 10:39:26.000000 idefix_cli-2.2.0/idefix_cli/_commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-05-06 10:39:26.000000 idefix_cli-2.2.0/idefix_cli/_commands/clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-05-06 10:39:26.000000 idefix_cli-2.2.0/idefix_cli/_commands/clone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9024 2023-05-06 10:39:26.000000 idefix_cli-2.2.0/idefix_cli/_commands/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-05-06 10:39:26.000000 idefix_cli-2.2.0/idefix_cli/_commands/read.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12694 2023-05-06 10:39:26.000000 idefix_cli-2.2.0/idefix_cli/_commands/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-05-06 10:39:26.000000 idefix_cli-2.2.0/idefix_cli/_commands/stamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-05-06 10:39:26.000000 idefix_cli-2.2.0/idefix_cli/_commands/switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-05-06 10:39:26.000000 idefix_cli-2.2.0/idefix_cli/_commands/write.py
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-06 10:39:26.000000 idefix_cli-2.2.0/idefix_cli/_theme.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13406 2023-05-06 10:39:26.000000 idefix_cli-2.2.0/idefix_cli/lib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 10:39:36.988097 idefix_cli-2.2.0/idefix_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-05-06 10:39:36.000000 idefix_cli-2.2.0/idefix_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-05-06 10:39:36.000000 idefix_cli-2.2.0/idefix_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 10:39:36.000000 idefix_cli-2.2.0/idefix_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-06 10:39:36.000000 idefix_cli-2.2.0/idefix_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-06 10:39:36.000000 idefix_cli-2.2.0/idefix_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-06 10:39:36.000000 idefix_cli-2.2.0/idefix_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-05-06 10:39:26.000000 idefix_cli-2.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 10:39:36.992097 idefix_cli-2.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 10:39:36.992097 idefix_cli-2.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3724 2023-05-06 10:39:26.000000 idefix_cli-2.2.0/tests/test_app_structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-05-06 10:39:26.000000 idefix_cli-2.2.0/tests/test_clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-05-06 10:39:26.000000 idefix_cli-2.2.0/tests/test_clone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-05-06 10:39:26.000000 idefix_cli-2.2.0/tests/test_commons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-05-06 10:39:26.000000 idefix_cli-2.2.0/tests/test_conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-05-06 10:39:26.000000 idefix_cli-2.2.0/tests/test_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-05-06 10:39:26.000000 idefix_cli-2.2.0/tests/test_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-05-06 10:39:26.000000 idefix_cli-2.2.0/tests/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-05-06 10:39:26.000000 idefix_cli-2.2.0/tests/test_stamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-05-06 10:39:26.000000 idefix_cli-2.2.0/tests/test_ux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-05-06 10:39:26.000000 idefix_cli-2.2.0/tests/test_write.py
```

### Comparing `idefix_cli-2.1.1/LICENSE` & `idefix_cli-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.1.1/PKG-INFO` & `idefix_cli-2.2.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idefix_cli
-Version: 2.1.1
+Version: 2.2.0
 Summary: A CLI to automate mundane tasks with Idefix
 Author: C.M.T. Robert
 License: GPL-3.0
 Project-URL: Homepage, https://github.com/neutrinoceros/idefix_cli
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -20,16 +20,16 @@
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/neutrinoceros/idefix_cli/main.svg)](https://results.pre-commit.ci/badge/github/neutrinoceros/idefix_cli/main.svg)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)
 
 # `idefix_cli`
 
 `idefix_cli` is command line framework to facilitate working with
-[Idefix](https://gricad-gitlab.univ-grenoble-alpes.fr/lesurg/idefix-public),
-written by Geoffroy Lesur et al.
+[Idefix](https://github.com/idefix-code/idefix), written by
+[Lesur et al](https://ui.adsabs.harvard.edu/abs/2023arXiv230413746L/abstract).
 
 It defines a `idfx` command namespace, ships with a collection of common helper
 script (`idfx conf`, `idfx run`, ...), and can be extended to include arbitrary
 helper scripts.
 
 
 ## Installation
```

### Comparing `idefix_cli-2.1.1/README.md` & `idefix_cli-2.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/neutrinoceros/idefix_cli/main.svg)](https://results.pre-commit.ci/badge/github/neutrinoceros/idefix_cli/main.svg)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)
 
 # `idefix_cli`
 
 `idefix_cli` is command line framework to facilitate working with
-[Idefix](https://gricad-gitlab.univ-grenoble-alpes.fr/lesurg/idefix-public),
-written by Geoffroy Lesur et al.
+[Idefix](https://github.com/idefix-code/idefix), written by
+[Lesur et al](https://ui.adsabs.harvard.edu/abs/2023arXiv230413746L/abstract).
 
 It defines a `idfx` command namespace, ships with a collection of common helper
 script (`idfx conf`, `idfx run`, ...), and can be extended to include arbitrary
 helper scripts.
 
 
 ## Installation
```

### Comparing `idefix_cli-2.1.1/idefix_cli/__main__.py` & `idefix_cli-2.2.0/idefix_cli/__main__.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.1.1/idefix_cli/_backports.py` & `idefix_cli-2.2.0/idefix_cli/_backports.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.1.1/idefix_cli/_commands/clean.py` & `idefix_cli-2.2.0/idefix_cli/_commands/clean.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.1.1/idefix_cli/_commands/clone.py` & `idefix_cli-2.2.0/idefix_cli/_commands/clone.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.1.1/idefix_cli/_commands/conf.py` & `idefix_cli-2.2.0/idefix_cli/_commands/conf.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.1.1/idefix_cli/_commands/read.py` & `idefix_cli-2.2.0/idefix_cli/_commands/read.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.1.1/idefix_cli/_commands/run.py` & `idefix_cli-2.2.0/idefix_cli/_commands/run.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 import os
 import re
 import subprocess
 import sys
 from copy import deepcopy
 from enum import auto
+from math import prod
 from multiprocessing import cpu_count
 from pathlib import Path
 from tempfile import NamedTemporaryFile
 from time import sleep, time
 from typing import Final
 
 import inifix
@@ -86,14 +87,42 @@
                         complete = True
                         break
             last_edit = new_edit
         sleep(0.01)
     return -1
 
 
+def get_command(
+    inputfile: str, *, nproc: int, idefix_args: tuple[str, ...]
+) -> list[str]:
+    cmd = ["./idefix", "-i", inputfile, *idefix_args]
+
+    if nproc < 0 and "-dec" in idefix_args:
+        # try to guess the number of processes
+        i0 = idefix_args.index("-dec")
+        dec_args: list[int] = []
+        for i in range(i0 + 1, len(idefix_args)):
+            try:
+                dec_args.append(int(idefix_args[i]))
+            except ValueError:
+                break
+        if dec_args:
+            nproc = prod(dec_args)
+        else:
+            print_warning(
+                "Couldn't parse -dec parameters, "
+                "this will likely result in idefix crashing at startup time "
+                "(if it doesn't, please report this)"
+            )
+
+    if nproc > 1:
+        cmd = ["mpirun", "-n", str(nproc), *cmd]
+    return cmd
+
+
 class RebuildMode(StrEnum):
     ALWAYS = auto()
     PROMPT = auto()
 
 
 # known end messages in Idefix
 KNOWN_SUCCESS: Final = (
@@ -152,18 +181,19 @@
         type=float,
         help="override TimeIntegrator.first_dt",
     )
     parser.add_argument(
         "--nproc",
         action="store",
         type=int,
-        default=1,
+        default=-1,
         help=(
             "run idefix in parallel over selected number of ALU. "
-            "Requires the code to be configured for MPI."
+            "Requires the code to be configured for MPI. "
+            "This parameter can be left unspecified if -dec is passed."
         ),
     )
     parser.add_argument(
         "--times",
         dest="multiplier",
         type=int,
         default=None,
@@ -176,15 +206,15 @@
     directory: str = ".",
     inifile: str = "idefix.ini",
     tstop: float | None = None,
     duration: float | None = None,
     time_step: float | None = None,
     one_step: list[str] | None = None,
     multiplier: int | None = None,
-    nproc: int = 1,
+    nproc: int = -1,
 ) -> int:
     if multiplier is not None:
         if one_step is None:
             print_err(
                 "--times argument is invalid if --one/--one-step isn't passed too"
             )
             return 1
@@ -334,18 +364,15 @@
         tmp_inifile = NamedTemporaryFile()
         with open(tmp_inifile.name, "wb") as fh:
             inifix.dump(conf, fh)
         inputfile = tmp_inifile.name
     else:
         inputfile = str(pinifile.relative_to(d.resolve()))
 
-    cmd = ["./idefix", "-i", inputfile, *unknown_args]
-
-    if nproc > 1:
-        cmd = ["mpirun", "-n", str(nproc), *cmd]
+    cmd = get_command(inputfile, nproc=nproc, idefix_args=unknown_args)
 
     print_subcommand(cmd, loc=d)
     with chdir(d):
         ret = spawn_idefix(cmd, step_count=multiplier)
 
     if ret < 0:
         # special retcodes from spawn_idefix
```

### Comparing `idefix_cli-2.1.1/idefix_cli/_commands/stamp.py` & `idefix_cli-2.2.0/idefix_cli/_commands/stamp.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.1.1/idefix_cli/_commands/switch.py` & `idefix_cli-2.2.0/idefix_cli/_commands/switch.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.1.1/idefix_cli/_commands/write.py` & `idefix_cli-2.2.0/idefix_cli/_commands/write.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.1.1/idefix_cli/lib.py` & `idefix_cli-2.2.0/idefix_cli/lib.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.1.1/idefix_cli.egg-info/PKG-INFO` & `idefix_cli-2.2.0/idefix_cli.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idefix-cli
-Version: 2.1.1
+Version: 2.2.0
 Summary: A CLI to automate mundane tasks with Idefix
 Author: C.M.T. Robert
 License: GPL-3.0
 Project-URL: Homepage, https://github.com/neutrinoceros/idefix_cli
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -20,16 +20,16 @@
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/neutrinoceros/idefix_cli/main.svg)](https://results.pre-commit.ci/badge/github/neutrinoceros/idefix_cli/main.svg)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)
 
 # `idefix_cli`
 
 `idefix_cli` is command line framework to facilitate working with
-[Idefix](https://gricad-gitlab.univ-grenoble-alpes.fr/lesurg/idefix-public),
-written by Geoffroy Lesur et al.
+[Idefix](https://github.com/idefix-code/idefix), written by
+[Lesur et al](https://ui.adsabs.harvard.edu/abs/2023arXiv230413746L/abstract).
 
 It defines a `idfx` command namespace, ships with a collection of common helper
 script (`idfx conf`, `idfx run`, ...), and can be extended to include arbitrary
 helper scripts.
 
 
 ## Installation
```

### Comparing `idefix_cli-2.1.1/idefix_cli.egg-info/SOURCES.txt` & `idefix_cli-2.2.0/idefix_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.1.1/pyproject.toml` & `idefix_cli-2.2.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "idefix_cli"
-version = "2.1.1"
+version = "2.2.0"
 description = "A CLI to automate mundane tasks with Idefix"
 authors = [
     { name = "C.M.T. Robert" },
 ]
 classifiers = [
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Programming Language :: Python :: 3",
```

### Comparing `idefix_cli-2.1.1/tests/test_app_structure.py` & `idefix_cli-2.2.0/tests/test_app_structure.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.1.1/tests/test_clean.py` & `idefix_cli-2.2.0/tests/test_clean.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.1.1/tests/test_clone.py` & `idefix_cli-2.2.0/tests/test_clone.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.1.1/tests/test_commons.py` & `idefix_cli-2.2.0/tests/test_commons.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.1.1/tests/test_conf.py` & `idefix_cli-2.2.0/tests/test_conf.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.1.1/tests/test_read.py` & `idefix_cli-2.2.0/tests/test_read.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.1.1/tests/test_run.py` & `idefix_cli-2.2.0/tests/test_run.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.1.1/tests/test_stamp.py` & `idefix_cli-2.2.0/tests/test_stamp.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.1.1/tests/test_ux.py` & `idefix_cli-2.2.0/tests/test_ux.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.1.1/tests/test_write.py` & `idefix_cli-2.2.0/tests/test_write.py`

 * *Files identical despite different names*

