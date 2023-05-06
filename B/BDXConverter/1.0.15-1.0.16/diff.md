# Comparing `tmp/BDXConverter-1.0.15.tar.gz` & `tmp/BDXConverter-1.0.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BDXConverter-1.0.15.tar", last modified: Fri May  5 14:08:47 2023, max compression
+gzip compressed data, was "BDXConverter-1.0.16.tar", last modified: Sat May  6 14:15:29 2023, max compression
```

## Comparing `BDXConverter-1.0.15.tar` & `BDXConverter-1.0.16.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:08:47.638987 BDXConverter-1.0.15/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:08:47.626987 BDXConverter-1.0.15/BDXConverter/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:08:47.630987 BDXConverter-1.0.15/BDXConverter/Converter/
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-05 14:08:36.000000 BDXConverter-1.0.15/BDXConverter/Converter/ConvertErrorDefine.py
--rw-r--r--   0 runner    (1001) docker     (123)     4536 2023-05-05 14:08:36.000000 BDXConverter-1.0.15/BDXConverter/Converter/Converter.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 14:08:36.000000 BDXConverter-1.0.15/BDXConverter/Converter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:08:47.630987 BDXConverter-1.0.15/BDXConverter/General/
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-05-05 14:08:36.000000 BDXConverter-1.0.15/BDXConverter/General/GeneralClass.py
--rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-05-05 14:08:36.000000 BDXConverter-1.0.15/BDXConverter/General/Operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-05-05 14:08:36.000000 BDXConverter-1.0.15/BDXConverter/General/Pool.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 14:08:36.000000 BDXConverter-1.0.15/BDXConverter/General/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:08:47.638987 BDXConverter-1.0.15/BDXConverter/Operation/
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-05 14:08:36.000000 BDXConverter-1.0.15/BDXConverter/Operation/AddInt16XValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-05 14:08:36.000000 BDXConverter-1.0.15/BDXConverter/Operation/AddInt16YValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-05 14:08:36.000000 BDXConverter-1.0.15/BDXConverter/Operation/AddInt16ZValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-05 14:08:36.000000 BDXConverter-1.0.15/BDXConverter/Operation/AddInt16ZValue0.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-05 14:08:36.000000 BDXConverter-1.0.15/BDXConverter/Operation/AddInt32XValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-05 14:08:36.000000 BDXConverter-1.0.15/BDXConverter/Operation/AddInt32YValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-05 14:08:36.000000 BDXConverter-1.0.15/BDXConverter/Operation/AddInt32ZValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-05-05 14:08:36.000000 BDXConverter-1.0.15/BDXConverter/Operation/AddInt32ZValue0.py
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-05 14:08:36.000000 BDXConverter-1.0.15/BDXConverter/Operation/AddInt8XValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-05 14:08:36.000000 BDXConverter-1.0.15/BDXConverter/Operation/AddInt8YValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-05 14:08:36.000000 BDXConverter-1.0.15/BDXConverter/Operation/AddInt8ZValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-05 14:08:36.000000 BDXConverter-1.0.15/BDXConverter/Operation/AddXValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-05 14:08:36.000000 BDXConverter-1.0.15/BDXConverter/Operation/AddYValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-05 14:08:36.000000 BDXConverter-1.0.15/BDXConverter/Operation/AddZValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-05 14:08:36.000000 BDXConverter-1.0.15/BDXConverter/Operation/AddZValue0.py
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-05-05 14:08:36.000000 BDXConverter-1.0.15/BDXConverter/Operation/AssignDebugData.py
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-05 14:08:36.000000 BDXConverter-1.0.15/BDXConverter/Operation/CreateConstantString.py
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-05 14:08:36.000000 BDXConverter-1.0.15/BDXConverter/Operation/NOP.py
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-05 14:08:36.000000 BDXConverter-1.0.15/BDXConverter/Operation/PlaceBlock.py
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-05 14:08:36.000000 BDXConverter-1.0.15/BDXConverter/Operation/PlaceBlockWithBlockStates.py
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-05-05 14:08:36.000000 BDXConverter-1.0.15/BDXConverter/Operation/PlaceBlockWithBlockStatesDeprecated.py
--rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-05-05 14:08:36.000000 BDXConverter-1.0.15/BDXConverter/Operation/PlaceBlockWithChestData.py
--rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-05-05 14:08:36.000000 BDXConverter-1.0.15/BDXConverter/Operation/PlaceBlockWithCommandBlockData.py
--rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-05-05 14:08:36.000000 BDXConverter-1.0.15/BDXConverter/Operation/PlaceBlockWithNBTData.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-05 14:08:36.000000 BDXConverter-1.0.15/BDXConverter/Operation/PlaceBlockWithRuntimeId.py
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-05-05 14:08:36.000000 BDXConverter-1.0.15/BDXConverter/Operation/PlaceCommandBlockWithCommandBlockData.py
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-05-05 14:08:36.000000 BDXConverter-1.0.15/BDXConverter/Operation/PlaceRuntimeBlock.py
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-05-05 14:08:36.000000 BDXConverter-1.0.15/BDXConverter/Operation/PlaceRuntimeBlockWithChestData.py
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-05-05 14:08:36.000000 BDXConverter-1.0.15/BDXConverter/Operation/PlaceRuntimeBlockWithChestDataAndUint32RuntimeID.py
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-05-05 14:08:36.000000 BDXConverter-1.0.15/BDXConverter/Operation/PlaceRuntimeBlockWithCommandBlockData.py
--rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-05-05 14:08:36.000000 BDXConverter-1.0.15/BDXConverter/Operation/PlaceRuntimeBlockWithCommandBlockDataAndUint32RuntimeID.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-05 14:08:36.000000 BDXConverter-1.0.15/BDXConverter/Operation/SetCommandBlockData.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-05 14:08:36.000000 BDXConverter-1.0.15/BDXConverter/Operation/SubtractXValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-05 14:08:36.000000 BDXConverter-1.0.15/BDXConverter/Operation/SubtractYValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-05 14:08:36.000000 BDXConverter-1.0.15/BDXConverter/Operation/SubtractZValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-05 14:08:36.000000 BDXConverter-1.0.15/BDXConverter/Operation/Terminate.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-05-05 14:08:36.000000 BDXConverter-1.0.15/BDXConverter/Operation/UseRuntimeIDPool.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 14:08:36.000000 BDXConverter-1.0.15/BDXConverter/Operation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-05-05 14:08:36.000000 BDXConverter-1.0.15/BDXConverter/Operation/structOfChest.py
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-05 14:08:36.000000 BDXConverter-1.0.15/BDXConverter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:08:47.638987 BDXConverter-1.0.15/BDXConverter/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 14:08:36.000000 BDXConverter-1.0.15/BDXConverter/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-05 14:08:36.000000 BDXConverter-1.0.15/BDXConverter/utils/getByte.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-05 14:08:36.000000 BDXConverter-1.0.15/BDXConverter/utils/getString.py
--rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-05-05 14:08:36.000000 BDXConverter-1.0.15/BDXConverter/utils/marshalNBT.py
--rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-05-05 14:08:36.000000 BDXConverter-1.0.15/BDXConverter/utils/marshalNBT_OldVersion.py
--rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-05-05 14:08:36.000000 BDXConverter-1.0.15/BDXConverter/utils/unmarshalNBT.py
--rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-05-05 14:08:36.000000 BDXConverter-1.0.15/BDXConverter/utils/unmarshalNBT_OldVersion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:08:47.630987 BDXConverter-1.0.15/BDXConverter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5874 2023-05-05 14:08:47.000000 BDXConverter-1.0.15/BDXConverter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-05-05 14:08:47.000000 BDXConverter-1.0.15/BDXConverter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 14:08:47.000000 BDXConverter-1.0.15/BDXConverter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-05 14:08:47.000000 BDXConverter-1.0.15/BDXConverter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-05 14:08:47.000000 BDXConverter-1.0.15/BDXConverter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-05 14:08:36.000000 BDXConverter-1.0.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5874 2023-05-05 14:08:47.638987 BDXConverter-1.0.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5345 2023-05-05 14:08:36.000000 BDXConverter-1.0.15/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 14:08:47.638987 BDXConverter-1.0.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-05-05 14:08:36.000000 BDXConverter-1.0.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 14:15:29.594804 BDXConverter-1.0.16/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 14:15:29.578803 BDXConverter-1.0.16/BDXConverter/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 14:15:29.578803 BDXConverter-1.0.16/BDXConverter/Converter/
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-06 14:15:18.000000 BDXConverter-1.0.16/BDXConverter/Converter/ConvertErrorDefine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4536 2023-05-06 14:15:18.000000 BDXConverter-1.0.16/BDXConverter/Converter/Converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 14:15:18.000000 BDXConverter-1.0.16/BDXConverter/Converter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 14:15:29.582803 BDXConverter-1.0.16/BDXConverter/General/
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-05-06 14:15:18.000000 BDXConverter-1.0.16/BDXConverter/General/GeneralClass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-05-06 14:15:18.000000 BDXConverter-1.0.16/BDXConverter/General/Operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-05-06 14:15:18.000000 BDXConverter-1.0.16/BDXConverter/General/Pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 14:15:18.000000 BDXConverter-1.0.16/BDXConverter/General/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 14:15:29.590803 BDXConverter-1.0.16/BDXConverter/Operation/
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-06 14:15:18.000000 BDXConverter-1.0.16/BDXConverter/Operation/AddInt16XValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-06 14:15:18.000000 BDXConverter-1.0.16/BDXConverter/Operation/AddInt16YValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-06 14:15:18.000000 BDXConverter-1.0.16/BDXConverter/Operation/AddInt16ZValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-06 14:15:18.000000 BDXConverter-1.0.16/BDXConverter/Operation/AddInt16ZValue0.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-06 14:15:18.000000 BDXConverter-1.0.16/BDXConverter/Operation/AddInt32XValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-06 14:15:18.000000 BDXConverter-1.0.16/BDXConverter/Operation/AddInt32YValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-06 14:15:18.000000 BDXConverter-1.0.16/BDXConverter/Operation/AddInt32ZValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-05-06 14:15:18.000000 BDXConverter-1.0.16/BDXConverter/Operation/AddInt32ZValue0.py
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-06 14:15:18.000000 BDXConverter-1.0.16/BDXConverter/Operation/AddInt8XValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-06 14:15:18.000000 BDXConverter-1.0.16/BDXConverter/Operation/AddInt8YValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-06 14:15:18.000000 BDXConverter-1.0.16/BDXConverter/Operation/AddInt8ZValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-06 14:15:18.000000 BDXConverter-1.0.16/BDXConverter/Operation/AddXValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-06 14:15:18.000000 BDXConverter-1.0.16/BDXConverter/Operation/AddYValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-06 14:15:18.000000 BDXConverter-1.0.16/BDXConverter/Operation/AddZValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-06 14:15:18.000000 BDXConverter-1.0.16/BDXConverter/Operation/AddZValue0.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-05-06 14:15:18.000000 BDXConverter-1.0.16/BDXConverter/Operation/AssignDebugData.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-06 14:15:18.000000 BDXConverter-1.0.16/BDXConverter/Operation/CreateConstantString.py
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-06 14:15:18.000000 BDXConverter-1.0.16/BDXConverter/Operation/NOP.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-06 14:15:18.000000 BDXConverter-1.0.16/BDXConverter/Operation/PlaceBlock.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-06 14:15:18.000000 BDXConverter-1.0.16/BDXConverter/Operation/PlaceBlockWithBlockStates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-05-06 14:15:18.000000 BDXConverter-1.0.16/BDXConverter/Operation/PlaceBlockWithBlockStatesDeprecated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-05-06 14:15:18.000000 BDXConverter-1.0.16/BDXConverter/Operation/PlaceBlockWithChestData.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-05-06 14:15:18.000000 BDXConverter-1.0.16/BDXConverter/Operation/PlaceBlockWithCommandBlockData.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-05-06 14:15:18.000000 BDXConverter-1.0.16/BDXConverter/Operation/PlaceBlockWithNBTData.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-06 14:15:18.000000 BDXConverter-1.0.16/BDXConverter/Operation/PlaceBlockWithRuntimeId.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-05-06 14:15:18.000000 BDXConverter-1.0.16/BDXConverter/Operation/PlaceCommandBlockWithCommandBlockData.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-05-06 14:15:18.000000 BDXConverter-1.0.16/BDXConverter/Operation/PlaceRuntimeBlock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-05-06 14:15:18.000000 BDXConverter-1.0.16/BDXConverter/Operation/PlaceRuntimeBlockWithChestData.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-05-06 14:15:18.000000 BDXConverter-1.0.16/BDXConverter/Operation/PlaceRuntimeBlockWithChestDataAndUint32RuntimeID.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-05-06 14:15:18.000000 BDXConverter-1.0.16/BDXConverter/Operation/PlaceRuntimeBlockWithCommandBlockData.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-05-06 14:15:18.000000 BDXConverter-1.0.16/BDXConverter/Operation/PlaceRuntimeBlockWithCommandBlockDataAndUint32RuntimeID.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-06 14:15:18.000000 BDXConverter-1.0.16/BDXConverter/Operation/SetCommandBlockData.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-06 14:15:18.000000 BDXConverter-1.0.16/BDXConverter/Operation/SubtractXValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-06 14:15:18.000000 BDXConverter-1.0.16/BDXConverter/Operation/SubtractYValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-06 14:15:18.000000 BDXConverter-1.0.16/BDXConverter/Operation/SubtractZValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-06 14:15:18.000000 BDXConverter-1.0.16/BDXConverter/Operation/Terminate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-05-06 14:15:18.000000 BDXConverter-1.0.16/BDXConverter/Operation/UseRuntimeIDPool.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 14:15:18.000000 BDXConverter-1.0.16/BDXConverter/Operation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-05-06 14:15:18.000000 BDXConverter-1.0.16/BDXConverter/Operation/structOfChest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-06 14:15:18.000000 BDXConverter-1.0.16/BDXConverter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 14:15:29.594804 BDXConverter-1.0.16/BDXConverter/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 14:15:18.000000 BDXConverter-1.0.16/BDXConverter/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-06 14:15:18.000000 BDXConverter-1.0.16/BDXConverter/utils/getByte.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-06 14:15:18.000000 BDXConverter-1.0.16/BDXConverter/utils/getString.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-05-06 14:15:18.000000 BDXConverter-1.0.16/BDXConverter/utils/marshalNBT.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-05-06 14:15:18.000000 BDXConverter-1.0.16/BDXConverter/utils/marshalNBT_OldVersion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-05-06 14:15:18.000000 BDXConverter-1.0.16/BDXConverter/utils/unmarshalNBT.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-05-06 14:15:18.000000 BDXConverter-1.0.16/BDXConverter/utils/unmarshalNBT_OldVersion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 14:15:29.578803 BDXConverter-1.0.16/BDXConverter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5725 2023-05-06 14:15:29.000000 BDXConverter-1.0.16/BDXConverter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-05-06 14:15:29.000000 BDXConverter-1.0.16/BDXConverter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 14:15:29.000000 BDXConverter-1.0.16/BDXConverter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-06 14:15:29.000000 BDXConverter-1.0.16/BDXConverter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-06 14:15:29.000000 BDXConverter-1.0.16/BDXConverter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-06 14:15:18.000000 BDXConverter-1.0.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5725 2023-05-06 14:15:29.594804 BDXConverter-1.0.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5196 2023-05-06 14:15:18.000000 BDXConverter-1.0.16/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 14:15:29.594804 BDXConverter-1.0.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-05-06 14:15:18.000000 BDXConverter-1.0.16/setup.py
```

### Comparing `BDXConverter-1.0.15/BDXConverter/Converter/ConvertErrorDefine.py` & `BDXConverter-1.0.16/BDXConverter/Converter/ConvertErrorDefine.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.15/BDXConverter/Converter/Converter.py` & `BDXConverter-1.0.16/BDXConverter/Converter/Converter.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.15/BDXConverter/General/GeneralClass.py` & `BDXConverter-1.0.16/BDXConverter/General/GeneralClass.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from io import BytesIO
+from copy import deepcopy
 
 
 class GeneralClass:
     """
     Any operation of the BDX file will inherit this class
     """
 
