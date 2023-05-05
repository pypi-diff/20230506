# Comparing `tmp/spotlight-dev-0.0.1b4.tar.gz` & `tmp/spotlight-dev-0.0.1b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotlight-dev-0.0.1b4.tar", last modified: Fri May  5 18:15:16 2023, max compression
+gzip compressed data, was "spotlight-dev-0.0.1b5.tar", last modified: Fri May  5 22:35:30 2023, max compression
```

## Comparing `spotlight-dev-0.0.1b4.tar` & `spotlight-dev-0.0.1b5.tar`

### file list

```diff
@@ -1,131 +1,131 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:15:16.793636 spotlight-dev-0.0.1b4/
--rw-r--r--   0 root         (0) root         (0)     1413 2023-05-05 18:15:16.792636 spotlight-dev-0.0.1b4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      852 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-05 18:15:16.793636 spotlight-dev-0.0.1b4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1368 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:15:16.747632 spotlight-dev-0.0.1b4/spotlight/
--rw-rw-rw-   0 root         (0) root         (0)       44 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:15:16.749633 spotlight-dev-0.0.1b4/spotlight/api/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:15:16.751633 spotlight-dev-0.0.1b4/spotlight/api/auth/
--rw-rw-rw-   0 root         (0) root         (0)      214 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/api/auth/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1340 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/api/auth/__util.py
--rw-rw-rw-   0 root         (0) root         (0)     2262 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/api/auth/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)     1726 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/api/auth/synchronous.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:15:16.754633 spotlight-dev-0.0.1b4/spotlight/api/job/
--rw-rw-rw-   0 root         (0) root         (0)      313 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/api/job/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      745 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/api/job/__util.py
--rw-rw-rw-   0 root         (0) root         (0)     2640 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/api/job/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)      772 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/api/job/model.py
--rw-rw-rw-   0 root         (0) root         (0)     2339 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/api/job/synchronous.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:15:16.756633 spotlight-dev-0.0.1b4/spotlight/api/job/view/
--rw-rw-rw-   0 root         (0) root         (0)      127 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/api/job/view/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       98 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/api/job/view/__util.py
--rw-rw-rw-   0 root         (0) root         (0)      547 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/api/job/view/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)      454 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/api/job/view/model.py
--rw-rw-rw-   0 root         (0) root         (0)      508 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/api/job/view/synchronous.py
--rw-rw-rw-   0 root         (0) root         (0)      236 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/api/model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:15:16.758633 spotlight-dev-0.0.1b4/spotlight/api/organization/
--rw-rw-rw-   0 root         (0) root         (0)      381 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/api/organization/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      799 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/api/organization/__util.py
--rw-rw-rw-   0 root         (0) root         (0)     2805 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/api/organization/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)      396 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/api/organization/model.py
--rw-rw-rw-   0 root         (0) root         (0)     2503 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/api/organization/synchronous.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:15:16.761633 spotlight-dev-0.0.1b4/spotlight/api/organization/user/
--rw-rw-rw-   0 root         (0) root         (0)      314 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/api/organization/user/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      657 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/api/organization/user/__util.py
--rw-rw-rw-   0 root         (0) root         (0)     1876 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/api/organization/user/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)      154 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/api/organization/user/enum.py
--rw-rw-rw-   0 root         (0) root         (0)      535 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/api/organization/user/model.py
--rw-rw-rw-   0 root         (0) root         (0)     1644 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/api/organization/user/synchronous.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:15:16.763634 spotlight-dev-0.0.1b4/spotlight/api/organization/view/
--rw-rw-rw-   0 root         (0) root         (0)      163 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/api/organization/view/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      112 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/api/organization/view/__util.py
--rw-rw-rw-   0 root         (0) root         (0)      618 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/api/organization/view/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)      393 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/api/organization/view/model.py
--rw-rw-rw-   0 root         (0) root         (0)      561 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/api/organization/view/synchronous.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:15:16.766634 spotlight-dev-0.0.1b4/spotlight/api/rule/
--rw-rw-rw-   0 root         (0) root         (0)      453 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/api/rule/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1105 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/api/rule/__util.py
--rw-rw-rw-   0 root         (0) root         (0)     3667 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/api/rule/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)      828 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/api/rule/model.py
--rw-rw-rw-   0 root         (0) root         (0)     3270 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/api/rule/synchronous.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:15:16.769634 spotlight-dev-0.0.1b4/spotlight/api/tag/
--rw-rw-rw-   0 root         (0) root         (0)      327 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/api/tag/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1297 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/api/tag/__util.py
--rw-rw-rw-   0 root         (0) root         (0)     4324 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/api/tag/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)      341 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/api/tag/model.py
--rw-rw-rw-   0 root         (0) root         (0)     3844 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/api/tag/synchronous.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:15:16.772634 spotlight-dev-0.0.1b4/spotlight/api/tag/view/
--rw-rw-rw-   0 root         (0) root         (0)      127 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/api/tag/view/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      221 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/api/tag/view/__util.py
--rw-rw-rw-   0 root         (0) root         (0)      963 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/api/tag/view/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)      347 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/api/tag/view/model.py
--rw-rw-rw-   0 root         (0) root         (0)      867 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/api/tag/view/synchronous.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:15:16.772634 spotlight-dev-0.0.1b4/spotlight/core/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/core/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:15:16.777635 spotlight-dev-0.0.1b4/spotlight/core/common/
--rw-rw-rw-   0 root         (0) root         (0)       47 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/core/common/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2648 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/core/common/base.py
--rw-rw-rw-   0 root         (0) root         (0)      230 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/core/common/base_enum.py
--rw-rw-rw-   0 root         (0) root         (0)     2718 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/core/common/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:15:16.777635 spotlight-dev-0.0.1b4/spotlight/core/common/date/
--rw-rw-rw-   0 root         (0) root         (0)      206 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/core/common/date/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2478 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/core/common/date/function.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:15:16.779635 spotlight-dev-0.0.1b4/spotlight/core/common/decorators/
--rw-rw-rw-   0 root         (0) root         (0)      344 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/core/common/decorators/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:15:16.780635 spotlight-dev-0.0.1b4/spotlight/core/common/decorators/authorization/
--rw-rw-rw-   0 root         (0) root         (0)      253 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/core/common/decorators/authorization/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1154 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/core/common/decorators/authorization/__util.py
--rw-rw-rw-   0 root         (0) root         (0)     3920 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/core/common/decorators/authorization/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)     3898 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/core/common/decorators/authorization/synchronous.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:15:16.782635 spotlight-dev-0.0.1b4/spotlight/core/common/decorators/data/
--rw-rw-rw-   0 root         (0) root         (0)      190 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/core/common/decorators/data/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      696 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/core/common/decorators/data/__util.py
--rw-rw-rw-   0 root         (0) root         (0)     1401 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/core/common/decorators/data/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)     1399 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/core/common/decorators/data/synchronous.py
--rw-rw-rw-   0 root         (0) root         (0)      686 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/core/common/decorators/timeit.py
--rw-rw-rw-   0 root         (0) root         (0)      271 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/core/common/enum.py
--rw-rw-rw-   0 root         (0) root         (0)      726 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/core/common/errors.py
--rw-rw-rw-   0 root         (0) root         (0)     4794 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/core/common/function.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:15:16.782635 spotlight-dev-0.0.1b4/spotlight/core/common/metaclass/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/core/common/metaclass/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      924 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/core/common/metaclass/singleton.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:15:16.783635 spotlight-dev-0.0.1b4/spotlight/core/common/requests/
--rw-rw-rw-   0 root         (0) root         (0)      403 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/core/common/requests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4689 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/core/common/requests/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)     3788 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/core/common/requests/synchronous.py
--rw-rw-rw-   0 root         (0) root         (0)      241 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/core/common/type.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:15:16.785636 spotlight-dev-0.0.1b4/spotlight/core/pipeline/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/core/pipeline/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5958 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/core/pipeline/abstract.py
--rw-rw-rw-   0 root         (0) root         (0)     1004 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/core/pipeline/decorator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:15:16.786635 spotlight-dev-0.0.1b4/spotlight/core/pipeline/execution/
--rw-rw-rw-   0 root         (0) root         (0)       75 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/core/pipeline/execution/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:15:16.787636 spotlight-dev-0.0.1b4/spotlight/core/pipeline/execution/rule/
--rw-rw-rw-   0 root         (0) root         (0)      178 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/core/pipeline/execution/rule/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1817 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/core/pipeline/execution/rule/abstract.py
--rw-rw-rw-   0 root         (0) root         (0)      130 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/core/pipeline/execution/rule/enum.py
--rw-rw-rw-   0 root         (0) root         (0)     1477 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/core/pipeline/execution/rule/sql_rule.py
--rw-rw-rw-   0 root         (0) root         (0)     3363 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/core/pipeline/execution/synchronous.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:15:16.788636 spotlight-dev-0.0.1b4/spotlight/core/pipeline/model/
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/core/pipeline/model/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1704 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/core/pipeline/model/pipeline.py
--rw-rw-rw-   0 root         (0) root         (0)      282 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/core/pipeline/model/rule.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:15:16.788636 spotlight-dev-0.0.1b4/spotlight/core/pipeline/runner/
--rw-rw-rw-   0 root         (0) root         (0)     6327 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/core/pipeline/runner/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:15:16.789636 spotlight-dev-0.0.1b4/spotlight/core/pipeline/runner/utils/
--rw-rw-rw-   0 root         (0) root         (0)      192 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/core/pipeline/runner/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3573 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/core/pipeline/runner/utils/asynchronously.py
--rw-rw-rw-   0 root         (0) root         (0)     3356 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/core/pipeline/runner/utils/synchronously.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:15:16.790636 spotlight-dev-0.0.1b4/spotlight/pandas/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/pandas/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2204 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/pandas/__util.py
--rw-rw-rw-   0 root         (0) root         (0)     1069 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/pandas/pipeline.py
--rw-rw-rw-   0 root         (0) root         (0)     1738 2023-05-05 18:15:00.000000 spotlight-dev-0.0.1b4/spotlight/pandas/runners.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:15:16.792636 spotlight-dev-0.0.1b4/spotlight_dev.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1413 2023-05-05 18:15:16.000000 spotlight-dev-0.0.1b4/spotlight_dev.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3859 2023-05-05 18:15:16.000000 spotlight-dev-0.0.1b4/spotlight_dev.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-05 18:15:16.000000 spotlight-dev-0.0.1b4/spotlight_dev.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      227 2023-05-05 18:15:16.000000 spotlight-dev-0.0.1b4/spotlight_dev.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-05-05 18:15:16.000000 spotlight-dev-0.0.1b4/spotlight_dev.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 22:35:30.877600 spotlight-dev-0.0.1b5/
+-rw-r--r--   0 root         (0) root         (0)     1413 2023-05-05 22:35:30.877600 spotlight-dev-0.0.1b5/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      852 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-05 22:35:30.877600 spotlight-dev-0.0.1b5/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1216 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 22:35:30.833597 spotlight-dev-0.0.1b5/spotlight/
+-rw-rw-rw-   0 root         (0) root         (0)       44 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 22:35:30.834597 spotlight-dev-0.0.1b5/spotlight/api/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 22:35:30.835597 spotlight-dev-0.0.1b5/spotlight/api/auth/
+-rw-rw-rw-   0 root         (0) root         (0)      214 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/api/auth/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1340 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/api/auth/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)     2262 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/api/auth/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)     1726 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/api/auth/synchronous.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 22:35:30.837597 spotlight-dev-0.0.1b5/spotlight/api/job/
+-rw-rw-rw-   0 root         (0) root         (0)      313 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/api/job/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      745 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/api/job/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)     2640 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/api/job/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)      772 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/api/job/model.py
+-rw-rw-rw-   0 root         (0) root         (0)     2339 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/api/job/synchronous.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 22:35:30.839597 spotlight-dev-0.0.1b5/spotlight/api/job/view/
+-rw-rw-rw-   0 root         (0) root         (0)      127 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/api/job/view/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       98 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/api/job/view/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)      547 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/api/job/view/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)      454 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/api/job/view/model.py
+-rw-rw-rw-   0 root         (0) root         (0)      508 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/api/job/view/synchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)      236 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/api/model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 22:35:30.841597 spotlight-dev-0.0.1b5/spotlight/api/organization/
+-rw-rw-rw-   0 root         (0) root         (0)      381 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/api/organization/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      799 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/api/organization/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)     2805 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/api/organization/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)      396 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/api/organization/model.py
+-rw-rw-rw-   0 root         (0) root         (0)     2503 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/api/organization/synchronous.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 22:35:30.843598 spotlight-dev-0.0.1b5/spotlight/api/organization/user/
+-rw-rw-rw-   0 root         (0) root         (0)      314 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/api/organization/user/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      657 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/api/organization/user/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)     1876 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/api/organization/user/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)      154 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/api/organization/user/enum.py
+-rw-rw-rw-   0 root         (0) root         (0)      535 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/api/organization/user/model.py
+-rw-rw-rw-   0 root         (0) root         (0)     1644 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/api/organization/user/synchronous.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 22:35:30.845598 spotlight-dev-0.0.1b5/spotlight/api/organization/view/
+-rw-rw-rw-   0 root         (0) root         (0)      163 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/api/organization/view/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      112 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/api/organization/view/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)      618 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/api/organization/view/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)      393 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/api/organization/view/model.py
+-rw-rw-rw-   0 root         (0) root         (0)      561 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/api/organization/view/synchronous.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 22:35:30.847598 spotlight-dev-0.0.1b5/spotlight/api/rule/
+-rw-rw-rw-   0 root         (0) root         (0)      453 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/api/rule/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1105 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/api/rule/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)     3667 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/api/rule/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)      828 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/api/rule/model.py
+-rw-rw-rw-   0 root         (0) root         (0)     3270 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/api/rule/synchronous.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 22:35:30.849598 spotlight-dev-0.0.1b5/spotlight/api/tag/
+-rw-rw-rw-   0 root         (0) root         (0)      327 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/api/tag/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1297 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/api/tag/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)     4324 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/api/tag/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)      341 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/api/tag/model.py
+-rw-rw-rw-   0 root         (0) root         (0)     3844 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/api/tag/synchronous.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 22:35:30.851598 spotlight-dev-0.0.1b5/spotlight/api/tag/view/
+-rw-rw-rw-   0 root         (0) root         (0)      127 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/api/tag/view/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      221 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/api/tag/view/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)      963 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/api/tag/view/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)      347 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/api/tag/view/model.py
+-rw-rw-rw-   0 root         (0) root         (0)      867 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/api/tag/view/synchronous.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 22:35:30.851598 spotlight-dev-0.0.1b5/spotlight/core/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/core/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 22:35:30.854598 spotlight-dev-0.0.1b5/spotlight/core/common/
+-rw-rw-rw-   0 root         (0) root         (0)       47 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/core/common/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2648 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/core/common/base.py
+-rw-rw-rw-   0 root         (0) root         (0)      230 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/core/common/base_enum.py
+-rw-rw-rw-   0 root         (0) root         (0)     2718 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/core/common/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 22:35:30.855598 spotlight-dev-0.0.1b5/spotlight/core/common/date/
+-rw-rw-rw-   0 root         (0) root         (0)      206 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/core/common/date/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2478 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/core/common/date/function.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 22:35:30.855598 spotlight-dev-0.0.1b5/spotlight/core/common/decorators/
+-rw-rw-rw-   0 root         (0) root         (0)      344 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/core/common/decorators/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 22:35:30.857599 spotlight-dev-0.0.1b5/spotlight/core/common/decorators/authorization/
+-rw-rw-rw-   0 root         (0) root         (0)      253 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/core/common/decorators/authorization/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1154 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/core/common/decorators/authorization/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)     3920 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/core/common/decorators/authorization/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)     3898 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/core/common/decorators/authorization/synchronous.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 22:35:30.858599 spotlight-dev-0.0.1b5/spotlight/core/common/decorators/data/
+-rw-rw-rw-   0 root         (0) root         (0)      190 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/core/common/decorators/data/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      696 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/core/common/decorators/data/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)     1401 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/core/common/decorators/data/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)     1399 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/core/common/decorators/data/synchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)      686 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/core/common/decorators/timeit.py
+-rw-rw-rw-   0 root         (0) root         (0)      271 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/core/common/enum.py
+-rw-rw-rw-   0 root         (0) root         (0)      726 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/core/common/errors.py
+-rw-rw-rw-   0 root         (0) root         (0)     4794 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/core/common/function.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 22:35:30.858599 spotlight-dev-0.0.1b5/spotlight/core/common/metaclass/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/core/common/metaclass/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      924 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/core/common/metaclass/singleton.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 22:35:30.860599 spotlight-dev-0.0.1b5/spotlight/core/common/requests/
+-rw-rw-rw-   0 root         (0) root         (0)      403 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/core/common/requests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4689 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/core/common/requests/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)     3788 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/core/common/requests/synchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)      241 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/core/common/type.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 22:35:30.861599 spotlight-dev-0.0.1b5/spotlight/core/pipeline/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/core/pipeline/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5958 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/core/pipeline/abstract.py
+-rw-rw-rw-   0 root         (0) root         (0)     1004 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/core/pipeline/decorator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 22:35:30.862599 spotlight-dev-0.0.1b5/spotlight/core/pipeline/execution/
+-rw-rw-rw-   0 root         (0) root         (0)       75 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/core/pipeline/execution/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 22:35:30.864599 spotlight-dev-0.0.1b5/spotlight/core/pipeline/execution/rule/
+-rw-rw-rw-   0 root         (0) root         (0)      178 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/core/pipeline/execution/rule/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1817 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/core/pipeline/execution/rule/abstract.py
+-rw-rw-rw-   0 root         (0) root         (0)      130 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/core/pipeline/execution/rule/enum.py
+-rw-rw-rw-   0 root         (0) root         (0)     1477 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/core/pipeline/execution/rule/sql_rule.py
+-rw-rw-rw-   0 root         (0) root         (0)     3363 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/core/pipeline/execution/synchronous.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 22:35:30.866599 spotlight-dev-0.0.1b5/spotlight/core/pipeline/model/
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/core/pipeline/model/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1704 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/core/pipeline/model/pipeline.py
+-rw-rw-rw-   0 root         (0) root         (0)      282 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/core/pipeline/model/rule.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 22:35:30.866599 spotlight-dev-0.0.1b5/spotlight/core/pipeline/runner/
+-rw-rw-rw-   0 root         (0) root         (0)     6327 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/core/pipeline/runner/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 22:35:30.871600 spotlight-dev-0.0.1b5/spotlight/core/pipeline/runner/utils/
+-rw-rw-rw-   0 root         (0) root         (0)      192 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/core/pipeline/runner/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3573 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/core/pipeline/runner/utils/asynchronously.py
+-rw-rw-rw-   0 root         (0) root         (0)     3356 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/core/pipeline/runner/utils/synchronously.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 22:35:30.872600 spotlight-dev-0.0.1b5/spotlight/pandas/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/pandas/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2204 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/pandas/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)     1069 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/pandas/pipeline.py
+-rw-rw-rw-   0 root         (0) root         (0)     1738 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/pandas/runners.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 22:35:30.876600 spotlight-dev-0.0.1b5/spotlight_dev.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1413 2023-05-05 22:35:30.000000 spotlight-dev-0.0.1b5/spotlight_dev.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3859 2023-05-05 22:35:30.000000 spotlight-dev-0.0.1b5/spotlight_dev.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-05 22:35:30.000000 spotlight-dev-0.0.1b5/spotlight_dev.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      141 2023-05-05 22:35:30.000000 spotlight-dev-0.0.1b5/spotlight_dev.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-05-05 22:35:30.000000 spotlight-dev-0.0.1b5/spotlight_dev.egg-info/top_level.txt
```

### Comparing `spotlight-dev-0.0.1b4/PKG-INFO` & `spotlight-dev-0.0.1b5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotlight-dev
-Version: 0.0.1b4
+Version: 0.0.1b5
 Summary: Spotlight Python SDK
 Home-page: https://alpha.dev
 Author: Spotlight
 Author-email: hello@spotlight.dev
 License: UNKNOWN
 Description: # Spotlight: The data quality platform for developers
