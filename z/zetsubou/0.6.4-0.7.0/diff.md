# Comparing `tmp/zetsubou-0.6.4.tar.gz` & `tmp/zetsubou-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zetsubou-0.6.4.tar", last modified: Mon Nov  7 11:03:04 2022, max compression
+gzip compressed data, was "zetsubou-0.7.0.tar", last modified: Sat May  6 10:40:26 2023, max compression
```

## Comparing `zetsubou-0.6.4.tar` & `zetsubou-0.7.0.tar`

### file list

```diff
@@ -1,104 +1,106 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-07 11:03:04.363628 zetsubou-0.6.4/
--rw-r--r--   0 runner    (1001) docker     (121)     2849 2022-11-07 11:03:04.363628 zetsubou-0.6.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2397 2022-11-07 11:02:36.000000 zetsubou-0.6.4/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     1527 2022-11-07 11:02:36.000000 zetsubou-0.6.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-07 11:03:04.363628 zetsubou-0.6.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       37 2022-11-07 11:02:36.000000 zetsubou-0.6.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-07 11:03:04.355628 zetsubou-0.6.4/zetsubou/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-07 11:02:36.000000 zetsubou-0.6.4/zetsubou/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      927 2022-11-07 11:02:36.000000 zetsubou-0.6.4/zetsubou/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)      153 2022-11-07 11:02:36.000000 zetsubou-0.6.4/zetsubou/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-07 11:03:04.355628 zetsubou-0.6.4/zetsubou/commands/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-07 11:02:36.000000 zetsubou-0.6.4/zetsubou/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6152 2022-11-07 11:02:36.000000 zetsubou-0.6.4/zetsubou/commands/base_command.py
--rw-r--r--   0 runner    (1001) docker     (121)     6542 2022-11-07 11:02:36.000000 zetsubou-0.6.4/zetsubou/commands/build.py
--rw-r--r--   0 runner    (1001) docker     (121)     1407 2022-11-07 11:02:36.000000 zetsubou-0.6.4/zetsubou/commands/clean.py
--rw-r--r--   0 runner    (1001) docker     (121)     1244 2022-11-07 11:02:36.000000 zetsubou-0.6.4/zetsubou/commands/clean_build.py
--rw-r--r--   0 runner    (1001) docker     (121)     1918 2022-11-07 11:02:36.000000 zetsubou-0.6.4/zetsubou/commands/command_context.py
--rw-r--r--   0 runner    (1001) docker     (121)      789 2022-11-07 11:02:36.000000 zetsubou-0.6.4/zetsubou/commands/command_registry.py
--rw-r--r--   0 runner    (1001) docker     (121)      917 2022-11-07 11:02:36.000000 zetsubou-0.6.4/zetsubou/commands/config.py
--rw-r--r--   0 runner    (1001) docker     (121)     1896 2022-11-07 11:02:36.000000 zetsubou-0.6.4/zetsubou/commands/create.py
--rw-r--r--   0 runner    (1001) docker     (121)      730 2022-11-07 11:02:36.000000 zetsubou-0.6.4/zetsubou/commands/execute_stage.py
--rw-r--r--   0 runner    (1001) docker     (121)     7794 2022-11-07 11:02:36.000000 zetsubou-0.6.4/zetsubou/commands/generate.py
--rw-r--r--   0 runner    (1001) docker     (121)     5231 2022-11-07 11:02:36.000000 zetsubou-0.6.4/zetsubou/commands/install.py
--rw-r--r--   0 runner    (1001) docker     (121)     1223 2022-11-07 11:02:36.000000 zetsubou-0.6.4/zetsubou/commands/regen.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-07 11:03:04.355628 zetsubou-0.6.4/zetsubou/conan/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-07 11:02:36.000000 zetsubou-0.6.4/zetsubou/conan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1091 2022-11-07 11:02:36.000000 zetsubou-0.6.4/zetsubou/conan/conan.py
--rw-r--r--   0 runner    (1001) docker     (121)      239 2022-11-07 11:02:36.000000 zetsubou-0.6.4/zetsubou/conan/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (121)     5546 2022-11-07 11:02:36.000000 zetsubou-0.6.4/zetsubou/conan/from_conan.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-07 11:03:04.355628 zetsubou-0.6.4/zetsubou/conan/generator/
--rw-r--r--   0 runner    (1001) docker     (121)     4888 2022-11-07 11:02:36.000000 zetsubou-0.6.4/zetsubou/conan/generator/conanfile.py
--rw-r--r--   0 runner    (1001) docker     (121)     4282 2022-11-07 11:02:36.000000 zetsubou-0.6.4/zetsubou/conan/to_conan.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-07 11:02:36.000000 zetsubou-0.6.4/zetsubou/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-07 11:03:04.355628 zetsubou-0.6.4/zetsubou/data/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-07 11:02:36.000000 zetsubou-0.6.4/zetsubou/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-07 11:03:04.355628 zetsubou-0.6.4/zetsubou/data/rules/
--rw-r--r--   0 runner    (1001) docker     (121)     2608 2022-11-07 11:02:36.000000 zetsubou-0.6.4/zetsubou/data/rules/ClangRules.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2665 2022-11-07 11:02:36.000000 zetsubou-0.6.4/zetsubou/data/rules/MsvcRules.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-07 11:03:04.359628 zetsubou-0.6.4/zetsubou/fastbuild/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-07 11:02:36.000000 zetsubou-0.6.4/zetsubou/fastbuild/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1034 2022-11-07 11:02:36.000000 zetsubou-0.6.4/zetsubou/fastbuild/compiler.py
--rw-r--r--   0 runner    (1001) docker     (121)    45554 2022-11-07 11:02:36.000000 zetsubou-0.6.4/zetsubou/fastbuild/fastbuild_emit.py
--rw-r--r--   0 runner    (1001) docker     (121)    10399 2022-11-07 11:02:36.000000 zetsubou-0.6.4/zetsubou/fastbuild/target_kinds.py
--rw-r--r--   0 runner    (1001) docker     (121)      420 2022-11-07 11:02:36.000000 zetsubou-0.6.4/zetsubou/fastbuild/to_fastbuild.py
--rw-r--r--   0 runner    (1001) docker     (121)     7538 2022-11-07 11:02:36.000000 zetsubou-0.6.4/zetsubou/fastbuild/vcxproject.py
--rw-r--r--   0 runner    (1001) docker     (121)     2534 2022-11-07 11:02:36.000000 zetsubou-0.6.4/zetsubou/fastbuild/vssolution.py
--rw-r--r--   0 runner    (1001) docker     (121)      710 2022-11-07 11:02:36.000000 zetsubou-0.6.4/zetsubou/logo.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-07 11:03:04.359628 zetsubou-0.6.4/zetsubou/project/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-07 11:02:36.000000 zetsubou-0.6.4/zetsubou/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      303 2022-11-07 11:02:36.000000 zetsubou-0.6.4/zetsubou/project/base_context.py
--rw-r--r--   0 runner    (1001) docker     (121)     3093 2022-11-07 11:02:36.000000 zetsubou-0.6.4/zetsubou/project/config_matrix.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-07 11:03:04.359628 zetsubou-0.6.4/zetsubou/project/model/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-07 11:02:36.000000 zetsubou-0.6.4/zetsubou/project/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      113 2022-11-07 11:02:36.000000 zetsubou-0.6.4/zetsubou/project/model/config_string.py
--rw-r--r--   0 runner    (1001) docker     (121)      764 2022-11-07 11:02:36.000000 zetsubou-0.6.4/zetsubou/project/model/configuration.py
--rw-r--r--   0 runner    (1001) docker     (121)      265 2022-11-07 11:02:36.000000 zetsubou-0.6.4/zetsubou/project/model/configuration_enums.py
--rw-r--r--   0 runner    (1001) docker     (121)      339 2022-11-07 11:02:36.000000 zetsubou-0.6.4/zetsubou/project/model/filter.py
--rw-r--r--   0 runner    (1001) docker     (121)      476 2022-11-07 11:02:36.000000 zetsubou-0.6.4/zetsubou/project/model/kind.py
--rw-r--r--   0 runner    (1001) docker     (121)      231 2022-11-07 11:02:36.000000 zetsubou-0.6.4/zetsubou/project/model/platform.py
--rw-r--r--   0 runner    (1001) docker     (121)     1132 2022-11-07 11:02:36.000000 zetsubou-0.6.4/zetsubou/project/model/platform_data.py
--rw-r--r--   0 runner    (1001) docker     (121)      215 2022-11-07 11:02:36.000000 zetsubou-0.6.4/zetsubou/project/model/platform_enums.py
--rw-r--r--   0 runner    (1001) docker     (121)      935 2022-11-07 11:02:36.000000 zetsubou-0.6.4/zetsubou/project/model/project_template.py
--rw-r--r--   0 runner    (1001) docker     (121)      416 2022-11-07 11:02:36.000000 zetsubou-0.6.4/zetsubou/project/model/rule.py
--rw-r--r--   0 runner    (1001) docker     (121)      152 2022-11-07 11:02:36.000000 zetsubou-0.6.4/zetsubou/project/model/runtime_library.py
--rw-r--r--   0 runner    (1001) docker     (121)     2584 2022-11-07 11:02:36.000000 zetsubou-0.6.4/zetsubou/project/model/target.py
--rw-r--r--   0 runner    (1001) docker     (121)     8593 2022-11-07 11:02:36.000000 zetsubou-0.6.4/zetsubou/project/model/toolchain.py
--rw-r--r--   0 runner    (1001) docker     (121)      527 2022-11-07 11:02:36.000000 zetsubou-0.6.4/zetsubou/project/model/toolchain_enums.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-07 11:03:04.359628 zetsubou-0.6.4/zetsubou/project/runtime/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-07 11:02:36.000000 zetsubou-0.6.4/zetsubou/project/runtime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1945 2022-11-07 11:02:36.000000 zetsubou-0.6.4/zetsubou/project/runtime/emit.py
--rw-r--r--   0 runner    (1001) docker     (121)     3030 2022-11-07 11:02:36.000000 zetsubou-0.6.4/zetsubou/project/runtime/filter_toolchains.py
--rw-r--r--   0 runner    (1001) docker     (121)    17153 2022-11-07 11:02:36.000000 zetsubou-0.6.4/zetsubou/project/runtime/project_loader.py
--rw-r--r--   0 runner    (1001) docker     (121)    12890 2022-11-07 11:02:36.000000 zetsubou-0.6.4/zetsubou/project/runtime/resolve.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-07 11:03:04.359628 zetsubou-0.6.4/zetsubou/system/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-07 11:02:36.000000 zetsubou-0.6.4/zetsubou/system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2714 2022-11-07 11:02:36.000000 zetsubou-0.6.4/zetsubou/system/discover_toolchains.py
--rw-r--r--   0 runner    (1001) docker     (121)      925 2022-11-07 11:02:36.000000 zetsubou-0.6.4/zetsubou/system/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-07 11:03:04.359628 zetsubou-0.6.4/zetsubou/system/windows/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-07 11:02:36.000000 zetsubou-0.6.4/zetsubou/system/windows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      742 2022-11-07 11:02:36.000000 zetsubou-0.6.4/zetsubou/system/windows/msvc.py
--rw-r--r--   0 runner    (1001) docker     (121)      785 2022-11-07 11:02:36.000000 zetsubou-0.6.4/zetsubou/system/windows/vswhere.py
--rw-r--r--   0 runner    (1001) docker     (121)    18485 2022-11-07 11:02:36.000000 zetsubou-0.6.4/zetsubou/system/windows/windows.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-07 11:03:04.363628 zetsubou-0.6.4/zetsubou/utils/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-07 11:02:36.000000 zetsubou-0.6.4/zetsubou/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1044 2022-11-07 11:02:36.000000 zetsubou-0.6.4/zetsubou/utils/busy_indicator.py
--rw-r--r--   0 runner    (1001) docker     (121)     2229 2022-11-07 11:02:36.000000 zetsubou-0.6.4/zetsubou/utils/cmd_arguments.py
--rw-r--r--   0 runner    (1001) docker     (121)     2857 2022-11-07 11:02:36.000000 zetsubou-0.6.4/zetsubou/utils/common.py
--rw-r--r--   0 runner    (1001) docker     (121)      183 2022-11-07 11:02:36.000000 zetsubou-0.6.4/zetsubou/utils/dataclass_loader.py
--rw-r--r--   0 runner    (1001) docker     (121)       85 2022-11-07 11:02:36.000000 zetsubou-0.6.4/zetsubou/utils/error.py
--rw-r--r--   0 runner    (1001) docker     (121)      760 2022-11-07 11:02:36.000000 zetsubou-0.6.4/zetsubou/utils/error_codes.py
--rw-r--r--   0 runner    (1001) docker     (121)      390 2022-11-07 11:02:36.000000 zetsubou-0.6.4/zetsubou/utils/json_tools.py
--rw-r--r--   0 runner    (1001) docker     (121)     2678 2022-11-07 11:02:36.000000 zetsubou-0.6.4/zetsubou/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (121)     1923 2022-11-07 11:02:36.000000 zetsubou-0.6.4/zetsubou/utils/subprocess.py
--rw-r--r--   0 runner    (1001) docker     (121)      908 2022-11-07 11:02:36.000000 zetsubou-0.6.4/zetsubou/utils/yaml_loader.py
--rw-r--r--   0 runner    (1001) docker     (121)     1884 2022-11-07 11:02:36.000000 zetsubou-0.6.4/zetsubou/utils/yaml_simple_writer.py
--rw-r--r--   0 runner    (1001) docker     (121)      189 2022-11-07 11:02:36.000000 zetsubou-0.6.4/zetsubou/utils/yaml_tools.py
--rw-r--r--   0 runner    (1001) docker     (121)     2984 2022-11-07 11:02:36.000000 zetsubou-0.6.4/zetsubou/zetsubou.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-07 11:03:04.355628 zetsubou-0.6.4/zetsubou.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2849 2022-11-07 11:03:04.000000 zetsubou-0.6.4/zetsubou.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2737 2022-11-07 11:03:04.000000 zetsubou-0.6.4/zetsubou.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-07 11:03:04.000000 zetsubou-0.6.4/zetsubou.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       52 2022-11-07 11:03:04.000000 zetsubou-0.6.4/zetsubou.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      199 2022-11-07 11:03:04.000000 zetsubou-0.6.4/zetsubou.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-11-07 11:03:04.000000 zetsubou-0.6.4/zetsubou.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 10:40:26.097418 zetsubou-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-05-06 10:40:26.097418 zetsubou-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-05-06 10:40:10.000000 zetsubou-0.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-05-06 10:40:10.000000 zetsubou-0.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 10:40:26.097418 zetsubou-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-06 10:40:10.000000 zetsubou-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 10:40:26.085418 zetsubou-0.7.0/zetsubou/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 10:40:26.089418 zetsubou-0.7.0/zetsubou/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/commands/base_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6692 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/commands/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/commands/clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/commands/clean_build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/commands/command_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/commands/command_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/commands/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/commands/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/commands/execute_stage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8412 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/commands/generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5944 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/commands/install.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/commands/regen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 10:40:26.089418 zetsubou-0.7.0/zetsubou/conan/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/conan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/conan/conan.py
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/conan/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/conan/deployer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9725 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/conan/from_conan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/conan/to_conan.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 10:40:26.089418 zetsubou-0.7.0/zetsubou/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 10:40:26.089418 zetsubou-0.7.0/zetsubou/data/rules/
+-rw-r--r--   0 runner    (1001) docker     (123)     3306 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/data/rules/ClangRules.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/data/rules/MsvcRules.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 10:40:26.093418 zetsubou-0.7.0/zetsubou/fastbuild/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/fastbuild/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/fastbuild/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54351 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/fastbuild/fastbuild_emit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10396 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/fastbuild/target_kinds.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/fastbuild/to_fastbuild.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7538 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/fastbuild/vcxproject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/fastbuild/vssolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/logo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 10:40:26.093418 zetsubou-0.7.0/zetsubou/project/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/project/base_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/project/config_matrix.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 10:40:26.093418 zetsubou-0.7.0/zetsubou/project/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/project/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/project/model/cli_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/project/model/config_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/project/model/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/project/model/configuration_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/project/model/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/project/model/kind.py
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/project/model/platform.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/project/model/platform_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/project/model/project_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/project/model/rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/project/model/runtime_library.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/project/model/target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8906 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/project/model/toolchain.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/project/model/toolchain_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/project/model/toolchain_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/project/model/virtual_environment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 10:40:26.097418 zetsubou-0.7.0/zetsubou/project/runtime/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/project/runtime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/project/runtime/emit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10993 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/project/runtime/project_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13274 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/project/runtime/resolve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7995 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/project/runtime/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 10:40:26.097418 zetsubou-0.7.0/zetsubou/system/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7667 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/system/discover_toolchains.py
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/system/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 10:40:26.097418 zetsubou-0.7.0/zetsubou/system/windows/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/system/windows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/system/windows/msvc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/system/windows/vswhere.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18517 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/system/windows/windows.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 10:40:26.097418 zetsubou-0.7.0/zetsubou/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/utils/busy_indicator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/utils/cmd_arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/utils/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/utils/dataclass_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/utils/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/utils/error_codes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/utils/json_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/utils/subprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/utils/yaml_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/utils/yaml_simple_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/utils/yaml_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/zetsubou.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7855 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/zetsubou_conan_toolchain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 10:40:26.085418 zetsubou-0.7.0/zetsubou.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-05-06 10:40:26.000000 zetsubou-0.7.0/zetsubou.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-05-06 10:40:26.000000 zetsubou-0.7.0/zetsubou.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 10:40:26.000000 zetsubou-0.7.0/zetsubou.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-06 10:40:26.000000 zetsubou-0.7.0/zetsubou.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-06 10:40:26.000000 zetsubou-0.7.0/zetsubou.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-06 10:40:26.000000 zetsubou-0.7.0/zetsubou.egg-info/top_level.txt
```

### Comparing `zetsubou-0.6.4/PKG-INFO` & `zetsubou-0.7.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zetsubou
-Version: 0.6.4
+Version: 0.7.0
 Summary: FASTbuild generator for the helpless
 Author: BentouDev
 Project-URL: Homepage, https://github.com/BentouDev/Zetsubou
 Keywords: fastbuild,C++,cpp,C/C++,developer,tool
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `zetsubou-0.6.4/README.md` & `zetsubou-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `zetsubou-0.6.4/pyproject.toml` & `zetsubou-0.7.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 include = [ 'zetsubou*' ]
 
 [tool.setuptools.package-data]
 'zetsubou.data.rules' = ["*.yml"]
 
 [project]
 name = "zetsubou"