@@ -25,16 +26,31 @@
     def Loads(self, jsonDict: dict) -> None:
         """
         Load datas from jsonDict:dict
         """
         if 'operationNumber' in self.__dict__:
             jsonDict['operationNumber'] = self.operationNumber
             jsonDict['operationName'] = self.operationName
-        for i in self.__dict__:
-            if i in jsonDict:
-                self.__dict__[i] = jsonDict[i]
+        if 'operationDatas' in self.__dict__:
+            for i in self.__dict__['operationDatas']:
+                if i in jsonDict:
+                    self.__dict__['operationDatas'][i] = jsonDict[i]
+        else:
+            for i in self.__dict__:
+                if i in jsonDict:
+                    self.__dict__[i] = jsonDict[i]
 
     def Dumps(self) -> dict:
         """
         Convert Self@GeneralClass into the basic dictionary
         """
-        return self.__dict__
+        if 'operationNumber' in self.__dict__:
+            copyDict = deepcopy(self.__dict__)
+            del copyDict['operationNumber']
+            del copyDict['operationName']
+            return {
+                'operationNumber': self.operationNumber,
+                'operationName': self.operationName,
+                'operationDatas': copyDict
+            }
+        else:
+            return self.__dict__
```

### Comparing `BDXConverter-1.0.15/BDXConverter/General/Operation.py` & `BDXConverter-1.0.16/BDXConverter/General/Operation.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.15/BDXConverter/General/Pool.py` & `BDXConverter-1.0.16/BDXConverter/General/Pool.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.15/BDXConverter/Operation/AddInt16XValue.py` & `BDXConverter-1.0.16/BDXConverter/Operation/AddInt16XValue.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.15/BDXConverter/Operation/AddInt16YValue.py` & `BDXConverter-1.0.16/BDXConverter/Operation/AddInt16YValue.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.15/BDXConverter/Operation/AddInt16ZValue.py` & `BDXConverter-1.0.16/BDXConverter/Operation/AddInt16ZValue.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.15/BDXConverter/Operation/AddInt16ZValue0.py` & `BDXConverter-1.0.16/BDXConverter/Operation/AddInt16ZValue0.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.15/BDXConverter/Operation/AddInt32XValue.py` & `BDXConverter-1.0.16/BDXConverter/Operation/AddInt32XValue.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.15/BDXConverter/Operation/AddInt32YValue.py` & `BDXConverter-1.0.16/BDXConverter/Operation/AddInt32YValue.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.15/BDXConverter/Operation/AddInt32ZValue.py` & `BDXConverter-1.0.16/BDXConverter/Operation/AddInt32ZValue.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.15/BDXConverter/Operation/AddInt32ZValue0.py` & `BDXConverter-1.0.16/BDXConverter/Operation/AddInt32ZValue0.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.15/BDXConverter/Operation/AddInt8XValue.py` & `BDXConverter-1.0.16/BDXConverter/Operation/AddInt8XValue.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.15/BDXConverter/Operation/AddInt8YValue.py` & `BDXConverter-1.0.16/BDXConverter/Operation/AddInt8YValue.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.15/BDXConverter/Operation/AddInt8ZValue.py` & `BDXConverter-1.0.16/BDXConverter/Operation/AddInt8ZValue.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.15/BDXConverter/Operation/AssignDebugData.py` & `BDXConverter-1.0.16/BDXConverter/Operation/AssignDebugData.py`

 * *Files 25% similar despite different names*

```diff
@@ -15,23 +15,26 @@
         writer.write(pack('>I', self.length) + self.buffer)
 
     def UnMarshal(self, buffer: BytesIO) -> None:
         self.length = unpack('>I', getByte(buffer, 4))[0]
         self.buffer = getByte(buffer, self.length)
 
     def Loads(self, jsonDict: dict) -> None:
-        self.length = jsonDict['length'] if 'length' in jsonDict else 0
-        self.buffer = b''.join(
-            [
-                i.to_bytes(length=1, byteorder='big', signed=False)
-                for i in jsonDict['buffer']
-            ]
-        ) if 'buffer' in jsonDict else b''
+        if 'operationDatas' in jsonDict:
+            jsonDict = jsonDict['operationDatas']
+            self.length = jsonDict['length'] if 'length' in jsonDict else 0
+            self.buffer = b''.join(
+                [
+                    i.to_bytes(length=1, byteorder='big', signed=False)
+                    for i in jsonDict['buffer']
+                ]
+            ) if 'buffer' in jsonDict else b''
 
     def Dumps(self) -> dict:
-        result: dict = {
+        return {
             'operationName': self.operationName,
             'operationNumber': self.operationNumber,
-            'length': self.length,
-            'buffer': [i for i in self.buffer]
+            'operationDatas': {
+                'length': self.length,
+                'buffer': [i for i in self.buffer]
+            }
         }
-        return result
```

### Comparing `BDXConverter-1.0.15/BDXConverter/Operation/CreateConstantString.py` & `BDXConverter-1.0.16/BDXConverter/Operation/CreateConstantString.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.15/BDXConverter/Operation/PlaceBlock.py` & `BDXConverter-1.0.16/BDXConverter/Operation/PlaceBlock.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.15/BDXConverter/Operation/PlaceBlockWithBlockStates.py` & `BDXConverter-1.0.16/BDXConverter/Operation/PlaceBlockWithBlockStates.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.15/BDXConverter/Operation/PlaceBlockWithBlockStatesDeprecated.py` & `BDXConverter-1.0.16/BDXConverter/Operation/PlaceBlockWithBlockStatesDeprecated.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.15/BDXConverter/Operation/PlaceBlockWithChestData.py` & `BDXConverter-1.0.16/BDXConverter/Operation/PlaceBlockWithChestData.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,25 +24,28 @@
         self.blockConstantStringID = unpack('>H', getByte(buffer, 2))[0]
         self.blockData = unpack('>H', getByte(buffer, 2))[0]
         self.slotCount = getByte(buffer, 1)[0]
         self.data.slotCount = self.slotCount
         self.data.UnMarshal(buffer)
 
     def Loads(self, jsonDict: dict) -> None:
-        self.blockConstantStringID = jsonDict['blockConstantStringID'] if 'blockConstantStringID' in jsonDict else 0
-        self.blockData = jsonDict['blockData'] if 'blockData' in jsonDict else 0
-        newChestData = ChestData()
-        if 'data' in jsonDict:
-            newChestData.Loads(jsonDict['data'])
-        self.slotCount = self.data.slotCount
-        self.data = newChestData
+        if 'operationDatas' in jsonDict:
+            jsonDict = jsonDict['operationDatas']
+            self.blockConstantStringID = jsonDict['blockConstantStringID'] if 'blockConstantStringID' in jsonDict else 0
+            self.blockData = jsonDict['blockData'] if 'blockData' in jsonDict else 0
+            newChestData = ChestData()
+            if 'data' in jsonDict:
+                newChestData.Loads(jsonDict['data'])
+            self.slotCount = self.data.slotCount
+            self.data = newChestData
 
     def Dumps(self) -> dict:
-        result: dict = {
+        return {
             'operationName': self.operationName,
             'operationNumber': self.operationNumber,
-            'blockConstantStringID': self.blockConstantStringID,
-            'blockData': self.blockData,
-            'slotCount': len(self.data.chestData),
-            'data': self.data.Dumps()
+            'operationDatas': {
+                'blockConstantStringID': self.blockConstantStringID,
+                'blockData': self.blockData,
+                'slotCount': len(self.data.chestData),
+                'data': self.data.Dumps()
+            }
         }
-        return result
```

### Comparing `BDXConverter-1.0.15/BDXConverter/Operation/PlaceBlockWithCommandBlockData.py` & `BDXConverter-1.0.16/BDXConverter/Operation/PlaceBlockWithCommandBlockData.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.15/BDXConverter/Operation/PlaceBlockWithNBTData.py` & `BDXConverter-1.0.16/BDXConverter/Operation/PlaceBlockWithNBTData.py`

 * *Files 10% similar despite different names*

```diff
@@ -32,22 +32,25 @@
         self.blockConstantStringID = unpack('>H', getByte(buffer, 2))[0]
         self.blockStatesConstantStringID = unpack('>H', getByte(buffer, 2))[0]
         getByte(buffer, 2)  # do not delete this line because it is correct
         self.blockNBT, _ = UnMarshalBufferToPythonNBTObject(  # type: ignore
             buffer)
 
     def Loads(self, jsonDict: dict) -> None:
-        self.blockConstantStringID = jsonDict['blockConstantStringID'] if 'blockConstantStringID' in jsonDict else 0
-        self.blockStatesConstantStringID = jsonDict[
-            'blockStatesConstantStringID'] if 'blockStatesConstantStringID' in jsonDict else 0
-        self.blockNBT = nbtlib.parse_nbt(
-            jsonDict['blockNBT']) if 'blockNBT' in jsonDict else nbtlib.tag.Compound({})
+        if 'operationDatas' in jsonDict:
+            jsonDict = jsonDict['operationDatas']
+            self.blockConstantStringID = jsonDict['blockConstantStringID'] if 'blockConstantStringID' in jsonDict else 0
+            self.blockStatesConstantStringID = jsonDict[
+                'blockStatesConstantStringID'] if 'blockStatesConstantStringID' in jsonDict else 0
+            self.blockNBT = nbtlib.parse_nbt(
+                jsonDict['blockNBT']) if 'blockNBT' in jsonDict else nbtlib.tag.Compound({})
 
     def Dumps(self) -> dict:
-        result: dict = {
+        return {
             'operationName': self.operationName,
             'operationNumber': self.operationNumber,
-            'blockConstantStringID': self.blockConstantStringID,
-            'blockStatesConstantStringID': self.blockStatesConstantStringID,
-            'blockNBT': nbtlib.serialize_tag(self.blockNBT)
+            'operationDatas': {
+                'blockConstantStringID': self.blockConstantStringID,
+                'blockStatesConstantStringID': self.blockStatesConstantStringID,
+                'blockNBT': nbtlib.serialize_tag(self.blockNBT)
+            }
         }
-        return result
```

### Comparing `BDXConverter-1.0.15/BDXConverter/Operation/PlaceBlockWithRuntimeId.py` & `BDXConverter-1.0.16/BDXConverter/Operation/PlaceBlockWithRuntimeId.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.15/BDXConverter/Operation/PlaceCommandBlockWithCommandBlockData.py` & `BDXConverter-1.0.16/BDXConverter/Operation/PlaceCommandBlockWithCommandBlockData.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.15/BDXConverter/Operation/PlaceRuntimeBlock.py` & `BDXConverter-1.0.16/BDXConverter/Operation/PlaceRuntimeBlock.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.15/BDXConverter/Operation/PlaceRuntimeBlockWithChestData.py` & `BDXConverter-1.0.16/BDXConverter/Operation/PlaceRuntimeBlockWithChestData.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,23 +22,26 @@
     def UnMarshal(self, buffer: BytesIO) -> None:
         self.runtimeId = unpack('>H', getByte(buffer, 2))[0]
         self.slotCount = getByte(buffer, 1)[0]
         self.data.slotCount = self.slotCount
         self.data.UnMarshal(buffer)
 
     def Loads(self, jsonDict: dict) -> None:
-        self.runtimeId = jsonDict['runtimeId'] if 'runtimeId' in jsonDict else 0
-        newChestData = ChestData()
-        if 'data' in jsonDict:
-            newChestData.Loads(jsonDict['data'])
-        self.slotCount = self.data.slotCount
-        self.data = newChestData
+        if 'operationDatas' in jsonDict:
+            jsonDict = jsonDict['operationDatas']
+            self.runtimeId = jsonDict['runtimeId'] if 'runtimeId' in jsonDict else 0
+            newChestData = ChestData()
+            if 'data' in jsonDict:
+                newChestData.Loads(jsonDict['data'])
+            self.slotCount = self.data.slotCount
+            self.data = newChestData
 
     def Dumps(self) -> dict:
-        result: dict = {
+        return {
             'operationName': self.operationName,
             'operationNumber': self.operationNumber,
-            'runtimeId': self.runtimeId,
-            'slotCount': len(self.data.chestData),
-            'data': self.data.Dumps()
+            'operationDatas': {
+                'runtimeId': self.runtimeId,
+                'slotCount': len(self.data.chestData),
+                'data': self.data.Dumps()
+            }
         }
-        return result
```

### Comparing `BDXConverter-1.0.15/BDXConverter/Operation/PlaceRuntimeBlockWithChestDataAndUint32RuntimeID.py` & `BDXConverter-1.0.16/BDXConverter/Operation/PlaceRuntimeBlockWithChestDataAndUint32RuntimeID.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,23 +22,26 @@
     def UnMarshal(self, buffer: BytesIO) -> None:
         self.runtimeId = unpack('>I', getByte(buffer, 4))[0]
         self.slotCount = getByte(buffer, 1)[0]
         self.data.slotCount = self.slotCount
         self.data.UnMarshal(buffer)
 
     def Loads(self, jsonDict: dict) -> None:
-        self.runtimeId = jsonDict['runtimeId'] if 'runtimeId' in jsonDict else 0
-        newChestData = ChestData()
-        if 'data' in jsonDict:
-            newChestData.Loads(jsonDict['data'])
-        self.slotCount = self.data.slotCount
-        self.data = newChestData
+        if 'operationDatas' in jsonDict:
+            jsonDict = jsonDict['operationDatas']
+            self.runtimeId = jsonDict['runtimeId'] if 'runtimeId' in jsonDict else 0
+            newChestData = ChestData()
+            if 'data' in jsonDict:
+                newChestData.Loads(jsonDict['data'])
+            self.slotCount = self.data.slotCount
+            self.data = newChestData
 
     def Dumps(self) -> dict:
-        result: dict = {
+        return {
             'operationName': self.operationName,
             'operationNumber': self.operationNumber,
-            'runtimeId': self.runtimeId,
-            'slotCount': len(self.data.chestData),
-            'data': self.data.Dumps()
+            'operationDatas': {
+                'runtimeId': self.runtimeId,
+                'slotCount': len(self.data.chestData),
+                'data': self.data.Dumps()
+            }
         }
-        return result
```

### Comparing `BDXConverter-1.0.15/BDXConverter/Operation/PlaceRuntimeBlockWithCommandBlockData.py` & `BDXConverter-1.0.16/BDXConverter/Operation/PlaceRuntimeBlockWithCommandBlockData.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.15/BDXConverter/Operation/PlaceRuntimeBlockWithCommandBlockDataAndUint32RuntimeID.py` & `BDXConverter-1.0.16/BDXConverter/Operation/PlaceRuntimeBlockWithCommandBlockDataAndUint32RuntimeID.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.15/BDXConverter/Operation/SetCommandBlockData.py` & `BDXConverter-1.0.16/BDXConverter/Operation/SetCommandBlockData.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.15/BDXConverter/Operation/UseRuntimeIDPool.py` & `BDXConverter-1.0.16/BDXConverter/Operation/UseRuntimeIDPool.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.15/BDXConverter/Operation/structOfChest.py` & `BDXConverter-1.0.16/BDXConverter/Operation/structOfChest.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.15/BDXConverter/utils/marshalNBT.py` & `BDXConverter-1.0.16/BDXConverter/utils/marshalNBT.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.15/BDXConverter/utils/marshalNBT_OldVersion.py` & `BDXConverter-1.0.16/BDXConverter/utils/marshalNBT_OldVersion.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.15/BDXConverter/utils/unmarshalNBT.py` & `BDXConverter-1.0.16/BDXConverter/utils/unmarshalNBT.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.15/BDXConverter/utils/unmarshalNBT_OldVersion.py` & `BDXConverter-1.0.16/BDXConverter/utils/unmarshalNBT_OldVersion.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.15/BDXConverter.egg-info/PKG-INFO` & `BDXConverter-1.0.16/BDXConverter.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BDXConverter
-Version: 1.0.15
+Version: 1.0.16
 Summary: A code library to marshal, unmarshal, visual and reverse visualization of BDX files
 Home-page: https://github.com/TriM-Organization/BDXConverter
 Author: Minecraft Muti-Media Organization
 Author-email: TriM-Organization@hotmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -35,14 +35,15 @@
 
 
 
 
 # 目录
 - [目录](#目录)
 - [`BDX Converter`](#bdx-converter)
+- [注意事项](#注意事项)
 - [快速上手](#快速上手)
 - [🐍 Pypi Packages](#-pypi-packages)
 - [第三方依赖](#第三方依赖)
 - [特性](#特性)
 - [什么是 `BDX` 文件](#什么是-bdx-文件)
 - [关于 `PhoenixBuilder`](#关于-phoenixbuilder)
 - [待办列表](#待办列表)
@@ -55,14 +56,21 @@
 # `BDX Converter`
 `BDX Converter` 是一个轻量化的纯 `Python` 实现，它提供了基本的 `BDX` 解析、反解析、`JSON` 可视化和反可视化功能。 
 
 
 
 
 
+# 注意事项
+- 版本 `1.0.16` 在可视化和反可视化字典方面不兼容之前的版本
+
+
+
+
+
 # 快速上手
 您可以利用 [`BDXConverter/Converter/Converter.py`](https://github.com/TriM-Organization/BDXConverter/blob/main/BDXConverter/Converter/Converter.py) 中已提供的 `4` 个函数来完成 `BDX` 文件和 `JSON` 文件的相关操作。 
 
 
 
 
 
@@ -116,26 +124,21 @@
         """
         ...
 
     def Loads(self, jsonDict: dict) -> None:
         """
         Load datas from jsonDict:dict
         """
-        if 'operationNumber' in self.__dict__:
-            jsonDict['operationNumber'] = self.operationNumber
-            jsonDict['operationName'] = self.operationName
-        for i in self.__dict__:
-            if i in jsonDict:
-                self.__dict__[i] = jsonDict[i]
+        ...
 
     def Dumps(self) -> dict:
         """
         Convert Self@GeneralClass into the basic dictionary
         """
-        return self.__dict__
+        ...
 ```
 
 因此，通过 `Marshal` 和 `UnMarshal` 函数，`BDX Converter` 可以自由的将 `二进制数据` 转换为 `Python Class` ，亦或转换回去。 <br/>
 而 `Loads` 和 `Dumps` 分别支持了把只带有基本数据类型的字典转换为 `Python Class` 亦或转换回去的功能。 
 
 目前 `BDX Converter` 支持了所有的操作符(不含签名功能)，包括但不限于 `Operation 5, Operation 13, Operation 40` 和 `Operation 41` 。
```

### Comparing `BDXConverter-1.0.15/BDXConverter.egg-info/SOURCES.txt` & `BDXConverter-1.0.16/BDXConverter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.15/LICENSE` & `BDXConverter-1.0.16/LICENSE`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.15/PKG-INFO` & `BDXConverter-1.0.16/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BDXConverter
-Version: 1.0.15
+Version: 1.0.16
 Summary: A code library to marshal, unmarshal, visual and reverse visualization of BDX files
 Home-page: https://github.com/TriM-Organization/BDXConverter
 Author: Minecraft Muti-Media Organization
 Author-email: TriM-Organization@hotmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -35,14 +35,15 @@
 
 
 
 
 # 目录
 - [目录](#目录)
 - [`BDX Converter`](#bdx-converter)
+- [注意事项](#注意事项)
 - [快速上手](#快速上手)
 - [🐍 Pypi Packages](#-pypi-packages)
 - [第三方依赖](#第三方依赖)
 - [特性](#特性)
 - [什么是 `BDX` 文件](#什么是-bdx-文件)
 - [关于 `PhoenixBuilder`](#关于-phoenixbuilder)
 - [待办列表](#待办列表)
@@ -55,14 +56,21 @@
 # `BDX Converter`
 `BDX Converter` 是一个轻量化的纯 `Python` 实现，它提供了基本的 `BDX` 解析、反解析、`JSON` 可视化和反可视化功能。 
 
 
 
 
 
+# 注意事项
+- 版本 `1.0.16` 在可视化和反可视化字典方面不兼容之前的版本
+
+
+
+
+
 # 快速上手
 您可以利用 [`BDXConverter/Converter/Converter.py`](https://github.com/TriM-Organization/BDXConverter/blob/main/BDXConverter/Converter/Converter.py) 中已提供的 `4` 个函数来完成 `BDX` 文件和 `JSON` 文件的相关操作。 
 
 
 
 
 
@@ -116,26 +124,21 @@
         """
         ...
 
     def Loads(self, jsonDict: dict) -> None:
         """
         Load datas from jsonDict:dict
         """
-        if 'operationNumber' in self.__dict__:
-            jsonDict['operationNumber'] = self.operationNumber
-            jsonDict['operationName'] = self.operationName
-        for i in self.__dict__:
-            if i in jsonDict:
-                self.__dict__[i] = jsonDict[i]
+        ...
 
     def Dumps(self) -> dict:
         """
         Convert Self@GeneralClass into the basic dictionary
         """
-        return self.__dict__
+        ...
 ```
 
 因此，通过 `Marshal` 和 `UnMarshal` 函数，`BDX Converter` 可以自由的将 `二进制数据` 转换为 `Python Class` ，亦或转换回去。 <br/>
 而 `Loads` 和 `Dumps` 分别支持了把只带有基本数据类型的字典转换为 `Python Class` 亦或转换回去的功能。 
 
 目前 `BDX Converter` 支持了所有的操作符(不含签名功能)，包括但不限于 `Operation 5, Operation 13, Operation 40` 和 `Operation 41` 。
```

### Comparing `BDXConverter-1.0.15/README.md` & `BDXConverter-1.0.16/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 
 
 
 
 # 目录
 - [目录](#目录)
 - [`BDX Converter`](#bdx-converter)
+- [注意事项](#注意事项)
 - [快速上手](#快速上手)
 - [🐍 Pypi Packages](#-pypi-packages)
 - [第三方依赖](#第三方依赖)
 - [特性](#特性)
 - [什么是 `BDX` 文件](#什么是-bdx-文件)
 - [关于 `PhoenixBuilder`](#关于-phoenixbuilder)
 - [待办列表](#待办列表)
@@ -41,14 +42,21 @@
 # `BDX Converter`
 `BDX Converter` 是一个轻量化的纯 `Python` 实现，它提供了基本的 `BDX` 解析、反解析、`JSON` 可视化和反可视化功能。 
 
 
 
 
 
+# 注意事项
+- 版本 `1.0.16` 在可视化和反可视化字典方面不兼容之前的版本
+
+
+
+
+
 # 快速上手
 您可以利用 [`BDXConverter/Converter/Converter.py`](https://github.com/TriM-Organization/BDXConverter/blob/main/BDXConverter/Converter/Converter.py) 中已提供的 `4` 个函数来完成 `BDX` 文件和 `JSON` 文件的相关操作。 
 
 
 
 
 
@@ -102,26 +110,21 @@
         """
         ...
 
     def Loads(self, jsonDict: dict) -> None:
         """
         Load datas from jsonDict:dict
         """
-        if 'operationNumber' in self.__dict__:
-            jsonDict['operationNumber'] = self.operationNumber
-            jsonDict['operationName'] = self.operationName
-        for i in self.__dict__:
-            if i in jsonDict:
-                self.__dict__[i] = jsonDict[i]
+        ...
 
     def Dumps(self) -> dict:
         """
         Convert Self@GeneralClass into the basic dictionary
         """
-        return self.__dict__
+        ...
 ```
 
 因此，通过 `Marshal` 和 `UnMarshal` 函数，`BDX Converter` 可以自由的将 `二进制数据` 转换为 `Python Class` ，亦或转换回去。 <br/>
 而 `Loads` 和 `Dumps` 分别支持了把只带有基本数据类型的字典转换为 `Python Class` 亦或转换回去的功能。 
 
 目前 `BDX Converter` 支持了所有的操作符(不含签名功能)，包括但不限于 `Operation 5, Operation 13, Operation 40` 和 `Operation 41` 。
```

### Comparing `BDXConverter-1.0.15/setup.py` & `BDXConverter-1.0.16/setup.py`

 * *Files identical despite different names*

