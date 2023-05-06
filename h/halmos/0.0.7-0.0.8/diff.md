# Comparing `tmp/halmos-0.0.7.tar.gz` & `tmp/halmos-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "halmos-0.0.7.tar", last modified: Wed Mar 22 04:47:23 2023, max compression
+gzip compressed data, was "halmos-0.0.8.tar", last modified: Sat May  6 03:04:02 2023, max compression
```

## Comparing `halmos-0.0.7.tar` & `halmos-0.0.8.tar`

### file list

```diff
@@ -1,62 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 04:47:23.874739 halmos-0.0.7/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 04:47:23.862739 halmos-0.0.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 04:47:23.866739 halmos-0.0.7/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-03-22 04:47:09.000000 halmos-0.0.7/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-03-22 04:47:09.000000 halmos-0.0.7/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 04:47:23.866739 halmos-0.0.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-03-22 04:47:09.000000 halmos-0.0.7/.github/workflows/codeql.yml
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-03-22 04:47:09.000000 halmos-0.0.7/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-03-22 04:47:09.000000 halmos-0.0.7/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-03-22 04:47:09.000000 halmos-0.0.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-03-22 04:47:09.000000 halmos-0.0.7/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-03-22 04:47:09.000000 halmos-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4542 2023-03-22 04:47:23.874739 halmos-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-03-22 04:47:09.000000 halmos-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 04:47:23.866739 halmos-0.0.7/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-03-22 04:47:09.000000 halmos-0.0.7/examples/foundry.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 04:47:23.866739 halmos-0.0.7/examples/src/
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-03-22 04:47:09.000000 halmos-0.0.7/examples/src/Example.sol
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 04:47:23.866739 halmos-0.0.7/examples/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-03-22 04:47:09.000000 halmos-0.0.7/examples/test/Example.t.sol
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-03-22 04:47:09.000000 halmos-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-03-22 04:47:09.000000 halmos-0.0.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-22 04:47:23.874739 halmos-0.0.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 04:47:23.862739 halmos-0.0.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 04:47:23.866739 halmos-0.0.7/src/halmos/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-03-22 04:47:09.000000 halmos-0.0.7/src/halmos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21684 2023-03-22 04:47:09.000000 halmos-0.0.7/src/halmos/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-03-22 04:47:09.000000 halmos-0.0.7/src/halmos/byte2op.py
--rw-r--r--   0 runner    (1001) docker     (123)    53359 2023-03-22 04:47:09.000000 halmos-0.0.7/src/halmos/sevm.py
--rw-r--r--   0 runner    (1001) docker     (123)    29746 2023-03-22 04:47:09.000000 halmos-0.0.7/src/halmos/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 04:47:23.870739 halmos-0.0.7/src/halmos.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4542 2023-03-22 04:47:23.000000 halmos-0.0.7/src/halmos.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-03-22 04:47:23.000000 halmos-0.0.7/src/halmos.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-22 04:47:23.000000 halmos-0.0.7/src/halmos.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-03-22 04:47:23.000000 halmos-0.0.7/src/halmos.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-03-22 04:47:23.000000 halmos-0.0.7/src/halmos.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-22 04:47:23.000000 halmos-0.0.7/src/halmos.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 04:47:23.870739 halmos-0.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-03-22 04:47:09.000000 halmos-0.0.7/tests/foundry.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 04:47:23.870739 halmos-0.0.7/tests/src/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-03-22 04:47:09.000000 halmos-0.0.7/tests/src/Const.sol
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-03-22 04:47:09.000000 halmos-0.0.7/tests/src/Counter.sol
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-03-22 04:47:09.000000 halmos-0.0.7/tests/src/Create.sol
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-03-22 04:47:09.000000 halmos-0.0.7/tests/src/List.sol
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-03-22 04:47:09.000000 halmos-0.0.7/tests/src/SignExtend.sol
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-03-22 04:47:09.000000 halmos-0.0.7/tests/src/Storage.sol
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 04:47:23.874739 halmos-0.0.7/tests/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-03-22 04:47:09.000000 halmos-0.0.7/tests/test/Arith.t.sol
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-03-22 04:47:09.000000 halmos-0.0.7/tests/test/Const.t.sol
--rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-03-22 04:47:09.000000 halmos-0.0.7/tests/test/Counter.t.sol
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-03-22 04:47:09.000000 halmos-0.0.7/tests/test/Create.t.sol
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-03-22 04:47:09.000000 halmos-0.0.7/tests/test/Foundry.t.sol
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-03-22 04:47:09.000000 halmos-0.0.7/tests/test/Library.t.sol
--rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-03-22 04:47:09.000000 halmos-0.0.7/tests/test/List.t.sol
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-03-22 04:47:09.000000 halmos-0.0.7/tests/test/Opcode.t.sol
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-03-22 04:47:09.000000 halmos-0.0.7/tests/test/Setup.t.sol
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-03-22 04:47:09.000000 halmos-0.0.7/tests/test/SetupPlus.t.sol
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-03-22 04:47:09.000000 halmos-0.0.7/tests/test/SignExtend.t.sol
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-03-22 04:47:09.000000 halmos-0.0.7/tests/test/Storage.t.sol
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-03-22 04:47:09.000000 halmos-0.0.7/tests/test/Struct.t.sol
--rw-r--r--   0 runner    (1001) docker     (123)     6091 2023-03-22 04:47:09.000000 halmos-0.0.7/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6019 2023-03-22 04:47:09.000000 halmos-0.0.7/tests/test_sevm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:04:02.497822 halmos-0.0.8/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:04:02.493822 halmos-0.0.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:04:02.493822 halmos-0.0.8/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-06 03:03:54.000000 halmos-0.0.8/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-05-06 03:03:54.000000 halmos-0.0.8/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:04:02.493822 halmos-0.0.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-05-06 03:03:54.000000 halmos-0.0.8/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-06 03:03:54.000000 halmos-0.0.8/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-05-06 03:03:54.000000 halmos-0.0.8/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-06 03:03:54.000000 halmos-0.0.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-06 03:03:54.000000 halmos-0.0.8/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-06 03:03:54.000000 halmos-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4542 2023-05-06 03:04:02.497822 halmos-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-05-06 03:03:54.000000 halmos-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:04:02.493822 halmos-0.0.8/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-06 03:03:54.000000 halmos-0.0.8/examples/foundry.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:04:02.493822 halmos-0.0.8/examples/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-05-06 03:03:54.000000 halmos-0.0.8/examples/src/Example.sol
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:04:02.493822 halmos-0.0.8/examples/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-05-06 03:03:54.000000 halmos-0.0.8/examples/test/Example.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-05-06 03:03:54.000000 halmos-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-06 03:03:54.000000 halmos-0.0.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 03:04:02.497822 halmos-0.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:04:02.493822 halmos-0.0.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:04:02.493822 halmos-0.0.8/src/halmos/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-06 03:03:54.000000 halmos-0.0.8/src/halmos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23618 2023-05-06 03:03:54.000000 halmos-0.0.8/src/halmos/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-05-06 03:03:54.000000 halmos-0.0.8/src/halmos/byte2op.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-05-06 03:03:54.000000 halmos-0.0.8/src/halmos/cheatcodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59143 2023-05-06 03:03:54.000000 halmos-0.0.8/src/halmos/sevm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28892 2023-05-06 03:03:54.000000 halmos-0.0.8/src/halmos/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:04:02.493822 halmos-0.0.8/src/halmos.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4542 2023-05-06 03:04:02.000000 halmos-0.0.8/src/halmos.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-05-06 03:04:02.000000 halmos-0.0.8/src/halmos.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 03:04:02.000000 halmos-0.0.8/src/halmos.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-06 03:04:02.000000 halmos-0.0.8/src/halmos.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-06 03:04:02.000000 halmos-0.0.8/src/halmos.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-06 03:04:02.000000 halmos-0.0.8/src/halmos.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:04:02.493822 halmos-0.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-06 03:03:54.000000 halmos-0.0.8/tests/foundry.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:04:02.497822 halmos-0.0.8/tests/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-06 03:03:54.000000 halmos-0.0.8/tests/src/Const.sol
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-05-06 03:03:54.000000 halmos-0.0.8/tests/src/Counter.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-06 03:03:54.000000 halmos-0.0.8/tests/src/Create.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-06 03:03:54.000000 halmos-0.0.8/tests/src/List.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-06 03:03:54.000000 halmos-0.0.8/tests/src/SignExtend.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-05-06 03:03:54.000000 halmos-0.0.8/tests/src/Storage.sol
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:04:02.497822 halmos-0.0.8/tests/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-06 03:03:54.000000 halmos-0.0.8/tests/test/Arith.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-06 03:03:54.000000 halmos-0.0.8/tests/test/Block.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-06 03:03:54.000000 halmos-0.0.8/tests/test/Const.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-05-06 03:03:54.000000 halmos-0.0.8/tests/test/Counter.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-06 03:03:54.000000 halmos-0.0.8/tests/test/Create.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-05-06 03:03:54.000000 halmos-0.0.8/tests/test/Deal.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-05-06 03:03:54.000000 halmos-0.0.8/tests/test/Foundry.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-05-06 03:03:54.000000 halmos-0.0.8/tests/test/Invalid.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-06 03:03:54.000000 halmos-0.0.8/tests/test/Library.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-05-06 03:03:54.000000 halmos-0.0.8/tests/test/List.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-05-06 03:03:54.000000 halmos-0.0.8/tests/test/Opcode.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-05-06 03:03:54.000000 halmos-0.0.8/tests/test/Prank.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-05-06 03:03:54.000000 halmos-0.0.8/tests/test/Send.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-06 03:03:54.000000 halmos-0.0.8/tests/test/Setup.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-05-06 03:03:54.000000 halmos-0.0.8/tests/test/SetupPlus.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-06 03:03:54.000000 halmos-0.0.8/tests/test/SignExtend.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-05-06 03:03:54.000000 halmos-0.0.8/tests/test/Storage.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-06 03:03:54.000000 halmos-0.0.8/tests/test/Struct.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-05-06 03:03:54.000000 halmos-0.0.8/tests/test/Warp.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)     6085 2023-05-06 03:03:54.000000 halmos-0.0.8/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6151 2023-05-06 03:03:54.000000 halmos-0.0.8/tests/test_sevm.py
```

### Comparing `halmos-0.0.7/.github/ISSUE_TEMPLATE/feature_request.md` & `halmos-0.0.8/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `halmos-0.0.7/.github/workflows/codeql.yml` & `halmos-0.0.8/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `halmos-0.0.7/.github/workflows/test.yml` & `halmos-0.0.8/.github/workflows/test.yml`

 * *Files 4% similar despite different names*

```diff
@@ -35,8 +35,8 @@
       - name: Install Halmos
         run: pip install -e .
 
       - name: Run pytest
         run: pytest
 
       - name: Test Halmos