-version = "0.6.4"
+version = "0.7.0"
 description = "FASTbuild generator for the helpless"
 readme = "README.md"
 authors = [{ name = "BentouDev" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -40,18 +40,18 @@
 [project.urls]
 Homepage = "https://github.com/BentouDev/Zetsubou"
 
 [project.scripts]
 zetsubou = "zetsubou.zetsubou:main"
 
 [tool.bumpver]
-current_version = "0.6.4"
+current_version = "0.7.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "[bot] Bump version {old_version} -> {new_version}"
 commit = false
 tag = false
 push = false
 
 [tool.bumpver.file_patterns]
 "pyproject.toml" = [ 'current_version = "{version}"', 'version = "{version}"' ]
 "zetsubou/_version.py" = [ '__version__ = "{version}"' ]
-"zetsubou/conan/generator/conanfile.py" = [ 'version = "{version}"' ]
+"zetsubou/zetsubou_conan_toolchain.py" = [ 'version = "{version}"' ]
```

### Comparing `zetsubou-0.6.4/zetsubou/__main__.py` & `zetsubou-0.7.0/zetsubou/__main__.py`

 * *Files identical despite different names*

### Comparing `zetsubou-0.6.4/zetsubou/commands/base_command.py` & `zetsubou-0.7.0/zetsubou/commands/base_command.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,19 +2,18 @@
 from typing import List, Optional
 import os
 
 import bentoudev.dataclass.base as base
 
 from zetsubou.commands.execute_stage import execute_stage
 from zetsubou.commands.command_context import CommandContext
-from zetsubou.conan.from_conan import build_type_from_conan
 from zetsubou.project.model.config_string import EDefaultConfigSlots
-from zetsubou.project.runtime.filter_toolchains import get_toolchains_per_platform
-from zetsubou.project.runtime.project_loader import ProjectTemplate, ValidationContext, load_project_from_file, validate_platforms, ExternalConfig
+from zetsubou.project.runtime.project_loader import ProjectTemplate, load_project_from_file, ExternalConfig
 from zetsubou.project.config_matrix import ConfigMatrix, ConfigVariant, create_config_matrix
+from zetsubou.project.runtime.validation import ValidationContext, validate_profile
 from zetsubou.system import discover_toolchains, tools
 from zetsubou.utils import logger
 from zetsubou.utils.common import fix_path
 from zetsubou.utils.error_codes import EErrorCode
 
 
 class Command:
@@ -85,23 +84,19 @@
         if context.project_template is None:
 
             logger.Command('load_project')
 
             external_config = ExternalConfig()
 
             # handle platform from external file
-            if hasattr(context.command_args, 'platform') and context.command_args.platform is not None:
-                platform_file = os.path.relpath(context.command_args.platform, context.fs_root) if os.path.isabs(context.command_args.platform) else context.command_args.platform
-                external_config.platform_file = fix_path(platform_file)
-
-                logger.Info(f"Using platform from external file '{external_config.platform_file}'")
-
-            # handle forced build type
-            if hasattr(context.command_args, 'base_config') and context.command_args.base_config is not None:
-                external_config.base_config = build_type_from_conan(context.command_args.base_config)
+            if hasattr(context.command_args, 'profile') and context.command_args.profile is not None:
+                profile_file = os.path.relpath(context.command_args.profile, context.fs_root) if os.path.isabs(context.command_args.profile) else context.command_args.profile
+                external_config.profile_file = fix_path(profile_file)
+
+                logger.Info(f"Using profile from external file '{external_config.profile_file}'")
 
             # load and process project
             context.project_template = execute_stage(lambda: load_project_from_file(
                                         context.project_fs,
                                         context.fs_root,
                                         context.project_file,
                                         external_config=external_config),
@@ -112,43 +107,39 @@
                 context.host_system,
                 context.host_arch,
                 context.project_template.platforms)
 
             # validate platforms
             vctx = ValidationContext()
             vctx.error_format = base.EErrorFormat.MSVC if context.command_args.ide else base.EErrorFormat.Pretty
-            validate_platforms(vctx, context.project_template.platforms)
-
-            # discover toolchains
-            context.toolchains = execute_stage(lambda: discover_toolchains.discover_toolchain_list(context),
-                                   'Toolchains discovered',
-                                    EErrorCode.UNABLE_TO_DISCOVER_TOOLCHAIN)
+            validate_profile(vctx, context.project_template.profile)
 
-            context.project_template.toolchains = context.toolchains
+            # discovering and filtering of toolchains
+            context.project_template.platform_toolchains, context.project_template.system_toolchains = execute_stage(
+                lambda: discover_toolchains.discover_toolchain_list(context),
+                'Toolchains discovered',
+                EErrorCode.UNABLE_TO_DISCOVER_TOOLCHAIN)
 
             # create matrix of all options and their possible values
             context.config_matrix = execute_stage(lambda: resolve_config_matrix(context.project_template),
                                       'Config matrix created',
                                       EErrorCode.UNABLE_TO_CREATE_CONFIGURATIONS)
 
 
 def resolve_config_matrix(project_template:ProjectTemplate) -> Optional[ConfigMatrix]:
     # Full config matrix, contains incorrect entries (toolchain/platform mismatched)
     config_matrix = create_config_matrix(project_template.project.config.config_string,
         project_template.slot_values())
 
-    tools_per_plat = get_toolchains_per_platform(project_template)
-
     def filter_tool_by_plat(variant: ConfigVariant):
-        platform = project_template.find_platform(variant.get_slot(EDefaultConfigSlots.platform.name))
-        toolchain = project_template.find_toolchain(variant.get_slot(EDefaultConfigSlots.toolchain.name))
+        toolchain = project_template.find_toolchain(
+            variant.get_slot(EDefaultConfigSlots.platform.name),
+            variant.get_slot(EDefaultConfigSlots.toolchain.name))
 
-        if toolchain.name not in tools_per_plat[platform.platform]:
-            return False
-
-        return True
+        return toolchain is not None
 
+    # Filter out incorrect variants
     config_matrix.variants = list(filter(filter_tool_by_plat, config_matrix.variants))
     if len(config_matrix.variants) == 0:
         return None
 
     return config_matrix
```

### Comparing `zetsubou-0.6.4/zetsubou/commands/build.py` & `zetsubou-0.7.0/zetsubou/commands/build.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,32 +72,33 @@
             target_variants = []
 
             if not null_or_empty(arg_variant):
                 target_and_kind, config = ProjectTemplate.decompose_variant_name(arg_variant, context.project_template.project.config.config_string)
                 if target_and_kind is None or config is None:
                     raise ProjectError(f"Unable to parse target variant string '{arg_variant}'")
 
+                # TODO make this more robust
                 target_parts = target_and_kind.split('_')
-                if len(target_parts) > 1:
-                    kind = target_parts[1]
-                    if kind not in ETargetKind.__members__:
+                if len(target_parts) > 2:
+                    kind = f"{target_parts[1]}_{target_parts[2]}"
+                    if not any(filter(lambda e : kind.startswith(e[0]), ETargetKind.__members__)):
                         raise ProjectError(f"Unknown target kind '{kind}'")
 
                 target = target_parts[0]
 
                 if not context.project_template.find_target(target) and target != EDefaultTargets.All.name:
                     raise ProjectError(f"Unknown target '{target}'")
 
                 if not context.project_template.find_config(config[EDefaultConfigSlots.configuration.name]):
                     raise ProjectError(f"Unknown configuration '{config[EDefaultConfigSlots.configuration.name]}'")
 
                 if not context.project_template.find_platform(config[EDefaultConfigSlots.platform.name]):
                     raise ProjectError(f"Unknown platform '{config[EDefaultConfigSlots.platform.name]}'")
 
-                if not context.project_template.find_toolchain(config[EDefaultConfigSlots.toolchain.name]):
+                if not context.project_template.find_toolchain(config[EDefaultConfigSlots.platform.name], config[EDefaultConfigSlots.toolchain.name]):
                     raise ProjectError(f"Unknown toolchain '{config[EDefaultConfigSlots.toolchain.name]}'")
 
                 target_variants = [ arg_variant ]
 
             else:
                 # We have four options
                 # - target with config
```

### Comparing `zetsubou-0.6.4/zetsubou/commands/clean.py` & `zetsubou-0.7.0/zetsubou/commands/clean.py`

 * *Files identical despite different names*

### Comparing `zetsubou-0.6.4/zetsubou/commands/clean_build.py` & `zetsubou-0.7.0/zetsubou/commands/clean_build.py`

 * *Files identical despite different names*

### Comparing `zetsubou-0.6.4/zetsubou/commands/command_context.py` & `zetsubou-0.7.0/zetsubou/project/runtime/emit.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,52 +1,64 @@
-import os
+from typing import List, ClassVar
 from dataclasses import dataclass, field
-from typing import List, Optional, Any
+from enum import Enum
+
 from fs.base import FS
+from fs.path import combine as fs_combine
+from fs.path import dirname as fs_dirname
+from fs.path import basename as fs_basename
 
-from zetsubou.commands.execute_stage import execute_stage
-from zetsubou.utils import logger
-from zetsubou.utils.common import null_or_empty, fix_path
-from zetsubou.project.config_matrix import ConfigMatrix
 from zetsubou.project.base_context import BaseContext
-from zetsubou.project.model.target import Target
-from zetsubou.project.model.toolchain import Toolchain
+from zetsubou.project.runtime.project_loader import ProjectTemplate
 from zetsubou.project.runtime.resolve import ResolvedTarget
-from zetsubou.project.runtime.project_loader import ProjectTemplate, resolve_venv
-from zetsubou.utils.error_codes import EErrorCode
+from zetsubou.project.config_matrix import ConfigMatrix
+from zetsubou.commands.command_context import Conan
 
-@dataclass
-class Fastbuild:
-    emit_fs : FS
-    bff_dir : str
-    bff_file : str
+
+class EDefaultTargets(Enum):
+    All = 0x1
+    Update = 0x2
 
 
 @dataclass
-class Conan:
-    yml_files: List[str] = field(default_factory=list)
-    dependencies: List[Target] = field(default_factory=list)
+class EmitContext(BaseContext):
+    project_template: ProjectTemplate = None
     resolved_targets: List[ResolvedTarget] = field(default_factory=list)
+    config_matrix: ConfigMatrix = None
+    conan: Conan = None
+    mem_fs: FS = None
+    ROOT_DIR: ClassVar[str] = "."
 
+    @classmethod
+    def from_base(cls, source : BaseContext):
+        result = EmitContext()
+        result.__dict__.update(source.__dict__)
+        return result
 
-@dataclass
-class CommandContext(BaseContext):
-    command_args: Any = None
+    def write_file(self, rw_path: str, content: str):
+        dirname = fs_dirname(rw_path)
+        filename = fs_basename(rw_path)
+
+        dirname = fs_combine(EmitContext.ROOT_DIR, dirname)
+
+        with self.mem_fs.makedirs(dirname, recreate=True) as out_dir:
+            with out_dir.open(filename, 'w') as out_file:
+                out_file.write(content)
+
+
+class Emitter:
+    def emit_solution(self, context: EmitContext) -> str:
+        raise NotImplementedError()
+
+    def emit_target(self, context: EmitContext, target: ResolvedTarget):
+        raise NotImplementedError()
 
-    project_template: Optional[ProjectTemplate] = None
-    toolchains: List[Toolchain] = field(default_factory=list)
-    config_matrix: Optional[ConfigMatrix] = None
-    resolved_targets: List[ResolvedTarget] = field(default_factory=list)
-    fastbuild: Optional[Fastbuild] = None
-    conan: Conan = field(default_factory=Conan)
 
-    def to_out_path(self, path : str):
-        return fix_path(os.path.join(self.fs_root, path))
+def emit_project(context: EmitContext, emitter: Emitter):
+    # emit target files
+    for target in context.resolved_targets:
+        emitter.emit_target(context, target)
 
-    def resolve_venv(self):
-        if null_or_empty(self.fs_venv):
-            venv_path = execute_stage(lambda: resolve_venv(self.project_fs, self.project_template.project, self.fs_root),
-                                        'Virtual environemnt found',
-                                        EErrorCode.UNABLE_TO_FIND_VENV)
+    # emit main project file
+    main_file = emitter.emit_solution(context)
 
-            logger.Info(f"Virtual environement - '{venv_path}'")
-            self.fs_venv = fix_path(venv_path)
+    return (context.mem_fs, EmitContext.ROOT_DIR, main_file)
```

### Comparing `zetsubou-0.6.4/zetsubou/commands/command_registry.py` & `zetsubou-0.7.0/zetsubou/commands/command_registry.py`

 * *Files identical despite different names*

### Comparing `zetsubou-0.6.4/zetsubou/commands/config.py` & `zetsubou-0.7.0/zetsubou/commands/config.py`

 * *Files identical despite different names*

### Comparing `zetsubou-0.6.4/zetsubou/commands/create.py` & `zetsubou-0.7.0/zetsubou/commands/create.py`

 * *Files identical despite different names*

### Comparing `zetsubou-0.6.4/zetsubou/commands/execute_stage.py` & `zetsubou-0.7.0/zetsubou/commands/execute_stage.py`

 * *Files identical despite different names*

### Comparing `zetsubou-0.6.4/zetsubou/commands/generate.py` & `zetsubou-0.7.0/zetsubou/commands/generate.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,80 +1,83 @@
 from argparse import ArgumentParser
 import os
 from fs.base import FS
 from fs.copy import copy_fs
 from zetsubou.commands.base_command import Command
 from zetsubou.commands.command_context import CommandContext, Fastbuild
 from zetsubou.commands.execute_stage import execute_stage
+from zetsubou.commands.install import Install
 from zetsubou.conan.dependencies import ConanDependencies
 from zetsubou.fastbuild.fastbuild_emit import FastbuildEmitter
 from zetsubou.project.model.target import Target
+from zetsubou.project.model.virtual_environment import VirtualEnvironment
 from zetsubou.project.runtime.emit import EmitContext, emit_project
-from zetsubou.project.runtime.project_loader import ValidationContext, load_dataclass_list, validate_targets
-from zetsubou.project.runtime.resolve import ResolveContext, process_target_variants_list
+from zetsubou.project.runtime.project_loader import load_dataclass_list
+from zetsubou.project.runtime.resolve import ResolveContext, resolve_target_variants
+from zetsubou.project.runtime.validation import ValidationContext, validate_targets, validate_cli_tools
 
 from zetsubou.utils import logger
 from zetsubou.utils.error_codes import EErrorCode
 from zetsubou.utils.subprocess import call_process_venv
 from zetsubou.utils.yaml_loader import YamlDataclassLoader as YAMLLoader
 import bentoudev.dataclass.base as base
 
 from fs import open_fs as fs_create
 
 def commit_to_filesystem(project_fs : FS, mem_fs : FS, fs_root : str):
     copy_fs(mem_fs, project_fs)
     return True
 
 
-def check_fastbuild_present(venv : str):
+def check_fastbuild_present(venv : VirtualEnvironment):
     out, err = call_process_venv(['fbuild', '-version'], venv, capture=True, realtime=False)
     if err is not None:
         logger.CriticalError('FASTbuild is missing, unable to proceed')
         return False
 
     logger.Success("FASTbuild present")
     logger.Verbose(out)
     return True
 
 
-def call_fbuild_projects(fs_root : dir, bff_dir : str, bff_file : str, venv : str):
+def call_fbuild_projects(fs_root : dir, bff_dir : str, bff_file : str, venv_obj : VirtualEnvironment):
     bff_dir = os.path.join(fs_root, bff_dir)
     bff_file = os.path.join(fs_root, bff_dir, bff_file)
 
     verbose = logger.IsVisible(logger.ELogLevel.Verbose)
 
     assert os.path.isfile(bff_file)
     assert not os.path.isfile(bff_dir)
 
-    out, err = call_process_venv(['fbuild', '-config', bff_file], venv, capture = not verbose, realtime = verbose, cwd = bff_dir)
+    out, err = call_process_venv(['fbuild', '-config', bff_file], venv_obj, capture = not verbose, realtime = verbose, cwd = bff_dir)
     if err is not None:
 
         if not verbose:
             logger.Error(out)
 
         logger.CriticalError(f"FASTbuild returned error '{err}'")
         return False
 
     if verbose:
         print('')
     return True
 
 
-def call_fbuild_solution(fs_root : dir, bff_dir : str, bff_file : str, project_name : str, venv : str):
+def call_fbuild_solution(fs_root : dir, bff_dir : str, bff_file : str, project_name : str, venv_obj : VirtualEnvironment):
     bff_dir = os.path.join(fs_root, bff_dir)
     bff_file = os.path.join(fs_root, bff_dir, bff_file)
 
     verbose = logger.IsVisible(logger.ELogLevel.Verbose)
     if verbose:
         print('')
 
     assert os.path.isfile(bff_file)
     assert not os.path.isfile(bff_dir)
 
-    out, err = call_process_venv(['fbuild', '-config', bff_file, project_name, '-ide'], venv, capture=not verbose, realtime=verbose, cwd=bff_dir)
+    out, err = call_process_venv(['fbuild', '-config', bff_file, project_name, '-ide'], venv_obj, capture=not verbose, realtime=verbose, cwd=bff_dir)
     if err is not None:
 
         if not verbose:
             logger.Error(out)
 
         logger.CriticalError(f"FASTbuild returned error '{err}'")
         return False
@@ -85,43 +88,57 @@
 
 
 def load_dependencies(context: CommandContext):
     loader = YAMLLoader()
     local_types = base.get_types_from_modules([__name__, 'zetsubou.project.model.target'])
     dep_targets = []
 
-    if len(context.conan.yml_files) == 0:
+    conan_deps = context.project_template.project.conan.dependencies
+    if conan_deps is None:
+        return
+
+    conan_deps = context.to_out_path(conan_deps)
+
+    def load_deps():
         path = 'build/conan_deps.yml'
 
-        if context.project_fs.exists(path):
+        # Merge files, only parts from deployer exist
+        if not context.project_fs.exists(path):
+            Command.get_command_instance(Install).merge_generated_part_files(context, conan_deps)
+            return True
 
-            with context.project_fs.open(path, 'r', encoding='utf-8') as obj_file:
-                obj_templ : ConanDependencies = loader.load_dataclass(ConanDependencies, path, obj_file.read(), local_types)
+        # Load merged yaml
+        with context.project_fs.open(path, 'r', encoding='utf-8') as obj_file:
+            obj_templ : ConanDependencies = loader.load_dataclass(ConanDependencies, path, obj_file.read(), local_types)
 
-                if obj_templ is None:
-                    return False
+            if obj_templ is None:
+                return False
 
-                dep_targets = obj_templ.targets
-    else:
-        dep_targets = context.conan.yml_files
+            context.conan.yml_files = obj_templ.targets
+
+        return True
+
+    if len(context.conan.yml_files) == 0:
+        if not load_deps():
+            return False
+
+    dep_targets = context.conan.yml_files
 
     if len(dep_targets) != 0:
         context.conan.dependencies = load_dataclass_list(Target, dep_targets, '', context.project_fs, loader, local_types)
 
     return True
 
 
 def validate_project(context: CommandContext):
     vctx = ValidationContext()
     vctx.error_format = base.EErrorFormat.MSVC if context.command_args.ide else base.EErrorFormat.Pretty
 
-    if len(context.conan.dependencies) > 0:
-        validate_targets(vctx, context.conan.dependencies)
-
     validate_targets(vctx, context.project_template.targets + context.conan.dependencies)
+    validate_cli_tools(vctx, context.project_template.targets, context.project_template.cli_tools)
 
     return True
 
 
 class Generate(Command):
     @property
     def name(self):
@@ -153,20 +170,20 @@
                     EErrorCode.UNABLE_TO_VALIDATE_TARGETS)
 
         resolve_context = ResolveContext.from_base(context)
         resolve_context.project=context.project_template
 
         if len(context.conan.dependencies) > 0:
             # create variants of conan deps per configuration
-            context.conan.resolved_targets = execute_stage(lambda: process_target_variants_list(resolve_context, context.config_matrix, context.conan.dependencies),
+            context.conan.resolved_targets = execute_stage(lambda: resolve_target_variants(resolve_context, context.config_matrix, context.conan.dependencies),
                                         'Resolved Conan target variants',
                                         EErrorCode.UNABLE_TO_RESOLVE_VARIANTS)
 
         # create variants of targets per configuration
-        context.resolved_targets = execute_stage(lambda: process_target_variants_list(resolve_context, context.config_matrix, context.project_template.targets),
+        context.resolved_targets = execute_stage(lambda: resolve_target_variants(resolve_context, context.config_matrix, context.project_template.targets),
                                     'Resolved target variants dependencies',
                                     EErrorCode.UNABLE_TO_RESOLVE_VARIANTS)
 
         emit_context = EmitContext.from_base(context)
         emit_context.project_template=context.project_template
         emit_context.resolved_targets=context.resolved_targets
         emit_context.config_matrix=context.config_matrix
@@ -185,19 +202,17 @@
 
         # commit virtual filesystem to os
         if not context.command_args.dry:
             execute_stage(lambda: commit_to_filesystem(context.project_fs, context.fastbuild.emit_fs, context.fastbuild.bff_dir),
                 'Files commited to filesystem',
                 EErrorCode.UNABLE_TO_COMMIT_FS)
 
-            venv_path = os.path.join(context.fs_root, context.fs_venv)
-            if check_fastbuild_present(venv_path):
-
+            if check_fastbuild_present(context.fs_venv):
                 execute_stage(lambda: call_fbuild_projects(context.fs_root, context.fastbuild.bff_dir, context.fastbuild.bff_file,
-                    venv_path),
+                    context.fs_venv),
                     'FASTbuild projects generated',
                     EErrorCode.UNABLE_TO_CREATE_VS_PROJECTS)
 
                 execute_stage(lambda: call_fbuild_solution(context.fs_root, context.fastbuild.bff_dir, context.fastbuild.bff_file,
-                    context.project_template.project.project, venv_path),
+                    context.project_template.project.project, context.fs_venv),
                     'FASTbuild solution generated',
                     EErrorCode.UNABLE_TO_CREATE_VS_SOLUTION)
```

### Comparing `zetsubou-0.6.4/zetsubou/commands/install.py` & `zetsubou-0.7.0/zetsubou/commands/install.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 from argparse import ArgumentParser
 import os
-import venv
 from zetsubou.commands.base_command import Command
 from zetsubou.commands.command_context import CommandContext
 from zetsubou.commands.execute_stage import execute_stage
 from zetsubou.conan.dependencies import ConanDependencies
+from zetsubou.project.model.toolchain_profile import Windows_ToolchainProfile
+from zetsubou.project.model.virtual_environment import generate_empty_environment
 from zetsubou.utils import logger
 from zetsubou.utils.error_codes import EErrorCode
 from zetsubou.utils.yaml_tools import to_yaml
 from zetsubou.conan.conan import check_conan_present, call_conan
-from zetsubou.conan.to_conan import toolchain_to_conan, platform_to_conan, config_base_to_conan
+from zetsubou.conan.to_conan import runtime_to_conan, toolchain_to_conan, platform_to_conan, config_base_to_conan
+from zetsubou.conan.deployer import get_conan_deployer_path
+
+
+CONAN_OUT_PATH = 'build/conan'
 
 
 class Install(Command):
     @property
     def name(self):
         return 'install'
 
@@ -30,66 +35,25 @@
 
     def OnExecute(self, context: CommandContext):
         context.project_fs.makedirs('build/venv', recreate=True)
 
         if context.project_template.project.conan is not None and check_conan_present():
             self.generate_conan_environment(context)
         else:
-            self.generate_empty_environment(context)
-
-    def generate_empty_environment(self, context: CommandContext):
-        env_builder = venv.EnvBuilder()
-        venv_fs = context.project_fs.geturl('build/venv', purpose='fs')
-        venv_fs = venv_fs.split('osfs://')[1]
-        env_builder.create(venv_fs)
-        logger.Info('Created new virtual environment')
-
-    def generate_conan_environment(self, context: CommandContext):
-        CONAN_OUT_PATH = 'build/conan'
-        conan_build_tools = context.project_template.project.conan.build_tools
-        if conan_build_tools is not None:
-            conan_build_tools = context.to_out_path(conan_build_tools)
-            execute_stage(lambda: call_conan(['install', conan_build_tools, '-g=virtualenv'], context.to_out_path('build/venv')),
-                        'Conan build tools installed',
-                        EErrorCode.UNABLE_TO_INSTALL_CONAN_BUILD_TOOLS)
-
-            context.resolve_venv()
-
-        conan_deps = context.project_template.project.conan.dependencies
-        if conan_deps is None:
-            return
-
-        conan_deps = context.to_out_path(conan_deps)
-
-        for config_variant in context.config_matrix.variants:
-            logger.Verbose(f"Installing configuration '{config_variant.config_string}'")
-
-            platform = context.project_template.find_platform(config_variant.get_slot('platform'))
-            toolchain = context.project_template.find_toolchain(config_variant.get_slot('toolchain'))
-            config = context.project_template.find_config(config_variant.get_slot('configuration'))
-
-            conan_settings = []
-            conan_settings.extend(platform_to_conan(context, platform))
-            conan_settings.extend(toolchain_to_conan(context, toolchain))
-            conan_settings.extend(config_base_to_conan(context, config, toolchain))
-
-            conan_config_out_path = f'{CONAN_OUT_PATH}/{config_variant.config_string.replace("-", ".")}'
-            context.project_fs.makedirs(conan_config_out_path, recreate=True)
-
-            execute_stage(lambda: call_conan(
-                        ['install', conan_deps, f'--build={context.project_template.project.conan.build}'] + conan_settings,
-                        context.to_out_path(conan_config_out_path),
-                        context.to_out_path(context.fs_venv)),
-                        f"Conan configuration '{config_variant.config_string}' installed",
-                        EErrorCode.UNABLE_TO_INSTALL_CONAN_DEPENDENCIES)
+            generate_empty_environment(context.project_fs)
 
+    def merge_generated_part_files(self, context:CommandContext, conan_deps:str):
         dep_matrix = {}
         for path in context.project_fs.walk.files(path=CONAN_OUT_PATH, filter=['*.part.yml']):
             dep_name = os.path.basename(path).rsplit('.')[0]
+
             config_string = (os.path.basename(os.path.dirname(path))).replace('.', '-')
+            if not context.config_matrix.has_variant(config_string):
+                logger.Verbose(f"Conan dependency '{dep_name}' uses '*' fallback for all variants")
+                config_string = '*'
 
             if dep_name not in dep_matrix:
                 dep_matrix[dep_name] = [
                     f'target: {dep_name}\n'
                     'config:\n'
                     '  kind: IMPORTED_TARGET\n'
                     'filters:\n'
@@ -116,7 +80,58 @@
         if len(out_ymls) > 0:
 
             with context.project_fs.open('build/conan_deps.yml', mode='w') as out_file:
                 conan_deps = ConanDependencies(conanfile=conan_deps, targets=out_ymls)
                 out_file.write(to_yaml(conan_deps))
 
             context.conan.yml_files = out_ymls
+
+    def generate_conan_environment(self, context: CommandContext):
+        conan_build_tools = context.project_template.project.conan.build_tools
+        if conan_build_tools is not None:
+            conan_build_tools = context.to_out_path(conan_build_tools)
+            conan_out_directory = context.to_out_path("build/venv")
+            execute_stage(lambda: call_conan(['install', conan_build_tools, '-g=VirtualBuildEnv', f'-of={conan_out_directory}'], conan_out_directory),
+                        'Conan build tools installed',
+                        EErrorCode.UNABLE_TO_INSTALL_CONAN_BUILD_TOOLS)
+
+            context.resolve_venv()
+
+        conan_deps = context.project_template.project.conan.dependencies
+        if conan_deps is None:
+            return
+
+        conan_deps = context.to_out_path(conan_deps)
+
+        for config_variant in context.config_matrix.variants:
+            logger.Verbose(f"Installing configuration '{config_variant.config_string}'")
+
+            plat_name = config_variant.get_slot('platform')
+            platform = context.project_template.find_platform(plat_name)
+            toolchain = context.project_template.find_toolchain(plat_name, config_variant.get_slot('toolchain'))
+            config = context.project_template.find_config(config_variant.get_slot('configuration'))
+
+            conan_settings = []
+            conan_settings.extend(platform_to_conan(context, platform))
+            conan_settings.extend(toolchain_to_conan(context, toolchain))
+            conan_settings.extend(config_base_to_conan(context, config))
+
+            if isinstance(toolchain.profile, Windows_ToolchainProfile):
+                conan_settings.extend(runtime_to_conan(config, toolchain))
+
+            conan_config_out_path = f'{CONAN_OUT_PATH}/{config_variant.config_string.replace("-", ".")}'
+            context.project_fs.makedirs(conan_config_out_path, recreate=True)
+
+            conan_call_args = [
+                'install', conan_deps, f'--build={context.project_template.project.conan.build}',
+                '--deploy', get_conan_deployer_path(),
+                f'-of={conan_config_out_path}'
+            ]
+
+            # pylint: disable=cell-var-from-loop
+            execute_stage(lambda: call_conan(conan_call_args + conan_settings,
+                        context.to_out_path(conan_config_out_path),
+                        context.fs_venv),
+                        f"Conan configuration '{config_variant.config_string}' installed",
+                        EErrorCode.UNABLE_TO_INSTALL_CONAN_DEPENDENCIES)
+
+        self.merge_generated_part_files(context, conan_deps)
```

### Comparing `zetsubou-0.6.4/zetsubou/commands/regen.py` & `zetsubou-0.7.0/zetsubou/commands/regen.py`

 * *Files identical despite different names*

### Comparing `zetsubou-0.6.4/zetsubou/conan/to_conan.py` & `zetsubou-0.7.0/zetsubou/conan/to_conan.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,124 +1,140 @@
 from copy import copy
 from zetsubou.commands.base_command import CommandContext
-from typing import List
+from typing import Set, Tuple, List
 from zetsubou.project.model.configuration import Configuration
+from zetsubou.project.model.configuration_enums import EBaseConfiguration
 from zetsubou.project.model.platform_enums import EArch, ESystem
 from zetsubou.project.model.platform import Platform
 from zetsubou.project.model.runtime_library import ERuntimeLibrary
-
+from zetsubou.project.model.toolchain_profile import Windows_ToolchainProfile
 from zetsubou.project.model.toolchain import ECompilerFamily, ECppStandard, Toolchain
+from zetsubou.utils.common import Version
 
 
 def platform_to_conan(context: CommandContext, plat : Platform) -> List[str]:
     return [
         '-s', f'os={plat.host_system.name}'
     ]
 
 
+def msvc_version_to_conan(msvc_ver:Version) -> Tuple[str, str]:
+    version = str(msvc_ver.major)
+    version += str(msvc_ver.minor)[0]
+    return (version, str(msvc_ver.minor)[1:])
+
+
+def compiler_family_to_conan(family : ECompilerFamily):
+    return {
+        ECompilerFamily.MSVC.name  : 'msvc',
+        ECompilerFamily.CLANG.name : 'clang',
+        ECompilerFamily.GCC.name   : 'gcc'
+    }.get(family.name)
+
+
 def toolchain_to_conan(context: CommandContext, toolchain: Toolchain) -> List[str]:
     if toolchain is not None:
 
         arch = {
             EArch.x86.name : 'x86',
             EArch.x64.name : 'x86_64'
-        }.get(toolchain.arch)
+        }.get(toolchain.definition.arch)
 
-        compiler = {
-            ECompilerFamily.MSVC.name  : 'Visual Studio',
-            ECompilerFamily.CLANG.name : 'clang',
-            ECompilerFamily.GCC.name   : 'gcc'
-        }.get(toolchain.CompilerFamily.name)
+        compiler = compiler_family_to_conan(toolchain.definition.CompilerFamily)
 
         result = [
             '-s', f'arch={arch}',
             '-s', f'compiler={compiler}',
         ]
 
-        for path in toolchain.PathEnv:
-            result.extend([
-                '-e', f'PATH=[{path}]'
-            ])
+        # TODO FIXME Conan should know about these, but there is no way to pass them via CLI anymore in 2.0 :(
+        # for path in toolchain.definition.PathEnv:
+        #     result.extend([
+        #         '-e', f'PATH=[{path}]'
+        #     ])
 
-        if context.host_system == ESystem.Windows and toolchain.Toolset is not None:
-            if toolchain.CompilerFamily == ECompilerFamily.MSVC:
-                result.extend([
-                    '-s', f'compiler.toolset={toolchain.Toolset}'
-                ])
-            elif toolchain.CompilerFamily == ECompilerFamily.CLANG:
+        result.extend(cppstd_to_conan(toolchain.profile.cppstd))
+
+        if context.host_system == ESystem.Windows and toolchain.toolset is not None:
+            if toolchain.definition.CompilerFamily == ECompilerFamily.CLANG:
                 result.extend([
-                    '-s', f'compiler.runtime_version={toolchain.Toolset}'
+                    '-s', f'compiler.runtime_version={toolchain.toolset}'
                 ])
 
-        if toolchain.CompilerFamily == ECompilerFamily.MSVC:
+        if toolchain.definition.CompilerFamily == ECompilerFamily.MSVC:
+            version = msvc_version_to_conan(toolchain.definition.version)
             result.extend([
-                '-s', f'compiler.version={toolchain.ide_version.major}'
+                '-s', f'compiler.version={version[0]}',
+                '-s', f'compiler.update={version[1]}'
             ])
         else:
             # Remove path, conan is interested only in Major.Minor at best
-            ver_no_path = copy(toolchain.version)
+            ver_no_path = copy(toolchain.definition.version)
             ver_no_path.path = 0
 
             result.extend([
                 '-s', f'compiler.version={ver_no_path}'
             ])
 
         return result
 
     return []
 
 
-def config_base_to_conan(context: CommandContext, config: Configuration, toolchain:Toolchain) -> List[str]:
-    if config is not None and toolchain is not None:
+def config_base_to_conan(context: CommandContext, config: Configuration) -> List[str]:
+    if config is not None:
 
         build_type = {
-            'DEBUG' : 'Debug',
-            'RELEASE' : 'Release',
-            'RELEASE_WITH_DEBUG_INFO' : 'RelWithDebInfo'
-        }.get(config.base_configuration.name)
+            EBaseConfiguration.DEBUG : 'Debug',
+            EBaseConfiguration.RELEASE : 'Release',
+            EBaseConfiguration.RELEASE_WITH_DEBUG_INFO : 'RelWithDebInfo'
+        }.get(config.base_configuration)
 
         result = [
             '-s', f'build_type={build_type}',
         ]
 
