# Comparing `tmp/bytecodemanipulation-0.2.4.tar.gz` & `tmp/bytecodemanipulation-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bytecodemanipulation-0.2.4.tar", last modified: Thu May  4 14:18:13 2023, max compression
+gzip compressed data, was "bytecodemanipulation-0.2.8.tar", last modified: Sat May  6 15:08:32 2023, max compression
```

## Comparing `bytecodemanipulation-0.2.4.tar` & `bytecodemanipulation-0.2.8.tar`

### file list

```diff
@@ -1,65 +1,127 @@
-drwxrwxrwx   0        0        0        0 2023-05-04 14:18:13.448355 bytecodemanipulation-0.2.4/
--rw-rw-rw-   0        0        0     1082 2022-01-23 14:31:25.000000 bytecodemanipulation-0.2.4/LICENSE
--rw-rw-rw-   0        0        0     5572 2023-05-04 14:18:13.446350 bytecodemanipulation-0.2.4/PKG-INFO
--rw-rw-rw-   0        0        0     4854 2023-05-03 20:01:14.000000 bytecodemanipulation-0.2.4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-04 14:18:13.260793 bytecodemanipulation-0.2.4/bytecodemanipulation/
--rw-rw-rw-   0        0        0    22555 2023-01-08 18:17:44.000000 bytecodemanipulation-0.2.4/bytecodemanipulation/Emulator.py
--rw-rw-rw-   0        0        0    20982 2023-01-15 10:09:48.000000 bytecodemanipulation-0.2.4/bytecodemanipulation/Mixin.py
--rw-rw-rw-   0        0        0    54236 2023-05-04 14:08:30.000000 bytecodemanipulation-0.2.4/bytecodemanipulation/MutableFunction.py
--rw-rw-rw-   0        0        0    12635 2023-05-04 14:15:29.000000 bytecodemanipulation-0.2.4/bytecodemanipulation/MutableFunctionHelpers.py
--rw-rw-rw-   0        0        0     5578 2023-05-02 17:20:16.000000 bytecodemanipulation-0.2.4/bytecodemanipulation/Opcodes.py
--rw-rw-rw-   0        0        0    27090 2023-05-04 14:05:25.000000 bytecodemanipulation-0.2.4/bytecodemanipulation/Optimiser.py
--rw-rw-rw-   0        0        0    11943 2023-05-03 20:02:56.000000 bytecodemanipulation-0.2.4/bytecodemanipulation/Specialization.py
--rw-rw-rw-   0        0        0      165 2023-01-08 18:17:42.000000 bytecodemanipulation-0.2.4/bytecodemanipulation/__init__.py
--rw-rw-rw-   0        0        0       53 2022-11-18 20:41:26.000000 bytecodemanipulation-0.2.4/bytecodemanipulation/annotated_std.py
-drwxrwxrwx   0        0        0        0 2023-05-04 14:18:13.310264 bytecodemanipulation-0.2.4/bytecodemanipulation/assembler/
--rw-rw-rw-   0        0        0    11767 2023-05-04 14:11:24.000000 bytecodemanipulation-0.2.4/bytecodemanipulation/assembler/Emitter.py
--rw-rw-rw-   0        0        0     5543 2023-05-04 09:43:13.000000 bytecodemanipulation-0.2.4/bytecodemanipulation/assembler/Lexer.py
--rw-rw-rw-   0        0        0    74735 2023-05-04 14:14:17.000000 bytecodemanipulation-0.2.4/bytecodemanipulation/assembler/Parser.py
--rw-rw-rw-   0        0        0        0 2023-01-11 16:22:00.000000 bytecodemanipulation-0.2.4/bytecodemanipulation/assembler/__init__.py
--rw-rw-rw-   0        0        0     1570 2023-05-02 12:53:48.000000 bytecodemanipulation-0.2.4/bytecodemanipulation/assembler/hook.py
--rw-rw-rw-   0        0        0     3430 2023-05-04 07:22:54.000000 bytecodemanipulation-0.2.4/bytecodemanipulation/assembler/target.py
-drwxrwxrwx   0        0        0        0 2023-05-04 14:18:13.330884 bytecodemanipulation-0.2.4/bytecodemanipulation/assembler/util/
--rw-rw-rw-   0        0        0      351 2023-01-06 18:03:42.000000 bytecodemanipulation-0.2.4/bytecodemanipulation/assembler/util/CommonUtil.py
--rw-rw-rw-   0        0        0        0 2023-01-13 11:24:36.000000 bytecodemanipulation-0.2.4/bytecodemanipulation/assembler/util/__init__.py
--rw-rw-rw-   0        0        0    11291 2023-05-04 09:24:29.000000 bytecodemanipulation-0.2.4/bytecodemanipulation/assembler/util/parser.py
--rw-rw-rw-   0        0        0     8566 2023-05-02 12:34:49.000000 bytecodemanipulation-0.2.4/bytecodemanipulation/assembler/util/tokenizer.py
--rw-rw-rw-   0        0        0     2530 2023-01-08 18:17:42.000000 bytecodemanipulation-0.2.4/bytecodemanipulation/compiler.py
-drwxrwxrwx   0        0        0        0 2023-05-04 14:18:13.337601 bytecodemanipulation-0.2.4/bytecodemanipulation/data/
--rw-rw-rw-   0        0        0        0 2022-11-18 20:41:26.000000 bytecodemanipulation-0.2.4/bytecodemanipulation/data/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-04 14:18:13.347132 bytecodemanipulation-0.2.4/bytecodemanipulation/data/shared/
--rw-rw-rw-   0        0        0       28 2022-11-18 20:41:26.000000 bytecodemanipulation-0.2.4/bytecodemanipulation/data/shared/__init__.py
--rw-rw-rw-   0        0        0    13614 2023-05-03 20:02:56.000000 bytecodemanipulation-0.2.4/bytecodemanipulation/data/shared/builtin_spec.py
-drwxrwxrwx   0        0        0        0 2023-05-04 14:18:13.364157 bytecodemanipulation-0.2.4/bytecodemanipulation/data/v3_10/
--rw-rw-rw-   0        0        0        0 2022-11-18 20:41:26.000000 bytecodemanipulation-0.2.4/bytecodemanipulation/data/v3_10/__init__.py
--rw-rw-rw-   0        0        0    80683 2023-05-04 14:13:06.000000 bytecodemanipulation-0.2.4/bytecodemanipulation/data/v3_10/assembly_instructions.py
--rw-rw-rw-   0        0        0       48 2023-01-08 18:17:42.000000 bytecodemanipulation-0.2.4/bytecodemanipulation/data/v3_10/specialize.py
-drwxrwxrwx   0        0        0        0 2023-05-04 14:18:13.384909 bytecodemanipulation-0.2.4/bytecodemanipulation/data/v3_11/
--rw-rw-rw-   0        0        0        0 2022-11-26 17:49:51.000000 bytecodemanipulation-0.2.4/bytecodemanipulation/data/v3_11/__init__.py
--rw-rw-rw-   0        0        0    78725 2023-05-04 14:13:06.000000 bytecodemanipulation-0.2.4/bytecodemanipulation/data/v3_11/assembly_instructions.py
--rw-rw-rw-   0        0        0       48 2023-01-08 18:17:42.000000 bytecodemanipulation-0.2.4/bytecodemanipulation/data/v3_11/specialize.py
-drwxrwxrwx   0        0        0        0 2023-05-04 14:18:13.390895 bytecodemanipulation-0.2.4/bytecodemanipulation/data/v3_12/
--rw-rw-rw-   0        0        0        0 2022-11-26 17:50:05.000000 bytecodemanipulation-0.2.4/bytecodemanipulation/data/v3_12/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-04 14:18:13.397909 bytecodemanipulation-0.2.4/bytecodemanipulation/data/v3_9/
--rw-rw-rw-   0        0        0        0 2022-11-26 17:49:58.000000 bytecodemanipulation-0.2.4/bytecodemanipulation/data/v3_9/__init__.py
--rw-rw-rw-   0        0        0     2940 2023-03-25 14:33:01.000000 bytecodemanipulation-0.2.4/bytecodemanipulation/data_loader.py
--rw-rw-rw-   0        0        0     4233 2023-01-08 18:17:43.000000 bytecodemanipulation-0.2.4/bytecodemanipulation/mixin_util.py
--rw-rw-rw-   0        0        0      455 2023-01-08 18:17:43.000000 bytecodemanipulation-0.2.4/bytecodemanipulation/optimise_self.py
--rw-rw-rw-   0        0        0    17871 2023-05-04 14:07:34.000000 bytecodemanipulation-0.2.4/bytecodemanipulation/optimiser_util.py
--rw-rw-rw-   0        0        0      652 2023-01-14 14:32:32.000000 bytecodemanipulation-0.2.4/bytecodemanipulation/util.py
-drwxrwxrwx   0        0        0        0 2023-05-04 14:18:13.280710 bytecodemanipulation-0.2.4/bytecodemanipulation.egg-info/
--rw-rw-rw-   0        0        0     5572 2023-05-04 14:18:12.000000 bytecodemanipulation-0.2.4/bytecodemanipulation.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1894 2023-05-04 14:18:13.000000 bytecodemanipulation-0.2.4/bytecodemanipulation.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-04 14:18:12.000000 bytecodemanipulation-0.2.4/bytecodemanipulation.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2023-05-04 14:18:12.000000 bytecodemanipulation-0.2.4/bytecodemanipulation.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      108 2022-01-27 09:48:33.000000 bytecodemanipulation-0.2.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-04 14:18:13.449354 bytecodemanipulation-0.2.4/setup.cfg
--rw-rw-rw-   0        0        0     1360 2023-05-04 14:17:31.000000 bytecodemanipulation-0.2.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-04 14:18:13.439986 bytecodemanipulation-0.2.4/tests/
--rw-rw-rw-   0        0        0    46901 2023-05-04 14:06:22.000000 bytecodemanipulation-0.2.4/tests/test_Assembly.py
--rw-rw-rw-   0        0        0     3278 2023-01-15 08:18:00.000000 bytecodemanipulation-0.2.4/tests/test_Mixin.py
--rw-rw-rw-   0        0        0     1648 2022-11-19 21:26:32.000000 bytecodemanipulation-0.2.4/tests/test_MutableFunction.py
--rw-rw-rw-   0        0        0      792 2023-05-04 14:06:22.000000 bytecodemanipulation-0.2.4/tests/test_MutableFunctionHelper.py
--rw-rw-rw-   0        0        0     4932 2023-05-04 13:27:16.000000 bytecodemanipulation-0.2.4/tests/test_StandardLibrary.py
--rw-rw-rw-   0        0        0     5944 2023-05-04 14:06:55.000000 bytecodemanipulation-0.2.4/tests/test_issues.py
--rw-rw-rw-   0        0        0    10760 2023-05-04 14:16:08.000000 bytecodemanipulation-0.2.4/tests/test_optimiser_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:08:32.990570 bytecodemanipulation-0.2.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5442 2023-05-06 15:08:32.990570 bytecodemanipulation-0.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4742 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:08:32.974570 bytecodemanipulation-0.2.8/bytecodemanipulation/
+-rw-r--r--   0 runner    (1001) docker     (123)    21892 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/Emulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20385 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/Mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55947 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/MutableFunction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12253 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/MutableFunctionHelpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/Opcodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26316 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/Optimiser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11617 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/Specialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/annotated_std.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:08:32.978570 bytecodemanipulation-0.2.8/bytecodemanipulation/assembler/
+-rw-r--r--   0 runner    (1001) docker     (123)     6816 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/assembler/AbstractBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11963 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/assembler/Emitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5355 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/assembler/Lexer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19821 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/assembler/Parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/assembler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/assembler/hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/assembler/syntax_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/assembler/target.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:08:32.978570 bytecodemanipulation-0.2.8/bytecodemanipulation/assembler/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/assembler/util/CommonUtil.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/assembler/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10926 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/assembler/util/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8259 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/assembler/util/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/compiler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:08:32.978570 bytecodemanipulation-0.2.8/bytecodemanipulation/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:08:32.978570 bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13194 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/builtin_spec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:08:32.982570 bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/expressions/
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/expressions/AttributeAccessExpression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/expressions/CompoundExpression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/expressions/ConstantAccessExpression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/expressions/DerefAccessExpression.py
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/expressions/DiscardValueExpression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/expressions/DynamicAccessExpression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/expressions/GlobalAccessExpression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/expressions/GlobalStaticAccessExpression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/expressions/LocalAccessExpression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/expressions/MacroAccessExpression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/expressions/MacroParameterAcessExpression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/expressions/ModuleAccessExpression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/expressions/StaticAttributeAcccessExpression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/expressions/SubscriptionAccessExpression.py
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/expressions/TopOfStackAccessExpression.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/expressions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:08:32.986570 bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/instructions/
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/instructions/AbstractInstruction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12275 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/instructions/CallAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/instructions/ClassDefinitionAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/instructions/ForEachAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7703 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/instructions/FunctionDefinitionAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3603 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/instructions/IfAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/instructions/JumpAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/instructions/LabelAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/instructions/LoadAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/instructions/LoadConstAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/instructions/LoadFastAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/instructions/LoadGlobalAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22643 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/instructions/MacroAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4438 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/instructions/MacroImportAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/instructions/MacroPasteAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/instructions/MacroReturnAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/instructions/NamespaceAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11250 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/instructions/OpAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/instructions/PopElementAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/instructions/PythonCodeAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/instructions/RaiseAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/instructions/ReturnAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/instructions/StoreAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/instructions/StoreFastAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/instructions/StoreGlobalAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/instructions/WhileAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/instructions/YieldAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/instructions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:08:32.986570 bytecodemanipulation-0.2.8/bytecodemanipulation/data/v3_10/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/v3_10/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/v3_10/assembly_instructions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:08:32.990570 bytecodemanipulation-0.2.8/bytecodemanipulation/data/v3_10/instructions/
+-rw-r--r--   0 runner    (1001) docker     (123)     6805 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/v3_10/instructions/CallAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/v3_10/instructions/ClassDefinitionAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/v3_10/instructions/ForEachAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4985 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/v3_10/instructions/FunctionDefinitionAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/v3_10/instructions/IfAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/v3_10/instructions/JumpAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/v3_10/instructions/LoadConstAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/v3_10/instructions/LoadFastAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/v3_10/instructions/LoadGlobalAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/v3_10/instructions/OpAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/v3_10/instructions/PopElementAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/v3_10/instructions/RaiseAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/v3_10/instructions/ReturnAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/v3_10/instructions/StoreFastAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/v3_10/instructions/StoreGlobalAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/v3_10/instructions/WhileAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/v3_10/instructions/YieldAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/v3_10/instructions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/v3_10/specialize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:08:32.990570 bytecodemanipulation-0.2.8/bytecodemanipulation/data/v3_11/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/v3_11/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data/v3_11/specialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/data_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/mixin_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/optimise_self.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17382 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/optimiser_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/bytecodemanipulation/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:08:32.978570 bytecodemanipulation-0.2.8/bytecodemanipulation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5442 2023-05-06 15:08:32.000000 bytecodemanipulation-0.2.8/bytecodemanipulation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5990 2023-05-06 15:08:32.000000 bytecodemanipulation-0.2.8/bytecodemanipulation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 15:08:32.000000 bytecodemanipulation-0.2.8/bytecodemanipulation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-06 15:08:32.000000 bytecodemanipulation-0.2.8/bytecodemanipulation.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 15:08:32.990570 bytecodemanipulation-0.2.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-05-06 15:08:26.000000 bytecodemanipulation-0.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:08:32.990570 bytecodemanipulation-0.2.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    50336 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/tests/test_Assembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/tests/test_Mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/tests/test_MutableFunction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/tests/test_MutableFunctionHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5288 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/tests/test_StandardLibrary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5730 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/tests/test_issues.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10417 2023-05-06 15:08:16.000000 bytecodemanipulation-0.2.8/tests/test_optimiser_util.py
```

### Comparing `bytecodemanipulation-0.2.4/LICENSE` & `bytecodemanipulation-0.2.8/LICENSE`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2022 uuk0
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2022 uuk0
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `bytecodemanipulation-0.2.4/PKG-INFO` & `bytecodemanipulation-0.2.8/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,130 +1,130 @@
-Metadata-Version: 2.1
-Name: bytecodemanipulation
-Version: 0.2.4
-Summary: High level python bytecode manipulation
-Home-page: https://github.com/uuk0/PyBytecodeManipulator
-Author: uuk
-Author-email: uuk1301@gmail.com
-Project-URL: Bug Tracker, https://github.com/uuk0/PyBytecodeManipulator/issues
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# PyBytecodeManipulator
-A high level cross-version python bytecode manipulation library build ontop 
-of 'dis' and 'inspect' 
-
-Supports code inlining, branch removing and arbitrary code injection into 
-existing functions.
-
-WARNING: using bytecode manipulation on a so low level as we do can break 
-the python runtime at any point without a warning. We circumvent a lot of 
-safety checks normally done. 
-
-WARNING: We cannot make sure that everything works as it should, expect broken code 
-at runtime!
-
-
-Supported python versions:
-
-- 3.10 (main development)
-- 3.11.0[b3] (forward porting; WIP; Currently not working)
-
-Other versions will not work as a lot of config is stored in .json files per-version,
-so you may need to provide your own .json config files for the version you need.
-
-(Some versions might be plug-and-play, but most will require code changes additionally)
-
-## Why are there so many print()-s?
-
-Due to the breaking nature of anything this code touches, and the absents of any traces 
-in the function itself, we decided to add a lot of "debug" statements indicating 
-mostly the who-has-done-what-to-which-method for the runtime. 
-This makes debugging broken code easier, as it is more clear what happened to each transformed function.
-
-If you want them removed, create your own Fork of this and remove them, on your own risk.
-
-We may use in the future the logging library, so you can disable our logger instance, but we 
-are currently in an inter-stage of the code, so other stuff has priority.
-
-## Compatibility with other libraries 
-
-- Nuitka (https://github.com/Nuitka/Nuitka): Incompatible; will break as nuitka removes the \_\_code__ attribute 
-  we modify
-- Other bytecode modification / analysers: Should work as long as you as the user does NOT expose intermediate
-  results which might contain internal instructions
-
-
-## Debugging your injections 
-
-There is the possibility to "debug" functions using the execution emulator.
-It will be able to give you more information about a crash than the python core interpreter,
-but will be a lot slower than it. 
-
-It comes also with the possibility to run your bytecode in another interpreter version, so 
-you can experiment with some stuff.
-In theory, it is also possible to run in python versions not supported by the 
-bytecode manipulation system, but it is not recommended.
-
-TransformationHandler() takes as an arg debug_code and debug_further_calls
-for activating it for all accessed methods. 
-
-BytecodePatchHelper() contains a method enable_verbose_exceptions() for activating it on 
-that exact method.
-
-
-# Examples
-
-TODO
-
-
-# Applied Optimisations
-
-- Constant Expression inlining (can be declared for custom functions to be constant)
-- LOAD_GLOBAL for builtins (if enabled)
-- standard library inlining (if enabled)
-- specialization of methods based on arguments, e.g. constant arguments (when already resolved before, requires one of above options)
-- branch elimination when jumping on a constant (TODO: also if condition can be inferred ahead-of-time, see specialization)
-- local variable elimination
-
-
-# Currently Limitations
-
-- Line Numbers get mixed up, we need some way to assign meaningful line numbers
-- With python 3.11 (?), exception table exists, and this breaks our current concept of one big flow diagram,
-  as exception handling code might exist outside the default flow
-- During optimization, a lot of stuff is being recomputed each optimisation pass, we need to cache that drastically
-- Method inlining is not working properly and needs a lot more testing
-- If the exact type is known at optimisation time (e.g. object creation via class call, or type annotation), we can try to
-  inline method accesses for further optimisation
-- Python 3.12 will likely break how certain operations are stored in instructions, combing opcodes-without-args into a single
-  parent instruction, using the arg to switch between modes
-
-
-# Assembly Code
-
-- The library provides also a way to use some "python-assembly" for writing code
-- This is only python bytecode, so no fancy stuff can be done
-- See ASSEMBLY.md for more information on instructions
-- We provide an import system hook for importing .pyasm files via bytecodemanipulation.assembler.hook
-- You may use the functions from bytecodemanipulation.assembler.target for creating inline-assembly
-
-
-## Code Formatting
-
-We use the python formatting library "black" on our code
-
-# TODO's
-
-- abstract opcode affect away into a .json file describing all opcodes
-- create a json file for defining certain bytecode sequences
-- write more library-specific optimisations
-- write generating bytecode system for emulator, constructing a function pointing to the
-.json file for exception printing, and optimizing wherever possible
-
+Metadata-Version: 2.1
+Name: bytecodemanipulation
+Version: 0.2.8
+Summary: High level python bytecode manipulation
+Home-page: https://github.com/uuk0/PyBytecodeManipulator
+Author: uuk
+Author-email: uuk1301@gmail.com
+Project-URL: Bug Tracker, https://github.com/uuk0/PyBytecodeManipulator/issues
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# PyBytecodeManipulator
+A high level cross-version python bytecode manipulation library build ontop 
+of 'dis' and 'inspect' 
+
+Supports code inlining, branch removing and arbitrary code injection into 
+existing functions.
+
+WARNING: using bytecode manipulation on a so low level as we do can break 
+the python runtime at any point without a warning. We circumvent a lot of 
+safety checks normally done. 
+
+WARNING: We cannot make sure that everything works as it should, expect broken code 
+at runtime!
+
+
+Supported python versions:
+
+- 3.10 (main development)
+- 3.11.0[b3] (forward porting; WIP; Currently not working)
+
+Other versions will not work as a lot of config is stored in .json files per-version,
+so you may need to provide your own .json config files for the version you need.
+
+(Some versions might be plug-and-play, but most will require code changes additionally)
+
+## Why are there so many print()-s?
+
+Due to the breaking nature of anything this code touches, and the absents of any traces 
+in the function itself, we decided to add a lot of "debug" statements indicating 
+mostly the who-has-done-what-to-which-method for the runtime. 
+This makes debugging broken code easier, as it is more clear what happened to each transformed function.
+
+If you want them removed, create your own Fork of this and remove them, on your own risk.
+
+We may use in the future the logging library, so you can disable our logger instance, but we 
+are currently in an inter-stage of the code, so other stuff has priority.
+
+## Compatibility with other libraries 
+
+- Nuitka (https://github.com/Nuitka/Nuitka): Incompatible; will break as nuitka removes the \_\_code__ attribute 
+  we modify
+- Other bytecode modification / analysers: Should work as long as you as the user does NOT expose intermediate
+  results which might contain internal instructions
+
+
+## Debugging your injections 
+
+There is the possibility to "debug" functions using the execution emulator.
+It will be able to give you more information about a crash than the python core interpreter,
+but will be a lot slower than it. 
+
+It comes also with the possibility to run your bytecode in another interpreter version, so 
+you can experiment with some stuff.
+In theory, it is also possible to run in python versions not supported by the 
+bytecode manipulation system, but it is not recommended.
+
+TransformationHandler() takes as an arg debug_code and debug_further_calls
+for activating it for all accessed methods. 
+
+BytecodePatchHelper() contains a method enable_verbose_exceptions() for activating it on 
+that exact method.
+
+
+# Examples
+
+TODO
+
+
+# Applied Optimisations
+
+- Constant Expression inlining (can be declared for custom functions to be constant)
+- LOAD_GLOBAL for builtins (if enabled)
+- standard library inlining (if enabled)
+- specialization of methods based on arguments, e.g. constant arguments (when already resolved before, requires one of above options)
+- branch elimination when jumping on a constant (TODO: also if condition can be inferred ahead-of-time, see specialization)
+- local variable elimination
+
+
+# Currently Limitations
+
+- Line Numbers get mixed up, we need some way to assign meaningful line numbers
+- With python 3.11 (?), exception table exists, and this breaks our current concept of one big flow diagram,
+  as exception handling code might exist outside the default flow
+- During optimization, a lot of stuff is being recomputed each optimisation pass, we need to cache that drastically
+- Method inlining is not working properly and needs a lot more testing
+- If the exact type is known at optimisation time (e.g. object creation via class call, or type annotation), we can try to
+  inline method accesses for further optimisation
+- Python 3.12 will likely break how certain operations are stored in instructions, combing opcodes-without-args into a single
+  parent instruction, using the arg to switch between modes
+
+
+# Assembly Code
+
+- The library provides also a way to use some "python-assembly" for writing code
+- This is only python bytecode, so no fancy stuff can be done
+- See ASSEMBLY.md for more information on instructions
+- We provide an import system hook for importing .pyasm files via bytecodemanipulation.assembler.hook
+- You may use the functions from bytecodemanipulation.assembler.target for creating inline-assembly
+
+
+## Code Formatting
+
+We use the python formatting library "black" on our code
+
+# TODO's
+
+- abstract opcode affect away into a .json file describing all opcodes
+- create a json file for defining certain bytecode sequences
+- write more library-specific optimisations
+- write generating bytecode system for emulator, constructing a function pointing to the
+.json file for exception printing, and optimizing wherever possible
+
```

### Comparing `bytecodemanipulation-0.2.4/README.md` & `bytecodemanipulation-0.2.8/README.md`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,112 +1,112 @@
-# PyBytecodeManipulator
-A high level cross-version python bytecode manipulation library build ontop 
-of 'dis' and 'inspect' 
-
-Supports code inlining, branch removing and arbitrary code injection into 
-existing functions.
-
-WARNING: using bytecode manipulation on a so low level as we do can break 
-the python runtime at any point without a warning. We circumvent a lot of 
-safety checks normally done. 
-
-WARNING: We cannot make sure that everything works as it should, expect broken code 
-at runtime!
-
-
-Supported python versions:
-
-- 3.10 (main development)
-- 3.11.0[b3] (forward porting; WIP; Currently not working)
-
-Other versions will not work as a lot of config is stored in .json files per-version,
-so you may need to provide your own .json config files for the version you need.
-
-(Some versions might be plug-and-play, but most will require code changes additionally)
-
-## Why are there so many print()-s?
-
-Due to the breaking nature of anything this code touches, and the absents of any traces 
-in the function itself, we decided to add a lot of "debug" statements indicating 
-mostly the who-has-done-what-to-which-method for the runtime. 
-This makes debugging broken code easier, as it is more clear what happened to each transformed function.
-
-If you want them removed, create your own Fork of this and remove them, on your own risk.
-
-We may use in the future the logging library, so you can disable our logger instance, but we 
-are currently in an inter-stage of the code, so other stuff has priority.
-
-## Compatibility with other libraries 
-
-- Nuitka (https://github.com/Nuitka/Nuitka): Incompatible; will break as nuitka removes the \_\_code__ attribute 
-  we modify
-- Other bytecode modification / analysers: Should work as long as you as the user does NOT expose intermediate
-  results which might contain internal instructions
-
-
-## Debugging your injections 
-
-There is the possibility to "debug" functions using the execution emulator.
-It will be able to give you more information about a crash than the python core interpreter,
-but will be a lot slower than it. 
-
-It comes also with the possibility to run your bytecode in another interpreter version, so 
-you can experiment with some stuff.
-In theory, it is also possible to run in python versions not supported by the 
-bytecode manipulation system, but it is not recommended.
-
-TransformationHandler() takes as an arg debug_code and debug_further_calls
-for activating it for all accessed methods. 
-
-BytecodePatchHelper() contains a method enable_verbose_exceptions() for activating it on 
-that exact method.
-
-
-# Examples
-
-TODO
-
-
-# Applied Optimisations
-
-- Constant Expression inlining (can be declared for custom functions to be constant)
-- LOAD_GLOBAL for builtins (if enabled)
-- standard library inlining (if enabled)
-- specialization of methods based on arguments, e.g. constant arguments (when already resolved before, requires one of above options)
-- branch elimination when jumping on a constant (TODO: also if condition can be inferred ahead-of-time, see specialization)
-- local variable elimination
-
-
-# Currently Limitations
-
-- Line Numbers get mixed up, we need some way to assign meaningful line numbers
-- With python 3.11 (?), exception table exists, and this breaks our current concept of one big flow diagram,
-  as exception handling code might exist outside the default flow
-- During optimization, a lot of stuff is being recomputed each optimisation pass, we need to cache that drastically
-- Method inlining is not working properly and needs a lot more testing
-- If the exact type is known at optimisation time (e.g. object creation via class call, or type annotation), we can try to
-  inline method accesses for further optimisation
-- Python 3.12 will likely break how certain operations are stored in instructions, combing opcodes-without-args into a single
-  parent instruction, using the arg to switch between modes
-
-
-# Assembly Code
-
-- The library provides also a way to use some "python-assembly" for writing code
-- This is only python bytecode, so no fancy stuff can be done
-- See ASSEMBLY.md for more information on instructions
-- We provide an import system hook for importing .pyasm files via bytecodemanipulation.assembler.hook
-- You may use the functions from bytecodemanipulation.assembler.target for creating inline-assembly
-
-
-## Code Formatting
-
-We use the python formatting library "black" on our code
-
-# TODO's
-
-- abstract opcode affect away into a .json file describing all opcodes
-- create a json file for defining certain bytecode sequences
-- write more library-specific optimisations
-- write generating bytecode system for emulator, constructing a function pointing to the
-.json file for exception printing, and optimizing wherever possible
-
+# PyBytecodeManipulator
+A high level cross-version python bytecode manipulation library build ontop 
+of 'dis' and 'inspect' 
+
+Supports code inlining, branch removing and arbitrary code injection into 
+existing functions.
+
+WARNING: using bytecode manipulation on a so low level as we do can break 
+the python runtime at any point without a warning. We circumvent a lot of 
+safety checks normally done. 
+
+WARNING: We cannot make sure that everything works as it should, expect broken code 
+at runtime!
+
+
+Supported python versions:
+
+- 3.10 (main development)
+- 3.11.0[b3] (forward porting; WIP; Currently not working)
+
+Other versions will not work as a lot of config is stored in .json files per-version,
+so you may need to provide your own .json config files for the version you need.
+
+(Some versions might be plug-and-play, but most will require code changes additionally)
+
+## Why are there so many print()-s?
+
+Due to the breaking nature of anything this code touches, and the absents of any traces 
+in the function itself, we decided to add a lot of "debug" statements indicating 
+mostly the who-has-done-what-to-which-method for the runtime. 
+This makes debugging broken code easier, as it is more clear what happened to each transformed function.
+
+If you want them removed, create your own Fork of this and remove them, on your own risk.
+
+We may use in the future the logging library, so you can disable our logger instance, but we 
+are currently in an inter-stage of the code, so other stuff has priority.
+
+## Compatibility with other libraries 
+
+- Nuitka (https://github.com/Nuitka/Nuitka): Incompatible; will break as nuitka removes the \_\_code__ attribute 
+  we modify
+- Other bytecode modification / analysers: Should work as long as you as the user does NOT expose intermediate
+  results which might contain internal instructions
+
+
+## Debugging your injections 
+
+There is the possibility to "debug" functions using the execution emulator.
+It will be able to give you more information about a crash than the python core interpreter,
+but will be a lot slower than it. 
+
+It comes also with the possibility to run your bytecode in another interpreter version, so 
+you can experiment with some stuff.
+In theory, it is also possible to run in python versions not supported by the 
+bytecode manipulation system, but it is not recommended.
+
+TransformationHandler() takes as an arg debug_code and debug_further_calls
+for activating it for all accessed methods. 
+
+BytecodePatchHelper() contains a method enable_verbose_exceptions() for activating it on 
+that exact method.
+
+
+# Examples
+
+TODO
+
+
+# Applied Optimisations
+
+- Constant Expression inlining (can be declared for custom functions to be constant)
+- LOAD_GLOBAL for builtins (if enabled)
+- standard library inlining (if enabled)
+- specialization of methods based on arguments, e.g. constant arguments (when already resolved before, requires one of above options)
+- branch elimination when jumping on a constant (TODO: also if condition can be inferred ahead-of-time, see specialization)
+- local variable elimination
+
+
+# Currently Limitations
+
+- Line Numbers get mixed up, we need some way to assign meaningful line numbers
+- With python 3.11 (?), exception table exists, and this breaks our current concept of one big flow diagram,
+  as exception handling code might exist outside the default flow
+- During optimization, a lot of stuff is being recomputed each optimisation pass, we need to cache that drastically
+- Method inlining is not working properly and needs a lot more testing
+- If the exact type is known at optimisation time (e.g. object creation via class call, or type annotation), we can try to
+  inline method accesses for further optimisation
+- Python 3.12 will likely break how certain operations are stored in instructions, combing opcodes-without-args into a single
+  parent instruction, using the arg to switch between modes
+
+
+# Assembly Code
+
+- The library provides also a way to use some "python-assembly" for writing code
+- This is only python bytecode, so no fancy stuff can be done
+- See ASSEMBLY.md for more information on instructions
+- We provide an import system hook for importing .pyasm files via bytecodemanipulation.assembler.hook
+- You may use the functions from bytecodemanipulation.assembler.target for creating inline-assembly
+
+
+## Code Formatting
+
+We use the python formatting library "black" on our code
+
+# TODO's
+
+- abstract opcode affect away into a .json file describing all opcodes
+- create a json file for defining certain bytecode sequences
+- write more library-specific optimisations
+- write generating bytecode system for emulator, constructing a function pointing to the
+.json file for exception printing, and optimizing wherever possible
+
```

### Comparing `bytecodemanipulation-0.2.4/bytecodemanipulation/Mixin.py` & `bytecodemanipulation-0.2.8/bytecodemanipulation/Mixin.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,597 +1,597 @@
-import importlib
-import os
-import typing
-from abc import ABC
-
-from bytecodemanipulation import Emulator
-
-from bytecodemanipulation.mixin_util import resolve_accesses
-from bytecodemanipulation.MutableFunction import MutableFunction
-from bytecodemanipulation.MutableFunctionHelpers import insert_method_into
-from bytecodemanipulation.MutableFunctionHelpers import MutableFunctionWithTree
-from bytecodemanipulation.Optimiser import _OptimisationContainer
-from bytecodemanipulation.util import AbstractInstructionWalker
-from bytecodemanipulation.MutableFunction import Instruction
-from bytecodemanipulation.Opcodes import Opcodes
-
-
-class MixinInjectionNotSupportedException(Exception):
-    pass
-
-
-def _invoke_emulator(*args):
-    return Emulator.run_code(100, *args)
-
-
-class _MixinContainer:
-    class MixinFunctionContainer:
-        def __init__(self, target: typing.Callable):
-            self.target = target
-            self.mixins: typing.List[Mixin._MixinHandle] = []
-
-        def sort_and_apply(self):
-            # todo: sort
-
-            mutable = MutableFunction(self.target)
-            mutable.update_instruction_offsets(mutable.get_instructions())
-
-            for mixin in self.mixins:
-                mixin.apply_on(mutable)
-
-            try:
-                state = os.environ["DEBUG_MIXINS"]
-            except KeyError:
-                state = False
-
-            if state:
-                print("DEBUGGING MIXINS!")
-
-            if state:
-                target = MutableFunction(self.target)
-                override_target = MutableFunction(_invoke_emulator)
-                override_target.constants[
-                    override_target.constants.index(100)
-                ] = mutable
-                target.copy_from(override_target)
-                target.reassign_to_function()
-                target.target._debug_wrapper = mutable
-            else:
-                mutable.reassign_to_function()
-
-        def reset(self):
-            pass
-
-        def run_optimiser(self):
-            pass
-
-    @classmethod
-    def get_container_for_target(cls, target: typing.Type) -> "_MixinContainer":
-        if hasattr(target, "_MIXIN_CONTAINER"):
-            return getattr(target, "_MIXIN_CONTAINER")
-
-        container = _MixinContainer(target)
-        target._MIXIN_CONTAINER = container
-        return container
-
-    def __init__(self, target: typing.Type):
-        self.target = target
-        self.mixins: typing.List["Mixin"] = []
-        self.function_containers: typing.Dict[
-            str, _MixinContainer.MixinFunctionContainer
-        ] = {}
-
-    def sort_and_apply(self):
-        for mixin in self.function_containers.values():
-            mixin.sort_and_apply()
-
-    def reset(self):
-        for mixin in self.function_containers.values():
-            mixin.reset()
-
-    def run_optimiser(self):
-        # todo: copy optimisations over!
-        _OptimisationContainer.get_for_target(self.target).run_optimisers()
-
-
-class InjectionPosition:
-    class AbstractInjectionPosition(AbstractInstructionWalker, ABC):
-        def __init__(
-            self, parent: "InjectionPosition.AbstractInjectionPosition" = None
-        ):
-            self.parent = parent
-            self._positions: typing.List[Instruction] = []
-
-        def get_positions(self, root: Instruction) -> typing.List[Instruction]:
-            self._positions.clear()
-            self.init()
-            root.apply_visitor(self)
-            positions = self._positions.copy()
-            self._positions.clear()
-            return positions
-
-        def mark(self, instruction: Instruction):
-            self._positions.append(instruction)
-
-        @typing.final
-        def visit(self, instruction: Instruction) -> bool:
-            if self.parent is not None:
-                if not self.parent.visit(instruction):
-                    return False
-
-            return self.visit_instruction(instruction)
-
-        def init(self):
-            pass
-
-        def visit_instruction(self, instruction: Instruction) -> bool:
-            raise NotImplementedError
-
-    class _AtHeadInject(AbstractInjectionPosition):
-        def __init__(
-            self, parent: "InjectionPosition.AbstractInjectionPosition" = None
-        ):
-            super().__init__(parent=parent)
-            self.has_met_instr = False
-
-        def init(self):
-            self.has_met_instr = False
-
-        def visit_instruction(self, instruction: Instruction) -> bool:
-            if not self.has_met_instr:
-                self.mark(instruction)
-                self.has_met_instr = True
-                return True
-            return False
-
-    HEAD = _AtHeadInject()
-
-    class _AtFirstReturn(AbstractInjectionPosition):
-        def visit_instruction(self, instruction: Instruction) -> bool:
-            if instruction.opcode == Opcodes.RETURN_VALUE and not self._positions:
-                self.mark(instruction.previous_instructions[0])
-                return True
-            return False
-
-    FIRST_RETURN = _AtFirstReturn()
-
-    class _AtLastReturn(AbstractInjectionPosition):
-        def visit_instruction(self, instruction: Instruction) -> bool:
-            if instruction.opcode == Opcodes.RETURN_VALUE:
-                self._positions.clear()
-                self.mark(instruction.previous_instructions[0])
-                return True
-            return False
-
-    LAST_RETURN = _AtLastReturn()
-
-    class _AtReturn(AbstractInjectionPosition):
-        def visit_instruction(self, instruction: Instruction) -> bool:
-            if instruction.opcode == Opcodes.RETURN_VALUE:
-                self.mark(instruction.previous_instructions[0])
-                return True
-            return False
-
-    ALL_RETURN = _AtReturn()
-
-    class CountedRanges(AbstractInjectionPosition):
-        def __init__(
-            self,
-            start: int = None,
-            end: int = None,
-            parent: "InjectionPosition.AbstractInjectionPosition" = None,
-        ):
-            super().__init__(parent=parent)
-            self.ranges = []
-            self._counter = 0
-
-            if start is not None:
-                if end is not None:
-                    self.add_counted_range(start, end)
-                else:
-                    self.add_counted_range(start, -1)
-            elif end is not None:
-                self.add_counted_range(0, end)
-
-        def add_counted_range(self, start: int, end: int):
-            self.ranges.append((start, end))
-            return self
-
-        def init(self):
-            self.ranges.sort(key=lambda e: e[0])
-            self._counter = 0
-
-        def visit_instruction(self, instruction: Instruction) -> bool:
-            c = self._counter
-            self._counter += 1
-
-            for start, end in self.ranges:
-                if start <= c and (end == -1 or c <= end):
-                    self.mark(instruction)
-                    return True
-
-            return False
-
-
-def override(target_name: str, soft_override=False):
-    """
-    Overrides the target method
-
-    :param target_name: the function name
-    :param soft_override: if True, applies it only when no other mixin is applied, otherwise,
-        this may result in a crash when multiple are mixing into
-    """
-
-    def annotation(target):
-        _PREPARED_ANNOTATIONS.setdefault(target_name, []).append(
-            Mixin._OverrideHandle(MutableFunction(target))
-        )
-        return target
-
-    return annotation
-
-
-def inject_at(
-    target_name: str,
-    position: InjectionPosition.AbstractInjectionPosition,
-    deduplicate=False,
-    hard_deduplicate=False,
-):
-    """
-    Injects the target at the specified position
-
-    :param target_name: the function name
-    :param position: the position to inject at, might be 0 - inf
-    :param deduplicate: when True, tries to remove duplicated code segments by jumping around
-    :param hard_deduplicate: in version <= 3.10, it is possible to write small subroutines in bytecode via exception handling.
-        By setting this to True, this strategy is used. In versions >= 3.11, this is not supported and will be ignored
-    """
-
-    def annotation(target):
-        _PREPARED_ANNOTATIONS.setdefault(target_name, []).append(
-            Mixin._InjectAtHandle(position, MutableFunction(target))
-        )
-        return target
-
-    return annotation
-
-
-def exception_handle(
-    target_name: str,
-    exception_type: typing.Type[Exception],
-    start: InjectionPosition.AbstractInjectionPosition = None,
-    end: InjectionPosition.AbstractInjectionPosition = None,
-):
-    """
-    Adds a new exception handle, overriding the existing exception handles for the type in the region.
-
-    :param target_name: the function name
-    :param exception_type: the type of the exception to handle
-    :param start: where the exception handle starts, by default HEAD
-    :param end: where the exception handle ends, by default end of function
-    """
-
-    def annotation(target):
-        return target
-
-    return annotation
-
-
-def inject_by_known_call(
-    target_name: str,
-    invoke_target: typing.Callable,
-    checker: InjectionPosition.AbstractInjectionPosition,
-    replace=False,
-    before=False,
-    deduplicate=False,
-    hard_deduplicate=False,
-):
-    """
-    Injects the target at a function call, specified by exact function.
-
-    Parameters to the call might be accessed via resolve_prepared_parameter(<i>) where i is a constant, including slice.
-
-    Use override_function_call_result(<value>) to replace the result of the call when replace is False.
-
-    :param target_name: the function name
-    :param invoke_target: what function calls to inject at
-    :param checker: check function for each position
-    :param replace: if True, replaces the function call, otherwise, injects around
-    :param before: only affective if replace is False. If True, the target will be injected before the targeted call,
-        otherwise, behind, making the result arrival via resolve_prepared_parameter(-1)
-    :param deduplicate: when True, tries to remove duplicated code segments by jumping around
-    :param hard_deduplicate: in version <= 3.10, it is possible to write small subroutines in bytecode via exception handling.
-        By setting this to True, this strategy is used. In versions >= 3.11, this is not supported and will be ignored
-    """
-
-    def annotation(target):
-        return target
-
-    return annotation
-
-
-def inject_by_named_call(
-    target_name: str,
-    invoke_target: str,
-    checker: InjectionPosition.AbstractInjectionPosition,
-    replace=False,
-    before=False,
-    deduplicate=False,
-    hard_deduplicate=False,
-):
-    """
-    Injects the target at a function call, specified by exact function.
-
-    Parameters to the call might be accessed via resolve_prepared_parameter(<i>) where i is a constant, including slice.
-
-    Use override_function_call_result(<value>) to replace the result of the call when replace is False.
-
-    :param target_name: the function name
-    :param invoke_target: what function name calls to inject at
-    :param checker: check function for each position
-    :param replace: if True, replaces the function call, otherwise, injects around
-    :param before: only affective if replace is False. If True, the target will be injected before the targeted call,
-        otherwise, behind, making the result arrival via resolve_prepared_parameter(-1)
-    :param deduplicate: when True, tries to remove duplicated code segments by jumping around
-    :param hard_deduplicate: in version <= 3.10, it is possible to write small subroutines in bytecode via exception handling.
-        By setting this to True, this strategy is used. In versions >= 3.11, this is not supported and will be ignored
-    """
-
-    def annotation(target):
-        return target
-
-    return annotation
-
-
-def inject_by_named_call_on_known_type(
-    target_name: str,
-    obj_type: type,
-    invoke_target: str,
-    checker: InjectionPosition.AbstractInjectionPosition,
-    replace=False,
-    before=False,
-    deduplicate=False,
-    hard_deduplicate=False,
-):
-    """
-    Injects the target at a function call, specified by exact function.
-
-    Parameters to the call might be accessed via resolve_prepared_parameter(<i>) where i is a constant, including slice.
-
-    Use override_function_call_result(<value>) to replace the result of the call when replace is False.
-
-    :param target_name: the function name
-    :param obj_type: what type the object needs, can be None for static methods loaded from e.g. global namespace
-    :param invoke_target: what function name calls to inject at
-    :param checker: check function for each position
-    :param replace: if True, replaces the function call, otherwise, injects around
-    :param before: only affective if replace is False. If True, the target will be injected before the targeted call,
-        otherwise, behind, making the result arrival via resolve_prepared_parameter(-1)
-    :param deduplicate: when True, tries to remove duplicated code segments by jumping around
-    :param hard_deduplicate: in version <= 3.10, it is possible to write small subroutines in bytecode via exception handling.
-        By setting this to True, this strategy is used. In versions >= 3.11, this is not supported and will be ignored
-    """
-
-    def annotation(target):
-        return target
-
-    return annotation
-
-
-_PREPARED_ANNOTATIONS: typing.Dict[str, typing.List["Mixin._MixinHandle"]] = {}
-
-
-class Mixin:
-    """
-    Mixin class providing an abstract interface for bytecode manipulation
-
-    Example use:
-
-    class TestClass:
-        def test():
-            return 0
-
-    @Mixin(TestClass)
-    class TestClassMixin(Mixin.Interface):
-        @override("test")
-        def test():
-            return 1
-
-    The result of TestClass.test() will be without the mixin 0, with it 1
-    """
-
-    _INSTANCES: typing.List["Mixin"] = []
-
-    @classmethod
-    def _reset(cls):
-        cls._INSTANCES.clear()
-
-    @classmethod
-    def for_unbound_method(cls, target: typing.Callable) -> "Mixin":
-        raise NotImplementedError
-
-    class Interface:
-        """
-        @Mixin-annotated classes MUST implement this so the neat helper functions can be used
-        """
-
-        MIXIN_CONTAINER: _MixinContainer = None
-
-        @classmethod
-        def resolve_local(cls, name: str) -> object:
-            raise MixinInjectionNotSupportedException(
-                "Not implemented, should not happen!"
-            )
-
-        @classmethod
-        def resolve_exception_instance(cls) -> Exception:
-            raise MixinInjectionNotSupportedException("Not implemented!")
-
-        @classmethod
-        def resolve_prepared_parameter(cls, index: int) -> object:
-            raise MixinInjectionNotSupportedException("Not implemented!")
-
-        @classmethod
-        def resolve_cell_variable(cls, name: str) -> object:
-            raise MixinInjectionNotSupportedException(
-                "Not implemented, should not happen!"
-            )
-
-        @classmethod
-        def return_outer(cls, value=None):
-            raise MixinInjectionNotSupportedException("Not implemented!")
-
-        @classmethod
-        def jump_to(cls, position: InjectionPosition.AbstractInjectionPosition):
-            # todo: check that <position> only matches one position
-            raise MixinInjectionNotSupportedException("Not implemented!")
-
-        @classmethod
-        def jump_to_exception_handler(
-            cls, exception_type: Exception | typing.Type[Exception]
-        ):
-            raise MixinInjectionNotSupportedException("Not implemented!")
-
-        @classmethod
-        def override_function_call_result(cls, result: object):
-            raise MixinInjectionNotSupportedException("Not implemented!")
-
-    class _MixinHandle:
-        def apply_on(self, mutable: MutableFunction):
-            raise NotImplementedError
-
-    class _OverrideHandle(_MixinHandle):
-        def __init__(self, override_with: MutableFunction):
-            self.override_with = override_with
-
-        def apply_on(self, mutable: MutableFunction):
-            resolve_accesses(mutable, self.override_with)
-
-            mutable.copy_from(self.override_with)
-
-    class _InjectAtHandle(_MixinHandle):
-        def __init__(
-            self,
-            at: InjectionPosition.AbstractInjectionPosition,
-            inject: MutableFunction,
-        ):
-            self.at = at
-            self.inject = inject
-
-        def apply_on(self, mutable: MutableFunction):
-            protected_locals = resolve_accesses(mutable, self.inject)
-
-            if self.inject.shared_variable_names[0] in ("cls", "self"):
-                protected_locals.append(self.inject.shared_variable_names[0])
-
-            tree = MutableFunctionWithTree(mutable)
-
-            for position_instr in self.at.get_positions(mutable.instructions[0])[:]:
-                if position_instr not in mutable.instructions:
-                    continue
-
-                insert_method_into(
-                    tree,
-                    position_instr.offset - 1,
-                    self.inject,
-                    protected_locals=protected_locals,
-                )
-
-                mutable.assemble_instructions_from_tree(tree.root)
-
-    def __init__(
-        self,
-        target_class: str | typing.Type | typing.Callable[[], typing.Type],
-        priority=0,
-        optional=False,
-        apply_on_others=True,
-    ):
-        if not callable(target_class) and not isinstance(target_class, str):
-            raise ValueError(
-                f"'target_class' must be str (for resolving), class or lazy class, got {type(target_class)}"
-            )
-
-        self.__target_class = target_class
-        self.__resolved = False
-        self.__mixin_class: typing.Optional[typing.Type[Mixin.Interface]] = None
-        self.__mixin_container: typing.Optional[_MixinContainer] = None
-        self.__priority = priority
-        self.__optional = optional
-        self.__apply_on_others = apply_on_others
-        self.__prepared_data = {}
-
-        Mixin._INSTANCES.append(self)
-
-    def __call__(self, cls: typing.Type):
-        if self.__mixin_class is not None:
-            raise ValueError("Can only annotate one class with one Mixin-instance!")
-
-        if not issubclass(cls, Mixin.Interface):
-            raise ValueError(
-                "@Mixin-annotated classes must implement the Mixin.Interface!"
-            )
-
-        self.__mixin_class = cls
-        self.__prepared_data.update(_PREPARED_ANNOTATIONS)
-        _PREPARED_ANNOTATIONS.clear()
-        return self
-
-    def _resolve(self) -> bool:
-        self.__resolved = True
-
-        if isinstance(self.__target_class, str):
-            if ":" not in self.__target_class:
-                self.__target_class = importlib.import_module(self.__target_class)
-                return True
-
-            module, path = self.__target_class.split(":")
-            module = importlib.import_module(module)
-
-            for e in path.split("."):
-                module = getattr(module, e)
-
-            self.__target_class = module
-            return True
-
-        try:
-            issubclass(self.__target_class, Mixin.Interface)
-        except TypeError:
-            pass
-        else:
-            return True
-
-        self.__target_class = self.__target_class()
-        return True
-
-    def _bind_to_target(self):
-        if not self.__resolved:
-            raise RuntimeError("_resolve() must be called before _bind_to_target()")
-
-        self.__mixin_container = (
-            container
-        ) = (
-            self.__mixin_class.MIXIN_CONTAINER
-        ) = _MixinContainer.get_container_for_target(self.__target_class)
-        container.mixins.append(self)
-
-        for key, value in self.__prepared_data.items():
-            if not isinstance(key, str):
-                key = key.__name__
-
-            if key not in self.__mixin_container.function_containers:
-                cont = self.__mixin_container.MixinFunctionContainer(
-                    getattr(self.__target_class, key)
-                )
-                self.__mixin_container.function_containers[key] = cont
-            else:
-                cont = self.__mixin_container.function_containers[key]
-
-            cont.mixins += value
-
-    def _apply(self):
-        if not self.__resolved:
-            self._resolve()
-
-        if self.__mixin_container is None:
-            self._bind_to_target()
-
-        self.__mixin_container.sort_and_apply()
+import importlib
+import os
+import typing
+from abc import ABC
+
+from bytecodemanipulation import Emulator
+
+from bytecodemanipulation.mixin_util import resolve_accesses
+from bytecodemanipulation.MutableFunction import MutableFunction
+from bytecodemanipulation.MutableFunctionHelpers import insert_method_into
+from bytecodemanipulation.MutableFunctionHelpers import MutableFunctionWithTree
+from bytecodemanipulation.Optimiser import _OptimisationContainer
+from bytecodemanipulation.util import AbstractInstructionWalker
+from bytecodemanipulation.MutableFunction import Instruction
+from bytecodemanipulation.Opcodes import Opcodes
+
+
+class MixinInjectionNotSupportedException(Exception):
+    pass
+
+
+def _invoke_emulator(*args):
+    return Emulator.run_code(100, *args)
+
+
+class _MixinContainer:
+    class MixinFunctionContainer:
+        def __init__(self, target: typing.Callable):
+            self.target = target
+            self.mixins: typing.List[Mixin._MixinHandle] = []
+
+        def sort_and_apply(self):
+            # todo: sort
+
+            mutable = MutableFunction(self.target)
+            mutable.update_instruction_offsets(mutable.get_instructions())
+
+            for mixin in self.mixins:
+                mixin.apply_on(mutable)
+
+            try:
+                state = os.environ["DEBUG_MIXINS"]
+            except KeyError:
+                state = False
+
+            if state:
+                print("DEBUGGING MIXINS!")
+
+            if state:
+                target = MutableFunction(self.target)
+                override_target = MutableFunction(_invoke_emulator)
+                override_target.constants[
+                    override_target.constants.index(100)
+                ] = mutable
+                target.copy_from(override_target)
+                target.reassign_to_function()
+                target.target._debug_wrapper = mutable
+            else:
+                mutable.reassign_to_function()
+
+        def reset(self):
+            pass
+
+        def run_optimiser(self):
+            pass
+
+    @classmethod
+    def get_container_for_target(cls, target: typing.Type) -> "_MixinContainer":
+        if hasattr(target, "_MIXIN_CONTAINER"):
+            return getattr(target, "_MIXIN_CONTAINER")
+
+        container = _MixinContainer(target)
+        target._MIXIN_CONTAINER = container
+        return container
+
+    def __init__(self, target: typing.Type):
+        self.target = target
+        self.mixins: typing.List["Mixin"] = []
+        self.function_containers: typing.Dict[
+            str, _MixinContainer.MixinFunctionContainer
+        ] = {}
+
+    def sort_and_apply(self):
+        for mixin in self.function_containers.values():
+            mixin.sort_and_apply()
+
+    def reset(self):
+        for mixin in self.function_containers.values():
+            mixin.reset()
+
+    def run_optimiser(self):
+        # todo: copy optimisations over!
+        _OptimisationContainer.get_for_target(self.target).run_optimisers()
+
+
+class InjectionPosition:
+    class AbstractInjectionPosition(AbstractInstructionWalker, ABC):
+        def __init__(
+            self, parent: "InjectionPosition.AbstractInjectionPosition" = None
+        ):
+            self.parent = parent
+            self._positions: typing.List[Instruction] = []
+
+        def get_positions(self, root: Instruction) -> typing.List[Instruction]:
+            self._positions.clear()
+            self.init()
+            root.apply_visitor(self)
+            positions = self._positions.copy()
+            self._positions.clear()
+            return positions
+
+        def mark(self, instruction: Instruction):
+            self._positions.append(instruction)
+
+        @typing.final
+        def visit(self, instruction: Instruction) -> bool:
+            if self.parent is not None:
+                if not self.parent.visit(instruction):
+                    return False
+
+            return self.visit_instruction(instruction)
+
+        def init(self):
+            pass
+
+        def visit_instruction(self, instruction: Instruction) -> bool:
+            raise NotImplementedError
+
+    class _AtHeadInject(AbstractInjectionPosition):
+        def __init__(
+            self, parent: "InjectionPosition.AbstractInjectionPosition" = None
+        ):
+            super().__init__(parent=parent)
+            self.has_met_instr = False
+
+        def init(self):
+            self.has_met_instr = False
+
+        def visit_instruction(self, instruction: Instruction) -> bool:
+            if not self.has_met_instr:
+                self.mark(instruction)
+                self.has_met_instr = True
+                return True
+            return False
+
+    HEAD = _AtHeadInject()
+
+    class _AtFirstReturn(AbstractInjectionPosition):
+        def visit_instruction(self, instruction: Instruction) -> bool:
+            if instruction.opcode == Opcodes.RETURN_VALUE and not self._positions:
+                self.mark(instruction.previous_instructions[0])
+                return True
+            return False
+
+    FIRST_RETURN = _AtFirstReturn()
+
+    class _AtLastReturn(AbstractInjectionPosition):
+        def visit_instruction(self, instruction: Instruction) -> bool:
+            if instruction.opcode == Opcodes.RETURN_VALUE:
+                self._positions.clear()
+                self.mark(instruction.previous_instructions[0])
+                return True
+            return False
+
+    LAST_RETURN = _AtLastReturn()
+
+    class _AtReturn(AbstractInjectionPosition):
+        def visit_instruction(self, instruction: Instruction) -> bool:
+            if instruction.opcode == Opcodes.RETURN_VALUE:
+                self.mark(instruction.previous_instructions[0])
+                return True
+            return False
+
+    ALL_RETURN = _AtReturn()
+
+    class CountedRanges(AbstractInjectionPosition):
+        def __init__(
+            self,
+            start: int = None,
+            end: int = None,
+            parent: "InjectionPosition.AbstractInjectionPosition" = None,
+        ):
+            super().__init__(parent=parent)
+            self.ranges = []
+            self._counter = 0
+
+            if start is not None:
+                if end is not None:
+                    self.add_counted_range(start, end)
+                else:
+                    self.add_counted_range(start, -1)
+            elif end is not None:
+                self.add_counted_range(0, end)
+
+        def add_counted_range(self, start: int, end: int):
+            self.ranges.append((start, end))
+            return self
+
+        def init(self):
+            self.ranges.sort(key=lambda e: e[0])
+            self._counter = 0
+
+        def visit_instruction(self, instruction: Instruction) -> bool:
+            c = self._counter
+            self._counter += 1
+
+            for start, end in self.ranges:
+                if start <= c and (end == -1 or c <= end):
+                    self.mark(instruction)
+                    return True
+
+            return False
+
+
+def override(target_name: str, soft_override=False):
+    """
+    Overrides the target method
+
+    :param target_name: the function name
+    :param soft_override: if True, applies it only when no other mixin is applied, otherwise,
+        this may result in a crash when multiple are mixing into
+    """
+
+    def annotation(target):
+        _PREPARED_ANNOTATIONS.setdefault(target_name, []).append(
+            Mixin._OverrideHandle(MutableFunction(target))
+        )
+        return target
+
+    return annotation
+
+
+def inject_at(
+    target_name: str,
+    position: InjectionPosition.AbstractInjectionPosition,
+    deduplicate=False,
+    hard_deduplicate=False,
+):
+    """
+    Injects the target at the specified position
+
+    :param target_name: the function name
+    :param position: the position to inject at, might be 0 - inf
+    :param deduplicate: when True, tries to remove duplicated code segments by jumping around
+    :param hard_deduplicate: in version <= 3.10, it is possible to write small subroutines in bytecode via exception handling.
+        By setting this to True, this strategy is used. In versions >= 3.11, this is not supported and will be ignored
+    """
+
+    def annotation(target):
+        _PREPARED_ANNOTATIONS.setdefault(target_name, []).append(
+            Mixin._InjectAtHandle(position, MutableFunction(target))
+        )
+        return target
+
+    return annotation
+
+
+def exception_handle(
+    target_name: str,
+    exception_type: typing.Type[Exception],
+    start: InjectionPosition.AbstractInjectionPosition = None,
+    end: InjectionPosition.AbstractInjectionPosition = None,
+):
+    """
+    Adds a new exception handle, overriding the existing exception handles for the type in the region.
+
+    :param target_name: the function name
+    :param exception_type: the type of the exception to handle
+    :param start: where the exception handle starts, by default HEAD
+    :param end: where the exception handle ends, by default end of function
+    """
+
+    def annotation(target):
+        return target
+
+    return annotation
+
+
+def inject_by_known_call(
+    target_name: str,
+    invoke_target: typing.Callable,
+    checker: InjectionPosition.AbstractInjectionPosition,
+    replace=False,
+    before=False,
+    deduplicate=False,
+    hard_deduplicate=False,
+):
+    """
+    Injects the target at a function call, specified by exact function.
+
+    Parameters to the call might be accessed via resolve_prepared_parameter(<i>) where i is a constant, including slice.
+
+    Use override_function_call_result(<value>) to replace the result of the call when replace is False.
+
+    :param target_name: the function name
+    :param invoke_target: what function calls to inject at
+    :param checker: check function for each position
+    :param replace: if True, replaces the function call, otherwise, injects around
+    :param before: only affective if replace is False. If True, the target will be injected before the targeted call,
+        otherwise, behind, making the result arrival via resolve_prepared_parameter(-1)
+    :param deduplicate: when True, tries to remove duplicated code segments by jumping around
+    :param hard_deduplicate: in version <= 3.10, it is possible to write small subroutines in bytecode via exception handling.
+        By setting this to True, this strategy is used. In versions >= 3.11, this is not supported and will be ignored
+    """
+
+    def annotation(target):
+        return target
+
+    return annotation
+
+
+def inject_by_named_call(
+    target_name: str,
+    invoke_target: str,
+    checker: InjectionPosition.AbstractInjectionPosition,
+    replace=False,
+    before=False,
+    deduplicate=False,
+    hard_deduplicate=False,
+):
+    """
+    Injects the target at a function call, specified by exact function.
+
+    Parameters to the call might be accessed via resolve_prepared_parameter(<i>) where i is a constant, including slice.
+
+    Use override_function_call_result(<value>) to replace the result of the call when replace is False.
+
+    :param target_name: the function name
+    :param invoke_target: what function name calls to inject at
+    :param checker: check function for each position
+    :param replace: if True, replaces the function call, otherwise, injects around
+    :param before: only affective if replace is False. If True, the target will be injected before the targeted call,
+        otherwise, behind, making the result arrival via resolve_prepared_parameter(-1)
+    :param deduplicate: when True, tries to remove duplicated code segments by jumping around
+    :param hard_deduplicate: in version <= 3.10, it is possible to write small subroutines in bytecode via exception handling.
+        By setting this to True, this strategy is used. In versions >= 3.11, this is not supported and will be ignored
+    """
+
+    def annotation(target):
+        return target
+
+    return annotation
+
+
+def inject_by_named_call_on_known_type(
+    target_name: str,
+    obj_type: type,
+    invoke_target: str,
+    checker: InjectionPosition.AbstractInjectionPosition,
+    replace=False,
+    before=False,
+    deduplicate=False,
+    hard_deduplicate=False,
+):
+    """
+    Injects the target at a function call, specified by exact function.
+
+    Parameters to the call might be accessed via resolve_prepared_parameter(<i>) where i is a constant, including slice.
+
+    Use override_function_call_result(<value>) to replace the result of the call when replace is False.
+
+    :param target_name: the function name
+    :param obj_type: what type the object needs, can be None for static methods loaded from e.g. global namespace
+    :param invoke_target: what function name calls to inject at
+    :param checker: check function for each position
+    :param replace: if True, replaces the function call, otherwise, injects around
+    :param before: only affective if replace is False. If True, the target will be injected before the targeted call,
+        otherwise, behind, making the result arrival via resolve_prepared_parameter(-1)
+    :param deduplicate: when True, tries to remove duplicated code segments by jumping around
+    :param hard_deduplicate: in version <= 3.10, it is possible to write small subroutines in bytecode via exception handling.
+        By setting this to True, this strategy is used. In versions >= 3.11, this is not supported and will be ignored
+    """
+
+    def annotation(target):
+        return target
+
+    return annotation
+
+
+_PREPARED_ANNOTATIONS: typing.Dict[str, typing.List["Mixin._MixinHandle"]] = {}
+
+
+class Mixin:
+    """
+    Mixin class providing an abstract interface for bytecode manipulation
+
+    Example use:
+
+    class TestClass:
+        def test():
+            return 0
+
+    @Mixin(TestClass)
+    class TestClassMixin(Mixin.Interface):
+        @override("test")
+        def test():
+            return 1
+
+    The result of TestClass.test() will be without the mixin 0, with it 1
+    """
+
+    _INSTANCES: typing.List["Mixin"] = []
+
+    @classmethod
+    def _reset(cls):
+        cls._INSTANCES.clear()
+
+    @classmethod
+    def for_unbound_method(cls, target: typing.Callable) -> "Mixin":
+        raise NotImplementedError
+
+    class Interface:
+        """
+        @Mixin-annotated classes MUST implement this so the neat helper functions can be used
+        """
+
+        MIXIN_CONTAINER: _MixinContainer = None
+
+        @classmethod
+        def resolve_local(cls, name: str) -> object:
+            raise MixinInjectionNotSupportedException(
+                "Not implemented, should not happen!"
+            )
+
+        @classmethod
+        def resolve_exception_instance(cls) -> Exception:
+            raise MixinInjectionNotSupportedException("Not implemented!")
+
+        @classmethod
+        def resolve_prepared_parameter(cls, index: int) -> object:
+            raise MixinInjectionNotSupportedException("Not implemented!")
+
+        @classmethod
+        def resolve_cell_variable(cls, name: str) -> object:
+            raise MixinInjectionNotSupportedException(
+                "Not implemented, should not happen!"
+            )
+
+        @classmethod
+        def return_outer(cls, value=None):
+            raise MixinInjectionNotSupportedException("Not implemented!")
+
+        @classmethod
+        def jump_to(cls, position: InjectionPosition.AbstractInjectionPosition):
+            # todo: check that <position> only matches one position
+            raise MixinInjectionNotSupportedException("Not implemented!")
+
+        @classmethod
+        def jump_to_exception_handler(
+            cls, exception_type: Exception | typing.Type[Exception]
+        ):
+            raise MixinInjectionNotSupportedException("Not implemented!")
+
+        @classmethod
+        def override_function_call_result(cls, result: object):
+            raise MixinInjectionNotSupportedException("Not implemented!")
+
+    class _MixinHandle:
+        def apply_on(self, mutable: MutableFunction):
+            raise NotImplementedError
+
+    class _OverrideHandle(_MixinHandle):
+        def __init__(self, override_with: MutableFunction):
+            self.override_with = override_with
+
+        def apply_on(self, mutable: MutableFunction):
+            resolve_accesses(mutable, self.override_with)
+
+            mutable.copy_from(self.override_with)
+
+    class _InjectAtHandle(_MixinHandle):
+        def __init__(
+            self,
+            at: InjectionPosition.AbstractInjectionPosition,
+            inject: MutableFunction,
+        ):
+            self.at = at
+            self.inject = inject
+
+        def apply_on(self, mutable: MutableFunction):
+            protected_locals = resolve_accesses(mutable, self.inject)
+
+            if self.inject.shared_variable_names[0] in ("cls", "self"):
+                protected_locals.append(self.inject.shared_variable_names[0])
+
+            tree = MutableFunctionWithTree(mutable)
+
+            for position_instr in self.at.get_positions(mutable.instructions[0])[:]:
+                if position_instr not in mutable.instructions:
+                    continue
+
+                insert_method_into(
+                    tree,
+                    position_instr.offset - 1,
+                    self.inject,
+                    protected_locals=protected_locals,
+                )
+
+                mutable.assemble_instructions_from_tree(tree.root)
+
+    def __init__(
+        self,
+        target_class: str | typing.Type | typing.Callable[[], typing.Type],
+        priority=0,
+        optional=False,
+        apply_on_others=True,
+    ):
+        if not callable(target_class) and not isinstance(target_class, str):
+            raise ValueError(
+                f"'target_class' must be str (for resolving), class or lazy class, got {type(target_class)}"
+            )
+
+        self.__target_class = target_class
+        self.__resolved = False
+        self.__mixin_class: typing.Optional[typing.Type[Mixin.Interface]] = None
+        self.__mixin_container: typing.Optional[_MixinContainer] = None
+        self.__priority = priority
+        self.__optional = optional
+        self.__apply_on_others = apply_on_others
+        self.__prepared_data = {}
+
+        Mixin._INSTANCES.append(self)
+
+    def __call__(self, cls: typing.Type):
+        if self.__mixin_class is not None:
+            raise ValueError("Can only annotate one class with one Mixin-instance!")
+
+        if not issubclass(cls, Mixin.Interface):
+            raise ValueError(
+                "@Mixin-annotated classes must implement the Mixin.Interface!"
+            )
+
+        self.__mixin_class = cls
+        self.__prepared_data.update(_PREPARED_ANNOTATIONS)
+        _PREPARED_ANNOTATIONS.clear()
+        return self
+
+    def _resolve(self) -> bool:
+        self.__resolved = True
+
+        if isinstance(self.__target_class, str):
+            if ":" not in self.__target_class:
+                self.__target_class = importlib.import_module(self.__target_class)
+                return True
+
+            module, path = self.__target_class.split(":")
+            module = importlib.import_module(module)
+
+            for e in path.split("."):
+                module = getattr(module, e)
+
+            self.__target_class = module
+            return True
+
+        try:
+            issubclass(self.__target_class, Mixin.Interface)
+        except TypeError:
+            pass
+        else:
+            return True
+
+        self.__target_class = self.__target_class()
+        return True
+
+    def _bind_to_target(self):
+        if not self.__resolved:
+            raise RuntimeError("_resolve() must be called before _bind_to_target()")
+
+        self.__mixin_container = (
+            container
+        ) = (
+            self.__mixin_class.MIXIN_CONTAINER
+        ) = _MixinContainer.get_container_for_target(self.__target_class)
+        container.mixins.append(self)
+
+        for key, value in self.__prepared_data.items():
+            if not isinstance(key, str):
+                key = key.__name__
+
+            if key not in self.__mixin_container.function_containers:
+                cont = self.__mixin_container.MixinFunctionContainer(
+                    getattr(self.__target_class, key)
+                )
+                self.__mixin_container.function_containers[key] = cont
+            else:
+                cont = self.__mixin_container.function_containers[key]
+
+            cont.mixins += value
+
+    def _apply(self):
+        if not self.__resolved:
+            self._resolve()
+
+        if self.__mixin_container is None:
+            self._bind_to_target()
+
+        self.__mixin_container.sort_and_apply()
```

### Comparing `bytecodemanipulation-0.2.4/bytecodemanipulation/MutableFunction.py` & `bytecodemanipulation-0.2.8/bytecodemanipulation/MutableFunction.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,1509 +1,1604 @@
-import copy
-import dis
-import sys
-import types
-import typing
-import simplejson
-
-import bytecodemanipulation.assembler.util.tokenizer
-from bytecodemanipulation.Opcodes import HAS_CELL_VARIABLE
-from bytecodemanipulation.Opcodes import HAS_JUMP_BACKWARDS
-from bytecodemanipulation.Opcodes import (
-    Opcodes,
-    END_CONTROL_FLOW,
-    OPCODE2NAME,
-    OPNAME2CODE,
-    HAS_NAME,
-    HAS_CONST,
-    HAS_LOCAL,
-    HAS_JUMP_ABSOLUTE,
-    HAS_JUMP_FORWARD,
-    UNCONDITIONAL_JUMPS,
-)
-import bytecodemanipulation.data_loader
-from bytecodemanipulation.util import AbstractInstructionWalker
-
-
-class LinearCodeConstraintViolationException(Exception):
-    pass
-
-
-class Instruction:
-    @classmethod
-    def _pair_instruction(cls, opcode: int | str) -> typing.Tuple[int, str]:
-        if isinstance(opcode, int):
-            return opcode, OPCODE2NAME[opcode]
-
-        return OPNAME2CODE[opcode], opcode
-
-    __slots__ = (
-        "function",
-        "offset",
-        "opcode",
-        "opname",
-        "arg_value",
-        "arg",
-        "_next_instruction",
-        "previous_instructions",
-        "source_location",
-    )
-
-    @classmethod
-    def create(cls, *args, **kwargs):
-        return cls(None, -1, *args, **kwargs)
-
-    @classmethod
-    def create_with_token(
-        cls,
-        token: bytecodemanipulation.assembler.util.tokenizer.AbstractToken,
-        function: typing.Optional["MutableFunction"],
-        offset: int | None,
-        opcode_or_name: int | str,
-        arg_value: object = None,
-        arg: int = None,
-        _decode_next=True,
-    ) -> "Instruction":
-        raise NotImplementedError("not bound!")
-
-    def __init__(
-        self,
-        function: typing.Optional["MutableFunction"],
-        offset: int | None,
-        opcode_or_name: int | str,
-        arg_value: object = None,
-        arg: int = None,
-        _decode_next=True,
-        pos_info=None,
-    ):
-        self.function = function
-        self.offset = offset
-        self.opcode, self.opname = self._pair_instruction(opcode_or_name)
-        self.arg_value = arg_value
-        self.arg = arg
-        self.source_location = pos_info
-
-        if (
-            self.arg is not None
-            and self.arg_value is None
-            and (_decode_next or not self.has_jump())
-        ):
-            self.change_arg(self.arg)
-        elif (
-            self.arg_value is not None or self.opcode == Opcodes.LOAD_CONST
-        ) and self.arg is None:
-            self.change_arg_value(self.arg_value)
-
-        # Reference to the next instruction
-        # Will raise an exception if changed and not using assemble_instructions_from_tree()
-        self._next_instruction: typing.Optional[Instruction] = (
-            None
-            if function is None
-            or offset is None
-            or self.opcode in END_CONTROL_FLOW
-            or not _decode_next
-            else function.instructions[offset + 1]
-        )
-
-        self.previous_instructions: typing.List["Instruction"] | None = None
-
-    def copy(self, owner: "MutableFunction" = None) -> "Instruction":
-        instance = type(self)(
-            self.function,
-            self.offset,
-            self.opcode,
-            self.arg_value if self.arg_value is not None or self.opcode == Opcodes.LOAD_CONST else self.arg,
-        )
-
-        if owner:
-            instance.update_owner(owner, -1, force_change_arg_index=True)
-
-        return instance
-
-    def apply_visitor(
-        self,
-        visitor: AbstractInstructionWalker,
-        visited: typing.Set["Instruction"] = None,
-    ):
-        if visited is None:
-            visited = set()
-
-        if self in visited:
-            return
-
-        visited.add(self)
-
-        visitor.visit(self)
-
-        if self.has_stop_flow():
-            return
-
-        if self.next_instruction is not None and self.next_instruction != self:
-            self.next_instruction.apply_visitor(visitor, visited)
-
-        if self.has_jump() and isinstance(self.arg_value, Instruction):
-            typing.cast(Instruction, self.arg_value).apply_visitor(visitor, visited)
-
-    def apply_value_visitor(
-        self,
-        callback: typing.Callable[
-            ["Instruction", typing.Any | None, typing.Any | None], typing.Any
-        ],
-        visited: typing.Dict["Instruction", typing.Any] = None,
-    ) -> typing.Any:
-        if visited is None:
-            visited = {}
-
-        elif self in visited:
-            return visited[self]
-
-        visited[self] = None
-
-        if self.has_stop_flow():
-            return callback(self, None, None)
-
-        if self.has_jump() and isinstance(self.arg_value, Instruction):
-            return callback(
-                self,
-                self.next_instruction.apply_value_visitor(callback, visited),
-                self.arg_value.apply_value_visitor(callback, visited),
-            )
-
-        if self.next_instruction is not None:
-            return callback(
-                self, self.next_instruction.apply_value_visitor(callback, visited), None
-            )
-
-        return callback(self, None, None)
-
-    def add_previous_instruction(self, instruction: "Instruction"):
-        if self.previous_instructions is None:
-            self.previous_instructions = [instruction]
-        elif instruction not in self.previous_instructions:
-            self.previous_instructions.append(instruction)
-
-    def remove_previous_instruction(self, instruction: "Instruction"):
-        if (
-            self.previous_instructions is not None
-            and instruction in self.previous_instructions
-        ):
-            self.previous_instructions.remove(instruction)
-
-    def get_previous_instructions(self) -> typing.List["Instruction"]:
-        if self.has_stop_flow():
-            return []
-
-        if self.previous_instructions is None:
-            if self.function is None:
-                raise ValueError(
-                    f"Instruction {self} is not bound to a MutableFunction object, making retrieving the previous instruction list impossible!!"
-                )
-
-            self.function.prepare_previous_instructions()
-
-            if self.previous_instructions is None:
-                raise RuntimeError(
-                    f"Could not find previous instructions for {self}. This should NOT happen, as we asked the method which MUST yield results. (See MutableFunction.prepare_previous_instructions())"
-                )
-
-        return self.previous_instructions
-
-    def set_next_instruction(self, instruction: typing.Optional["Instruction"]):
-        if self._next_instruction is not None:
-            self._next_instruction.remove_previous_instruction(self)
-
-        self._next_instruction = instruction
-
-        if instruction is not None:
-            instruction.add_previous_instruction(self)
-
-    def get_next_instruction(self) -> typing.Optional["Instruction"]:
-        return self._next_instruction
-
-    next_instruction = property(get_next_instruction, set_next_instruction)
-
-    def __repr__(self):
-        assert self.function is None or isinstance(self.function.function_name, str)
-        assert isinstance(self.offset, int)
-        assert isinstance(self.opcode, int)
-        assert isinstance(self.arg, int) or self.arg is None
-        if id(self) == id(self.arg_value):
-            return self.repr_safe() + "@self_arg_value"
-
-        return f"Instruction(function={self.function.function_name if self.function else '{Not Bound}'}, position={self.offset}, opcode={self.opcode}, opname={self.opname}, arg={self.arg}, arg_value={self.arg_value.repr_safe() if self.arg_value is not None and isinstance(self.arg_value, Instruction) else self.arg_value}, has_next={self.next_instruction is not None})"
-
-    def repr_safe(self):
-        return f"Instruction(function={self.function.function_name if self.function else '{Not Bound}'}, position={self.offset}, opcode={self.opcode}, opname={self.opname}, arg={self.arg}, arg_value=..., has_next={self.next_instruction is not None})"
-
-    def __eq__(self, other):
-        if not isinstance(other, Instruction):
-            return False
-
-        return (
-            self.opcode == other.opcode
-            and (
-                self.offset == other.offset
-                or self.offset is None
-                or other.offset is None
-            )
-            and (
-                (self.arg_value == other.arg_value)
-                if not isinstance(self.arg_value, Instruction)
-                else (id(self.arg_value) == id(other.arg_value))
-                if self.arg_value is not None and other.arg_value is not None
-                else True
-            )
-        )
-
-    def lossy_eq(self, other: "Instruction") -> bool:
-        if not isinstance(other, Instruction):
-            return False
-
-        return self.opcode == other.opcode and (
-            (
-                (self.arg_value == other.arg_value)
-                if not isinstance(self.arg_value, Instruction)
-                else self.arg_value.lossy_eq(other.arg_value)
-            )
-            if (self.arg_value is not None and other.arg_value is not None)
-            or self.opcode == Opcodes.LOAD_CONST
-            else True
-        )
-
-    def __hash__(self):
-        return id(self)
-
-    def get_arg(self):
-        return 0 if self.arg is None else self.arg
-
-    def change_opcode(self, opcode: int | str, arg_value=None):
-        self.opcode, self.opname = self._pair_instruction(opcode)
-        # todo: what happens with the arg?
-
-        self.next_instruction = (
-            None
-            if self.function is None
-            or self.offset is None
-            or self.opcode in END_CONTROL_FLOW
-            or self.offset == -1
-            else self.function.instructions[self.offset + 1]
-        )
-
-        if self.opcode < dis.HAVE_ARGUMENT:
-            self.arg = 0
-            self.arg_value = None
-
-        if arg_value:
-            self.change_arg_value(arg_value)
-
-        return self
-
-    def change_arg_value(self, value: object):
-        self.arg_value = value
-
-        if self.function is not None:
-            if self.opcode in HAS_NAME:
-                assert isinstance(value, str)
-                self.arg = self.function.allocate_shared_name(value)
-            elif self.opcode in HAS_CELL_VARIABLE:
-                assert isinstance(value, str)
-                self.arg = self.function.allocate_shared_cell(value)
-            elif self.opcode in HAS_CONST:
-                self.arg = self.function.allocate_shared_constant(value)
-            elif self.opcode in HAS_LOCAL:
-                assert isinstance(value, str), (value, self.opname)
-                self.arg = self.function.allocate_shared_variable_name(value)
-            elif self.opcode in HAS_JUMP_ABSOLUTE:
-                if isinstance(value, Instruction):
-                    self.arg = value.offset
-            elif self.opcode == Opcodes.FOR_ITER:
-                assert isinstance(value, Instruction), value
-                self.arg = value.offset - self.offset
-            elif self.opcode in HAS_JUMP_FORWARD:
-                assert isinstance(value, Instruction), value
-                self.arg = value.offset - self.offset
-        else:
-            self.arg = None
-
-    def change_arg(self, arg: int):
-        self.arg = arg
-
-        if self.function is not None:
-            try:
-                flag = False
-                if sys.version_info.minor >= 11:
-                    if self.opcode == Opcodes.LOAD_GLOBAL:
-                        self.arg_value = self.function.shared_names[arg >> 1]
-                        flag = True
-
-                if flag:
-                    pass
-                elif self.opcode in HAS_NAME:
-                    self.arg_value = self.function.shared_names[arg]
-                elif self.opcode in HAS_CELL_VARIABLE:
-                    self.arg_value = self.function.cell_variables[arg]
-                elif self.opcode in HAS_CONST:
-                    self.arg_value = self.function.constants[arg]
-                elif self.opcode in HAS_LOCAL:
-                    self.arg_value = self.function.shared_variable_names[arg]
-                elif self.opcode in HAS_JUMP_ABSOLUTE:
-                    self.arg_value = self.function.instructions[arg]
-                elif self.opcode in (Opcodes.FOR_ITER, Opcodes.SETUP_FINALLY):
-                    self.arg_value = self.function.instructions[arg + self.offset]
-                elif self.opcode in HAS_JUMP_FORWARD and self.offset is not None:
-                    self.arg_value = self.function.instructions[arg + self.offset]
-            except:
-                print(
-                    self.opname,
-                    arg,
-                    self.function.shared_names,
-                    self.function.constants,
-                    self.function.shared_variable_names,
-                )
-                raise
-        else:
-            self.arg_value = None
-
-    def has_name(self):
-        return self.opcode in HAS_NAME
-
-    def has_constant(self):
-        return self.opcode in HAS_CONST
-
-    def has_local(self):
-        return self.opcode in HAS_LOCAL
-
-    def has_jump_absolute(self):
-        return self.opcode in HAS_JUMP_ABSOLUTE
-
-    def has_jump_forward(self):
-        return self.opcode in HAS_JUMP_FORWARD
-
-    def has_jump_backward(self):
-        return self.opcode in HAS_JUMP_BACKWARDS
-
-    def has_cell_variable(self):
-        return self.opcode in HAS_CELL_VARIABLE
-
-    def has_jump(self):
-        return (
-            self.has_jump_absolute()
-            or self.has_jump_forward()
-            or self.has_jump_backward()
-        )
-
-    def has_unconditional_jump(self):
-        return self.opcode in UNCONDITIONAL_JUMPS
-
-    def has_stop_flow(self):
-        return self.opcode in END_CONTROL_FLOW
-
-    def update_owner(
-        self,
-        function: "MutableFunction",
-        offset: int,
-        update_following=True,
-        force_change_arg_index=False,
-    ):
-        previous_function = self.function
-
-        self.function = function
-        self.offset = offset
-
-        # If previously the ownership was unset, and we have not fully referenced args, do it now!
-        # todo: when previous owner was set, and arg is not None, we might need to de-ref the value
-        #    and re-ref afterwards, so the value lives in the new owner
-        if (
-            self.arg is not None
-            and self.arg_value is None
-            and (not force_change_arg_index or self.opcode != Opcodes.LOAD_CONST)
-        ):
-            self.change_arg(self.arg)
-        elif (self.arg_value is not None or self.opcode == Opcodes.LOAD_CONST) and (
-            self.arg is None or force_change_arg_index
-        ):
-            self.change_arg_value(self.arg_value)
-
-        if update_following:
-            self.next_instruction = (
-                (None if previous_function != function else self.next_instruction)
-                if function is None
-                or offset is None
-                or self.opcode in END_CONTROL_FLOW
-                or offset == -1
-                or offset + 1 >= len(function.instructions)
-                else function.instructions[offset + 1]
-            )
-
-        return self
-
-    def optimise_tree(self, visited: typing.Set["Instruction"] = None) -> "Instruction":
-        """
-        Optimises the instruction tree, removing NOP's and inlining unconditional jumps
-        WARNING: this WILL invalidate the linearity of any instruction list, you MUST use assemble_instructions_from_tree()
-        for inserting it back into the Function.
-
-        Requires next_instruction's to be set, meaning it must be owned at some point by a function
-        """
-
-        if self.has_unconditional_jump():
-            return self.arg_value.optimise_tree(visited)
-
-        if visited is None:
-            visited = set()
-
-        if self in visited:
-            return self
-
-        visited.add(self)
-
-        if self.opcode == Opcodes.NOP and self.next_instruction is not None:
-            return self.next_instruction.optimise_tree(visited)
-
-        while self.next_instruction is not None:
-            assert isinstance(self.next_instruction, Instruction)
-
-            if self.next_instruction.opname == "NOP":
-                self.next_instruction = self.next_instruction.next_instruction
-                continue
-
-            if self.next_instruction.opname in ("JUMP_ABSOLUTE", "JUMP_FORWARD"):
-                self.next_instruction = self.next_instruction.arg_value
-                continue
-
-            break
-
-        if (
-            self.next_instruction is not None
-            and not self.has_stop_flow()
-            and not self.has_unconditional_jump()
-        ):
-            self.next_instruction = self.next_instruction.optimise_tree(visited)
-
-        if (
-            self.has_jump_absolute()
-            or self.has_jump_forward()
-            or self.has_jump_backward()
-        ) and self.arg_value is not None:
-            assert isinstance(self.arg_value, Instruction)
-            self.change_arg_value(self.arg_value.optimise_tree(visited))
-
-        return self
-
-    def trace_variable_set(
-        self, name: str, visited: typing.Set[str] = None
-    ) -> typing.Iterator["Instruction"]:
-        if visited and self in visited:
-            return
-
-        if self.opcode == Opcodes.STORE_FAST and self.arg_value == name:
-            yield self
-            return
-
-        if self.opcode == Opcodes.DELETE_FAST:
-            return
-
-        if visited is None:
-            visited = {self}
-
-        if self.previous_instructions is None:
-            return
-
-        for prev in self.previous_instructions:
-            yield from prev.trace_variable_set(name, visited)
-
-    def trace_stack_position(
-        self, stack_position: int
-    ) -> typing.Iterator["Instruction"]:
-        for instr in self.get_priorities_previous():
-            yield from instr._trace_stack_position(stack_position, set(), self)
-
-    def get_priorities_previous(self) -> typing.List["Instruction"]:
-        if not self.previous_instructions:
-            return []
-
-        real_previous = [
-            instr
-            for instr in self.previous_instructions
-            if instr.next_instruction == self
-        ]
-        unreal_previous = [
-            instr
-            for instr in self.previous_instructions
-            if instr.next_instruction != self
-        ]
-        highest = None
-
-        for e in real_previous:
-            if e.offset == self.offset - 1 or e.opcode == Opcodes.SETUP_FINALLY:
-                highest = e
-
-        if not highest:
-            return real_previous + unreal_previous
-
-        return [highest] + [e for e in real_previous if e != highest] + unreal_previous
-
-    def trace_normalized_stack_position(
-        self, stack_position: int
-    ) -> typing.Optional["Instruction"]:
-        target = next(self.trace_stack_position(stack_position))
-
-        if target.opcode == Opcodes.DUP_TOP:
-            return target.trace_normalized_stack_position(0)
-
-        if target.opcode == Opcodes.LOAD_FAST:
-            try:
-                variable_set = next(
-                    target.trace_variable_set(typing.cast(str, target.arg_value))
-                )
-            except StopIteration:
-                return target
-
-            return variable_set.trace_normalized_stack_position(0)
-
-        return target
-
-    def _trace_stack_position(
-        self,
-        stack_position: int,
-        yielded: typing.Set["Instruction"],
-        previous_instr: "Instruction" = None,
-    ) -> typing.Iterator["Instruction"]:
-        assert stack_position >= 0
-
-        if self in yielded:
-            return
-
-        if self.has_unconditional_jump():
-            pushed, popped, additional_pos = 0, 0, None
-        elif self.opcode == Opcodes.SETUP_FINALLY and previous_instr == self.arg_value:
-            pushed, popped, additional_pos = 3, 0, None
-        elif self.opcode in (
-            Opcodes.JUMP_IF_TRUE_OR_POP,
-            Opcodes.JUMP_IF_FALSE_OR_POP,
-        ):
-            if self.arg_value == previous_instr:
-                pushed, popped, additional_pos = 0, 0, None
-            else:
-                pushed, popped, additional_pos = 0, 1, None
-        else:
-            pushed, popped, additional_pos = self.get_stack_affect()
-
-        # print(self, stack_position, (pushed, popped, additional_pos), self.arg_value, previous_instr)
-
-        if pushed > stack_position:
-            yielded.add(self)
-            # print("hit")
-            yield self
-            # print("cont")
-
-            if additional_pos:
-                for instr in self.get_priorities_previous():
-                    yield from instr._trace_stack_position(
-                        additional_pos, yielded, self
-                    )
-
-            return
-
-        stack_position -= pushed
-        stack_position += popped
-
-        yielded.add(self)
-
-        for instr in self.get_priorities_previous():
-            try:
-                yield from instr._trace_stack_position(stack_position, yielded, self)
-            except:
-                # print(self, instr)
-                raise
-
-        if additional_pos:
-            for instr in self.get_priorities_previous():
-                yield from instr._trace_stack_position(additional_pos, yielded, self)
-
-    def trace_stack_position_use(
-        self, stack_position: int
-    ) -> typing.Iterator["Instruction"]:
-        # print(self, 0)
-
-        if not self.has_stop_flow():
-            yield from self.next_instruction._trace_stack_position_use(
-                stack_position, set()
-            )
-
-        if self.has_jump():
-            yield from typing.cast(
-                Instruction, self.arg_value
-            )._trace_stack_position_use(stack_position, set())
-
-    def _trace_stack_position_use(
-        self, stack_position: int, yielded: typing.Set["Instruction"]
-    ) -> typing.Iterator["Instruction"]:
-        assert stack_position >= 0
-
-        if self in yielded:
-            return
-
-        yielded.add(self)
-
-        pushed, popped, additional_pos = self.get_stack_affect()
-
-        if popped > stack_position:
-            yielded.add(self)
-            yield self
-
-            if additional_pos:
-                yield from self.next_instruction._trace_stack_position_use(
-                    additional_pos, yielded
-                )
-
-            return
-
-        stack_position -= popped
-        stack_position += pushed
-
-        if not self.has_stop_flow():
-            yield from self.next_instruction._trace_stack_position_use(
-                stack_position, yielded
-            )
-
-        if self.has_jump():
-            yield from typing.cast(
-                Instruction, self.arg_value
-            )._trace_stack_position_use(stack_position, yielded)
-
-        if additional_pos:
-            yield from self.next_instruction._trace_stack_position_use(
-                additional_pos, yielded
-            )
-
-    def get_stack_affect(self) -> typing.Tuple[int, int, int | None]:
-        # pushed, popped, additional
-        if self.opcode in (
-            Opcodes.NOP,
-            Opcodes.POP_BLOCK,
-            Opcodes.POP_EXCEPT,
-            Opcodes.SETUP_FINALLY,
-            Opcodes.GEN_START,
-            Opcodes.JUMP_ABSOLUTE,
-            Opcodes.BYTECODE_LABEL,
-            Opcodes.CACHE,
-            Opcodes.PRECALL,
-            Opcodes.RESUME,
-        ):
-            return 0, 0, None
-
-        if self.opcode == Opcodes.DUP_TOP:
-            return 2, 1, None
-
-        if self.opcode in (Opcodes.GET_ITER, Opcodes.FOR_ITER):
-            return 1, 0, None
-
-        if self.opcode in (
-            Opcodes.LOAD_CONST,
-            Opcodes.LOAD_GLOBAL,
-            Opcodes.LOAD_FAST,
-            Opcodes.LOAD_DEREF,
-            Opcodes.LOAD_CLOSURE,
-            Opcodes.LOAD_BUILD_CLASS,
-        ):
-            return 1, 0, None
-
-        if self.opcode in (
-            Opcodes.BUILD_TUPLE,
-            Opcodes.BUILD_LIST,
-            Opcodes.BUILD_SET,
-            Opcodes.BUILD_SLICE,
-            Opcodes.BUILD_STRING,
-        ):
-            return 1, self.arg, None
-
-        if self.opcode in (Opcodes.ROT_TWO,):
-            return 2, 2, None
-
-        if self.opcode in (Opcodes.FORMAT_VALUE,):
-            return 1, (2 if (self.arg & 0x04) == 0x04 else 1), None
-
-        if self.opcode in (
-            Opcodes.CALL_FUNCTION,
-            Opcodes.CALL_METHOD,
-            Opcodes.CALL_FUNCTION_KW,
-            Opcodes.CALL,
-        ):
-            return 1, self.arg + 1, None
-
-        if self.opcode in (Opcodes.CALL_FUNCTION_EX,):
-            count = 2
-
-            if self.arg & 0x01:
-                count += 1
-
-            return 1, count, None
-
-        if self.opcode == Opcodes.BUILD_MAP:
-            return 1, self.arg * 2, None
-
-        if self.opcode in (
-            Opcodes.COMPARE_OP,
-            Opcodes.IS_OP,
-            Opcodes.BINARY_SUBSCR,
-            Opcodes.CONTAINS_OP,
-            Opcodes.LIST_EXTEND,
-            Opcodes.LIST_APPEND,
-            Opcodes.SET_ADD,
-            Opcodes.SET_UPDATE,
-            Opcodes.DICT_UPDATE,
-            Opcodes.DICT_MERGE,
-            Opcodes.BINARY_FLOOR_DIVIDE,
-            Opcodes.BINARY_ADD,
-            Opcodes.BINARY_SUBTRACT,
-            Opcodes.BINARY_MULTIPLY,
-            Opcodes.BINARY_TRUE_DIVIDE,
-            Opcodes.BINARY_FLOOR_DIVIDE,
-            Opcodes.BINARY_MODULO,
-            Opcodes.BINARY_XOR,
-            Opcodes.BINARY_AND,
-            Opcodes.BINARY_OR,
-            Opcodes.BINARY_POWER,
-            Opcodes.INPLACE_SUBTRACT,
-            Opcodes.IMPORT_NAME,
-            Opcodes.YIELD_FROM,
-        ):
-            return 1, 2, None
-
-        if self.opcode in (
-            Opcodes.LOAD_ATTR,
-            Opcodes.LOAD_METHOD,
-            Opcodes.GET_AWAITABLE,
-            Opcodes.LIST_TO_TUPLE,
-            Opcodes.IMPORT_FROM,
-            Opcodes.UNARY_NEGATIVE,
-            Opcodes.YIELD_VALUE,
-            Opcodes.GET_YIELD_FROM_ITER,
-            Opcodes.UNARY_NOT,
-            Opcodes.UNARY_NEGATIVE,
-            Opcodes.UNARY_INVERT,
-            Opcodes.UNARY_POSITIVE,
-            Opcodes.STATIC_ATTRIBUTE_ACCESS,
-        ):
-            return 1, 1, None
-
-        if self.opcode in (Opcodes.STORE_ATTR,):
-            return 2, 0, None
-
-        if self.opcode in (
-            Opcodes.POP_TOP,
-            Opcodes.POP_JUMP_IF_TRUE,
-            Opcodes.POP_JUMP_IF_FALSE,
-            Opcodes.STORE_FAST,
-            Opcodes.STORE_NAME,
-            Opcodes.STORE_DEREF,
-            Opcodes.STORE_GLOBAL,
-            Opcodes.RETURN_VALUE,
-        ):
-            return 0, 1, None
-
-        if self.opcode == Opcodes.UNPACK_SEQUENCE:
-            return self.arg, 1, None
-
-        if self.opcode == Opcodes.JUMP_IF_NOT_EXC_MATCH:
-            return 0, 2, None
-
-        if self.opcode == Opcodes.MAKE_FUNCTION:
-            return 1, 2 + self.arg.bit_count(), None
-
-        if self.opcode == Opcodes.RAISE_VARARGS:
-            return 0, self.arg, None
-
-        if self.opcode == Opcodes.DUP_TOP_TWO:
-            return 2, 4, None
-
-        raise RuntimeError(self)
-
-    def insert_after(self, *instructions: "Instruction" | typing.List["Instruction"]):
-        if not instructions:
-            return self
-
-        if isinstance(instructions[0], (list, tuple)):
-            if len(instructions) > 1:
-                raise ValueError
-
-            instructions = instructions[0]
-
-        if len(instructions) == 0:
-            return self
-
-        instructions[0].next_instruction = self.next_instruction
-        self.next_instruction = instructions[0]
-
-        if len(instructions) > 1:
-            instructions[0].insert_after(instructions[1:])
-
-        return self
-
-
-class MutableFunction:
-    @classmethod
-    def create(cls, target):
-        if isinstance(target, staticmethod):
-            return cls(target.__func__)
-        elif isinstance(target, classmethod):
-            return cls(target.__func__)
-        return cls(target)
-
-    def __init__(self, target: types.FunctionType | types.MethodType):
-        self.target = target
-
-        self.code_object: types.CodeType = target.__code__
-
-        self._load_from_code_object(self.code_object)
-
-    if sys.version_info.major == 3 and sys.version_info.minor == 10:
-
-        def _load_from_code_object(self, obj: types.CodeType):
-            self.argument_count = self.code_object.co_argcount
-            self.cell_variables = list(self.code_object.co_cellvars)
-            self.__raw_code = bytearray(self.code_object.co_code)
-            self.constants = list(self.code_object.co_consts)
-            self.filename = self.code_object.co_filename
-            self.first_line_number = self.code_object.co_firstlineno
-            self.code_flags = self.code_object.co_flags
-            self.free_variables = list(self.code_object.co_freevars)
-            self.keyword_only_argument_count = self.code_object.co_kwonlyargcount
-            self.line_table = self.code_object.co_linetable
-            self.lnotab = bytearray(self.code_object.co_lnotab)
-
-            self.function_name = self.code_object.co_name
-            self.shared_names = list(self.code_object.co_names)
-            # Local variable count is implied by co_varnames
-            self.positional_only_argument_count = self.code_object.co_posonlyargcount
-            self.stack_size = self.code_object.co_stacksize
-            self.shared_variable_names = list(self.code_object.co_varnames)
-
-            self.__instructions: typing.Optional[typing.List[Instruction]] = None
-
-    elif sys.version_info.major == 3 and sys.version_info.minor == 11:
-
-        def _load_from_code_object(self, obj: types.CodeType):
-            self.argument_count = self.code_object.co_argcount
-            self.cell_variables = list(self.code_object.co_cellvars)
-            self.__raw_code = bytearray(self.code_object.co_code)
-            self.constants = list(self.code_object.co_consts)
-            self.filename = self.code_object.co_filename
-            self.first_line_number = self.code_object.co_firstlineno
-            self.code_flags = self.code_object.co_flags
-            self.free_variables = list(self.code_object.co_freevars)
-            self.keyword_only_argument_count = self.code_object.co_kwonlyargcount
-            self.line_table = self.code_object.co_linetable
-            self.lnotab = bytearray(self.code_object.co_lnotab)
-
-            self.function_name = self.code_object.co_name
-            self.shared_names = list(self.code_object.co_names)
-            # Local variable count is implied by co_varnames
-            self.positional_only_argument_count = self.code_object.co_posonlyargcount
-            self.stack_size = self.code_object.co_stacksize
-            self.shared_variable_names = list(self.code_object.co_varnames)
-
-            self.exception_table = bytearray(self.code_object.co_exceptiontable)
-
-            self.__instructions: typing.Optional[typing.List[Instruction]] = None
-
-    else:
-        raise RuntimeError(sys.version_info)
-
-    def __repr__(self):
-        return f"MutableFunction({self.target})"
-
-    def copy(self):
-        def _():
-            pass
-
-        instance = type(self)(_)
-        instance.copy_from(self)
-
-        return instance
-
-    def copy_from(self, mutable: "MutableFunction"):
-        # self.target = mutable.target
-        self.code_object = mutable.code_object
-
-        self.argument_count = mutable.argument_count
-        self.cell_variables = mutable.cell_variables.copy()
-        self.__raw_code = mutable.raw_code.copy()
-        self.constants = copy.deepcopy(mutable.constants)
-        self.filename = mutable.filename
-        self.first_line_number = mutable.first_line_number
-        self.code_flags = mutable.code_flags
-        self.free_variables = mutable.free_variables.copy()
-        self.keyword_only_argument_count = mutable.keyword_only_argument_count
-        self.line_table = copy.copy(mutable.line_table)
-        self.lnotab = mutable.lnotab
-        self.function_name = mutable.function_name
-        self.shared_names = mutable.shared_names.copy()
-        self.positional_only_argument_count = mutable.positional_only_argument_count
-        self.stack_size = mutable.stack_size
-        self.shared_variable_names = mutable.shared_variable_names.copy()
-
-        self.__instructions = None
-
-    if sys.version_info.major == 3 and sys.version_info.minor == 10:
-
-        def create_code_obj(self) -> types.CodeType:
-            if self.__instructions is None:
-                self.get_instructions()
-
-            self.assemble_fast(self.__instructions)
-
-            return types.CodeType(
-                self.argument_count,
-                self.positional_only_argument_count,
-                self.keyword_only_argument_count,
-                len(self.shared_variable_names),
-                self.stack_size,
-                self.code_flags,
-                bytes(self.raw_code),
-                tuple(self.constants),
-                tuple(self.shared_names),
-                tuple(self.shared_variable_names),
-                self.filename,
-                self.function_name,
-                self.first_line_number,
-                self.get_lnotab(),
-                tuple(self.free_variables),
-                tuple(self.cell_variables),
-            )
-
-    elif sys.version_info.major == 3 and sys.version_info.minor == 11:
-
-        def create_code_obj(self) -> types.CodeType:
-            if self.__instructions is None:
-                self.get_instructions()
-
-            self.assemble_fast(self.__instructions)
-
-            return types.CodeType(
-                self.argument_count,
-                self.positional_only_argument_count,
-                self.keyword_only_argument_count,
-                len(self.shared_variable_names),
-                self.stack_size,
-                self.code_flags,
-                bytes(self.raw_code),
-                tuple(self.constants),
-                tuple(self.shared_names),
-                tuple(self.shared_variable_names),
-                self.filename,
-                self.function_name,
-                self.function_name,
-                self.first_line_number,
-                self.get_lnotab(),
-                bytes(self.exception_table),
-                tuple(self.free_variables),
-                tuple(self.cell_variables),
-            )
-
-    def get_lnotab(self) -> bytes:
-        items = []
-
-        prev_line = self.first_line_number
-        count_since_previous = 0
-
-        for instr in self.__instructions:
-            count_since_previous += 1
-
-            if instr.source_location is None or instr.source_location[0] == prev_line:
-                continue
-
-            offset = instr.source_location[0] - prev_line
-
-            if offset > 127:
-                return bytes()
-
-            if offset < 0:
-                return bytes()
-
-            items.append(count_since_previous)
-            items.append(offset)
-            count_since_previous = 0
-
-        return bytes(items)
-
-    def reassign_to_function(self):
-        self.target.__code__ = self.create_code_obj()
-
-    def decode_instructions(self):
-        if self.__instructions is not None:
-            self.__instructions.clear()
-        else:
-            self.__instructions = []
-
-        line = self.first_line_number
-        lnotab = list(self.lnotab)
-
-        extra: int = 0
-        for i in range(0, len(self.__raw_code), 2):
-            opcode, arg = self.__raw_code[i : i + 2]
-
-            if opcode == Opcodes.EXTENDED_ARG:
-                extra = extra * 256 + arg
-                instr = Instruction(self, i // 2, "NOP", _decode_next=False)
-
-            else:
-                arg += extra * 256
-                extra = 0
-
-                if opcode in (Opcodes.FOR_ITER, Opcodes.SETUP_FINALLY):
-                    arg += 1
-
-                instr = Instruction(self, i // 2, opcode, arg=arg, _decode_next=False)
-
-            if lnotab:
-                lnotab[0] -= 1
-
-                if lnotab[0] == 0:
-                    line_incr = lnotab[1]
-                    del lnotab[:2]
-
-                    line += line_incr
-
-            instr.source_location = (line, None, None)
-
-            self.__instructions.append(instr)
-            # print(instr, instr.source_location)
-
-        for i, instruction in enumerate(self.instructions):
-            instruction.update_owner(self, i)
-
-        self.prepare_previous_instructions()
-
-    def prepare_previous_instructions(self):
-        for instruction in self.instructions:
-            if instruction.previous_instructions:
-                instruction.previous_instructions.clear()
-
-        for instruction in self.instructions:
-            if instruction.has_stop_flow() or instruction.has_unconditional_jump():
-                continue
-
-            instruction.next_instruction.add_previous_instruction(instruction)
-
-            if instruction.has_jump():
-                # print(instruction.arg_value, typing.cast, typing.cast(Instruction, instruction.arg_value))
-
-                typing.cast(
-                    Instruction, instruction.arg_value
-                ).add_previous_instruction(instruction)
-
-    def assemble_instructions_from_tree(self, root: Instruction, breaks_flow=tuple()):
-        # 1. Assemble a linear stream of instructions, containing all instructions
-        # 2. check instructions which require unconditional JUMP's and insert them
-        # 3. update instruction positions
-        # 4. Update the arg value of jumps
-        # 5. Walk over all instructions and set extended arg count + insert NOP's, and recheck if instructions need more extended
-        # 6. Resolve jump target into real values
-        # 7. Profit! (Maybe use assemble_fast() here!
-
-        instructions = self.assemble_linear_instructions(breaks_flow, root)
-
-        self.update_instruction_offsets(instructions)
-
-        self.insert_needed_jumps(instructions)
-
-        self.update_instruction_offsets(instructions)
-
-        self.update_jump_args(instructions)
-        required_extends = self.get_required_arg_extensions(instructions)
-        self.insert_required_nops(instructions, required_extends)
-        self.update_jump_args(instructions)
-
-        # Check how many EXTENDED_ARG we really need
-        required_extends_2 = self.get_required_arg_extensions(instructions)
-
-        if required_extends != required_extends_2:
-            # todo: here, walk again over the instruction list
-            raise NotImplementedError
-
-        # For a last time, walk over the instructions and tie them together
-        for i, instruction in enumerate(instructions[:]):
-            if (
-                not instruction.has_stop_flow()
-                and not instruction.has_unconditional_jump()
-            ):
-                try:
-                    instruction.next_instruction = instructions[i + 1]
-                except IndexError:
-                    instruction.next_instruction = None
-                except:
-                    print(instruction)
-                    print(instruction.next_instruction)
-                    raise
-
-        self.assemble_fast(instructions)
-        self.update_instruction_offsets(self.instructions)
-        # We do not re-decode, as that would invalidate the instruction instances here
-
-    def update_instruction_offsets(self, instructions):
-        # Update instruction positions
-        for i, instruction in enumerate(instructions):
-            instruction.offset = i
-
-    def insert_required_nops(self, instructions, required_extends):
-        write_offset = 0
-        # Now insert the required NOP's
-        for instruction, count in zip(instructions[:], required_extends):
-            if count == 0:
-                continue
-
-            for _ in range(count):
-                pos = instruction.offset + write_offset
-                instructions.insert(
-                    pos, nop_instr := Instruction.create(self, pos, "NOP")
-                )
-
-            write_offset += count
-
-    def get_required_arg_extensions(self, instructions):
-        # Check how many EXTENDED_ARG we need
-        required_extends = [0] * len(instructions)
-        for i, instruction in enumerate(instructions):
-            arg = instruction.arg
-
-            if arg is None:
-                if instruction.opcode < dis.HAVE_ARGUMENT:
-                    arg = 0
-                else:
-                    print("error", instruction)
-
-            if arg >= 256**3:
-                count = 3
-            elif arg >= 256**2:
-                count = 2
-            elif arg >= 256:
-                count = 1
-            else:
-                count = 0
-            required_extends[i] = count
-        return required_extends
-
-    def update_jump_args(self, instructions):
-        # Update the raw arg for jumps
-        for i, instruction in enumerate(instructions):
-            if instruction.next_instruction is None:
-                continue
-
-            instruction.update_owner(self, i)
-
-            if instruction.has_jump_absolute():
-                instruction.change_arg_value(instruction.arg_value)
-            elif instruction.offset in (Opcodes.FOR_ITER, Opcodes.SETUP_FINALLY):
-                instruction.change_arg_value(instruction.arg_value)
-            elif instruction.has_jump_forward():
-                instruction.change_arg_value(instruction.arg_value)
-            elif instruction.has_jump_backward():
-                instruction.change_arg_value(instruction.arg_value)
-
-    def insert_needed_jumps(self, instructions):
-        # Check for unconditional jumps required
-        for instruction in instructions[:]:
-            if instruction.has_stop_flow():
-                continue
-
-            # FOR_ITER can only jump FORWARD, so insert a new jump absolute to jump there
-            # TODO: insert the JUMP somewhere else than here!
-            if instruction.opcode == Opcodes.FOR_ITER:
-                jump = Instruction(
-                    self,
-                    -1,
-                    "JUMP_ABSOLUTE",
-                    instruction.next_instruction,
-                )
-                jump.change_arg_value(instruction.arg_value)
-                instruction.change_arg_value(jump)
-                instructions.append(jump)
-
-            if (
-                instruction.next_instruction is not None
-                and instruction.offset + 1 != instruction.next_instruction.offset
-            ):
-                jump = Instruction(
-                    self,
-                    -1,
-                    "JUMP_ABSOLUTE",
-                    instruction.next_instruction,
-                )
-                jump.next_instruction = instruction
-                instruction.next_instruction = jump
-                instructions.insert(instructions.index(instruction) + 1, jump)
-
-    def assemble_linear_instructions(self, breaks_flow, root):
-
-        # While we have branches, we need to decode them
-        pending_instructions = [root]
-        visited: typing.Set[Instruction] = set()
-        instructions: typing.List[Instruction] = []
-
-        while pending_instructions:
-            instruction = pending_instructions.pop()
-
-            if not isinstance(instruction, Instruction):
-                print(f"Invalid task instruction: {instruction}")
-                continue
-
-            if not isinstance(instruction, Instruction):
-                raise ValueError(instruction)
-
-            # If we visited it, we can skip
-            if instruction in visited:
-                continue
-
-            # Walk over the instructions as long as we have not met them
-            while instruction not in visited:
-                if not isinstance(instruction, Instruction):
-                    print(f"Invalid task instruction: {instruction}")
-                    break
-
-                # If it branches off, it needs to be visited later on
-                if instruction.has_jump():
-                    if instruction.arg_value is None:
-                        instruction.update_owner(self, instruction.offset)
-
-                    assert instruction.arg_value is not None, instruction
-
-                    pending_instructions.append(instruction.arg_value)
-
-                instructions.append(instruction)
-                visited.add(instruction)
-
-                if (
-                    instruction.has_stop_flow()
-                    or instruction in breaks_flow
-                    or instruction.opcode in breaks_flow
-                ):
-                    break
-
-                if instruction.next_instruction is None:
-                    instruction.update_owner(self, instruction.offset)
-
-                # The next instruction MUST be set if it does NOT end the control flow
-                if instruction.next_instruction is None:
-                    print("---- start dump")
-                    for instr in instructions:
-                        print(instr)
-                    print("---- end dump")
-                    raise RuntimeError(f"next instruction is None: {instruction}")
-
-                instruction = instruction.next_instruction
-
-        return instructions
-
-    def assemble_instructions(self):
-
-        # Check for linearity violations
-        for i, instruction in enumerate(self.__instructions):
-            if (
-                instruction.next_instruction is not None
-                and instruction.offset + 1 != instruction.next_instruction.offset
-                and not instruction.has_unconditional_jump()
-                and not instruction.has_stop_flow()
-            ):
-                # todo: do we want to dynamic use assemble_instructions_from_tree()?
-                raise LinearCodeConstraintViolationException(
-                    f"Failed between instruction {instruction} and {instruction.next_instruction}, use assemble_instructions_from_tree(...) to assemble from an non-normal tree"
-                )
-
-        needs_tree_assemble = False
-        root = self.__instructions[0]
-        previous = None
-
-        # Check if the NOP's ahead of instructions are enough to hold the extra args
-        nop_count = 0
-        for i, instruction in enumerate(self.__instructions):
-            if instruction.opname == "NOP":
-                nop_count += 1
-                previous = instruction
-                continue
-
-            if instruction.arg is not None:
-                if instruction.arg >= 256**3:
-                    count = 3
-                elif instruction.arg >= 256**2:
-                    count = 2
-                elif instruction.arg >= 256:
-                    count = 1
-                else:
-                    count = 0
-
-                # Are there NOP's missing for the needed EXTENDED_ARG?
-                if count > nop_count:
-                    # todo: move this code up into assemble_instructions_from_tree()
-
-                    missing = count - nop_count  # how many we need
-                    needs_tree_assemble = True  # make sure that we use the assemble_instructions_from_tree() now
-
-                    # If we are at HEAD, we require some clever handling, as "previous" is None at the moment
-                    if i == 0:
-                        root = previous = Instruction(
-                            self,
-                            0,
-                            "NOP",
-                        )
-                        root.next_instruction = instruction
-                        missing -= 1
-
-                    previous.insert_after(
-                        [
-                            Instruction(self, previous.offset + i + 1, Opcodes.NOP)
-                            for i in range(missing)
-                        ]
-                    )
-
-                nop_count = 0
-
-            previous = instruction
-
-        if needs_tree_assemble:
-            self.assemble_instructions_from_tree(root)
-            return
-
-        # We are now sure that we have enough space for all data, so we can assemble the EXTENDED_ARG instructions
-        # duplicate of assemble_fast() with less safety checks, as we checked that stuff beforehand
-        self.__raw_code.clear()
-        for i, instruction in enumerate(self.__instructions):
-            arg = instruction.get_arg()
-
-            if instruction.opcode in (Opcodes.FOR_ITER, Opcodes.SETUP_FINALLY):
-                arg -= 1
-
-            if arg > 255:
-                extend = arg // 256
-                arg %= 256
-
-                offset = 1
-                while extend > 0:
-                    iarg = extend % 256
-                    extend //= 256
-
-                    self.__raw_code[(i - offset) * 2 : (i - offset + 1) * 2] = bytes(
-                        [Opcodes.EXTENDED_ARG, iarg]
-                    )
-                    offset += 1
-
-            self.__raw_code += bytes([instruction.opcode, arg])
-
-    def assemble_fast(self, instructions: typing.List[Instruction]):
-        """
-        Assembles the instruction list in FAST mode
-        Removes some safety checks, and removes the dynamic assemble_instructions_from_tree() forwarding.
-        Requires the linking of instructions to be LINEAR.
-
-        :raises ValueError: if not enough space for EXTENDED_ARG's is available
-        """
-
-        self.__instructions = [
-            instruction.update_owner(self, i, update_following=False)
-            for i, instruction in enumerate(instructions)
-        ]
-
-        self.__raw_code.clear()
-        for i, instruction in enumerate(self.__instructions):
-            if instruction.opcode > 255:
-                raise ValueError(f"invalid instruction at result level: {instruction}")
-
-            arg = instruction.get_arg()
-
-            if arg > 255:
-                extend = arg // 256
-                arg %= 256
-
-                offset = 1
-                while extend > 0:
-                    iarg = extend % 256
-                    extend //= 256
-
-                    if self.__raw_code[(i - offset) * 2] != Opcodes.NOP:
-                        raise ValueError(
-                            f"Cannot assemble fast, not enough NOP's for instruction {instruction}"
-                        )
-
-                    self.__raw_code[(i - offset) * 2 : (i - offset + 1) * 2] = bytes(
-                        [Opcodes.EXTENDED_ARG, iarg]
-                    )
-                    offset += 1
-
-            if not (0 <= arg <= 255 and 0 <= instruction.opcode <= 255):
-                print("error", instruction)
-
-            self.__raw_code += bytes([instruction.opcode, arg])
-
-    def get_raw_code(self):
-        if self.__instructions is not None:
-            self.assemble_instructions()
-
-        return self.__raw_code
-
-    def set_raw_code(self, raw_code: bytearray):
-        self.__raw_code = raw_code
-
-        if self.__instructions is not None:
-            self.decode_instructions()
-
-    raw_code = property(get_raw_code, set_raw_code)
-
-    def get_instructions(self):
-        if self.__instructions is None:
-            self.decode_instructions()
-
-        return self.__instructions
-
-    def set_instructions(self, instructions: typing.List[Instruction]):
-        # Update the ownerships of the instructions, so they point to us now
-        # todo: do we want to copy in some cases?
-        self.__instructions = [
-            instruction.update_owner(self, i)
-            for i, instruction in enumerate(instructions)
-        ]
-
-    instructions = property(get_instructions, set_instructions)
-
-    def allocate_shared_name(self, name: str) -> int:
-        if name in self.shared_names:
-            return self.shared_names.index(name)
-        self.shared_names.append(name)
-        return len(self.shared_names) - 1
-
-    def allocate_shared_constant(self, value: object) -> int:
-        if value in self.constants:
-            return self.constants.index(value)
-        self.constants.append(value)
-        return len(self.constants) - 1
-
-    def allocate_shared_variable_name(self, variable_name: str) -> int:
-        if variable_name in self.shared_variable_names:
-            return self.shared_variable_names.index(variable_name)
-        self.shared_variable_names.append(variable_name)
-        return len(self.shared_variable_names) - 1
-
-    def allocate_shared_cell(self, name: str):
-        if name in self.cell_variables:
-            return self.cell_variables.index(name)
-        self.cell_variables.append(name)
-        return len(self.cell_variables) - 1
-
-    def dump_info(self, file: str):
-        data = {
-            "instructions": [
-                {
-                    "opcode": instr.opcode,
-                    "opname": instr.opname,
-                    "arg": instr.arg,
-                    "arg_value": repr(instr.arg_value),
-                    "offset": instr.offset,
-                }
-                for instr in self.instructions
-            ]
-        }
-
-        with open(file, mode="w") as f:
-            simplejson.dump(data, f, indent="  ")
-
-
-bytecodemanipulation.data_loader.init()
+import copy
+import dis
+import sys
+import types
+import typing
+import simplejson
+
+import bytecodemanipulation.assembler.util.tokenizer
+from bytecodemanipulation.Opcodes import HAS_CELL_VARIABLE
+from bytecodemanipulation.Opcodes import HAS_JUMP_BACKWARDS
+from bytecodemanipulation.Opcodes import (
+    Opcodes,
+    END_CONTROL_FLOW,
+    OPCODE2NAME,
+    OPNAME2CODE,
+    HAS_NAME,
+    HAS_CONST,
+    HAS_LOCAL,
+    HAS_JUMP_ABSOLUTE,
+    HAS_JUMP_FORWARD,
+    UNCONDITIONAL_JUMPS,
+)
+import bytecodemanipulation.data_loader
+from bytecodemanipulation.util import AbstractInstructionWalker
+
+
+class LinearCodeConstraintViolationException(Exception):
+    pass
+
+
+class Instruction:
+    @classmethod
+    def _pair_instruction(cls, opcode: int | str) -> typing.Tuple[int, str]:
+        if isinstance(opcode, int):
+            return opcode, OPCODE2NAME[opcode]
+
+        return OPNAME2CODE[opcode], opcode
+
+    __slots__ = (
+        "function",
+        "offset",
+        "opcode",
+        "opname",
+        "arg_value",
+        "arg",
+        "_next_instruction",
+        "previous_instructions",
+        "source_location",
+    )
+
+    @classmethod
+    def create(cls, *args, **kwargs):
+        return cls(None, -1, *args, **kwargs)
+
+    @classmethod
+    def create_with_token(
+        cls,
+        token: bytecodemanipulation.assembler.util.tokenizer.AbstractToken,
+        function: typing.Optional["MutableFunction"],
+        offset: int | None,
+        opcode_or_name: int | str,
+        arg_value: object = None,
+        arg: int = None,
+        _decode_next=True,
+    ) -> "Instruction":
+        raise NotImplementedError("not bound!")
+
+    def __init__(
+        self,
+        function: typing.Optional["MutableFunction"],
+        offset: int | None,
+        opcode_or_name: int | str,
+        arg_value: object = None,
+        arg: int = None,
+        _decode_next=True,
+        pos_info=None,
+    ):
+        self.function = function
+        self.offset = offset
+        self.opcode, self.opname = self._pair_instruction(opcode_or_name)
+        self.arg_value = arg_value
+        self.arg = arg
+        self.source_location = pos_info
+
+        if (
+            self.arg is not None
+            and self.arg_value is None
+            and (_decode_next or not self.has_jump())
+        ):
+            self.change_arg(self.arg)
+        elif (
+            self.arg_value is not None or self.opcode == Opcodes.LOAD_CONST
+        ) and self.arg is None:
+            self.change_arg_value(self.arg_value)
+
+        # Reference to the next instruction
+        # Will raise an exception if changed and not using assemble_instructions_from_tree()
+        self._next_instruction: typing.Optional[Instruction] = (
+            None
+            if function is None
+            or offset is None
+            or self.opcode in END_CONTROL_FLOW
+            or not _decode_next
+            else function.instructions[offset + 1]
+        )
+
+        self.previous_instructions: typing.List["Instruction"] | None = None
+
+    def copy(self, owner: "MutableFunction" = None) -> "Instruction":
+        instance = type(self)(
+            self.function,
+            self.offset,
+            self.opcode,
+            self.arg_value
+            if self.arg_value is not None or self.opcode == Opcodes.LOAD_CONST
+            else self.arg,
+        )
+
+        if owner:
+            instance.update_owner(owner, -1, force_change_arg_index=True)
+
+        return instance
+
+    def apply_visitor(
+        self,
+        visitor: AbstractInstructionWalker,
+        visited: typing.Set["Instruction"] = None,
+    ):
+        if visited is None:
+            visited = set()
+
+        if self in visited:
+            return
+
+        visited.add(self)
+
+        visitor.visit(self)
+
+        if self.has_stop_flow():
+            return
+
+        if self.next_instruction is not None and self.next_instruction != self:
+            self.next_instruction.apply_visitor(visitor, visited)
+
+        if self.has_jump() and isinstance(self.arg_value, Instruction):
+            typing.cast(Instruction, self.arg_value).apply_visitor(visitor, visited)
+
+    def apply_value_visitor(
+        self,
+        callback: typing.Callable[
+            ["Instruction", typing.Any | None, typing.Any | None], typing.Any
+        ],
+        visited: typing.Dict["Instruction", typing.Any] = None,
+    ) -> typing.Any:
+        if visited is None:
+            visited = {}
+
+        elif self in visited:
+            return visited[self]
+
+        visited[self] = None
+
+        if self.has_stop_flow():
+            return callback(self, None, None)
+
+        if self.has_jump() and isinstance(self.arg_value, Instruction):
+            return callback(
+                self,
+                self.next_instruction.apply_value_visitor(callback, visited),
+                self.arg_value.apply_value_visitor(callback, visited),
+            )
+
+        if self.next_instruction is not None:
+            return callback(
+                self, self.next_instruction.apply_value_visitor(callback, visited), None
+            )
+
+        return callback(self, None, None)
+
+    def add_previous_instruction(self, instruction: "Instruction"):
+        if self.previous_instructions is None:
+            self.previous_instructions = [instruction]
+        elif instruction not in self.previous_instructions:
+            self.previous_instructions.append(instruction)
+
+    def remove_previous_instruction(self, instruction: "Instruction"):
+        if (
+            self.previous_instructions is not None
+            and instruction in self.previous_instructions
+        ):
+            self.previous_instructions.remove(instruction)
+
+    def get_previous_instructions(self) -> typing.List["Instruction"]:
+        if self.has_stop_flow():
+            return []
+
+        if self.previous_instructions is None:
+            if self.function is None:
+                raise ValueError(
+                    f"Instruction {self} is not bound to a MutableFunction object, making retrieving the previous instruction list impossible!!"
+                )
+
+            self.function.prepare_previous_instructions()
+
+            if self.previous_instructions is None:
+                raise RuntimeError(
+                    f"Could not find previous instructions for {self}. This should NOT happen, as we asked the method which MUST yield results. (See MutableFunction.prepare_previous_instructions())"
+                )
+
+        return self.previous_instructions
+
+    def set_next_instruction(self, instruction: typing.Optional["Instruction"]):
+        if self._next_instruction is not None:
+            self._next_instruction.remove_previous_instruction(self)
+
+        self._next_instruction = instruction
+
+        if instruction is not None:
+            instruction.add_previous_instruction(self)
+
+    def get_next_instruction(self) -> typing.Optional["Instruction"]:
+        return self._next_instruction
+
+    next_instruction = property(get_next_instruction, set_next_instruction)
+
+    def __repr__(self):
+        assert self.function is None or isinstance(self.function.function_name, str)
+        assert isinstance(self.offset, int)
+        assert isinstance(self.opcode, int)
+        assert isinstance(self.arg, int) or self.arg is None
+        if id(self) == id(self.arg_value):
+            return self.repr_safe() + "@self_arg_value"
+
+        return f"Instruction(function={self.function.function_name if self.function else '{Not Bound}'}, position={self.offset}, opcode={self.opcode}, opname={self.opname}, arg={self.arg}, arg_value={self.arg_value.repr_safe() if self.arg_value is not None and isinstance(self.arg_value, Instruction) else self.arg_value}, has_next={self.next_instruction is not None})"
+
+    def repr_safe(self):
+        return f"Instruction(function={self.function.function_name if self.function else '{Not Bound}'}, position={self.offset}, opcode={self.opcode}, opname={self.opname}, arg={self.arg}, arg_value=..., has_next={self.next_instruction is not None})"
+
+    def __eq__(self, other):
+        if not isinstance(other, Instruction):
+            return False
+
+        return (
+            self.opcode == other.opcode
+            and (
+                self.offset == other.offset
+                or self.offset is None
+                or other.offset is None
+            )
+            and (
+                (self.arg_value == other.arg_value)
+                if not isinstance(self.arg_value, Instruction)
+                else (id(self.arg_value) == id(other.arg_value))
+                if self.arg_value is not None and other.arg_value is not None
+                else True
+            )
+        )
+
+    def lossy_eq(self, other: "Instruction") -> bool:
+        if not isinstance(other, Instruction):
+            return False
+
+        return self.opcode == other.opcode and (
+            (
+                (self.arg_value == other.arg_value)
+                if not isinstance(self.arg_value, Instruction)
+                else self.arg_value.lossy_eq(other.arg_value)
+            )
+            if (self.arg_value is not None and other.arg_value is not None)
+            or self.opcode == Opcodes.LOAD_CONST
+            else True
+        )
+
+    def __hash__(self):
+        return id(self)
+
+    def get_arg(self):
+        return 0 if self.arg is None else self.arg
+
+    def change_opcode(self, opcode: int | str, arg_value=None, update_next=True):
+        self.opcode, self.opname = self._pair_instruction(opcode)
+        # todo: what happens with the arg?
+
+        if update_next:
+            self.next_instruction = (
+                None
+                if self.function is None
+                or self.offset is None
+                or self.opcode in END_CONTROL_FLOW
+                or self.offset == -1
+                else self.function.instructions[self.offset + 1]
+            )
+
+        if self.opcode < dis.HAVE_ARGUMENT:
+            self.arg = 0
+            self.arg_value = None
+
+        if arg_value:
+            self.change_arg_value(arg_value)
+
+        return self
+
+    def change_arg_value(self, value: object):
+        self.arg_value = value
+
+        if self.function is not None:
+            if self.opcode in HAS_NAME:
+                assert isinstance(value, str)
+                self.arg = self.function.allocate_shared_name(value)
+            elif self.opcode in HAS_CELL_VARIABLE:
+                assert isinstance(value, str)
+                self.arg = self.function.allocate_shared_cell(value)
+            elif self.opcode in HAS_CONST:
+                self.arg = self.function.allocate_shared_constant(value)
+            elif self.opcode in HAS_LOCAL:
+                assert isinstance(value, str), (value, self.opname)
+                self.arg = self.function.allocate_shared_variable_name(value)
+            elif self.opcode in HAS_JUMP_ABSOLUTE:
+                if isinstance(value, Instruction):
+                    self.arg = value.offset
+            elif self.opcode == Opcodes.FOR_ITER:
+                if isinstance(value, Instruction):
+                    self.arg = value.offset - self.offset
+            elif self.opcode in HAS_JUMP_FORWARD:
+                assert isinstance(value, Instruction), value
+                self.arg = value.offset - self.offset
+        else:
+            self.arg = None
+
+    def change_arg(self, arg: int):
+        self.arg = arg
+
+        if self.function is not None:
+            try:
+                flag = False
+                if sys.version_info.minor >= 11:
+                    if self.opcode == Opcodes.LOAD_GLOBAL:
+                        self.arg_value = self.function.shared_names[arg >> 1]
+                        flag = True
+
+                if flag:
+                    pass
+                elif self.opcode in HAS_NAME:
+                    self.arg_value = self.function.shared_names[arg]
+                elif self.opcode in HAS_CELL_VARIABLE:
+                    self.arg_value = self.function.cell_variables[arg]
+                elif self.opcode in HAS_CONST:
+                    self.arg_value = self.function.constants[arg]
+                elif self.opcode in HAS_LOCAL:
+                    self.arg_value = self.function.shared_variable_names[arg]
+                elif self.opcode in HAS_JUMP_ABSOLUTE:
+                    self.arg_value = self.function.instructions[arg]
+                elif self.opcode in (Opcodes.FOR_ITER, Opcodes.SETUP_FINALLY):
+                    self.arg_value = self.function.instructions[arg + self.offset]
+                elif self.opcode in HAS_JUMP_FORWARD and self.offset is not None:
+                    self.arg_value = self.function.instructions[arg + self.offset]
+            except:
+                print(
+                    self.opname,
+                    arg,
+                    self.function.shared_names,
+                    self.function.constants,
+                    self.function.shared_variable_names,
+                )
+                raise
+        else:
+            self.arg_value = None
+
+    def has_name(self):
+        return self.opcode in HAS_NAME
+
+    def has_constant(self):
+        return self.opcode in HAS_CONST
+
+    def has_local(self):
+        return self.opcode in HAS_LOCAL
+
+    def has_jump_absolute(self):
+        return self.opcode in HAS_JUMP_ABSOLUTE
+
+    def has_jump_forward(self):
+        return self.opcode in HAS_JUMP_FORWARD
+
+    def has_jump_backward(self):
+        return self.opcode in HAS_JUMP_BACKWARDS
+
+    def has_cell_variable(self):
+        return self.opcode in HAS_CELL_VARIABLE
+
+    def has_jump(self):
+        return (
+            self.has_jump_absolute()
+            or self.has_jump_forward()
+            or self.has_jump_backward()
+        )
+
+    def has_unconditional_jump(self):
+        return self.opcode in UNCONDITIONAL_JUMPS
+
+    def has_stop_flow(self):
+        return self.opcode in END_CONTROL_FLOW
+
+    def update_owner(
+        self,
+        function: "MutableFunction",
+        offset: int,
+        update_following=True,
+        force_change_arg_index=False,
+    ):
+        previous_function = self.function
+
+        self.function = function
+        self.offset = offset
+
+        # If previously the ownership was unset, and we have not fully referenced args, do it now!
+        # todo: when previous owner was set, and arg is not None, we might need to de-ref the value
+        #    and re-ref afterwards, so the value lives in the new owner
+        if (
+            self.arg is not None
+            and self.arg_value is None
+            and (not force_change_arg_index or self.opcode != Opcodes.LOAD_CONST)
+        ):
+            self.change_arg(self.arg)
+        elif (self.arg_value is not None or self.opcode == Opcodes.LOAD_CONST) and (
+            self.arg is None or force_change_arg_index
+        ):
+            self.change_arg_value(self.arg_value)
+
+        if update_following:
+            self.next_instruction = (
+                (None if previous_function != function else self.next_instruction)
+                if function is None
+                or offset is None
+                or self.opcode in END_CONTROL_FLOW
+                or offset == -1
+                or offset + 1 >= len(function.instructions)
+                else function.instructions[offset + 1]
+            )
+
+        return self
+
+    def optimise_tree(self, visited: typing.Set["Instruction"] = None) -> "Instruction":
+        """
+        Optimises the instruction tree, removing NOP's and inlining unconditional jumps
+        WARNING: this WILL invalidate the linearity of any instruction list, you MUST use assemble_instructions_from_tree()
+        for inserting it back into the Function.
+
+        Requires next_instruction's to be set, meaning it must be owned at some point by a function
+        """
+
+        if self.has_unconditional_jump():
+            return self.arg_value.optimise_tree(visited)
+
+        if visited is None:
+            visited = set()
+
+        if self in visited:
+            return self
+
+        visited.add(self)
+
+        if self.opcode == Opcodes.NOP and self.next_instruction is not None:
+            return self.next_instruction.optimise_tree(visited)
+
+        while self.next_instruction is not None:
+            assert isinstance(self.next_instruction, Instruction)
+
+            if self.next_instruction.opname == "NOP":
+                self.next_instruction = self.next_instruction.next_instruction
+                continue
+
+            if self.next_instruction.opname in ("JUMP_ABSOLUTE", "JUMP_FORWARD"):
+                self.next_instruction = self.next_instruction.arg_value
+                continue
+
+            break
+
+        if (
+            self.next_instruction is not None
+            and not self.has_stop_flow()
+            and not self.has_unconditional_jump()
+        ):
+            self.next_instruction = self.next_instruction.optimise_tree(visited)
+
+        if (
+            self.has_jump_absolute()
+            or self.has_jump_forward()
+            or self.has_jump_backward()
+        ) and self.arg_value is not None:
+            assert isinstance(self.arg_value, Instruction)
+            self.change_arg_value(self.arg_value.optimise_tree(visited))
+
+        return self
+
+    def trace_variable_set(
+        self, name: str, visited: typing.Set[str] = None
+    ) -> typing.Iterator["Instruction"]:
+        if visited and self in visited:
+            return
+
+        if self.opcode == Opcodes.STORE_FAST and self.arg_value == name:
+            yield self
+            return
+
+        if self.opcode == Opcodes.DELETE_FAST:
+            return
+
+        if visited is None:
+            visited = {self}
+
+        if self.previous_instructions is None:
+            return
+
+        for prev in self.previous_instructions:
+            yield from prev.trace_variable_set(name, visited)
+
+    def trace_stack_position(
+        self, stack_position: int
+    ) -> typing.Iterator["Instruction"]:
+        for instr in self.get_priorities_previous():
+            yield from instr._trace_stack_position(stack_position, set(), self)
+
+    def get_priorities_previous(self) -> typing.List["Instruction"]:
+        if not self.previous_instructions:
+            return []
+
+        real_previous = [
+            instr
+            for instr in self.previous_instructions
+            if instr.next_instruction == self
+        ]
+        unreal_previous = [
+            instr
+            for instr in self.previous_instructions
+            if instr.next_instruction != self
+        ]
+        highest = None
+
+        for e in real_previous:
+            if e.offset == self.offset - 1 or e.opcode == Opcodes.SETUP_FINALLY:
+                highest = e
+
+        if not highest:
+            return real_previous + unreal_previous
+
+        return [highest] + [e for e in real_previous if e != highest] + unreal_previous
+
+    def trace_normalized_stack_position(
+        self, stack_position: int
+    ) -> typing.Optional["Instruction"]:
+        target = next(self.trace_stack_position(stack_position))
+
+        if target.opcode == Opcodes.DUP_TOP:
+            return target.trace_normalized_stack_position(0)
+
+        if target.opcode == Opcodes.LOAD_FAST:
+            try:
+                variable_set = next(
+                    target.trace_variable_set(typing.cast(str, target.arg_value))
+                )
+            except StopIteration:
+                return target
+
+            return variable_set.trace_normalized_stack_position(0)
+
+        return target
+
+    def _trace_stack_position(
+        self,
+        stack_position: int,
+        yielded: typing.Set["Instruction"],
+        previous_instr: "Instruction" = None,
+    ) -> typing.Iterator["Instruction"]:
+        assert stack_position >= 0
+
+        if self in yielded:
+            return
+
+        if self.has_unconditional_jump():
+            pushed, popped, additional_pos = 0, 0, None
+        elif self.opcode == Opcodes.SETUP_FINALLY and previous_instr == self.arg_value:
+            pushed, popped, additional_pos = 3, 0, None
+        elif self.opcode in (
+            Opcodes.JUMP_IF_TRUE_OR_POP,
+            Opcodes.JUMP_IF_FALSE_OR_POP,
+        ):
+            if self.arg_value == previous_instr:
+                pushed, popped, additional_pos = 0, 0, None
+            else:
+                pushed, popped, additional_pos = 0, 1, None
+        else:
+            pushed, popped, additional_pos = self.get_stack_affect()
+
+        # print(self, stack_position, (pushed, popped, additional_pos), self.arg_value, previous_instr)
+
+        if pushed > stack_position:
+            yielded.add(self)
+            # print("hit")
+            yield self
+            # print("cont")
+
+            if additional_pos:
+                for instr in self.get_priorities_previous():
+                    yield from instr._trace_stack_position(
+                        additional_pos, yielded, self
+                    )
+
+            return
+
+        stack_position -= pushed
+        stack_position += popped
+
+        yielded.add(self)
+
+        for instr in self.get_priorities_previous():
+            try:
+                yield from instr._trace_stack_position(stack_position, yielded, self)
+            except:
+                # print(self, instr)
+                raise
+
+        if additional_pos:
+            for instr in self.get_priorities_previous():
+                yield from instr._trace_stack_position(additional_pos, yielded, self)
+
+    def trace_stack_position_use(
+        self, stack_position: int
+    ) -> typing.Iterator["Instruction"]:
+        # print(self, 0)
+
+        if not self.has_stop_flow():
+            yield from self.next_instruction._trace_stack_position_use(
+                stack_position, set()
+            )
+
+        if self.has_jump():
+            yield from typing.cast(
+                Instruction, self.arg_value
+            )._trace_stack_position_use(stack_position, set())
+
+    def _trace_stack_position_use(
+        self, stack_position: int, yielded: typing.Set["Instruction"]
+    ) -> typing.Iterator["Instruction"]:
+        assert stack_position >= 0
+
+        if self in yielded:
+            return
+
+        yielded.add(self)
+
+        pushed, popped, additional_pos = self.get_stack_affect()
+
+        if popped > stack_position:
+            yielded.add(self)
+            yield self
+
+            if additional_pos:
+                yield from self.next_instruction._trace_stack_position_use(
+                    additional_pos, yielded
+                )
+
+            return
+
+        stack_position -= popped
+        stack_position += pushed
+
+        if not self.has_stop_flow():
+            yield from self.next_instruction._trace_stack_position_use(
+                stack_position, yielded
+            )
+
+        if self.has_jump():
+            yield from typing.cast(
+                Instruction, self.arg_value
+            )._trace_stack_position_use(stack_position, yielded)
+
+        if additional_pos:
+            yield from self.next_instruction._trace_stack_position_use(
+                additional_pos, yielded
+            )
+
+    def get_stack_affect(self) -> typing.Tuple[int, int, int | None]:
+        # pushed, popped, additional
+        if self.opcode in (
+            Opcodes.NOP,
+            Opcodes.POP_BLOCK,
+            Opcodes.POP_EXCEPT,
+            Opcodes.SETUP_FINALLY,
+            Opcodes.GEN_START,
+            Opcodes.JUMP_ABSOLUTE,
+            Opcodes.BYTECODE_LABEL,
+            # Opcodes.CACHE,
+            # Opcodes.PRECALL,
+            # Opcodes.RESUME,
+        ):
+            return 0, 0, None
+
+        if self.opcode == Opcodes.DUP_TOP:
+            return 2, 1, None
+
+        if self.opcode == Opcodes.GET_ITER:
+            return 1, 0, None
+
+        if self.opcode == Opcodes.FOR_ITER:
+            return 1, 1, None
+
+        if self.opcode in (
+            Opcodes.LOAD_CONST,
+            Opcodes.LOAD_GLOBAL,
+            Opcodes.LOAD_FAST,
+            Opcodes.LOAD_DEREF,
+            Opcodes.LOAD_CLOSURE,
+            Opcodes.LOAD_BUILD_CLASS,
+            Opcodes.LOAD_ASSERTION_ERROR,
+            Opcodes.LOAD_NAME,
+        ):
+            return 1, 0, None
+
+        if self.opcode in (
+            Opcodes.BUILD_TUPLE,
+            Opcodes.BUILD_LIST,
+            Opcodes.BUILD_SET,
+            Opcodes.BUILD_SLICE,
+            Opcodes.BUILD_STRING,
+        ):
+            return 1, self.arg, None
+
+        if self.opcode in (Opcodes.ROT_TWO,):
+            return 2, 2, None
+
+        if self.opcode in (Opcodes.FORMAT_VALUE,):
+            return 1, (2 if (self.arg & 0x04) == 0x04 else 1), None
+
+        if self.opcode in (
+            Opcodes.CALL_FUNCTION,
+            Opcodes.CALL_METHOD,
+            Opcodes.CALL_FUNCTION_KW,
+            # Opcodes.CALL,
+        ):
+            return 1, self.arg + 1, None
+
+        if self.opcode in (Opcodes.CALL_FUNCTION_EX,):
+            count = 2
+
+            if self.arg & 0x01:
+                count += 1
+
+            return 1, count, None
+
+        if self.opcode == Opcodes.BUILD_MAP:
+            return 1, self.arg * 2, None
+
+        if self.opcode in (
+            Opcodes.COMPARE_OP,
+            Opcodes.IS_OP,
+            Opcodes.BINARY_SUBSCR,
+            Opcodes.CONTAINS_OP,
+            Opcodes.LIST_EXTEND,
+            Opcodes.LIST_APPEND,
+            Opcodes.SET_ADD,
+            Opcodes.SET_UPDATE,
+            Opcodes.DICT_UPDATE,
+            Opcodes.DICT_MERGE,
+            Opcodes.BINARY_FLOOR_DIVIDE,
+            Opcodes.BINARY_ADD,
+            Opcodes.INPLACE_ADD,
+            Opcodes.BINARY_SUBTRACT,
+            Opcodes.BINARY_MULTIPLY,
+            Opcodes.BINARY_TRUE_DIVIDE,
+            Opcodes.BINARY_FLOOR_DIVIDE,
+            Opcodes.BINARY_MODULO,
+            Opcodes.BINARY_XOR,
+            Opcodes.BINARY_AND,
+            Opcodes.BINARY_OR,
+            Opcodes.BINARY_POWER,
+            Opcodes.INPLACE_SUBTRACT,
+            Opcodes.IMPORT_NAME,
+            Opcodes.YIELD_FROM,
+        ):
+            return 1, 2, None
+
+        if self.opcode in (
+            Opcodes.LOAD_ATTR,
+            Opcodes.LOAD_METHOD,
+            Opcodes.GET_AWAITABLE,
+            Opcodes.LIST_TO_TUPLE,
+            Opcodes.IMPORT_FROM,
+            Opcodes.UNARY_NEGATIVE,
+            Opcodes.YIELD_VALUE,
+            Opcodes.GET_YIELD_FROM_ITER,
+            Opcodes.UNARY_NOT,
+            Opcodes.UNARY_NEGATIVE,
+            Opcodes.UNARY_INVERT,
+            Opcodes.UNARY_POSITIVE,
+            Opcodes.STATIC_ATTRIBUTE_ACCESS,
+        ):
+            return 1, 1, None
+
+        if self.opcode in (Opcodes.STORE_ATTR,):
+            return 2, 0, None
+
+        if self.opcode in (
+            Opcodes.POP_TOP,
+            Opcodes.POP_JUMP_IF_TRUE,
+            Opcodes.POP_JUMP_IF_FALSE,
+            Opcodes.STORE_FAST,
+            Opcodes.STORE_NAME,
+            Opcodes.STORE_DEREF,
+            Opcodes.STORE_GLOBAL,
+            Opcodes.RETURN_VALUE,
+        ):
+            return 0, 1, None
+
+        if self.opcode == Opcodes.UNPACK_SEQUENCE:
+            return self.arg, 1, None
+
+        if self.opcode == Opcodes.JUMP_IF_NOT_EXC_MATCH:
+            return 0, 2, None
+
+        if self.opcode == Opcodes.MAKE_FUNCTION:
+            return 1, 2 + self.arg.bit_count(), None
+
+        if self.opcode == Opcodes.RAISE_VARARGS:
+            return 0, self.arg, None
+
+        if self.opcode == Opcodes.DUP_TOP_TWO:
+            return 2, 4, None
+
+        raise RuntimeError(self)
+
+    def special_stack_affect_when_followed_by(self, instr: "Instruction") -> int:
+        if self.opcode == Opcodes.FOR_ITER and instr == self.arg_value:
+            return -2
+
+        return 0
+
+    def insert_after(self, *instructions: "Instruction" | typing.List["Instruction"]):
+        if not instructions:
+            return self
+
+        if isinstance(instructions[0], (list, tuple)):
+            if len(instructions) > 1:
+                raise ValueError
+
+            instructions = instructions[0]
+
+        if len(instructions) == 0:
+            return self
+
+        instructions[0].next_instruction = self.next_instruction
+        self.next_instruction = instructions[0]
+
+        if len(instructions) > 1:
+            instructions[0].insert_after(instructions[1:])
+
+        return self
+
+
+class MutableFunction:
+    @classmethod
+    def create(cls, target):
+        if isinstance(target, staticmethod):
+            return cls(target.__func__)
+        elif isinstance(target, classmethod):
+            return cls(target.__func__)
+        return cls(target)
+
+    def __init__(self, target: types.FunctionType | types.MethodType):
+        self.target = target
+
+        self.code_object: types.CodeType = target.__code__
+
+        self._load_from_code_object(self.code_object)
+
+    if sys.version_info.major == 3 and sys.version_info.minor == 10:
+
+        def _load_from_code_object(self, obj: types.CodeType):
+            self.argument_count = self.code_object.co_argcount
+            self.cell_variables = list(self.code_object.co_cellvars)
+            self.__raw_code = bytearray(self.code_object.co_code)
+            self.constants = list(self.code_object.co_consts)
+            self.filename = self.code_object.co_filename
+            self.first_line_number = self.code_object.co_firstlineno
+            self.code_flags = self.code_object.co_flags
+            self.free_variables = list(self.code_object.co_freevars)
+            self.keyword_only_argument_count = self.code_object.co_kwonlyargcount
+            self.line_table = self.code_object.co_linetable
+            self.lnotab = bytearray(self.code_object.co_lnotab)
+
+            self.function_name = self.code_object.co_name
+            self.shared_names = list(self.code_object.co_names)
+            # Local variable count is implied by co_varnames
+            self.positional_only_argument_count = self.code_object.co_posonlyargcount
+            self.stack_size = self.code_object.co_stacksize
+            self.shared_variable_names = list(self.code_object.co_varnames)
+
+            self.__instructions: typing.Optional[typing.List[Instruction]] = None
+
+    elif sys.version_info.major == 3 and sys.version_info.minor == 11:
+
+        def _load_from_code_object(self, obj: types.CodeType):
+            self.argument_count = self.code_object.co_argcount
+            self.cell_variables = list(self.code_object.co_cellvars)
+            self.__raw_code = bytearray(self.code_object.co_code)
+            self.constants = list(self.code_object.co_consts)
+            self.filename = self.code_object.co_filename
+            self.first_line_number = self.code_object.co_firstlineno
+            self.code_flags = self.code_object.co_flags
+            self.free_variables = list(self.code_object.co_freevars)
+            self.keyword_only_argument_count = self.code_object.co_kwonlyargcount
+            self.line_table = self.code_object.co_linetable
+            self.lnotab = bytearray(self.code_object.co_lnotab)
+
+            self.function_name = self.code_object.co_name
+            self.shared_names = list(self.code_object.co_names)
+            # Local variable count is implied by co_varnames
+            self.positional_only_argument_count = self.code_object.co_posonlyargcount
+            self.stack_size = self.code_object.co_stacksize
+            self.shared_variable_names = list(self.code_object.co_varnames)
+
+            self.exception_table = bytearray(self.code_object.co_exceptiontable)
+
+            self.__instructions: typing.Optional[typing.List[Instruction]] = None
+
+    else:
+        raise RuntimeError(sys.version_info)
+
+    def __repr__(self):
+        return f"MutableFunction({self.target})"
+
+    def copy(self):
+        def _():
+            pass
+
+        instance = type(self)(_)
+        instance.copy_from(self)
+
+        return instance
+
+    def copy_from(self, mutable: "MutableFunction"):
+        # self.target = mutable.target
+        self.code_object = mutable.code_object
+
+        self.argument_count = mutable.argument_count
+        self.cell_variables = mutable.cell_variables.copy()
+        self.__raw_code = mutable.raw_code.copy()
+        self.constants = copy.deepcopy(mutable.constants)
+        self.filename = mutable.filename
+        self.first_line_number = mutable.first_line_number
+        self.code_flags = mutable.code_flags
+        self.free_variables = mutable.free_variables.copy()
+        self.keyword_only_argument_count = mutable.keyword_only_argument_count
+        self.line_table = copy.copy(mutable.line_table)
+        self.lnotab = mutable.lnotab
+        self.function_name = mutable.function_name
+        self.shared_names = mutable.shared_names.copy()
+        self.positional_only_argument_count = mutable.positional_only_argument_count
+        self.stack_size = mutable.stack_size
+        self.shared_variable_names = mutable.shared_variable_names.copy()
+
+        self.__instructions = None
+
+    if sys.version_info.major == 3 and sys.version_info.minor == 10:
+
+        def create_code_obj(self) -> types.CodeType:
+            if self.__instructions is None:
+                self.get_instructions()
+
+            self.assemble_fast(self.__instructions)
+
+            return types.CodeType(
+                self.argument_count,
+                self.positional_only_argument_count,
+                self.keyword_only_argument_count,
+                len(self.shared_variable_names),
+                self.stack_size,
+                self.code_flags,
+                bytes(self.raw_code),
+                tuple(self.constants),
+                tuple(self.shared_names),
+                tuple(self.shared_variable_names),
+                self.filename,
+                self.function_name,
+                self.first_line_number,
+                self.get_lnotab(),
+                tuple(self.free_variables),
+                tuple(self.cell_variables),
+            )
+
+    elif sys.version_info.major == 3 and sys.version_info.minor == 11:
+
+        def create_code_obj(self) -> types.CodeType:
+            if self.__instructions is None:
+                self.get_instructions()
+
+            self.assemble_fast(self.__instructions)
+
+            return types.CodeType(
+                self.argument_count,
+                self.positional_only_argument_count,
+                self.keyword_only_argument_count,
+                len(self.shared_variable_names),
+                self.stack_size,
+                self.code_flags,
+                bytes(self.raw_code),
+                tuple(self.constants),
+                tuple(self.shared_names),
+                tuple(self.shared_variable_names),
+                self.filename,
+                self.function_name,
+                self.function_name,
+                self.first_line_number,
+                self.get_lnotab(),
+                bytes(self.exception_table),
+                tuple(self.free_variables),
+                tuple(self.cell_variables),
+            )
+
+    def get_lnotab(self) -> bytes:
+        items = []
+
+        prev_line = self.first_line_number
+        count_since_previous = 0
+
+        for instr in self.__instructions:
+            count_since_previous += 1
+
+            if instr.source_location is None or instr.source_location[0] == prev_line:
+                continue
+
+            offset = instr.source_location[0] - prev_line
+
+            if offset > 127:
+                return bytes()
+
+            if offset < 0:
+                return bytes()
+
+            items.append(count_since_previous)
+            items.append(offset)
+            count_since_previous = 0
+
+        return bytes(items)
+
+    def calculate_max_stack_size(self) -> int:
+        stack_size_table = self.get_max_stack_size_table()
+
+        self.stack_size = max(max(stack_size_table), 0)
+        return self.stack_size
+
+    def get_max_stack_size_table(
+        self, instructions: typing.List[Instruction] = None
+    ) -> typing.List[int]:
+        stack_size_table = [-1] * len(instructions or self.instructions)
+
+        if not instructions:
+            self.prepare_previous_instructions()
+
+        for i, instr in enumerate(instructions or self.instructions):
+            stack = -1
+            if i != 0:
+                prev = (instructions or self.instructions)[i - 1]
+
+                if not prev.has_stop_flow() and not prev.has_unconditional_jump():
+                    stack = stack_size_table[i - 1]
+            else:
+                stack = 0
+
+            if instr.previous_instructions:
+                for instruction in instr.previous_instructions:
+                    if stack_size_table[instruction.offset] != -1:
+                        stack = max(stack, stack_size_table[instruction.offset])
+                        stack += instruction.special_stack_affect_when_followed_by(
+                            instr
+                        )
+
+            if stack != -1:
+                add, sub, _ = instr.get_stack_affect()
+                stack += add
+                stack -= sub
+
+            stack_size_table[i] = stack
+
+        if -1 in stack_size_table:
+            pending = list(filter(lambda e: e[1] == -1, enumerate(stack_size_table)))
+            last_next = -1
+
+            while pending:
+                i, _ = pending.pop(0)
+                instr = (instructions or self.instructions)[i]
+                stack = -1
+
+                if i == last_next:
+                    break
+
+                if not instr.previous_instructions:
+                    print("WARN:", instr)
+                    continue
+
+                for instruction in instr.previous_instructions:
+                    if stack_size_table[instruction.offset] != -1:
+                        stack = max(stack, stack_size_table[instruction.offset])
+                        stack += instruction.special_stack_affect_when_followed_by(
+                            instr
+                        )
+
+                if stack != -1:
+                    add, sub, _ = instr.get_stack_affect()
+                    stack += add
+                    stack -= sub
+
+                    stack_size_table[i] = stack
+
+                    if pending:
+                        last_next = pending[0][0]
+                else:
+                    pending.append((i, -1))
+
+                if last_next == -1:
+                    last_next = i
+
+        return stack_size_table
+
+    def reassign_to_function(self):
+        self.calculate_max_stack_size()
+        self.target.__code__ = self.create_code_obj()
+
+    def decode_instructions(self):
+        if self.__instructions is not None:
+            self.__instructions.clear()
+        else:
+            self.__instructions = []
+
+        line = self.first_line_number
+        lnotab = list(self.lnotab)
+
+        extra: int = 0
+        for i in range(0, len(self.__raw_code), 2):
+            opcode, arg = self.__raw_code[i : i + 2]
+
+            if opcode == Opcodes.EXTENDED_ARG:
+                extra = extra * 256 + arg
+                instr = Instruction(self, i // 2, "NOP", _decode_next=False)
+
+            else:
+                arg += extra * 256
+                extra = 0
+
+                if opcode in (Opcodes.FOR_ITER, Opcodes.SETUP_FINALLY):
+                    arg += 1
+
+                instr = Instruction(self, i // 2, opcode, arg=arg, _decode_next=False)
+
+            if lnotab:
+                lnotab[0] -= 1
+
+                if lnotab[0] == 0:
+                    line_incr = lnotab[1]
+                    del lnotab[:2]
+
+                    line += line_incr
+
+            instr.source_location = (line, None, None)
+
+            self.__instructions.append(instr)
+            # print(instr, instr.source_location)
+
+        for i, instruction in enumerate(self.instructions):
+            instruction.update_owner(self, i)
+
+        self.prepare_previous_instructions()
+
+    def prepare_previous_instructions(self):
+        for instruction in self.instructions:
+            if instruction.previous_instructions:
+                instruction.previous_instructions.clear()
+
+        for instruction in self.instructions:
+            if instruction.has_stop_flow() or instruction.has_unconditional_jump():
+                continue
+
+            instruction.next_instruction.add_previous_instruction(instruction)
+
+            if instruction.has_jump():
+                # print(instruction.arg_value, typing.cast, typing.cast(Instruction, instruction.arg_value))
+
+                typing.cast(
+                    Instruction, instruction.arg_value
+                ).add_previous_instruction(instruction)
+
+    def assemble_instructions_from_tree(self, root: Instruction, breaks_flow=tuple()):
+        # 1. Assemble a linear stream of instructions, containing all instructions
+        # 2. check instructions which require unconditional JUMP's and insert them
+        # 3. update instruction positions
+        # 4. Update the arg value of jumps
+        # 5. Walk over all instructions and set extended arg count + insert NOP's, and recheck if instructions need more extended
+        # 6. Resolve jump target into real values
+        # 7. Profit! (Maybe use assemble_fast() here!
+
+        instructions = self.assemble_linear_instructions(breaks_flow, root)
+
+        self.update_instruction_offsets(instructions)
+
+        self.insert_needed_jumps(instructions)
+
+        self.update_instruction_offsets(instructions)
+
+        self.update_jump_args(instructions)
+        required_extends = self.get_required_arg_extensions(instructions)
+        self.insert_required_nops(instructions, required_extends)
+        self.update_jump_args(instructions)
+
+        # Check how many EXTENDED_ARG we really need
+        required_extends_2 = self.get_required_arg_extensions(instructions)
+
+        if required_extends != required_extends_2:
+            # todo: here, walk again over the instruction list
+            raise NotImplementedError
+
+        # For a last time, walk over the instructions and tie them together
+        for i, instruction in enumerate(instructions[:]):
+            if (
+                not instruction.has_stop_flow()
+                and not instruction.has_unconditional_jump()
+            ):
+                try:
+                    instruction.next_instruction = instructions[i + 1]
+                except IndexError:
+                    instruction.next_instruction = None
+                except:
+                    print(instruction)
+                    print(instruction.next_instruction)
+                    raise
+
+        self.assemble_fast(instructions)
+        self.update_instruction_offsets(self.instructions)
+        # We do not re-decode, as that would invalidate the instruction instances here
+
+    def update_instruction_offsets(self, instructions):
+        # Update instruction positions
+        for i, instruction in enumerate(instructions):
+            instruction.offset = i
+
+    def insert_required_nops(self, instructions, required_extends):
+        write_offset = 0
+        # Now insert the required NOP's
+        for instruction, count in zip(instructions[:], required_extends):
+            if count == 0:
+                continue
+
+            for _ in range(count):
+                pos = instruction.offset + write_offset
+                instructions.insert(
+                    pos, nop_instr := Instruction.create(self, pos, "NOP")
+                )
+
+            write_offset += count
+
+    def get_required_arg_extensions(self, instructions):
+        # Check how many EXTENDED_ARG we need
+        required_extends = [0] * len(instructions)
+        for i, instruction in enumerate(instructions):
+            arg = instruction.arg
+
+            if arg is None:
+                if instruction.opcode < dis.HAVE_ARGUMENT:
+                    arg = 0
+                else:
+                    print("error", instruction)
+
+            if arg >= 256**3:
+                count = 3
+            elif arg >= 256**2:
+                count = 2
+            elif arg >= 256:
+                count = 1
+            else:
+                count = 0
+            required_extends[i] = count
+        return required_extends
+
+    def update_jump_args(self, instructions):
+        # Update the raw arg for jumps
+        for i, instruction in enumerate(instructions):
+            if instruction.next_instruction is None:
+                continue
+
+            instruction.update_owner(self, i)
+
+            if instruction.has_jump_absolute():
+                instruction.change_arg_value(instruction.arg_value)
+            elif instruction.offset in (Opcodes.FOR_ITER, Opcodes.SETUP_FINALLY):
+                instruction.change_arg_value(instruction.arg_value)
+            elif instruction.has_jump_forward():
+                instruction.change_arg_value(instruction.arg_value)
+            elif instruction.has_jump_backward():
+                instruction.change_arg_value(instruction.arg_value)
+
+    def insert_needed_jumps(self, instructions):
+        # Check for unconditional jumps required
+        for instruction in instructions[:]:
+            if instruction.has_stop_flow():
+                continue
+
+            # FOR_ITER can only jump FORWARD, so insert a new jump absolute to jump there
+            # TODO: insert the JUMP somewhere else than here!
+            if instruction.opcode == Opcodes.FOR_ITER:
+                jump = Instruction(
+                    self,
+                    -1,
+                    "JUMP_ABSOLUTE",
+                    instruction.next_instruction,
+                )
+                jump.change_arg_value(instruction.arg_value)
+                instruction.change_arg_value(jump)
+                instructions.append(jump)
+
+            if (
+                instruction.next_instruction is not None
+                and instruction.offset + 1 != instruction.next_instruction.offset
+            ):
+                jump = Instruction(
+                    self,
+                    -1,
+                    "JUMP_ABSOLUTE",
+                    instruction.next_instruction,
+                )
+                jump.next_instruction = instruction
+                instruction.next_instruction = jump
+                instructions.insert(instructions.index(instruction) + 1, jump)
+
+    def assemble_linear_instructions(self, breaks_flow, root):
+
+        # While we have branches, we need to decode them
+        pending_instructions = [root]
+        visited: typing.Set[Instruction] = set()
+        instructions: typing.List[Instruction] = []
+
+        while pending_instructions:
+            instruction = pending_instructions.pop()
+
+            if not isinstance(instruction, Instruction):
+                print(f"Invalid task instruction: {instruction}")
+                continue
+
+            if not isinstance(instruction, Instruction):
+                raise ValueError(instruction)
+
+            # If we visited it, we can skip
+            if instruction in visited:
+                continue
+
+            # Walk over the instructions as long as we have not met them
+            while instruction not in visited:
+                if not isinstance(instruction, Instruction):
+                    print(f"Invalid task instruction: {instruction}")
+                    break
+
+                # If it branches off, it needs to be visited later on
+                if instruction.has_jump():
+                    if instruction.arg_value is None:
+                        instruction.update_owner(self, instruction.offset)
+
+                    assert instruction.arg_value is not None, instruction
+
+                    pending_instructions.append(instruction.arg_value)
+
+                instructions.append(instruction)
+                visited.add(instruction)
+
+                if (
+                    instruction.has_stop_flow()
+                    or instruction in breaks_flow
+                    or instruction.opcode in breaks_flow
+                ):
+                    break
+
+                if instruction.next_instruction is None:
+                    instruction.update_owner(self, instruction.offset)
+
+                # The next instruction MUST be set if it does NOT end the control flow
+                if instruction.next_instruction is None:
+                    print("---- start dump")
+                    for instr in instructions:
+                        print(instr)
+                    print("---- end dump")
+                    raise RuntimeError(f"next instruction is None: {instruction}")
+
+                instruction = instruction.next_instruction
+
+        return instructions
+
+    def assemble_instructions(self):
+
+        # Check for linearity violations
+        for i, instruction in enumerate(self.__instructions):
+            if (
+                instruction.next_instruction is not None
+                and instruction.offset + 1 != instruction.next_instruction.offset
+                and not instruction.has_unconditional_jump()
+                and not instruction.has_stop_flow()
+            ):
+                # todo: do we want to dynamic use assemble_instructions_from_tree()?
+                raise LinearCodeConstraintViolationException(
+                    f"Failed between instruction {instruction} and {instruction.next_instruction}, use assemble_instructions_from_tree(...) to assemble from an non-normal tree"
+                )
+
+        needs_tree_assemble = False
+        root = self.__instructions[0]
+        previous = None
+
+        # Check if the NOP's ahead of instructions are enough to hold the extra args
+        nop_count = 0
+        for i, instruction in enumerate(self.__instructions):
+            if instruction.opname == "NOP":
+                nop_count += 1
+                previous = instruction
+                continue
+
+            if instruction.arg is not None:
+                if instruction.arg >= 256**3:
+                    count = 3
+                elif instruction.arg >= 256**2:
+                    count = 2
+                elif instruction.arg >= 256:
+                    count = 1
+                else:
+                    count = 0
+
+                # Are there NOP's missing for the needed EXTENDED_ARG?
+                if count > nop_count:
+                    # todo: move this code up into assemble_instructions_from_tree()
+
+                    missing = count - nop_count  # how many we need
+                    needs_tree_assemble = True  # make sure that we use the assemble_instructions_from_tree() now
+
+                    # If we are at HEAD, we require some clever handling, as "previous" is None at the moment
+                    if i == 0:
+                        root = previous = Instruction(
+                            self,
+                            0,
+                            "NOP",
+                        )
+                        root.next_instruction = instruction
+                        missing -= 1
+
+                    previous.insert_after(
+                        [
+                            Instruction(self, previous.offset + i + 1, Opcodes.NOP)
+                            for i in range(missing)
+                        ]
+                    )
+
+                nop_count = 0
+
+            previous = instruction
+
+        if needs_tree_assemble:
+            self.assemble_instructions_from_tree(root)
+            return
+
+        # We are now sure that we have enough space for all data, so we can assemble the EXTENDED_ARG instructions
+        # duplicate of assemble_fast() with less safety checks, as we checked that stuff beforehand
+        self.__raw_code.clear()
+        for i, instruction in enumerate(self.__instructions):
+            arg = instruction.get_arg()
+
+            if instruction.opcode in (Opcodes.FOR_ITER, Opcodes.SETUP_FINALLY):
+                arg -= 1
+
+            if arg > 255:
+                extend = arg // 256
+                arg %= 256
+
+                offset = 1
+                while extend > 0:
+                    iarg = extend % 256
+                    extend //= 256
+
+                    self.__raw_code[(i - offset) * 2 : (i - offset + 1) * 2] = bytes(
+                        [Opcodes.EXTENDED_ARG, iarg]
+                    )
+                    offset += 1
+
+            self.__raw_code += bytes([instruction.opcode, arg])
+
+    def assemble_fast(self, instructions: typing.List[Instruction]):
+        """
+        Assembles the instruction list in FAST mode
+        Removes some safety checks, and removes the dynamic assemble_instructions_from_tree() forwarding.
+        Requires the linking of instructions to be LINEAR.
+
+        :raises ValueError: if not enough space for EXTENDED_ARG's is available
+        """
+
+        self.__instructions = [
+            instruction.update_owner(self, i, update_following=False)
+            for i, instruction in enumerate(instructions)
+        ]
+
+        self.__raw_code.clear()
+        for i, instruction in enumerate(self.__instructions):
+            if instruction.opcode > 255:
+                raise ValueError(f"invalid instruction at result level: {instruction}")
+
+            arg = instruction.get_arg()
+
+            if arg > 255:
+                extend = arg // 256
+                arg %= 256
+
+                offset = 1
+                while extend > 0:
+                    iarg = extend % 256
+                    extend //= 256
+
+                    if self.__raw_code[(i - offset) * 2] != Opcodes.NOP:
+                        raise ValueError(
+                            f"Cannot assemble fast, not enough NOP's for instruction {instruction}"
+                        )
+
+                    self.__raw_code[(i - offset) * 2 : (i - offset + 1) * 2] = bytes(
+                        [Opcodes.EXTENDED_ARG, iarg]
+                    )
+                    offset += 1
+
+            if not (0 <= arg <= 255 and 0 <= instruction.opcode <= 255):
+                print("error", instruction)
+
+            self.__raw_code += bytes([instruction.opcode, arg])
+
+    def get_raw_code(self):
+        if self.__instructions is not None:
+            self.assemble_instructions()
+
+        return self.__raw_code
+
+    def set_raw_code(self, raw_code: bytearray):
+        self.__raw_code = raw_code
+
+        if self.__instructions is not None:
+            self.decode_instructions()
+
+    raw_code = property(get_raw_code, set_raw_code)
+
+    def get_instructions(self):
+        if self.__instructions is None:
+            self.decode_instructions()
+
+        return self.__instructions
+
+    def set_instructions(self, instructions: typing.List[Instruction]):
+        # Update the ownerships of the instructions, so they point to us now
+        # todo: do we want to copy in some cases?
+        self.__instructions = [
+            instruction.update_owner(self, i)
+            for i, instruction in enumerate(instructions)
+        ]
+
+    instructions = property(get_instructions, set_instructions)
+
+    def allocate_shared_name(self, name: str) -> int:
+        if name in self.shared_names:
+            return self.shared_names.index(name)
+        self.shared_names.append(name)
+        return len(self.shared_names) - 1
+
+    def allocate_shared_constant(self, value: object) -> int:
+        if value in self.constants:
+            return self.constants.index(value)
+        self.constants.append(value)
+        return len(self.constants) - 1
+
+    def allocate_shared_variable_name(self, variable_name: str) -> int:
+        if variable_name in self.shared_variable_names:
+            return self.shared_variable_names.index(variable_name)
+        self.shared_variable_names.append(variable_name)
+        return len(self.shared_variable_names) - 1
+
+    def allocate_shared_cell(self, name: str):
+        if name in self.cell_variables:
+            return self.cell_variables.index(name)
+        self.cell_variables.append(name)
+        return len(self.cell_variables) - 1
+
+    def dump_info(self, file: str):
+        data = {
+            "instructions": [
+                {
+                    "opcode": instr.opcode,
+                    "opname": instr.opname,
+                    "arg": instr.arg,
+                    "arg_value": repr(instr.arg_value),
+                    "offset": instr.offset,
+                }
+                for instr in self.instructions
+            ]
+        }
+
+        with open(file, mode="w") as f:
+            simplejson.dump(data, f, indent="  ")
+
+
+bytecodemanipulation.data_loader.init()
```

### Comparing `bytecodemanipulation-0.2.4/bytecodemanipulation/MutableFunctionHelpers.py` & `bytecodemanipulation-0.2.8/bytecodemanipulation/MutableFunctionHelpers.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,382 +1,382 @@
-import typing
-
-from bytecodemanipulation.MutableFunction import MutableFunction, Instruction
-from bytecodemanipulation.Opcodes import Opcodes, HAS_GLOBAL
-from bytecodemanipulation.Opcodes import UNCONDITIONAL_JUMPS
-
-
-class Guarantees:
-    class AbstractGuarantee:
-        pass
-
-    RESULT_IS_CONSTANT = AbstractGuarantee()
-    NO_DISCARD = AbstractGuarantee()
-
-    class ArgIsNotMutated(AbstractGuarantee):
-        def __init__(self, arg_index: int, arg_name: str):
-            self.arg_index = arg_index
-            self.arg_name = arg_name
-
-    class ReturnType(AbstractGuarantee):
-        def __init__(self, data_type: type, may_subclass=False):
-            self.data_type = data_type
-            self.may_subclass = may_subclass
-
-
-class MethodInvocationInfo:
-    def __init__(self, call_instruction: Instruction):
-        self.call_instruction = call_instruction
-
-        if call_instruction.opcode == Opcodes.CALL_FUNCTION:
-            self.arg_loads = [
-                next(call_instruction.trace_stack_position(i))
-                for i in range(call_instruction.arg - 1, -1, -1)
-            ]
-            self.function_load = call_instruction.trace_normalized_stack_position(
-                call_instruction.arg
-            )
-        else:
-            raise NotImplementedError(call_instruction)
-
-        self._guarantees: typing.List[Guarantees.AbstractGuarantee] = None
-
-    def get_guarantees(self) -> typing.List[Guarantees.AbstractGuarantee]:
-        if self._guarantees:
-            return self._guarantees
-
-        if self.function_load.opcode != Opcodes.LOAD_CONST:
-            return []
-
-        from bytecodemanipulation.Optimiser import _OptimisationContainer
-
-        function_target = self.function_load.arg_value
-        optimisation_container = _OptimisationContainer.get_for_target(function_target)
-
-        self._guarantees = []
-        if optimisation_container.guarantees:
-            self._guarantees += optimisation_container.guarantees
-
-        return self._guarantees
-
-    def is_argument_mutated(self, name_or_index: str | int) -> bool:
-        for guarantee in self.get_guarantees():
-            if isinstance(guarantee, Guarantees.ArgIsNotMutated) and (
-                guarantee.arg_index == name_or_index
-                or guarantee.arg_name == name_or_index
-            ):
-                return False
-
-        return True
-
-
-class MutableFunctionWithTree:
-    def __init__(self, mutable: MutableFunction, root: Instruction = None):
-        self.mutable = mutable
-        self.root = root or mutable.instructions[0]
-
-    def visitor(
-        self, visitor: typing.Callable[[Instruction, typing.List[Instruction]], None]
-    ):
-        def visit(
-            instruction: Instruction,
-            visited: typing.Set[Instruction],
-            path: typing.List[Instruction],
-        ):
-            visitor(instruction, path)
-
-            if instruction in visited:
-                return
-
-            visited.add(instruction)
-
-            if not instruction.has_stop_flow():
-                visit(instruction.next_instruction, visited, path + [instruction])
-
-            if instruction.has_jump():
-                # visit the jump target, but reset the instruction path, as we cannot make sure that
-                # it is the only path leading there
-                # TODO: is there a better way? (first visit the main tree, and than branch?)
-                visit(instruction.arg_value, visited, [instruction])
-
-        visit(self.root, set(), [])
-
-    def print_recursive(self, root: Instruction = None, visited: set = None, level=0):
-        if root is None:
-            print("Starting Dump...")
-            root = self.root
-
-        if visited is None:
-            visited = set()
-        elif root in visited:
-            return
-
-        print(
-            " " * level + repr(root),
-            "-> -1"
-            if root.next_instruction is None
-            else "-> " + str(root.next_instruction.offset),
-        )
-        visited.add(root)
-
-        if root.has_stop_flow():
-            return
-
-        if root.next_instruction is None:
-            print("-" * level, "END OF CONTROL FLOW")
-            return
-
-        self.print_recursive(root.next_instruction, visited, level)
-
-        if root.has_jump():
-            self.print_recursive(root.arg_value, visited, level + 1)
-
-
-def prefix_all_locals_with(
-    mutable: MutableFunction | MutableFunctionWithTree,
-    prefix: str,
-    protected_locals: typing.List[str] = tuple(),
-):
-    if isinstance(mutable, MutableFunctionWithTree):
-        mutable.mutable.assemble_instructions_from_tree(mutable.root)
-        mutable = mutable.mutable
-
-    mutable.shared_variable_names = [
-        prefix + e if e not in protected_locals else e
-        for e in mutable.shared_variable_names
-    ]
-
-    print(mutable.shared_variable_names)
-
-    for instruction in mutable.instructions:
-        if instruction.has_local():
-            instruction.update_owner(mutable, instruction.offset)
-
-
-def replace_opcode_with_other(
-    mutable: MutableFunction | MutableFunctionWithTree,
-    old_opcode: int,
-    new_opcode: int,
-    handle_new: typing.Callable[[Instruction], None] = lambda _: None,
-):
-    if isinstance(mutable, MutableFunctionWithTree):
-        mutable.mutable.assemble_instructions_from_tree(mutable.root)
-        mutable = mutable.mutable
-
-    for instruction in mutable.instructions:
-        if instruction.opcode == old_opcode:
-            instruction.change_opcode(new_opcode)
-
-            handle_new(instruction)
-
-
-def inline_access_to_global(
-    mutable: MutableFunction | MutableFunctionWithTree, global_name: str, value=...
-):
-    if isinstance(mutable, MutableFunctionWithTree):
-        mutable.mutable.assemble_instructions_from_tree(mutable.root)
-        mutable = mutable.mutable
-
-    if value == ...:
-        value = mutable.target.__globals__[global_name]
-
-    for i, instruction in enumerate(mutable.instructions):
-        if instruction.opcode == Opcodes.LOAD_GLOBAL:
-            if instruction.arg_value == global_name:
-                instruction.change_opcode(Opcodes.LOAD_CONST)
-                instruction.change_arg_value(value)
-
-
-def replace_const_func_call_with_opcode(
-    mutable: MutableFunctionWithTree,
-    func: typing.Callable,
-    opcode: int,
-    handle_args: typing.Callable[
-        [MutableFunctionWithTree, Instruction, typing.List[Instruction]], bool
-    ],
-):
-    def visitor(instruction: Instruction, path: typing.List[Instruction]):
-        if instruction.opcode == Opcodes.CALL_FUNCTION:
-            counter = instruction.arg
-            args = path[-counter:]
-            load_method = path[-counter - 1]
-
-            if (
-                load_method.opcode == Opcodes.LOAD_CONST
-                and load_method.arg_value == func
-                and all(instr.opcode == Opcodes.LOAD_CONST for instr in args)
-            ):
-                instruction.change_opcode(opcode)
-                if not handle_args(mutable, instruction, args):
-                    instruction.change_opcode(Opcodes.CALL_FUNCTION)
-
-    mutable.visitor(visitor)
-
-
-def capture_local(name: str):
-    pass
-
-
-def outer_return(value=None):
-    pass
-
-
-def _inline_capture_local(
-    tree: MutableFunctionWithTree,
-    instruction: Instruction,
-    args: typing.List[Instruction],
-) -> bool:
-    if len(args) != 1:
-        return False
-    if args[0].opcode != Opcodes.LOAD_CONST:
-        return False
-
-    instruction.arg = args[0].arg
-    instruction.arg_value = args[0].arg_value
-    args[0].change_opcode(Opcodes.NOP)
-    args[0].arg = 0
-    args[0].arg_value = None
-
-    return True
-
-
-def _inline_outer_return(
-    tree: MutableFunctionWithTree,
-    instruction: Instruction,
-    args: typing.List[Instruction],
-) -> bool:
-    if len(args) > 1:
-        return False
-    if len(args) > 0 and args[0].opcode != Opcodes.LOAD_CONST:
-        return False
-
-    # In case we have no args, we need to add a LOAD_CONST(None)
-    if len(args) == 0:
-        instruction.change_opcode(Opcodes.LOAD_CONST)
-        instruction.change_arg_value(None)
-        return_instr = Instruction.create(Opcodes.RETURN_VALUE)
-        return_instr.update_owner(tree.mutable, -1)
-        return_instr.next_instruction = instruction.next_instruction
-        instruction.next_instruction = return_instr
-
-    return True
-
-
-def insert_method_into(
-    body: MutableFunction | MutableFunctionWithTree,
-    offset: typing.Union[Instruction, int],
-    to_insert: MutableFunction | MutableFunctionWithTree,
-    protected_locals: typing.List[str] = tuple(),
-):
-    """
-    Inserts the function AFTER the given offset / Instruction.
-    If wanted at HEAD, set offset to -1
-    """
-
-    if isinstance(to_insert, MutableFunctionWithTree):
-        to_insert.mutable.assemble_instructions_from_tree(to_insert.root)
-        to_insert = to_insert.mutable
-
-    if not isinstance(body, MutableFunctionWithTree):
-        body = MutableFunctionWithTree(body)
-
-    if offset == -1:
-        HEAD_INSTRUCTION = Instruction.create("NOP")
-        HEAD_INSTRUCTION.function = body.mutable
-        HEAD_INSTRUCTION.next_instruction = body.root
-        body.root = HEAD_INSTRUCTION
-    elif isinstance(offset, int):
-        body.mutable.assemble_instructions_from_tree(body.root)
-        HEAD_INSTRUCTION = body.mutable.instructions[offset]
-    else:
-        HEAD_INSTRUCTION = offset
-
-    for instr in to_insert.instructions:
-        instr.offset = -1
-
-    prefix_all_locals_with(to_insert, to_insert.function_name + ":", protected_locals)
-    replace_opcode_with_other(
-        to_insert, Opcodes.RETURN_VALUE, Opcodes.INTERMEDIATE_INNER_RETURN
-    )
-    inline_access_to_global(to_insert, "capture_local", capture_local)
-    inline_access_to_global(to_insert, "outer_return", outer_return)
-
-    # MutableFunctionWithTree(to_insert).print_recursive()
-
-    instr = None
-    previous = None
-    for instr in to_insert.instructions:
-        if previous is not None:
-            previous.next_instruction = instr
-
-        if instr.opcode == Opcodes.INTERMEDIATE_INNER_RETURN:
-            previous.next_instruction = Instruction.create(Opcodes.POP_TOP)
-            previous.next_instruction.update_owner(to_insert, -1)
-            previous.next_instruction.next_instruction = instr
-
-            instr.change_opcode(Opcodes.JUMP_ABSOLUTE)
-            instr.change_arg_value(HEAD_INSTRUCTION.next_instruction)
-
-        previous = instr
-
-    if instr is not None and instr.next_instruction is None:
-        instr.next_instruction = HEAD_INSTRUCTION.next_instruction
-
-    to_insert.assemble_instructions_from_tree(
-        to_insert.instructions[0],
-        breaks_flow=(
-            Instruction.create(
-                Opcodes.JUMP_ABSOLUTE, HEAD_INSTRUCTION.next_instruction
-            ),
-        ),
-    )
-    # MutableFunctionWithTree(to_insert).print_recursive()
-    # to_insert.decode_instructions()
-
-    for instr in to_insert.instructions:
-        instr.update_owner(body.mutable, -1, False)
-
-    to_insert_tree = MutableFunctionWithTree(to_insert)
-    # to_insert_tree.print_recursive()
-    replace_const_func_call_with_opcode(
-        to_insert_tree,
-        capture_local,
-        Opcodes.LOAD_FAST,
-        _inline_capture_local,
-    )
-    # to_insert_tree.print_recursive()
-    replace_const_func_call_with_opcode(
-        to_insert_tree,
-        outer_return,
-        Opcodes.RETURN_VALUE,
-        _inline_outer_return,
-    )
-    # to_insert_tree.print_recursive()
-
-    def visit(instruction: Instruction, path):
-        if instruction is None:
-            print(path)
-            raise
-
-        instruction.function = body.mutable
-
-        if instruction.has_constant():
-            instruction.arg = body.mutable.allocate_shared_constant(
-                instruction.arg_value
-            )
-
-        elif instruction.has_name():
-            instruction.arg = body.mutable.allocate_shared_name(instruction.arg_value)
-
-        elif instruction.has_local():
-            instruction.arg = body.mutable.allocate_shared_variable_name(
-                instruction.arg_value
-            )
-
-    HEAD_INSTRUCTION.next_instruction = to_insert_tree.root
-    body.visitor(visit)
-
-    # body.print_recursive()
-
-    body.mutable.assemble_instructions_from_tree(body.root)
-
-    # body.print_recursive()
+import typing
+
+from bytecodemanipulation.MutableFunction import MutableFunction, Instruction
+from bytecodemanipulation.Opcodes import Opcodes, HAS_GLOBAL
+from bytecodemanipulation.Opcodes import UNCONDITIONAL_JUMPS
+
+
+class Guarantees:
+    class AbstractGuarantee:
+        pass
+
+    RESULT_IS_CONSTANT = AbstractGuarantee()
+    NO_DISCARD = AbstractGuarantee()
+
+    class ArgIsNotMutated(AbstractGuarantee):
+        def __init__(self, arg_index: int, arg_name: str):
+            self.arg_index = arg_index
+            self.arg_name = arg_name
+
+    class ReturnType(AbstractGuarantee):
+        def __init__(self, data_type: type, may_subclass=False):
+            self.data_type = data_type
+            self.may_subclass = may_subclass
+
+
+class MethodInvocationInfo:
+    def __init__(self, call_instruction: Instruction):
+        self.call_instruction = call_instruction
+
+        if call_instruction.opcode == Opcodes.CALL_FUNCTION:
+            self.arg_loads = [
+                next(call_instruction.trace_stack_position(i))
+                for i in range(call_instruction.arg - 1, -1, -1)
+            ]
+            self.function_load = call_instruction.trace_normalized_stack_position(
+                call_instruction.arg
+            )
+        else:
+            raise NotImplementedError(call_instruction)
+
+        self._guarantees: typing.List[Guarantees.AbstractGuarantee] = None
+
+    def get_guarantees(self) -> typing.List[Guarantees.AbstractGuarantee]:
+        if self._guarantees:
+            return self._guarantees
+
+        if self.function_load.opcode != Opcodes.LOAD_CONST:
+            return []
+
+        from bytecodemanipulation.Optimiser import _OptimisationContainer
+
+        function_target = self.function_load.arg_value
+        optimisation_container = _OptimisationContainer.get_for_target(function_target)
+
+        self._guarantees = []
+        if optimisation_container.guarantees:
+            self._guarantees += optimisation_container.guarantees
+
+        return self._guarantees
+
+    def is_argument_mutated(self, name_or_index: str | int) -> bool:
+        for guarantee in self.get_guarantees():
+            if isinstance(guarantee, Guarantees.ArgIsNotMutated) and (
+                guarantee.arg_index == name_or_index
+                or guarantee.arg_name == name_or_index
+            ):
+                return False
+
+        return True
+
+
+class MutableFunctionWithTree:
+    def __init__(self, mutable: MutableFunction, root: Instruction = None):
+        self.mutable = mutable
+        self.root = root or mutable.instructions[0]
+
+    def visitor(
+        self, visitor: typing.Callable[[Instruction, typing.List[Instruction]], None]
+    ):
+        def visit(
+            instruction: Instruction,
+            visited: typing.Set[Instruction],
+            path: typing.List[Instruction],
+        ):
+            visitor(instruction, path)
+
+            if instruction in visited:
+                return
+
+            visited.add(instruction)
+
+            if not instruction.has_stop_flow():
+                visit(instruction.next_instruction, visited, path + [instruction])
+
+            if instruction.has_jump():
+                # visit the jump target, but reset the instruction path, as we cannot make sure that
+                # it is the only path leading there
+                # TODO: is there a better way? (first visit the main tree, and than branch?)
+                visit(instruction.arg_value, visited, [instruction])
+
+        visit(self.root, set(), [])
+
+    def print_recursive(self, root: Instruction = None, visited: set = None, level=0):
+        if root is None:
+            print("Starting Dump...")
+            root = self.root
+
+        if visited is None:
+            visited = set()
+        elif root in visited:
+            return
+
+        print(
+            " " * level + repr(root),
+            "-> -1"
+            if root.next_instruction is None
+            else "-> " + str(root.next_instruction.offset),
+        )
+        visited.add(root)
+
+        if root.has_stop_flow():
+            return
+
+        if root.next_instruction is None:
+            print("-" * level, "END OF CONTROL FLOW")
+            return
+
+        self.print_recursive(root.next_instruction, visited, level)
+
+        if root.has_jump():
+            self.print_recursive(root.arg_value, visited, level + 1)
+
+
+def prefix_all_locals_with(
+    mutable: MutableFunction | MutableFunctionWithTree,
+    prefix: str,
+    protected_locals: typing.List[str] = tuple(),
+):
+    if isinstance(mutable, MutableFunctionWithTree):
+        mutable.mutable.assemble_instructions_from_tree(mutable.root)
+        mutable = mutable.mutable
+
+    mutable.shared_variable_names = [
+        prefix + e if e not in protected_locals else e
+        for e in mutable.shared_variable_names
+    ]
+
+    print(mutable.shared_variable_names)
+
+    for instruction in mutable.instructions:
+        if instruction.has_local():
+            instruction.update_owner(mutable, instruction.offset)
+
+
+def replace_opcode_with_other(
+    mutable: MutableFunction | MutableFunctionWithTree,
+    old_opcode: int,
+    new_opcode: int,
+    handle_new: typing.Callable[[Instruction], None] = lambda _: None,
+):
+    if isinstance(mutable, MutableFunctionWithTree):
+        mutable.mutable.assemble_instructions_from_tree(mutable.root)
+        mutable = mutable.mutable
+
+    for instruction in mutable.instructions:
+        if instruction.opcode == old_opcode:
+            instruction.change_opcode(new_opcode)
+
+            handle_new(instruction)
+
+
+def inline_access_to_global(
+    mutable: MutableFunction | MutableFunctionWithTree, global_name: str, value=...
+):
+    if isinstance(mutable, MutableFunctionWithTree):
+        mutable.mutable.assemble_instructions_from_tree(mutable.root)
+        mutable = mutable.mutable
+
+    if value == ...:
+        value = mutable.target.__globals__[global_name]
+
+    for i, instruction in enumerate(mutable.instructions):
+        if instruction.opcode == Opcodes.LOAD_GLOBAL:
+            if instruction.arg_value == global_name:
+                instruction.change_opcode(Opcodes.LOAD_CONST)
+                instruction.change_arg_value(value)
+
+
+def replace_const_func_call_with_opcode(
+    mutable: MutableFunctionWithTree,
+    func: typing.Callable,
+    opcode: int,
+    handle_args: typing.Callable[
+        [MutableFunctionWithTree, Instruction, typing.List[Instruction]], bool
+    ],
+):
+    def visitor(instruction: Instruction, path: typing.List[Instruction]):
+        if instruction.opcode == Opcodes.CALL_FUNCTION:
+            counter = instruction.arg
+            args = path[-counter:]
+            load_method = path[-counter - 1]
+
+            if (
+                load_method.opcode == Opcodes.LOAD_CONST
+                and load_method.arg_value == func
+                and all(instr.opcode == Opcodes.LOAD_CONST for instr in args)
+            ):
+                instruction.change_opcode(opcode)
+                if not handle_args(mutable, instruction, args):
+                    instruction.change_opcode(Opcodes.CALL_FUNCTION)
+
+    mutable.visitor(visitor)
+
+
+def capture_local(name: str):
+    pass
+
+
+def outer_return(value=None):
+    pass
+
+
+def _inline_capture_local(
+    tree: MutableFunctionWithTree,
+    instruction: Instruction,
+    args: typing.List[Instruction],
+) -> bool:
+    if len(args) != 1:
+        return False
+    if args[0].opcode != Opcodes.LOAD_CONST:
+        return False
+
+    instruction.arg = args[0].arg
+    instruction.arg_value = args[0].arg_value
+    args[0].change_opcode(Opcodes.NOP)
+    args[0].arg = 0
+    args[0].arg_value = None
+
+    return True
+
+
+def _inline_outer_return(
+    tree: MutableFunctionWithTree,
+    instruction: Instruction,
+    args: typing.List[Instruction],
+) -> bool:
+    if len(args) > 1:
+        return False
+    if len(args) > 0 and args[0].opcode != Opcodes.LOAD_CONST:
+        return False
+
+    # In case we have no args, we need to add a LOAD_CONST(None)
+    if len(args) == 0:
+        instruction.change_opcode(Opcodes.LOAD_CONST)
+        instruction.change_arg_value(None)
+        return_instr = Instruction.create(Opcodes.RETURN_VALUE)
+        return_instr.update_owner(tree.mutable, -1)
+        return_instr.next_instruction = instruction.next_instruction
+        instruction.next_instruction = return_instr
+
+    return True
+
+
+def insert_method_into(
+    body: MutableFunction | MutableFunctionWithTree,
+    offset: typing.Union[Instruction, int],
+    to_insert: MutableFunction | MutableFunctionWithTree,
+    protected_locals: typing.List[str] = tuple(),
+):
+    """
+    Inserts the function AFTER the given offset / Instruction.
+    If wanted at HEAD, set offset to -1
+    """
+
+    if isinstance(to_insert, MutableFunctionWithTree):
+        to_insert.mutable.assemble_instructions_from_tree(to_insert.root)
+        to_insert = to_insert.mutable
+
+    if not isinstance(body, MutableFunctionWithTree):
+        body = MutableFunctionWithTree(body)
+
+    if offset == -1:
+        HEAD_INSTRUCTION = Instruction.create("NOP")
+        HEAD_INSTRUCTION.function = body.mutable
+        HEAD_INSTRUCTION.next_instruction = body.root
+        body.root = HEAD_INSTRUCTION
+    elif isinstance(offset, int):
+        body.mutable.assemble_instructions_from_tree(body.root)
+        HEAD_INSTRUCTION = body.mutable.instructions[offset]
+    else:
+        HEAD_INSTRUCTION = offset
+
+    for instr in to_insert.instructions:
+        instr.offset = -1
+
+    prefix_all_locals_with(to_insert, to_insert.function_name + ":", protected_locals)
+    replace_opcode_with_other(
+        to_insert, Opcodes.RETURN_VALUE, Opcodes.INTERMEDIATE_INNER_RETURN
+    )
+    inline_access_to_global(to_insert, "capture_local", capture_local)
+    inline_access_to_global(to_insert, "outer_return", outer_return)
+
+    # MutableFunctionWithTree(to_insert).print_recursive()
+
+    instr = None
+    previous = None
+    for instr in to_insert.instructions:
+        if previous is not None:
+            previous.next_instruction = instr
+
+        if instr.opcode == Opcodes.INTERMEDIATE_INNER_RETURN:
+            previous.next_instruction = Instruction.create(Opcodes.POP_TOP)
+            previous.next_instruction.update_owner(to_insert, -1)
+            previous.next_instruction.next_instruction = instr
+
+            instr.change_opcode(Opcodes.JUMP_ABSOLUTE)
+            instr.change_arg_value(HEAD_INSTRUCTION.next_instruction)
+
+        previous = instr
+
+    if instr is not None and instr.next_instruction is None:
+        instr.next_instruction = HEAD_INSTRUCTION.next_instruction
+
+    to_insert.assemble_instructions_from_tree(
+        to_insert.instructions[0],
+        breaks_flow=(
+            Instruction.create(
+                Opcodes.JUMP_ABSOLUTE, HEAD_INSTRUCTION.next_instruction
+            ),
+        ),
+    )
+    # MutableFunctionWithTree(to_insert).print_recursive()
+    # to_insert.decode_instructions()
+
+    for instr in to_insert.instructions:
+        instr.update_owner(body.mutable, -1, False)
+
+    to_insert_tree = MutableFunctionWithTree(to_insert)
+    # to_insert_tree.print_recursive()
+    replace_const_func_call_with_opcode(
+        to_insert_tree,
+        capture_local,
+        Opcodes.LOAD_FAST,
+        _inline_capture_local,
+    )
+    # to_insert_tree.print_recursive()
+    replace_const_func_call_with_opcode(
+        to_insert_tree,
+        outer_return,
+        Opcodes.RETURN_VALUE,
+        _inline_outer_return,
+    )
+    # to_insert_tree.print_recursive()
+
+    def visit(instruction: Instruction, path):
+        if instruction is None:
+            print(path)
+            raise
+
+        instruction.function = body.mutable
+
+        if instruction.has_constant():
+            instruction.arg = body.mutable.allocate_shared_constant(
+                instruction.arg_value
+            )
+
+        elif instruction.has_name():
+            instruction.arg = body.mutable.allocate_shared_name(instruction.arg_value)
+
+        elif instruction.has_local():
+            instruction.arg = body.mutable.allocate_shared_variable_name(
+                instruction.arg_value
+            )
+
+    HEAD_INSTRUCTION.next_instruction = to_insert_tree.root
+    body.visitor(visit)
+
+    # body.print_recursive()
+
+    body.mutable.assemble_instructions_from_tree(body.root)
+
+    # body.print_recursive()
```

### Comparing `bytecodemanipulation-0.2.4/bytecodemanipulation/Opcodes.py` & `bytecodemanipulation-0.2.8/bytecodemanipulation/Opcodes.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,218 +1,223 @@
-import typing
-
-
-class Opcodes:
-    POP_TOP = 1
-    ROT_TWO = 2
-    ROT_THREE = 3
-    DUP_TOP = 4
-    DUP_TOP_TWO = 5
-    ROT_FOUR = 6
-
-    NOP = 9
-    UNARY_POSITIVE = 10
-    UNARY_NEGATIVE = 11
-    UNARY_NOT = 12
-
-    UNARY_INVERT = 15
-    BINARY_MATRIX_MULTIPLY = 16
-    INPLACE_MATRIX_MULTIPLY = 17
-
-    BINARY_POWER = 19
-    BINARY_MULTIPLY = 20
-
-    BINARY_MODULO = 22
-    BINARY_ADD = 23
-    BINARY_SUBTRACT = 24
-    BINARY_SUBSCR = 25
-    BINARY_FLOOR_DIVIDE = 26
-    BINARY_TRUE_DIVIDE = 27
-    INPLACE_FLOOR_DIVIDE = 28
-    INPLACE_TRUE_DIVIDE = 29
-    GET_LEN = 30
-    MATCH_MAPPING = 31
-    MATCH_SEQUENCE = 32
-    MATCH_KEYS = 33
-    COPY_DICT_WITHOUT_KEYS = 34
-
-    WITH_EXCEPT_START = 49
-    GET_AITER = 50
-    GET_ANEXT = 51
-    BEFORE_ASYNC_WITH = 52
-
-    END_ASYNC_FOR = 54
-    INPLACE_ADD = 55
-    INPLACE_SUBTRACT = 56
-    INPLACE_MULTIPLY = 57
-
-    INPLACE_MODULO = 59
-    STORE_SUBSCR = 60
-    DELETE_SUBSCR = 61
-    BINARY_LSHIFT = 62
-    BINARY_RSHIFT = 63
-    BINARY_AND = 64
-    BINARY_XOR = 65
-    BINARY_OR = 66
-    INPLACE_POWER = 67
-    GET_ITER = 68
-    GET_YIELD_FROM_ITER = 69
-    PRINT_EXPR = 70
-    LOAD_BUILD_CLASS = 71
-    YIELD_FROM = 72
-    GET_AWAITABLE = 73
-    LOAD_ASSERTION_ERROR = 74
-    INPLACE_LSHIFT = 75
-    INPLACE_RSHIFT = 76
-    INPLACE_AND = 77
-    INPLACE_XOR = 78
-    INPLACE_OR = 79
-
-    LIST_TO_TUPLE = 82
-    RETURN_VALUE = 83
-    IMPORT_STAR = 84
-    SETUP_ANNOTATIONS = 85
-    YIELD_VALUE = 86
-    POP_BLOCK = 87
-
-    POP_EXCEPT = 89
-
-    HAVE_ARGUMENT = 90  # Opcodes from here have an argument:
-
-    STORE_NAME = 90  # Index in name list
-    DELETE_NAME = 91  # ""
-    UNPACK_SEQUENCE = 92  # Number of tuple items
-    FOR_ITER = 93
-    UNPACK_EX = 94
-    STORE_ATTR = 95  # Index in name list
-    DELETE_ATTR = 96  # ""
-    STORE_GLOBAL = 97  # ""
-    DELETE_GLOBAL = 98  # ""
-    ROT_N = 99
-    LOAD_CONST = 100  # Index in const list
-    LOAD_NAME = 101  # Index in name list
-    BUILD_TUPLE = 102  # Number of tuple items
-    BUILD_LIST = 103  # Number of list items
-    BUILD_SET = 104  # Number of set items
-    BUILD_MAP = 105  # Number of dict entries
-    LOAD_ATTR = 106  # Index in name list
-    COMPARE_OP = 107  # Comparison operator
-    IMPORT_NAME = 108  # Index in name list
-    IMPORT_FROM = 109  # Index in name list
-    JUMP_FORWARD = 110  # Number of bytes to skip
-    JUMP_IF_FALSE_OR_POP = 111  # Target byte offset from beginning of code
-    JUMP_IF_TRUE_OR_POP = 112  # ""
-    JUMP_ABSOLUTE = 113  # ""
-    POP_JUMP_IF_FALSE = 114  # ""
-    POP_JUMP_IF_TRUE = 115  # ""
-    LOAD_GLOBAL = 116  # Index in name list
-    IS_OP = 117
-    CONTAINS_OP = 118
-    RERAISE = 119
-
-    JUMP_IF_NOT_EXC_MATCH = 121
-    SETUP_FINALLY = 122  # Distance to target address
-
-    LOAD_FAST = 124  # Local variable number
-    STORE_FAST = 125  # Local variable number
-    DELETE_FAST = 126  # Local variable number
-
-    GEN_START = 129  # Kind of generator/coroutine
-    RAISE_VARARGS = 130  # Number of raise arguments (1, 2, or 3
-    CALL_FUNCTION = 131  # #args
-    MAKE_FUNCTION = 132  # Flags
-    BUILD_SLICE = 133  # Number of items
-
-    LOAD_CLOSURE = 135
-    LOAD_DEREF = 136
-    STORE_DEREF = 137
-    DELETE_DEREF = 138
-
-    CALL_FUNCTION_KW = 141  # #args + #kwargs
-    CALL_FUNCTION_EX = 142  # Flags
-    SETUP_WITH = 143
-    EXTENDED_ARG = 144
-    LIST_APPEND = 145
-    SET_ADD = 146
-    MAP_ADD = 147
-    LOAD_CLASSDEREF = 148
-
-    MATCH_CLASS = 152
-
-    SETUP_ASYNC_WITH = 154
-    FORMAT_VALUE = 155
-    BUILD_CONST_KEY_MAP = 156
-    BUILD_STRING = 157
-
-    LOAD_METHOD = 160
-    CALL_METHOD = 161
-    LIST_EXTEND = 162
-    SET_UPDATE = 163
-    DICT_MERGE = 164
-    DICT_UPDATE = 165
-
-    # Since python 3.11
-    CACHE = 166
-    PUSH_NULL = 167
-    PUSH_EXC_INFO = 168
-    CHECK_EXC_MATCH = 169
-    CHECK_EG_MATCH = 170
-    BEFORE_WITH = 171
-    RETURN_GENERATOR = 172
-    ASYNC_GEN_WRAP = 173
-    PREP_RERAISE_STAR = 174
-    SWAP = 175
-    POP_JUMP_FORWARD_IF_FALSE = 176
-    POP_JUMP_FORWARD_IF_TRUE = 177
-    COPY = 178
-    BINARY_OP = 179
-    SEND = 180
-    POP_JUMP_FORWARD_IF_NOT_NONE = 181
-    POP_JUMP_FORWARD_IF_NONE = 182
-    JUMP_BACKWARD_NO_INTERRUPT = 183
-    MAKE_CELL = 184
-    JUMP_BACKWARD = 185
-    COPY_FREE_VARS = 186
-    RESUME = 187
-    PRECALL = 188
-    CALL = 189
-    KW_NAMES = 190
-    POP_JUMP_BACKWARD_IF_NOT_NONE = 191
-    POP_JUMP_BACKWARD_IF_NONE = 192
-    POP_JUMP_BACKWARD_IF_FALSE = 193
-    POP_JUMP_BACKWARD_IF_TRUE = 194
-
-    INTERMEDIATE_INNER_RETURN = 256
-    INTERMEDIATE_OUTER_RETURN = 257
-    INTERMEDIATE_LOAD_FAST = 258
-    BYTECODE_LABEL = 259
-    MACRO_PARAMETER_EXPANSION = 260
-    STATIC_ATTRIBUTE_ACCESS = 261
-
-
-OPCODE2NAME = {}
-OPNAME2CODE = {}
-
-
-def init_maps():
-    OPNAME2CODE.clear()
-    OPCODE2NAME.clear()
-
-    for key, value in Opcodes.__dict__.items():
-        key: str
-        if key.isupper() and isinstance(value, int):
-            OPNAME2CODE[key] = value
-            OPCODE2NAME[value] = key
-
-
-END_CONTROL_FLOW: typing.List[int] = []
-HAS_NAME: typing.List[int] = []
-HAS_GLOBAL: typing.List[int] = []
-HAS_CONST: typing.List[int] = []
-HAS_LOCAL: typing.List[int] = []
-HAS_JUMP_ABSOLUTE: typing.List[int] = []
-HAS_JUMP_FORWARD: typing.List[int] = []
-HAS_JUMP_BACKWARDS: typing.List[int] = []
-UNCONDITIONAL_JUMPS: typing.List[int] = []
-HAS_CELL_VARIABLE: typing.List[int] = []
-
-SIDE_EFFECT_FREE_LOADS: typing.List[int] = []
+import sys
+import typing
+
+
+class Opcodes:
+    POP_TOP = 1
+    ROT_TWO = 2
+    ROT_THREE = 3
+    DUP_TOP = 4
+    DUP_TOP_TWO = 5
+    ROT_FOUR = 6
+
+    NOP = 9
+    UNARY_POSITIVE = 10
+    UNARY_NEGATIVE = 11
+    UNARY_NOT = 12
+
+    UNARY_INVERT = 15
+    BINARY_MATRIX_MULTIPLY = 16
+    INPLACE_MATRIX_MULTIPLY = 17
+
+    BINARY_POWER = 19
+    BINARY_MULTIPLY = 20
+
+    BINARY_MODULO = 22
+    BINARY_ADD = 23
+    BINARY_SUBTRACT = 24
+    BINARY_SUBSCR = 25
+    BINARY_FLOOR_DIVIDE = 26
+    BINARY_TRUE_DIVIDE = 27
+    INPLACE_FLOOR_DIVIDE = 28
+    INPLACE_TRUE_DIVIDE = 29
+    GET_LEN = 30
+    MATCH_MAPPING = 31
+    MATCH_SEQUENCE = 32
+    MATCH_KEYS = 33
+    COPY_DICT_WITHOUT_KEYS = 34
+
+    WITH_EXCEPT_START = 49
+    GET_AITER = 50
+    GET_ANEXT = 51
+    BEFORE_ASYNC_WITH = 52
+
+    END_ASYNC_FOR = 54
+    INPLACE_ADD = 55
+    INPLACE_SUBTRACT = 56
+    INPLACE_MULTIPLY = 57
+
+    INPLACE_MODULO = 59
+    STORE_SUBSCR = 60
+    DELETE_SUBSCR = 61
+    BINARY_LSHIFT = 62
+    BINARY_RSHIFT = 63
+    BINARY_AND = 64
+    BINARY_XOR = 65
+    BINARY_OR = 66
+    INPLACE_POWER = 67
+    GET_ITER = 68
+    GET_YIELD_FROM_ITER = 69
+    PRINT_EXPR = 70
+    LOAD_BUILD_CLASS = 71
+    YIELD_FROM = 72
+    GET_AWAITABLE = 73
+    LOAD_ASSERTION_ERROR = 74
+    INPLACE_LSHIFT = 75
+    INPLACE_RSHIFT = 76
+    INPLACE_AND = 77
+    INPLACE_XOR = 78
+    INPLACE_OR = 79
+
+    LIST_TO_TUPLE = 82
+    RETURN_VALUE = 83
+    IMPORT_STAR = 84
+    SETUP_ANNOTATIONS = 85
+    YIELD_VALUE = 86
+    POP_BLOCK = 87
+
+    POP_EXCEPT = 89
+
+    HAVE_ARGUMENT = 90  # Opcodes from here have an argument:
+
+    STORE_NAME = 90  # Index in name list
+    DELETE_NAME = 91  # ""
+    UNPACK_SEQUENCE = 92  # Number of tuple items
+    FOR_ITER = 93
+    UNPACK_EX = 94
+    STORE_ATTR = 95  # Index in name list
+    DELETE_ATTR = 96  # ""
+    STORE_GLOBAL = 97  # ""
+    DELETE_GLOBAL = 98  # ""
+    ROT_N = 99
+    LOAD_CONST = 100  # Index in const list
+    LOAD_NAME = 101  # Index in name list
+    BUILD_TUPLE = 102  # Number of tuple items
+    BUILD_LIST = 103  # Number of list items
+    BUILD_SET = 104  # Number of set items
+    BUILD_MAP = 105  # Number of dict entries
+    LOAD_ATTR = 106  # Index in name list
+    COMPARE_OP = 107  # Comparison operator
+    IMPORT_NAME = 108  # Index in name list
+    IMPORT_FROM = 109  # Index in name list
+    JUMP_FORWARD = 110  # Number of bytes to skip
+    JUMP_IF_FALSE_OR_POP = 111  # Target byte offset from beginning of code
+    JUMP_IF_TRUE_OR_POP = 112  # ""
+    JUMP_ABSOLUTE = 113  # ""
+    POP_JUMP_IF_FALSE = 114  # ""
+    POP_JUMP_IF_TRUE = 115  # ""
+    LOAD_GLOBAL = 116  # Index in name list
+    IS_OP = 117
+    CONTAINS_OP = 118
+    RERAISE = 119
+
+    JUMP_IF_NOT_EXC_MATCH = 121
+    SETUP_FINALLY = 122  # Distance to target address
+
+    LOAD_FAST = 124  # Local variable number
+    STORE_FAST = 125  # Local variable number
+    DELETE_FAST = 126  # Local variable number
+
+    GEN_START = 129  # Kind of generator/coroutine
+    RAISE_VARARGS = 130  # Number of raise arguments (1, 2, or 3
+    CALL_FUNCTION = 131  # #args
+    MAKE_FUNCTION = 132  # Flags
+    BUILD_SLICE = 133  # Number of items
+
+    LOAD_CLOSURE = 135
+    LOAD_DEREF = 136
+    STORE_DEREF = 137
+    DELETE_DEREF = 138
+
+    CALL_FUNCTION_KW = 141  # #args + #kwargs
+    CALL_FUNCTION_EX = 142  # Flags
+    SETUP_WITH = 143
+    EXTENDED_ARG = 144
+    LIST_APPEND = 145
+    SET_ADD = 146
+    MAP_ADD = 147
+    LOAD_CLASSDEREF = 148
+
+    MATCH_CLASS = 152
+
+    SETUP_ASYNC_WITH = 154
+    FORMAT_VALUE = 155
+    BUILD_CONST_KEY_MAP = 156
+    BUILD_STRING = 157
+
+    LOAD_METHOD = 160
+    CALL_METHOD = 161
+    LIST_EXTEND = 162
+    SET_UPDATE = 163
+    DICT_MERGE = 164
+    DICT_UPDATE = 165
+
+    # Since python 3.11
+    if sys.version_info.minor >= 11 or typing.TYPE_CHECKING:
+        CACHE = 166
+        PUSH_NULL = 167
+        PUSH_EXC_INFO = 168
+        CHECK_EXC_MATCH = 169
+        CHECK_EG_MATCH = 170
+        BEFORE_WITH = 171
+        RETURN_GENERATOR = 172
+        ASYNC_GEN_WRAP = 173
+        PREP_RERAISE_STAR = 174
+        SWAP = 175
+        POP_JUMP_FORWARD_IF_FALSE = 176
+        POP_JUMP_FORWARD_IF_TRUE = 177
+        COPY = 178
+        BINARY_OP = 179
+        SEND = 180
+        POP_JUMP_FORWARD_IF_NOT_NONE = 181
+        POP_JUMP_FORWARD_IF_NONE = 182
+        JUMP_BACKWARD_NO_INTERRUPT = 183
+        MAKE_CELL = 184
+        JUMP_BACKWARD = 185
+        COPY_FREE_VARS = 186
+        RESUME = 187
+        PRECALL = 188
+        CALL = 189
+        KW_NAMES = 190
+        POP_JUMP_BACKWARD_IF_NOT_NONE = 191
+        POP_JUMP_BACKWARD_IF_NONE = 192
+        POP_JUMP_BACKWARD_IF_FALSE = 193
+        POP_JUMP_BACKWARD_IF_TRUE = 194
+
+    INTERMEDIATE_INNER_RETURN = 256
+    INTERMEDIATE_OUTER_RETURN = 257
+    INTERMEDIATE_LOAD_FAST = 258
+    BYTECODE_LABEL = 259
+    MACRO_PARAMETER_EXPANSION = 260
+    STATIC_ATTRIBUTE_ACCESS = 261
+    MACRO_RETURN_VALUE = 262
+    MACRO_LOAD_PARAMETER = 263
+    MACRO_STORE_PARAMETER = 264
+
+
+OPCODE2NAME = {}
+OPNAME2CODE = {}
+
+
+def init_maps():
+    OPNAME2CODE.clear()
+    OPCODE2NAME.clear()
+
+    for key, value in Opcodes.__dict__.items():
+        key: str
+        if key.isupper() and isinstance(value, int):
+            OPNAME2CODE[key] = value
+            OPCODE2NAME[value] = key
+
+
+END_CONTROL_FLOW: typing.List[int] = []
+HAS_NAME: typing.List[int] = []
+HAS_GLOBAL: typing.List[int] = []
+HAS_CONST: typing.List[int] = []
+HAS_LOCAL: typing.List[int] = []
+HAS_JUMP_ABSOLUTE: typing.List[int] = []
+HAS_JUMP_FORWARD: typing.List[int] = []
+HAS_JUMP_BACKWARDS: typing.List[int] = []
+UNCONDITIONAL_JUMPS: typing.List[int] = []
+HAS_CELL_VARIABLE: typing.List[int] = []
+
+SIDE_EFFECT_FREE_LOADS: typing.List[int] = []
```

### Comparing `bytecodemanipulation-0.2.4/bytecodemanipulation/Specialization.py` & `bytecodemanipulation-0.2.8/bytecodemanipulation/Specialization.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,326 +1,326 @@
-import typing
-import warnings
-
-from bytecodemanipulation.MutableFunction import Instruction
-from bytecodemanipulation.MutableFunction import MutableFunction
-from bytecodemanipulation.Opcodes import Opcodes
-
-
-class TypeAnnotation:
-    pass
-
-
-class MethodCallDescriptor:
-    def __init__(
-        self,
-        lookup_method_instr: Instruction = None,
-        call_method_instr: Instruction = None,
-    ):
-        self.lookup_method_instr: Instruction = lookup_method_instr
-        self.call_method_instr: Instruction = call_method_instr
-
-
-class ArgDescriptor:
-    def __init__(self, real: Instruction, normal: Instruction, arg_id: int):
-        self.real = real
-        self.normal = normal
-        self.arg_id = arg_id
-        self.is_self = False
-        self.discarded = False
-        self.parent: "SpecializationContainer" = None
-
-    def get_real_data_instr(self) -> Instruction:
-        return self.real
-
-    def get_normalized_data_instr(self) -> Instruction | None:
-        return self.normal
-
-    def get_type_annotation(self) -> TypeAnnotation:
-        pass
-
-    def discard(self):
-        self.discarded = True
-
-        if self.parent:
-            self.parent.no_special = False
-
-    def __repr__(self):
-        return f"ArgDescriptor({self.real}, {self.normal}, {self.arg_id}, {self.discarded})"
-
-
-class SpecializationContainer:
-    def __init__(self):
-        self.underlying_function: typing.Callable | None = None
-        self.target: MutableFunction | None = None
-        self.method_call_descriptor: MethodCallDescriptor | None = None
-        self.arg_descriptors: typing.List[ArgDescriptor] = []
-        self.return_type_annotation: TypeAnnotation | None = None
-
-        self.no_special = True
-        self.result_arg: ArgDescriptor | None = None
-        self.replaced_call_target: typing.Callable | None = None
-        self.replace_raised_exception: Exception | None = None
-        self.constant_value = tuple()
-        self.invoke_before: typing.Callable | None = None
-        self.replacement_bytecode = None
-
-    def set_arg_descriptors(self, descriptors: typing.List[ArgDescriptor]):
-        for e in descriptors:
-            e.parent = self
-
-        self.arg_descriptors[:] = descriptors
-
-    def get_arg_specification(self, arg: int) -> ArgDescriptor:
-        return self.arg_descriptors[arg]
-
-    def get_arg_specifications(self) -> typing.List[ArgDescriptor]:
-        return self.arg_descriptors
-
-    def get_return_type(self) -> TypeAnnotation:
-        return self.return_type_annotation
-
-    def replace_with_constant_value(
-        self, value: object, side_effect: typing.Callable[[...], None] = None
-    ):
-
-        if side_effect is None:
-            for arg in self.arg_descriptors:
-                arg.discard()
-
-        self.invoke_before = side_effect
-        self.constant_value = (value,)
-        return self
-
-    def replace_with_constant_lazy_value(
-        self,
-        value: typing.Callable[[], object],
-        side_effect: typing.Callable[[...], None] = None,
-    ):
-        pass  # todo: implement!
-
-    def replace_with_variant(self, target: typing.Callable[[...], object]):
-        self.replaced_call_target = target
-        self.no_special = False
-        return self
-
-    def replace_with_raise_exception(
-        self,
-        exception: Exception | typing.Callable[[], Exception],
-        side_effect: typing.Callable[[...], None] = None,
-        arg: int = None,
-        stackoffset=0,
-    ):
-        # todo: emit such warnings via the location emitter
-        if self.replace_raised_exception:
-            return
-
-        assert side_effect is None, "not implemented!"
-
-        if not isinstance(exception, Exception):
-            exception = exception()
-
-        warnings.warn(
-            exception.__class__.__name__
-            + ": "
-            + exception.args[0]
-            + (f" [AT ARG {arg}]" if arg is not None else "")
-            + " (Statically emitted)",
-            stacklevel=2 + stackoffset,
-        )
-        self.replace_raised_exception = exception
-
-        for arg in self.arg_descriptors:
-            arg.discard()
-
-        self.no_special = False
-
-        return self
-
-    def replace_with_raise_exception_if(
-        self,
-        predicate: typing.Callable[[], bool] | bool,
-        construct: typing.Callable[[], Exception] | Exception | None,
-        construct_exception_at_runtime=False,
-        side_effect: typing.Callable[[...], Exception | None] = None,
-        side_effect_returns_exception=False,
-        arg: int = None,
-    ) -> bool:
-        """
-        Replaces the call with an 'raise <exception>' iff predicate() evaluated to True
-
-        :param predicate: the predicate to decide on, either bool or callable(->bool)
-        :param construct: the Exception instance, or a callable to get such instance
-        :param construct_exception_at_runtime: if True, 'construct' MUST be a callable, and it is called now
-            each time the exception should be raised, instead of onces ahead of time
-        :param side_effect: a callable to call before raising the exception, for doing side effect magic; args are given
-            directly to the side effect; Discarded args are skipped
-        :param  side_effect_returns_exception: if True, 'side_effect' must be provided, and it must return an Exception,
-            which is then raised
-        :param arg: Optional: the arg the exception is raised for; will be included in the emitted warning
-        :return: the result of the predicate, if possible
-        """
-        if predicate() if callable(predicate) else predicate:
-            self.replace_with_raise_exception(
-                construct, side_effect, arg=arg, stackoffset=1
-            )
-            return True
-        return False
-
-    def replace_call_with_opcodes(
-        self,
-        opcodes: typing.List[Instruction | ArgDescriptor],
-        leave_args_on_stack=False,
-    ):
-        """
-        Replaces the call with a set of instructions.
-        Arguments can be accessed by their arg descriptor as an "instruction".
-        Writing is currently not allowed
-
-        :param opcodes: the opcodes to use, possibly mixed with arg descriptors to access the args to the call;
-            args are de-duplicated, and stored in temporary locals if needed
-        :param leave_args_on_stack: if True, the args of the call will be at the stack top like in a real call; This makes
-            using ArgDescriptor as instructions impossible!
-        """
-
-        if not leave_args_on_stack:
-            # Store values in temporary variables
-            bytecode = [
-                Instruction(
-                    self.target,
-                    -1,
-                    Opcodes.STORE_FAST,
-                    f"&fast_tmp_specialize_local::{i}",
-                )
-                for i in range(self.method_call_descriptor.call_method_instr.arg)
-            ]
-
-            bytecode += [
-                (
-                    instruction.update_owner(self.target, -1)
-                    if isinstance(instruction, Instruction)
-                    else Instruction(
-                        self.target,
-                        -1,
-                        Opcodes.LOAD_FAST,
-                        f"&fast_tmp_specialize_local::{instruction.arg_id}",
-                    )
-                )
-                for instruction in opcodes
-            ]
-        else:
-            bytecode = opcodes
-
-        self.no_special = False
-        self.replacement_bytecode = bytecode
-        return self
-
-    def replace_call_with_arg(self, arg: ArgDescriptor):
-        """
-        Replaces the function call with a constant argument return
-        Automatically discards all other arguments
-        """
-
-        if arg not in self.arg_descriptors:
-            raise ValueError(arg)
-
-        self.no_special = False
-        self.result_arg = arg
-        return self
-
-    def apply(self):
-        if self.no_special:
-            return
-
-        if self.replacement_bytecode is not None:
-            self.method_call_descriptor.call_method_instr.change_opcode(Opcodes.NOP)
-            self.method_call_descriptor.call_method_instr.insert_after(
-                self.replacement_bytecode
-            )
-            self.method_call_descriptor.lookup_method_instr.change_opcode(Opcodes.NOP)
-            return
-
-        if self.result_arg:
-            for arg in self.arg_descriptors:
-                if arg != self.result_arg:
-                    arg.discard()
-
-            self._discard_args()
-            self.method_call_descriptor.lookup_method_instr.change_opcode(Opcodes.NOP)
-            self.method_call_descriptor.call_method_instr.change_opcode(Opcodes.NOP)
-            return
-
-        if self.constant_value != tuple():
-            self._discard_args()
-            arg_count = sum(int(not arg.discarded) for arg in self.arg_descriptors)
-            self.method_call_descriptor.call_method_instr.change_arg(arg_count)
-
-            if self.invoke_before:
-                self.method_call_descriptor.lookup_method_instr.change_opcode(
-                    Opcodes.LOAD_CONST
-                )
-                self.method_call_descriptor.lookup_method_instr.change_arg_value(
-                    self.invoke_before
-                )
-                self.method_call_descriptor.call_method_instr.change_arg(arg_count)
-
-                self.method_call_descriptor.call_method_instr.insert_after(
-                    Instruction(
-                        self.underlying_function, -1, opcode_or_name=Opcodes.POP_TOP
-                    ),
-                    Instruction(
-                        self.underlying_function,
-                        -1,
-                        opcode_or_name=Opcodes.LOAD_CONST,
-                        arg_value=self.constant_value[0],
-                    ),
-                )
-
-            else:
-                self.method_call_descriptor.lookup_method_instr.change_opcode(
-                    Opcodes.NOP
-                )
-                self.method_call_descriptor.call_method_instr.change_opcode(
-                    Opcodes.LOAD_CONST
-                )
-                self.method_call_descriptor.call_method_instr.change_arg_value(
-                    self.constant_value[0]
-                )
-
-            return
-
-        self._discard_args()
-        arg_count = sum(int(not arg.discarded) for arg in self.arg_descriptors)
-        self.method_call_descriptor.call_method_instr.change_arg(arg_count)
-
-        if self.replace_raised_exception:
-            self.method_call_descriptor.lookup_method_instr.change_opcode(
-                Opcodes.LOAD_CONST,
-                self.replace_raised_exception,
-            )
-            self.method_call_descriptor.call_method_instr.change_opcode(
-                Opcodes.RAISE_VARARGS,
-            )
-            self.method_call_descriptor.call_method_instr.change_arg(1)
-
-        elif self.replaced_call_target is not None:
-            self.method_call_descriptor.lookup_method_instr.change_opcode(
-                Opcodes.LOAD_CONST,
-                self.replaced_call_target,
-            )
-
-    def _discard_args(self):
-        for arg in self.arg_descriptors:
-            if arg.discarded:
-                # todo: safe-guard when multi-use
-                arg.get_real_data_instr().change_opcode(Opcodes.NOP)
-
-
-def register(target: typing.Callable):
-    def annotation(special: typing.Callable[[SpecializationContainer], None]):
-        from bytecodemanipulation.Optimiser import _OptimisationContainer
-
-        _OptimisationContainer.get_for_target(target).specializations.append(special)
-
-        return special
-
-    return annotation
+import typing
+import warnings
+
+from bytecodemanipulation.MutableFunction import Instruction
+from bytecodemanipulation.MutableFunction import MutableFunction
+from bytecodemanipulation.Opcodes import Opcodes
+
+
+class TypeAnnotation:
+    pass
+
+
+class MethodCallDescriptor:
+    def __init__(
+        self,
+        lookup_method_instr: Instruction = None,
+        call_method_instr: Instruction = None,
+    ):
+        self.lookup_method_instr: Instruction = lookup_method_instr
+        self.call_method_instr: Instruction = call_method_instr
+
+
+class ArgDescriptor:
+    def __init__(self, real: Instruction, normal: Instruction, arg_id: int):
+        self.real = real
+        self.normal = normal
+        self.arg_id = arg_id
+        self.is_self = False
+        self.discarded = False
+        self.parent: "SpecializationContainer" = None
+
+    def get_real_data_instr(self) -> Instruction:
+        return self.real
+
+    def get_normalized_data_instr(self) -> Instruction | None:
+        return self.normal
+
+    def get_type_annotation(self) -> TypeAnnotation:
+        pass
+
+    def discard(self):
+        self.discarded = True
+
+        if self.parent:
+            self.parent.no_special = False
+
+    def __repr__(self):
+        return f"ArgDescriptor({self.real}, {self.normal}, {self.arg_id}, {self.discarded})"
+
+
+class SpecializationContainer:
+    def __init__(self):
+        self.underlying_function: typing.Callable | None = None
+        self.target: MutableFunction | None = None
+        self.method_call_descriptor: MethodCallDescriptor | None = None
+        self.arg_descriptors: typing.List[ArgDescriptor] = []
+        self.return_type_annotation: TypeAnnotation | None = None
+
+        self.no_special = True
+        self.result_arg: ArgDescriptor | None = None
+        self.replaced_call_target: typing.Callable | None = None
+        self.replace_raised_exception: Exception | None = None
+        self.constant_value = tuple()
+        self.invoke_before: typing.Callable | None = None
+        self.replacement_bytecode = None
+
+    def set_arg_descriptors(self, descriptors: typing.List[ArgDescriptor]):
+        for e in descriptors:
+            e.parent = self
+
+        self.arg_descriptors[:] = descriptors
+
+    def get_arg_specification(self, arg: int) -> ArgDescriptor:
+        return self.arg_descriptors[arg]
+
+    def get_arg_specifications(self) -> typing.List[ArgDescriptor]:
+        return self.arg_descriptors
+
+    def get_return_type(self) -> TypeAnnotation:
+        return self.return_type_annotation
+
+    def replace_with_constant_value(
+        self, value: object, side_effect: typing.Callable[[...], None] = None
+    ):
+
+        if side_effect is None:
+            for arg in self.arg_descriptors:
+                arg.discard()
+
+        self.invoke_before = side_effect
+        self.constant_value = (value,)
+        return self
+
+    def replace_with_constant_lazy_value(
+        self,
+        value: typing.Callable[[], object],
+        side_effect: typing.Callable[[...], None] = None,
+    ):
+        pass  # todo: implement!
+
+    def replace_with_variant(self, target: typing.Callable[[...], object]):
+        self.replaced_call_target = target
+        self.no_special = False
+        return self
+
+    def replace_with_raise_exception(
+        self,
+        exception: Exception | typing.Callable[[], Exception],
+        side_effect: typing.Callable[[...], None] = None,
+        arg: int = None,
+        stackoffset=0,
+    ):
+        # todo: emit such warnings via the location emitter
+        if self.replace_raised_exception:
+            return
+
+        assert side_effect is None, "not implemented!"
+
+        if not isinstance(exception, Exception):
+            exception = exception()
+
+        warnings.warn(
+            exception.__class__.__name__
+            + ": "
+            + exception.args[0]
+            + (f" [AT ARG {arg}]" if arg is not None else "")
+            + " (Statically emitted)",
+            stacklevel=2 + stackoffset,
+        )
+        self.replace_raised_exception = exception
+
+        for arg in self.arg_descriptors:
+            arg.discard()
+
+        self.no_special = False
+
+        return self
+
+    def replace_with_raise_exception_if(
+        self,
+        predicate: typing.Callable[[], bool] | bool,
+        construct: typing.Callable[[], Exception] | Exception | None,
+        construct_exception_at_runtime=False,
+        side_effect: typing.Callable[[...], Exception | None] = None,
+        side_effect_returns_exception=False,
+        arg: int = None,
+    ) -> bool:
+        """
+        Replaces the call with an 'raise <exception>' iff predicate() evaluated to True
+
+        :param predicate: the predicate to decide on, either bool or callable(->bool)
+        :param construct: the Exception instance, or a callable to get such instance
+        :param construct_exception_at_runtime: if True, 'construct' MUST be a callable, and it is called now
+            each time the exception should be raised, instead of onces ahead of time
+        :param side_effect: a callable to call before raising the exception, for doing side effect magic; args are given
+            directly to the side effect; Discarded args are skipped
+        :param  side_effect_returns_exception: if True, 'side_effect' must be provided, and it must return an Exception,
+            which is then raised
+        :param arg: Optional: the arg the exception is raised for; will be included in the emitted warning
+        :return: the result of the predicate, if possible
+        """
+        if predicate() if callable(predicate) else predicate:
+            self.replace_with_raise_exception(
+                construct, side_effect, arg=arg, stackoffset=1
+            )
+            return True
+        return False
+
+    def replace_call_with_opcodes(
+        self,
+        opcodes: typing.List[Instruction | ArgDescriptor],
+        leave_args_on_stack=False,
+    ):
+        """
+        Replaces the call with a set of instructions.
+        Arguments can be accessed by their arg descriptor as an "instruction".
+        Writing is currently not allowed
+
+        :param opcodes: the opcodes to use, possibly mixed with arg descriptors to access the args to the call;
+            args are de-duplicated, and stored in temporary locals if needed
+        :param leave_args_on_stack: if True, the args of the call will be at the stack top like in a real call; This makes
+            using ArgDescriptor as instructions impossible!
+        """
+
+        if not leave_args_on_stack:
+            # Store values in temporary variables
+            bytecode = [
+                Instruction(
+                    self.target,
+                    -1,
+                    Opcodes.STORE_FAST,
+                    f"&fast_tmp_specialize_local::{i}",
+                )
+                for i in range(self.method_call_descriptor.call_method_instr.arg)
+            ]
+
+            bytecode += [
+                (
+                    instruction.update_owner(self.target, -1)
+                    if isinstance(instruction, Instruction)
+                    else Instruction(
+                        self.target,
+                        -1,
+                        Opcodes.LOAD_FAST,
+                        f"&fast_tmp_specialize_local::{instruction.arg_id}",
+                    )
+                )
+                for instruction in opcodes
+            ]
+        else:
+            bytecode = opcodes
+
+        self.no_special = False
+        self.replacement_bytecode = bytecode
+        return self
+
+    def replace_call_with_arg(self, arg: ArgDescriptor):
+        """
+        Replaces the function call with a constant argument return
+        Automatically discards all other arguments
+        """
+
+        if arg not in self.arg_descriptors:
+            raise ValueError(arg)
+
+        self.no_special = False
+        self.result_arg = arg
+        return self
+
+    def apply(self):
+        if self.no_special:
+            return
+
+        if self.replacement_bytecode is not None:
+            self.method_call_descriptor.call_method_instr.change_opcode(Opcodes.NOP)
+            self.method_call_descriptor.call_method_instr.insert_after(
+                self.replacement_bytecode
+            )
+            self.method_call_descriptor.lookup_method_instr.change_opcode(Opcodes.NOP)
+            return
+
+        if self.result_arg:
+            for arg in self.arg_descriptors:
+                if arg != self.result_arg:
+                    arg.discard()
+
+            self._discard_args()
+            self.method_call_descriptor.lookup_method_instr.change_opcode(Opcodes.NOP)
+            self.method_call_descriptor.call_method_instr.change_opcode(Opcodes.NOP)
+            return
+
+        if self.constant_value != tuple():
+            self._discard_args()
+            arg_count = sum(int(not arg.discarded) for arg in self.arg_descriptors)
+            self.method_call_descriptor.call_method_instr.change_arg(arg_count)
+
+            if self.invoke_before:
+                self.method_call_descriptor.lookup_method_instr.change_opcode(
+                    Opcodes.LOAD_CONST
+                )
+                self.method_call_descriptor.lookup_method_instr.change_arg_value(
+                    self.invoke_before
+                )
+                self.method_call_descriptor.call_method_instr.change_arg(arg_count)
+
+                self.method_call_descriptor.call_method_instr.insert_after(
+                    Instruction(
+                        self.underlying_function, -1, opcode_or_name=Opcodes.POP_TOP
+                    ),
+                    Instruction(
+                        self.underlying_function,
+                        -1,
+                        opcode_or_name=Opcodes.LOAD_CONST,
+                        arg_value=self.constant_value[0],
+                    ),
+                )
+
+            else:
+                self.method_call_descriptor.lookup_method_instr.change_opcode(
+                    Opcodes.NOP
+                )
+                self.method_call_descriptor.call_method_instr.change_opcode(
+                    Opcodes.LOAD_CONST
+                )
+                self.method_call_descriptor.call_method_instr.change_arg_value(
+                    self.constant_value[0]
+                )
+
+            return
+
+        self._discard_args()
+        arg_count = sum(int(not arg.discarded) for arg in self.arg_descriptors)
+        self.method_call_descriptor.call_method_instr.change_arg(arg_count)
+
+        if self.replace_raised_exception:
+            self.method_call_descriptor.lookup_method_instr.change_opcode(
+                Opcodes.LOAD_CONST,
+                self.replace_raised_exception,
+            )
+            self.method_call_descriptor.call_method_instr.change_opcode(
+                Opcodes.RAISE_VARARGS,
+            )
+            self.method_call_descriptor.call_method_instr.change_arg(1)
+
+        elif self.replaced_call_target is not None:
+            self.method_call_descriptor.lookup_method_instr.change_opcode(
+                Opcodes.LOAD_CONST,
+                self.replaced_call_target,
+            )
+
+    def _discard_args(self):
+        for arg in self.arg_descriptors:
+            if arg.discarded:
+                # todo: safe-guard when multi-use
+                arg.get_real_data_instr().change_opcode(Opcodes.NOP)
+
+
+def register(target: typing.Callable):
+    def annotation(special: typing.Callable[[SpecializationContainer], None]):
+        from bytecodemanipulation.Optimiser import _OptimisationContainer
+
+        _OptimisationContainer.get_for_target(target).specializations.append(special)
+
+        return special
+
+    return annotation
```

### Comparing `bytecodemanipulation-0.2.4/bytecodemanipulation/assembler/Emitter.py` & `bytecodemanipulation-0.2.8/bytecodemanipulation/assembler/Emitter.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,339 +1,355 @@
-import dis
-import string
-import types
-import typing
-
-import bytecodemanipulation.assembler.Lexer
-from bytecodemanipulation.MutableFunction import MutableFunction, Instruction
-from bytecodemanipulation.Opcodes import Opcodes
-from bytecodemanipulation.assembler.Parser import (
-    Parser as AssemblyParser,
-    JumpToLabel,
-    ParsingScope,
-)
-from bytecodemanipulation.assembler import target as assembly_targets
-from bytecodemanipulation.util import LambdaInstructionWalker
-
-
-def _visit_for_stack_effect(
-    ins: Instruction,
-    eff_a: typing.Tuple[int, int] | None,
-    eff_b: typing.Tuple[int, int] | None,
-) -> typing.Tuple[int, int]:
-    eff = 0
-    max_size = 0
-
-    if eff_b is not None:
-        max_size = eff_b[1]
-
-    if eff_a is not None:
-        eff += eff_a[0]
-
-        max_size = max(max_size, eff, eff_a[0])
-
-    push, pop, *_ = ins.get_stack_affect()
-
-    eff += push - pop
-
-    max_size = max(max_size, max_size + eff)
-
-    return eff, max_size
-
-
-GLOBAL_SCOPE_CACHE: typing.Dict[str, dict] = {}
-
-
-def apply_inline_assemblies(
-    target: MutableFunction | typing.Callable, store_at_target: bool = None
-):
-    """
-    Processes all assembly() calls and label() calls in 'target'
-    """
-
-    if not isinstance(target, MutableFunction):
-        target = MutableFunction(target)
-        if store_at_target is None:
-            store_at_target = True
-
-    labels = set()
-    insertion_points: typing.List[typing.Tuple[str, Instruction]] = []
-
-    for instr in target.instructions[:]:
-        if instr.opcode == Opcodes.LOAD_GLOBAL:
-            try:
-                value = target.target.__globals__.get(instr.arg_value)
-            except KeyError:
-                continue
-
-            if value == assembly_targets.assembly:
-                invoke = next(instr.trace_stack_position_use(0))
-                arg = next(invoke.trace_stack_position(0))
-                assert (
-                    arg.opcode == Opcodes.LOAD_CONST
-                ), "only constant assembly code is allowed!"
-
-                if invoke.next_instruction.opcode == Opcodes.POP_TOP:
-                    insertion_points.append((arg.arg_value, invoke.next_instruction))
-                else:
-                    insertion_points.append((arg.arg_value, invoke))
-
-                instr.change_opcode(Opcodes.NOP)
-                arg.change_opcode(Opcodes.NOP)
-                invoke.change_opcode(Opcodes.LOAD_CONST, None)
-
-            elif value == assembly_targets.jump:
-                invoke = next(instr.trace_stack_position_use(0))
-                arg = next(invoke.trace_stack_position(0))
-                assert (
-                    arg.opcode == Opcodes.LOAD_CONST
-                ), "only constant assembly code is allowed!"
-                assert all(
-                    e in string.ascii_letters + string.digits for e in arg.arg_value
-                ), "only characters and digits are allowed for label names!"
-
-                if invoke.next_instruction.opcode == Opcodes.POP_TOP:
-                    insertion_points.append(
-                        (f"JUMP {arg.arg_value}", invoke.next_instruction)
-                    )
-                else:
-                    insertion_points.append((f"JUMP {arg.arg_value}", invoke))
-
-                instr.change_opcode(Opcodes.NOP)
-                arg.change_opcode(Opcodes.NOP)
-                invoke.change_opcode(Opcodes.LOAD_CONST, None)
-
-            elif value == assembly_targets.label:
-                invoke = next(instr.trace_stack_position_use(0))
-                arg = next(invoke.trace_stack_position(0))
-                assert (
-                    arg.opcode == Opcodes.LOAD_CONST
-                ), "only constant label names are allowed!"
-
-                labels.add(arg.arg_value)
-                invoke.change_opcode(Opcodes.BYTECODE_LABEL, arg.arg_value)
-                invoke.insert_after(Instruction(target, -1, Opcodes.LOAD_CONST, None))
-                instr.change_opcode(Opcodes.NOP)
-                # print(type(arg))
-                arg.change_opcode(Opcodes.NOP)
-
-    if not insertion_points:
-        raise RuntimeError("no target found!")
-
-    scope = ParsingScope()
-    scope.globals_dict = target.target.__globals__
-    scope.module_file = target.target.__globals__["__file__"]
-
-    if target.target.__module__ in GLOBAL_SCOPE_CACHE:
-        scope.global_scope = GLOBAL_SCOPE_CACHE[target.target.__module__]
-    else:
-        GLOBAL_SCOPE_CACHE[target.target.__module__] = scope.global_scope
-
-    assemblies = [
-        AssemblyParser(
-            bytecodemanipulation.assembler.Lexer.Lexer(code)
-            .add_line_offset(instr.source_location[0] + 1)
-            .lex(),
-            scope.scope_path.clear() or scope,
-        ).parse()
-        for code, instr in insertion_points
-    ]
-
-    for asm in assemblies:
-        labels.update(asm.collect_label_info())
-
-    scope.labels |= labels
-
-    max_stack_effects = []
-
-    label_targets: typing.Dict[str, Instruction] = {}
-
-    # for asm in assemblies:
-    #     asm.fill_scope_complete(scope)
-
-    scope.scope_path.clear()
-
-    for (_, instr), asm in zip(insertion_points, assemblies):
-        bytecode = asm.create_bytecode(target, scope)
-
-        for i, ins in enumerate(bytecode[:-1]):
-            ins.next_instruction = bytecode[i + 1]
-
-        # print("---- start ----")
-        # for e in bytecode:
-        #     print(e)
-        # print("---- end ----")
-
-        if bytecode:
-            stack_effect, max_stack_effect = bytecode[0].apply_value_visitor(
-                _visit_for_stack_effect
-            )
-        else:
-            stack_effect = max_stack_effect = 0
-
-        if (
-            stack_effect != 0
-            and bytecode
-            and not (
-                bytecode[-1].has_unconditional_jump() or bytecode[-1].has_stop_flow()
-            )
-        ):
-            print(asm)
-
-            total = 0
-
-            for e in enumerate(bytecode):
-                add, subtract, _ = e[1].get_stack_affect()
-                total += add - subtract
-                print(*e, total)
-
-            print(stack_effect)
-
-            raise RuntimeError(
-                f"Inline assembly code mustn't change overall stack size at exit, got a delta of {stack_effect}!"
-            )
-
-        max_stack_effects.append(max_stack_effect)
-
-        if bytecode:
-            for i, ins in enumerate(bytecode[:-1]):
-                if not ins.has_stop_flow() and not ins.has_unconditional_jump():
-                    ins.next_instruction = bytecode[i + 1]
-
-            bytecode[-1].next_instruction = following_instr = instr.next_instruction
-
-            # print("inserting AFTER", instr)
-            instr.insert_after(bytecode)
-        # else:
-        #     print("empty bytecode block")
-        #     print(asm)
-
-        for i, ins in enumerate(bytecode):
-            if ins.opcode == Opcodes.BYTECODE_LABEL:
-                label_targets[ins.arg_value] = ins.next_instruction
-
-                if not isinstance(ins, Instruction):
-                    print("error: ", ins)
-
-                ins.change_opcode(Opcodes.NOP)
-                ins.next_instruction = bytecode[i + 1] if i < len(bytecode) - 1 else following_instr
-
-    for i, ins in enumerate(target.instructions):
-        if ins.opcode == Opcodes.BYTECODE_LABEL:
-            label_targets[ins.arg_value] = ins.next_instruction
-            ins.change_opcode(Opcodes.NOP)
-            ins.next_instruction = target.instructions[i+1]
-
-    def resolve_special_code(ins: Instruction):
-        if ins.has_jump() and isinstance(ins.arg_value, JumpToLabel):
-            ins.change_arg_value(label_targets[ins.arg_value.name])
-
-        elif ins.opcode == Opcodes.STATIC_ATTRIBUTE_ACCESS:
-            source = next(ins.trace_stack_position(0))
-
-            if source.opcode != Opcodes.LOAD_CONST:
-                raise RuntimeError("expected 'constant' for constant attribute access!")
-
-            obj = source.arg_value
-            source.change_opcode(Opcodes.NOP)
-            ins.change_opcode(Opcodes.LOAD_CONST, getattr(obj, ins.arg_value))
-
-    target.instructions[0].apply_visitor(LambdaInstructionWalker(resolve_special_code))
-
-    target.stack_size += max(max_stack_effects)
-
-    # target.instructions[0].apply_value_visitor(lambda instr, *_: print(instr))
-
-    target.assemble_instructions_from_tree(target.instructions[0])
-
-    if store_at_target:
-        target.reassign_to_function()
-
-    return target
-
-
-def execute_module_in_instance(
-    asm_code: str, module: types.ModuleType, file: str = None
-):
-    scope = ParsingScope()
-
-    try:
-        scope.module_file = file or module.__file__
-    except AttributeError:
-        pass
-
-    if module.__name__ in GLOBAL_SCOPE_CACHE:
-        scope.global_scope = GLOBAL_SCOPE_CACHE[module.__name__]
-    else:
-        GLOBAL_SCOPE_CACHE[module.__name__] = scope.global_scope
-
-    asm = AssemblyParser(asm_code, scope).parse()
-    scope.labels = asm.get_labels()
-    # asm.fill_scope_complete(scope)
-    scope.scope_path.clear()
-    create_function = lambda m: None
-    target = MutableFunction(create_function)
-    target.shared_variable_names[0] = "$module$"
-    bytecode = asm.create_bytecode(target, scope)
-
-    if bytecode is None:
-        return
-
-    label_targets = {}
-    for ins in bytecode:
-        if ins.opcode == Opcodes.BYTECODE_LABEL:
-            label_targets[ins.arg_value] = ins.next_instruction
-            ins.change_opcode(Opcodes.NOP)
-
-    for i, ins in enumerate(bytecode[:-1]):
-        ins.next_instruction = bytecode[i + 1]
-
-    def resolve_jump_to_label(ins: Instruction):
-        if ins.has_jump() and isinstance(ins.arg_value, JumpToLabel):
-            ins.change_arg_value(label_targets[ins.arg_value.name])
-
-    for instr in bytecode:
-        instr.update_owner(
-            target, -1, force_change_arg_index=True, update_following=False
-        )
-
-    if not bytecode:
-        bytecode.append(Instruction(target, -1, "NOP"))
-
-    bytecode[-1].next_instruction = target.instructions[0]
-    target.assemble_instructions_from_tree(bytecode[0])
-
-    target.instructions[0].apply_visitor(LambdaInstructionWalker(resolve_jump_to_label))
-    target.stack_size = bytecode[0].apply_value_visitor(_visit_for_stack_effect)[1]
-
-    target.assemble_instructions_from_tree(target.instructions[0])
-
-    for instr in target.instructions:
-        if instr.opcode == Opcodes.STORE_FAST:
-            load_module = Instruction(target, -1, Opcodes.LOAD_FAST, "$module$")
-            store = Instruction(target, -1, Opcodes.STORE_ATTR, instr.arg_value)
-
-            instr.change_opcode(Opcodes.NOP)
-            instr.insert_after([load_module, store])
-
-        elif instr.opcode == Opcodes.LOAD_FAST:
-            load_module = Instruction(target, -1, Opcodes.LOAD_FAST, "$module$")
-            load = Instruction(target, -1, Opcodes.LOAD_ATTR, instr.arg_value)
-
-            instr.change_opcode(Opcodes.NOP)
-            instr.insert_after([load_module, load])
-
-        elif instr.opcode == Opcodes.DELETE_FAST:
-            load_module = Instruction(target, -1, Opcodes.LOAD_FAST, "$module$")
-            delete = Instruction(target, -1, Opcodes.DELETE_ATTR, instr.arg_value)
-
-            instr.change_opcode(Opcodes.NOP)
-            instr.insert_after([load_module, delete])
-
-    target.assemble_instructions_from_tree(target.instructions[0])
-    target.function_name = module.__name__
-
-    target.reassign_to_function()
-
-    # dis.dis(target)
-
-    create_function(module)
+import dis
+import string
+import types
+import typing
+
+from bytecodemanipulation.assembler.Lexer import Lexer
+from bytecodemanipulation.MutableFunction import MutableFunction, Instruction
+from bytecodemanipulation.Opcodes import Opcodes
+from bytecodemanipulation.assembler.Parser import (
+    Parser as AssemblyParser,
+)
+from bytecodemanipulation.assembler.AbstractBase import JumpToLabel
+from bytecodemanipulation.assembler.AbstractBase import ParsingScope
+from bytecodemanipulation.assembler import target as assembly_targets
+from bytecodemanipulation.util import LambdaInstructionWalker
+
+
+def _visit_for_stack_effect(
+    ins: Instruction,
+    eff_a: typing.Tuple[int, int] | None,
+    eff_b: typing.Tuple[int, int] | None,
+) -> typing.Tuple[int, int]:
+    if ins.opcode == Opcodes.FOR_ITER:
+        raise RuntimeError
+
+    eff = 0
+    max_size = 0
+
+    if eff_b is not None:
+        max_size = eff_b[1]
+
+    if eff_a is not None:
+        eff += eff_a[0]
+
+        max_size = max(max_size, eff, eff_a[0])
+
+    push, pop, *_ = ins.get_stack_affect()
+
+    eff += push - pop
+
+    max_size = max(max_size, max_size + eff)
+
+    return eff, max_size
+
+
+GLOBAL_SCOPE_CACHE: typing.Dict[str, dict] = {}
+
+
+def apply_inline_assemblies(
+    target: MutableFunction | typing.Callable, store_at_target: bool = None
+):
+    """
+    Processes all assembly() calls and label() calls in 'target'
+    """
+
+    if not isinstance(target, MutableFunction):
+        target = MutableFunction(target)
+        if store_at_target is None:
+            store_at_target = True
+
+    labels = set()
+    insertion_points: typing.List[typing.Tuple[str, Instruction]] = []
+
+    for instr in target.instructions[:]:
+        if instr.opcode == Opcodes.LOAD_GLOBAL:
+            try:
+                value = target.target.__globals__.get(instr.arg_value)
+            except KeyError:
+                continue
+
+            if value == assembly_targets.assembly:
+                invoke = next(instr.trace_stack_position_use(0))
+                arg = next(invoke.trace_stack_position(0))
+                assert (
+                    arg.opcode == Opcodes.LOAD_CONST
+                ), "only constant assembly code is allowed!"
+
+                if invoke.next_instruction.opcode == Opcodes.POP_TOP:
+                    insertion_points.append((arg.arg_value, invoke.next_instruction))
+                else:
+                    insertion_points.append((arg.arg_value, invoke))
+
+                instr.change_opcode(Opcodes.NOP)
+                arg.change_opcode(Opcodes.NOP)
+                invoke.change_opcode(Opcodes.LOAD_CONST, None)
+
+            elif value == assembly_targets.jump:
+                invoke = next(instr.trace_stack_position_use(0))
+                arg = next(invoke.trace_stack_position(0))
+                assert (
+                    arg.opcode == Opcodes.LOAD_CONST
+                ), "only constant assembly code is allowed!"
+                assert all(
+                    e in string.ascii_letters + string.digits for e in arg.arg_value
+                ), "only characters and digits are allowed for label names!"
+
+                if invoke.next_instruction.opcode == Opcodes.POP_TOP:
+                    insertion_points.append(
+                        (f"JUMP {arg.arg_value}", invoke.next_instruction)
+                    )
+                else:
+                    insertion_points.append((f"JUMP {arg.arg_value}", invoke))
+
+                instr.change_opcode(Opcodes.NOP)
+                arg.change_opcode(Opcodes.NOP)
+                invoke.change_opcode(Opcodes.LOAD_CONST, None)
+
+            elif value == assembly_targets.label:
+                invoke = next(instr.trace_stack_position_use(0))
+                arg = next(invoke.trace_stack_position(0))
+                assert (
+                    arg.opcode == Opcodes.LOAD_CONST
+                ), "only constant label names are allowed!"
+
+                labels.add(arg.arg_value)
+                invoke.change_opcode(Opcodes.BYTECODE_LABEL, arg.arg_value)
+                invoke.insert_after(Instruction(target, -1, Opcodes.LOAD_CONST, None))
+                instr.change_opcode(Opcodes.NOP)
+                # print(type(arg))
+                arg.change_opcode(Opcodes.NOP)
+
+    if not insertion_points:
+        raise RuntimeError("no target found!")
+
+    scope = ParsingScope()
+    scope.globals_dict = target.target.__globals__
+    scope.module_file = target.target.__globals__["__file__"]
+
+    if target.target.__module__ in GLOBAL_SCOPE_CACHE:
+        scope.global_scope = GLOBAL_SCOPE_CACHE[target.target.__module__]
+    else:
+        GLOBAL_SCOPE_CACHE[target.target.__module__] = scope.global_scope
+
+    assemblies = [
+        AssemblyParser(
+            Lexer(code).add_line_offset(instr.source_location[0] + 1).lex(),
+            scope.scope_path.clear() or scope,
+        ).parse()
+        for code, instr in insertion_points
+    ]
+
+    for asm in assemblies:
+        labels.update(asm.collect_label_info())
+
+    scope.labels |= labels
+
+    max_stack_effects = []
+
+    label_targets: typing.Dict[str, Instruction] = {}
+
+    # for asm in assemblies:
+    #     asm.fill_scope_complete(scope)
+
+    scope.scope_path.clear()
+
+    for (_, instr), asm in zip(insertion_points, assemblies):
+        bytecode = asm.create_bytecode(target, scope)
+
+        for i, ins in enumerate(bytecode[:-1]):
+            ins.next_instruction = bytecode[i + 1]
+
+        # print("---- start ----")
+        # for e in bytecode:
+        #     print(e)
+        # print("---- end ----")
+
+        if bytecode:
+            try:
+                stack_effect, max_stack_effect = bytecode[0].apply_value_visitor(
+                    _visit_for_stack_effect
+                )
+            except RuntimeError:
+                stack_effect = 0
+                max_stack_effect = 0
+        else:
+            stack_effect = max_stack_effect = 0
+
+        if (
+            stack_effect != 0
+            and bytecode
+            and not (
+                bytecode[-1].has_unconditional_jump() or bytecode[-1].has_stop_flow()
+            )
+        ):
+            print(asm)
+
+            total = 0
+
+            for e in enumerate(bytecode):
+                add, subtract, _ = e[1].get_stack_affect()
+                total += add - subtract
+                print(*e, total)
+
+            print(stack_effect)
+
+            raise RuntimeError(
+                f"Inline assembly code mustn't change overall stack size at exit, got a delta of {stack_effect}!"
+            )
+
+        max_stack_effects.append(max_stack_effect)
+
+        if bytecode:
+            for i, ins in enumerate(bytecode[:-1]):
+                if not ins.has_stop_flow() and not ins.has_unconditional_jump():
+                    ins.next_instruction = bytecode[i + 1]
+
+            bytecode[-1].next_instruction = following_instr = instr.next_instruction
+
+            # print("inserting AFTER", instr)
+            instr.insert_after(bytecode)
+        # else:
+        #     print("empty bytecode block")
+        #     print(asm)
+
+        for i, ins in enumerate(bytecode):
+            if ins.opcode == Opcodes.BYTECODE_LABEL:
+                label_targets[ins.arg_value] = ins.next_instruction
+
+                if not isinstance(ins, Instruction):
+                    print("error: ", ins)
+
+                ins.change_opcode(Opcodes.NOP)
+                ins.next_instruction = (
+                    bytecode[i + 1] if i < len(bytecode) - 1 else following_instr
+                )
+
+    for i, ins in enumerate(target.instructions):
+        if ins.opcode == Opcodes.BYTECODE_LABEL:
+            label_targets[ins.arg_value] = ins.next_instruction
+            ins.change_opcode(Opcodes.NOP)
+            ins.next_instruction = target.instructions[i + 1]
+
+    pending: typing.List[Instruction] = []
+
+    def resolve_special_code(ins: Instruction, *_):
+        # print(ins)
+        if ins.has_jump() and isinstance(ins.arg_value, JumpToLabel):
+            ins.change_arg_value(label_targets[ins.arg_value.name])
+            pending.append(ins.arg_value)
+
+        elif ins.opcode == Opcodes.STATIC_ATTRIBUTE_ACCESS:
+            source = next(ins.trace_stack_position(0))
+
+            if source.opcode != Opcodes.LOAD_CONST:
+                raise RuntimeError("expected 'constant' for constant attribute access!")
+
+            obj = source.arg_value
+            source.change_opcode(Opcodes.NOP, update_next=False)
+            ins.change_opcode(
+                Opcodes.LOAD_CONST, getattr(obj, ins.arg_value), update_next=False
+            )
+
+    target.instructions[0].apply_value_visitor(resolve_special_code)
+
+    while pending:
+        pending.pop().apply_value_visitor(resolve_special_code)
+
+    target.stack_size += max(max_stack_effects)
+
+    # target.instructions[0].apply_value_visitor(lambda instr, *_: print(instr))
+
+    target.assemble_instructions_from_tree(target.instructions[0])
+
+    if store_at_target:
+        target.reassign_to_function()
+
+    return target
+
+
+def execute_module_in_instance(
+    asm_code: str, module: types.ModuleType, file: str = None
+):
+    scope = ParsingScope()
+
+    try:
+        scope.module_file = file or module.__file__
+    except AttributeError:
+        pass
+
+    if module.__name__ in GLOBAL_SCOPE_CACHE:
+        scope.global_scope = GLOBAL_SCOPE_CACHE[module.__name__]
+    else:
+        GLOBAL_SCOPE_CACHE[module.__name__] = scope.global_scope
+
+    asm = AssemblyParser(asm_code, scope).parse()
+    scope.labels = asm.get_labels()
+    # asm.fill_scope_complete(scope)
+    scope.scope_path.clear()
+    create_function = lambda m: None
+    target = MutableFunction(create_function)
+    target.shared_variable_names[0] = "$module$"
+    bytecode = asm.create_bytecode(target, scope)
+
+    if bytecode is None:
+        return
+
+    label_targets = {}
+    for ins in bytecode:
+        if ins.opcode == Opcodes.BYTECODE_LABEL:
+            label_targets[ins.arg_value] = ins.next_instruction
+            ins.change_opcode(Opcodes.NOP)
+
+    for i, ins in enumerate(bytecode[:-1]):
+        ins.next_instruction = bytecode[i + 1]
+
+    def resolve_jump_to_label(ins: Instruction):
+        if ins.has_jump() and isinstance(ins.arg_value, JumpToLabel):
+            ins.change_arg_value(label_targets[ins.arg_value.name])
+
+    for instr in bytecode:
+        instr.update_owner(
+            target, -1, force_change_arg_index=True, update_following=False
+        )
+
+    if not bytecode:
+        bytecode.append(Instruction(target, -1, "NOP"))
+
+    bytecode[-1].next_instruction = target.instructions[0]
+    target.assemble_instructions_from_tree(bytecode[0])
+
+    target.instructions[0].apply_visitor(LambdaInstructionWalker(resolve_jump_to_label))
+    target.stack_size = bytecode[0].apply_value_visitor(_visit_for_stack_effect)[1]
+
+    target.assemble_instructions_from_tree(target.instructions[0])
+
+    for instr in target.instructions:
+        if instr.opcode == Opcodes.STORE_FAST:
+            load_module = Instruction(target, -1, Opcodes.LOAD_FAST, "$module$")
+            store = Instruction(target, -1, Opcodes.STORE_ATTR, instr.arg_value)
+
+            instr.change_opcode(Opcodes.NOP)
+            instr.insert_after([load_module, store])
+
+        elif instr.opcode == Opcodes.LOAD_FAST:
+            load_module = Instruction(target, -1, Opcodes.LOAD_FAST, "$module$")
+            load = Instruction(target, -1, Opcodes.LOAD_ATTR, instr.arg_value)
+
+            instr.change_opcode(Opcodes.NOP)
+            instr.insert_after([load_module, load])
+
+        elif instr.opcode == Opcodes.DELETE_FAST:
+            load_module = Instruction(target, -1, Opcodes.LOAD_FAST, "$module$")
+            delete = Instruction(target, -1, Opcodes.DELETE_ATTR, instr.arg_value)
+
+            instr.change_opcode(Opcodes.NOP)
+            instr.insert_after([load_module, delete])
+
+    target.assemble_instructions_from_tree(target.instructions[0])
+    target.function_name = module.__name__
+
+    target.reassign_to_function()
+
+    # dis.dis(target)
+
+    create_function(module)
```

### Comparing `bytecodemanipulation-0.2.4/bytecodemanipulation/assembler/Lexer.py` & `bytecodemanipulation-0.2.8/bytecodemanipulation/assembler/Lexer.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,189 +1,189 @@
-import string
-import typing
-import warnings
-
-try:
-    from code_parser.lexers.common import (
-        AbstractLexer,
-        IntegerToken,
-        FloatToken,
-        BinaryOperatorToken,
-        BracketToken,
-        IdentifierToken,
-        StringLiteralToken,
-        CommentToken,
-        AbstractToken,
-    )
-
-except ImportError:
-    from bytecodemanipulation.assembler.util.tokenizer import (
-        AbstractLexer,
-        IntegerToken,
-        FloatToken,
-        BinaryOperatorToken,
-        BracketToken,
-        IdentifierToken,
-        StringLiteralToken,
-        CommentToken,
-        AbstractToken,
-    )
-
-
-SPECIAL_CHARS = "@$+-~/%?;[]{}()<>=!,.*':§\\"
-
-
-class SpecialToken(AbstractToken):
-    pass
-
-
-class PythonCodeToken(AbstractToken):
-    pass
-
-
-def _count_chars_at_end(text: str, c: str) -> int:
-    count = 0
-
-    while text.endswith(c):
-        text = text.removesuffix(c)
-        count += 1
-
-    return count
-
-
-class Lexer(AbstractLexer):
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self.had_newline = False
-
-    def lex_single(self) -> typing.List[AbstractToken] | AbstractToken | None:
-        char = self.inspect()
-
-        self.had_newline = False
-
-        if char == "#":
-            token = CommentToken(
-                self.consume_until("\n", include=False).removesuffix("\r")
-            )
-            return token
-
-        if char in string.digits or (
-            char == "-" and self.try_inspect_multi(2)[1] in string.digits
-        ):
-            text = ""
-            if self.try_consume("-"):
-                text += "."
-            text += self.consume_while(string.digits + "_")
-
-            if self.try_inspect() == ".":
-                remaining = self.consume(".") + self.consume_while(string.digits + "_")
-
-                if self.try_inspect() and self.try_inspect() in string.ascii_letters:
-                    return [
-                        IntegerToken(text),
-                        SpecialToken("."),
-                        IdentifierToken(
-                            remaining[1:]
-                            + self.consume_while(
-                                string.ascii_letters + string.digits + "_"
-                            )
-                        ),
-                    ]
-
-                text += remaining
-
-            elif self.try_inspect() and self.try_inspect() in string.ascii_letters:
-                text += self.consume_while(string.ascii_letters + string.digits + "_")
-
-                return IdentifierToken(text)
-
-            return IntegerToken(text)
-
-        if char in string.ascii_letters + "_":
-            identifier = self.consume_while(string.ascii_letters + string.digits + "_")
-
-            if identifier == "PYTHON" and self.try_consume_multi(2, " {"):
-                python = self.consume_python_code()
-                self.consume("}")
-
-                return [IdentifierToken("PYTHON"), PythonCodeToken(python)]
-
-            return IdentifierToken(identifier)
-
-        if char in SPECIAL_CHARS:
-            return SpecialToken(self.consume(char))
-
-        if char == '"':
-            self.consume(char)
-            text = ""
-
-            escape_count = 0
-            while (c := self.try_inspect()) and (c != '"' or escape_count % 2 == 1):
-                if c == "\\":
-                    escape_count += 1
-                else:
-                    escape_count = 0
-                text += c
-                self.consume(c)
-            self.consume('"')
-            return StringLiteralToken(text, '"')
-
-        if char in string.whitespace:
-            self.consume_while(string.whitespace)
-            return
-
-        raise SyntaxError(f"Invalid char: '{char}' (at {self.cursor})")
-
-    def consume_python_code(self):
-        bracket_level = 0
-
-        code = ""
-
-        while True:
-            code += self.consume_while(
-                string.ascii_letters
-                + string.digits
-                + string.whitespace
-                + "@!$+~*-_.,:;%&/\\[]()<>|"
-            )
-
-            n = self.try_inspect()
-
-            if n is None:
-                raise SyntaxError("expected '}' at python end, got EOF")
-
-            if n == "#":
-                code += self.consume_until("\n")
-            elif n in "\"'":
-                # todo: f-strings
-
-                if code[-2:] == " f":
-                    warnings.warn(
-                        "Found f-string in python literal, this might not work!"
-                    )
-
-                triple = self.try_inspect_multi(3)
-
-                if triple == n * 3:
-                    code += self.consume(triple) + self.consume_until(
-                        lambda text, c: text.endswith(triple)
-                        and _count_chars_at_end(text.removesuffix(triple), "\\") % 1
-                        == 0
-                    )
-                    pass
-
-                code += self.consume(n) + self.consume_until(
-                    lambda text, c: text.endswith(n)
-                    and _count_chars_at_end(text.removesuffix(n), "\\") % 1 == 0
-                )
-
-            elif n == "{":
-                bracket_level += 1
-
-            elif n == "}":
-                bracket_level -= 1
-
-                if bracket_level == -1:
-                    return code.strip()
-
-            else:
-                raise NotImplementedError(n)
+import string
+import typing
+import warnings
+
+try:
+    from code_parser.lexers.common import (
+        AbstractLexer,
+        IntegerToken,
+        FloatToken,
+        BinaryOperatorToken,
+        BracketToken,
+        IdentifierToken,
+        StringLiteralToken,
+        CommentToken,
+        AbstractToken,
+    )
+
+except ImportError:
+    from bytecodemanipulation.assembler.util.tokenizer import (
+        AbstractLexer,
+        IntegerToken,
+        FloatToken,
+        BinaryOperatorToken,
+        BracketToken,
+        IdentifierToken,
+        StringLiteralToken,
+        CommentToken,
+        AbstractToken,
+    )
+
+
+SPECIAL_CHARS = "@$+-~/%?;[]{}()<>=!,.*':§&\\"
+
+
+class SpecialToken(AbstractToken):
+    pass
+
+
+class PythonCodeToken(AbstractToken):
+    pass
+
+
+def _count_chars_at_end(text: str, c: str) -> int:
+    count = 0
+
+    while text.endswith(c):
+        text = text.removesuffix(c)
+        count += 1
+
+    return count
+
+
+class Lexer(AbstractLexer):
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.had_newline = False
+
+    def lex_single(self) -> typing.List[AbstractToken] | AbstractToken | None:
+        char = self.inspect()
+
+        self.had_newline = False
+
+        if char == "#":
+            token = CommentToken(
+                self.consume_until("\n", include=False).removesuffix("\r")
+            )
+            return token
+
+        if char in string.digits or (
+            char == "-" and self.try_inspect_multi(2)[1] in string.digits
+        ):
+            text = ""
+            if self.try_consume("-"):
+                text += "."
+            text += self.consume_while(string.digits + "_")
+
+            if self.try_inspect() == ".":
+                remaining = self.consume(".") + self.consume_while(string.digits + "_")
+
+                if self.try_inspect() and self.try_inspect() in string.ascii_letters:
+                    return [
+                        IntegerToken(text),
+                        SpecialToken("."),
+                        IdentifierToken(
+                            remaining[1:]
+                            + self.consume_while(
+                                string.ascii_letters + string.digits + "_"
+                            )
+                        ),
+                    ]
+
+                text += remaining
+
+            elif self.try_inspect() and self.try_inspect() in string.ascii_letters:
+                text += self.consume_while(string.ascii_letters + string.digits + "_")
+
+                return IdentifierToken(text)
+
+            return IntegerToken(text)
+
+        if char in string.ascii_letters + "_":
+            identifier = self.consume_while(string.ascii_letters + string.digits + "_")
+
+            if identifier == "PYTHON" and self.try_consume_multi(2, " {"):
+                python = self.consume_python_code()
+                self.consume("}")
+
+                return [IdentifierToken("PYTHON"), PythonCodeToken(python)]
+
+            return IdentifierToken(identifier)
+
+        if char in SPECIAL_CHARS:
+            return SpecialToken(self.consume(char))
+
+        if char == '"':
+            self.consume(char)
+            text = ""
+
+            escape_count = 0
+            while (c := self.try_inspect()) and (c != '"' or escape_count % 2 == 1):
+                if c == "\\":
+                    escape_count += 1
+                else:
+                    escape_count = 0
+                text += c
+                self.consume(c)
+            self.consume('"')
+            return StringLiteralToken(text, '"')
+
+        if char in string.whitespace:
+            self.consume_while(string.whitespace)
+            return
+
+        raise SyntaxError(f"Invalid char: '{char}' (at {self.cursor})")
+
+    def consume_python_code(self):
+        bracket_level = 0
+
+        code = ""
+
+        while True:
+            code += self.consume_while(
+                string.ascii_letters
+                + string.digits
+                + string.whitespace
+                + "@!$+~*-_.,:;%&/\\[]()<>|"
+            )
+
+            n = self.try_inspect()
+
+            if n is None:
+                raise SyntaxError("expected '}' at python end, got EOF")
+
+            if n == "#":
+                code += self.consume_until("\n")
+            elif n in "\"'":
+                # todo: f-strings
+
+                if code[-2:] == " f":
+                    warnings.warn(
+                        "Found f-string in python literal, this might not work!"
+                    )
+
+                triple = self.try_inspect_multi(3)
+
+                if triple == n * 3:
+                    code += self.consume(triple) + self.consume_until(
+                        lambda text, c: text.endswith(triple)
+                        and _count_chars_at_end(text.removesuffix(triple), "\\") % 1
+                        == 0
+                    )
+                    pass
+
+                code += self.consume(n) + self.consume_until(
+                    lambda text, c: text.endswith(n)
+                    and _count_chars_at_end(text.removesuffix(n), "\\") % 1 == 0
+                )
+
+            elif n == "{":
+                bracket_level += 1
+
+            elif n == "}":
+                bracket_level -= 1
+
+                if bracket_level == -1:
+                    return code.strip()
+
+            else:
+                raise NotImplementedError(n)
```

### Comparing `bytecodemanipulation-0.2.4/bytecodemanipulation/assembler/target.py` & `bytecodemanipulation-0.2.8/bytecodemanipulation/assembler/target.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,105 +1,119 @@
-import typing
-
-import bytecodemanipulation.MutableFunction
-
-import bytecodemanipulation.assembler.Parser
-
-T = typing.TypeVar("T")
-
-
-class VARIABLE(typing.Generic[T]):
-    pass
-
-
-class VARIABLE_ARG(typing.Generic[T]):
-    pass
-
-
-class CODE_BLOCK:
-    pass
-
-
-def assembly(code: str):
-    raise RuntimeError("Function must be annotated first!")
-
-
-def label(name: str):
-    raise RuntimeError("Function must be annotated first!")
-
-
-def jump(label_name: str):
-    raise RuntimeError("Function must be annotated first!")
-
-
-def _raise_macro_direct_call_error():
-    raise RuntimeError("Cannot call <macro> with normal call!")
-
-
-def make_macro(export_name: str = None, /, prevent_direct_calls=False):
-    """
-    Makes the annotated function a macro function, making it possible to use as a macro
-
-    WARNING: the internal system needs to do some clever stuff around parameters, and might reject
-    your parameter configuration (this mostly includes keyword arguments)
-
-    To use the macro somewhere else, the target should be also annotated with some processing
-    function, and the reference should be static-decidable.
-    Otherwise, a call to the real function will be used, and the bytecode of the callee
-    will be tried to be modified
-
-    WARNING: returns are currently not allowed in macros!
-        they will be changed into JUMP-TO-END-OF-MACRO!
-
-    :param export_name: the name to export into the global namespace
-    :param prevent_direct_calls: if to prevent calls in non-macro form
-    """
-
-    def annotation(function):
-        from bytecodemanipulation.assembler.Parser import MacroAssembly
-        from bytecodemanipulation.assembler.Lexer import IdentifierToken
-
-        macro_name = (export_name or function.__qualname__).replace(".", ":")
-
-        mutable = bytecodemanipulation.MutableFunction.MutableFunction(function)
-
-        macro_asm = MacroAssembly(
-            [IdentifierToken(macro_name[-1])],
-            [
-                # todo: add data type here!
-                MacroAssembly.MacroArg(IdentifierToken(name))
-                for name in mutable.shared_variable_names[:mutable.argument_count]
-            ],
-            MacroAssembly.Function2CompoundMapper(function, scoped_names=mutable.shared_variable_names[:mutable.argument_count]),
-        )
-
-        namespace = macro_name.split(":")[:-1]
-
-        scope = bytecodemanipulation.assembler.Parser.ParsingScope.create_for_function(function)
-        namespace_obj = scope.lookup_namespace(namespace)
-
-        if macro_name.split(":")[-1] not in namespace_obj:
-            namespace_obj[macro_name.split(":")[-1]] = MacroAssembly.MacroOverloadPage(macro_name.split(":"))
-
-        namespace_obj[macro_name.split(":")[-1]].add_assembly(macro_asm)
-
-        if prevent_direct_calls:
-            mutable.copy_from(bytecodemanipulation.MutableFunction.MutableFunction(_raise_macro_direct_call_error))
-            mutable.reassign_to_function()
-
-        return function
-
-    return annotation
-
-
-def configurate_makro_parameter(name: str | int, config_pattern: typing.Type):
-    """
-    Configures the type of parameter of a @make_macro annotated function
-
-    :param name: the name of the parameter, or the index
-    :param config_pattern: the type of parameter
-    """
-
-    def annotation(function):
-        return function
-
-    return annotation
+import typing
+
+import bytecodemanipulation.assembler.AbstractBase
+import bytecodemanipulation.MutableFunction
+
+import bytecodemanipulation.assembler.Parser
+
+T = typing.TypeVar("T")
+
+
+class VARIABLE(typing.Generic[T]):
+    pass
+
+
+class VARIABLE_ARG(typing.Generic[T]):
+    pass
+
+
+class CODE_BLOCK:
+    pass
+
+
+def assembly(code: str):
+    raise RuntimeError("Function must be annotated first!")
+
+
+def label(name: str):
+    raise RuntimeError("Function must be annotated first!")
+
+
+def jump(label_name: str):
+    raise RuntimeError("Function must be annotated first!")
+
+
+def _raise_macro_direct_call_error():
+    raise RuntimeError("Cannot call <macro> with normal call!")
+
+
+def make_macro(export_name: str = None, /, prevent_direct_calls=False):
+    """
+    Makes the annotated function a macro function, making it possible to use as a macro
+
+    WARNING: the internal system needs to do some clever stuff around parameters, and might reject
+    your parameter configuration (this mostly includes keyword arguments)
+
+    To use the macro somewhere else, the target should be also annotated with some processing
+    function, and the reference should be static-decidable.
+    Otherwise, a call to the real function will be used, and the bytecode of the callee
+    will be tried to be modified
+
+    WARNING: returns are currently not allowed in macros!
+        they will be changed into JUMP-TO-END-OF-MACRO!
+
+    :param export_name: the name to export into the global namespace
+    :param prevent_direct_calls: if to prevent calls in non-macro form
+    """
+
+    def annotation(function):
+        from bytecodemanipulation.data.shared.instructions.MacroAssembly import (
+            MacroAssembly,
+        )
+        from bytecodemanipulation.assembler.Lexer import IdentifierToken
+
+        macro_name = (export_name or function.__qualname__).replace(".", ":")
+
+        mutable = bytecodemanipulation.MutableFunction.MutableFunction(function)
+
+        macro_asm = MacroAssembly(
+            [IdentifierToken(macro_name[-1])],
+            [
+                # todo: add data type here!
+                MacroAssembly.MacroArg(IdentifierToken(name))
+                for name in mutable.shared_variable_names[: mutable.argument_count]
+            ],
+            MacroAssembly.Function2CompoundMapper(
+                function,
+                scoped_names=mutable.shared_variable_names[: mutable.argument_count],
+            ),
+        )
+
+        namespace = macro_name.split(":")[:-1]
+
+        scope = bytecodemanipulation.assembler.AbstractBase.ParsingScope.create_for_function(
+            function
+        )
+        namespace_obj = scope.lookup_namespace(namespace)
+
+        if macro_name.split(":")[-1] not in namespace_obj:
+            namespace_obj[macro_name.split(":")[-1]] = MacroAssembly.MacroOverloadPage(
+                macro_name.split(":")
+            )
+
+        namespace_obj[macro_name.split(":")[-1]].add_assembly(macro_asm)
+
+        if prevent_direct_calls:
+            mutable.copy_from(
+                bytecodemanipulation.MutableFunction.MutableFunction(
+                    _raise_macro_direct_call_error
+                )
+            )
+            mutable.reassign_to_function()
+
+        return function
+
+    return annotation
+
+
+def configurate_makro_parameter(name: str | int, config_pattern: typing.Type):
+    """
+    Configures the type of parameter of a @make_macro annotated function
+
+    :param name: the name of the parameter, or the index
+    :param config_pattern: the type of parameter
+    """
+
+    def annotation(function):
+        return function
+
+    return annotation
```

### Comparing `bytecodemanipulation-0.2.4/bytecodemanipulation/assembler/util/parser.py` & `bytecodemanipulation-0.2.8/bytecodemanipulation/assembler/util/parser.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,366 +1,367 @@
-import abc
-import typing
-from bytecodemanipulation.assembler.util.tokenizer import (
-    AbstractToken,
-    IntegerToken,
-    BinaryOperatorToken,
-    BracketToken,
-    IdentifierToken,
-    EndOfFileToken,
-)
-from .CommonUtil import AbstractCursorStateItem
-
-
-class AbstractExpression(abc.ABC):
-    def visit_topdown(
-        self,
-        visitor: typing.Callable[["AbstractExpression", "AbstractExpression"], None],
-        previous=None,
-    ):
-        visitor(self)
-
-    def visit_depth_first(
-        self,
-        visitor: typing.Callable[["AbstractExpression", "AbstractExpression"], None],
-        previous=None,
-    ):
-        visitor(previous, self)
-
-    def copy(self) -> "AbstractExpression":
-        raise NotImplementedError
-
-    def __copy__(self):
-        return self.copy()
-
-    def __deepcopy__(self):
-        return self.copy()
-
-    def replace_inner(
-        self, node: "AbstractExpression", replacement: "AbstractExpression"
-    ):
-        raise ValueError(node)
-
-
-class NumericExpression(AbstractExpression):
-    def __init__(self, token: IntegerToken | str):
-        self.token = token if isinstance(token, IntegerToken) else IntegerToken(token)
-
-    def __eq__(self, other):
-        return type(other) == type(self) and self.token == other.token
-
-    def __repr__(self):
-        return f"IntegerExpression({self.token})"
-
-    def copy(self) -> "NumericExpression":
-        return NumericExpression(self.token)
-
-
-class BracketExpression(AbstractExpression):
-    def __init__(
-        self,
-        left_bracket: BracketToken | str,
-        inner: AbstractExpression,
-        right_bracket: BracketToken | str = None,
-    ):
-        self.left_bracket = (
-            left_bracket
-            if isinstance(left_bracket, BracketToken)
-            else BracketToken(left_bracket)
-        )
-        self.inner = inner
-        self.right_bracket = (
-            (
-                right_bracket
-                if isinstance(right_bracket, BracketToken)
-                else BracketToken(right_bracket)
-            )
-            if right_bracket
-            else BracketToken(self.left_bracket.get_other())
-        )
-
-    def visit_topdown(
-        self,
-        visitor: typing.Callable[["AbstractExpression", "AbstractExpression"], None],
-        previous=None,
-    ):
-        visitor(previous, self)
-        self.inner.visit_topdown(visitor, self)
-
-    def visit_depth_first(
-        self,
-        visitor: typing.Callable[["AbstractExpression", "AbstractExpression"], None],
-        previous=None,
-    ):
-        self.inner.visit_depth_first(visitor, self)
-        visitor(previous, self)
-
-    def replace_inner(
-        self, node: "AbstractExpression", replacement: "AbstractExpression"
-    ):
-        if id(node) == id(self.inner):
-            self.inner = replacement
-        else:
-            raise ValueError(node)
-
-    def __eq__(self, other):
-        return (
-            type(other) == type(self)
-            and self.left_bracket == other.left_bracket
-            and self.inner == other.inner
-            and self.right_bracket == other.right_bracket
-        )
-
-    def __repr__(self):
-        return f"BracketExpression({self.left_bracket}, {self.inner}, {self.right_bracket})"
-
-    def copy(self):
-        return BracketExpression(
-            self.left_bracket,
-            self.inner.copy(),
-            self.right_bracket,
-        )
-
-
-class BinaryExpression(AbstractExpression):
-    def __init__(
-        self,
-        lhs: AbstractExpression,
-        operator: BinaryOperatorToken | str,
-        rhs: AbstractExpression,
-    ):
-        self.lhs = lhs
-        self.operator = (
-            operator
-            if isinstance(operator, BinaryOperatorToken)
-            else BinaryOperatorToken(operator)
-        )
-        self.rhs = rhs
-
-    def visit_topdown(
-        self,
-        visitor: typing.Callable[["AbstractExpression", "AbstractExpression"], None],
-        previous=None,
-    ):
-        visitor(previous, self)
-        self.lhs.visit_topdown(visitor, self)
-        self.rhs.visit_topdown(visitor, self)
-
-    def visit_depth_first(
-        self,
-        visitor: typing.Callable[["AbstractExpression", "AbstractExpression"], None],
-        previous=None,
-    ):
-        self.lhs.visit_depth_first(visitor, self)
-        self.rhs.visit_depth_first(visitor, self)
-        visitor(previous, self)
-
-    def replace_inner(
-        self, node: "AbstractExpression", replacement: "AbstractExpression"
-    ):
-        if id(node) == id(self.lhs):
-            self.lhs = replacement
-        elif id(node) == id(self.rhs):
-            self.rhs = replacement
-        else:
-            raise ValueError(node)
-
-    def __eq__(self, other):
-        return (
-            type(other) == type(self)
-            and self.lhs == other.lhs
-            and self.operator == other.operator
-            and self.rhs == other.rhs
-        )
-
-    def __repr__(self):
-        return f"BinaryExpression({self.lhs}, {self.operator}, {self.rhs})"
-
-    def copy(self):
-        return BinaryExpression(self.lhs.copy(), self.operator, self.rhs.copy())
-
-
-class IdentifierExpression(AbstractExpression):
-    def __init__(self, token: IntegerToken | str):
-        self.token = (
-            token if isinstance(token, IdentifierToken) else IdentifierToken(token)
-        )
-
-    def __eq__(self, other):
-        return type(other) == type(self) and self.token == other.token
-
-    def __repr__(self):
-        return f"IdentifierExpression({self.token})"
-
-    def copy(self) -> "IdentifierExpression":
-        return IdentifierExpression(self.token)
-
-
-def raise_syntax_error(token: AbstractToken, message: str, arg):
-    raise SyntaxError(f"{token}: {message}")
-
-
-class AbstractParser(AbstractCursorStateItem, abc.ABC):
-    def __init__(self, tokens: typing.List[AbstractToken]):
-        super().__init__()
-        self.tokens = tokens
-    def __getitem__(
-        self, item: int | slice
-    ) -> AbstractToken | typing.List[AbstractToken] | None:
-        if isinstance(item, int):
-            index = self.cursor + item
-
-            if index < 0 or index >= len(self.tokens):
-                return
-
-            return self.tokens[index]
-
-        elif isinstance(item, slice):
-            start = self.cursor + item.start
-            stop = (self.cursor + item.stop) if item.stop else None
-            step = item.step if item.step is not None else 1
-
-            if (
-                start < 0
-                or start >= len(self.tokens)
-                or stop < 0
-                or stop >= len(self.tokens)
-            ):
-                return
-
-            return self.tokens[start:stop:step]
-
-        raise IndexError(item)
-
-    def is_empty(self) -> bool:
-        return len(self.tokens) == self.cursor + 1
-
-    def assert_EOF(self):
-        if not self.is_empty():
-            raise SyntaxError("EOF expected")
-
-    def inspect(self, eof_allowed=False) -> AbstractToken:
-        if self.is_empty():
-            raise SyntaxError("EOF reached!")
-
-        token = self.tokens[self.cursor]
-
-        if isinstance(token, EndOfFileToken) and not eof_allowed:
-            raise SyntaxError("EOF reached!")
-
-        return token
-
-    def try_inspect(self, eof_allowed=False) -> AbstractToken | None:
-        if self.is_empty():
-            return
-
-        token = self.tokens[self.cursor]
-
-        if isinstance(token, EndOfFileToken) and not eof_allowed:
-            return
-
-        return token
-
-    T = typing.TypeVar(
-        "T", AbstractToken, typing.List[typing.Type[AbstractToken] | AbstractToken]
-    )
-
-    def consume(self, expected: T | typing.Type[T], err_arg=None) -> T:
-        """
-        Consumes a token and compares it against the 'expected' (which is an instance or the expected type of token)
-
-        :return: the parsed token
-        :raises SyntaxError: if it failed to parse the token (either invalid type or end of stream)
-        """
-        token: AbstractToken = self.inspect()
-
-        if expected:
-            if isinstance(expected, AbstractToken):
-                if token != expected:
-                    raise_syntax_error(token, f"Expected {expected}", err_arg)
-                    raise SyntaxError
-
-            elif isinstance(expected, list):
-                for element in expected:
-                    if isinstance(element, AbstractToken):
-                        if token == element:
-                            break
-                    else:
-                        if isinstance(token, element):
-                            break
-                else:
-                    raise SyntaxError(
-                        f"Expected any of {repr(list(expected))[1:-1]}, got {token} (at token token position: {self.cursor+1})"
-                    )
-
-            else:
-                if not isinstance(token, expected):
-                    raise SyntaxError(
-                        f"Expected type {expected.__name__}, got {token} (type: {type(token).__name__})"
-                    )
-
-        self.cursor += 1
-
-        return token
-
-    def try_consume(self, expected: T | typing.Type[T]) -> T | None:
-        """
-        Tries to consume a token from the token stream
-
-        :param expected: the expected type of token, either instance or type
-        :return: the consumed token or None
-        """
-        token: AbstractToken = self.try_inspect()
-
-        if token is None:
-            return
-
-        if expected:
-            if isinstance(expected, AbstractToken):
-                if token != expected:
-                    return
-
-            elif isinstance(expected, (list, tuple)):
-                for element in expected:
-                    if isinstance(element, AbstractToken):
-                        if token == element:
-                            break
-                    else:
-                        if isinstance(token, element):
-                            break
-                else:
-                    return
-            else:
-                if not isinstance(token, expected):
-                    return
-
-        self.cursor += 1
-
-        return token
-
-    def try_consume_multi(
-        self, elements: typing.List[T | typing.Type[T]]
-    ) -> typing.List[T] | None:
-        """
-        Tries to consume multiple tokens at ones, and fails completely if any fails to be parsed
-
-        :param elements: the stuff to be parsed, like the parameters to try_consume(...)
-        :return: a list of tokens, or None in case of a parsing error
-        """
-
-        self.save()
-        parsed: typing.List[AbstractParser.T | typing.Type[AbstractParser.T]] = []
-
-        for element in elements:
-            if expr := self.try_consume(element):
-                expr: AbstractParser.T | typing.Type[AbstractParser.T]
-                parsed.append(expr)
-                continue
-
-            self.rollback()
-            return
-
-        self.discard_save()
-        return parsed
-
-    def parse(self) -> AbstractExpression:
-        raise NotImplementedError
+import abc
+import typing
+from bytecodemanipulation.assembler.util.tokenizer import (
+    AbstractToken,
+    IntegerToken,
+    BinaryOperatorToken,
+    BracketToken,
+    IdentifierToken,
+    EndOfFileToken,
+)
+from .CommonUtil import AbstractCursorStateItem
+
+
+class AbstractExpression(abc.ABC):
+    def visit_topdown(
+        self,
+        visitor: typing.Callable[["AbstractExpression", "AbstractExpression"], None],
+        previous=None,
+    ):
+        visitor(self)
+
+    def visit_depth_first(
+        self,
+        visitor: typing.Callable[["AbstractExpression", "AbstractExpression"], None],
+        previous=None,
+    ):
+        visitor(previous, self)
+
+    def copy(self) -> "AbstractExpression":
+        raise NotImplementedError
+
+    def __copy__(self):
+        return self.copy()
+
+    def __deepcopy__(self):
+        return self.copy()
+
+    def replace_inner(
+        self, node: "AbstractExpression", replacement: "AbstractExpression"
+    ):
+        raise ValueError(node)
+
+
+class NumericExpression(AbstractExpression):
+    def __init__(self, token: IntegerToken | str):
+        self.token = token if isinstance(token, IntegerToken) else IntegerToken(token)
+
+    def __eq__(self, other):
+        return type(other) == type(self) and self.token == other.token
+
+    def __repr__(self):
+        return f"IntegerExpression({self.token})"
+
+    def copy(self) -> "NumericExpression":
+        return NumericExpression(self.token)
+
+
+class BracketExpression(AbstractExpression):
+    def __init__(
+        self,
+        left_bracket: BracketToken | str,
+        inner: AbstractExpression,
+        right_bracket: BracketToken | str = None,
+    ):
+        self.left_bracket = (
+            left_bracket
+            if isinstance(left_bracket, BracketToken)
+            else BracketToken(left_bracket)
+        )
+        self.inner = inner
+        self.right_bracket = (
+            (
+                right_bracket
+                if isinstance(right_bracket, BracketToken)
+                else BracketToken(right_bracket)
+            )
+            if right_bracket
+            else BracketToken(self.left_bracket.get_other())
+        )
+
+    def visit_topdown(
+        self,
+        visitor: typing.Callable[["AbstractExpression", "AbstractExpression"], None],
+        previous=None,
+    ):
+        visitor(previous, self)
+        self.inner.visit_topdown(visitor, self)
+
+    def visit_depth_first(
+        self,
+        visitor: typing.Callable[["AbstractExpression", "AbstractExpression"], None],
+        previous=None,
+    ):
+        self.inner.visit_depth_first(visitor, self)
+        visitor(previous, self)
+
+    def replace_inner(
+        self, node: "AbstractExpression", replacement: "AbstractExpression"
+    ):
+        if id(node) == id(self.inner):
+            self.inner = replacement
+        else:
+            raise ValueError(node)
+
+    def __eq__(self, other):
+        return (
+            type(other) == type(self)
+            and self.left_bracket == other.left_bracket
+            and self.inner == other.inner
+            and self.right_bracket == other.right_bracket
+        )
+
+    def __repr__(self):
+        return f"BracketExpression({self.left_bracket}, {self.inner}, {self.right_bracket})"
+
+    def copy(self):
+        return BracketExpression(
+            self.left_bracket,
+            self.inner.copy(),
+            self.right_bracket,
+        )
+
+
+class BinaryExpression(AbstractExpression):
+    def __init__(
+        self,
+        lhs: AbstractExpression,
+        operator: BinaryOperatorToken | str,
+        rhs: AbstractExpression,
+    ):
+        self.lhs = lhs
+        self.operator = (
+            operator
+            if isinstance(operator, BinaryOperatorToken)
+            else BinaryOperatorToken(operator)
+        )
+        self.rhs = rhs
+
+    def visit_topdown(
+        self,
+        visitor: typing.Callable[["AbstractExpression", "AbstractExpression"], None],
+        previous=None,
+    ):
+        visitor(previous, self)
+        self.lhs.visit_topdown(visitor, self)
+        self.rhs.visit_topdown(visitor, self)
+
+    def visit_depth_first(
+        self,
+        visitor: typing.Callable[["AbstractExpression", "AbstractExpression"], None],
+        previous=None,
+    ):
+        self.lhs.visit_depth_first(visitor, self)
+        self.rhs.visit_depth_first(visitor, self)
+        visitor(previous, self)
+
+    def replace_inner(
+        self, node: "AbstractExpression", replacement: "AbstractExpression"
+    ):
+        if id(node) == id(self.lhs):
+            self.lhs = replacement
+        elif id(node) == id(self.rhs):
+            self.rhs = replacement
+        else:
+            raise ValueError(node)
+
+    def __eq__(self, other):
+        return (
+            type(other) == type(self)
+            and self.lhs == other.lhs
+            and self.operator == other.operator
+            and self.rhs == other.rhs
+        )
+
+    def __repr__(self):
+        return f"BinaryExpression({self.lhs}, {self.operator}, {self.rhs})"
+
+    def copy(self):
+        return BinaryExpression(self.lhs.copy(), self.operator, self.rhs.copy())
+
+
+class IdentifierExpression(AbstractExpression):
+    def __init__(self, token: IntegerToken | str):
+        self.token = (
+            token if isinstance(token, IdentifierToken) else IdentifierToken(token)
+        )
+
+    def __eq__(self, other):
+        return type(other) == type(self) and self.token == other.token
+
+    def __repr__(self):
+        return f"IdentifierExpression({self.token})"
+
+    def copy(self) -> "IdentifierExpression":
+        return IdentifierExpression(self.token)
+
+
+def raise_syntax_error(token: AbstractToken, message: str, arg):
+    raise SyntaxError(f"{token}: {message}")
+
+
+class AbstractParser(AbstractCursorStateItem, abc.ABC):
+    def __init__(self, tokens: typing.List[AbstractToken]):
+        super().__init__()
+        self.tokens = tokens
+
+    def __getitem__(
+        self, item: int | slice
+    ) -> AbstractToken | typing.List[AbstractToken] | None:
+        if isinstance(item, int):
+            index = self.cursor + item
+
+            if index < 0 or index >= len(self.tokens):
+                return
+
+            return self.tokens[index]
+
+        elif isinstance(item, slice):
+            start = self.cursor + item.start
+            stop = (self.cursor + item.stop) if item.stop else None
+            step = item.step if item.step is not None else 1
+
+            if (
+                start < 0
+                or start >= len(self.tokens)
+                or stop < 0
+                or stop >= len(self.tokens)
+            ):
+                return
+
+            return self.tokens[start:stop:step]
+
+        raise IndexError(item)
+
+    def is_empty(self) -> bool:
+        return len(self.tokens) == self.cursor + 1
+
+    def assert_EOF(self):
+        if not self.is_empty():
+            raise SyntaxError("EOF expected")
+
+    def inspect(self, eof_allowed=False) -> AbstractToken:
+        if self.is_empty():
+            raise SyntaxError("EOF reached!")
+
+        token = self.tokens[self.cursor]
+
+        if isinstance(token, EndOfFileToken) and not eof_allowed:
+            raise SyntaxError("EOF reached!")
+
+        return token
+
+    def try_inspect(self, eof_allowed=False) -> AbstractToken | None:
+        if self.is_empty():
+            return
+
+        token = self.tokens[self.cursor]
+
+        if isinstance(token, EndOfFileToken) and not eof_allowed:
+            return
+
+        return token
+
+    T = typing.TypeVar(
+        "T", AbstractToken, typing.List[typing.Type[AbstractToken] | AbstractToken]
+    )
+
+    def consume(self, expected: T | typing.Type[T], err_arg=None) -> T:
+        """
+        Consumes a token and compares it against the 'expected' (which is an instance or the expected type of token)
+
+        :return: the parsed token
+        :raises SyntaxError: if it failed to parse the token (either invalid type or end of stream)
+        """
+        token: AbstractToken = self.inspect()
+
+        if expected:
+            if isinstance(expected, AbstractToken):
+                if token != expected:
+                    raise_syntax_error(token, f"Expected {expected}", err_arg)
+                    raise SyntaxError
+
+            elif isinstance(expected, list):
+                for element in expected:
+                    if isinstance(element, AbstractToken):
+                        if token == element:
+                            break
+                    else:
+                        if isinstance(token, element):
+                            break
+                else:
+                    raise SyntaxError(
+                        f"Expected any of {repr(list(expected))[1:-1]}, got {token} (at token token position: {self.cursor+1})"
+                    )
+
+            else:
+                if not isinstance(token, expected):
+                    raise SyntaxError(
+                        f"Expected type {expected.__name__}, got {token} (type: {type(token).__name__})"
+                    )
+
+        self.cursor += 1
+
+        return token
+
+    def try_consume(self, expected: T | typing.Type[T]) -> T | None:
+        """
+        Tries to consume a token from the token stream
+
+        :param expected: the expected type of token, either instance or type
+        :return: the consumed token or None
+        """
+        token: AbstractToken = self.try_inspect()
+
+        if token is None:
+            return
+
+        if expected:
+            if isinstance(expected, AbstractToken):
+                if token != expected:
+                    return
+
+            elif isinstance(expected, (list, tuple)):
+                for element in expected:
+                    if isinstance(element, AbstractToken):
+                        if token == element:
+                            break
+                    else:
+                        if isinstance(token, element):
+                            break
+                else:
+                    return
+            else:
+                if not isinstance(token, expected):
+                    return
+
+        self.cursor += 1
+
+        return token
+
+    def try_consume_multi(
+        self, elements: typing.List[T | typing.Type[T]]
+    ) -> typing.List[T] | None:
+        """
+        Tries to consume multiple tokens at ones, and fails completely if any fails to be parsed
+
+        :param elements: the stuff to be parsed, like the parameters to try_consume(...)
+        :return: a list of tokens, or None in case of a parsing error
+        """
+
+        self.save()
+        parsed: typing.List[AbstractParser.T | typing.Type[AbstractParser.T]] = []
+
+        for element in elements:
+            if expr := self.try_consume(element):
+                expr: AbstractParser.T | typing.Type[AbstractParser.T]
+                parsed.append(expr)
+                continue
+
+            self.rollback()
+            return
+
+        self.discard_save()
+        return parsed
+
+    def parse(self) -> AbstractExpression:
+        raise NotImplementedError
```

### Comparing `bytecodemanipulation-0.2.4/bytecodemanipulation/assembler/util/tokenizer.py` & `bytecodemanipulation-0.2.8/bytecodemanipulation/assembler/util/tokenizer.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,303 +1,303 @@
-import abc
-import typing
-
-from .CommonUtil import AbstractCursorStateItem
-
-
-class AbstractToken(abc.ABC):
-    __slots__ = ("text", "line", "column", "span")
-
-    def __init__(self, text: str):
-        self.text = text
-        self.line: int | None = None
-        self.column: int | None = None
-        self.span: int | None = None
-
-    def __eq__(self, other):
-        return type(other) == type(self) and self.text == other.text
-
-    def __repr__(self):
-        return f"{type(self).__name__}({repr(self.text)})"
-
-
-class IntegerToken(AbstractToken):
-    pass
-
-
-class FloatToken(AbstractToken):
-    pass
-
-
-class BinaryOperatorToken(AbstractToken):
-    pass
-
-
-class BracketToken(AbstractToken):
-    def is_opening(self) -> bool:
-        return self.text in "([{<"
-
-    def get_other(self) -> str:
-        match self.text:
-            case "(":
-                return ")"
-            case ")":
-                return "("
-            case "[":
-                return "]"
-            case "]":
-                return "["
-            case "{":
-                return "}"
-            case "}":
-                return "{"
-            case "<":
-                return ">"
-            case ">":
-                return "<"
-
-        raise NotImplementedError
-
-
-class IdentifierToken(AbstractToken):
-    pass
-
-
-class CommentToken(AbstractToken):
-    pass
-
-
-class StringLiteralToken(AbstractToken):
-    __slots__ = ("text", "quotes")
-
-    def __init__(self, string: str, quotes: str):
-        super().__init__(string)
-        self.quotes = quotes
-
-    def __eq__(self, other):
-        return (
-            type(other) == type(self)
-            and self.text == other.text
-            and self.quotes == other.quotes
-        )
-
-    def __repr__(self):
-        return f"{type(self).__name__}({repr(self.text)}, {self.quotes})"
-
-
-class EndOfFileToken(AbstractToken):
-    def __init__(self):
-        super().__init__("")
-
-
-class AbstractLexer(AbstractCursorStateItem, abc.ABC):
-    """
-    Base class for Lexers (also known as Tokenizers)
-
-    Contains handling code for a linear tokenizer,
-    and functions for collecting text easily.
-    """
-
-    INCLUDE_LINE_INFO = True
-
-    def __init__(self, text: str, initial_line_offset=0):
-        super().__init__()
-        self.text = text
-        self.old_line_number = 1
-        self.old_column_number = 0
-        self._line_offset = initial_line_offset
-
-    def add_line_offset(self, offset: int):
-        self._line_offset += offset
-        return self
-
-    def is_empty(self) -> bool:
-        """
-        Checks if no text is left to visit
-        """
-        return len(self.text) <= self.cursor
-
-    def assert_EOF(self):
-        """
-        asserts that EOF is reached
-
-        :raises SyntaxError: if EOF is not reached
-        """
-        if not self.is_empty():
-            raise SyntaxError("EOF expected")
-
-    def inspect(self) -> str:
-        """
-        Returns the current char the cursor is at
-
-        :raises SyntaxError: when the cursor is outside the bounds of the text
-        """
-        if self.is_empty():
-            raise SyntaxError("EOF reached!")
-
-        return self.text[self.cursor]
-
-    def try_inspect_multi(self, count: int) -> str | None:
-        if len(self.text) < self.cursor + count:
-            return
-
-        return self.text[self.cursor : self.cursor + count]
-
-    def try_inspect(self) -> str | None:
-        """
-        Returns the current char the cursor is at, or None
-        """
-        if self.is_empty():
-            return
-
-        return self.text[self.cursor]
-
-    def consume(self, expected: str = None) -> str:
-        """
-        Returns the current char the cursor is at, and increments the cursor
-
-        :raises SyntaxError: when the cursor is outside the bounds of the text
-        """
-        t = self.inspect()
-
-        if expected and t not in expected:
-            raise SyntaxError(
-                f"Expected any of {repr(list(expected))[1:-1]}, got '{t}' (at position {self.cursor+1})"
-            )
-
-        self.cursor += 1
-        return t
-
-    def consume_multi(self, count: int, expected: str = None):
-        t = self.try_inspect_multi(count)
-
-        if expected and t not in expected:
-            raise SyntaxError(
-                f"Expected any of {repr(list(expected))[1:-1]}, got {t} (at position {self.cursor + 1})"
-            )
-
-        self.cursor += count
-        return t
-
-    def try_consume(self, expected: str = None) -> str | None:
-        """
-        Returns the current char the cursor is at and increments the cursor, or None
-        """
-        t = self.try_inspect()
-
-        if t is None or (expected and t not in expected):
-            return
-
-        self.cursor += 1
-        return t
-
-    def try_consume_multi(self, count: int, expected: str = None) -> str | None:
-        t = self.try_inspect_multi(count)
-
-        if t is None or (expected and t not in expected):
-            return
-
-        self.cursor += count
-        return t
-
-    def consume_while(self, predicate: typing.Callable[[str, str], bool] | str):
-        """
-        Consumes chars while predicate(text, char) returns True
-
-        :param predicate: the predicate
-        """
-        if isinstance(predicate, str):
-            options = set(predicate)
-            predicate = lambda _, char: char in options
-
-        text = ""
-
-        while not self.is_empty() and predicate(text, self.inspect()):
-            text += self.consume()
-
-        return text
-
-    def consume_until(
-        self, predicate: typing.Callable[[str, str], bool] | str, include=True
-    ):
-        """
-        Consumes chars while predicate(text, char) returns False
-
-        :param predicate: the predicate
-        :param include: if to include when the predicate is met
-        """
-        if isinstance(predicate, str):
-            options = set(predicate)
-            predicate = lambda _, char: char in options
-
-        text = ""
-
-        while not self.is_empty() and not predicate(text, self.inspect()):
-            text += self.consume()
-
-        if include:
-            text += self.consume()
-
-        return text
-
-    def lex(self) -> typing.List[AbstractToken]:
-        """
-        Lex-es the text the object was constructed from.
-        Returns the list of tokens.
-        """
-        skipped = 0
-        self.old_column_number = 0
-
-        tokens = []
-        while not self.is_empty():
-            old_cursor = self.cursor
-
-            try:
-                result = self.lex_single()
-            except SyntaxError:
-                print(tokens)
-                raise
-
-            if self.cursor == old_cursor:
-                print(result, tokens)
-                raise RuntimeError("Lexer did not increment cursor!")
-
-            if result is None:
-                skipped += self.cursor - old_cursor
-                self.old_column_number += self.cursor - old_cursor
-                continue
-
-            if self.INCLUDE_LINE_INFO:
-                partial = self.text[old_cursor - skipped : self.cursor]
-                whitespace_count = len(partial) - len(partial.lstrip())
-
-                self.old_line_number += partial.count("\n")
-                if "\n" in partial[:whitespace_count]:
-                    self.old_column_number = len(partial.split("\n")[-1]) - len(
-                        partial.split("\n")[-1].lstrip()
-                    )
-
-                for r in result if isinstance(result, list) else (result,):
-                    newline_count = partial[:whitespace_count].count("\n")
-                    r.line = self.old_line_number + self._line_offset - 1
-                    r.column = self.old_column_number - newline_count
-                    r.span = self.cursor - old_cursor
-
-                    # print(
-                    #     f"parsed string '{repr(partial)[1:-1]}' (line: {r.line}, column: {r.column}, span: {r.span})"
-                    # )
-
-                    self.old_column_number += r.span
-
-                skipped = 0
-
-            if isinstance(result, list):
-                tokens += result
-            else:
-                tokens.append(result)
-
-        tokens.append(EndOfFileToken())
-
-        return tokens
-
-    def lex_single(self) -> typing.List[AbstractToken] | AbstractToken | None:
-        raise NotImplementedError()
+import abc
+import typing
+
+from .CommonUtil import AbstractCursorStateItem
+
+
+class AbstractToken(abc.ABC):
+    __slots__ = ("text", "line", "column", "span")
+
+    def __init__(self, text: str):
+        self.text = text
+        self.line: int | None = None
+        self.column: int | None = None
+        self.span: int | None = None
+
+    def __eq__(self, other):
+        return type(other) == type(self) and self.text == other.text
+
+    def __repr__(self):
+        return f"{type(self).__name__}({repr(self.text)})"
+
+
+class IntegerToken(AbstractToken):
+    pass
+
+
+class FloatToken(AbstractToken):
+    pass
+
+
+class BinaryOperatorToken(AbstractToken):
+    pass
+
+
+class BracketToken(AbstractToken):
+    def is_opening(self) -> bool:
+        return self.text in "([{<"
+
+    def get_other(self) -> str:
+        match self.text:
+            case "(":
+                return ")"
+            case ")":
+                return "("
+            case "[":
+                return "]"
+            case "]":
+                return "["
+            case "{":
+                return "}"
+            case "}":
+                return "{"
+            case "<":
+                return ">"
+            case ">":
+                return "<"
+
+        raise NotImplementedError
+
+
+class IdentifierToken(AbstractToken):
+    pass
+
+
+class CommentToken(AbstractToken):
+    pass
+
+
+class StringLiteralToken(AbstractToken):
+    __slots__ = ("text", "quotes")
+
+    def __init__(self, string: str, quotes: str):
+        super().__init__(string)
+        self.quotes = quotes
+
+    def __eq__(self, other):
+        return (
+            type(other) == type(self)
+            and self.text == other.text
+            and self.quotes == other.quotes
+        )
+
+    def __repr__(self):
+        return f"{type(self).__name__}({repr(self.text)}, {self.quotes})"
+
+
+class EndOfFileToken(AbstractToken):
+    def __init__(self):
+        super().__init__("")
+
+
+class AbstractLexer(AbstractCursorStateItem, abc.ABC):
+    """
+    Base class for Lexers (also known as Tokenizers)
+
+    Contains handling code for a linear tokenizer,
+    and functions for collecting text easily.
+    """
+
+    INCLUDE_LINE_INFO = True
+
+    def __init__(self, text: str, initial_line_offset=0):
+        super().__init__()
+        self.text = text
+        self.old_line_number = 1
+        self.old_column_number = 0
+        self._line_offset = initial_line_offset
+
+    def add_line_offset(self, offset: int):
+        self._line_offset += offset
+        return self
+
+    def is_empty(self) -> bool:
+        """
+        Checks if no text is left to visit
+        """
+        return len(self.text) <= self.cursor
+
+    def assert_EOF(self):
+        """
+        asserts that EOF is reached
+
+        :raises SyntaxError: if EOF is not reached
+        """
+        if not self.is_empty():
+            raise SyntaxError("EOF expected")
+
+    def inspect(self) -> str:
+        """
+        Returns the current char the cursor is at
+
+        :raises SyntaxError: when the cursor is outside the bounds of the text
+        """
+        if self.is_empty():
+            raise SyntaxError("EOF reached!")
+
+        return self.text[self.cursor]
+
+    def try_inspect_multi(self, count: int) -> str | None:
+        if len(self.text) < self.cursor + count:
+            return
+
+        return self.text[self.cursor : self.cursor + count]
+
+    def try_inspect(self) -> str | None:
+        """
+        Returns the current char the cursor is at, or None
+        """
+        if self.is_empty():
+            return
+
+        return self.text[self.cursor]
+
+    def consume(self, expected: str = None) -> str:
+        """
+        Returns the current char the cursor is at, and increments the cursor
+
+        :raises SyntaxError: when the cursor is outside the bounds of the text
+        """
+        t = self.inspect()
+
+        if expected and t not in expected:
+            raise SyntaxError(
+                f"Expected any of {repr(list(expected))[1:-1]}, got '{t}' (at position {self.cursor+1})"
+            )
+
+        self.cursor += 1
+        return t
+
+    def consume_multi(self, count: int, expected: str = None):
+        t = self.try_inspect_multi(count)
+
+        if expected and t not in expected:
+            raise SyntaxError(
+                f"Expected any of {repr(list(expected))[1:-1]}, got {t} (at position {self.cursor + 1})"
+            )
+
+        self.cursor += count
+        return t
+
+    def try_consume(self, expected: str = None) -> str | None:
+        """
+        Returns the current char the cursor is at and increments the cursor, or None
+        """
+        t = self.try_inspect()
+
+        if t is None or (expected and t not in expected):
+            return
+
+        self.cursor += 1
+        return t
+
+    def try_consume_multi(self, count: int, expected: str = None) -> str | None:
+        t = self.try_inspect_multi(count)
+
+        if t is None or (expected and t not in expected):
+            return
+
+        self.cursor += count
+        return t
+
+    def consume_while(self, predicate: typing.Callable[[str, str], bool] | str):
+        """
+        Consumes chars while predicate(text, char) returns True
+
+        :param predicate: the predicate
+        """
+        if isinstance(predicate, str):
+            options = set(predicate)
+            predicate = lambda _, char: char in options
+
+        text = ""
+
+        while not self.is_empty() and predicate(text, self.inspect()):
+            text += self.consume()
+
+        return text
+
+    def consume_until(
+        self, predicate: typing.Callable[[str, str], bool] | str, include=True
+    ):
+        """
+        Consumes chars while predicate(text, char) returns False
+
+        :param predicate: the predicate
+        :param include: if to include when the predicate is met
+        """
+        if isinstance(predicate, str):
+            options = set(predicate)
+            predicate = lambda _, char: char in options
+
+        text = ""
+
+        while not self.is_empty() and not predicate(text, self.inspect()):
+            text += self.consume()
+
+        if include:
+            text += self.consume()
+
+        return text
+
+    def lex(self) -> typing.List[AbstractToken]:
+        """
+        Lex-es the text the object was constructed from.
+        Returns the list of tokens.
+        """
+        skipped = 0
+        self.old_column_number = 0
+
+        tokens = []
+        while not self.is_empty():
+            old_cursor = self.cursor
+
+            try:
+                result = self.lex_single()
+            except SyntaxError:
+                print(tokens)
+                raise
+
+            if self.cursor == old_cursor:
+                print(result, tokens)
+                raise RuntimeError("Lexer did not increment cursor!")
+
+            if result is None:
+                skipped += self.cursor - old_cursor
+                self.old_column_number += self.cursor - old_cursor
+                continue
+
+            if self.INCLUDE_LINE_INFO:
+                partial = self.text[old_cursor - skipped : self.cursor]
+                whitespace_count = len(partial) - len(partial.lstrip())
+
+                self.old_line_number += partial.count("\n")
+                if "\n" in partial[:whitespace_count]:
+                    self.old_column_number = len(partial.split("\n")[-1]) - len(
+                        partial.split("\n")[-1].lstrip()
+                    )
+
+                for r in result if isinstance(result, list) else (result,):
+                    newline_count = partial[:whitespace_count].count("\n")
+                    r.line = self.old_line_number + self._line_offset
+                    r.column = self.old_column_number - newline_count
+                    r.span = self.cursor - old_cursor
+
+                    # print(
+                    #     f"parsed string '{repr(partial)[1:-1]}' (line: {r.line}, column: {r.column}, span: {r.span})"
+                    # )
+
+                    self.old_column_number += r.span
+
+                skipped = 0
+
+            if isinstance(result, list):
+                tokens += result
+            else:
+                tokens.append(result)
+
+        tokens.append(EndOfFileToken())
+
+        return tokens
+
+    def lex_single(self) -> typing.List[AbstractToken] | AbstractToken | None:
+        raise NotImplementedError()
```

### Comparing `bytecodemanipulation-0.2.4/bytecodemanipulation/data/shared/builtin_spec.py` & `bytecodemanipulation-0.2.8/bytecodemanipulation/data/shared/builtin_spec.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,420 +1,420 @@
-import typing
-import random
-
-from bytecodemanipulation.Opcodes import Opcodes
-from bytecodemanipulation.Specialization import SpecializationContainer, register
-from bytecodemanipulation.MutableFunction import Instruction
-
-
-ASSERT_TYPE_CASTS = False
-DISCARD_ALL_ANY_WITHOUT_SIDE_EFFECT_CHECK = True
-
-
-@register(typing.cast)
-def specialize_typing_cast(container: SpecializationContainer):
-    # typing.cast(<type>, <obj>) -> <obj>
-    data_type, value = container.get_arg_specifications()
-
-    if ASSERT_TYPE_CASTS:
-        # todo: add check type
-        pass
-
-    container.replace_call_with_arg(value)
-
-
-@register(min)
-def specialize_min(container: SpecializationContainer):
-    # remove when constants are mixed with no constant all but the smallest constant
-    args = container.get_arg_specifications()
-
-    if args[0].is_self:
-        self = args.pop(0)
-    else:
-        self = None
-
-    min_const: Instruction = None
-
-    # todo: catch compare exceptions
-    for arg in args:
-        instr: Instruction = arg.get_normalized_data_instr()
-
-        if instr and instr.has_constant():
-            if min_const is None or min_const.arg_value > instr.arg_value:
-                min_const = instr
-
-    if min_const is not None:
-        # todo: for non constants, do a clever try-eval-ahead with the type if arrival
-
-        for arg in args:
-            norm_instr = arg.get_normalized_data_instr()
-            if norm_instr and norm_instr != min_const and norm_instr.has_constant():
-                arg.discard()
-
-
-@register(max)
-def specialize_min(container: SpecializationContainer):
-    # remove when constants are mixed with no constant all but the smallest constant
-    args = container.get_arg_specifications()
-
-    if args[0].is_self:
-        self = args.pop(0)
-    else:
-        self = None
-
-    min_const: Instruction = None
-
-    # todo: catch compare exceptions
-    for arg in args:
-        instr: Instruction = arg.get_normalized_data_instr()
-
-        if instr and instr.has_constant():
-            if min_const is None or min_const.arg_value < instr.arg_value:
-                min_const = instr
-
-    if min_const is not None:
-        # todo: for non constants, do a clever try-eval-ahead with the type if arrival
-
-        for arg in args:
-            norm_instr = arg.get_normalized_data_instr()
-            if norm_instr and norm_instr != min_const and norm_instr.has_constant():
-                arg.discard()
-
-
-@register(tuple)
-def create_empty_tuple(container: SpecializationContainer):
-    if len(container.get_arg_specifications()) == 0:
-        container.replace_with_constant_value(tuple())
-
-
-def _check_int(c) -> bool:
-    if isinstance(c, int):
-        return True
-    if isinstance(c, float):
-        return int(c) == c
-    return False
-
-
-@register(range)
-@register(random.randrange)
-@register(random.Random.randrange)
-def specialize_range_3rd_argument(container: SpecializationContainer):
-    args = container.get_arg_specifications()
-    sources = [arg.get_normalized_data_instr() for arg in args]
-
-    # Argument length checks and type checks
-    if len(sources) in (1, 2, 3):
-        if sources[0].opcode == Opcodes.LOAD_CONST:
-            container.replace_with_raise_exception_if(
-                not _check_int(sources[0].arg_value),
-                lambda: TypeError(
-                    f"'{type(sources[0].arg_value).__name__}' object cannot be interpreted as an integer"
-                ),
-                arg=0,
-            )
-
-        if len(sources) > 1 and sources[1].opcode == Opcodes.LOAD_CONST:
-            container.replace_with_raise_exception_if(
-                not _check_int(sources[1].arg_value),
-                lambda: TypeError(
-                    f"'{type(sources[1].arg_value).__name__}' object cannot be interpreted as an integer"
-                ),
-                arg=1,
-            )
-
-        if (
-            len(sources) == 2
-            and sources[0].opcode == sources[1].opcode == Opcodes.LOAD_CONST
-            and sources[0].arg_value > sources[1].arg_value
-        ):
-            container.replace_with_constant_value(tuple())
-
-        if len(sources) > 2 and sources[2].opcode == Opcodes.LOAD_CONST:
-            if (
-                not container.replace_with_raise_exception_if(
-                    not _check_int(sources[2].arg_value),
-                    lambda: TypeError(
-                        f"'{type(sources[2].arg_value).__name__}' object cannot be interpreted as an integer"
-                    ),
-                    arg=2,
-                )
-                and sources[2].arg_value == 0
-            ):
-                container.replace_with_raise_exception(
-                    lambda: ValueError("range() arg 3 must not be zero"),
-                    arg=2,
-                )
-
-        if (
-            len(sources) == 3
-            and sources[0].opcode
-            == sources[1].opcode
-            == sources[2].opcode
-            == Opcodes.LOAD_CONST
-            and sources[0].arg_value > sources[1].arg_value
-            and sources[2].arg_value > 0
-        ):
-            container.replace_with_constant_value(tuple())
-
-        if (
-            len(sources) == 3
-            and sources[0].opcode
-            == sources[1].opcode
-            == sources[2].opcode
-            == Opcodes.LOAD_CONST
-            and sources[0].arg_value < sources[1].arg_value
-            and sources[2].arg_value < 0
-        ):
-            container.replace_with_constant_value(tuple())
-
-    elif len(sources) == 0:
-        if container.method_call_descriptor.lookup_method_instr.arg_value == range:
-            container.replace_with_raise_exception(
-                TypeError("range expected at least 1 argument, got 0")
-            )
-        elif (
-            container.method_call_descriptor.lookup_method_instr.arg_value
-            == random.randrange
-        ):
-            container.replace_with_raise_exception(
-                TypeError(
-                    "Random.randrange() missing 1 required positional argument: 'start'"
-                )
-            )
-        elif (
-            container.method_call_descriptor.lookup_method_instr.arg_value
-            == random.Random.randrange
-        ):
-            pass
-        else:
-            raise NotImplementedError
-    else:
-        if container.method_call_descriptor.lookup_method_instr.arg_value == range:
-            container.replace_with_raise_exception(
-                TypeError(f"range expected at most 3 arguments, got {len(sources)}")
-            )
-        elif (
-            container.method_call_descriptor.lookup_method_instr.arg_value
-            == random.randrange
-        ):
-            container.replace_with_raise_exception(
-                TypeError(
-                    f"Random.randrange() takes from 2 to 4 positional arguments but {len(sources)} were given"
-                )
-            )
-        elif (
-            container.method_call_descriptor.lookup_method_instr.arg_value
-            == random.Random.randrange
-        ):
-            container.replace_with_raise_exception(
-                TypeError(
-                    f"Random.randrange() takes from 2 to 4 positional arguments but {len(sources)} were given"
-                )
-            )
-        else:
-            raise NotImplementedError
-
-    if len(args) != 3:
-        return
-
-    if (
-        args[2]
-        and sources[2].opcode == Opcodes.LOAD_CONST
-        and sources[2].arg_value == 1
-    ):
-        args[2].discard()
-
-
-@register(range)
-@register(random.randrange)
-@register(random.Random.randrange)
-def specialize_range_start_0(container: SpecializationContainer):
-    args = container.get_arg_specifications()
-
-    if len(args) != 2:
-        return
-
-    if (
-        args[0]
-        and args[0].get_normalized_data_instr().opcode == Opcodes.LOAD_CONST
-        and args[0].get_normalized_data_instr().arg_value == 0
-    ):
-        args[0].discard()
-
-
-@register(range)
-def specialize_small_range(container: SpecializationContainer):
-    args = container.get_arg_specifications()
-
-    if len(args) == 1:
-        start = 0
-        instr = args[0].get_normalized_data_instr()
-
-        if not instr or instr.opcode != Opcodes.LOAD_CONST:
-            return
-
-        end = instr.arg_value
-    elif len(args) == 2:
-        instr = args[0].get_normalized_data_instr()
-        if not instr or instr.opcode != Opcodes.LOAD_CONST:
-            return
-        start = instr.arg_value
-
-        instr = args[1].get_normalized_data_instr()
-        if not instr or instr.opcode != Opcodes.LOAD_CONST:
-            return
-        end = instr.arg_value
-    else:
-        return
-
-    if start == end:
-        container.replace_with_constant_value(tuple())
-    elif start + 1 == end:
-        container.replace_with_constant_value((start,))
-    elif start + 2 == end:
-        container.replace_with_constant_value((start, start + 1))
-
-
-@register(all)
-def specialize_all(container: SpecializationContainer):
-    args = container.get_arg_specifications()
-
-    if len(args) != 1:
-        return
-
-    create_primitive_arg = args[0].get_normalized_data_instr()
-
-    if create_primitive_arg is None:
-        return
-
-    # todo: can we specialize more?
-    if create_primitive_arg.opcode not in (
-        Opcodes.BUILD_LIST,
-        Opcodes.BUILD_TUPLE,
-        Opcodes.BUILD_SET,
-    ):
-        return
-
-    primitive_creation_args = [
-        (
-            create_primitive_arg.trace_normalized_stack_position(i),
-            next(create_primitive_arg.trace_stack_position(i)),
-        )
-        for i in range(create_primitive_arg.arg)
-    ]
-
-    defined_result = None
-    arg_count = len(primitive_creation_args)
-
-    for normal, real in primitive_creation_args:
-        if normal:
-            if normal.opcode != Opcodes.LOAD_CONST:
-                continue
-
-            if not normal.arg_value:
-                if DISCARD_ALL_ANY_WITHOUT_SIDE_EFFECT_CHECK:
-                    defined_result = False
-                    break
-            else:
-                real.change_opcode(Opcodes.NOP)
-                arg_count -= 1
-
-    if arg_count == 0:
-        defined_result = True
-
-    if defined_result is not None:
-        for _, real in primitive_creation_args:
-            real.change_opcode(Opcodes.NOP)
-
-        create_primitive_arg.change_opcode(Opcodes.NOP)
-        container.replace_with_constant_value(defined_result)
-    elif arg_count == 1:
-        create_primitive_arg.change_opcode(Opcodes.NOP)
-        container.replace_call_with_arg(args[0])
-    elif arg_count != create_primitive_arg.arg:
-        create_primitive_arg.change_arg(arg_count)
-
-        container.no_special = False
-
-
-@register(any)
-def specialize_any(container: SpecializationContainer):
-    args = container.get_arg_specifications()
-
-    if len(args) != 1:
-        return
-
-    create_primitive_arg = args[0].get_normalized_data_instr()
-
-    if create_primitive_arg is None:
-        return
-
-    # todo: can we specialize more?
-    if create_primitive_arg.opcode not in (
-        Opcodes.BUILD_LIST,
-        Opcodes.BUILD_TUPLE,
-        Opcodes.BUILD_SET,
-    ):
-        return
-
-    primitive_creation_args = [
-        (
-            create_primitive_arg.trace_normalized_stack_position(i),
-            next(create_primitive_arg.trace_stack_position(i)),
-        )
-        for i in range(create_primitive_arg.arg)
-    ]
-
-    defined_result = None
-    arg_count = len(primitive_creation_args)
-
-    for normal, real in primitive_creation_args:
-        if normal:
-            if normal.opcode != Opcodes.LOAD_CONST:
-                continue
-
-            if normal.arg_value:
-                if DISCARD_ALL_ANY_WITHOUT_SIDE_EFFECT_CHECK:
-                    defined_result = True
-                    break
-            else:
-                real.change_opcode(Opcodes.NOP)
-                arg_count -= 1
-
-    if arg_count == 0:
-        defined_result = False
-
-    if defined_result is not None:
-        for _, real in primitive_creation_args:
-            real.change_opcode(Opcodes.NOP)
-
-        create_primitive_arg.change_opcode(Opcodes.NOP)
-        container.replace_with_constant_value(defined_result)
-    elif arg_count == 1:
-        create_primitive_arg.change_opcode(Opcodes.NOP)
-        container.replace_call_with_arg(args[0])
-    elif arg_count != create_primitive_arg.arg:
-        create_primitive_arg.change_arg(arg_count)
-
-        container.no_special = False
-
-
-@register(sum)
-def specialize_any(container: SpecializationContainer):
-    args = container.get_arg_specifications()
-
-    if len(args) == 1:
-        if args[0].get_normalized_data_instr().opcode == Opcodes.LOAD_CONST:
-            container.replace_with_constant_value(
-                sum(args[0].get_normalized_data_instr().arg_value)
-            )
-        elif args[0].get_normalized_data_instr().opcode in (
-            Opcodes.BUILD_LIST,
-            Opcodes.BUILD_TUPLE,
-            Opcodes.BUILD_SET,
-        ):
-            count = args[0].get_normalized_data_instr().arg
-            args[0].get_normalized_data_instr().change_opcode(Opcodes.NOP)
-            container.replace_call_with_opcodes(
-                [Instruction(None, -1, Opcodes.BINARY_ADD) for _ in range(count - 1)],
-                leave_args_on_stack=True,
-            )
+import typing
+import random
+
+from bytecodemanipulation.Opcodes import Opcodes
+from bytecodemanipulation.Specialization import SpecializationContainer, register
+from bytecodemanipulation.MutableFunction import Instruction
+
+
+ASSERT_TYPE_CASTS = False
+DISCARD_ALL_ANY_WITHOUT_SIDE_EFFECT_CHECK = True
+
+
+@register(typing.cast)
+def specialize_typing_cast(container: SpecializationContainer):
+    # typing.cast(<type>, <obj>) -> <obj>
+    data_type, value = container.get_arg_specifications()
+
+    if ASSERT_TYPE_CASTS:
+        # todo: add check type
+        pass
+
+    container.replace_call_with_arg(value)
+
+
+@register(min)
+def specialize_min(container: SpecializationContainer):
+    # remove when constants are mixed with no constant all but the smallest constant
+    args = container.get_arg_specifications()
+
+    if args[0].is_self:
+        self = args.pop(0)
+    else:
+        self = None
+
+    min_const: Instruction = None
+
+    # todo: catch compare exceptions
+    for arg in args:
+        instr: Instruction = arg.get_normalized_data_instr()
+
+        if instr and instr.has_constant():
+            if min_const is None or min_const.arg_value > instr.arg_value:
+                min_const = instr
+
+    if min_const is not None:
+        # todo: for non constants, do a clever try-eval-ahead with the type if arrival
+
+        for arg in args:
+            norm_instr = arg.get_normalized_data_instr()
+            if norm_instr and norm_instr != min_const and norm_instr.has_constant():
+                arg.discard()
+
+
+@register(max)
+def specialize_min(container: SpecializationContainer):
+    # remove when constants are mixed with no constant all but the smallest constant
+    args = container.get_arg_specifications()
+
+    if args[0].is_self:
+        self = args.pop(0)
+    else:
+        self = None
+
+    min_const: Instruction = None
+
+    # todo: catch compare exceptions
+    for arg in args:
+        instr: Instruction = arg.get_normalized_data_instr()
+
+        if instr and instr.has_constant():
+            if min_const is None or min_const.arg_value < instr.arg_value:
+                min_const = instr
+
+    if min_const is not None:
+        # todo: for non constants, do a clever try-eval-ahead with the type if arrival
+
+        for arg in args:
+            norm_instr = arg.get_normalized_data_instr()
+            if norm_instr and norm_instr != min_const and norm_instr.has_constant():
+                arg.discard()
+
+
+@register(tuple)
+def create_empty_tuple(container: SpecializationContainer):
+    if len(container.get_arg_specifications()) == 0:
+        container.replace_with_constant_value(tuple())
+
+
+def _check_int(c) -> bool:
+    if isinstance(c, int):
+        return True
+    if isinstance(c, float):
+        return int(c) == c
+    return False
+
+
+@register(range)
+@register(random.randrange)
+@register(random.Random.randrange)
+def specialize_range_3rd_argument(container: SpecializationContainer):
+    args = container.get_arg_specifications()
+    sources = [arg.get_normalized_data_instr() for arg in args]
+
+    # Argument length checks and type checks
+    if len(sources) in (1, 2, 3):
+        if sources[0].opcode == Opcodes.LOAD_CONST:
+            container.replace_with_raise_exception_if(
+                not _check_int(sources[0].arg_value),
+                lambda: TypeError(
+                    f"'{type(sources[0].arg_value).__name__}' object cannot be interpreted as an integer"
+                ),
+                arg=0,
+            )
+
+        if len(sources) > 1 and sources[1].opcode == Opcodes.LOAD_CONST:
+            container.replace_with_raise_exception_if(
+                not _check_int(sources[1].arg_value),
+                lambda: TypeError(
+                    f"'{type(sources[1].arg_value).__name__}' object cannot be interpreted as an integer"
+                ),
+                arg=1,
+            )
+
+        if (
+            len(sources) == 2
+            and sources[0].opcode == sources[1].opcode == Opcodes.LOAD_CONST
+            and sources[0].arg_value > sources[1].arg_value
+        ):
+            container.replace_with_constant_value(tuple())
+
+        if len(sources) > 2 and sources[2].opcode == Opcodes.LOAD_CONST:
+            if (
+                not container.replace_with_raise_exception_if(
+                    not _check_int(sources[2].arg_value),
+                    lambda: TypeError(
+                        f"'{type(sources[2].arg_value).__name__}' object cannot be interpreted as an integer"
+                    ),
+                    arg=2,
+                )
+                and sources[2].arg_value == 0
+            ):
+                container.replace_with_raise_exception(
+                    lambda: ValueError("range() arg 3 must not be zero"),
+                    arg=2,
+                )
+
+        if (
+            len(sources) == 3
+            and sources[0].opcode
+            == sources[1].opcode
+            == sources[2].opcode
+            == Opcodes.LOAD_CONST
+            and sources[0].arg_value > sources[1].arg_value
+            and sources[2].arg_value > 0
+        ):
+            container.replace_with_constant_value(tuple())
+
+        if (
+            len(sources) == 3
+            and sources[0].opcode
+            == sources[1].opcode
+            == sources[2].opcode
+            == Opcodes.LOAD_CONST
+            and sources[0].arg_value < sources[1].arg_value
+            and sources[2].arg_value < 0
+        ):
+            container.replace_with_constant_value(tuple())
+
+    elif len(sources) == 0:
+        if container.method_call_descriptor.lookup_method_instr.arg_value == range:
+            container.replace_with_raise_exception(
+                TypeError("range expected at least 1 argument, got 0")
+            )
+        elif (
+            container.method_call_descriptor.lookup_method_instr.arg_value
+            == random.randrange
+        ):
+            container.replace_with_raise_exception(
+                TypeError(
+                    "Random.randrange() missing 1 required positional argument: 'start'"
+                )
+            )
+        elif (
+            container.method_call_descriptor.lookup_method_instr.arg_value
+            == random.Random.randrange
+        ):
+            pass
+        else:
+            raise NotImplementedError
+    else:
+        if container.method_call_descriptor.lookup_method_instr.arg_value == range:
+            container.replace_with_raise_exception(
+                TypeError(f"range expected at most 3 arguments, got {len(sources)}")
+            )
+        elif (
+            container.method_call_descriptor.lookup_method_instr.arg_value
+            == random.randrange
+        ):
+            container.replace_with_raise_exception(
+                TypeError(
+                    f"Random.randrange() takes from 2 to 4 positional arguments but {len(sources)} were given"
+                )
+            )
+        elif (
+            container.method_call_descriptor.lookup_method_instr.arg_value
+            == random.Random.randrange
+        ):
+            container.replace_with_raise_exception(
+                TypeError(
+                    f"Random.randrange() takes from 2 to 4 positional arguments but {len(sources)} were given"
+                )
+            )
+        else:
+            raise NotImplementedError
+
+    if len(args) != 3:
+        return
+
+    if (
+        args[2]
+        and sources[2].opcode == Opcodes.LOAD_CONST
+        and sources[2].arg_value == 1
+    ):
+        args[2].discard()
+
+
+@register(range)
+@register(random.randrange)
+@register(random.Random.randrange)
+def specialize_range_start_0(container: SpecializationContainer):
+    args = container.get_arg_specifications()
+
+    if len(args) != 2:
+        return
+
+    if (
+        args[0]
+        and args[0].get_normalized_data_instr().opcode == Opcodes.LOAD_CONST
+        and args[0].get_normalized_data_instr().arg_value == 0
+    ):
+        args[0].discard()
+
+
+@register(range)
+def specialize_small_range(container: SpecializationContainer):
+    args = container.get_arg_specifications()
+
+    if len(args) == 1:
+        start = 0
+        instr = args[0].get_normalized_data_instr()
+
+        if not instr or instr.opcode != Opcodes.LOAD_CONST:
+            return
+
+        end = instr.arg_value
+    elif len(args) == 2:
+        instr = args[0].get_normalized_data_instr()
+        if not instr or instr.opcode != Opcodes.LOAD_CONST:
+            return
+        start = instr.arg_value
+
+        instr = args[1].get_normalized_data_instr()
+        if not instr or instr.opcode != Opcodes.LOAD_CONST:
+            return
+        end = instr.arg_value
+    else:
+        return
+
+    if start == end:
+        container.replace_with_constant_value(tuple())
+    elif start + 1 == end:
+        container.replace_with_constant_value((start,))
+    elif start + 2 == end:
+        container.replace_with_constant_value((start, start + 1))
+
+
+@register(all)
+def specialize_all(container: SpecializationContainer):
+    args = container.get_arg_specifications()
+
+    if len(args) != 1:
+        return
+
+    create_primitive_arg = args[0].get_normalized_data_instr()
+
+    if create_primitive_arg is None:
+        return
+
+    # todo: can we specialize more?
+    if create_primitive_arg.opcode not in (
+        Opcodes.BUILD_LIST,
+        Opcodes.BUILD_TUPLE,
+        Opcodes.BUILD_SET,
+    ):
+        return
+
+    primitive_creation_args = [
+        (
+            create_primitive_arg.trace_normalized_stack_position(i),
+            next(create_primitive_arg.trace_stack_position(i)),
+        )
+        for i in range(create_primitive_arg.arg)
+    ]
+
+    defined_result = None
+    arg_count = len(primitive_creation_args)
+
+    for normal, real in primitive_creation_args:
+        if normal:
+            if normal.opcode != Opcodes.LOAD_CONST:
+                continue
+
+            if not normal.arg_value:
+                if DISCARD_ALL_ANY_WITHOUT_SIDE_EFFECT_CHECK:
+                    defined_result = False
+                    break
+            else:
+                real.change_opcode(Opcodes.NOP)
+                arg_count -= 1
+
+    if arg_count == 0:
+        defined_result = True
+
+    if defined_result is not None:
+        for _, real in primitive_creation_args:
+            real.change_opcode(Opcodes.NOP)
+
+        create_primitive_arg.change_opcode(Opcodes.NOP)
+        container.replace_with_constant_value(defined_result)
+    elif arg_count == 1:
+        create_primitive_arg.change_opcode(Opcodes.NOP)
+        container.replace_call_with_arg(args[0])
+    elif arg_count != create_primitive_arg.arg:
+        create_primitive_arg.change_arg(arg_count)
+
+        container.no_special = False
+
+
+@register(any)
+def specialize_any(container: SpecializationContainer):
+    args = container.get_arg_specifications()
+
+    if len(args) != 1:
+        return
+
+    create_primitive_arg = args[0].get_normalized_data_instr()
+
+    if create_primitive_arg is None:
+        return
+
+    # todo: can we specialize more?
+    if create_primitive_arg.opcode not in (
+        Opcodes.BUILD_LIST,
+        Opcodes.BUILD_TUPLE,
+        Opcodes.BUILD_SET,
+    ):
+        return
+
+    primitive_creation_args = [
+        (
+            create_primitive_arg.trace_normalized_stack_position(i),
+            next(create_primitive_arg.trace_stack_position(i)),
+        )
+        for i in range(create_primitive_arg.arg)
+    ]
+
+    defined_result = None
+    arg_count = len(primitive_creation_args)
+
+    for normal, real in primitive_creation_args:
+        if normal:
+            if normal.opcode != Opcodes.LOAD_CONST:
+                continue
+
+            if normal.arg_value:
+                if DISCARD_ALL_ANY_WITHOUT_SIDE_EFFECT_CHECK:
+                    defined_result = True
+                    break
+            else:
+                real.change_opcode(Opcodes.NOP)
+                arg_count -= 1
+
+    if arg_count == 0:
+        defined_result = False
+
+    if defined_result is not None:
+        for _, real in primitive_creation_args:
+            real.change_opcode(Opcodes.NOP)
+
+        create_primitive_arg.change_opcode(Opcodes.NOP)
+        container.replace_with_constant_value(defined_result)
+    elif arg_count == 1:
+        create_primitive_arg.change_opcode(Opcodes.NOP)
+        container.replace_call_with_arg(args[0])
+    elif arg_count != create_primitive_arg.arg:
+        create_primitive_arg.change_arg(arg_count)
+
+        container.no_special = False
+
+
+@register(sum)
+def specialize_any(container: SpecializationContainer):
+    args = container.get_arg_specifications()
+
+    if len(args) == 1:
+        if args[0].get_normalized_data_instr().opcode == Opcodes.LOAD_CONST:
+            container.replace_with_constant_value(
+                sum(args[0].get_normalized_data_instr().arg_value)
+            )
+        elif args[0].get_normalized_data_instr().opcode in (
+            Opcodes.BUILD_LIST,
+            Opcodes.BUILD_TUPLE,
+            Opcodes.BUILD_SET,
+        ):
+            count = args[0].get_normalized_data_instr().arg
+            args[0].get_normalized_data_instr().change_opcode(Opcodes.NOP)
+            container.replace_call_with_opcodes(
+                [Instruction(None, -1, Opcodes.BINARY_ADD) for _ in range(count - 1)],
+                leave_args_on_stack=True,
+            )
```

### Comparing `bytecodemanipulation-0.2.4/bytecodemanipulation/data_loader.py` & `bytecodemanipulation-0.2.8/bytecodemanipulation/data_loader.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,100 +1,100 @@
-import importlib
-import json
-import logging
-import os
-import sys
-from bytecodemanipulation.Opcodes import Opcodes, init_maps, OPNAME2CODE
-from bytecodemanipulation import Opcodes as OpcodesM
-from bytecodemanipulation.annotated_std import CONSTANT_BUILTINS
-
-
-local = os.path.dirname(__file__)
-
-version = f"{sys.version_info.major}_{sys.version_info.minor}"
-folder = local + "/data/v" + version
-sys.path.append(os.path.dirname(local))
-
-
-INIT_ASSEMBLY = True
-
-
-def load_opcode_data():
-    opcode_data: dict = json.load(open(folder + "/opcodes.json"))
-
-    valid_opcode_names = [
-        key
-        for key, value in Opcodes.__dict__.items()
-        if isinstance(value, int) and not key.startswith("__") and value < 256
-    ]
-
-    for key, opcode in opcode_data.items():
-        if key not in valid_opcode_names:
-            logging.warning(f"unknown opcode name encountered: {key} - Adding manually")
-
-        setattr(Opcodes, key, opcode)
-
-    for key in valid_opcode_names:
-        if key not in opcode_data:
-            setattr(Opcodes, key, -1)
-
-
-def load_instruction_spec():
-    spec_data = json.load(open(folder + "/instruction_spec.json"))
-
-    for key, opcodes in spec_data.items():
-        getattr(OpcodesM, key)[:] = map(OPNAME2CODE.__getitem__, opcodes)
-
-
-def load_builtin_spec():
-    import builtins
-    from bytecodemanipulation.annotated_std import CONSTANT_BUILTINS
-    from bytecodemanipulation.annotated_std import CONSTANT_BUILTIN_TYPES
-
-    builtin_spec = json.load(open(folder + "/builtins.json"))
-
-    CONSTANT_BUILTINS[:] = [getattr(builtins, key) for key in builtin_spec["constant"]]
-    CONSTANT_BUILTIN_TYPES[:] = [
-        getattr(builtins, key) for key in builtin_spec["const_builtin_types"]
-    ]
-
-    importlib.import_module("bytecodemanipulation.data.v" + version + ".specialize")
-
-
-def load_standard_library_annotations():
-    import importlib
-
-    std_annot = json.load(open(folder + "/standard_library.json"))
-
-    for module_name, data in std_annot.items():
-        module = importlib.import_module(module_name)
-
-        for name in data.setdefault("constant", []):
-            attr = module
-            for e in name.split("."):
-                attr = getattr(attr, e)
-
-            CONSTANT_BUILTINS.append(attr)
-
-
-ASSEMBLY_MODULE = {}
-
-
-def load_assembly_instructions():
-    if os.path.exists(folder + "/assembly_instructions.py"):
-        # exec(open(folder + "/assembly_instructions.py").read(), ASSEMBLY_MODULE)
-        ASSEMBLY_MODULE.update(
-            importlib.import_module(
-                "bytecodemanipulation.data.v" + version + ".assembly_instructions"
-            ).__dict__
-        )
-
-
-def init():
-    load_opcode_data()
-    init_maps()
-    load_instruction_spec()
-    load_builtin_spec()
-    load_standard_library_annotations()
-
-    if INIT_ASSEMBLY:
-        load_assembly_instructions()
+import importlib
+import json
+import logging
+import os
+import sys
+from bytecodemanipulation.Opcodes import Opcodes, init_maps, OPNAME2CODE
+from bytecodemanipulation import Opcodes as OpcodesM
+from bytecodemanipulation.annotated_std import CONSTANT_BUILTINS
+
+
+local = os.path.dirname(__file__)
+
+version = f"{sys.version_info.major}_{sys.version_info.minor}"
+folder = local + "/data/v" + version
+sys.path.append(os.path.dirname(local))
+
+
+INIT_ASSEMBLY = True
+
+
+def load_opcode_data():
+    opcode_data: dict = json.load(open(folder + "/opcodes.json"))
+
+    valid_opcode_names = [
+        key
+        for key, value in Opcodes.__dict__.items()
+        if isinstance(value, int) and not key.startswith("__") and value < 256
+    ]
+
+    for key, opcode in opcode_data.items():
+        if key not in valid_opcode_names:
+            logging.warning(f"unknown opcode name encountered: {key} - Adding manually")
+
+        setattr(Opcodes, key, opcode)
+
+    for key in valid_opcode_names:
+        if key not in opcode_data:
+            setattr(Opcodes, key, -1)
+
+
+def load_instruction_spec():
+    spec_data = json.load(open(folder + "/instruction_spec.json"))
+
+    for key, opcodes in spec_data.items():
+        getattr(OpcodesM, key)[:] = map(OPNAME2CODE.__getitem__, opcodes)
+
+
+def load_builtin_spec():
+    import builtins
+    from bytecodemanipulation.annotated_std import CONSTANT_BUILTINS
+    from bytecodemanipulation.annotated_std import CONSTANT_BUILTIN_TYPES
+
+    builtin_spec = json.load(open(folder + "/builtins.json"))
+
+    CONSTANT_BUILTINS[:] = [getattr(builtins, key) for key in builtin_spec["constant"]]
+    CONSTANT_BUILTIN_TYPES[:] = [
+        getattr(builtins, key) for key in builtin_spec["const_builtin_types"]
+    ]
+
+    importlib.import_module("bytecodemanipulation.data.v" + version + ".specialize")
+
+
+def load_standard_library_annotations():
+    import importlib
+
+    std_annot = json.load(open(folder + "/standard_library.json"))
+
+    for module_name, data in std_annot.items():
+        module = importlib.import_module(module_name)
+
+        for name in data.setdefault("constant", []):
+            attr = module
+            for e in name.split("."):
+                attr = getattr(attr, e)
+
+            CONSTANT_BUILTINS.append(attr)
+
+
+ASSEMBLY_MODULE = {}
+
+
+def load_assembly_instructions():
+    if os.path.exists(folder + "/assembly_instructions.py"):
+        # exec(open(folder + "/assembly_instructions.py").read(), ASSEMBLY_MODULE)
+        ASSEMBLY_MODULE.update(
+            importlib.import_module(
+                "bytecodemanipulation.data.v" + version + ".assembly_instructions"
+            ).__dict__
+        )
+
+
+def init():
+    load_opcode_data()
+    init_maps()
+    load_instruction_spec()
+    load_builtin_spec()
+    load_standard_library_annotations()
+
+    if INIT_ASSEMBLY:
+        load_assembly_instructions()
```

### Comparing `bytecodemanipulation-0.2.4/bytecodemanipulation/optimiser_util.py` & `bytecodemanipulation-0.2.8/bytecodemanipulation/optimiser_util.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,489 +1,489 @@
-import traceback
-import typing
-from bytecodemanipulation.annotated_std import CONSTANT_BUILTIN_TYPES
-from bytecodemanipulation.annotated_std import CONSTANT_BUILTINS
-
-from bytecodemanipulation.MutableFunction import Instruction
-from bytecodemanipulation.MutableFunction import MutableFunction
-from bytecodemanipulation.Opcodes import Opcodes
-from bytecodemanipulation.Opcodes import SIDE_EFFECT_FREE_LOADS
-from bytecodemanipulation.Specialization import ArgDescriptor
-from bytecodemanipulation.Specialization import MethodCallDescriptor
-from bytecodemanipulation.Specialization import SpecializationContainer
-
-OPCODE_TO_ATTR_SINGLE = {
-    Opcodes.UNARY_POSITIVE: "__pos__",
-    Opcodes.UNARY_NEGATIVE: "__neg__",
-    Opcodes.UNARY_INVERT: "__invert__",
-    Opcodes.UNARY_NOT: "__not__",
-}
-
-OPCODE_TO_ATTR_DOUBLE = {
-    Opcodes.BINARY_MATRIX_MULTIPLY: "__matmul__",
-    Opcodes.INPLACE_MATRIX_MULTIPLY: "__imatmul__",
-    Opcodes.BINARY_POWER: "__pow__",
-    Opcodes.INPLACE_POWER: "__ipow__",
-    Opcodes.BINARY_MULTIPLY: "__mul__",
-    Opcodes.INPLACE_MULTIPLY: "__imul__",
-    Opcodes.BINARY_MODULO: "__mod__",
-    Opcodes.INPLACE_MODULO: "__imod__",
-    Opcodes.BINARY_ADD: "__add__",
-    Opcodes.INPLACE_ADD: "__iadd__",
-    Opcodes.BINARY_SUBTRACT: "__sub__",
-    Opcodes.INPLACE_SUBTRACT: "__isub__",
-    Opcodes.BINARY_SUBSCR: "__getitem__",
-    Opcodes.BINARY_FLOOR_DIVIDE: "__floordiv__",
-    Opcodes.INPLACE_FLOOR_DIVIDE: "__ifloordiv__",
-    Opcodes.BINARY_TRUE_DIVIDE: "__truediv__",
-    Opcodes.INPLACE_TRUE_DIVIDE: "__itruediv__",
-    Opcodes.GET_LEN: "__len__",
-    Opcodes.BINARY_LSHIFT: "__lshift__",
-    Opcodes.INPLACE_LSHIFT: "__ilshift__",
-    Opcodes.BINARY_RSHIFT: "__rshift__",
-    Opcodes.INPLACE_RSHIFT: "__irshift__",
-    Opcodes.BINARY_AND: "__and__",
-    Opcodes.BINARY_XOR: "__xor__",
-    Opcodes.BINARY_OR: "__or__",
-    (Opcodes.IS_OP, 0): lambda a, b: a is b,
-    (Opcodes.IS_OP, 1): lambda a, b: a is not b,
-    (Opcodes.COMPARE_OP, 0): lambda a, b: a < b,
-    (Opcodes.COMPARE_OP, 1): lambda a, b: a <= b,
-    (Opcodes.COMPARE_OP, 2): lambda a, b: a == b,
-    (Opcodes.COMPARE_OP, 3): lambda a, b: a != b,
-    (Opcodes.COMPARE_OP, 4): lambda a, b: a > b,
-    (Opcodes.COMPARE_OP, 5): lambda a, b: a >= b,
-}
-
-
-def inline_const_value_pop_pairs(mutable: MutableFunction) -> bool:
-    dirty = False
-
-    for instruction in mutable.instructions:
-        if instruction.opcode == Opcodes.POP_TOP:
-            try:
-                # print("search")
-                source = next(instruction.trace_stack_position(0))
-            except StopIteration:
-                # source = next(instruction.trace_stack_position(0))
-
-                print("---")
-
-                for instr in mutable.instructions:
-                    print(instr)
-
-                print("---")
-                print(instruction)
-                print(instruction.get_priorities_previous())
-                raise
-
-            # Inline LOAD_XX - POP pairs
-            if source.opcode in SIDE_EFFECT_FREE_LOADS:
-                instruction.change_opcode(Opcodes.NOP)
-                source.change_opcode(Opcodes.NOP)
-                return True
-
-            # Inline CALL_XX (constant expr) - POP pairs
-            if source.opcode == Opcodes.CALL_FUNCTION:
-                func_resolve = next(source.trace_stack_position(source.arg))
-
-                if func_resolve.opcode == Opcodes.LOAD_CONST:
-                    function = func_resolve.arg_value
-
-                    if function in CONSTANT_BUILTINS or (
-                        hasattr(function, "_OPTIMISER_CONTAINER")
-                        and getattr(
-                            function, "_OPTIMISER_CONTAINER"
-                        ).is_side_effect_free_op
-                    ):
-                        instruction.change_opcode(Opcodes.NOP)
-
-                        if func_resolve.arg == 0:
-                            func_resolve.change_opcode(Opcodes.NOP)
-                            continue
-                        pops = func_resolve.arg
-
-                        func_resolve.change_opcode(Opcodes.POP_TOP)
-                        pops -= 1
-
-                        if not pops:
-                            continue
-
-                        for _ in range(pops):
-                            nop = Instruction.create(Opcodes.NOP)
-                            nop.next_instruction = func_resolve.next_instruction
-                            func_resolve.next_instruction = nop
-
-                        mutable.assemble_instructions_from_tree(
-                            mutable.instructions[0].optimise_tree()
-                        )
-                        return True
-
-            if source.opcode in (
-                Opcodes.BUILD_LIST,
-                Opcodes.BUILD_SET,
-                Opcodes.BUILD_MAP,
-            ):
-                count = source.arg
-
-                if source.opcode == Opcodes.BUILD_MAP:
-                    count *= 2
-
-                instruction.change_opcode(Opcodes.NOP)
-
-                if count == 0:
-                    source.change_opcode(Opcodes.NOP)
-                    dirty = True
-                    continue
-
-                source.change_opcode(Opcodes.POP_TOP)
-
-                if count == 1:
-                    dirty = True
-                    continue
-
-                count -= 1
-
-                for _ in range(count):
-                    nop = Instruction.create(Opcodes.NOP)
-                    nop.next_instruction = source.next_instruction
-                    source.next_instruction = nop
-
-                mutable.assemble_instructions_from_tree(
-                    mutable.instructions[0].optimise_tree()
-                )
-                return True
-
-    return dirty
-
-
-def remove_local_var_assign_without_use(mutable: MutableFunction) -> bool:
-    dirty = False
-
-    last_loads_of_local = [-1] * len(mutable.shared_variable_names)
-
-    for instruction in mutable.instructions:
-        if instruction.opcode == Opcodes.LOAD_FAST:
-            last_loads_of_local[instruction.arg] = instruction.offset
-
-    for instruction in mutable.instructions:
-        if (
-            instruction.opcode in (Opcodes.STORE_FAST, Opcodes.DELETE_FAST)
-            and last_loads_of_local[instruction.arg] < instruction.offset
-        ):
-            instruction.change_opcode(Opcodes.POP_TOP)
-            dirty = True
-
-    return dirty
-
-
-def inline_constant_method_invokes(mutable: MutableFunction) -> bool:
-    dirty = False
-
-    for instr in mutable.instructions:
-        if instr.opcode in (Opcodes.CALL_FUNCTION, Opcodes.CALL_METHOD):
-            target = next(instr.trace_stack_position(instr.arg))
-
-            if target.opcode == Opcodes.LOAD_CONST:
-                function: typing.Callable = target.arg_value
-
-                if function in CONSTANT_BUILTINS or (
-                    hasattr(function, "_OPTIMISER_CONTAINER")
-                    and getattr(function, "_OPTIMISER_CONTAINER").is_constant_op
-                ):
-                    args = [
-                        next(instr.trace_stack_position(i))
-                        for i in range(instr.arg - 1, -1, -1)
-                    ]
-
-                    if all(ins.opcode == Opcodes.LOAD_CONST for ins in args):
-                        result = function(*(e.arg_value for e in args))
-
-                        instr.change_opcode(Opcodes.LOAD_CONST)
-                        instr.change_arg_value(result)
-                        target.change_opcode(Opcodes.NOP)
-
-                        for arg in args:
-                            arg.change_opcode(Opcodes.NOP)
-
-                        dirty = True
-
-    return dirty
-
-
-def inline_constant_binary_ops(mutable: MutableFunction) -> bool:
-    dirty = False
-
-    for instruction in mutable.instructions:
-        if (
-            instruction.opcode in OPCODE_TO_ATTR_SINGLE
-            or (instruction.opcode, instruction.arg) in OPCODE_TO_ATTR_SINGLE
-        ):
-            method = OPCODE_TO_ATTR_SINGLE[
-                instruction.opcode
-                if instruction.opcode in OPCODE_TO_ATTR_SINGLE
-                else (instruction.opcode, instruction.arg)
-            ]
-
-            target = next(instruction.trace_stack_position(0))
-
-            if target.opcode == Opcodes.LOAD_CONST:
-                value = target.arg_value
-
-                if hasattr(value, method):
-                    method = (
-                        getattr(value, method) if isinstance(method, str) else method
-                    )
-
-                    if not callable(method) or not (
-                        type(value) in CONSTANT_BUILTIN_TYPES
-                        or (
-                            hasattr(method, "_OPTIMISER_CONTAINER")
-                            and getattr(method, "_OPTIMISER_CONTAINER").is_constant_op
-                        )
-                    ):
-                        continue
-
-                    try:
-                        value = method()
-                    except:
-                        continue
-
-                    instruction.change_opcode(Opcodes.LOAD_CONST)
-                    instruction.change_arg_value(value)
-                    target.change_opcode(Opcodes.NOP)
-                    dirty = True
-
-        elif (
-            instruction.opcode in OPCODE_TO_ATTR_DOUBLE
-            or (instruction.opcode, instruction.arg) in OPCODE_TO_ATTR_DOUBLE
-        ):
-            method = OPCODE_TO_ATTR_DOUBLE[
-                instruction.opcode
-                if instruction.opcode in OPCODE_TO_ATTR_DOUBLE
-                else (instruction.opcode, instruction.arg)
-            ]
-
-            arg = next(instruction.trace_stack_position(1))
-            target = next(instruction.trace_stack_position(0))
-
-            if arg.opcode == target.opcode == Opcodes.LOAD_CONST:
-                value = target.arg_value
-
-                if isinstance(method, str):
-                    method = getattr(value, method)
-
-                    if not callable(method) or not (
-                        type(value) in CONSTANT_BUILTIN_TYPES
-                        or (
-                            hasattr(method, "_OPTIMISER_CONTAINER")
-                            and getattr(method, "_OPTIMISER_CONTAINER").is_constant_op
-                        )
-                    ):
-                        continue
-
-                try:
-                    value = method(arg.arg_value, target.arg_value)
-                except:
-                    traceback.print_exc()
-                    continue
-
-                instruction.change_opcode(Opcodes.LOAD_CONST)
-                instruction.change_arg_value(value)
-                target.change_opcode(Opcodes.NOP)
-                arg.change_opcode(Opcodes.NOP)
-                dirty = True
-
-        elif instruction.opcode == Opcodes.BUILD_TUPLE:
-            args = [
-                next(instruction.trace_stack_position(i))
-                for i in range(instruction.arg - 1, -1, -1)
-            ]
-
-            if all(instr.opcode == Opcodes.LOAD_CONST for instr in args):
-                instruction.change_opcode(Opcodes.LOAD_CONST)
-                instruction.change_arg_value(tuple(e.arg_value for e in args))
-
-                for arg in args:
-                    arg.change_opcode(Opcodes.NOP)
-
-                dirty = True
-
-        elif instruction.opcode == Opcodes.BUILD_SLICE:
-            args = [
-                next(instruction.trace_stack_position(i))
-                for i in range(instruction.arg - 1, -1, -1)
-            ]
-
-            if all(instr.opcode == Opcodes.LOAD_CONST for instr in args):
-                instruction.change_opcode(Opcodes.LOAD_CONST)
-                instruction.change_arg_value(slice(*(e.arg_value for e in args)))
-
-                for arg in args:
-                    arg.change_opcode(Opcodes.NOP)
-
-                dirty = True
-
-        elif instruction.opcode == Opcodes.BUILD_STRING:
-            args = [
-                next(instruction.trace_stack_position(i))
-                for i in range(instruction.arg - 1, -1, -1)
-            ]
-
-            if all(instr.opcode == Opcodes.LOAD_CONST for instr in args):
-                instruction.change_opcode(Opcodes.LOAD_CONST)
-                instruction.change_arg_value("".join(e.arg_value for e in args))
-
-                for arg in args:
-                    arg.change_opcode(Opcodes.NOP)
-
-                dirty = True
-
-    return dirty
-
-
-def remove_branch_on_constant(mutable: MutableFunction) -> bool:
-    dirty = False
-
-    for instruction in mutable.instructions:
-        if (
-            instruction.has_jump()
-            and not instruction.has_unconditional_jump()
-            and instruction.opcode not in (Opcodes.SETUP_FINALLY, Opcodes.SETUP_WITH)
-        ):
-            if instruction.previous_instructions is None:
-                if (
-                    instruction.offset == 0
-                    and instruction.opcode == Opcodes.SETUP_FINALLY
-                ):
-                    continue
-
-                raise RuntimeError
-
-            source = next(instruction.trace_stack_position(0))
-
-            if source.opcode == Opcodes.LOAD_CONST:
-                flag = bool(source.arg_value)
-
-                if instruction.opcode in (
-                    Opcodes.JUMP_IF_TRUE_OR_POP,
-                    Opcodes.JUMP_IF_FALSE_OR_POP,
-                ):
-                    if instruction.opcode == Opcodes.JUMP_IF_FALSE_OR_POP:
-                        flag = not flag
-
-                    if flag:
-                        instruction.change_opcode(Opcodes.JUMP_ABSOLUTE)
-                    else:
-                        source.change_opcode(Opcodes.NOP)
-                        instruction.change_opcode(Opcodes.NOP)
-
-                    dirty = True
-
-                    continue
-
-                if instruction.opcode in (
-                    Opcodes.POP_JUMP_IF_TRUE,
-                    Opcodes.POP_JUMP_IF_FALSE,
-                ):
-                    flag = bool(source.arg_value)
-
-                    if instruction.opcode == Opcodes.POP_JUMP_IF_FALSE:
-                        flag = not flag
-
-                    source.change_opcode(Opcodes.NOP)
-
-                    if flag:
-                        instruction.change_opcode(Opcodes.JUMP_ABSOLUTE)
-                    else:
-                        instruction.change_opcode(Opcodes.NOP)
-
-                    dirty = True
-
-    return dirty
-
-
-def inline_static_attribute_access(mutable: MutableFunction) -> bool:
-    dirty = False
-
-    for instruction in mutable.instructions:
-        if instruction.opcode in (Opcodes.LOAD_ATTR, Opcodes.LOAD_METHOD):
-            source_instr = next(instruction.trace_stack_position(0))
-
-            if source_instr.opcode == Opcodes.LOAD_CONST:
-                source: typing.Any = source_instr.arg_value
-
-                if hasattr(
-                    source, "_OPTIMISER_CONTAINER"
-                ) and source._OPTIMISER_CONTAINER.is_attribute_static(
-                    instruction.arg_value
-                ):
-                    attr_name = instruction.arg_value
-                    source_instr.change_opcode(Opcodes.NOP)
-                    instruction.change_opcode(Opcodes.LOAD_CONST)
-                    instruction.change_arg_value(getattr(source, attr_name))
-
-                    # print(instruction)
-
-                    use = next(instruction.trace_stack_position_use(0))
-
-                    if use.opcode == Opcodes.CALL_METHOD:
-                        use.change_opcode(Opcodes.CALL_FUNCTION)
-
-                    dirty = True
-
-    return dirty
-
-
-def apply_specializations(mutable: MutableFunction) -> bool:
-    from bytecodemanipulation.Optimiser import _OptimisationContainer
-
-    dirty = False
-
-    for instruction in mutable.instructions:
-        if instruction.opcode in (Opcodes.CALL_FUNCTION, Opcodes.CALL_METHOD):
-            load_stack_pos = instruction.arg
-            source = instruction.trace_normalized_stack_position(load_stack_pos)
-            safe_source = next(instruction.trace_stack_position(load_stack_pos))
-
-            if source and source.opcode == Opcodes.LOAD_CONST:
-                container = _OptimisationContainer.get_for_target(source.arg_value)
-
-                if not container.specializations:
-                    continue
-
-                target_func = source.arg_value
-
-                spec = SpecializationContainer()
-                spec.target = mutable
-                spec.underlying_function = target_func
-                spec.method_call_descriptor = MethodCallDescriptor(
-                    safe_source, instruction
-                )
-                spec.set_arg_descriptors(
-                    [
-                        ArgDescriptor(
-                            next(instruction.trace_stack_position(arg_id)),
-                            instruction.trace_normalized_stack_position(arg_id),
-                            arg_id,
-                        )
-                        for arg_id in range(instruction.arg - 1, -1, -1)
-                    ]
-                )
-
-                for special in container.specializations:
-                    special(spec)
-
-                    if spec.no_special:
-                        continue
-
-                    spec.apply()
-                    dirty = True
-                    break
-
-    return dirty
-
-
-def remove_nops(mutable: MutableFunction):
-    root = mutable.instructions[0]
-    root = root.optimise_tree()
-    mutable.assemble_instructions_from_tree(root)
+import traceback
+import typing
+from bytecodemanipulation.annotated_std import CONSTANT_BUILTIN_TYPES
+from bytecodemanipulation.annotated_std import CONSTANT_BUILTINS
+
+from bytecodemanipulation.MutableFunction import Instruction
+from bytecodemanipulation.MutableFunction import MutableFunction
+from bytecodemanipulation.Opcodes import Opcodes
+from bytecodemanipulation.Opcodes import SIDE_EFFECT_FREE_LOADS
+from bytecodemanipulation.Specialization import ArgDescriptor
+from bytecodemanipulation.Specialization import MethodCallDescriptor
+from bytecodemanipulation.Specialization import SpecializationContainer
+
+OPCODE_TO_ATTR_SINGLE = {
+    Opcodes.UNARY_POSITIVE: "__pos__",
+    Opcodes.UNARY_NEGATIVE: "__neg__",
+    Opcodes.UNARY_INVERT: "__invert__",
+    Opcodes.UNARY_NOT: "__not__",
+}
+
+OPCODE_TO_ATTR_DOUBLE = {
+    Opcodes.BINARY_MATRIX_MULTIPLY: "__matmul__",
+    Opcodes.INPLACE_MATRIX_MULTIPLY: "__imatmul__",
+    Opcodes.BINARY_POWER: "__pow__",
+    Opcodes.INPLACE_POWER: "__ipow__",
+    Opcodes.BINARY_MULTIPLY: "__mul__",
+    Opcodes.INPLACE_MULTIPLY: "__imul__",
+    Opcodes.BINARY_MODULO: "__mod__",
+    Opcodes.INPLACE_MODULO: "__imod__",
+    Opcodes.BINARY_ADD: "__add__",
+    Opcodes.INPLACE_ADD: "__iadd__",
+    Opcodes.BINARY_SUBTRACT: "__sub__",
+    Opcodes.INPLACE_SUBTRACT: "__isub__",
+    Opcodes.BINARY_SUBSCR: "__getitem__",
+    Opcodes.BINARY_FLOOR_DIVIDE: "__floordiv__",
+    Opcodes.INPLACE_FLOOR_DIVIDE: "__ifloordiv__",
+    Opcodes.BINARY_TRUE_DIVIDE: "__truediv__",
+    Opcodes.INPLACE_TRUE_DIVIDE: "__itruediv__",
+    Opcodes.GET_LEN: "__len__",
+    Opcodes.BINARY_LSHIFT: "__lshift__",
+    Opcodes.INPLACE_LSHIFT: "__ilshift__",
+    Opcodes.BINARY_RSHIFT: "__rshift__",
+    Opcodes.INPLACE_RSHIFT: "__irshift__",
+    Opcodes.BINARY_AND: "__and__",
+    Opcodes.BINARY_XOR: "__xor__",
+    Opcodes.BINARY_OR: "__or__",
+    (Opcodes.IS_OP, 0): lambda a, b: a is b,
+    (Opcodes.IS_OP, 1): lambda a, b: a is not b,
+    (Opcodes.COMPARE_OP, 0): lambda a, b: a < b,
+    (Opcodes.COMPARE_OP, 1): lambda a, b: a <= b,
+    (Opcodes.COMPARE_OP, 2): lambda a, b: a == b,
+    (Opcodes.COMPARE_OP, 3): lambda a, b: a != b,
+    (Opcodes.COMPARE_OP, 4): lambda a, b: a > b,
+    (Opcodes.COMPARE_OP, 5): lambda a, b: a >= b,
+}
+
+
+def inline_const_value_pop_pairs(mutable: MutableFunction) -> bool:
+    dirty = False
+
+    for instruction in mutable.instructions:
+        if instruction.opcode == Opcodes.POP_TOP:
+            try:
+                # print("search")
+                source = next(instruction.trace_stack_position(0))
+            except StopIteration:
+                # source = next(instruction.trace_stack_position(0))
+
+                print("---")
+
+                for instr in mutable.instructions:
+                    print(instr)
+
+                print("---")
+                print(instruction)
+                print(instruction.get_priorities_previous())
+                raise
+
+            # Inline LOAD_XX - POP pairs
+            if source.opcode in SIDE_EFFECT_FREE_LOADS:
+                instruction.change_opcode(Opcodes.NOP)
+                source.change_opcode(Opcodes.NOP)
+                return True
+
+            # Inline CALL_XX (constant expr) - POP pairs
+            if source.opcode == Opcodes.CALL_FUNCTION:
+                func_resolve = next(source.trace_stack_position(source.arg))
+
+                if func_resolve.opcode == Opcodes.LOAD_CONST:
+                    function = func_resolve.arg_value
+
+                    if function in CONSTANT_BUILTINS or (
+                        hasattr(function, "_OPTIMISER_CONTAINER")
+                        and getattr(
+                            function, "_OPTIMISER_CONTAINER"
+                        ).is_side_effect_free_op
+                    ):
+                        instruction.change_opcode(Opcodes.NOP)
+
+                        if func_resolve.arg == 0:
+                            func_resolve.change_opcode(Opcodes.NOP)
+                            continue
+                        pops = func_resolve.arg
+
+                        func_resolve.change_opcode(Opcodes.POP_TOP)
+                        pops -= 1
+
+                        if not pops:
+                            continue
+
+                        for _ in range(pops):
+                            nop = Instruction.create(Opcodes.NOP)
+                            nop.next_instruction = func_resolve.next_instruction
+                            func_resolve.next_instruction = nop
+
+                        mutable.assemble_instructions_from_tree(
+                            mutable.instructions[0].optimise_tree()
+                        )
+                        return True
+
+            if source.opcode in (
+                Opcodes.BUILD_LIST,
+                Opcodes.BUILD_SET,
+                Opcodes.BUILD_MAP,
+            ):
+                count = source.arg
+
+                if source.opcode == Opcodes.BUILD_MAP:
+                    count *= 2
+
+                instruction.change_opcode(Opcodes.NOP)
+
+                if count == 0:
+                    source.change_opcode(Opcodes.NOP)
+                    dirty = True
+                    continue
+
+                source.change_opcode(Opcodes.POP_TOP)
+
+                if count == 1:
+                    dirty = True
+                    continue
+
+                count -= 1
+
+                for _ in range(count):
+                    nop = Instruction.create(Opcodes.NOP)
+                    nop.next_instruction = source.next_instruction
+                    source.next_instruction = nop
+
+                mutable.assemble_instructions_from_tree(
+                    mutable.instructions[0].optimise_tree()
+                )
+                return True
+
+    return dirty
+
+
+def remove_local_var_assign_without_use(mutable: MutableFunction) -> bool:
+    dirty = False
+
+    last_loads_of_local = [-1] * len(mutable.shared_variable_names)
+
+    for instruction in mutable.instructions:
+        if instruction.opcode == Opcodes.LOAD_FAST:
+            last_loads_of_local[instruction.arg] = instruction.offset
+
+    for instruction in mutable.instructions:
+        if (
+            instruction.opcode in (Opcodes.STORE_FAST, Opcodes.DELETE_FAST)
+            and last_loads_of_local[instruction.arg] < instruction.offset
+        ):
+            instruction.change_opcode(Opcodes.POP_TOP)
+            dirty = True
+
+    return dirty
+
+
+def inline_constant_method_invokes(mutable: MutableFunction) -> bool:
+    dirty = False
+
+    for instr in mutable.instructions:
+        if instr.opcode in (Opcodes.CALL_FUNCTION, Opcodes.CALL_METHOD):
+            target = next(instr.trace_stack_position(instr.arg))
+
+            if target.opcode == Opcodes.LOAD_CONST:
+                function: typing.Callable = target.arg_value
+
+                if function in CONSTANT_BUILTINS or (
+                    hasattr(function, "_OPTIMISER_CONTAINER")
+                    and getattr(function, "_OPTIMISER_CONTAINER").is_constant_op
+                ):
+                    args = [
+                        next(instr.trace_stack_position(i))
+                        for i in range(instr.arg - 1, -1, -1)
+                    ]
+
+                    if all(ins.opcode == Opcodes.LOAD_CONST for ins in args):
+                        result = function(*(e.arg_value for e in args))
+
+                        instr.change_opcode(Opcodes.LOAD_CONST)
+                        instr.change_arg_value(result)
+                        target.change_opcode(Opcodes.NOP)
+
+                        for arg in args:
+                            arg.change_opcode(Opcodes.NOP)
+
+                        dirty = True
+
+    return dirty
+
+
+def inline_constant_binary_ops(mutable: MutableFunction) -> bool:
+    dirty = False
+
+    for instruction in mutable.instructions:
+        if (
+            instruction.opcode in OPCODE_TO_ATTR_SINGLE
+            or (instruction.opcode, instruction.arg) in OPCODE_TO_ATTR_SINGLE
+        ):
+            method = OPCODE_TO_ATTR_SINGLE[
+                instruction.opcode
+                if instruction.opcode in OPCODE_TO_ATTR_SINGLE
+                else (instruction.opcode, instruction.arg)
+            ]
+
+            target = next(instruction.trace_stack_position(0))
+
+            if target.opcode == Opcodes.LOAD_CONST:
+                value = target.arg_value
+
+                if hasattr(value, method):
+                    method = (
+                        getattr(value, method) if isinstance(method, str) else method
+                    )
+
+                    if not callable(method) or not (
+                        type(value) in CONSTANT_BUILTIN_TYPES
+                        or (
+                            hasattr(method, "_OPTIMISER_CONTAINER")
+                            and getattr(method, "_OPTIMISER_CONTAINER").is_constant_op
+                        )
+                    ):
+                        continue
+
+                    try:
+                        value = method()
+                    except:
+                        continue
+
+                    instruction.change_opcode(Opcodes.LOAD_CONST)
+                    instruction.change_arg_value(value)
+                    target.change_opcode(Opcodes.NOP)
+                    dirty = True
+
+        elif (
+            instruction.opcode in OPCODE_TO_ATTR_DOUBLE
+            or (instruction.opcode, instruction.arg) in OPCODE_TO_ATTR_DOUBLE
+        ):
+            method = OPCODE_TO_ATTR_DOUBLE[
+                instruction.opcode
+                if instruction.opcode in OPCODE_TO_ATTR_DOUBLE
+                else (instruction.opcode, instruction.arg)
+            ]
+
+            arg = next(instruction.trace_stack_position(1))
+            target = next(instruction.trace_stack_position(0))
+
+            if arg.opcode == target.opcode == Opcodes.LOAD_CONST:
+                value = target.arg_value
+
+                if isinstance(method, str):
+                    method = getattr(value, method)
+
+                    if not callable(method) or not (
+                        type(value) in CONSTANT_BUILTIN_TYPES
+                        or (
+                            hasattr(method, "_OPTIMISER_CONTAINER")
+                            and getattr(method, "_OPTIMISER_CONTAINER").is_constant_op
+                        )
+                    ):
+                        continue
+
+                try:
+                    value = method(arg.arg_value, target.arg_value)
+                except:
+                    traceback.print_exc()
+                    continue
+
+                instruction.change_opcode(Opcodes.LOAD_CONST)
+                instruction.change_arg_value(value)
+                target.change_opcode(Opcodes.NOP)
+                arg.change_opcode(Opcodes.NOP)
+                dirty = True
+
+        elif instruction.opcode == Opcodes.BUILD_TUPLE:
+            args = [
+                next(instruction.trace_stack_position(i))
+                for i in range(instruction.arg - 1, -1, -1)
+            ]
+
+            if all(instr.opcode == Opcodes.LOAD_CONST for instr in args):
+                instruction.change_opcode(Opcodes.LOAD_CONST)
+                instruction.change_arg_value(tuple(e.arg_value for e in args))
+
+                for arg in args:
+                    arg.change_opcode(Opcodes.NOP)
+
+                dirty = True
+
+        elif instruction.opcode == Opcodes.BUILD_SLICE:
+            args = [
+                next(instruction.trace_stack_position(i))
+                for i in range(instruction.arg - 1, -1, -1)
+            ]
+
+            if all(instr.opcode == Opcodes.LOAD_CONST for instr in args):
+                instruction.change_opcode(Opcodes.LOAD_CONST)
+                instruction.change_arg_value(slice(*(e.arg_value for e in args)))
+
+                for arg in args:
+                    arg.change_opcode(Opcodes.NOP)
+
+                dirty = True
+
+        elif instruction.opcode == Opcodes.BUILD_STRING:
+            args = [
+                next(instruction.trace_stack_position(i))
+                for i in range(instruction.arg - 1, -1, -1)
+            ]
+
+            if all(instr.opcode == Opcodes.LOAD_CONST for instr in args):
+                instruction.change_opcode(Opcodes.LOAD_CONST)
+                instruction.change_arg_value("".join(e.arg_value for e in args))
+
+                for arg in args:
+                    arg.change_opcode(Opcodes.NOP)
+
+                dirty = True
+
+    return dirty
+
+
+def remove_branch_on_constant(mutable: MutableFunction) -> bool:
+    dirty = False
+
+    for instruction in mutable.instructions:
+        if (
+            instruction.has_jump()
+            and not instruction.has_unconditional_jump()
+            and instruction.opcode not in (Opcodes.SETUP_FINALLY, Opcodes.SETUP_WITH)
+        ):
+            if instruction.previous_instructions is None:
+                if (
+                    instruction.offset == 0
+                    and instruction.opcode == Opcodes.SETUP_FINALLY
+                ):
+                    continue
+
+                raise RuntimeError
+
+            source = next(instruction.trace_stack_position(0))
+
+            if source.opcode == Opcodes.LOAD_CONST:
+                flag = bool(source.arg_value)
+
+                if instruction.opcode in (
+                    Opcodes.JUMP_IF_TRUE_OR_POP,
+                    Opcodes.JUMP_IF_FALSE_OR_POP,
+                ):
+                    if instruction.opcode == Opcodes.JUMP_IF_FALSE_OR_POP:
+                        flag = not flag
+
+                    if flag:
+                        instruction.change_opcode(Opcodes.JUMP_ABSOLUTE)
+                    else:
+                        source.change_opcode(Opcodes.NOP)
+                        instruction.change_opcode(Opcodes.NOP)
+
+                    dirty = True
+
+                    continue
+
+                if instruction.opcode in (
+                    Opcodes.POP_JUMP_IF_TRUE,
+                    Opcodes.POP_JUMP_IF_FALSE,
+                ):
+                    flag = bool(source.arg_value)
+
+                    if instruction.opcode == Opcodes.POP_JUMP_IF_FALSE:
+                        flag = not flag
+
+                    source.change_opcode(Opcodes.NOP)
+
+                    if flag:
+                        instruction.change_opcode(Opcodes.JUMP_ABSOLUTE)
+                    else:
+                        instruction.change_opcode(Opcodes.NOP)
+
+                    dirty = True
+
+    return dirty
+
+
+def inline_static_attribute_access(mutable: MutableFunction) -> bool:
+    dirty = False
+
+    for instruction in mutable.instructions:
+        if instruction.opcode in (Opcodes.LOAD_ATTR, Opcodes.LOAD_METHOD):
+            source_instr = next(instruction.trace_stack_position(0))
+
+            if source_instr.opcode == Opcodes.LOAD_CONST:
+                source: typing.Any = source_instr.arg_value
+
+                if hasattr(
+                    source, "_OPTIMISER_CONTAINER"
+                ) and source._OPTIMISER_CONTAINER.is_attribute_static(
+                    instruction.arg_value
+                ):
+                    attr_name = instruction.arg_value
+                    source_instr.change_opcode(Opcodes.NOP)
+                    instruction.change_opcode(Opcodes.LOAD_CONST)
+                    instruction.change_arg_value(getattr(source, attr_name))
+
+                    # print(instruction)
+
+                    use = next(instruction.trace_stack_position_use(0))
+
+                    if use.opcode == Opcodes.CALL_METHOD:
+                        use.change_opcode(Opcodes.CALL_FUNCTION)
+
+                    dirty = True
+
+    return dirty
+
+
+def apply_specializations(mutable: MutableFunction) -> bool:
+    from bytecodemanipulation.Optimiser import _OptimisationContainer
+
+    dirty = False
+
+    for instruction in mutable.instructions:
+        if instruction.opcode in (Opcodes.CALL_FUNCTION, Opcodes.CALL_METHOD):
+            load_stack_pos = instruction.arg
+            source = instruction.trace_normalized_stack_position(load_stack_pos)
+            safe_source = next(instruction.trace_stack_position(load_stack_pos))
+
+            if source and source.opcode == Opcodes.LOAD_CONST:
+                container = _OptimisationContainer.get_for_target(source.arg_value)
+
+                if not container.specializations:
+                    continue
+
+                target_func = source.arg_value
+
+                spec = SpecializationContainer()
+                spec.target = mutable
+                spec.underlying_function = target_func
+                spec.method_call_descriptor = MethodCallDescriptor(
+                    safe_source, instruction
+                )
+                spec.set_arg_descriptors(
+                    [
+                        ArgDescriptor(
+                            next(instruction.trace_stack_position(arg_id)),
+                            instruction.trace_normalized_stack_position(arg_id),
+                            arg_id,
+                        )
+                        for arg_id in range(instruction.arg - 1, -1, -1)
+                    ]
+                )
+
+                for special in container.specializations:
+                    special(spec)
+
+                    if spec.no_special:
+                        continue
+
+                    spec.apply()
+                    dirty = True
+                    break
+
+    return dirty
+
+
+def remove_nops(mutable: MutableFunction):
+    root = mutable.instructions[0]
+    root = root.optimise_tree()
+    mutable.assemble_instructions_from_tree(root)
```

### Comparing `bytecodemanipulation-0.2.4/bytecodemanipulation/util.py` & `bytecodemanipulation-0.2.8/bytecodemanipulation/util.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-import functools
-import inspect
-import typing
-
-
-def _is_parent_of(obj, possible_parent: typing.Type) -> bool:
-    if isinstance(obj, staticmethod):
-        obj = obj.__func__
-    if inspect.getfile(obj) != inspect.getfile(possible_parent):
-        return False
-    return obj.__qualname__.startswith(possible_parent.__qualname__ + ".")
-
-
-class AbstractInstructionWalker:
-    def visit(self, instruction):
-        raise NotImplementedError
-
-
-class LambdaInstructionWalker(AbstractInstructionWalker):
-    def __init__(self, target):
-        self.target = target
-
-    def visit(self, instruction):
-        self.target(instruction)
+import functools
+import inspect
+import typing
+
+
+def _is_parent_of(obj, possible_parent: typing.Type) -> bool:
+    if isinstance(obj, staticmethod):
+        obj = obj.__func__
+    if inspect.getfile(obj) != inspect.getfile(possible_parent):
+        return False
+    return obj.__qualname__.startswith(possible_parent.__qualname__ + ".")
+
+
+class AbstractInstructionWalker:
+    def visit(self, instruction):
+        raise NotImplementedError
+
+
+class LambdaInstructionWalker(AbstractInstructionWalker):
+    def __init__(self, target):
+        self.target = target
+
+    def visit(self, instruction):
+        self.target(instruction)
```

### Comparing `bytecodemanipulation-0.2.4/bytecodemanipulation.egg-info/PKG-INFO` & `bytecodemanipulation-0.2.8/bytecodemanipulation.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,130 +1,130 @@
-Metadata-Version: 2.1
-Name: bytecodemanipulation
-Version: 0.2.4
-Summary: High level python bytecode manipulation
-Home-page: https://github.com/uuk0/PyBytecodeManipulator
-Author: uuk
-Author-email: uuk1301@gmail.com
-Project-URL: Bug Tracker, https://github.com/uuk0/PyBytecodeManipulator/issues
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# PyBytecodeManipulator
-A high level cross-version python bytecode manipulation library build ontop 
-of 'dis' and 'inspect' 
-
-Supports code inlining, branch removing and arbitrary code injection into 
-existing functions.
-
-WARNING: using bytecode manipulation on a so low level as we do can break 
-the python runtime at any point without a warning. We circumvent a lot of 
-safety checks normally done. 
-
-WARNING: We cannot make sure that everything works as it should, expect broken code 
-at runtime!
-
-
-Supported python versions:
-
-- 3.10 (main development)
-- 3.11.0[b3] (forward porting; WIP; Currently not working)
-
-Other versions will not work as a lot of config is stored in .json files per-version,
-so you may need to provide your own .json config files for the version you need.
-
-(Some versions might be plug-and-play, but most will require code changes additionally)
-
-## Why are there so many print()-s?
-
-Due to the breaking nature of anything this code touches, and the absents of any traces 
-in the function itself, we decided to add a lot of "debug" statements indicating 
-mostly the who-has-done-what-to-which-method for the runtime. 
-This makes debugging broken code easier, as it is more clear what happened to each transformed function.
-
-If you want them removed, create your own Fork of this and remove them, on your own risk.
-
-We may use in the future the logging library, so you can disable our logger instance, but we 
-are currently in an inter-stage of the code, so other stuff has priority.
-
-## Compatibility with other libraries 
-
-- Nuitka (https://github.com/Nuitka/Nuitka): Incompatible; will break as nuitka removes the \_\_code__ attribute 
-  we modify
-- Other bytecode modification / analysers: Should work as long as you as the user does NOT expose intermediate
-  results which might contain internal instructions
-
-
-## Debugging your injections 
-
-There is the possibility to "debug" functions using the execution emulator.
-It will be able to give you more information about a crash than the python core interpreter,
-but will be a lot slower than it. 
-
-It comes also with the possibility to run your bytecode in another interpreter version, so 
-you can experiment with some stuff.
-In theory, it is also possible to run in python versions not supported by the 
-bytecode manipulation system, but it is not recommended.
-
-TransformationHandler() takes as an arg debug_code and debug_further_calls
-for activating it for all accessed methods. 
-
-BytecodePatchHelper() contains a method enable_verbose_exceptions() for activating it on 
-that exact method.
-
-
-# Examples
-
-TODO
-
-
-# Applied Optimisations
-
-- Constant Expression inlining (can be declared for custom functions to be constant)
-- LOAD_GLOBAL for builtins (if enabled)
-- standard library inlining (if enabled)
-- specialization of methods based on arguments, e.g. constant arguments (when already resolved before, requires one of above options)
-- branch elimination when jumping on a constant (TODO: also if condition can be inferred ahead-of-time, see specialization)
-- local variable elimination
-
-
-# Currently Limitations
-
-- Line Numbers get mixed up, we need some way to assign meaningful line numbers
-- With python 3.11 (?), exception table exists, and this breaks our current concept of one big flow diagram,
-  as exception handling code might exist outside the default flow
-- During optimization, a lot of stuff is being recomputed each optimisation pass, we need to cache that drastically
-- Method inlining is not working properly and needs a lot more testing
-- If the exact type is known at optimisation time (e.g. object creation via class call, or type annotation), we can try to
-  inline method accesses for further optimisation
-- Python 3.12 will likely break how certain operations are stored in instructions, combing opcodes-without-args into a single
-  parent instruction, using the arg to switch between modes
-
-
-# Assembly Code
-
-- The library provides also a way to use some "python-assembly" for writing code
-- This is only python bytecode, so no fancy stuff can be done
-- See ASSEMBLY.md for more information on instructions
-- We provide an import system hook for importing .pyasm files via bytecodemanipulation.assembler.hook
-- You may use the functions from bytecodemanipulation.assembler.target for creating inline-assembly
-
-
-## Code Formatting
-
-We use the python formatting library "black" on our code
-
-# TODO's
-
-- abstract opcode affect away into a .json file describing all opcodes
-- create a json file for defining certain bytecode sequences
-- write more library-specific optimisations
-- write generating bytecode system for emulator, constructing a function pointing to the
-.json file for exception printing, and optimizing wherever possible
-
+Metadata-Version: 2.1
+Name: bytecodemanipulation
+Version: 0.2.8
+Summary: High level python bytecode manipulation
+Home-page: https://github.com/uuk0/PyBytecodeManipulator
+Author: uuk
+Author-email: uuk1301@gmail.com
+Project-URL: Bug Tracker, https://github.com/uuk0/PyBytecodeManipulator/issues
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# PyBytecodeManipulator
+A high level cross-version python bytecode manipulation library build ontop 
+of 'dis' and 'inspect' 
+
+Supports code inlining, branch removing and arbitrary code injection into 
+existing functions.
+
+WARNING: using bytecode manipulation on a so low level as we do can break 
+the python runtime at any point without a warning. We circumvent a lot of 
+safety checks normally done. 
+
+WARNING: We cannot make sure that everything works as it should, expect broken code 
+at runtime!
+
+
+Supported python versions:
+
+- 3.10 (main development)
+- 3.11.0[b3] (forward porting; WIP; Currently not working)
+
+Other versions will not work as a lot of config is stored in .json files per-version,
+so you may need to provide your own .json config files for the version you need.
+
+(Some versions might be plug-and-play, but most will require code changes additionally)
+
+## Why are there so many print()-s?
+
+Due to the breaking nature of anything this code touches, and the absents of any traces 
+in the function itself, we decided to add a lot of "debug" statements indicating 
+mostly the who-has-done-what-to-which-method for the runtime. 
+This makes debugging broken code easier, as it is more clear what happened to each transformed function.
+
+If you want them removed, create your own Fork of this and remove them, on your own risk.
+
+We may use in the future the logging library, so you can disable our logger instance, but we 
+are currently in an inter-stage of the code, so other stuff has priority.
+
+## Compatibility with other libraries 
+
+- Nuitka (https://github.com/Nuitka/Nuitka): Incompatible; will break as nuitka removes the \_\_code__ attribute 
+  we modify
+- Other bytecode modification / analysers: Should work as long as you as the user does NOT expose intermediate
+  results which might contain internal instructions
+
+
+## Debugging your injections 
+
+There is the possibility to "debug" functions using the execution emulator.
+It will be able to give you more information about a crash than the python core interpreter,
+but will be a lot slower than it. 
+
+It comes also with the possibility to run your bytecode in another interpreter version, so 
+you can experiment with some stuff.
+In theory, it is also possible to run in python versions not supported by the 
+bytecode manipulation system, but it is not recommended.
+
+TransformationHandler() takes as an arg debug_code and debug_further_calls
+for activating it for all accessed methods. 
+
+BytecodePatchHelper() contains a method enable_verbose_exceptions() for activating it on 
+that exact method.
+
+
+# Examples
+
+TODO
+
+
+# Applied Optimisations
+
+- Constant Expression inlining (can be declared for custom functions to be constant)
+- LOAD_GLOBAL for builtins (if enabled)
+- standard library inlining (if enabled)
+- specialization of methods based on arguments, e.g. constant arguments (when already resolved before, requires one of above options)
+- branch elimination when jumping on a constant (TODO: also if condition can be inferred ahead-of-time, see specialization)
+- local variable elimination
+
+
+# Currently Limitations
+
+- Line Numbers get mixed up, we need some way to assign meaningful line numbers
+- With python 3.11 (?), exception table exists, and this breaks our current concept of one big flow diagram,
+  as exception handling code might exist outside the default flow
+- During optimization, a lot of stuff is being recomputed each optimisation pass, we need to cache that drastically
+- Method inlining is not working properly and needs a lot more testing
+- If the exact type is known at optimisation time (e.g. object creation via class call, or type annotation), we can try to
+  inline method accesses for further optimisation
+- Python 3.12 will likely break how certain operations are stored in instructions, combing opcodes-without-args into a single
+  parent instruction, using the arg to switch between modes
+
+
+# Assembly Code
+
+- The library provides also a way to use some "python-assembly" for writing code
+- This is only python bytecode, so no fancy stuff can be done
+- See ASSEMBLY.md for more information on instructions
+- We provide an import system hook for importing .pyasm files via bytecodemanipulation.assembler.hook
+- You may use the functions from bytecodemanipulation.assembler.target for creating inline-assembly
+
+
+## Code Formatting
+
+We use the python formatting library "black" on our code
+
+# TODO's
+
+- abstract opcode affect away into a .json file describing all opcodes
+- create a json file for defining certain bytecode sequences
+- write more library-specific optimisations
+- write generating bytecode system for emulator, constructing a function pointing to the
+.json file for exception printing, and optimizing wherever possible
+
```

### Comparing `bytecodemanipulation-0.2.4/setup.py` & `bytecodemanipulation-0.2.8/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,41 +1,41 @@
-import setuptools
-
-with open("README.md", "r", encoding="utf-8") as fh:
-    long_description = fh.read()
-
-
-setuptools.setup(
-    name="bytecodemanipulation",
-    version="0.2.4",
-    author="uuk",
-    author_email="uuk1301@gmail.com",
-    description="High level python bytecode manipulation",
-    long_description=long_description,
-    long_description_content_type="text/markdown",
-    url="https://github.com/uuk0/PyBytecodeManipulator",
-    project_urls={
-        "Bug Tracker": "https://github.com/uuk0/PyBytecodeManipulator/issues",
-    },
-    classifiers=[
-        "Programming Language :: Python :: 3.10",
-        "Programming Language :: Python :: 3.11",
-        "License :: OSI Approved :: MIT License",
-        "Operating System :: OS Independent",
-        "Development Status :: 2 - Pre-Alpha",
-        "Programming Language :: Python :: Implementation :: CPython",
-    ],
-    packages=["bytecodemanipulation"]
-    + [
-        "bytecodemanipulation." + e
-        for e in setuptools.find_packages(where="bytecodemanipulation")
-    ],
-    package_data={
-        "bytecodemanipulation": [
-            "data/3_10/builtins.json",
-            "data/3_10/instruction_spec.json",
-            "data/3_10/opcodes.json",
-            "data/3_10/standard_library.json",
-        ]
-    },
-    python_requires=">=3.10",
-)
+import setuptools
+
+with open("README.md", "r", encoding="utf-8") as fh:
+    long_description = fh.read()
+
+
+setuptools.setup(
+    name="bytecodemanipulation",
+    version="0.2.8",
+    author="uuk",
+    author_email="uuk1301@gmail.com",
+    description="High level python bytecode manipulation",
+    long_description=long_description,
+    long_description_content_type="text/markdown",
+    url="https://github.com/uuk0/PyBytecodeManipulator",
+    project_urls={
+        "Bug Tracker": "https://github.com/uuk0/PyBytecodeManipulator/issues",
+    },
+    classifiers=[
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "License :: OSI Approved :: MIT License",
+        "Operating System :: OS Independent",
+        "Development Status :: 2 - Pre-Alpha",
+        "Programming Language :: Python :: Implementation :: CPython",
+    ],
+    packages=["bytecodemanipulation"]
+    + [
+        "bytecodemanipulation." + e
+        for e in setuptools.find_packages(where="bytecodemanipulation")
+    ],
+    package_data={
+        "bytecodemanipulation": [
+            "data/3_10/builtins.json",
+            "data/3_10/instruction_spec.json",
+            "data/3_10/opcodes.json",
+            "data/3_10/standard_library.json",
+        ]
+    },
+    python_requires=">=3.10",
+)
```

### Comparing `bytecodemanipulation-0.2.4/tests/test_MutableFunctionHelper.py` & `bytecodemanipulation-0.2.8/tests/test_MutableFunctionHelper.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-import dis
-from unittest import TestCase
-
-from bytecodemanipulation.MutableFunction import MutableFunction
-from bytecodemanipulation.MutableFunctionHelpers import *
-
-INVOKED = False
-
-
-class TestMethodInsert(TestCase):
-    def test_simple(self):
-        def main():
-            pass
-
-        def insert():
-            global INVOKED
-            INVOKED = True
-
-        global INVOKED
-        INVOKED = False
-        insert()
-        self.assertTrue(INVOKED)
-        INVOKED = False
-
-        main_mut = MutableFunction(main)
-        insert_mut = MutableFunction(insert)
-
-        insert_method_into(main_mut, main_mut.instructions[0], insert_mut)
-        main_mut.reassign_to_function()
-
-        # dis.dis(main)
-
-        main()
-        self.assertTrue(INVOKED)
+import dis
+from unittest import TestCase
+
+from bytecodemanipulation.MutableFunction import MutableFunction
+from bytecodemanipulation.MutableFunctionHelpers import *
+
+INVOKED = False
+
+
+class TestMethodInsert(TestCase):
+    def test_simple(self):
+        def main():
+            pass
+
+        def insert():
+            global INVOKED
+            INVOKED = True
+
+        global INVOKED
+        INVOKED = False
+        insert()
+        self.assertTrue(INVOKED)
+        INVOKED = False
+
+        main_mut = MutableFunction(main)
+        insert_mut = MutableFunction(insert)
+
+        insert_method_into(main_mut, main_mut.instructions[0], insert_mut)
+        main_mut.reassign_to_function()
+
+        # dis.dis(main)
+
+        main()
+        self.assertTrue(INVOKED)
```

### Comparing `bytecodemanipulation-0.2.4/tests/test_StandardLibrary.py` & `bytecodemanipulation-0.2.8/tests/test_StandardLibrary.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,178 +1,202 @@
-import os.path
-import time
-from unittest import TestCase
-import dis
-
-from bytecodemanipulation.MutableFunction import MutableFunction
-from bytecodemanipulation.assembler.target import *
-from bytecodemanipulation.assembler.Emitter import apply_inline_assemblies
-
-
-class StandardLibraryTest(TestCase):
-    def setUp(self):
-        import bytecodemanipulation.assembler.hook as hook
-
-        hook.hook()
-
-        def target():
-            assembly("""MACRO_IMPORT bytecodemanipulation.standard_library""")
-
-        mutable = MutableFunction(target)
-        apply_inline_assemblies(mutable)
-        mutable.reassign_to_function()
-
-        target()
-
-    def test_macro_import(self):
-        def target():
-            assembly(
-                """CALL MACRO std:print("Hello World"); CALL MACRO std:print("Hello World", "World Hello!"); CALL MACRO std:print("hello", "world", "test", 123)"""
-            )
-
-        mutable = MutableFunction(target)
-        apply_inline_assemblies(mutable)
-        mutable.reassign_to_function()
-        target()
-
-    def test_macro_as_assembly(self):
-        def target():
-            assembly("""std:print("Hello World")""")
-
-        mutable = MutableFunction(target)
-        apply_inline_assemblies(mutable)
-        mutable.reassign_to_function()
-
-        target()
-
-    # todo: can we test somehow the input system
-
-    def test_type_check_raise(self):
-        def target():
-            assembly("""std:check_type(@int, "test", "exception")""")
-
-        mutable = MutableFunction(target)
-        apply_inline_assemblies(mutable)
-        mutable.reassign_to_function()
-
-        self.assertRaises(ValueError, target)
-
-    def test_type_check_raise_with_default_text(self):
-        def target():
-            assembly("""std:check_type(@int, "test")""")
-
-        mutable = MutableFunction(target)
-        apply_inline_assemblies(mutable)
-        mutable.reassign_to_function()
-
-        self.assertRaises(ValueError, target)
-
-    def test_file_list(self):
-        file_name = os.path.dirname(__file__).replace("\\", "\\\\")
-        code = f'''def target():
-            assembly("""
-MACRO_IMPORT bytecodemanipulation.standard_library
-
-std:os:file_walker("{file_name}", $file, {{
-    YIELD $file
-}})
-""")
-            yield 0'''
-
-        space = globals().copy()
-        exec(code, space)
-        target = space["target"]
-
-        mutable = MutableFunction(target)
-        apply_inline_assemblies(mutable)
-        mutable.reassign_to_function()
-
-        files = list(target())[:-1]
-        self.assertEqual(
-            set(files),
-            set(
-                filter(
-                    lambda e: os.path.isfile(e), os.listdir(os.path.dirname(__file__))
-                )
-            ),
-        )
-
-    def test_stream_simple(self):
-        def target():
-            data = (0, 1, 2)
-            stream = None
-            output = None
-            assembly("""
-std:stream:initialize($stream)
-std:stream:extend($stream, $data)
-std:stream:to_list($stream, $output)
-""")
-            return output
-
-        mutable = MutableFunction(target)
-        apply_inline_assemblies(mutable)
-        mutable.reassign_to_function()
-
-        self.assertEqual(target(), [0, 1, 2])
-
-    def test_stream_simple_reduce(self):
-        def target():
-            data = (0, 1, 2)
-            stream = None
-            output = None
-            assembly("""
-std:stream:initialize($stream)
-std:stream:extend($stream, $data)
-std:stream:reduce($stream, $lhs, $rhs, {
-    OP $lhs + $rhs
-})
-STORE $output
-""")
-            return output
-
-        mutable = MutableFunction(target)
-        apply_inline_assemblies(mutable)
-        mutable.reassign_to_function()
-
-        self.assertEqual(target(), 3)
-
-    def test_stream_simple_filter(self):
-        def target():
-            data = (0, 1, 2)
-            stream = None
-            output = None
-            assembly("""
-std:stream:initialize($stream)
-std:stream:extend($stream, $data)
-std:stream:filter($stream, $var, {
-    OP $var < 2 -> %
-})
-std:stream:to_list($stream, $output)
-""")
-            return output
-
-        mutable = MutableFunction(target)
-        apply_inline_assemblies(mutable)
-        mutable.reassign_to_function()
-
-        self.assertEqual(target(), [0, 1])
-
-    def test_stream_simple_map(self):
-        def target():
-            data = (0, 1, 2)
-            stream = None
-            output = None
-            assembly("""
-std:stream:initialize($stream)
-std:stream:extend($stream, $data)
-std:stream:map($stream, $var, {
-    OP $var + 1 -> $var
-})
-std:stream:to_list($stream, $output)
-""")
-            return output
-
-        mutable = MutableFunction(target)
-        apply_inline_assemblies(mutable)
-        mutable.reassign_to_function()
-
-        self.assertEqual(target(), [1, 2, 3])
+import os.path
+import time
+from unittest import TestCase
+import dis
+
+from bytecodemanipulation.MutableFunction import MutableFunction
+from bytecodemanipulation.assembler.target import *
+from bytecodemanipulation.assembler.Emitter import apply_inline_assemblies
+
+
+class StandardLibraryTest(TestCase):
+    def setUp(self):
+        import bytecodemanipulation.assembler.hook as hook
+
+        hook.hook()
+
+        def target():
+            assembly("""MACRO_IMPORT bytecodemanipulation.standard_library""")
+
+        mutable = MutableFunction(target)
+        apply_inline_assemblies(mutable)
+        mutable.reassign_to_function()
+
+        target()
+
+    def test_macro_import(self):
+        def target():
+            assembly(
+                """CALL MACRO std:print("Hello World"); CALL MACRO std:print("Hello World", "World Hello!"); CALL MACRO std:print("hello", "world", "test", 123)"""
+            )
+
+        mutable = MutableFunction(target)
+        apply_inline_assemblies(mutable)
+        mutable.reassign_to_function()
+        target()
+
+    def test_macro_as_assembly(self):
+        def target():
+            assembly("""std:print("Hello World")""")
+
+        mutable = MutableFunction(target)
+        apply_inline_assemblies(mutable)
+        mutable.reassign_to_function()
+
+        target()
+
+    # todo: can we test somehow the input system
+
+    def test_type_check_raise(self):
+        def target():
+            assembly("""std:check_type(@int, "test", "exception")""")
+
+        mutable = MutableFunction(target)
+        apply_inline_assemblies(mutable)
+        mutable.reassign_to_function()
+
+        self.assertRaises(ValueError, target)
+
+    def test_type_check_raise_with_default_text(self):
+        def target():
+            assembly("""std:check_type(@int, "test")""")
+
+        mutable = MutableFunction(target)
+        apply_inline_assemblies(mutable)
+        mutable.reassign_to_function()
+
+        self.assertRaises(ValueError, target)
+
+    def test_file_list(self):
+        file_name = os.path.dirname(__file__).replace("\\", "\\\\")
+        code = f'''def target():
+            assembly("""
+MACRO_IMPORT bytecodemanipulation.standard_library
+
+std:os:file_walker("{file_name}", $file, {{
+    YIELD $file
+}})
+""")
+            yield 0'''
+
+        space = globals().copy()
+        exec(code, space)
+        target = space["target"]
+
+        mutable = MutableFunction(target)
+        apply_inline_assemblies(mutable)
+        mutable.reassign_to_function()
+
+        files = list(target())[:-1]
+        self.assertEqual(
+            set(files),
+            set(
+                filter(
+                    lambda e: os.path.isfile(e), os.listdir(os.path.dirname(__file__))
+                )
+            ),
+        )
+
+    def test_stream_simple(self):
+        def target():
+            data = (0, 1, 2)
+            stream = None
+            output = None
+            assembly(
+                """
+std:stream:initialize($stream)
+std:stream:extend($stream, $data)
+std:stream:to_list($stream, $output)
+"""
+            )
+            return output
+
+        mutable = MutableFunction(target)
+        apply_inline_assemblies(mutable)
+        mutable.reassign_to_function()
+
+        self.assertEqual(target(), [0, 1, 2])
+
+    def test_stream_simple_reduce(self):
+        def target():
+            data = (0, 1, 2)
+            stream = None
+            output = None
+            assembly(
+                """
+std:stream:initialize($stream)
+std:stream:extend($stream, $data)
+std:stream:reduce($stream, $lhs, $rhs, {
+    OP $lhs + $rhs
+})
+STORE $output
+"""
+            )
+            return output
+
+        mutable = MutableFunction(target)
+        apply_inline_assemblies(mutable)
+        mutable.reassign_to_function()
+
+        self.assertEqual(target(), 3)
+
+    def test_stream_simple_filter(self):
+        def target():
+            data = (0, 1, 2)
+            stream = None
+            output = None
+            assembly(
+                """
+std:stream:initialize($stream)
+std:stream:extend($stream, $data)
+std:stream:filter($stream, $var, {
+    OP $var < 2 -> %
+})
+std:stream:to_list($stream, $output)
+"""
+            )
+            return output
+
+        mutable = MutableFunction(target)
+        apply_inline_assemblies(mutable)
+        mutable.reassign_to_function()
+
+        self.assertEqual(target(), [0, 1])
+
+    def test_stream_simple_map(self):
+        def target():
+            data = (0, 1, 2)
+            stream = None
+            output = None
+            assembly(
+                """
+std:stream:initialize($stream)
+std:stream:extend($stream, $data)
+std:stream:map($stream, $var, {
+    OP $var + 1 -> $var
+})
+std:stream:to_list($stream, $output)
+"""
+            )
+            return output
+
+        mutable = MutableFunction(target)
+        apply_inline_assemblies(mutable)
+        mutable.reassign_to_function()
+
+        self.assertEqual(target(), [1, 2, 3])
+
+
+#     def test_comprehension_list(self):
+#         def target():
+#             l = [1, 2, 3, 4]
+#             assembly("""
+# std:comprehension:list($l, $value, { OP $value + 1 -> % }) -> %
+# RETURN %""")
+#
+#         mutable = MutableFunction(target)
+#         apply_inline_assemblies(mutable)
+#         mutable.reassign_to_function()
+#
+#         dis.dis(target)
+#
+#         self.assertEqual(target(), [1, 2, 3])
```