-        run: halmos tests
+        run: halmos tests --solver-axioms
```

### Comparing `halmos-0.0.7/LICENSE` & `halmos-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `halmos-0.0.7/PKG-INFO` & `halmos-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: halmos
-Version: 0.0.7
+Version: 0.0.8
 Summary: Halmos: Symbolic Bounded Model Checker for Ethereum Smart Contracts Bytecode
 Author: Daejun Park
 Project-URL: Homepage, https://github.com/a16z/halmos
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `halmos-0.0.7/README.md` & `halmos-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `halmos-0.0.7/examples/src/Example.sol` & `halmos-0.0.8/examples/src/Example.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.0.7/examples/test/Example.t.sol` & `halmos-0.0.8/examples/test/Example.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.0.7/pyproject.toml` & `halmos-0.0.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `halmos-0.0.7/src/halmos/__main__.py` & `halmos-0.0.8/src/halmos/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 from timeit import default_timer as timer
 
 from crytic_compile import cryticparser
 from crytic_compile import CryticCompile, InvalidCompilation
 
 from .utils import color_good, color_warn
+from .byte2op import mnemonic
 from .sevm import *
 
 if hasattr(sys, 'set_int_max_str_digits'): # Python verion >=3.8.14, >=3.9.14, >=3.10.7, or >=3.11
     sys.set_int_max_str_digits(0)
 
 def parse_args(args) -> argparse.Namespace:
     parser = argparse.ArgumentParser(prog='halmos', epilog='For more information, see https://github.com/a16z/halmos')
@@ -41,14 +42,16 @@
     parser.add_argument(   '--smt-div',          action='store_true', help=       'interpret `/`')
     parser.add_argument(   '--smt-div-by-const', action='store_true', help=       'interpret division by constant')
     parser.add_argument(   '--smt-mod-by-const', action='store_true', help=       'interpret constant modulo')
     parser.add_argument(   '--smt-exp-by-const', metavar='N', type=int, default=2, help='interpret constant power up to N (default: %(default)s)')
 
     parser.add_argument('--solver-timeout-branching', metavar='TIMEOUT', type=int, default=1000, help='set timeout (in milliseconds) for solving branching conditions (default: %(default)s)')
     parser.add_argument('--solver-timeout-assertion', metavar='TIMEOUT', type=int, default=60000, help='set timeout (in milliseconds) for solving assertion violation conditions (default: %(default)s)')
+    parser.add_argument('--solver-fresh', action='store_true', help='run an extra solver with a fresh state for unknown')
+    parser.add_argument('--solver-axioms', action='store_true', help='run an extra solver with axioms for unknown')
     parser.add_argument('--solver-subprocess', action='store_true', help='run an extra solver in subprocess for unknown')
 
     parser.add_argument('-v', '--verbose', action='count', default=0, help='increase verbosity levels: -v, -vv, -vvv, -vvvv')
     parser.add_argument('--debug', action='store_true', help='run in debug mode')
     parser.add_argument('--log', metavar='LOG_FILE_PATH', help='log individual execution steps in JSON')
     parser.add_argument('--print-revert', action='store_true', help='print reverting paths in verbose mode')
 
@@ -141,15 +144,28 @@
     pgm = ops_to_pgm(ops)
     return (pgm, code)
 
 def mk_callvalue() -> Word:
     return BitVec('msg_value', 256)
 
 def mk_balance() -> Word:
-    return BitVec('this_balance', 256)
+    return Array('balance0', BitVecSort(256), BitVecSort(256))
+
+def mk_block() -> Block:
+    block = Block(
+        basefee    = ZeroExt(160, BitVec('block_basefee', 96)),     # practical limit 96 bit
+        chainid    = ZeroExt(192, BitVec('block_chainid', 64)),     # chainid 64 bit
+        coinbase   = ZeroExt(96, BitVec('block_coinbase', 160)),    # address 160 bit
+        difficulty = BitVec('block_difficulty', 256),
+        gaslimit   = ZeroExt(160, BitVec('block_gaslimit', 96)),    # practical limit 96 bit
+        number     = ZeroExt(192, BitVec('block_number', 64)),      # practical limit 64 bit
+        timestamp  = ZeroExt(192, BitVec('block_timestamp', 64)),   # practical limit 64 bit
+    )
+    block.chainid = con(1) # for ethereum
+    return block
 
 def mk_caller(solver) -> Word:
     caller = BitVec('msg_sender', 256)
     solver.add(Extract(255, 160, caller) == BitVecVal(0, 96))
     return caller
 
 def mk_this(solver) -> Word:
@@ -166,41 +182,43 @@
     (pgm, code) = decode_hex(hexcode)
 
     storage = {}
 
     solver = mk_solver(args)
 
     balance = mk_balance()
+    block = mk_block()
     callvalue = mk_callvalue()
     caller = mk_caller(solver)
     this = mk_this(solver)
 
     sevm = SEVM(options)
     ex = sevm.mk_exec(
         pgm       = { this: pgm },
         code      = { this: code },
         storage   = { this: storage },
-        balance   = { this: balance },
+        balance   = balance,
+        block     = block,
         calldata  = [],
         callvalue = callvalue,
         caller    = caller,
         this      = this,
         symbolic  = True,
         solver    = solver,
     )
     (exs, _) = sevm.run(ex)
 
     models = []
     for idx, ex in enumerate(exs):
         opcode = ex.pgm[ex.this][ex.pc].op[0]
-        if is_bv_value(opcode) and opcode.as_long() in [EVM.STOP, EVM.RETURN, EVM.REVERT]:
+        if is_bv_value(opcode) and opcode.as_long() in [EVM.STOP, EVM.RETURN, EVM.REVERT, EVM.INVALID]:
             gen_model(args, models, idx, ex)
-            print(f'Final opcode: {opcode.as_long()} | Return data: {ex.output} | Input example: {models[-1][0]}')
+            print(f'Final opcode: {mnemonic(opcode)} | Return data: {ex.output} | Input example: {models[-1][0]}')
         else:
-            print(color_warn('Not supported: ' + opcode + ' ' + ex.error))
+            print(color_warn(f'Not supported: {mnemonic(opcode)} {ex.error}'))
         if args.verbose >= 1:
             print(f'# {idx+1} / {len(exs)}')
             print(ex)
 
     return exs
 
 def setup(
@@ -221,15 +239,16 @@
 
     sevm = SEVM(options)
 
     setup_ex = sevm.mk_exec(
         pgm       = { this: pgm },
         code      = { this: code },
         storage   = { this: {} },
-        balance   = { this: con(0) },
+        balance   = mk_balance(),
+        block     = mk_block(),
         calldata  = [],
         callvalue = con(0),
         caller    = mk_caller(solver),
         this      = this,
         symbolic  = False,
         solver    = solver,
     )
@@ -261,14 +280,16 @@
     funname: str,
     funsig: str,
     funselector: str,
     arrlen: Dict,
     args: argparse.Namespace,
     options: Dict
 ) -> int:
+    if args.debug: print(f'Executing {funname}')
+
     #
     # calldata
     #
 
     cd = []
 
     wstore(cd, 0, 4, BitVecVal(funselector, 32))
@@ -279,20 +300,14 @@
     #
     # callvalue
     #
 
     callvalue = mk_callvalue()
 
     #
-    # balance
-    #
-
-    balance = mk_balance()
-
-    #
     # run
     #
 
     start = timer()
 
     sevm = SEVM(options)
 
@@ -300,51 +315,57 @@
     solver.set(timeout=args.solver_timeout_branching)
     solver.add(setup_ex.solver.assertions())
 
     (exs, steps) = sevm.run(Exec(
         pgm       = setup_ex.pgm.copy(), # shallow copy
         code      = setup_ex.code.copy(), # shallow copy
         storage   = deepcopy(setup_ex.storage),
-        balance   = { setup_ex.this: sevm.arith(EVM.ADD, balance, callvalue) },
+        balance   = setup_ex.balance, # TODO: add callvalue
+        #
+        block     = deepcopy(setup_ex.block),
         #
         calldata  = cd,
         callvalue = callvalue,
         caller    = setup_ex.caller,
         this      = setup_ex.this,
         #
         pc        = 0,
         st        = State(),
         jumpis    = {},
         output    = None,
         symbolic  = True,
+        prank     = Prank(), # prank is reset after setUp()
         #
         solver    = solver,
         path      = deepcopy(setup_ex.path),
         #
         log       = deepcopy(setup_ex.log),
         cnts      = deepcopy(setup_ex.cnts),
         sha3s     = deepcopy(setup_ex.sha3s),
         storages  = deepcopy(setup_ex.storages),
+        balances  = deepcopy(setup_ex.balances),
         calls     = deepcopy(setup_ex.calls),
         failed    = setup_ex.failed,
         error     = setup_ex.error,
     ))
 
     # check assertion violations
     normal = 0
     models = []
     stuck = []
     for idx, ex in enumerate(exs):
+        if args.debug: print(f'Checking output: {idx+1} / {len(exs)}')
+
         opcode = ex.pgm[ex.this][ex.pc].op[0]
         if is_bv_value(opcode) and opcode.as_long() in [EVM.STOP, EVM.RETURN]:
             if ex.failed:
                 gen_model(args, models, idx, ex)
             else:
                 normal += 1
-        elif is_bv_value(opcode) and opcode.as_long() == EVM.REVERT:
+        elif is_bv_value(opcode) and opcode.as_long() in [EVM.REVERT, EVM.INVALID]:
             # Panic(1) # bytes4(keccak256("Panic(uint256)")) + bytes32(1)
             if ex.output == int('4e487b71' + '0000000000000000000000000000000000000000000000000000000000000001', 16): # 152078208365357342262005707660225848957176981554335715805457651098985835139029979365377
                 gen_model(args, models, idx, ex)
         else:
             stuck.append((opcode, idx, ex))
 
     end = timer()
@@ -355,22 +376,22 @@
     else:
         passfail = color_warn('[FAIL]')
 
     # print result
     print(f"{passfail} {funsig} (paths: {normal}/{len(exs)}, time: {end - start:0.2f}s, bounds: [{', '.join(dyn_param_size)}])")
     for model, idx, ex in models:
         if model:
-            print(color_warn('Counterexample: ' + str_model(model, args)))
+            print(color_warn(f'Counterexample: {str_model(model, args)}'))
         else:
-            print(color_warn('Counterexample: unknown'))
+            print(color_warn(f'Counterexample: unknown'))
         if args.verbose >= 1:
             print(f'# {idx+1} / {len(exs)}')
             print(ex)
     for opcode, idx, ex in stuck:
-        print(color_warn('Not supported: ' + opcode + ' ' + ex.error))
+        print(color_warn(f'Not supported: {mnemonic(opcode)} {ex.error}'))
         if args.verbose >= 1:
             print(f'# {idx+1} / {len(exs)}')
             print(ex)
 
     # print post-states
     if args.verbose >= 2:
         for idx, ex in enumerate(exs):
@@ -386,23 +407,29 @@
     # exitcode
     if passed:
         return 0
     else:
         return 1
 
 def gen_model(args: argparse.Namespace, models: List, idx: int, ex: Exec) -> None:
+    if args.debug: print(f'{" "*2}Checking assertion violation')
+
     res = ex.solver.check()
-    if res == sat: model = ex.solver.model()
-    if res == unknown:
+    if res == sat:
+        if args.debug: print(f'{" "*4}Generating a counterexample')
+        model = ex.solver.model()
+    if res == unknown and args.solver_fresh:
+        if args.debug: print(f'{" "*4}Checking again with a fresh solver')
         sol2 = SolverFor('QF_AUFBV', ctx=Context())
         sol2.set(timeout=args.solver_timeout_assertion)
         sol2.from_string(ex.solver.sexpr())
         res = sol2.check()
         if res == sat: model = sol2.model()
-    if res == sat and not is_valid_model(model):
+    if res == sat and not is_valid_model(model) and args.solver_axioms:
+        if args.debug: print(f'{" "*4}Checking again with axioms')
         ctx = Context()
         sol3 = Solver(ctx=ctx)
         sol3.set(timeout=args.solver_timeout_assertion)
         sol3.from_string(ex.solver.sexpr())
         x = BitVec('x', 256, ctx)
         y = BitVec('y', 256, ctx)
     #   zero = BitVecVal(0, 256, ctx)
@@ -427,31 +454,36 @@
     #   sol3.add(ForAll([x], evm_exp(x, zero) == one))          # x ** 0 == 1   # 0 ** 0 == 1
     #   sol3.add(ForAll([x], evm_exp(x, one) == x))             # x ** 1 == x
     #   sol3.add(ForAll([x], evm_exp(x, two) == x * x))         # x ** 2 == x * x
     #   #
         res = sol3.check()
         if res == sat: model = sol3.model()
     if res == unknown and args.solver_subprocess:
+        if args.debug: print(f'{" "*4}Checking again in an external process')
         fname = f'/tmp/{uuid.uuid4().hex}.smt2'
         if args.verbose >= 4: print(f'z3 -smt2 {fname}')
         with open(fname, 'w') as f:
             f.write('(set-logic QF_AUFBV)\n')
             f.write(ex.solver.to_smt2())
         res_str = subprocess.run(['z3', fname], capture_output=True, text=True).stdout.strip()
         if args.verbose >= 4: print(res_str)
         if res_str == 'unsat':
             res = unsat
     if res == unsat:
+        if args.debug: print(f'{" "*4}Passed')
         return
     if res == sat:
         if is_valid_model(model):
+            if args.debug: print(f'{" "*4}Done')
             models.append((model, idx, ex))
         else:
+            if args.debug: print(f'{" "*4}Invalid counterexample')
             models.append((None, idx, ex))
     else:
+        if args.debug: print(f'{" "*4}Timeout')
         models.append((None, idx, ex))
 
 def is_valid_model(model) -> bool:
     for decl in model:
         inter = model[decl]
         if str(decl).startswith('evm_'):
             return False
```

### Comparing `halmos-0.0.7/src/halmos/byte2op.py` & `halmos-0.0.8/src/halmos/byte2op.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,24 +12,26 @@
     op: List[Any] # opcode + argument (optional)
 
     def __init__(self, pc, op) -> None:
         self.pc = pc
         self.op = op
 
     def __str__(self) -> str:
-        opcode = self.op[0]
-        if is_bv_value(opcode):
-            opcode = opcode.as_long()
-            ret = str_opcode.get(opcode, hex(opcode))
-        else:
-            ret = str(opcode)
+        ret = mnemonic(self.op[0])
         if len(self.op) > 1:
             ret += ' ' + str(self.op[1])
         return ret
 
+def mnemonic(opcode) -> str:
+    if is_bv_value(opcode):
+        opcode = opcode.as_long()
+        return str_opcode.get(opcode, hex(opcode))
+    else:
+        return str(opcode)
+
 def concat(args):
     if len(args) > 1:
         return Concat(args)
     else:
         return args[0]
 
 # Decode ByteCodes to Opcodes
```

### Comparing `halmos-0.0.7/src/halmos/sevm.py` & `halmos-0.0.8/src/halmos/sevm.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,39 +5,33 @@
 
 from copy import deepcopy
 from collections import defaultdict
 from typing import List, Dict, Set, Tuple, Any
 from functools import reduce
 
 from z3 import *
-from .byte2op import Opcode, decode, concat
-from .utils import EVM, color_good, color_warn, hevm_cheat_code, sha3_inv
+from .byte2op import Opcode, decode, concat, mnemonic
+from .utils import EVM, color_good, color_warn, sha3_inv
+from .cheatcodes import hevm_cheat_code, Prank
 
 Word = Any # z3 expression (including constants)
 Byte = Any # z3 expression (including constants)
 Bytes = Any # z3 expression (including constants)
 
 Steps = Dict[int,Dict[str,Any]] # execution tree
 
 # symbolic states
 f_calldataload = Function('calldataload', BitVecSort(256), BitVecSort(256)) # index
 f_calldatasize = Function('calldatasize', BitVecSort(256))
-f_origin       = Function('origin'      , BitVecSort(256))
-f_coinbase     = Function('coinbase'    , BitVecSort(256))
 f_extcodesize  = Function('extcodesize' , BitVecSort(256), BitVecSort(256)) # target address
 f_extcodehash  = Function('extcodehash' , BitVecSort(256), BitVecSort(256)) # target address
 f_blockhash    = Function('blockhash'   , BitVecSort(256), BitVecSort(256)) # block number
 f_gas          = Function('gas'         , BitVecSort(256), BitVecSort(256)) # cnt
 f_gasprice     = Function('gasprice'    , BitVecSort(256))
-f_timestamp    = Function('timestamp'   , BitVecSort(256))
-f_blocknumber  = Function('blocknumber' , BitVecSort(256))
-f_difficulty   = Function('difficulty'  , BitVecSort(256))
-f_gaslimit     = Function('gaslimit'    , BitVecSort(256))
-f_chainid      = Function('chainid'     , BitVecSort(256))
-f_orig_balance = Function('orig_balance', BitVecSort(256), BitVecSort(256)) # target address
+f_origin       = Function('origin'      , BitVecSort(256))
 
 # uninterpreted arithmetic
 f_add  = Function('evm_add' , BitVecSort(256), BitVecSort(256), BitVecSort(256))
 f_sub  = Function('evm_sub' , BitVecSort(256), BitVecSort(256), BitVecSort(256))
 f_mul  = Function('evm_mul' , BitVecSort(256), BitVecSort(256), BitVecSort(256))
 f_div  = Function('evm_div' , BitVecSort(256), BitVecSort(256), BitVecSort(256))
 f_mod  = Function('evm_mod' , BitVecSort(256), BitVecSort(256), BitVecSort(256))
@@ -160,67 +154,93 @@
         loc: int = self.mloc()
         size: int = int(str(self.pop())) # size (in bytes) must be concrete
         if size > 0:
             return wload(self.memory, loc, size)
         else:
             return None
 
+class Block:
+    basefee: Any
+    chainid: Any
+    coinbase: Any
+    difficulty: Any # prevrandao
+    gaslimit: Any
+    number: Any
+    timestamp: Any
+
+    def __init__(self, **kwargs) -> None:
+        self.basefee    = kwargs['basefee']
+        self.chainid    = kwargs['chainid']
+        self.coinbase   = kwargs['coinbase']
+        self.difficulty = kwargs['difficulty']
+        self.gaslimit   = kwargs['gaslimit']
+        self.number     = kwargs['number']
+        self.timestamp  = kwargs['timestamp']
+
 class Exec: # an execution path
     # network
     pgm: Dict[Any,List[Opcode]] # address -> { opcode map: pc -> opcode }
     code: Dict[Any,List[Any]] # address -> opcode sequence
     storage: Dict[Any,Dict[int,Any]] # address -> { storage slot -> value }
-    balance: Dict[Any,Any] # address -> balance
+    balance: Any # address -> balance
+    # block
+    block: Block
     # tx
     calldata: List[Byte] # msg.data
     callvalue: Word # msg.value
     caller: Word # msg.sender
     this: Word # current account address
     # vm state
     pc: int
     st: State # stack and memory
     jumpis: Dict[str,Dict[bool,int]] # for loop detection
     output: Any # returndata
     symbolic: bool # symbolic or concrete storage
+    prank: Prank
     # path
     solver: Solver
     path: List[Any] # path conditions
     # logs
     log: List[Tuple[List[Word], Any]] # event logs emitted
     cnts: Dict[int,int] # opcode -> frequency
     sha3s: List[Tuple[Word,Word]] # sha3 hashes generated
-    storages: List[Tuple[Any,Any]] # storage updates
+    storages: Dict[Any,Any] # storage updates
+    balances: Dict[Any,Any] # balance updates
     calls: List[Any] # external calls
     failed: bool
     error: str
 
     def __init__(self, **kwargs) -> None:
         self.pgm      = kwargs['pgm']
         self.code     = kwargs['code']
         self.storage  = kwargs['storage']
         self.balance  = kwargs['balance']
         #
+        self.block    = kwargs['block']
+        #
         self.calldata = kwargs['calldata']
         self.callvalue= kwargs['callvalue']
         self.caller   = kwargs['caller']
         self.this     = kwargs['this']
         #
         self.pc       = kwargs['pc']
         self.st       = kwargs['st']
         self.jumpis   = kwargs['jumpis']
         self.output   = kwargs['output']
         self.symbolic = kwargs['symbolic']
+        self.prank    = kwargs['prank']
         #
         self.solver   = kwargs['solver']
         self.path     = kwargs['path']
         #
         self.log      = kwargs['log']
         self.cnts     = kwargs['cnts']
         self.sha3s    = kwargs['sha3s']
         self.storages = kwargs['storages']
+        self.balances = kwargs['balances']
         self.calls    = kwargs['calls']
         self.failed   = kwargs['failed']
         self.error    = kwargs['error']
 
     def str_cnts(self) -> str:
         return ''.join([f'{x[0]}: {x[1]}\n' for x in sorted(self.cnts.items(), key=lambda x: x[0])])
 
@@ -230,37 +250,67 @@
     def str_path(self) -> str:
         return ''.join(map(lambda x: '- ' + str(x) + '\n', filter(lambda x: str(x) != 'True', self.path)))
 
     def __str__(self) -> str:
         return ''.join([
             'PC: '              , str(self.this), ' ', str(self.pc), ' ', str(self.pgm[self.this][self.pc]), '\n',
             str(self.st),
+            'Balance: '         , str(self.balance), '\n',
             'Storage:\n'        , ''.join(map(lambda x: '- ' + str(x) + ': ' + str(self.storage[x]) + '\n', self.storage)),
-            'Balance:\n'        , ''.join(map(lambda x: '- ' + str(x) + ': ' + str(self.balance[x]) + '\n', self.balance)),
         #   'Solver:\n'         , self.str_solver(), '\n',
             'Path:\n'           , self.str_path(),
             'Output: '          , str(self.output) , '\n',
             'Log: '             , str(self.log)    , '\n',
         #   'Opcodes:\n'        , self.str_cnts(),
         #   'Memsize: '         , str(len(self.st.memory)), '\n',
-            'Storage updates:\n', ''.join(map(lambda x: '- ' + str(x) + '\n', self.storages)),
+            'Balance updates:\n', ''.join(map(lambda x: '- ' + str(x) + '\n', sorted(self.balances.items(), key=lambda x: str(x[0])))),
+            'Storage updates:\n', ''.join(map(lambda x: '- ' + str(x) + '\n', sorted(self.storages.items(), key=lambda x: str(x[0])))),
             'SHA3 hashes:\n'    , ''.join(map(lambda x: '- ' + str(x) + '\n', self.sha3s)),
             'External calls:\n' , ''.join(map(lambda x: '- ' + str(x) + '\n', self.calls)),
         #   'Calldata: '        , str(self.calldata), '\n',
         ])
 
     def next_pc(self) -> None:
         self.pc += 1
         while self.pgm[self.this][self.pc] is None:
             self.pc += 1
 