-        if context.host_system == ESystem.Windows:
-
-            if toolchain.CompilerFamily == ECompilerFamily.MSVC:
-                runtime_library = {
-                    ERuntimeLibrary.DYNAMIC_DEBUG.name   : 'MDd',
-                    ERuntimeLibrary.DYNAMIC_RELEASE.name : 'MD',
-                    ERuntimeLibrary.STATIC_DEBUG.name    : 'MTd',
-                    ERuntimeLibrary.STATIC_RELEASE.name : 'MT',
-                }.get(config.runtime_library.name)
-
-                result.extend([
-                    '-s', f'compiler.runtime={runtime_library}'
-                ])
-            elif toolchain.CompilerFamily == ECompilerFamily.CLANG:
-                runtime, runtime_type = {
-                    ERuntimeLibrary.DYNAMIC_DEBUG.name   : ('dynamic', 'Debug'),
-                    ERuntimeLibrary.DYNAMIC_RELEASE.name : ('dynamic', 'Release'),
-                    ERuntimeLibrary.STATIC_DEBUG.name    : ('static',  'Debug'),
-                    ERuntimeLibrary.STATIC_RELEASE.name  : ('static',  'Release'),
-                }.get(config.runtime_library.name)
-
-                result.extend([
-                    '-s', f'compiler.runtime={runtime}',
-                    '-s', f'compiler.runtime_type={runtime_type}',
-                ])
-
         return result
 
     return []
 
