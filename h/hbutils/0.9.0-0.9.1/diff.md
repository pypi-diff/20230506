# Comparing `tmp/hbutils-0.9.0.tar.gz` & `tmp/hbutils-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hbutils-0.9.0.tar", last modified: Mon Apr 17 06:11:04 2023, max compression
+gzip compressed data, was "hbutils-0.9.1.tar", last modified: Sat May  6 06:21:58 2023, max compression
```

## Comparing `hbutils-0.9.0.tar` & `hbutils-0.9.1.tar`

### file list

```diff
@@ -1,150 +1,151 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:11:04.438920 hbutils-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-17 06:08:39.000000 hbutils-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6485 2023-04-17 06:11:04.438920 hbutils-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5526 2023-04-17 06:08:39.000000 hbutils-0.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:11:04.402920 hbutils-0.9.0/hbutils/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-17 06:08:39.000000 hbutils-0.9.0/hbutils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:11:04.402920 hbutils-0.9.0/hbutils/algorithm/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-17 06:08:39.000000 hbutils-0.9.0/hbutils/algorithm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-04-17 06:08:39.000000 hbutils-0.9.0/hbutils/algorithm/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     6018 2023-04-17 06:08:39.000000 hbutils-0.9.0/hbutils/algorithm/topological.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:11:04.406920 hbutils-0.9.0/hbutils/binary/
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-17 06:08:39.000000 hbutils-0.9.0/hbutils/binary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-04-17 06:08:39.000000 hbutils-0.9.0/hbutils/binary/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-04-17 06:08:39.000000 hbutils-0.9.0/hbutils/binary/bool.py
--rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-04-17 06:08:39.000000 hbutils-0.9.0/hbutils/binary/buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-04-17 06:08:39.000000 hbutils-0.9.0/hbutils/binary/float.py
--rw-r--r--   0 runner    (1001) docker     (123)     5406 2023-04-17 06:08:39.000000 hbutils-0.9.0/hbutils/binary/int.py
--rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-04-17 06:08:39.000000 hbutils-0.9.0/hbutils/binary/str.py
--rw-r--r--   0 runner    (1001) docker     (123)     5314 2023-04-17 06:08:39.000000 hbutils-0.9.0/hbutils/binary/uint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:11:04.410920 hbutils-0.9.0/hbutils/collection/
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-17 06:08:39.000000 hbutils-0.9.0/hbutils/collection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-04-17 06:08:39.000000 hbutils-0.9.0/hbutils/collection/dimension.py
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-04-17 06:08:39.000000 hbutils-0.9.0/hbutils/collection/functional.py
--rw-r--r--   0 runner    (1001) docker     (123)     8601 2023-04-17 06:08:39.000000 hbutils-0.9.0/hbutils/collection/recover.py
--rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-04-17 06:08:39.000000 hbutils-0.9.0/hbutils/collection/sequence.py
--rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-04-17 06:08:39.000000 hbutils-0.9.0/hbutils/collection/stacked.py
--rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-04-17 06:08:39.000000 hbutils-0.9.0/hbutils/collection/structural.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:11:04.410920 hbutils-0.9.0/hbutils/color/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-17 06:08:39.000000 hbutils-0.9.0/hbutils/color/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4789 2023-04-17 06:08:39.000000 hbutils-0.9.0/hbutils/color/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    22809 2023-04-17 06:08:39.000000 hbutils-0.9.0/hbutils/color/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     6076 2023-04-17 06:08:39.000000 hbutils-0.9.0/hbutils/color/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:11:04.410920 hbutils-0.9.0/hbutils/config/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-17 06:08:39.000000 hbutils-0.9.0/hbutils/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-17 06:08:39.000000 hbutils-0.9.0/hbutils/config/meta.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:11:04.410920 hbutils-0.9.0/hbutils/design/
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-17 06:08:39.000000 hbutils-0.9.0/hbutils/design/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-04-17 06:08:39.000000 hbutils-0.9.0/hbutils/design/decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-04-17 06:08:39.000000 hbutils-0.9.0/hbutils/design/final.py
--rw-r--r--   0 runner    (1001) docker     (123)     7049 2023-04-17 06:08:39.000000 hbutils-0.9.0/hbutils/design/observer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4328 2023-04-17 06:08:39.000000 hbutils-0.9.0/hbutils/design/singleton.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:11:04.414920 hbutils-0.9.0/hbutils/encoding/
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-17 06:08:39.000000 hbutils-0.9.0/hbutils/encoding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-04-17 06:08:39.000000 hbutils-0.9.0/hbutils/encoding/ansi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-04-17 06:08:39.000000 hbutils-0.9.0/hbutils/encoding/base64.py
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-04-17 06:08:39.000000 hbutils-0.9.0/hbutils/encoding/decode.py
--rw-r--r--   0 runner    (1001) docker     (123)     4325 2023-04-17 06:08:39.000000 hbutils-0.9.0/hbutils/encoding/hash.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:11:04.414920 hbutils-0.9.0/hbutils/expression/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-17 06:08:39.000000 hbutils-0.9.0/hbutils/expression/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:11:04.414920 hbutils-0.9.0/hbutils/expression/native/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-17 06:08:39.000000 hbutils-0.9.0/hbutils/expression/native/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2994 2023-04-17 06:08:39.000000 hbutils-0.9.0/hbutils/expression/native/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6548 2023-04-17 06:08:39.000000 hbutils-0.9.0/hbutils/expression/native/feature.py
--rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-04-17 06:08:39.000000 hbutils-0.9.0/hbutils/expression/native/general.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:11:04.414920 hbutils-0.9.0/hbutils/file/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-17 06:08:39.000000 hbutils-0.9.0/hbutils/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-04-17 06:08:39.000000 hbutils-0.9.0/hbutils/file/stream.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:11:04.418920 hbutils-0.9.0/hbutils/model/
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-17 06:08:39.000000 hbutils-0.9.0/hbutils/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-17 06:08:39.000000 hbutils-0.9.0/hbutils/model/_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    12988 2023-04-17 06:08:39.000000 hbutils-0.9.0/hbutils/model/clazz.py
--rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-04-17 06:08:39.000000 hbutils-0.9.0/hbutils/model/compare.py
--rw-r--r--   0 runner    (1001) docker     (123)     6100 2023-04-17 06:08:39.000000 hbutils-0.9.0/hbutils/model/enum.py
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-04-17 06:08:39.000000 hbutils-0.9.0/hbutils/model/raw.py
--rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-04-17 06:08:39.000000 hbutils-0.9.0/hbutils/model/repr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:11:04.418920 hbutils-0.9.0/hbutils/random/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-17 06:08:39.000000 hbutils-0.9.0/hbutils/random/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-04-17 06:08:39.000000 hbutils-0.9.0/hbutils/random/binary.py
--rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-04-17 06:08:39.000000 hbutils-0.9.0/hbutils/random/sequence.py
--rw-r--r--   0 runner    (1001) docker     (123)     9022 2023-04-17 06:08:39.000000 hbutils-0.9.0/hbutils/random/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     7601 2023-04-17 06:08:39.000000 hbutils-0.9.0/hbutils/random/string.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:11:04.422920 hbutils-0.9.0/hbutils/reflection/
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-17 06:08:39.000000 hbutils-0.9.0/hbutils/reflection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-04-17 06:08:39.000000 hbutils-0.9.0/hbutils/reflection/clazz.py
--rw-r--r--   0 runner    (1001) docker     (123)    11549 2023-04-17 06:08:39.000000 hbutils-0.9.0/hbutils/reflection/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-04-17 06:08:39.000000 hbutils-0.9.0/hbutils/reflection/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)    14483 2023-04-17 06:08:39.000000 hbutils-0.9.0/hbutils/reflection/func.py
--rw-r--r--   0 runner    (1001) docker     (123)     4093 2023-04-17 06:08:39.000000 hbutils-0.9.0/hbutils/reflection/imports.py
--rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-04-17 06:08:39.000000 hbutils-0.9.0/hbutils/reflection/iter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3963 2023-04-17 06:08:39.000000 hbutils-0.9.0/hbutils/reflection/module.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:11:04.422920 hbutils-0.9.0/hbutils/scale/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-17 06:08:39.000000 hbutils-0.9.0/hbutils/scale/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-04-17 06:08:39.000000 hbutils-0.9.0/hbutils/scale/size.py
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-04-17 06:08:39.000000 hbutils-0.9.0/hbutils/scale/time.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:11:04.426920 hbutils-0.9.0/hbutils/string/
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-17 06:08:39.000000 hbutils-0.9.0/hbutils/string/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13096 2023-04-17 06:08:39.000000 hbutils-0.9.0/hbutils/string/inflection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-04-17 06:08:39.000000 hbutils-0.9.0/hbutils/string/plural.py
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-04-17 06:08:39.000000 hbutils-0.9.0/hbutils/string/template.py
--rw-r--r--   0 runner    (1001) docker     (123)     4397 2023-04-17 06:08:39.000000 hbutils-0.9.0/hbutils/string/tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-04-17 06:08:39.000000 hbutils-0.9.0/hbutils/string/trunc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:11:04.426920 hbutils-0.9.0/hbutils/system/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-17 06:08:39.000000 hbutils-0.9.0/hbutils/system/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:11:04.426920 hbutils-0.9.0/hbutils/system/filesystem/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-17 06:08:39.000000 hbutils-0.9.0/hbutils/system/filesystem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-04-17 06:08:39.000000 hbutils-0.9.0/hbutils/system/filesystem/binary.py
--rw-r--r--   0 runner    (1001) docker     (123)     5664 2023-04-17 06:08:39.000000 hbutils-0.9.0/hbutils/system/filesystem/directory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-04-17 06:08:39.000000 hbutils-0.9.0/hbutils/system/filesystem/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-04-17 06:08:39.000000 hbutils-0.9.0/hbutils/system/filesystem/tempfile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:11:04.426920 hbutils-0.9.0/hbutils/system/network/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-17 06:08:39.000000 hbutils-0.9.0/hbutils/system/network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-04-17 06:08:39.000000 hbutils-0.9.0/hbutils/system/network/hosts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-04-17 06:08:39.000000 hbutils-0.9.0/hbutils/system/network/port.py
--rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-04-17 06:08:39.000000 hbutils-0.9.0/hbutils/system/network/url.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:11:04.430920 hbutils-0.9.0/hbutils/system/os/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-17 06:08:39.000000 hbutils-0.9.0/hbutils/system/os/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-04-17 06:08:39.000000 hbutils-0.9.0/hbutils/system/os/executable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-04-17 06:08:39.000000 hbutils-0.9.0/hbutils/system/os/type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:11:04.430920 hbutils-0.9.0/hbutils/system/python/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-17 06:08:39.000000 hbutils-0.9.0/hbutils/system/python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-04-17 06:08:39.000000 hbutils-0.9.0/hbutils/system/python/implementation.py
--rw-r--r--   0 runner    (1001) docker     (123)    10379 2023-04-17 06:08:39.000000 hbutils-0.9.0/hbutils/system/python/package.py
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-04-17 06:08:39.000000 hbutils-0.9.0/hbutils/system/python/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:11:04.430920 hbutils-0.9.0/hbutils/testing/
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-17 06:08:39.000000 hbutils-0.9.0/hbutils/testing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:11:04.430920 hbutils-0.9.0/hbutils/testing/capture/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-17 06:08:39.000000 hbutils-0.9.0/hbutils/testing/capture/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-04-17 06:08:39.000000 hbutils-0.9.0/hbutils/testing/capture/exit.py
--rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-04-17 06:08:39.000000 hbutils-0.9.0/hbutils/testing/capture/output.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:11:04.430920 hbutils-0.9.0/hbutils/testing/compare/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-17 06:08:39.000000 hbutils-0.9.0/hbutils/testing/compare/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11727 2023-04-17 06:08:39.000000 hbutils-0.9.0/hbutils/testing/compare/text.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:11:04.434920 hbutils-0.9.0/hbutils/testing/generator/
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-17 06:08:39.000000 hbutils-0.9.0/hbutils/testing/generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7776 2023-04-17 06:08:39.000000 hbutils-0.9.0/hbutils/testing/generator/aetg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-04-17 06:08:39.000000 hbutils-0.9.0/hbutils/testing/generator/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-04-17 06:08:39.000000 hbutils-0.9.0/hbutils/testing/generator/func.py
--rw-r--r--   0 runner    (1001) docker     (123)     4225 2023-04-17 06:08:39.000000 hbutils-0.9.0/hbutils/testing/generator/matrix.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:11:04.434920 hbutils-0.9.0/hbutils/testing/isolated/
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-17 06:08:39.000000 hbutils-0.9.0/hbutils/testing/isolated/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-04-17 06:08:39.000000 hbutils-0.9.0/hbutils/testing/isolated/directory.py
--rw-r--r--   0 runner    (1001) docker     (123)    11485 2023-04-17 06:08:39.000000 hbutils-0.9.0/hbutils/testing/isolated/entry_point.py
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-04-17 06:08:39.000000 hbutils-0.9.0/hbutils/testing/isolated/input.py
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-04-17 06:08:39.000000 hbutils-0.9.0/hbutils/testing/isolated/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:11:04.434920 hbutils-0.9.0/hbutils/testing/requires/
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-04-17 06:08:39.000000 hbutils-0.9.0/hbutils/testing/requires/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-04-17 06:08:39.000000 hbutils-0.9.0/hbutils/testing/requires/cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     5725 2023-04-17 06:08:39.000000 hbutils-0.9.0/hbutils/testing/requires/expr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-04-17 06:08:39.000000 hbutils-0.9.0/hbutils/testing/requires/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:11:04.438920 hbutils-0.9.0/hbutils/testing/simulate/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-17 06:08:39.000000 hbutils-0.9.0/hbutils/testing/simulate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6486 2023-04-17 06:08:39.000000 hbutils-0.9.0/hbutils/testing/simulate/entry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:11:04.402920 hbutils-0.9.0/hbutils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6485 2023-04-17 06:11:04.000000 hbutils-0.9.0/hbutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-04-17 06:11:04.000000 hbutils-0.9.0/hbutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 06:11:04.000000 hbutils-0.9.0/hbutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-04-17 06:11:04.000000 hbutils-0.9.0/hbutils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-17 06:11:04.000000 hbutils-0.9.0/hbutils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 06:11:04.438920 hbutils-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-04-17 06:08:39.000000 hbutils-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 06:21:58.791018 hbutils-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-06 06:19:15.000000 hbutils-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6528 2023-05-06 06:21:58.791018 hbutils-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5526 2023-05-06 06:19:15.000000 hbutils-0.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 06:21:58.727017 hbutils-0.9.1/hbutils/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-06 06:19:15.000000 hbutils-0.9.1/hbutils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 06:21:58.731017 hbutils-0.9.1/hbutils/algorithm/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-06 06:19:15.000000 hbutils-0.9.1/hbutils/algorithm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-05-06 06:19:15.000000 hbutils-0.9.1/hbutils/algorithm/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6018 2023-05-06 06:19:15.000000 hbutils-0.9.1/hbutils/algorithm/topological.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 06:21:58.735017 hbutils-0.9.1/hbutils/binary/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-06 06:19:15.000000 hbutils-0.9.1/hbutils/binary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-05-06 06:19:15.000000 hbutils-0.9.1/hbutils/binary/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-05-06 06:19:15.000000 hbutils-0.9.1/hbutils/binary/bool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-05-06 06:19:15.000000 hbutils-0.9.1/hbutils/binary/buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-05-06 06:19:15.000000 hbutils-0.9.1/hbutils/binary/float.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5406 2023-05-06 06:19:15.000000 hbutils-0.9.1/hbutils/binary/int.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-05-06 06:19:15.000000 hbutils-0.9.1/hbutils/binary/str.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5314 2023-05-06 06:19:15.000000 hbutils-0.9.1/hbutils/binary/uint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 06:21:58.739017 hbutils-0.9.1/hbutils/collection/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-06 06:19:15.000000 hbutils-0.9.1/hbutils/collection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-05-06 06:19:15.000000 hbutils-0.9.1/hbutils/collection/dimension.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-05-06 06:19:15.000000 hbutils-0.9.1/hbutils/collection/functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8601 2023-05-06 06:19:15.000000 hbutils-0.9.1/hbutils/collection/recover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-05-06 06:19:15.000000 hbutils-0.9.1/hbutils/collection/sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-05-06 06:19:15.000000 hbutils-0.9.1/hbutils/collection/stacked.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-05-06 06:19:15.000000 hbutils-0.9.1/hbutils/collection/structural.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 06:21:58.743017 hbutils-0.9.1/hbutils/color/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-06 06:19:15.000000 hbutils-0.9.1/hbutils/color/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4789 2023-05-06 06:19:15.000000 hbutils-0.9.1/hbutils/color/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22809 2023-05-06 06:19:15.000000 hbutils-0.9.1/hbutils/color/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6076 2023-05-06 06:19:15.000000 hbutils-0.9.1/hbutils/color/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 06:21:58.743017 hbutils-0.9.1/hbutils/config/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-06 06:19:15.000000 hbutils-0.9.1/hbutils/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-06 06:19:15.000000 hbutils-0.9.1/hbutils/config/meta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 06:21:58.747017 hbutils-0.9.1/hbutils/design/
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-06 06:19:15.000000 hbutils-0.9.1/hbutils/design/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-05-06 06:19:15.000000 hbutils-0.9.1/hbutils/design/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-05-06 06:19:15.000000 hbutils-0.9.1/hbutils/design/final.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7049 2023-05-06 06:19:15.000000 hbutils-0.9.1/hbutils/design/observer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4328 2023-05-06 06:19:15.000000 hbutils-0.9.1/hbutils/design/singleton.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 06:21:58.751017 hbutils-0.9.1/hbutils/encoding/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-06 06:19:15.000000 hbutils-0.9.1/hbutils/encoding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-06 06:19:15.000000 hbutils-0.9.1/hbutils/encoding/ansi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-05-06 06:19:15.000000 hbutils-0.9.1/hbutils/encoding/base64.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-05-06 06:19:15.000000 hbutils-0.9.1/hbutils/encoding/decode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4325 2023-05-06 06:19:15.000000 hbutils-0.9.1/hbutils/encoding/hash.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 06:21:58.751017 hbutils-0.9.1/hbutils/expression/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-06 06:19:15.000000 hbutils-0.9.1/hbutils/expression/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 06:21:58.751017 hbutils-0.9.1/hbutils/expression/native/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-06 06:19:15.000000 hbutils-0.9.1/hbutils/expression/native/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2994 2023-05-06 06:19:15.000000 hbutils-0.9.1/hbutils/expression/native/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6548 2023-05-06 06:19:15.000000 hbutils-0.9.1/hbutils/expression/native/feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-05-06 06:19:15.000000 hbutils-0.9.1/hbutils/expression/native/general.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 06:21:58.755017 hbutils-0.9.1/hbutils/file/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-06 06:19:15.000000 hbutils-0.9.1/hbutils/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-05-06 06:19:15.000000 hbutils-0.9.1/hbutils/file/stream.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 06:21:58.759017 hbutils-0.9.1/hbutils/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-06 06:19:15.000000 hbutils-0.9.1/hbutils/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-06 06:19:15.000000 hbutils-0.9.1/hbutils/model/_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12988 2023-05-06 06:19:15.000000 hbutils-0.9.1/hbutils/model/clazz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-05-06 06:19:15.000000 hbutils-0.9.1/hbutils/model/compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6100 2023-05-06 06:19:15.000000 hbutils-0.9.1/hbutils/model/enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-05-06 06:19:15.000000 hbutils-0.9.1/hbutils/model/raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-05-06 06:19:15.000000 hbutils-0.9.1/hbutils/model/repr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 06:21:58.759017 hbutils-0.9.1/hbutils/random/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-06 06:19:15.000000 hbutils-0.9.1/hbutils/random/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-05-06 06:19:15.000000 hbutils-0.9.1/hbutils/random/binary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-05-06 06:19:15.000000 hbutils-0.9.1/hbutils/random/sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9022 2023-05-06 06:19:15.000000 hbutils-0.9.1/hbutils/random/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7601 2023-05-06 06:19:15.000000 hbutils-0.9.1/hbutils/random/string.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 06:21:58.767017 hbutils-0.9.1/hbutils/reflection/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-06 06:19:15.000000 hbutils-0.9.1/hbutils/reflection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-05-06 06:19:15.000000 hbutils-0.9.1/hbutils/reflection/clazz.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11549 2023-05-06 06:19:15.000000 hbutils-0.9.1/hbutils/reflection/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-06 06:19:15.000000 hbutils-0.9.1/hbutils/reflection/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14483 2023-05-06 06:19:15.000000 hbutils-0.9.1/hbutils/reflection/func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4093 2023-05-06 06:19:15.000000 hbutils-0.9.1/hbutils/reflection/imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-05-06 06:19:15.000000 hbutils-0.9.1/hbutils/reflection/iter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3963 2023-05-06 06:19:15.000000 hbutils-0.9.1/hbutils/reflection/module.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 06:21:58.767017 hbutils-0.9.1/hbutils/scale/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-06 06:19:15.000000 hbutils-0.9.1/hbutils/scale/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-05-06 06:19:15.000000 hbutils-0.9.1/hbutils/scale/size.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-05-06 06:19:15.000000 hbutils-0.9.1/hbutils/scale/time.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 06:21:58.771018 hbutils-0.9.1/hbutils/string/
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-06 06:19:15.000000 hbutils-0.9.1/hbutils/string/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13096 2023-05-06 06:19:15.000000 hbutils-0.9.1/hbutils/string/inflection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-05-06 06:19:15.000000 hbutils-0.9.1/hbutils/string/plural.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-05-06 06:19:15.000000 hbutils-0.9.1/hbutils/string/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4397 2023-05-06 06:19:15.000000 hbutils-0.9.1/hbutils/string/tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-05-06 06:19:15.000000 hbutils-0.9.1/hbutils/string/trunc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 06:21:58.771018 hbutils-0.9.1/hbutils/system/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-06 06:19:15.000000 hbutils-0.9.1/hbutils/system/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 06:21:58.775018 hbutils-0.9.1/hbutils/system/filesystem/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-06 06:19:15.000000 hbutils-0.9.1/hbutils/system/filesystem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-05-06 06:19:15.000000 hbutils-0.9.1/hbutils/system/filesystem/binary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5664 2023-05-06 06:19:15.000000 hbutils-0.9.1/hbutils/system/filesystem/directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-05-06 06:19:15.000000 hbutils-0.9.1/hbutils/system/filesystem/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-05-06 06:19:15.000000 hbutils-0.9.1/hbutils/system/filesystem/tempfile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 06:21:58.775018 hbutils-0.9.1/hbutils/system/network/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-06 06:19:15.000000 hbutils-0.9.1/hbutils/system/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-05-06 06:19:15.000000 hbutils-0.9.1/hbutils/system/network/hosts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-05-06 06:19:15.000000 hbutils-0.9.1/hbutils/system/network/port.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-05-06 06:19:15.000000 hbutils-0.9.1/hbutils/system/network/telnet_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-05-06 06:19:15.000000 hbutils-0.9.1/hbutils/system/network/url.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 06:21:58.779018 hbutils-0.9.1/hbutils/system/os/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-06 06:19:15.000000 hbutils-0.9.1/hbutils/system/os/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-05-06 06:19:15.000000 hbutils-0.9.1/hbutils/system/os/executable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-05-06 06:19:15.000000 hbutils-0.9.1/hbutils/system/os/type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 06:21:58.779018 hbutils-0.9.1/hbutils/system/python/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-06 06:19:15.000000 hbutils-0.9.1/hbutils/system/python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-05-06 06:19:15.000000 hbutils-0.9.1/hbutils/system/python/implementation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10379 2023-05-06 06:19:15.000000 hbutils-0.9.1/hbutils/system/python/package.py
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-06 06:19:15.000000 hbutils-0.9.1/hbutils/system/python/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 06:21:58.779018 hbutils-0.9.1/hbutils/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-06 06:19:15.000000 hbutils-0.9.1/hbutils/testing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 06:21:58.783018 hbutils-0.9.1/hbutils/testing/capture/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-06 06:19:15.000000 hbutils-0.9.1/hbutils/testing/capture/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-05-06 06:19:15.000000 hbutils-0.9.1/hbutils/testing/capture/exit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-05-06 06:19:15.000000 hbutils-0.9.1/hbutils/testing/capture/output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 06:21:58.783018 hbutils-0.9.1/hbutils/testing/compare/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-06 06:19:15.000000 hbutils-0.9.1/hbutils/testing/compare/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11727 2023-05-06 06:19:15.000000 hbutils-0.9.1/hbutils/testing/compare/text.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 06:21:58.787018 hbutils-0.9.1/hbutils/testing/generator/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-06 06:19:15.000000 hbutils-0.9.1/hbutils/testing/generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7776 2023-05-06 06:19:15.000000 hbutils-0.9.1/hbutils/testing/generator/aetg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-05-06 06:19:15.000000 hbutils-0.9.1/hbutils/testing/generator/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-05-06 06:19:15.000000 hbutils-0.9.1/hbutils/testing/generator/func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4225 2023-05-06 06:19:15.000000 hbutils-0.9.1/hbutils/testing/generator/matrix.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 06:21:58.787018 hbutils-0.9.1/hbutils/testing/isolated/
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-06 06:19:15.000000 hbutils-0.9.1/hbutils/testing/isolated/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-05-06 06:19:15.000000 hbutils-0.9.1/hbutils/testing/isolated/directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11485 2023-05-06 06:19:15.000000 hbutils-0.9.1/hbutils/testing/isolated/entry_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-05-06 06:19:15.000000 hbutils-0.9.1/hbutils/testing/isolated/input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-05-06 06:19:15.000000 hbutils-0.9.1/hbutils/testing/isolated/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 06:21:58.791018 hbutils-0.9.1/hbutils/testing/requires/
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-06 06:19:15.000000 hbutils-0.9.1/hbutils/testing/requires/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-05-06 06:19:15.000000 hbutils-0.9.1/hbutils/testing/requires/cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5725 2023-05-06 06:19:15.000000 hbutils-0.9.1/hbutils/testing/requires/expr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-05-06 06:19:15.000000 hbutils-0.9.1/hbutils/testing/requires/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 06:21:58.791018 hbutils-0.9.1/hbutils/testing/simulate/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-06 06:19:15.000000 hbutils-0.9.1/hbutils/testing/simulate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6486 2023-05-06 06:19:15.000000 hbutils-0.9.1/hbutils/testing/simulate/entry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 06:21:58.731017 hbutils-0.9.1/hbutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6528 2023-05-06 06:21:58.000000 hbutils-0.9.1/hbutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-05-06 06:21:58.000000 hbutils-0.9.1/hbutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 06:21:58.000000 hbutils-0.9.1/hbutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-06 06:21:58.000000 hbutils-0.9.1/hbutils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-06 06:21:58.000000 hbutils-0.9.1/hbutils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 06:21:58.791018 hbutils-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-05-06 06:19:15.000000 hbutils-0.9.1/setup.py
```

### Comparing `hbutils-0.9.0/LICENSE` & `hbutils-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hbutils-0.9.0/PKG-INFO` & `hbutils-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: hbutils
-Version: 0.9.0
+Version: 0.9.1
 Summary: Some useful functions and classes in Python infrastructure development.
 Home-page: https://github.com/hansbug/hbutils
 Author: HansBug
 Author-email: hansbug@buaa.edu.cn
 License: Apache License, Version 2.0