+    def check(self, cond: Any) -> Any:
+        self.solver.push()
+        self.solver.add(simplify(cond))
+        result = self.solver.check()
+        self.solver.pop()
+        return result
+
+    def select(self, array: Any, key: Word, arrays: Dict) -> Word:
+        if array in arrays:
+            store = arrays[array]
+            if store.decl().name() == 'store' and store.num_args() == 3:
+                base = store.arg(0)
+                key0 = store.arg(1)
+                val0 = store.arg(2)
+                if eq(key, key0): # structural equality
+                    return val0
+                if self.check(key == key0) == unsat: # key != key0
+                    return self.select(base, key, arrays)
+                if self.check(key != key0) == unsat: # key == key0
+                    return val0
+        return Select(array, key)
+
     def balance_of(self, addr: Word) -> Word:
-        if addr not in self.balance:
-            self.balance[addr] = f_orig_balance(addr)
-        return self.balance[addr]
+        value = self.select(self.balance, addr, self.balances)
+        self.solver.add(ULT(value, con(2**96))) # practical assumption on the max balance per account
+        return value
+
+    def balance_update(self, addr: Word, value: Word):
+        new_balance_var = Array(f'balance{1+len(self.balances)}', BitVecSort(256), BitVecSort(256))
+        new_balance = Store(self.balance, addr, value)
+        self.solver.add(new_balance_var == new_balance)
+        self.balance = new_balance_var
+        self.balances[new_balance_var] = new_balance
 
     def sinit(self, slot: int, keys) -> None:
         if slot not in self.storage[self.this]:
             self.storage[self.this][slot] = {}
         if len(keys) not in self.storage[self.this][slot]:
             if len(keys) == 0:
                 if self.symbolic:
@@ -277,29 +327,29 @@
         offsets = self.decode_storage_loc(loc)
         if not len(offsets) > 0: raise ValueError(offsets)
         slot, keys = int(str(offsets[0])), offsets[1:]
         self.sinit(slot, keys)
         if len(keys) == 0:
             return self.storage[self.this][slot][0]
         else:
-            return Select(self.storage[self.this][slot][len(keys)], concat(keys))
+            return self.select(self.storage[self.this][slot][len(keys)], concat(keys), self.storages)
 
     def sstore(self, loc: Any, val: Any) -> None:
         offsets = self.decode_storage_loc(loc)
         if not len(offsets) > 0: raise ValueError(offsets)
         slot, keys = int(str(offsets[0])), offsets[1:]
         self.sinit(slot, keys)
         if len(keys) == 0:
             self.storage[self.this][slot][0] = val
         else:
             new_storage_var = Array(f'storage{self.cnt_sstore()}', BitVecSort(len(keys)*256), BitVecSort(256))
             new_storage = Store(self.storage[self.this][slot][len(keys)], concat(keys), val)
             self.solver.add(new_storage_var == new_storage)
             self.storage[self.this][slot][len(keys)] = new_storage_var
-            self.storages.append((new_storage_var,new_storage))
+            self.storages[new_storage_var] = new_storage
 
     def decode_storage_loc(self, loc: Any) -> Any:
         def normalize(expr: Any) -> Any:
             # Concat(Extract(255, 8, bvadd(x, y)), bvadd(Extract(7, 0, x), Extract(7, 0, y))) => x + y
             if expr.decl().name() == 'concat' and expr.num_args() == 2:
                 arg0 = expr.arg(0) # Extract(255, 8, bvadd(x, y))
                 arg1 = expr.arg(1) # bvadd(Extract(7, 0, x), Extract(7, 0, y))
@@ -627,46 +677,54 @@
         arg_size: int = int(str(ex.st.pop())) # size (in bytes) must be concrete
         ret_loc: int = ex.st.mloc()
         ret_size: int = int(str(ex.st.pop())) # size (in bytes) must be concrete
 
         if not arg_size >= 0: raise ValueError(arg_size)
         if not ret_size >= 0: raise ValueError(ret_size)
 
-        ex.balance[ex.this] = self.arith(EVM.SUB, ex.balance_of(ex.this), fund)
+        caller = ex.prank.lookup(ex.this, to)
+
+        if not (is_bv_value(fund) and fund.as_long() == 0):
+            ex.balance_update(caller, self.arith(EVM.SUB, ex.balance_of(caller), fund))
+            ex.balance_update(to,     self.arith(EVM.ADD, ex.balance_of(to),     fund))
 
         def call_known() -> None:
             calldata = [None] * arg_size
             wextend(ex.st.memory, arg_loc, arg_size)
             wstore_bytes(calldata, 0, arg_size, ex.st.memory[arg_loc:arg_loc+arg_size])
 
             # execute external calls
             (new_exs, new_steps) = self.run(Exec(
                 pgm       = ex.pgm,
                 code      = ex.code,
                 storage   = ex.storage,
                 balance   = ex.balance,
                 #
+                block     = ex.block,
+                #
                 calldata  = calldata,
                 callvalue = fund,
-                caller    = ex.this,
+                caller    = caller,
                 this      = to,
                 #
                 pc        = 0,
                 st        = State(),
                 jumpis    = {},
                 output    = None,
                 symbolic  = ex.symbolic,
+                prank     = Prank(),
                 #
                 solver    = ex.solver,
                 path      = ex.path,
                 #
                 log       = ex.log,
                 cnts      = ex.cnts,
                 sha3s     = ex.sha3s,
                 storages  = ex.storages,
+                balances  = ex.balances,
                 calls     = ex.calls,
                 failed    = ex.failed,
                 error     = ex.error,
             ))
 
             # process result
             for idx, new_ex in enumerate(new_exs):
@@ -680,14 +738,15 @@
 
                 # restore vm state
                 new_ex.pc = ex.pc
                 new_ex.st = deepcopy(ex.st)
                 new_ex.jumpis = deepcopy(ex.jumpis)
                 # new_ex.output is passed into the caller
                 new_ex.symbolic = ex.symbolic
+                new_ex.prank = ex.prank
 
                 # set return data (in memory)
                 wstore_partial(new_ex.st.memory, ret_loc, 0, min(ret_size, new_ex.returndatasize()), new_ex.output, new_ex.returndatasize())
 
                 # set status code (in stack)
                 if is_bv_value(opcode) and opcode.as_long() in [EVM.STOP, EVM.RETURN, EVM.REVERT, EVM.INVALID]:
                     if opcode.as_long() in [EVM.STOP, EVM.RETURN]:
@@ -696,15 +755,15 @@
                         new_ex.st.push(con(0))
 
                     # add to worklist even if it reverted during the external call
                     new_ex.next_pc()
                     stack.append((new_ex, step_id))
                 else:
                     # got stuck during external call
-                    new_ex.error = str('external call stuck: ' + opcode)
+                    new_ex.error = f'external call stuck: {mnemonic(opcode)}'
                     out.append(new_ex)
 
         def call_unknown() -> None:
             # push exit code
             if arg_size > 0:
                 arg = wload(ex.st.memory, arg_loc, arg_size)
                 f_call = Function('call_'+str(arg_size*8), BitVecSort(256), BitVecSort(256), BitVecSort(256), BitVecSort(256), BitVecSort(arg_size*8), BitVecSort(256))
@@ -727,19 +786,20 @@
 
             # vm cheat code
             if to == con(hevm_cheat_code.address):
                 ex.solver.add(exit_code_var != con(0))
                 # vm.fail()
                 if arg == hevm_cheat_code.fail_payload: # BitVecVal(hevm_cheat_code.fail_payload, 800)
                     ex.failed = True
-                # vm.assume()
+                # vm.assume(bool)
                 elif eq(arg.sort(), BitVecSort((4+32)*8)) and simplify(Extract(287, 256, arg)) == hevm_cheat_code.assume_sig:
                     assume_cond = simplify(is_non_zero(Extract(255, 0, arg)))
                     ex.solver.add(assume_cond)
                     ex.path.append(str(assume_cond))