+
 def cppstd_to_conan(cppstd:ECppStandard):
     cpp = {
         ECppStandard.cpp11  : '11',
         ECppStandard.cpp14  : '14',
         ECppStandard.cpp17  : '17',
         ECppStandard.cpp20  : '20',
         ECppStandard.cpp23  : '23',
         ECppStandard.latest : '23',
     }.get(cppstd)
     return [
         '-s', f"compiler.cppstd={cpp}"
     ]
+
+
+def runtime_to_conan(config:Configuration, toolchain:Toolchain):
+    if not isinstance(toolchain.profile, Windows_ToolchainProfile):
+        return []
+
+    runtime = {
+        ERuntimeLibrary.dynamic : 'dynamic',
+        ERuntimeLibrary.static : 'static'
+    }.get(toolchain.profile.runtime)
+
+    runtime_type = 'Debug' if config.base_configuration == EBaseConfiguration.DEBUG else 'Release'
+
+    return [
+        '-s', f'compiler.runtime={runtime}',
+        '-s', f'compiler.runtime_type={runtime_type}'
+    ]
+
+
+def toolsets_from_settings(conan_settings : dict, compiler_family : ECompilerFamily) -> Set[str]:
+    conan_compiler = compiler_family_to_conan(compiler_family)
+    if compiler_family == ECompilerFamily.CLANG:
+        try:
+            return set(conan_settings['compiler'][conan_compiler]['runtime_version']) if conan_settings is not None else None
+        except KeyError:
+            return None
+    else:
+        return None
```

### Comparing `zetsubou-0.6.4/zetsubou/data/rules/ClangRules.yml` & `zetsubou-0.7.0/zetsubou/data/rules/ClangRules.yml`

 * *Files 21% similar despite different names*

```diff
@@ -20,14 +20,16 @@
         - -fms-compatibility
         - -fms-extensions
         - -fdelayed-template-parsing
         # Ignore warnings
         - -Wno-ignored-attributes
         - -Wno-dollar-in-identifier-extension
         - -Wno-unknown-pragmas
+        - -Wno-system-headers
+        - -Wno-gnu-line-marker
         # Disables exceptions
         - -fno-exceptions
         #- -Xlinker /NODEFAULTLIB
         # Disable rtti
         # - -fno-rtti
     defines:
       public:
@@ -62,57 +64,85 @@
       config_string: "*clang*x64*"
     compiler_flags:
       public:
         - -m64
 
   - filter:
       config_string: "*clang*"
-      runtime_library: STATIC_RELEASE
+      runtime_library: static
+      base_configuration:
+      - RELEASE
+      - RELEASE_WITH_DEBUG_INFO
     defines:
       public:
       - _MT
+    compiler_flags:
+      public:
+      - -Xclang -flto-visibility-public-std
+      - -Xclang --dependent-lib=libcmt
     linker_flags:
-      public: 
+      public:
       - libucrt.lib
       - libvcruntime.lib
       - libcmt.lib
       - libcpmt.lib
 
   - filter:
       config_string: "*clang*"
-      runtime_library: STATIC_DEBUG
+      runtime_library: static
+      base_configuration: DEBUG
     defines:
       public:
+      - _DEBUG
       - _MTd
+      - _MT
+    compiler_flags:
+      public:
+      - -flto-visibility-public-std
+      - -Xclang --dependent-lib=libcmtd
     linker_flags:
       public:
       - libucrtd.lib
       - libvcruntimed.lib
       - libcmtd.lib
       - libcpmtd.lib
 
   - filter:
       config_string: "*clang*"
-      runtime_library: DYNAMIC_RELEASE
+      runtime_library: dynamic
+      base_configuration:
+      - RELEASE
+      - RELEASE_WITH_DEBUG_INFO
     defines:
       public:
       - _MD
+      - _DLL
+    compiler_flags:
+      public:
+      - -Xclang --dependent-lib=msvcrt
     linker_flags:
       public:
       - ucrt.lib
       - vcruntime.lib
       - msvcrt.lib
       - msvcprt.lib
 
   - filter:
       config_string: "*clang*"
-      runtime_library: DYNAMIC_DEBUG
+      runtime_library: dynamic
+      base_configuration: DEBUG
     defines:
       public:
+      - _DEBUG
       - _MDd
+      - _MD
+      - _DLL
+    compiler_flags:
+      public:
+      - -Xclang --dependent-lib=msvcrtd
     linker_flags:
       public:
       - ucrtd.lib
       - vcruntimed.lib
       - msvcrtd.lib
       - msvcprtd.lib
```

### Comparing `zetsubou-0.6.4/zetsubou/data/rules/MsvcRules.yml` & `zetsubou-0.7.0/zetsubou/data/rules/MsvcRules.yml`

 * *Files 10% similar despite different names*

```diff
@@ -8,14 +8,16 @@
         - /Z7
         - /nologo
         - /W4
         - /Wall
         - /WX
         # Padding added after data member
         - /wd4820
+        # Bug in msvc std, fallthrough warnings for <atomic>
+        - /wd5262
         - /TP
         - /EHsc
         - /Zc:inline
         - /Zc:strictStrings
         - /fp:fast
         # Generate intrinsics functions
         - /Oi
@@ -63,51 +65,59 @@
       kind: DYNAMIC_LIBRARY
     linker_flags:
       private:
         - /DLL
 
   - filter:
       config_string: "*msvc*"
-      runtime_library: STATIC_RELEASE
+      runtime_library: static
+      base_configuration:
+      - RELEASE
+      - RELEASE_WITH_DEBUG_INFO
     compiler_flags:
       public: /MT
     linker_flags:
       public: 
       - libucrt.lib
       - libvcruntime.lib
       - libcmt.lib
       - libcpmt.lib
 
   - filter:
       config_string: "*msvc*"
-      runtime_library: STATIC_DEBUG
+      runtime_library: static
+      base_configuration: DEBUG
     compiler_flags:
       public: /MTd
     linker_flags:
       public:
       - libucrtd.lib
       - libvcruntimed.lib
       - libcmtd.lib
       - libcpmtd.lib
 
   - filter:
       config_string: "*msvc*"
-      runtime_library: DYNAMIC_RELEASE
+      runtime_library: dynamic
+      base_configuration:
+      - RELEASE
+      - RELEASE_WITH_DEBUG_INFO
     compiler_flags:
       public: /MD
     linker_flags:
       public:
       - ucrt.lib
       - vcruntime.lib
       - msvcrt.lib
       - msvcprt.lib
 
   - filter:
       config_string: "*msvc*"
-      runtime_library: DYNAMIC_DEBUG
+      runtime_library: dynamic
+      base_configuration: DEBUG
     compiler_flags:
       public: /MDd
     linker_flags:
       public:
       - ucrtd.lib
       - vcruntimed.lib
       - msvcrtd.lib
```

### Comparing `zetsubou-0.6.4/zetsubou/fastbuild/compiler.py` & `zetsubou-0.7.0/zetsubou/fastbuild/compiler.py`

 * *Files identical despite different names*

### Comparing `zetsubou-0.6.4/zetsubou/fastbuild/fastbuild_emit.py` & `zetsubou-0.7.0/zetsubou/fastbuild/fastbuild_emit.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,41 +1,44 @@
 import os
 import fs
+from pathlib import Path
 
 from dataclasses import dataclass, is_dataclass, fields
 from enum import Enum
 from inspect import isclass
 from typing import Optional, List, Any, Set, Callable, Tuple, Generic, TypeVar
 from typing_inspect import get_origin, is_optional_type
 from zetsubou.fastbuild.to_fastbuild import compiler_family_to_fastbuild
 
-from zetsubou.project.config_matrix import get_config_matrix_os_name
+from zetsubou.project.config_matrix import ConfigVariant, get_config_matrix_os_name
 from zetsubou.project.model.config_string import EDefaultConfigSlots
 from zetsubou.project.model.configuration import Configuration
 from zetsubou.project.runtime.emit import EDefaultTargets, Emitter, EmitContext
 from zetsubou.project.runtime.project_loader import ProjectTemplate
 from zetsubou.project.runtime.resolve import ResolvedTarget, TargetVariant
-from zetsubou.project.model.target import Target, TargetReference
-from zetsubou.project.model.kind import ETargetKind, is_target_kind_linkable, is_target_library
-from zetsubou.project.model.toolchain import ECompilerFamily, Toolchain
-from zetsubou.utils.common import join_unique, list_to_string, split
+from zetsubou.project.model.target import Target, TargetReference, Source
+from zetsubou.project.model.kind import ETargetKind, is_target_kind_linkable, is_target_library, is_target_prebuild_step
+from zetsubou.project.model.toolchain import Toolchain, ToolchainDefinition
+from zetsubou.utils.common import join_unique, list_to_string, split, filter_none
 
 import zetsubou.fastbuild.target_kinds as target_kinds
 import zetsubou.fastbuild.vcxproject as vcxproject
 import zetsubou.fastbuild.vssolution as vssolution
 from zetsubou.fastbuild.compiler import Compiler
 from zetsubou.system.windows.msvc import arch_to_msvc_platform
+from zetsubou.utils.subprocess import call_process_venv
 
 
 FASTBUILD_BFF_HEADER = '// Generated by Zetsubou, do not manually edit!'
 FASTBUILD_ALL_TARGET = 'AllTargets'
 PROJ_OUTPUT_DIR = '^$(SolutionDir)/build'
 FBUILD_OUTPUT_DIR = 'build/fbuild'
 DEFAULT_INDENT = 4
-T = TypeVar('T')
+T1 = TypeVar('T1')
+T2 = TypeVar('T2')
 
 
 class bff_writer:
     indent : List[int]
     str_buff : List[str]
 
     def __init__(self):
@@ -129,17 +132,18 @@
         elif is_dataclass(obj):
             return { f.name : getattr(obj, f.name) for f in fields(obj) }.items()
         else:
             return vars(obj).items()
 
 
 @dataclass
-class bff_using(Generic[T]):
+class bff_using(Generic[T1, T2]):
     name : str
-    obj : T
+    obj : T1
+    ref : T2
 
 
 @dataclass
 class bff_includes:
     includes: List[str]
     system_includes: List[str]
 
@@ -184,15 +188,15 @@
         write_assign(self.writer, name)
         self.writer.write(value)
 
     def write_usings(self, usings : List[Any]):
         for using in usings:
             # Register names for Using objects, so we append their fields instead of overwritting
             if isinstance(using, bff_using):
-                for name, _ in bff_writer.get_fields(using.obj):
+                for name, _ in bff_writer.get_fields(using.ref):
                     self.field_map.add(name)
                 write_using(self.writer, using.name)
             else:
                 write_using(self.writer, using)
 
     def write_object(self, obj : Any, hidden_fields : List[str] = []):
         for name, value in self.writer.get_fields(obj):
@@ -383,29 +387,38 @@
 
 def create_bff_writer():
     writer = bff_writer()
     writer.write(FASTBUILD_BFF_HEADER)
     return writer
 
 
-def get_min_max_msvc_version(proj : ProjectTemplate) -> Tuple[str, str]:
+def get_min_max_msvc_version(context : EmitContext, proj : ProjectTemplate) -> Tuple[str, str]:
     vmin = None
     vmax = None
-    for tool in proj.toolchains:
-        if vmin is None or tool.ide_version < vmin:
-            vmin = tool.ide_version
-        if vmax is None or tool.ide_version > vmax:
-            vmax = tool.ide_version
+
+    for plat in proj.platforms:
+        if plat.host_system == context.host_system and plat.target_arch == context.host_arch:
+            for tool in proj.platform_toolchains[plat.platform]:
+                if vmin is None or tool.definition.ide_version < vmin:
+                    vmin = tool.definition.ide_version
+                if vmax is None or tool.definition.ide_version > vmax:
+                    vmax = tool.definition.ide_version
+
     return (str(vmin), str(vmax))
 
 
-def find_toolchain(name : str, proj : ProjectTemplate) -> bff_using[Toolchain]:
-    tool = proj.find_toolchain(name)
+def find_cli_tool(tool_name : str, proj : ProjectTemplate):
+    tool = proj.find_cli_tool(tool_name)
+    return tool
+
+
+def find_toolchain(plat_name : str, tool_name : str, proj : ProjectTemplate) -> bff_using[Toolchain, ToolchainDefinition]:
+    tool = proj.find_toolchain(plat_name, tool_name)
     if tool is not None:
-        return bff_using(name=tool.name, obj=tool)
+        return bff_using(name=tool.name, obj=tool, ref=tool.definition)
     return None
 
 
 def find_configuration(name : str, proj : ProjectTemplate) -> Configuration:
     return proj.find_config(name)
 
 
@@ -422,14 +435,18 @@
     return is_target_library(ref.config.kind)
 
 
 def filter_target_executable(ref : Target):
     return not is_target_library(ref.config.kind)
 
 
+def filter_target_prebuild_step(ref : Target):
+    return is_target_prebuild_step(ref.config.kind)
+
+
 def to_str(obj) -> Optional[str]:
     if isinstance(obj, str):
         return obj
     elif isinstance(obj, TargetReference) or issubclass(type(obj), Enum):
         return obj.name
     else:
         return None
@@ -466,14 +483,19 @@
 
 
     def get_compiler_output_path(self, config_str : str, subdir : str):
         return f'build/{subdir}/{config_str}'
 
 
     @staticmethod
+    def get_copy_distributed_files_target_name(config_variant_name:str):
+        return f'COPY_DistributedFiles_{config_variant_name}'
+
+
+    @staticmethod
     def get_runner_path():
         return 'cd ^$(SolutionDir) &amp; .\\build\\scripts\\runner.bat'
 
 
     @staticmethod
     def get_vcxproj_path(name : str):
         return f'build/projects/{name}.vcxproj'
@@ -523,49 +545,56 @@
 
 
     @staticmethod
     def get_zetsubout_update_rebuild_command(context: EmitContext):
         return f'zetsubou regen {context.project_file} --ide --nologo'
 
 
+    # Formats path containing {root} and {config_variant} like so:
+    # {root}/mydir -> C:\Projects\MyProject\mydir
+    # build/generated/{config_variant} -> build/generated/Windows_Debug_MSVC_x64_v193_v143
+    @staticmethod
+    def format_path(format_path:str, context:EmitContext, config_variant:ConfigVariant):
+        return format_path.format(root=context.fs_root, config_variant=get_config_matrix_os_name(config_variant.config_string))
+
+
     def get_update_rebuild_command(self, context: EmitContext):
         return f'{FastbuildEmitter.get_runner_path()} {FastbuildEmitter.get_zetsubout_update_rebuild_command(context)}'
 
 
     def emit_runner_script(self, context: EmitContext):
-        env_dir = context.fs_venv
-
-        relative_env_dir = self.project_to_output_path(context, env_dir).replace('/', '\\')
+        relative_activate = self.project_to_output_path(context, context.fs_venv.activate).replace('/', '\\')
+        relative_deactivate = self.project_to_output_path(context, context.fs_venv.deactivate).replace('/', '\\')
         script = ''
 
-        script += f'CALL {relative_env_dir}\\activate.bat\n'
+        script += f'CALL {relative_activate}\n'
         script +=  'CALL %* \n'
         script +=  'SET taskexitcode=%errorlevel%\n'