-Keywords: Tree-structured Value Management
+Keywords: python,generic,utilities
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: doc
 License-File: LICENSE
```

### Comparing `hbutils-0.9.0/README.md` & `hbutils-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `hbutils-0.9.0/hbutils/algorithm/linear.py` & `hbutils-0.9.1/hbutils/algorithm/linear.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.9.0/hbutils/algorithm/topological.py` & `hbutils-0.9.1/hbutils/algorithm/topological.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.9.0/hbutils/binary/base.py` & `hbutils-0.9.1/hbutils/binary/base.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.9.0/hbutils/binary/bool.py` & `hbutils-0.9.1/hbutils/binary/bool.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.9.0/hbutils/binary/buffer.py` & `hbutils-0.9.1/hbutils/binary/buffer.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.9.0/hbutils/binary/float.py` & `hbutils-0.9.1/hbutils/binary/float.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.9.0/hbutils/binary/int.py` & `hbutils-0.9.1/hbutils/binary/int.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.9.0/hbutils/binary/str.py` & `hbutils-0.9.1/hbutils/binary/str.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.9.0/hbutils/binary/uint.py` & `hbutils-0.9.1/hbutils/binary/uint.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.9.0/hbutils/collection/dimension.py` & `hbutils-0.9.1/hbutils/collection/dimension.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.9.0/hbutils/collection/functional.py` & `hbutils-0.9.1/hbutils/collection/functional.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.9.0/hbutils/collection/recover.py` & `hbutils-0.9.1/hbutils/collection/recover.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.9.0/hbutils/collection/sequence.py` & `hbutils-0.9.1/hbutils/collection/sequence.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.9.0/hbutils/collection/stacked.py` & `hbutils-0.9.1/hbutils/collection/stacked.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.9.0/hbutils/collection/structural.py` & `hbutils-0.9.1/hbutils/collection/structural.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.9.0/hbutils/color/base.py` & `hbutils-0.9.1/hbutils/color/base.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.9.0/hbutils/color/model.py` & `hbutils-0.9.1/hbutils/color/model.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.9.0/hbutils/color/utils.py` & `hbutils-0.9.1/hbutils/color/utils.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.9.0/hbutils/design/decorator.py` & `hbutils-0.9.1/hbutils/design/decorator.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.9.0/hbutils/design/final.py` & `hbutils-0.9.1/hbutils/design/final.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.9.0/hbutils/design/observer.py` & `hbutils-0.9.1/hbutils/design/observer.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.9.0/hbutils/design/singleton.py` & `hbutils-0.9.1/hbutils/design/singleton.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.9.0/hbutils/encoding/ansi.py` & `hbutils-0.9.1/hbutils/encoding/ansi.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.9.0/hbutils/encoding/base64.py` & `hbutils-0.9.1/hbutils/encoding/base64.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.9.0/hbutils/encoding/decode.py` & `hbutils-0.9.1/hbutils/encoding/decode.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.9.0/hbutils/encoding/hash.py` & `hbutils-0.9.1/hbutils/encoding/hash.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.9.0/hbutils/expression/native/base.py` & `hbutils-0.9.1/hbutils/expression/native/base.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.9.0/hbutils/expression/native/feature.py` & `hbutils-0.9.1/hbutils/expression/native/feature.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.9.0/hbutils/expression/native/general.py` & `hbutils-0.9.1/hbutils/expression/native/general.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.9.0/hbutils/file/stream.py` & `hbutils-0.9.1/hbutils/file/stream.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.9.0/hbutils/model/clazz.py` & `hbutils-0.9.1/hbutils/model/clazz.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.9.0/hbutils/model/compare.py` & `hbutils-0.9.1/hbutils/model/compare.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.9.0/hbutils/model/enum.py` & `hbutils-0.9.1/hbutils/model/enum.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.9.0/hbutils/model/raw.py` & `hbutils-0.9.1/hbutils/model/raw.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.9.0/hbutils/model/repr.py` & `hbutils-0.9.1/hbutils/model/repr.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.9.0/hbutils/random/binary.py` & `hbutils-0.9.1/hbutils/random/binary.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.9.0/hbutils/random/sequence.py` & `hbutils-0.9.1/hbutils/random/sequence.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.9.0/hbutils/random/state.py` & `hbutils-0.9.1/hbutils/random/state.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.9.0/hbutils/random/string.py` & `hbutils-0.9.1/hbutils/random/string.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.9.0/hbutils/reflection/clazz.py` & `hbutils-0.9.1/hbutils/reflection/clazz.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.9.0/hbutils/reflection/context.py` & `hbutils-0.9.1/hbutils/reflection/context.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.9.0/hbutils/reflection/exception.py` & `hbutils-0.9.1/hbutils/reflection/exception.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.9.0/hbutils/reflection/func.py` & `hbutils-0.9.1/hbutils/reflection/func.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.9.0/hbutils/reflection/imports.py` & `hbutils-0.9.1/hbutils/reflection/imports.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.9.0/hbutils/reflection/iter.py` & `hbutils-0.9.1/hbutils/reflection/iter.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.9.0/hbutils/reflection/module.py` & `hbutils-0.9.1/hbutils/reflection/module.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.9.0/hbutils/scale/size.py` & `hbutils-0.9.1/hbutils/scale/size.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.9.0/hbutils/scale/time.py` & `hbutils-0.9.1/hbutils/scale/time.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.9.0/hbutils/string/inflection.py` & `hbutils-0.9.1/hbutils/string/inflection.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.9.0/hbutils/string/plural.py` & `hbutils-0.9.1/hbutils/string/plural.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.9.0/hbutils/string/template.py` & `hbutils-0.9.1/hbutils/string/template.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.9.0/hbutils/string/tree.py` & `hbutils-0.9.1/hbutils/string/tree.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.9.0/hbutils/string/trunc.py` & `hbutils-0.9.1/hbutils/string/trunc.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.9.0/hbutils/system/filesystem/binary.py` & `hbutils-0.9.1/hbutils/system/filesystem/binary.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.9.0/hbutils/system/filesystem/directory.py` & `hbutils-0.9.1/hbutils/system/filesystem/directory.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.9.0/hbutils/system/filesystem/file.py` & `hbutils-0.9.1/hbutils/system/filesystem/file.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.9.0/hbutils/system/filesystem/tempfile.py` & `hbutils-0.9.1/hbutils/system/filesystem/tempfile.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.9.0/hbutils/system/network/hosts.py` & `hbutils-0.9.1/hbutils/system/network/hosts.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.9.0/hbutils/system/network/port.py` & `hbutils-0.9.1/hbutils/system/network/port.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.9.0/hbutils/system/network/url.py` & `hbutils-0.9.1/hbutils/system/network/url.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.9.0/hbutils/system/os/executable.py` & `hbutils-0.9.1/hbutils/system/os/executable.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,15 +5,18 @@
     Based on `hweickert/where <https://github.com/hweickert/where>`_, \
     and this version below will be long-term maintained here.
 """
 import itertools
 import os
 from typing import Iterable, Iterator, Optional, List
 
+from deprecation import deprecated
+
 from .type import is_windows
+from ...config.meta import __VERSION__
 
 __all__ = [
     'where', 'which',
 ]
 
 
 def where(execfile: str) -> List[str]:
@@ -33,14 +36,16 @@
         ['/usr/bin/bash', '/bin/bash']
         >>> where('not_installed')
         []
     """
     return list(_iter_where(execfile))
 
 