```

### Comparing `spotlight-dev-0.0.1b4/README.md` & `spotlight-dev-0.0.1b5/README.md`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b4/setup.py` & `spotlight-dev-0.0.1b5/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     tag = subprocess.getoutput('git tag --sort=version:refname | tail -n1')
     commits = subprocess.getoutput(f'git rev-list {tag}..HEAD --count')
     return f'{tag}.{commits}'
 
 
 setuptools.setup(
     name="spotlight-dev",
-    version="0.0.1b4",
+    version="0.0.1b5",
     author="Spotlight",
     author_email="hello@spotlight.dev",
     description="Spotlight Python SDK",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://alpha.dev",
     classifiers=[
@@ -32,23 +32,17 @@
     python_requires=">=3.7",
     packages=setuptools.find_packages(
         include=['spotlight*'],
         exclude=['tests.*']
     ),
     install_requires=[
         "requests==2.28.1",
-        "pandas==1.3.5",
-        "cachetools==5.2.0",
-        "pydash==5.1.0",
-        "PyYaml==6.0",
-        "asyncio==3.4.3",
-        "aiohttp==3.8.1",
-        "ujson==5.4.0",
-        "msgpack==1.0.4",
-        "fastparquet==0.8.1",
-        "scipy==1.8.0",
-        "duckdb==0.7.1",
-        "pydantic==1.9.1",
-        "aiocache==0.11.1",
-        "trycast==1.0.0"
+        "aiohttp>=3.8.4",
+        "pandas>=2.0.1",
+        "duckdb>=0.7.1",
+        "trycast>=1.0.0",
+        "pydash>=7.0.3",
+        "cachetools>=5.3.0",
+        "pydantic>=1.10.7",
+        "aiocache>=0.12.1"
     ]
 )
```