-        script += f'CALL {relative_env_dir}\\deactivate.bat\n'
+        script += f'CALL {relative_deactivate}\n'
         script +=  'if %taskexitcode% NEQ 0 (\n'
         script +=  '    exit /b %taskexitcode%\n'
         script +=  ')\n'
 
         context.write_file('build/scripts/runner.bat', script)
 
 
     def fill_base_project(self, context : EmitContext, fbuild: target_kinds.LinkableTarget, target: ResolvedTarget, target_variant: TargetVariant, toolchain : Toolchain):
         subdir = 'bin' if target.get_kind() == ETargetKind.EXECUTABLE else 'lib'
         lib_dir = self.get_compiler_output_path(target_variant.config_variant.config_string, subdir)
         fbuild.LinkerOutput = f'{lib_dir}/{get_linker_output_name(target)}'
 
         fbuild.LinkerOptions = list_to_string(join_unique([
-            target_variant.linker_flags.public, 
+            target_variant.linker_flags.public,
             target_variant.linker_flags.private
         ]))
 
         # Append library paths as flags with /LIBPATH:
         lib_paths = join_unique([
             [ lib_dir ],
-            toolchain.LinkerPaths,
+            toolchain.definition.LinkerPaths,
             target_variant.linker_paths.public,
             target_variant.linker_paths.private
         ])
 
         link_libs_with_refs = join_unique([
             target_variant.link_libraries.public,
             target_variant.link_libraries.private
@@ -579,21 +608,27 @@
         # Linking only to matching variant of other targets
         def map_target_ref_to_str(ref):
             if isinstance(ref, TargetReference):
                 return ProjectTemplate.compile_target_variant_name(ref.target.config.kind, ref.name, target_variant.config_variant.config_string)
             return ref
 
         fbuild.Libraries = list(map(map_target_ref_to_str, filter(filter_target_linkable, refs)))
-        fbuild.LinkerOptions += list_to_string( [ toolchain.i_linker.link(l) for l in libs ])
-        fbuild.LinkerOptions += list_to_string( [ toolchain.i_linker.dir(l)  for l in lib_paths ])
+        fbuild.LinkerOptions += list_to_string( [ toolchain.definition.i_linker.link(l) for l in libs ])
+        fbuild.LinkerOptions += list_to_string( [ toolchain.definition.i_linker.dir(l)  for l in lib_paths ])
 
+        # Depend on copying distributed files to bin
+        fbuild.PreBuildDependencies = [ FastbuildEmitter.get_copy_distributed_files_target_name(target_variant.config_variant.config_string) ]
 
-    def compiler_relative_path(self, context : EmitContext, path : str, target : ResolvedTarget):
-        # return self.project_to_output_path(context, fs.path.join( fs.path.dirname(target.target.get_loaded_from_file()), path ), 'build/projects')
-        return fs.path.join( fs.path.dirname(target.target.get_loaded_from_file()), path )
+
+    def compiler_relative_path(self, context : EmitContext, path : str, target : ResolvedTarget, target_variant : TargetVariant):
+        formatted_path = self.format_path(path, context, target_variant.config_variant)
+        if not os.path.isabs(formatted_path):
+            return fs.path.join( fs.path.dirname(target.target.get_loaded_from_file()), formatted_path)
+        else:
+            return formatted_path
 
 
     def fill_object(self, context : EmitContext, fbuild: target_kinds.ObjTarget, target: ResolvedTarget, target_variant: TargetVariant, root_dir : str, toolchain : Toolchain, source_path : str, includes : bff_includes):
         fbuild.CompilerOutputPath = self.get_compiler_output_path(target_variant.config_variant.config_string, 'obj')
         fbuild.CompilerOutputPrefix = f'{target.target.target}_'
 
         fbuild.CompilerOptions = list_to_string(join_unique([
@@ -602,23 +637,28 @@
         ]))
 
         defines = join_unique([
             target_variant.defines.public,
             target_variant.defines.private
         ])
 
-        fbuild.CompilerOptions += list_to_string([ toolchain.i_compiler.define(d) for d in defines ])
+        fbuild.CompilerOptions += list_to_string([ toolchain.definition.i_compiler.cppstd(toolchain.profile.cppstd) ])
+        fbuild.CompilerOptions += list_to_string([ toolchain.definition.i_compiler.define(d) for d in defines ])
+
+        fbuild.CompilerOptions += list_to_string([ toolchain.definition.i_compiler.include(i) for i in includes.includes ])
+        fbuild.CompilerOptions += list_to_string([ toolchain.definition.i_compiler.system_include(i) for i in includes.system_includes ])
 
-        fbuild.CompilerOptions += list_to_string([ toolchain.i_compiler.include(i) for i in includes.includes ])
-        fbuild.CompilerOptions += list_to_string([ toolchain.i_compiler.system_include(i) for i in includes.system_includes ])
+        out_path = self.compiler_relative_path(context, source_path, target, target_variant)
 
-        out_path = self.compiler_relative_path(context, source_path, target)
+        excluded_paths = list(map(lambda p: self.compiler_relative_path(context, p, target, target_variant), target_variant.source_exclude.paths))
 
         fbuild.CompilerInputPath = out_path
         fbuild.CompilerInputPattern = target_variant.source.patterns
+        fbuild.CompilerInputExcludePath = excluded_paths
+        fbuild.CompilerInputExcludePattern = target_variant.source_exclude.patterns
 
 
     def fill_library(self, context : EmitContext, fbuild : target_kinds.StaticLibTarget, target: ResolvedTarget, target_variant: TargetVariant, root_dir : str, toolchain : Toolchain):
         # self.fill_object(context, fbuild, target, target_variant, root_dir, toolchain)
         fbuild.CompilerOutputPath = self.get_compiler_output_path(target_variant.config_variant.config_string, 'obj')
 
         fbuild.LibrarianOptions = list_to_string(join_unique([
@@ -657,15 +697,15 @@
         includes.append(imported_lib_name)
 
         with create_bff_writer() as writer:
             for config_variant in context.config_matrix.variants:
                 target_variant = target.variants[config_variant.config_string]
 
                 writer.newline()
-                alias = ProjectTemplate.compile_target_variant_name(ETargetKind.IMPORTED_TARGET, target_name, config_variant.config_string)
+                alias = ProjectTemplate.compile_target_variant_name(target.get_kind(), target_name, config_variant.config_string)
 
                 # Target config tuple to be imported into VCXProject
                 config_list_entry = f'{get_config_matrix_os_name(alias)}_Config'
 
                 writer.newline()
                 write_assign(writer, config_list_entry)
 
@@ -680,48 +720,116 @@
                 writer.write(f'.{project_configs_list} + {{ .{config_list_entry} }}')
 
         bff_content = writer.to_string()
         context.write_file(write_path, bff_content)
         return includes
 
 
+    def emit_custom_build_step(self, context: EmitContext, target: ResolvedTarget, target_name : str, project_configs_list : str) -> List[str]:
+        includes = []
+
+        for config_variant in context.config_matrix.variants:
+            target_variant = target.variants[config_variant.config_string]
+            target_variant_name = ProjectTemplate.compile_target_variant_name(ETargetKind.BUILD_STEP, target_name, config_variant.config_string)
+            fb_target_variant_name = get_config_matrix_os_name(target_variant_name)
+
+            cli_tool = find_cli_tool(target.target.config.compiler, context.project_template)
+            cli_fullpath = cli_tool.executable_fullpath
+
+            exclude_src_paths = list(map(lambda p: self.compiler_relative_path(context, p, target, target_variant), target_variant.source_exclude.paths))
+            output_dir = self.compiler_relative_path(context, cli_tool.output_dir, target, target_variant)
+
+            sub_parts = f'{fb_target_variant_name}_parts'
+
+            with create_bff_writer() as writer:
+                writer.newline()
+                write_field(writer, sub_parts, [])
+
+                # For each source path
+                for idx, source_path in enumerate(target_variant.source.paths):
+                    part_name = f'{fb_target_variant_name}_PART_{idx}'
+
+                    writer.newline()
+                    write_keyword(writer, 'Exec', part_name)
+
+                    with bff_struct(writer, is_keyword=True) as struct:
+                        struct.write_field('ExecExecutable', cli_fullpath)
+                        struct.write_field('ExecInputPath', self.compiler_relative_path(context, source_path, target, target_variant))
+                        struct.write_field('ExecInputPattern', target_variant.source.patterns)
+                        struct.write_field('ExecInputExcludePath', exclude_src_paths)
+                        struct.write_field('ExecInputExcludePattern', target_variant.source_exclude.patterns)
+                        struct.write_field('ExecArguments', list_to_string(cli_tool.options).replace('%3', output_dir))
+                        struct.write_field('ExecOutput', os.path.join(output_dir, cli_tool.output_file))
+
+                    writer.newline()
+                    writer.write(f'.{sub_parts} + {{ "{part_name}" }}')
+                    writer.newline()
+
+            write_keyword(writer, 'Alias', target_variant_name)
+            with bff_struct(writer, is_keyword=True) as struct:
+                writer.newline()
+                struct.write_assign('Targets', f'.{sub_parts}')
+
+            writer.newline()
+            writer.newline()
+
+            custom_platform = context.config_matrix.get_config_name(EDefaultConfigSlots.platform, target_variant.config_variant.config_string)
+
+            proj_config = vcxproject.ProjectConfig()
+            proj_config.Platform = find_base_platform_name(custom_platform, context.project_template)
+            proj_config.Config = target_variant.config_variant.config_string
+            proj_config.Target = target_variant_name
+            proj_config.ProjectBuildCommand = self.get_build_command(context, target_variant_name)
+
+            config_name = f'{fb_target_variant_name}_Config'
+            write_assign(writer, config_name)
+            with bff_struct(writer) as struct:
+                struct.write_object(proj_config)
+
+            writer.newline()
+            writer.write(f'.{project_configs_list} + {{ .{config_name} }}')
+
+            custom_step_path = f'configs/{fb_target_variant_name}.bff'
+            write_path = f'{FBUILD_OUTPUT_DIR}/{target_name}/{custom_step_path}'
+            includes.append(custom_step_path)
+
+            bff_content = writer.to_string()
+            context.write_file(write_path, bff_content)
+
+        return includes
+
+
     def gather_includes(self, context : EmitContext, target : ResolvedTarget, target_variant : TargetVariant, toolchain : Toolchain) -> bff_includes:
         raw_includes = join_unique([
             [".\\"],
             target_variant.includes.public,
             target_variant.includes.private
         ])
 
         raw_includes_sys = join_unique([
             target_variant.system_includes.public,
             target_variant.system_includes.private,
-            toolchain.IncludeDirectories,
+            toolchain.definition.IncludeDirectories,
         ])
 
-        def preprocess_includes(raw:List[str]) -> List[str]:
-            includes = []
-            for inc in raw:
-                if not os.path.isabs(inc):
-                    includes.append(self.compiler_relative_path(context, inc, target))
-                else:
-                    includes.append(inc)
-            return includes
+        def preprocess_includes(raw : List[str]) -> List[str]:
+            return list(map(lambda p: self.compiler_relative_path(context, p, target, target_variant), raw))
 
         return bff_includes(
             includes=preprocess_includes(raw_includes),
             system_includes=preprocess_includes(raw_includes_sys)
         )
 
 
     def emit_static_library(self, context: EmitContext, target: ResolvedTarget, target_name : str, project_configs_list : str) -> List[str]:
         includes = []
 
         for config_variant in context.config_matrix.variants:
             target_variant = target.variants[config_variant.config_string]
-            toolchain = find_toolchain(target_variant.compiler, context.project_template)
+            toolchain = find_toolchain(target_variant.platform, target_variant.compiler, context.project_template)
 
             obj_list : List[target_kinds.ObjTarget] = []
             intelisense_includes : List[str] = []
 
             for idx, source_path in enumerate(target_variant.source.paths):
 
                 headers = self.gather_includes(context, target, target_variant, toolchain.obj)
@@ -767,15 +875,15 @@
 
 
     def emit_linkable_target(self, context: EmitContext, target: ResolvedTarget, target_name : str, project_configs_list : str, ctor : Callable[[], target_kinds.LinkableTarget]) -> List[str]:
         includes = []
 
         for config_variant in context.config_matrix.variants:
             target_variant = target.variants[config_variant.config_string]
-            toolchain = find_toolchain(target_variant.compiler, context.project_template)
+            toolchain = find_toolchain(target_variant.platform, target_variant.compiler, context.project_template)
 
             obj_list : List[target_kinds.ObjTarget] = []
             intelisense_includes : List[str] = []
 
             for idx, source_path in enumerate(target_variant.source.paths):
 
                 headers = self.gather_includes(context, target, target_variant, toolchain.obj)
@@ -813,15 +921,15 @@
 
         return includes
 
 
     def emit_buildable_target_variant(self, context: EmitContext, writer : bff_writer, out_target : target_kinds.BaseTarget,
         obj_list : List[target_kinds.BaseTarget], target_variant : TargetVariant, append_to_list : str, includes : List[str]):
 
-        toolchain = find_toolchain(target_variant.compiler, context.project_template)
+        toolchain = find_toolchain(target_variant.platform, target_variant.compiler, context.project_template)
 
         # Sub objects, per source
         for obj in obj_list:
             write_keyword(writer, obj.keyword(), obj.Alias)
             with bff_struct(writer, is_keyword=True) as struct:
                 struct.write_usings([ toolchain ])
                 struct.write_object(obj)
@@ -846,66 +954,73 @@
             def relative_include_to_solution(include_path : str):
                 if os.path.isabs(include_path):
                     return include_path
                 return f'^$(SolutionDir)\\{include_path}'
 
             includes = list(map(relative_include_to_solution, includes))
 
-            struct.write_field('Platform', vs_platform)
-            struct.write_field('Config', target_variant.config_variant.config_string)
-            struct.write_field('Target', out_target.Alias)
-            struct.write_field('PlatformToolset', toolchain.obj.Toolset)
-            struct.write_field('ProjectBuildCommand', self.get_build_command(context, out_target.Alias))
-            struct.write_field('ProjectRebuildCommand', self.get_rebuild_command(context, out_target.Alias))
-            struct.write_field('OutputDirectory', self.get_bin_output_path(target_variant.config_variant.config_string))
-            struct.write_field('IncludeSearchPath', ';'.join(includes).replace('/', '\\'))
+            proj_config = vcxproject.ProjectConfig()
+            proj_config.Platform = vs_platform
+            proj_config.Config = target_variant.config_variant.config_string
+            proj_config.Target = out_target.Alias
+            proj_config.PlatformToolset = toolchain.obj.toolset
+            proj_config.ProjectBuildCommand = self.get_build_command(context, out_target.Alias)
+            proj_config.ProjectRebuildCommand = self.get_rebuild_command(context, out_target.Alias)
+            proj_config.OutputDirectory = self.get_bin_output_path(target_variant.config_variant.config_string)
+            proj_config.IncludeSearchPath = ';'.join(includes).replace('/', '\\')
+
+            struct.write_object(proj_config)
 
         writer.newline()
         writer.write(f'.{append_to_list} + {{ .{config_list_entry} }}')
 
 
     def emit_toolchain(self, context: EmitContext, toolchain: Toolchain):
         writer = create_bff_writer()
         writer.write_line('#once')
 
-        compiler_family = compiler_family_to_fastbuild(toolchain.CompilerFamily)
+        compiler_family = compiler_family_to_fastbuild(toolchain.definition.CompilerFamily)
         compiler = Compiler(
-            Executable=toolchain.Compiler,
+            Executable=toolchain.definition.Compiler,
             CompilerFamily=compiler_family
         )
         write_object(writer, compiler, name=toolchain.name)
 
         writer.newline()
 
         # Emit struct which will be then used by compilation targtes
         write_assign(writer, toolchain.name)
 
         with bff_struct(writer) as struct:
-            struct.write_object(toolchain, hidden_fields=['Compiler', 'CompilerFamily'] + toolchain.get_hidden_fields())
+            struct.write_object(toolchain.definition, hidden_fields=['Compiler', 'CompilerFamily'] + toolchain.definition.get_hidden_fields())
             struct.write_field('Compiler', toolchain.name)
 
         path = f'{FBUILD_OUTPUT_DIR}/toolchains/toolchain_{toolchain.name}.bff'
         context.write_file(path, writer.to_string())
         return path
 
 
     def emit_solution(self, context: EmitContext):
         with create_bff_writer() as writer:
+            #
             # Files to include as global project
+            #
             project_files = []
             def append_proj_files(element):
                 if element is not None:
                     project_files.append(element)
 
             if context.conan is not None and context.project_template.project.conan is not None:
                 append_proj_files(context.project_template.project.conan.build_tools)
                 append_proj_files(context.project_template.project.conan.dependencies)
             append_proj_files(context.project_template.project.get_loaded_from_file())
 
+            #
             # Environment
+            #
             writer.write_line('#import SystemRoot')
             writer.newline()
             writer.write_line('Settings')
             with bff_struct(writer, is_keyword=True) as struct:
                 struct.write_field('Environment', [
                     'SystemRoot=$SystemRoot$',
                     'TMP=$SystemRoot$\\temp',
@@ -913,30 +1028,78 @@
 
             writer.newline()
 
             project_name = context.project_template.project.project
             sln = vssolution.VSSolution()
             sln.Alias = project_name
 
+            #
             # Toolchains
-            for tool in context.project_template.toolchains:
-                tool_inc = self.emit_toolchain(context, tool)
-                if tool_inc != '':
-                    write_include(writer, fs.path.relativefrom(FBUILD_OUTPUT_DIR, tool_inc))
+            #
+            for plat in context.project_template.platforms:
+                if plat.host_system == context.host_system and plat.host_arch == context.host_arch:
+                    for tool in context.project_template.platform_toolchains[plat.platform]:
+                        tool_inc = self.emit_toolchain(context, tool)
+                        if tool_inc != '':
+                            write_include(writer, fs.path.relativefrom(FBUILD_OUTPUT_DIR, tool_inc))
 
             writer.newline()
 
-            # Include Targets bff's
-            for include in self.subprojects:
-                write_include(writer, fs.path.relativefrom(FBUILD_OUTPUT_DIR, include))
+            #
+            # Copy imported files to bin
+            #
+            write_comment_header(writer, 'Copy imported files to bin')
+
+            def path_join_if_not_abs(path:str, fs_root:str):
+                if os.path.isabs(path):
+                    return path
+                return os.path.join(fs_root, path)
+
+            def grep_files(file_src:Source, fs_root:str = ''):
+                results : List[str] = []
+                paths : List[str] = []
+                if fs_root != '':
+                    paths = list(map(lambda p : path_join_if_not_abs(p, fs_root), file_src.paths))
+                else:
+                    paths = file_src.paths
+
+                for search_path in paths:
+                    for pattern in file_src.patterns:
+                        results = join_unique([results, Path(search_path).glob(pattern)])
+                return results
+
+            for config_variant in context.config_matrix.variants:
+                writer.newline()
+
+                # Gather files per configuration
+                dist_files = []
 
+                resolved_target : ResolvedTarget
+                for resolved_target in join_unique([context.resolved_targets, context.conan.resolved_targets]):
+                    target_fs_root = os.path.dirname(resolved_target.target.get_loaded_from_file())
+                    target_variant = resolved_target.variants[config_variant.config_string]
+                    found_files = grep_files(target_variant.distribute_files, target_fs_root)
+                    dist_files = join_unique([dist_files, list(found_files)])
+
+                write_keyword(writer, 'Copy', FastbuildEmitter.get_copy_distributed_files_target_name(config_variant.config_string))
+                with bff_struct(writer, is_keyword=True) as struct:
+                    struct.write_field('Source', [str(fullpath) for fullpath in dist_files])
+                    # Slash at the end is very important! It indicates that we are copying to folder, not to a file
+                    struct.write_field('Dest', f"{self.get_compiler_output_path(config_variant.config_string, 'bin')}/")
+
+            #
             # Config matrix
+            #
             writer.newline()
             write_comment_header(writer, 'Config Matrix')
 
+            # Include Targets bff's
+            for include in self.subprojects:
+                write_include(writer, fs.path.relativefrom(FBUILD_OUTPUT_DIR, include))
+
             writer.newline()
             for config_variant in context.config_matrix.variants:
                 writer.newline()
                 variant_name = get_config_matrix_os_name(config_variant.config_string)
                 write_assign(writer, variant_name)
                 with bff_struct(writer) as struct:
                     custom_platform = context.config_matrix.get_config_name(EDefaultConfigSlots.platform, config_variant.config_string)
@@ -951,15 +1114,17 @@
 
             writer.newline()
             writer.newline()
             write_field(writer, 'ConfigMatrix',
                 [ f'.{get_config_matrix_os_name(config_variant.config_string)}' for config_variant in context.config_matrix.variants ],
                 no_quotations=True)
 
+            #
             # All alias
+            #
             all_target_proj = f'{EDefaultTargets.All.name}-proj'
 
             writer.newline()
             write_comment_header(writer, 'All Alias')
             all_projects = [ f'{target.name}-proj' for target in context.resolved_targets ]
 
             writer.newline()
@@ -1011,15 +1176,17 @@
 
                     writer.newline()
                     write_append_field(writer, 'Configs', '.ThisConfig', outer_scope=True, no_quotations=True)
 
                 writer.newline()
                 struct.write_assign('ProjectConfigs', '.Configs')
 
+            #
             # Update solution
+            #
             update_target_proj = f'{EDefaultTargets.Update.name}-proj'
 
             writer.newline()
             write_keyword(writer, vcxproject.VCXProject.keyword(), update_target_proj)
             with bff_struct(writer, is_keyword=True) as struct:
                 struct.write_field('ProjectOutput', self.get_vcxproj_path(EDefaultTargets.Update.name))
                 struct.write_field('OutputDirectory', PROJ_OUTPUT_DIR)
@@ -1044,18 +1211,22 @@
 
                     writer.newline()
                     write_append_field(writer, 'Configs', '.ThisConfig', outer_scope=True, no_quotations=True)
 
                 writer.newline()
                 struct.write_assign('ProjectConfigs', '.Configs')
 
+            #
             # Default targets - commands
+            #
             default_targets = [ all_target_proj, update_target_proj ]
 
+            #
             # Solution
+            #
             writer.newline()
             write_keyword(writer, sln.keyword(), f'{sln.Alias}')
             with bff_struct(writer, is_keyword=True) as struct:
                 struct.write_field('SolutionOutput', f'{project_name}.sln')
                 struct.write_field('SolutionProjects', default_targets + all_projects)
                 struct.next()
                 writer.write('.SolutionConfigs = .ConfigMatrix')
@@ -1063,15 +1234,15 @@
                 writer.write(f".SolutionBuildProject = '{all_target_proj}'")
                 writer.newline()
                 write_assign(writer, 'SolutionDependencies')
                 with bff_struct(writer) as substruct:
                     substruct.write_field('Projects', all_projects)
                     substruct.write_field('Dependencies', [all_target_proj])
 
-                min_ver, max_ver = get_min_max_msvc_version(context.project_template)
+                min_ver, max_ver = get_min_max_msvc_version(context, context.project_template)
                 struct.write_field('SolutionVisualStudioVersion', max_ver)
                 struct.write_field('SolutionMinimumVisualStudioVersion', min_ver)
 
                 # Folders
                 folders = []
                 def add_folder(name : str, title : str, targets : List[str]):
                     folders.append(f'.{name}')
@@ -1111,17 +1282,20 @@
 
         elif target.target.config.kind == ETargetKind.DYNAMIC_LIBRARY:
             config_includes = self.emit_dynamic_library(context, target, target_name, project_configs_list)
 
         elif target.target.config.kind == ETargetKind.STATIC_LIBRARY:
             config_includes = self.emit_static_library(context, target, target_name, project_configs_list)
 
-        elif target.target.config.kind == ETargetKind.IMPORTED_TARGET:
+        elif target.target.config.kind == ETargetKind.IMPORTED_TARGET or target.target.config.kind == ETargetKind.HEADER_ONLY:
             config_includes = self.emit_imported_target(context, target, target_name, project_configs_list)
 
+        elif target.target.config.kind == ETargetKind.BUILD_STEP:
+            config_includes = self.emit_custom_build_step(context, target, target_name, project_configs_list)
+
         else:
             raise NotImplementedError(f"FASTBuild bff emission for target kind '{target.target.config.kind.name}' is not yet implemented!")
 
         vcxproj = vcxproject.VCXProject()
         vcxproj.Alias = f'{target_name}-proj'
         vcxproj.ProjectOutput = self.get_vcxproj_path(target_name)
         vcxproj.ProjectConfigs = project_configs_list
```

### Comparing `zetsubou-0.6.4/zetsubou/fastbuild/target_kinds.py` & `zetsubou-0.7.0/zetsubou/fastbuild/target_kinds.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
     ###############################################
     # Additional options
     ###############################################
 
     # (optional) Force targets to be built before this DLL (Rarely needed,
     # but useful when DLL relies on externally generated files).
-    PreBuildDependencies : Optional[str]
+    PreBuildDependencies : List[str]
     # (optional) Environment variables to use for local build
     # If set, linker uses this environment
     # If not set, linker uses .Environment from your Settings node
     Environment: List[str]
 
 
 class AppTarget(LinkableTarget):
@@ -97,15 +97,15 @@
     # (optional) Recurse into dirs when finding files (default true)
     CompilerInputPathRecurse : Optional[bool]
     # (optional) Path(s) to exclude from compilation
     CompilerInputExcludePath : Optional[str]
     # (optional) File(s) to exclude from compilation (partial, root-relative of full path)
     CompilerInputExcludedFiles : Optional[str]
     # (optional) Pattern(s) to exclude from compilation
-    CompilerInputExcludePatter : Optional[str]
+    CompilerInputExcludePattern : Optional[str]
     # (optional) Explicit array of files to build
     CompilerInputFiles : Optional[List[str]]
     # (optional) Root path to use for .obj path generation for explicitly listed files
     CompilerInputFilesRoot : Optional[str]
     # (optional) Unity to build (or Unities)
     CompilerInputUnity : Optional[str]
     # (optional) Don't fail if no inputs are found
```

### Comparing `zetsubou-0.6.4/zetsubou/fastbuild/vcxproject.py` & `zetsubou-0.7.0/zetsubou/fastbuild/vcxproject.py`

 * *Files identical despite different names*

### Comparing `zetsubou-0.6.4/zetsubou/fastbuild/vssolution.py` & `zetsubou-0.7.0/zetsubou/fastbuild/vssolution.py`

 * *Files identical despite different names*

### Comparing `zetsubou-0.6.4/zetsubou/logo.py` & `zetsubou-0.7.0/zetsubou/logo.py`

 * *Files identical despite different names*

### Comparing `zetsubou-0.6.4/zetsubou/project/config_matrix.py` & `zetsubou-0.7.0/zetsubou/project/config_matrix.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,14 +22,19 @@
 
 
 @dataclass
 class ConfigMatrix:
     variants: List[ConfigVariant]
     slots: List[str]
 
+    def has_variant(self, variant_string:str):
+        return any(filter(lambda v : v.config_string == variant_string, self.variants))
+
+    # Queries variants matching slot values present in dictionary
+    # Egx. { 'configuration' : 'DEBUG' }
     def find_variants(self, data: dict):
         results = []
 
         for variant in self.variants:
             is_variant_ok = True
 
             for filter_name, filter_value in data.items():
```

### Comparing `zetsubou-0.6.4/zetsubou/project/model/configuration.py` & `zetsubou-0.7.0/zetsubou/project/model/configuration.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from typing import List
 from dataclasses import dataclass, field
 
 from zetsubou.project.model.configuration_enums import EBaseConfiguration
 from zetsubou.project.model.filter import TargetFilter
-from zetsubou.project.model.runtime_library import ERuntimeLibrary
 from zetsubou.project.model.target import TargetData
 from bentoudev.dataclass.base import loaded_from_file
 
 
 @dataclass
 class ConfigurationData(TargetData):
     filter: TargetFilter = field(default_factory=TargetFilter)
@@ -15,8 +14,7 @@
 
 @dataclass
 @loaded_from_file
 class Configuration(TargetData):
     configuration: str = None
     base_configuration: EBaseConfiguration = None
     filters: List[ConfigurationData] = field(default_factory=list)
-    runtime_library: ERuntimeLibrary = ERuntimeLibrary.DYNAMIC_RELEASE
```

### Comparing `zetsubou-0.6.4/zetsubou/project/model/platform_data.py` & `zetsubou-0.7.0/zetsubou/project/model/toolchain_profile.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,39 +1,48 @@
-from typing import List, Optional, Union
+# pyright: reportMissingImports=false
+# pylint: disable=import-error, bare-except
+from typing import Optional, List, Union
 from dataclasses import dataclass, field
 
-from zetsubou.project.model.platform_enums import ESystem, EArch, EVersionSelector
-from zetsubou.project.model.filter import TargetFilter
-from zetsubou.project.model.target import TargetData
-from zetsubou.project.model.toolchain import ECompilerFamily, ECppStandard
+# This file can be imported from conan generator
+# So it needs to support importing via absolute and relative packages
+try:
+    from zetsubou.project.model.configuration_enums import EBaseConfiguration
+    from zetsubou.project.model.platform_enums import EArch, EVersionSelector
+    from zetsubou.project.model.runtime_library import ERuntimeLibrary
+    from zetsubou.project.model.toolchain_enums import ECompilerFamily, ECppStandard
+except:
+    pass
+
+
+try:
+    from configuration_enums import EBaseConfiguration
+    from platform_enums import EArch, EVersionSelector
+    from runtime_library import ERuntimeLibrary
+    from toolchain_enums import ECompilerFamily, ECppStandard
+except:
+    pass
 
 
 @dataclass
-class PlatformData(TargetData):
-    filter: TargetFilter = field(default_factory=TargetFilter)
+class IToolchainProfile:
+    target_arch: Optional[EArch] = None
+    compiler_family: Optional[ECompilerFamily] = None
+    compiler_version: Optional[Union[EVersionSelector, str]] = None
+    cppstd: Optional[ECppStandard] = None
 
 
 @dataclass
-class IPlatformToolchain:
-    family: ECompilerFamily
-    version: Union[EVersionSelector, List[str]]
-    cppstd: ECppStandard
+class Windows_ToolchainProfile(IToolchainProfile):
+    toolset: Optional[Union[EVersionSelector, str]] = None
+    runtime: Optional[ERuntimeLibrary] = None
 
 
 @dataclass
-class IWindowsToolchain(IPlatformToolchain):
-    toolset: Union[EVersionSelector, List[str]]
+class Linux_ToolchainProfile(IToolchainProfile):
+    libcxx: Optional[str] = None
 
 
 @dataclass
-class ILinuxToolchain(IPlatformToolchain):
-    libcxx: List[str]
-
-
-@dataclass
-class PlatformDataclass(TargetData):
-    platform: str = None
-    host_system: ESystem = None
-    host_arch: EArch = None
-    target_arch: EArch = None
-    filters: Optional[List[PlatformData]] = field(default_factory=list)
-    toolchains: List[Union[IPlatformToolchain, IWindowsToolchain, ILinuxToolchain]] = field(default_factory=list)
+class Profile:
+    build_type: Optional[EBaseConfiguration] = None
+    toolchains: List[Union[IToolchainProfile, Windows_ToolchainProfile, Linux_ToolchainProfile]] = field(default_factory=list)
```

### Comparing `zetsubou-0.6.4/zetsubou/project/model/project_template.py` & `zetsubou-0.7.0/zetsubou/project/model/project_template.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,20 +3,22 @@
 
 from bentoudev.dataclass.base import loaded_from_file, track_source
 
 
 @dataclass
 @track_source
 class ProjectConfig:
-    verbose_build: bool = False
+    verbose_build: Optional[bool] = False
+    dev_profile: str = ''
     platforms: List[str] = field(default_factory=list)
     configurations: List[str] = field(default_factory=list)
+    cli_tools: Optional[List[str]] = field(default_factory=list)
     # slots: Optional[List[str]] = field(default_factory=list)
     rules: Optional[List[str]] = field(default_factory=list)
-    config_string: str = ''
+    config_string: Optional[str] = '{platform}-{configuration}-{toolchain}'
     venv: Optional[str] = ''
 
 
 @dataclass
 class Option:
     name: str
     values: List[str]
```

### Comparing `zetsubou-0.6.4/zetsubou/project/model/target.py` & `zetsubou-0.7.0/zetsubou/project/model/target.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     public: Optional[List['zetsubou.project.model.target.TargetReference']] = field(default_factory=list)    # noqa: F821
     private: Optional[List['zetsubou.project.model.target.TargetReference']] = field(default_factory=list)   # noqa: F821
 
 
 @dataclass
 class Source:
     paths: List[str] = field(default_factory=list)
-    patterns: List[str] = field(default_factory=list)
+    patterns: Optional[List[str]] = field(default_factory=list)
 
 
 @dataclass
 class PropertyList:
     interface: Optional[List[str]] = field(default_factory=list)
     public: Optional[List[str]] = field(default_factory=list)
     private: Optional[List[str]] = field(default_factory=list)
@@ -31,32 +31,35 @@
     pass
 
 
 @dataclass
 class TargetData:
     dependencies: Optional[Dependencies] = field(default=None)
     source: Optional[Source] = field(default=None)
+    source_exclude: Optional[Source] = field(default=None)
     includes: Optional[PathList] = field(default=None)
     system_includes: Optional[PathList] = field(default=None)
     defines: Optional[PropertyList] = field(default=None)
     compiler_flags: Optional[PropertyList] = field(default=None)
     linker_flags: Optional[PropertyList] = field(default=None)
     librarian_flags: Optional[PropertyList] = field(default=None)
     linker_paths: Optional[PathList] = field(default=None)
     link_libraries: Optional[PropertyList] = field(default=None)
+    distribute_files: Optional[Source] = field(default=None)
 
 
 @dataclass
 class TargetFilterData(TargetData):
     filter: TargetFilter = field(default_factory=TargetFilter)
 
 
 @dataclass
 class TargetConfig:
     kind: ETargetKind
+    compiler: Optional[str] = None
 
 
 @dataclass
 @loaded_from_file
 @track_source
 class Target(TargetData):
     target: str = ''
@@ -79,7 +82,14 @@
             return self.name == other.name
         return False
 
     def __ne__(self, other):
         # Not strictly necessary, but to avoid having both x==y and x!=y
         # True at the same time
         return not(self == other)
+
+
+def find_target(targets: List[Target], name: str) -> Optional[Target]:
+    for target in targets:
+        if target.target == name:
+            return target
+    return None
```

### Comparing `zetsubou-0.6.4/zetsubou/project/model/toolchain.py` & `zetsubou-0.7.0/zetsubou/project/model/toolchain.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from dataclasses import dataclass, fields
 from typing import List, Optional
-from enum import Enum, auto
 from abc import ABC, abstractmethod
 
 from zetsubou.project.model.kind import ETargetKind
 from zetsubou.project.model.toolchain_enums import ECompilerFamily, ELibrarianFamily, ELinkerFamily, ECppStandard
+from zetsubou.project.model.toolchain_profile import IToolchainProfile
 from zetsubou.utils.common import Version, filename_no_ext, fix_path
 
 
 class ICompiler(ABC):
     @abstractmethod
     def output(self) -> str:
         pass
@@ -232,27 +232,27 @@
         ELinkerFamily.LLD_LINK : LLD_LINK_Linker(),
         ELinkerFamily.LD_LLD : LD_LLD_Linker(),
         ELinkerFamily.LD : LD_Linker(),
     }.get(family)
 
 
 @dataclass
-class Toolchain:
+class ToolchainDefinition:
     name: str
     version : Version
     ide_version : Version
     vs_install_path : str
     arch : str
 
     i_compiler : ICompiler
     i_librarian : ILibrarian
     i_linker : ILinker
 
     # Toolset
-    Toolset : str
+    Toolset : List[str]
 
     # Directories added to PATH
     PathEnv: List[str]
 
     # Default include directories
     IncludeDirectories: List[str]
 
@@ -301,25 +301,25 @@
     # Librarian flags
     LibrarianOptions : str
 
 
 
     @staticmethod
     def create(name:str, compiler_exe:str, librarian_exe:str, linker_exe:str,
-     *, CompilerOptions: str = '', LibrarianOptions: str = '', LinkerOptions: str = '', **kwargs) -> Optional['Toolchain']:
+     *, CompilerOptions: str = '', LibrarianOptions: str = '', LinkerOptions: str = '', **kwargs) -> Optional['ToolchainDefinition']:
 
         compiler_family = guess_compiler_family(compiler_exe)
         librarian_family = guess_librarian_family(librarian_exe)
         linker_family = guess_linker_family(linker_exe)
 
         i_compiler = get_compiler_by_family(compiler_family)
         i_librarian = get_librarian_by_family(librarian_family)
         i_linker = get_linker_by_family(linker_family)
 
-        return Toolchain(
+        return ToolchainDefinition(
             name=name,
 
             i_compiler=i_compiler,
             Compiler=compiler_exe,
             CompilerFamily=compiler_family,
             CompilerOptions=i_compiler.output() + CompilerOptions,
 
@@ -337,11 +337,23 @@
         )
 
     def __hash__(self):
         return hash(self.name)
 
     def get_hidden_fields(self) -> List[str]:
         result = []
-        for field in fields(Toolchain):
+        for field in fields(ToolchainDefinition):
             if field.name.islower():
                 result.append(field.name)
         return result
+
+
+# The actual toolchain that can be used
+@dataclass
+class Toolchain:
+    name: str
+    profile: IToolchainProfile
+    definition: ToolchainDefinition
+    toolset: str
+
+    def __hash__(self):
+        return hash(self.name)
```

### Comparing `zetsubou-0.6.4/zetsubou/project/model/toolchain_enums.py` & `zetsubou-0.7.0/zetsubou/project/model/toolchain_enums.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,8 +24,12 @@
 
 class ECppStandard(Enum):
     cpp11 = auto()
     cpp14 = auto()
     cpp17 = auto()
     cpp20 = auto()
     cpp23 = auto()
-    latest = auto()
+    latest = auto()
+
+    @staticmethod
+    def default():
+        return ECppStandard.cpp20
```

### Comparing `zetsubou-0.6.4/zetsubou/project/runtime/resolve.py` & `zetsubou-0.7.0/zetsubou/project/runtime/resolve.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from zetsubou.project.model.filter import TargetFilter
 
 from zetsubou.project.base_context import BaseContext
 from zetsubou.project.model.kind import ETargetKind
 from zetsubou.project.config_matrix import ConfigVariant, ConfigMatrix
 from zetsubou.project.runtime.project_loader import ProjectTemplate
 from zetsubou.project.model.target import PathList, Target, TargetData, Source, TargetReference, PropertyList
+from zetsubou.project.model.toolchain import Toolchain
 
 
 def PrintDataclass(clazz, id = 0):
     prefix = ''
     for _ in range(id):
         prefix += ' '
 
@@ -38,19 +39,21 @@
         return True
 
     conf_lower = config.lower()
     matrix_lower = config_matrix.config_string.lower()
     return fnmatch.fnmatch(matrix_lower, conf_lower)
 
 
-def config_matches_filter(filter: TargetFilter, config_variant : ConfigVariant, target : Target, config: Configuration) -> bool:
+def config_matches_filter(filter: TargetFilter, config_variant : ConfigVariant, target : Target, config: Configuration, toolchain:Toolchain) -> bool:
     if (
             config_matches_variant(filter.config_string, config_variant) and
-            (filter.kind is None or target.config.kind == filter.kind) and
-            (filter.runtime_library is None or config.runtime_library == filter.runtime_library)
+            (filter.kind is None or target.config.kind in filter.kind) and
+            # TODO: FIXME: This is windows only!!!
+            (filter.runtime_library is None or toolchain.profile.runtime in filter.runtime_library) and
+            (filter.base_configuration is None or config.base_configuration in filter.base_configuration)
        ):
         return True
     return False
 
 
 def append_list(target: Optional[List[Any]], source: Optional[List[Any]]):
     if target is None:
@@ -72,14 +75,15 @@
         append_list(target.private, source.private)
 
 
 @dataclass
 class TargetVariant(TargetData):
     config_variant: ConfigVariant = None
     compiler: str = ''
+    platform: str = ''
 
     def __init__(self, config_variant: ConfigVariant):
         TargetData.__init__(self)
         self.config_variant = config_variant
 
         def init_sources(src: Source):
             src.paths = []
@@ -178,50 +182,51 @@
     if source is not None:
         base_fullpath = os.path.normpath(os.path.join(fs_root, base_path))
         dep_fullpath = os.path.normpath(os.path.join(fs_root, dep_path))
         rel_dep_to_base = os.path.relpath(os.path.dirname(dep_fullpath), os.path.dirname(base_fullpath))
         target += [ os.path.join(rel_dep_to_base, i) for i in source ]
 
 
-def apply_slot(context: ResolveContext, target_variant: TargetVariant, config_variant: ConfigVariant, slot_name: str, slot_value: str, target: Target, config: Configuration):
+def apply_slot(context: ResolveContext, target_variant: TargetVariant, config_variant: ConfigVariant, slot_name: str, slot_value: str, target: Target, config: Configuration, toolchain:Toolchain):
     if EDefaultConfigSlots.toolchain.name == slot_name:
         target_variant.compiler = slot_value
 
     elif EDefaultConfigSlots.platform.name == slot_name:
         platform = context.project.find_platform(slot_value)
+        target_variant.platform = platform.platform
         target_variant.apply(platform)
 
         for plat_filter in platform.filters:
-            if config_matches_filter(plat_filter.filter, config_variant, target, config):
+            if config_matches_filter(plat_filter.filter, config_variant, target, config, toolchain):
                 target_variant.apply(plat_filter)
 
     elif EDefaultConfigSlots.configuration.name == slot_name:
         config = context.project.find_config(slot_value)
         target_variant.apply(config)
 
         for conf_filter in config.filters:
-            if config_matches_filter(conf_filter.filter, config_variant, target, config):
+            if config_matches_filter(conf_filter.filter, config_variant, target, config, toolchain):
                 target_variant.apply(conf_filter)
 
 
-def apply_dependencies_refl(context: ResolveContext, target : Target, target_variant: TargetVariant, config_variant: ConfigVariant, config: Configuration):
+def apply_dependencies_refl(context: ResolveContext, target : Target, target_variant: TargetVariant, config_variant: ConfigVariant, config: Configuration, toolchain:Toolchain):
     target_cls_fields = fields(TargetData)
     target_source_path = target.get_loaded_from_file()
 
     accessors = [ 'private', 'public', 'interface' ]
     for access in accessors:
         deps : Optional[List[TargetReference]] = getattr(target_variant.dependencies, access)
 
         if deps is not None:
             for dep_ref in deps:
                 lnk_libs = getattr(target_variant.link_libraries, access)
                 lnk_libs.append(dep_ref)
                 setattr(target_variant.link_libraries, access, lnk_libs)
 
-                dep_variant = process_target_variant(context, dep_ref.target, config_variant, config)
+                dep_variant = create_target_variant(context, dep_ref.target, config_variant, config, toolchain)
                 dep_source_path = dep_ref.target.get_loaded_from_file()
 
                 imported_dep_target : bool = dep_ref.target.config.kind == ETargetKind.IMPORTED_TARGET
 
                 if imported_dep_target:
                     # Manually pass imported includes as system ones
                     sys_inc_value_access = getattr(target_variant.system_includes, access)
@@ -262,44 +267,39 @@
                             append_list(field_value_access, dep_field_iface)
 
                         setattr(field_value, access, field_value_access)
 
                     setattr(target_variant, data_field.name, field_value)
 
 
-def process_target_variant(context: ResolveContext, target: Target, config_variant: ConfigVariant, config: Configuration) -> TargetVariant:
+def create_target_variant(context: ResolveContext, target: Target, config_variant: ConfigVariant, config: Configuration, toolchain:Toolchain) -> TargetVariant:
     target_variant = context.find_target_variant(target, config_variant.config_string)
     if target_variant is None:
         target_variant = TargetVariant(config_variant)
         target_variant.apply(target)
 
         for filter_data in target.filters:
-            if config_matches_filter(filter_data.filter, config_variant, target, config):
+            if config_matches_filter(filter_data.filter, config_variant, target, config, toolchain):
                 target_variant.apply(filter_data)
 
         for slot_name, slot_value in config_variant.slots.items():
-            apply_slot(context, target_variant, config_variant, slot_name, slot_value, target, config)
+            apply_slot(context, target_variant, config_variant, slot_name, slot_value, target, config, toolchain)
 
         for rule in context.project.rules:
             for filter_data in rule.filters:
-                if config_matches_filter(filter_data.filter, config_variant, target, config):
+                if config_matches_filter(filter_data.filter, config_variant, target, config, toolchain):
                     target_variant.apply(filter_data)
 
-        apply_dependencies_refl(context, target, target_variant, config_variant, config)
+        apply_dependencies_refl(context, target, target_variant, config_variant, config, toolchain)
 
     context.add_target_variant(target, config_variant, target_variant)
     return target_variant
 
 
-def create_target_variants(proj_template: ProjectTemplate, config_matrix: ConfigMatrix, targets: List[Target]):
-    context = ResolveContext(project=proj_template)
-
-    return process_target_variants_list(context, config_matrix, targets)
-
-
-def process_target_variants_list(context: ResolveContext, config_matrix: ConfigMatrix, targets: List[Target]):
+def resolve_target_variants(context: ResolveContext, config_matrix: ConfigMatrix, targets: List[Target]):
     for target in targets:
         for config_variant in config_matrix.variants:
+            toolchain = context.project.find_toolchain(config_variant.get_slot(EDefaultConfigSlots.platform), config_variant.get_slot(EDefaultConfigSlots.toolchain))
             config = context.project.find_config(config_variant.get_slot(EDefaultConfigSlots.configuration))
-            process_target_variant(context, target, config_variant, config)
+            create_target_variant(context, target, config_variant, config, toolchain)
 
     return context.resolved_targets
```

### Comparing `zetsubou-0.6.4/zetsubou/system/tools.py` & `zetsubou-0.7.0/zetsubou/system/tools.py`

 * *Files identical despite different names*

### Comparing `zetsubou-0.6.4/zetsubou/system/windows/msvc.py` & `zetsubou-0.7.0/zetsubou/system/windows/msvc.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,14 +10,14 @@
     }
 
     if arch not in lookup:
         raise ProjectError(f"Arch '{arch}' is not supported for MSVC!")
 
     return lookup.get(arch)
 
-def runtime_from_msvc_legacy(runtime:str) -> Optional[ERuntimeLibrary]:
-    return {
-        'MD' : ERuntimeLibrary.DYNAMIC_RELEASE,
-        'MDd' : ERuntimeLibrary.DYNAMIC_DEBUG,
-        'MT' : ERuntimeLibrary.STATIC_RELEASE,
-        'MTd' : ERuntimeLibrary.STATIC_DEBUG
-    }.get(runtime, None)
+# def runtime_from_msvc_legacy(runtime:str) -> Optional[ERuntimeLibrary]:
+#     return {
+#         'MD' : ERuntimeLibrary.DYNAMIC_RELEASE,
+#         'MDd' : ERuntimeLibrary.DYNAMIC_DEBUG,
+#         'MT' : ERuntimeLibrary.STATIC_RELEASE,
+#         'MTd' : ERuntimeLibrary.STATIC_DEBUG
+#     }.get(runtime, None)
```

### Comparing `zetsubou-0.6.4/zetsubou/system/windows/vswhere.py` & `zetsubou-0.7.0/zetsubou/system/windows/vswhere.py`

 * *Files identical despite different names*

### Comparing `zetsubou-0.6.4/zetsubou/system/windows/windows.py` & `zetsubou-0.7.0/zetsubou/system/windows/windows.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import winreg
 import os, json
 from typing import List, Optional, Any
 from dataclasses import dataclass
 from zetsubou.project.model.platform_enums import EArch
 
-from zetsubou.project.model.toolchain import ECompilerFamily, Toolchain
+from zetsubou.project.model.toolchain import ECompilerFamily, ToolchainDefinition
 from zetsubou.system.windows import vswhere
 from zetsubou.utils import logger
 from zetsubou.utils.common import Version, get_env_path, get_files, get_subdirs
 from zetsubou.utils.subprocess import call_process
 
 
 def is_current_host(host: str, host_arch: EArch) -> bool:
@@ -42,14 +42,22 @@
                 identifier = os.path.basename(root)
                 if identifier.startswith('v'):
                     toolsets.append(Toolset(full_path=root, identifier=identifier))
 
     return toolsets
 
 
+def unique_toolsets(toolsets:List[Toolset]):
+    result = set()
+    for entry in toolsets:
+        result.add(entry.identifier)
+
+    return list(result)
+
+
 def get_toolset_ver(toolset:Toolset):
     if toolset.identifier.startswith('v'):
         return int(toolset.identifier[1:])
     return 0
 
 
 # Value defined in _MSVC_VER
@@ -147,16 +155,16 @@
                             lib=os.path.join(install_dir, 'Lib', latest_sdk),
                             bin=os.path.join(install_dir, 'bin', latest_sdk),
                         )
                         return sdk
     return None
 
 
-def discover_msvc(host_arch: EArch, vs_instances) -> List[Toolchain]:
-    toolchains : List[Toolchain] = []
+def discover_msvc(host_arch: EArch, vs_instances) -> List[ToolchainDefinition]:
+    toolchains : List[ToolchainDefinition] = []
 
     default_vc_path = 'VC\\Tools\\MSVC'
     default_bin_path = 'bin'
     default_lib_path = 'lib'
     default_include_paths = ['include', 'atlmfc\\include']
     default_compiler_msvc = 'cl.exe'
     default_linker_msvc = 'link.exe'
@@ -200,15 +208,15 @@
 
     for vs_itr in vs_instances:
         installation_path = vs_itr['installationPath']
         vs_ide_version = vs_itr['installationVersion']
         vc_tools = os.path.join(installation_path, default_vc_path)
         vs_version = vs_itr['catalog']['productLineVersion']
 
-        available_toolsets = find_toolsets(installation_path)
+        available_toolsets = unique_toolsets(find_toolsets(installation_path))
 
         if os.path.exists(vc_tools):
 
             vc_versions = get_subdirs(vc_tools)
             vc_ver = max(vc_versions)
 
             # for vc_ver in vc_versions:
@@ -220,61 +228,60 @@
                 if is_current_host(host, host_arch):
                     for arch in get_subdirs(os.path.join(vc_ver_binpath, host)):
 
                         msvc_name = vc_ver.replace('.','_')
                         arch_bin_fullpath = os.path.join(vc_ver_binpath, host, arch)
                         arch_lib_fullpath = os.path.join(vc_ver_libpath, arch)
 
-                        visited_toolsets = set()
+                        msvc_ver = get_cl_exe_compiler_version(os.path.join(arch_bin_fullpath, default_compiler_msvc))
+                        if msvc_ver is None:
+                            continue
 
-                        for toolset in available_toolsets:
-                            if arch in toolset.full_path and toolset.identifier not in visited_toolsets:
-                                visited_toolsets.add(toolset.identifier)
-                                toolchain_name = f'{ECompilerFamily.MSVC.name}_{arch}_vs{vs_version}_v{msvc_name}_{toolset.identifier}'
+                        toolchain_name = f'{ECompilerFamily.MSVC.name}_{arch}_vs{vs_version}_v{msvc_name}'
 
-                                includes = []
-                                includes += [ os.path.join(vc_ver_basepath, inc) for inc in default_include_paths ]
-                                includes += [ os.path.join(installation_path, inc) for inc in additional_include_dirs ]
+                        includes = []
+                        includes += [ os.path.join(vc_ver_basepath, inc) for inc in default_include_paths ]
+                        includes += [ os.path.join(installation_path, inc) for inc in additional_include_dirs ]
 
-                                # TODO: maybe this should be separate for compiler, librarian and linker?
-                                path_envs = []
-                                path_envs += [ arch_bin_fullpath ]
+                        # TODO: maybe this should be separate for compiler, librarian and linker?
+                        path_envs = []
+                        path_envs += [ arch_bin_fullpath ]
 
-                                machine_linker_options = f'/MACHINE:{arch} '
+                        machine_linker_options = f'/MACHINE:{arch} '
 
-                                compiler = Toolchain.create(
-                                    toolchain_name,
-                                    os.path.join(arch_bin_fullpath, default_compiler_msvc),
-                                    os.path.join(arch_bin_fullpath, default_librarian_msvc),
-                                    os.path.join(arch_bin_fullpath, default_linker_msvc),
+                        compiler = ToolchainDefinition.create(
+                            toolchain_name,
+                            os.path.join(arch_bin_fullpath, default_compiler_msvc),
+                            os.path.join(arch_bin_fullpath, default_librarian_msvc),
+                            os.path.join(arch_bin_fullpath, default_linker_msvc),
 
-                                    arch=arch,
+                            arch=arch,
 
-                                    version=Version(vc_ver),
-                                    ide_version=Version(vs_ide_version),
-                                    vs_install_path=installation_path,
+                            version=Version(msvc_ver),
+                            ide_version=Version(vs_ide_version),
+                            vs_install_path=installation_path,
 
-                                    Toolset=toolset.identifier,
+                            Toolset=available_toolsets,
 
-                                    PathEnv=path_envs,
+                            PathEnv=path_envs,
 
-                                    LinkerOptions=machine_linker_options,
+                            LinkerOptions=machine_linker_options,
 
-                                    LinkerPaths=[
-                                        arch_lib_fullpath,
-                                        arch_bin_fullpath,
-                                    ],
+                            LinkerPaths=[
+                                arch_lib_fullpath,
+                                arch_bin_fullpath,
+                            ],
 
-                                    ExtraFiles = default_extra_files,
+                            ExtraFiles = default_extra_files,
 
-                                    RequiredFiles=[],
-                                    IncludeDirectories=includes,
-                                    Defines=[]
-                                )
-                                toolchains.append(compiler)
+                            RequiredFiles=[],
+                            IncludeDirectories=includes,
+                            Defines=[]
+                        )
+                        toolchains.append(compiler)
 
     return toolchains
 
 
 def get_clang_version(clang_exe_path: str) -> Optional[str]:
     out, err = call_process([clang_exe_path, '--version'], capture=True, realtime=False)
     if err is not None:
@@ -283,15 +290,15 @@
     version_prefix = 'clang version '
     version = out[len(version_prefix):]
     version = version.split()[0]
 
     return version
 
 
-def discover_clang(host_arch:EArch, vs_instances) -> List[Toolchain]:
+def discover_clang(host_arch:EArch, vs_instances) -> List[ToolchainDefinition]:
     # We need to find visual studio installations anyway
     # But how to handle standalone LLVM? Ignore it? Or match with what version?
     # All of them? The latest? Per toolset?
 
     # There is a thing I cannot find documentation about
     # Seems the Clang toolset exists in two versions per visual studio installation
     #   egx. 2022 has v170 and v160 folders with Clang
@@ -308,24 +315,25 @@
     # clang.exe will work as an compiler, librarian and linker
     # but we need link.exe to be present in path when calling the compiler
     # how on earth would we do that in fastbuild..?
     # Compiler in fastbuild has environment option!
 
     # TODO: We need to pass Environment from Compiler to DLLs, Libraries and Execs!
     # This will set correct PATH with linker.exe
-    toolchains : List[Toolchain] = []
+    toolchains : List[ToolchainDefinition] = []
 
     default_msvc_path = 'VC\\Tools\\MSVC'
     default_llvm_path = 'VC\\Tools\\Llvm'
     default_bin_path = 'bin'
     default_lib_path = 'lib'
     default_llvm_include_path = 'include'
     default_msvc_include_paths = ['include', 'atlmfc\\include']
     default_compiler_clang = 'clang.exe'
     default_librarian_clang = 'llvm-ar.exe'
+    default_linker_clang = 'lld-link.exe'
     default_compiler_msvc = 'cl.exe'
     default_linker_msvc = 'link.exe'
 
     additional_include_dirs = [
         'VC\\Auxiliary\\VS\\include',
         'VC\\Auxiliary\\VS\\UnitTest\\include'
     ]
@@ -343,15 +351,15 @@
         'msvcp140.dll',
         'vcruntime140.dll',
         'vccorlib140.dll'
     ]
 
     standalone_clangs = []
 
-    def try_create_clang_toolchain(clang_exe_path, msvc_ver_basepath, msvc_host, msvc_arch, vs_version, toolset:Toolset) -> Optional[Toolchain]:
+    def try_create_clang_toolchain(clang_exe_path, msvc_ver_basepath, msvc_host, msvc_arch, vs_version, toolset:Toolset) -> Optional[ToolchainDefinition]:
         clang_ver = get_clang_version(clang_exe_path)
         if clang_ver is None:
             return None
 
         vc_ver_binpath = os.path.join(msvc_ver_basepath, default_bin_path)
         vc_ver_libpath = os.path.join(msvc_ver_basepath, default_lib_path)
         msvc_arch_bin_fullpath = os.path.join(vc_ver_binpath, msvc_host, msvc_arch)
@@ -365,45 +373,46 @@
         clang_ver_name = clang_ver.replace('.','_')
 
         clang_bin_dir = os.path.dirname(clang_exe_path)
         clang_base_dir = os.path.dirname(clang_bin_dir)
         clang_lib_dir = os.path.join(clang_base_dir, default_lib_path)
         clang_include_dir = os.path.join(clang_base_dir, default_llvm_include_path)
         clang_librarian_exe = os.path.join(clang_bin_dir, default_librarian_clang)
+        clang_linker_clang = os.path.join(clang_bin_dir, default_linker_clang)
 
-        compiler_name = f"{ECompilerFamily.CLANG.name}_{msvc_arch}_vs{vs_version}_v{clang_ver_name}_{toolset.identifier}"
+        compiler_name = f"{ECompilerFamily.CLANG.name}_{msvc_arch}_vs{vs_version}_v{clang_ver_name}"
 
         includes = [ clang_include_dir ]
         includes += [ os.path.join(msvc_ver_basepath, inc) for inc in default_msvc_include_paths ]
         includes += [ os.path.join(installation_path, inc) for inc in additional_include_dirs ]
 
         # TODO: maybe this should be separate for compiler, librarian and linker?
         path_envs = []
         path_envs += [ clang_bin_dir, msvc_arch_bin_fullpath ]
 
         machine_linker_options = f'/MACHINE:{msvc_arch} '
 
         sem_msvc_ver = Version(msvc_ver)
         msvc_compat_options = f"-fms-compatibility-version={sem_msvc_ver.major}{sem_msvc_ver.minor} "
 
-        return Toolchain.create(
+        return ToolchainDefinition.create(
             compiler_name,
             clang_exe_path,
             clang_librarian_exe,
             msvc_linker_exe,
 
             CompilerOptions = msvc_compat_options,
             LinkerOptions = machine_linker_options,
 
             arch = msvc_arch,
             version = Version(clang_ver),
             ide_version = Version(vs_ide_version),
             vs_install_path = installation_path,
 
-            Toolset = toolset.identifier,
+            Toolset = [ toolset.identifier ],
             PathEnv = path_envs,
             ExtraFiles = default_extra_files,
 
             LinkerPaths = [
                 clang_lib_dir,
                 clang_bin_dir,
                 msvc_arch_lib_fullpath,
@@ -470,15 +479,15 @@
                                         continue
 
                                     toolchains.append(compiler)
 
     return toolchains
 
 
-def discover_toolchain_list(host_arch: EArch) -> List[Toolchain] :
+def discover_toolchain_list(host_arch: EArch) -> List[ToolchainDefinition] :
     vswhere_path = None
 
     try:
         vswhere_path = vswhere.find_vswhere()
     except Exception:
         pass
 
@@ -487,15 +496,15 @@
         return []
 
     vs_instances = json.loads(vswhere.call_vswhere(vswhere_path))
     if vs_instances is None:
         logger.Warning("vswhere found no VS installations")
         return []
 
-    toolchains : List[Toolchain] = []
+    toolchains : List[ToolchainDefinition] = []
     toolchains += discover_msvc(host_arch, vs_instances)
     toolchains += discover_clang(host_arch, vs_instances)
 
     win10_sdk = discover_win10_sdk()
 
     if win10_sdk is not None:
         logger.Verbose(f"Found Win10SDK in {win10_sdk.base_path}")
```

### Comparing `zetsubou-0.6.4/zetsubou/utils/busy_indicator.py` & `zetsubou-0.7.0/zetsubou/utils/busy_indicator.py`

 * *Files identical despite different names*

### Comparing `zetsubou-0.6.4/zetsubou/utils/cmd_arguments.py` & `zetsubou-0.7.0/zetsubou/utils/cmd_arguments.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,16 +20,15 @@
     parent_parser = argparse.ArgumentParser(add_help=False)
 
     def add_global_options(parser):
         parser.add_argument('--nologo', action='store_true', default=False, help='skip printing of the logo')
         parser.add_argument('--ide', action='store_true', default=False, help='print messages in IDE friendly way')
         parser.add_argument('--dry', action='store_true', default=False, help='make no changes in filesystem')
 
-        parser.add_argument('--base_config', help='Constraints variant matrix to single config')
-        parser.add_argument('--platform', help='Constraints variant matrix to external platform file')
+        parser.add_argument('--profile', help='Constraints variant matrix to external profile')
 
         log_group = parser.add_mutually_exclusive_group()
         log_group.add_argument('--verbose', action='store_true', default=False, help='print more information during execution')
         log_group.add_argument('--silent', action='store_true', default=False, help='print only errors')
 
     add_global_options(parent_parser)
```

### Comparing `zetsubou-0.6.4/zetsubou/utils/common.py` & `zetsubou-0.7.0/zetsubou/utils/common.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,14 +49,27 @@
             return True
         elif self.path > other.path:
             return False
 
         return False
 
 
+def foreach(lst, fn):
+    if lst is None:
+        return
+    if len(lst) == 0:
+        return
+    for element in lst:
+        fn(element)
+
+
+def filter_none(lst):
+    return filter(lambda i : i is not None, lst)
+
+
 def is_in_enum(value, enum_class):
     if isinstance(value, enum_class):
         return True
     return value in enum_class.__members__
 
 
 # Find more appropriate way to do this...
@@ -112,14 +125,15 @@
         if pred(element):
             a.append(element)
         else:
             b.append(element)
     return a, b
 
 
+# TODO replace with *args, this inline temporary array is unnecessary
 def join_unique(lists : List[List[str]]):
     unique = list()
     for entry in lists:
         unique.extend(j for j in entry if j not in unique)
     return unique
```

### Comparing `zetsubou-0.6.4/zetsubou/utils/error_codes.py` & `zetsubou-0.7.0/zetsubou/utils/error_codes.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     UNABLE_TO_FIND_VENV = 150
     UNABLE_TO_DISCOVER_TOOLCHAIN = 200
     UNABLE_TO_INSTALL_CONAN_BUILD_TOOLS = 220
     UNABLE_TO_INSTALL_CONAN_DEPENDENCIES = 222
     UNABLE_TO_LOAD_DEPENDENCIES = 280
     UNABLE_TO_VALIDATE_TARGETS = 290
     UNABLE_TO_CREATE_CONFIGURATIONS = 300
+    UNABLE_TO_RESOLVE_CLI_TOOLS_FULLPATH = 350
     UNABLE_TO_RESOLVE_VARIANTS = 400
     UNABLE_TO_EMIT_PROJECT = 500
     UNABLE_TO_COMMIT_FS = 550
     UNABLE_TO_CREATE_VS_PROJECTS = 600
     UNABLE_TO_CREATE_VS_SOLUTION = 650
     UNABLE_TO_CLEAN = 700
     COMPILATION_FAILED = 800
```

### Comparing `zetsubou-0.6.4/zetsubou/utils/logger.py` & `zetsubou-0.7.0/zetsubou/utils/logger.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import sys
 import traceback
 from enum import Enum
 from colorama import Fore, Style, Back
 from colorama import init as colorama_init
 from zetsubou.utils.error_codes import EErrorCode
+from bentoudev.dataclass.base import EErrorFormat
 
 
 class ELogLevel(Enum):
     Verbose = 0
     Info = 1
     Warning = 2
     Error = 3
@@ -53,14 +54,18 @@
     return True
 
 
 def IsIde():
     return LoggerStorage.ide
 
 
+def GetErrorFormat() -> EErrorFormat:
+    return EErrorFormat.MSVC if IsIde() else EErrorFormat.Pretty
+
+
 def _prefix():
     if LoggerStorage.ide:
         return ''
     else:
         return '\r'
```

### Comparing `zetsubou-0.6.4/zetsubou/utils/subprocess.py` & `zetsubou-0.7.0/zetsubou/utils/subprocess.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 from subprocess import Popen as process_open
 from subprocess import PIPE, STDOUT
 from sys import stdout as sys_stdout
-from typing import List, Callable
+from typing import List, Callable, Optional
 
+from zetsubou.project.model.virtual_environment import VirtualEnvironment
 from zetsubou.utils.common import fix_path_os
 from zetsubou.utils.error_codes import EErrorCode
 
 
 class EnterVenv():
-    venv_path : str = None
+    venv_obj : Optional[VirtualEnvironment] = None
 
-    def __init__(self, venv_path: str):
-        self.venv_path = fix_path_os(f'{venv_path}/activate')
+    def __init__(self, venv_obj : VirtualEnvironment):
+        self.venv_obj = venv_obj
 
     def __enter__(self):
         pass
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         pass
 
     def call_process(self, args : List[str], realtime : bool = False, capture : bool = True, on_error : Callable[[int], EErrorCode] = None, cwd: str = '.'):
-        return call_process_venv(args, [ self.venv_path, '&&' ] + args, realtime, capture, on_error, cwd)
+        return call_process_venv(args, self.venv_obj, realtime, capture, on_error, cwd)
 
 
-def call_process_venv(args : List[str], venv : str, realtime : bool = False, capture : bool = True, on_error : Callable[[int], EErrorCode] = None, cwd: str = '.'):
-    return call_process([ fix_path_os(f'{venv}/activate'), '&&' ] + args, realtime, capture, on_error, cwd)
+def call_process_venv(args : List[str], venv : VirtualEnvironment, realtime : bool = False, capture : bool = True, on_error : Callable[[int], EErrorCode] = None, cwd: str = '.'):
+    return call_process([ fix_path_os(venv.activate), '&&' ] + args, realtime, capture, on_error, cwd)
 
 
 def call_process(args : List[str], realtime : bool = False, capture : bool = True, on_error : Callable[[int], EErrorCode] = None, cwd: str = '.'):
     str_buff : List[str] = []
     err = None
 
     with process_open(args, encoding=sys_stdout.encoding, shell=True, stdout=PIPE, stderr=STDOUT, bufsize=1,
```

### Comparing `zetsubou-0.6.4/zetsubou/utils/yaml_simple_writer.py` & `zetsubou-0.7.0/zetsubou/utils/yaml_simple_writer.py`

 * *Files identical despite different names*

### Comparing `zetsubou-0.6.4/zetsubou/zetsubou.py` & `zetsubou-0.7.0/zetsubou/zetsubou.py`

 * *Files 9% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     try:
         # populate command list
         command_registry = get_all_commands()
 
         # parse cmd arguments
         zet_args = parse_arguments(argv, progname, desc, command_registry)
 
-        if not zet_args.nologo and not zet_args.silent:
+        if not zet_args.nologo and not zet_args.ide and not zet_args.silent:
             print_logo(desc)
 
         if zet_args.ide:
             logger.SetIde(True)
 
         if zet_args.silent:
             logger.SetLogLevel(logger.ELogLevel.Silent)
```

### Comparing `zetsubou-0.6.4/zetsubou.egg-info/PKG-INFO` & `zetsubou-0.7.0/zetsubou.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zetsubou
-Version: 0.6.4
+Version: 0.7.0
 Summary: FASTbuild generator for the helpless
 Author: BentouDev
 Project-URL: Homepage, https://github.com/BentouDev/Zetsubou
 Keywords: fastbuild,C++,cpp,C/C++,developer,tool
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `zetsubou-0.6.4/zetsubou.egg-info/SOURCES.txt` & `zetsubou-0.7.0/zetsubou.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 setup.py
 zetsubou/__init__.py
 zetsubou/__main__.py
 zetsubou/_version.py
 zetsubou/configuration.py
 zetsubou/logo.py
 zetsubou/zetsubou.py
+zetsubou/zetsubou_conan_toolchain.py
 zetsubou.egg-info/PKG-INFO
 zetsubou.egg-info/SOURCES.txt
 zetsubou.egg-info/dependency_links.txt
 zetsubou.egg-info/entry_points.txt
 zetsubou.egg-info/requires.txt
 zetsubou.egg-info/top_level.txt
 zetsubou/commands/__init__.py
@@ -25,50 +26,52 @@
 zetsubou/commands/execute_stage.py
 zetsubou/commands/generate.py
 zetsubou/commands/install.py
 zetsubou/commands/regen.py
 zetsubou/conan/__init__.py
 zetsubou/conan/conan.py
 zetsubou/conan/dependencies.py
+zetsubou/conan/deployer.py
 zetsubou/conan/from_conan.py
 zetsubou/conan/to_conan.py
-zetsubou/conan/generator/conanfile.py
 zetsubou/data/__init__.py
 zetsubou/data/rules/ClangRules.yml
 zetsubou/data/rules/MsvcRules.yml
 zetsubou/fastbuild/__init__.py
 zetsubou/fastbuild/compiler.py
 zetsubou/fastbuild/fastbuild_emit.py
 zetsubou/fastbuild/target_kinds.py
 zetsubou/fastbuild/to_fastbuild.py
 zetsubou/fastbuild/vcxproject.py
 zetsubou/fastbuild/vssolution.py
 zetsubou/project/__init__.py
 zetsubou/project/base_context.py
 zetsubou/project/config_matrix.py
 zetsubou/project/model/__init__.py
+zetsubou/project/model/cli_tool.py
 zetsubou/project/model/config_string.py
 zetsubou/project/model/configuration.py
 zetsubou/project/model/configuration_enums.py
 zetsubou/project/model/filter.py
 zetsubou/project/model/kind.py
 zetsubou/project/model/platform.py
-zetsubou/project/model/platform_data.py
 zetsubou/project/model/platform_enums.py
 zetsubou/project/model/project_template.py
 zetsubou/project/model/rule.py
 zetsubou/project/model/runtime_library.py
 zetsubou/project/model/target.py
 zetsubou/project/model/toolchain.py
 zetsubou/project/model/toolchain_enums.py
+zetsubou/project/model/toolchain_profile.py
+zetsubou/project/model/virtual_environment.py
 zetsubou/project/runtime/__init__.py
 zetsubou/project/runtime/emit.py
-zetsubou/project/runtime/filter_toolchains.py
 zetsubou/project/runtime/project_loader.py
 zetsubou/project/runtime/resolve.py
+zetsubou/project/runtime/validation.py
 zetsubou/system/__init__.py
 zetsubou/system/discover_toolchains.py
 zetsubou/system/tools.py
 zetsubou/system/windows/__init__.py
 zetsubou/system/windows/msvc.py
 zetsubou/system/windows/vswhere.py
 zetsubou/system/windows/windows.py
```