+                # vm.getCode(string)
                 elif simplify(Extract(arg_size*8-1, arg_size*8-32, arg)) == hevm_cheat_code.get_code_sig:
                     calldata = bytes.fromhex(hex(arg.as_long())[2:])
                     path_len = int.from_bytes(calldata[36:68], 'big')
                     path = calldata[68:68+path_len].decode('utf-8')
 
                     if ':' in path:
                         [filename, contract_name] = path.split(':')
@@ -762,14 +822,54 @@
                     bytecode_len_ceil = (bytecode_len + 31) // 32 * 32
 
                     ret_bytes = '00' * 31 + '20' + bytecode_len_enc + bytecode.ljust(bytecode_len_ceil*2, '0')
                     ret_len = len(ret_bytes) // 2
                     ret_bytes = bytes.fromhex(ret_bytes)
 
                     ret = BitVecVal(int.from_bytes(ret_bytes, 'big'), ret_len * 8)
+                # vm.prank(address)
+                elif eq(arg.sort(), BitVecSort((4+32)*8)) and simplify(Extract(287, 256, arg)) == hevm_cheat_code.prank_sig:
+                    result = ex.prank.prank(simplify(Extract(255, 0, arg)))
+                    if not result:
+                        ex.error = 'You have an active prank already.'
+                        out.append(ex)
+                        return
+                # vm.startPrank(address)
+                elif eq(arg.sort(), BitVecSort((4+32)*8)) and simplify(Extract(287, 256, arg)) == hevm_cheat_code.start_prank_sig:
+                    result = ex.prank.startPrank(simplify(Extract(255, 0, arg)))
+                    if not result:
+                        ex.error = 'You have an active prank already.'
+                        out.append(ex)
+                        return
+                # vm.stopPrank()
+                elif eq(arg.sort(), BitVecSort((4)*8)) and simplify(Extract(31, 0, arg)) == hevm_cheat_code.stop_prank_sig:
+                    ex.prank.stopPrank()
+                # vm.deal(address,uint256)
+                elif eq(arg.sort(), BitVecSort((4+32*2)*8)) and simplify(Extract(543, 512, arg)) == hevm_cheat_code.deal_sig:
+                    who = simplify(Extract(511, 256, arg))
+                    amount = simplify(Extract(255, 0, arg))
+                    ex.balance_update(who, amount)
+                # vm.fee(uint256)
+                elif eq(arg.sort(), BitVecSort((4+32)*8)) and simplify(Extract(287, 256, arg)) == hevm_cheat_code.fee_sig:
+                    ex.block.basefee = simplify(Extract(255, 0, arg))
+                # vm.chainId(uint256)
+                elif eq(arg.sort(), BitVecSort((4+32)*8)) and simplify(Extract(287, 256, arg)) == hevm_cheat_code.chainid_sig:
+                    ex.block.chainid = simplify(Extract(255, 0, arg))
+                # vm.coinbase(address)
+                elif eq(arg.sort(), BitVecSort((4+32)*8)) and simplify(Extract(287, 256, arg)) == hevm_cheat_code.coinbase_sig:
+                    ex.block.coinbase = simplify(Extract(255, 0, arg))
+                # vm.difficulty(uint256)
+                elif eq(arg.sort(), BitVecSort((4+32)*8)) and simplify(Extract(287, 256, arg)) == hevm_cheat_code.difficulty_sig:
+                    ex.block.difficulty = simplify(Extract(255, 0, arg))
+                # vm.roll(uint256)
+                elif eq(arg.sort(), BitVecSort((4+32)*8)) and simplify(Extract(287, 256, arg)) == hevm_cheat_code.roll_sig:
+                    ex.block.number = simplify(Extract(255, 0, arg))
+                # vm.warp(uint256)
+                elif eq(arg.sort(), BitVecSort((4+32)*8)) and simplify(Extract(287, 256, arg)) == hevm_cheat_code.warp_sig:
+                    ex.block.timestamp = simplify(Extract(255, 0, arg))
                 else:
                     # TODO: support other cheat codes
                     ex.error = str('Unsupported cheat code: calldata: ' + str(arg))
                     out.append(ex)
                     return
 
             # store return value
@@ -798,51 +898,60 @@
         # contract creation code
         create_hexcode = wload(ex.st.memory, loc, size)
         (create_ops, create_code) = decode(create_hexcode)
         create_pgm = ops_to_pgm(create_ops)
 
         # new account address
         new_addr = create_address(ex.cnt_create())
+        for addr in ex.pgm:
+            ex.solver.add(new_addr != addr) # ensure new address is fresh
 
         # setup new account
         ex.pgm[new_addr] = create_pgm   # existing pgm must be empty
         ex.code[new_addr] = create_code # existing code must be empty
         ex.storage[new_addr] = {}       # existing storage may not be empty and reset here
-        ex.balance[new_addr] = f_orig_balance(new_addr)
+
+        # lookup prank
+        caller = ex.prank.lookup(ex.this, new_addr)
 
         # transfer value
-        ex.solver.add(UGE(ex.balance_of(ex.this), value)) # assume balance is enough; otherwise ignore this path
-        ex.balance[ex.this] = self.arith(EVM.SUB, ex.balance_of(ex.this), value)
-        ex.balance[new_addr] = self.arith(EVM.ADD, ex.balance_of(new_addr), value)
+        ex.solver.add(UGE(ex.balance_of(caller), value)) # assume balance is enough; otherwise ignore this path
+        if not (is_bv_value(value) and value.as_long() == 0):
+            ex.balance_update(caller,   self.arith(EVM.SUB, ex.balance_of(caller),   value))
+            ex.balance_update(new_addr, self.arith(EVM.ADD, ex.balance_of(new_addr), value))
 
         # execute contract creation code
         (new_exs, new_steps) = self.run(Exec(
             pgm       = ex.pgm,
             code      = ex.code,
             storage   = ex.storage,
             balance   = ex.balance,
             #
+            block     = ex.block,
+            #
             calldata  = [],
             callvalue = value,
             caller    = ex.this,
             this      = new_addr,
             #
             pc        = 0,
             st        = State(),
             jumpis    = {},
             output    = None,
             symbolic  = False,
+            prank     = Prank(),
             #
             solver    = ex.solver,
             path      = ex.path,
             #
             log       = ex.log,
             cnts      = ex.cnts,
             sha3s     = ex.sha3s,
             storages  = ex.storages,
+            balances  = ex.balances,
             calls     = ex.calls,
             failed    = ex.failed,
             error     = ex.error,
         ))
 
         # process result
         for idx, new_ex in enumerate(new_exs):
@@ -868,14 +977,15 @@
 
                 # restore vm state
                 new_ex.pc = ex.pc
                 new_ex.st = deepcopy(ex.st)
                 new_ex.jumpis = deepcopy(ex.jumpis)
                 new_ex.output = None # output is reset, not restored
                 new_ex.symbolic = ex.symbolic
+                new_ex.prank = ex.prank
 
                 # push new address to stack
                 new_ex.st.push(new_addr)
 
                 # add to worklist
                 new_ex.next_pc()
                 stack.append((new_ex, step_id))
@@ -935,15 +1045,15 @@
         elif self.options['sym_jump']:
             for target in valid_jump_destinations(ex.pgm[ex.this]):
                 ex.solver.push()
                 target_reachable = simplify(dst == target)
                 ex.solver.add(target_reachable)
                 if ex.solver.check() != unsat: # jump
                     if self.options.get('debug'):
-                        print(f"we can jump to {target} with model {ex.solver.model()}")
+                        print(f'we can jump to {target} with model {ex.solver.model()}')
                     new_ex = self.create_branch(ex, str(target_reachable), target)
                     stack.append((new_ex, step_id))
                 ex.solver.pop()
 
         else:
             raise ValueError(dst)
 
@@ -955,32 +1065,36 @@
         new_path.append(cond)
         new_ex = Exec(
             pgm      = ex.pgm.copy(), # shallow copy for potential new contract creation; existing code doesn't change
             code     = ex.code.copy(), # shallow copy
             storage  = deepcopy(ex.storage),
             balance  = deepcopy(ex.balance),
             #
+            block    = deepcopy(ex.block),
+            #
             calldata = ex.calldata,
             callvalue= ex.callvalue,
             caller   = ex.caller,
             this     = ex.this,
             #
             pc       = target,
             st       = deepcopy(ex.st),
             jumpis   = deepcopy(ex.jumpis),
             output   = deepcopy(ex.output),
             symbolic = ex.symbolic,
+            prank    = deepcopy(ex.prank),
             #
             solver   = new_solver,
             path     = new_path,
             #
             log      = deepcopy(ex.log),
             cnts     = deepcopy(ex.cnts),
             sha3s    = deepcopy(ex.sha3s),
             storages = deepcopy(ex.storages),
+            balances = deepcopy(ex.balances),
             calls    = deepcopy(ex.calls),
             failed   = ex.failed,
             error    = ex.error,
         )
         return new_ex
 
     def run(self, ex0: Exec) -> Tuple[List[Exec], Steps]:
@@ -1020,14 +1134,19 @@
                         print(ex)
 
                 if opcode == EVM.STOP:
                     ex.output = None
                     out.append(ex)
                     continue
 
+                elif opcode == EVM.INVALID:
+                    ex.output = None
+                    out.append(ex)
+                    continue
+
                 elif opcode == EVM.REVERT:
                     ex.output = ex.st.ret()
                     out.append(ex)
                     continue
 
                 elif opcode == EVM.RETURN:
                     ex.output = ex.st.ret()
@@ -1133,17 +1252,14 @@
                 elif opcode == EVM.CALLER:
                     ex.st.push(ex.caller)
                 elif opcode == EVM.ORIGIN:
                     ex.st.push(f_origin())
                     ex.solver.add(Extract(255, 160, f_origin()) == BitVecVal(0, 96))
                 elif opcode == EVM.ADDRESS:
                     ex.st.push(ex.this)
-                elif opcode == EVM.COINBASE:
-                    ex.st.push(f_coinbase())
-                    ex.solver.add(Extract(255, 160, f_coinbase()) == BitVecVal(0, 96))
                 elif opcode == EVM.EXTCODESIZE:
                     address = ex.st.pop()
                     if address in ex.code:
                         codesize = con(len(ex.code[address]))
                     else:
                         codesize = f_extcodesize(address)
                         if address == con(hevm_cheat_code.address):
@@ -1153,26 +1269,32 @@
                     ex.st.push(f_extcodehash(ex.st.pop()))
                 elif opcode == EVM.CODESIZE:
                     ex.st.push(con(len(ex.code[ex.this])))
                 elif opcode == EVM.GAS:
                     ex.st.push(f_gas(con(ex.cnt_gas())))
                 elif opcode == EVM.GASPRICE:
                     ex.st.push(f_gasprice())
-                elif opcode == EVM.TIMESTAMP:
-                    ex.st.push(f_timestamp())
-                elif opcode == EVM.NUMBER:
-                    ex.st.push(f_blocknumber())
+
+                elif opcode == EVM.BASEFEE:
+                    ex.st.push(ex.block.basefee)
+                elif opcode == EVM.CHAINID:
+                    ex.st.push(ex.block.chainid)
+                elif opcode == EVM.COINBASE:
+                    ex.st.push(ex.block.coinbase)
                 elif opcode == EVM.DIFFICULTY:
-                    ex.st.push(f_difficulty())
+                    ex.st.push(ex.block.difficulty)
                 elif opcode == EVM.GASLIMIT:
-                    ex.st.push(f_gaslimit())
+                    ex.st.push(ex.block.gaslimit)
+                elif opcode == EVM.NUMBER:
+                    ex.st.push(ex.block.number)
+                elif opcode == EVM.TIMESTAMP:
+                    ex.st.push(ex.block.timestamp)
 
-                elif opcode == EVM.CHAINID:
-                #   ex.st.push(f_chainid())
-                    ex.st.push(con(1)) # for ethereum
+                elif opcode == EVM.PC:
+                    ex.st.push(con(ex.pc))
 
                 elif opcode == EVM.BLOCKHASH:
                     ex.st.push(f_blockhash(ex.st.pop()))
 
                 elif opcode == EVM.BALANCE:
                     ex.st.push(ex.balance_of(ex.st.pop()))
                 elif opcode == EVM.SELFBALANCE:
@@ -1294,57 +1416,65 @@
         self,
         #
         pgm,
         code,
         storage,
         balance,
         #
+        block,
+        #
         calldata,
         callvalue,
         caller,
         this,
         #
     #   pc,
     #   st,
     #   jumpis,
     #   output,
         symbolic,
+    #   prank,
         #
         solver,
     #   path,
         #
     #   log,
     #   cnts,
     #   sha3s,
     #   storages,
+    #   balances,
     #   calls,
     #   failed,
     #   error,
     ) -> Exec:
         return Exec(
             pgm      = pgm,
             code     = code,
             storage  = storage,
             balance  = balance,
             #
+            block    = block,
+            #
             calldata = calldata,
             callvalue= callvalue,
             caller   = caller,
             this     = this,
             #
             pc       = 0,
             st       = State(),
             jumpis   = {},
             output   = None,
             symbolic = symbolic,
+            prank    = Prank(),
             #
             solver   = solver,
             path     = [],
             #
             log      = [],
             cnts     = defaultdict(int),
             sha3s    = [],
-            storages = [],
+            storages = {},
+            balances = {},
             calls    = [],
             failed   = False,
             error    = '',
         )
```

### Comparing `halmos-0.0.7/src/halmos/utils.py` & `halmos-0.0.8/src/halmos/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,38 +5,14 @@
 
 def color_good(text: str) -> str:
     return '\033[32m' + text + '\033[0m'
 
 def color_warn(text: str) -> str:
     return '\033[31m' + text + '\033[0m'
 
-class hevm_cheat_code:
-    # https://github.com/dapphub/ds-test/blob/cd98eff28324bfac652e63a239a60632a761790b/src/test.sol
-
-    # address constant HEVM_ADDRESS =
-    #     address(bytes20(uint160(uint256(keccak256('hevm cheat code')))));
-    address: int = 0x7109709ECfa91a80626fF3989D68f67F5b1DD12D
-
-    # abi.encodePacked(
-    #     bytes4(keccak256("store(address,bytes32,bytes32)")),
-    #     abi.encode(HEVM_ADDRESS, bytes32("failed"), bytes32(uint256(0x01)))
-    # )
-    fail_payload: int = int(
-        '70ca10bb' +
-        '0000000000000000000000007109709ecfa91a80626ff3989d68f67f5b1dd12d' +
-        '6661696c65640000000000000000000000000000000000000000000000000000' +
-        '0000000000000000000000000000000000000000000000000000000000000001', 16
-    )
-
-    # bytes4(keccak256("assume(bool)"))
-    assume_sig: int = 0x4C63E562
-
-    # bytes4(keccak256("getCode(string)))
-    get_code_sig: int = 0x8d1cc925
-
 class EVM:
     STOP           = 0x00
     ADD            = 0x01
     MUL            = 0x02
     SUB            = 0x03
     DIV            = 0x04
     SDIV           = 0x05
@@ -81,14 +57,15 @@
     COINBASE       = 0x41
     TIMESTAMP      = 0x42
     NUMBER         = 0x43
     DIFFICULTY     = 0x44
     GASLIMIT       = 0x45
     CHAINID        = 0x46
     SELFBALANCE    = 0x47
+    BASEFEE        = 0x48
     POP            = 0x50
     MLOAD          = 0x51
     MSTORE         = 0x52
     MSTORE8        = 0x53
     SLOAD          = 0x54
     SSTORE         = 0x55
     JUMP           = 0x56
@@ -225,14 +202,15 @@
     EVM.COINBASE       : 'COINBASE',
     EVM.TIMESTAMP      : 'TIMESTAMP',
     EVM.NUMBER         : 'NUMBER',
     EVM.DIFFICULTY     : 'DIFFICULTY',
     EVM.GASLIMIT       : 'GASLIMIT',
     EVM.CHAINID        : 'CHAINID',
     EVM.SELFBALANCE    : 'SELFBALANCE',
+    EVM.BASEFEE        : 'BASEFEE',
     EVM.POP            : 'POP',
     EVM.MLOAD          : 'MLOAD',
     EVM.MSTORE         : 'MSTORE',
     EVM.MSTORE8        : 'MSTORE8',
     EVM.SLOAD          : 'SLOAD',
     EVM.SSTORE         : 'SSTORE',
     EVM.JUMP           : 'JUMP',