### Comparing `spotlight-dev-0.0.1b4/spotlight/api/auth/__util.py` & `spotlight-dev-0.0.1b5/spotlight/api/auth/__util.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b4/spotlight/api/auth/asynchronous.py` & `spotlight-dev-0.0.1b5/spotlight/api/auth/asynchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b4/spotlight/api/auth/synchronous.py` & `spotlight-dev-0.0.1b5/spotlight/api/auth/synchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b4/spotlight/api/job/__util.py` & `spotlight-dev-0.0.1b5/spotlight/api/job/__util.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b4/spotlight/api/job/asynchronous.py` & `spotlight-dev-0.0.1b5/spotlight/api/job/asynchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b4/spotlight/api/job/model.py` & `spotlight-dev-0.0.1b5/spotlight/api/job/model.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b4/spotlight/api/job/synchronous.py` & `spotlight-dev-0.0.1b5/spotlight/api/job/synchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b4/spotlight/api/job/view/asynchronous.py` & `spotlight-dev-0.0.1b5/spotlight/api/job/view/asynchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b4/spotlight/api/organization/__util.py` & `spotlight-dev-0.0.1b5/spotlight/api/organization/__util.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b4/spotlight/api/organization/asynchronous.py` & `spotlight-dev-0.0.1b5/spotlight/api/organization/asynchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b4/spotlight/api/organization/synchronous.py` & `spotlight-dev-0.0.1b5/spotlight/api/organization/synchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b4/spotlight/api/organization/user/__util.py` & `spotlight-dev-0.0.1b5/spotlight/api/organization/user/__util.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b4/spotlight/api/organization/user/asynchronous.py` & `spotlight-dev-0.0.1b5/spotlight/api/organization/user/asynchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b4/spotlight/api/organization/user/model.py` & `spotlight-dev-0.0.1b5/spotlight/api/organization/user/model.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b4/spotlight/api/organization/user/synchronous.py` & `spotlight-dev-0.0.1b5/spotlight/api/organization/user/synchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b4/spotlight/api/organization/view/asynchronous.py` & `spotlight-dev-0.0.1b5/spotlight/api/organization/view/asynchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b4/spotlight/api/organization/view/synchronous.py` & `spotlight-dev-0.0.1b5/spotlight/api/organization/view/synchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b4/spotlight/api/rule/__util.py` & `spotlight-dev-0.0.1b5/spotlight/api/rule/__util.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b4/spotlight/api/rule/asynchronous.py` & `spotlight-dev-0.0.1b5/spotlight/api/rule/asynchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b4/spotlight/api/rule/model.py` & `spotlight-dev-0.0.1b5/spotlight/api/rule/model.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b4/spotlight/api/rule/synchronous.py` & `spotlight-dev-0.0.1b5/spotlight/api/rule/synchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b4/spotlight/api/tag/__util.py` & `spotlight-dev-0.0.1b5/spotlight/api/tag/__util.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b4/spotlight/api/tag/asynchronous.py` & `spotlight-dev-0.0.1b5/spotlight/api/tag/asynchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b4/spotlight/api/tag/synchronous.py` & `spotlight-dev-0.0.1b5/spotlight/api/tag/synchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b4/spotlight/api/tag/view/asynchronous.py` & `spotlight-dev-0.0.1b5/spotlight/api/tag/view/asynchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b4/spotlight/api/tag/view/synchronous.py` & `spotlight-dev-0.0.1b5/spotlight/api/tag/view/synchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b4/spotlight/core/common/base.py` & `spotlight-dev-0.0.1b5/spotlight/core/common/base.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b4/spotlight/core/common/config.py` & `spotlight-dev-0.0.1b5/spotlight/core/common/config.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b4/spotlight/core/common/date/function.py` & `spotlight-dev-0.0.1b5/spotlight/core/common/date/function.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b4/spotlight/core/common/decorators/authorization/__util.py` & `spotlight-dev-0.0.1b5/spotlight/core/common/decorators/authorization/__util.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b4/spotlight/core/common/decorators/authorization/asynchronous.py` & `spotlight-dev-0.0.1b5/spotlight/core/common/decorators/authorization/asynchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b4/spotlight/core/common/decorators/authorization/synchronous.py` & `spotlight-dev-0.0.1b5/spotlight/core/common/decorators/authorization/synchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b4/spotlight/core/common/decorators/data/__util.py` & `spotlight-dev-0.0.1b5/spotlight/core/common/decorators/data/__util.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b4/spotlight/core/common/decorators/data/asynchronous.py` & `spotlight-dev-0.0.1b5/spotlight/core/common/decorators/data/asynchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b4/spotlight/core/common/decorators/data/synchronous.py` & `spotlight-dev-0.0.1b5/spotlight/core/common/decorators/data/synchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b4/spotlight/core/common/decorators/timeit.py` & `spotlight-dev-0.0.1b5/spotlight/core/common/decorators/timeit.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b4/spotlight/core/common/errors.py` & `spotlight-dev-0.0.1b5/spotlight/core/common/errors.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b4/spotlight/core/common/function.py` & `spotlight-dev-0.0.1b5/spotlight/core/common/function.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b4/spotlight/core/common/metaclass/singleton.py` & `spotlight-dev-0.0.1b5/spotlight/core/common/metaclass/singleton.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b4/spotlight/core/common/requests/asynchronous.py` & `spotlight-dev-0.0.1b5/spotlight/core/common/requests/asynchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b4/spotlight/core/common/requests/synchronous.py` & `spotlight-dev-0.0.1b5/spotlight/core/common/requests/synchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b4/spotlight/core/pipeline/abstract.py` & `spotlight-dev-0.0.1b5/spotlight/core/pipeline/abstract.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b4/spotlight/core/pipeline/decorator.py` & `spotlight-dev-0.0.1b5/spotlight/core/pipeline/decorator.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b4/spotlight/core/pipeline/execution/rule/abstract.py` & `spotlight-dev-0.0.1b5/spotlight/core/pipeline/execution/rule/abstract.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b4/spotlight/core/pipeline/execution/rule/sql_rule.py` & `spotlight-dev-0.0.1b5/spotlight/core/pipeline/execution/rule/sql_rule.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b4/spotlight/core/pipeline/execution/synchronous.py` & `spotlight-dev-0.0.1b5/spotlight/core/pipeline/execution/synchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b4/spotlight/core/pipeline/model/pipeline.py` & `spotlight-dev-0.0.1b5/spotlight/core/pipeline/model/pipeline.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b4/spotlight/core/pipeline/runner/__init__.py` & `spotlight-dev-0.0.1b5/spotlight/core/pipeline/runner/__init__.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b4/spotlight/core/pipeline/runner/utils/asynchronously.py` & `spotlight-dev-0.0.1b5/spotlight/core/pipeline/runner/utils/asynchronously.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b4/spotlight/core/pipeline/runner/utils/synchronously.py` & `spotlight-dev-0.0.1b5/spotlight/core/pipeline/runner/utils/synchronously.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b4/spotlight/pandas/__util.py` & `spotlight-dev-0.0.1b5/spotlight/pandas/__util.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b4/spotlight/pandas/pipeline.py` & `spotlight-dev-0.0.1b5/spotlight/pandas/pipeline.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b4/spotlight/pandas/runners.py` & `spotlight-dev-0.0.1b5/spotlight/pandas/runners.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b4/spotlight_dev.egg-info/PKG-INFO` & `spotlight-dev-0.0.1b5/spotlight_dev.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotlight-dev
-Version: 0.0.1b4
+Version: 0.0.1b5
 Summary: Spotlight Python SDK
 Home-page: https://alpha.dev
 Author: Spotlight
 Author-email: hello@spotlight.dev
 License: UNKNOWN
 Description: # Spotlight: The data quality platform for developers
```

### Comparing `spotlight-dev-0.0.1b4/spotlight_dev.egg-info/SOURCES.txt` & `spotlight-dev-0.0.1b5/spotlight_dev.egg-info/SOURCES.txt`

 * *Files identical despite different names*