+@deprecated(deprecated_in="0.9", removed_in="1.0", current_version=__VERSION__,
+            details="Use the native :func:`shutil.which` instead")
 def which(execfile: str) -> Optional[str]:
     """
     Overview:
         Returns first matching file path, which is the one when we operate in terminal.
 
     :param execfile: Executable file to locate (such as ``python``).
     :return: Absolute path fo the executable file.
```

### Comparing `hbutils-0.9.0/hbutils/system/os/type.py` & `hbutils-0.9.1/hbutils/system/os/type.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.9.0/hbutils/system/python/implementation.py` & `hbutils-0.9.1/hbutils/system/python/implementation.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.9.0/hbutils/system/python/package.py` & `hbutils-0.9.1/hbutils/system/python/package.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.9.0/hbutils/testing/capture/exit.py` & `hbutils-0.9.1/hbutils/testing/capture/exit.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.9.0/hbutils/testing/capture/output.py` & `hbutils-0.9.1/hbutils/testing/capture/output.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.9.0/hbutils/testing/compare/text.py` & `hbutils-0.9.1/hbutils/testing/compare/text.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.9.0/hbutils/testing/generator/aetg.py` & `hbutils-0.9.1/hbutils/testing/generator/aetg.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.9.0/hbutils/testing/generator/base.py` & `hbutils-0.9.1/hbutils/testing/generator/base.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.9.0/hbutils/testing/generator/func.py` & `hbutils-0.9.1/hbutils/testing/generator/func.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.9.0/hbutils/testing/generator/matrix.py` & `hbutils-0.9.1/hbutils/testing/generator/matrix.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.9.0/hbutils/testing/isolated/directory.py` & `hbutils-0.9.1/hbutils/testing/isolated/directory.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.9.0/hbutils/testing/isolated/entry_point.py` & `hbutils-0.9.1/hbutils/testing/isolated/entry_point.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.9.0/hbutils/testing/isolated/input.py` & `hbutils-0.9.1/hbutils/testing/isolated/input.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.9.0/hbutils/testing/isolated/logging.py` & `hbutils-0.9.1/hbutils/testing/isolated/logging.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.9.0/hbutils/testing/requires/cmd.py` & `hbutils-0.9.1/hbutils/testing/requires/cmd.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.9.0/hbutils/testing/requires/expr.py` & `hbutils-0.9.1/hbutils/testing/requires/expr.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.9.0/hbutils/testing/requires/version.py` & `hbutils-0.9.1/hbutils/testing/requires/version.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.9.0/hbutils/testing/simulate/entry.py` & `hbutils-0.9.1/hbutils/testing/simulate/entry.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.9.0/hbutils.egg-info/PKG-INFO` & `hbutils-0.9.1/hbutils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: hbutils
-Version: 0.9.0
+Version: 0.9.1
 Summary: Some useful functions and classes in Python infrastructure development.
 Home-page: https://github.com/hansbug/hbutils
 Author: HansBug
 Author-email: hansbug@buaa.edu.cn
 License: Apache License, Version 2.0
-Keywords: Tree-structured Value Management
+Keywords: python,generic,utilities
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: doc
 License-File: LICENSE
```

### Comparing `hbutils-0.9.0/hbutils.egg-info/SOURCES.txt` & `hbutils-0.9.1/hbutils.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -82,14 +82,15 @@
 hbutils/system/filesystem/binary.py
 hbutils/system/filesystem/directory.py
 hbutils/system/filesystem/file.py
 hbutils/system/filesystem/tempfile.py
 hbutils/system/network/__init__.py
 hbutils/system/network/hosts.py
 hbutils/system/network/port.py
+hbutils/system/network/telnet_.py
 hbutils/system/network/url.py
 hbutils/system/os/__init__.py
 hbutils/system/os/executable.py
 hbutils/system/os/type.py
 hbutils/system/python/__init__.py
 hbutils/system/python/implementation.py
 hbutils/system/python/package.py
```

### Comparing `hbutils-0.9.0/hbutils.egg-info/requires.txt` & `hbutils-0.9.1/hbutils.egg-info/requires.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 packaging>=21.3
 setuptools>=50.0
 pytimeparse>=1.1.8
 bitmath>=1.3.3.1
 chardet<5,>=3.0.4
+deprecation>=2.0.0
 
 [:python_version < "3.8"]
 importlib_metadata>=6.0.0
 
 [doc]
 Jinja2~=3.0.0
 sphinx~=3.2.0
```

### Comparing `hbutils-0.9.0/setup.py` & `hbutils-0.9.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     ),
     description=meta['__DESCRIPTION__'],
     long_description=readme,
     long_description_content_type='text/markdown',
     author=meta['__AUTHOR__'],
     author_email=meta['__AUTHOR_EMAIL__'],
     license='Apache License, Version 2.0',
-    keywords='Tree-structured Value Management',
+    keywords='python, generic, utilities',
     url='https://github.com/hansbug/hbutils',
 
     # environment
     python_requires=">=3.7",
     install_requires=requirements,
     tests_require=group_requirements['test'],
     extras_require=group_requirements,
@@ -56,10 +56,11 @@
         'License :: OSI Approved :: Apache Software License',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: Implementation :: PyPy'
     ],
 )
```