```

### Comparing `halmos-0.0.7/src/halmos.egg-info/PKG-INFO` & `halmos-0.0.8/src/halmos.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: halmos
-Version: 0.0.7
+Version: 0.0.8
 Summary: Halmos: Symbolic Bounded Model Checker for Ethereum Smart Contracts Bytecode
 Author: Daejun Park
 Project-URL: Homepage, https://github.com/a16z/halmos
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `halmos-0.0.7/src/halmos.egg-info/SOURCES.txt` & `halmos-0.0.8/src/halmos.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 .github/workflows/test.yml
 examples/foundry.toml
 examples/src/Example.sol
 examples/test/Example.t.sol
 src/halmos/__init__.py
 src/halmos/__main__.py
 src/halmos/byte2op.py
+src/halmos/cheatcodes.py
 src/halmos/sevm.py
 src/halmos/utils.py
 src/halmos.egg-info/PKG-INFO
 src/halmos.egg-info/SOURCES.txt
 src/halmos.egg-info/dependency_links.txt
 src/halmos.egg-info/entry_points.txt
 src/halmos.egg-info/requires.txt
@@ -29,19 +30,25 @@
 tests/src/Const.sol
 tests/src/Counter.sol
 tests/src/Create.sol
 tests/src/List.sol
 tests/src/SignExtend.sol
 tests/src/Storage.sol
 tests/test/Arith.t.sol
+tests/test/Block.t.sol
 tests/test/Const.t.sol
 tests/test/Counter.t.sol
 tests/test/Create.t.sol
+tests/test/Deal.t.sol
 tests/test/Foundry.t.sol
+tests/test/Invalid.t.sol
 tests/test/Library.t.sol
 tests/test/List.t.sol
 tests/test/Opcode.t.sol
+tests/test/Prank.t.sol
+tests/test/Send.t.sol
 tests/test/Setup.t.sol
 tests/test/SetupPlus.t.sol
 tests/test/SignExtend.t.sol
 tests/test/Storage.t.sol
-tests/test/Struct.t.sol
+tests/test/Struct.t.sol
+tests/test/Warp.t.sol
```

### Comparing `halmos-0.0.7/tests/src/Counter.sol` & `halmos-0.0.8/tests/src/Counter.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.0.7/tests/src/Storage.sol` & `halmos-0.0.8/tests/src/Storage.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.0.7/tests/test/Arith.t.sol` & `halmos-0.0.8/tests/test/Arith.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.0.7/tests/test/Counter.t.sol` & `halmos-0.0.8/tests/test/Counter.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.0.7/tests/test/Create.t.sol` & `halmos-0.0.8/tests/test/Create.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.0.7/tests/test/Library.t.sol` & `halmos-0.0.8/tests/test/Library.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.0.7/tests/test/List.t.sol` & `halmos-0.0.8/tests/test/List.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.0.7/tests/test/Opcode.t.sol` & `halmos-0.0.8/tests/test/Opcode.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.0.7/tests/test/Setup.t.sol` & `halmos-0.0.8/tests/test/Setup.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.0.7/tests/test/SetupPlus.t.sol` & `halmos-0.0.8/tests/test/SetupPlus.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.0.7/tests/test/Storage.t.sol` & `halmos-0.0.8/tests/test/Storage.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.0.7/tests/test_cli.py` & `halmos-0.0.8/tests/test_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,15 @@
     setup_ex = halmos.__main__.setup(hexcode, abi, setup_name, setup_sig, setup_selector, arrlen, args, options)
     assert str(setup_ex.st.stack) == '[1]'
 
 def test_opcode():
     assert str(Opcode(0, [con(0)])) == 'STOP'
     assert str(Opcode(0, [con(1)])) == 'ADD'
     assert str(Opcode(0, [con(EVM.PUSH32), con(1)])) == 'PUSH32 1'
-    assert str(Opcode(0, [con(0x48)])) == '0x48' # TODO: BASEFEE
+    assert str(Opcode(0, [con(EVM.BASEFEE)])) == 'BASEFEE'
     assert str(Opcode(0, [BitVec('x',8)])) == 'x'
     assert str(Opcode(0, [BitVec('x',8), BitVec('y',8)])) == 'x y'
     assert str(Opcode(0, [BitVec('x',8), BitVec('y',8), BitVec('z',8)])) == 'x y'
 
 def test_decode_hex():
     (pgm, code) = decode_hex('600100')
     assert str(pgm[0]) == 'PUSH1 1'
```

### Comparing `halmos-0.0.7/tests/test_sevm.py` & `halmos-0.0.8/tests/test_sevm.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 
 from z3 import *
 
 from halmos.utils import EVM
 
 from halmos.byte2op import decode
 
-from halmos.sevm import SEVM, con, ops_to_pgm, f_div, f_sdiv, f_mod, f_smod, f_exp, f_orig_balance, f_origin
+from halmos.sevm import SEVM, con, ops_to_pgm, f_div, f_sdiv, f_mod, f_smod, f_exp, f_origin
 
-from halmos.__main__ import parse_args, mk_options
+from halmos.__main__ import parse_args, mk_options, mk_block
 
 @pytest.fixture
 def args():
     return parse_args([])
 
 @pytest.fixture
 def options(args):
@@ -23,15 +23,15 @@
 def sevm(options):
     return SEVM(options)
 
 caller = BitVec('msg_sender', 256)
 
 this = BitVec('this_address', 256)
 
-balance = BitVec('this_balance', 256)
+balance = Array('balance0', BitVecSort(256), BitVecSort(256))
 
 callvalue = BitVec('msg_value', 256)
 
 @pytest.fixture
 def solver(args):
     solver = SolverFor('QF_AUFBV') # quantifier-free bitvector + array theory; https://smtlib.cs.uiowa.edu/logics.shtml
     solver.set(timeout=args.solver_timeout_branching)
@@ -46,15 +46,16 @@
 def mk_ex(hexcode, sevm, solver, storage, caller, this):
     (ops, code) = decode(hexcode)
     pgm = ops_to_pgm(ops)
     return sevm.mk_exec(
         pgm       = { this: pgm },
         code      = { this: code },
         storage   = { this: storage },
-        balance   = { this: balance },
+        balance   = balance,
+        block     = mk_block(),
         calldata  = [],
         callvalue = callvalue,
         caller    = caller,
         this      = this,
         symbolic  = True,
         solver    = solver,
     )
@@ -66,14 +67,15 @@
     return BitVecVal(opcode, 8)
 
 @pytest.mark.parametrize('hexcode, stack, pc, opcode', [
     (BitVecVal(int('600100', 16), 24), '[1]', 2, '0'),
     (BitVec('x', 256), '[]', 0, 'Extract(255, 248, x)'),
     (Concat(BitVecVal(int('6001', 16), 16), BitVec('x', 8), BitVecVal(0, 8)), '[1]', 2, 'x'),
     (Concat(BitVecVal(int('6101', 16), 16), BitVec('x', 8), BitVecVal(0, 8)), '[Concat(1, x)]', 3, '0'),
+    (BitVecVal(int('58585B5860015800', 16), 64), '[6, 1, 3, 1, 0]', 7, '0'),
 ])
 def test_run(hexcode, stack, pc, opcode, sevm, solver, storage):
     ex = mk_ex(hexcode, sevm, solver, storage, caller, this)
     (exs, _) = sevm.run(ex)
     assert len(exs) == 1
     ex = exs[0]
     assert str(ex.st.stack) == stack
@@ -148,20 +150,20 @@
     (o(EVM.SAR), [x, y], y >> x),
     (o(EVM.SAR), [con(0), y], y),
     (o(EVM.SAR), [con(255), y], y >> con(255)),
     (o(EVM.SAR), [con(256), y], y >> con(256)), # not necessarily 0; TODO: prove it is equal to y >> 255
     (o(EVM.SAR), [con(2**256-1), y], y >> con(2**256-1)), # not necessarily 0; TODO: prove it is equal to y >> 255
     # TODO: SHA3
     (o(EVM.ADDRESS), [], this),
-    (o(EVM.BALANCE), [x], f_orig_balance(x)),
+    (o(EVM.BALANCE), [x], Select(balance, x)),
     (o(EVM.ORIGIN), [], f_origin()),
     (o(EVM.CALLER), [], caller),
     (o(EVM.CALLVALUE), [], callvalue),
     # TODO: CALLDATA*, CODE*, EXTCODE*, RETURNDATA*
-    (o(EVM.SELFBALANCE), [], balance),
+    (o(EVM.SELFBALANCE), [], Select(balance, this)),
 ])
 def test_opcode_simple(hexcode, params, output, sevm, solver, storage):
     ex = mk_ex(Concat(hexcode, o(EVM.STOP)), sevm, solver, storage, caller, this)
     ex.st.stack.extend(params)
     (exs, _) = sevm.run(ex)
     assert len(exs) == 1
     ex = exs[0]
```

