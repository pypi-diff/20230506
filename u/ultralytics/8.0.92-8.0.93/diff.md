# Comparing `tmp/ultralytics-8.0.92.tar.gz` & `tmp/ultralytics-8.0.93.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ultralytics-8.0.92.tar", last modified: Wed May  3 23:28:53 2023, max compression
+gzip compressed data, was "ultralytics-8.0.93.tar", last modified: Fri May  5 23:14:31 2023, max compression
```

## Comparing `ultralytics-8.0.92.tar` & `ultralytics-8.0.93.tar`

### file list

```diff
@@ -1,179 +1,180 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:28:53.674922 ultralytics-8.0.92/
--rw-r--r--   0 runner    (1001) docker     (123)     5624 2023-05-03 23:27:16.000000 ultralytics-8.0.92/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-03 23:27:16.000000 ultralytics-8.0.92/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-03 23:27:16.000000 ultralytics-8.0.92/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    25796 2023-05-03 23:28:53.674922 ultralytics-8.0.92/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    24235 2023-05-03 23:27:16.000000 ultralytics-8.0.92/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    23225 2023-05-03 23:27:16.000000 ultralytics-8.0.92/README.zh-CN.md
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-05-03 23:27:16.000000 ultralytics-8.0.92/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-03 23:28:53.674922 ultralytics-8.0.92/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-05-03 23:27:16.000000 ultralytics-8.0.92/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:28:53.658922 ultralytics-8.0.92/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-05-03 23:27:16.000000 ultralytics-8.0.92/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-05-03 23:27:16.000000 ultralytics-8.0.92/tests/test_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     7099 2023-05-03 23:27:16.000000 ultralytics-8.0.92/tests/test_python.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:28:53.658922 ultralytics-8.0.92/ultralytics/
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:28:53.658922 ultralytics-8.0.92/ultralytics/assets/
--rw-r--r--   0 runner    (1001) docker     (123)   137419 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/assets/bus.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    50427 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/assets/zidane.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:28:53.658922 ultralytics-8.0.92/ultralytics/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/datasets/Argoverse.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/datasets/GlobalWheat2020.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    42439 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/datasets/ImageNet.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     9270 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/datasets/Objects365.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/datasets/SKU-110K.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/datasets/VOC.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/datasets/VisDrone.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/datasets/coco-pose.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/datasets/coco.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/datasets/coco128-seg.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/datasets/coco128.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/datasets/coco8-pose.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/datasets/coco8-seg.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/datasets/coco8.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5178 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/datasets/xView.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:28:53.658922 ultralytics-8.0.92/ultralytics/hub/
--rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/hub/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     8479 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/hub/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     9157 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/hub/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:28:53.654922 ultralytics-8.0.92/ultralytics/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:28:53.662922 ultralytics-8.0.92/ultralytics/models/v3/
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/models/v3/yolov3-spp.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/models/v3/yolov3-tiny.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/models/v3/yolov3.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:28:53.662922 ultralytics-8.0.92/ultralytics/models/v5/
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/models/v5/yolov5-p6.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/models/v5/yolov5.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:28:53.662922 ultralytics-8.0.92/ultralytics/models/v8/
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/models/v8/yolov8-cls.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/models/v8/yolov8-p2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/models/v8/yolov8-p6.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/models/v8/yolov8-pose-p6.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/models/v8/yolov8-pose.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/models/v8/yolov8-seg.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/models/v8/yolov8.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:28:53.662922 ultralytics-8.0.92/ultralytics/nn/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/nn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24243 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/nn/autobackend.py
--rw-r--r--   0 runner    (1001) docker     (123)    12509 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/nn/autoshape.py
--rw-r--r--   0 runner    (1001) docker     (123)    25079 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/nn/modules.py
--rw-r--r--   0 runner    (1001) docker     (123)    27170 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/nn/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:28:53.662922 ultralytics-8.0.92/ultralytics/tracker/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/tracker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:28:53.662922 ultralytics-8.0.92/ultralytics/tracker/cfg/
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/tracker/cfg/botsort.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/tracker/cfg/bytetrack.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/tracker/track.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:28:53.662922 ultralytics-8.0.92/ultralytics/tracker/trackers/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/tracker/trackers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/tracker/trackers/basetrack.py
--rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/tracker/trackers/bot_sort.py
--rw-r--r--   0 runner    (1001) docker     (123)    14448 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/tracker/trackers/byte_tracker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:28:53.662922 ultralytics-8.0.92/ultralytics/tracker/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/tracker/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12214 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/tracker/utils/gmc.py
--rw-r--r--   0 runner    (1001) docker     (123)    18420 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/tracker/utils/kalman_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     8699 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/tracker/utils/matching.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:28:53.662922 ultralytics-8.0.92/ultralytics/vit/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/vit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:28:53.662922 ultralytics-8.0.92/ultralytics/vit/sam/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/vit/sam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13304 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/vit/sam/amg.py
--rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/vit/sam/autosize.py
--rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/vit/sam/build.py
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/vit/sam/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:28:53.666922 ultralytics-8.0.92/ultralytics/vit/sam/modules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/vit/sam/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6347 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/vit/sam/modules/decoders.py
--rw-r--r--   0 runner    (1001) docker     (123)    22502 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/vit/sam/modules/encoders.py
--rw-r--r--   0 runner    (1001) docker     (123)    15250 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/vit/sam/modules/mask_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11201 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/vit/sam/modules/prompt_predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)     7116 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/vit/sam/modules/sam.py
--rw-r--r--   0 runner    (1001) docker     (123)     8489 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/vit/sam/modules/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/vit/sam/predict.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:28:53.666922 ultralytics-8.0.92/ultralytics/yolo/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:28:53.666922 ultralytics-8.0.92/ultralytics/yolo/cfg/
--rw-r--r--   0 runner    (1001) docker     (123)    17675 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/cfg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6172 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/cfg/default.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:28:53.666922 ultralytics-8.0.92/ultralytics/yolo/data/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/data/annotator.py
--rw-r--r--   0 runner    (1001) docker     (123)    33512 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/data/augment.py
--rw-r--r--   0 runner    (1001) docker     (123)    11763 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/data/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6556 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/data/build.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:28:53.666922 ultralytics-8.0.92/ultralytics/yolo/data/dataloaders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/data/dataloaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13777 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/data/dataloaders/stream_loaders.py
--rw-r--r--   0 runner    (1001) docker     (123)    17646 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/data/dataloaders/v5augmentations.py
--rw-r--r--   0 runner    (1001) docker     (123)    51260 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/data/dataloaders/v5loader.py
--rw-r--r--   0 runner    (1001) docker     (123)    11980 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/data/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/data/dataset_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)    22741 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/data/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:28:53.666922 ultralytics-8.0.92/ultralytics/yolo/engine/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40265 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/engine/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)    21937 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/engine/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    15913 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/engine/predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)    20388 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/engine/results.py
--rw-r--r--   0 runner    (1001) docker     (123)    31310 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/engine/trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11462 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/engine/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:28:53.670922 ultralytics-8.0.92/ultralytics/yolo/utils/
--rw-r--r--   0 runner    (1001) docker     (123)    27889 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/utils/autobatch.py
--rw-r--r--   0 runner    (1001) docker     (123)     6676 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/utils/benchmarks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:28:53.670922 ultralytics-8.0.92/ultralytics/yolo/utils/callbacks/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/utils/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5544 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/utils/callbacks/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5831 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/utils/callbacks/clearml.py
--rw-r--r--   0 runner    (1001) docker     (123)    13190 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/utils/callbacks/comet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/utils/callbacks/hub.py
--rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/utils/callbacks/mlflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     3830 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/utils/callbacks/neptune.py
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/utils/callbacks/raytune.py
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/utils/callbacks/tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/utils/callbacks/wb.py
--rw-r--r--   0 runner    (1001) docker     (123)    14881 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/utils/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/utils/dist.py
--rw-r--r--   0 runner    (1001) docker     (123)    11486 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/utils/downloads.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/utils/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/utils/files.py
--rw-r--r--   0 runner    (1001) docker     (123)    14176 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/utils/instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/utils/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)    41829 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/utils/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    28191 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/utils/ops.py
--rw-r--r--   0 runner    (1001) docker     (123)    24037 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/utils/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)    13220 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/utils/tal.py
--rw-r--r--   0 runner    (1001) docker     (123)    20019 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/utils/torch_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/utils/tuner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:28:53.670922 ultralytics-8.0.92/ultralytics/yolo/v8/
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/v8/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:28:53.670922 ultralytics-8.0.92/ultralytics/yolo/v8/classify/
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/v8/classify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/v8/classify/predict.py
--rw-r--r--   0 runner    (1001) docker     (123)     7194 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/v8/classify/train.py
--rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/v8/classify/val.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:28:53.670922 ultralytics-8.0.92/ultralytics/yolo/v8/detect/
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/v8/detect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/v8/detect/predict.py
--rw-r--r--   0 runner    (1001) docker     (123)    12199 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/v8/detect/train.py
--rw-r--r--   0 runner    (1001) docker     (123)    14425 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/v8/detect/val.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:28:53.674922 ultralytics-8.0.92/ultralytics/yolo/v8/pose/
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/v8/pose/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/v8/pose/predict.py
--rw-r--r--   0 runner    (1001) docker     (123)     7836 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/v8/pose/train.py
--rw-r--r--   0 runner    (1001) docker     (123)    10840 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/v8/pose/val.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:28:53.674922 ultralytics-8.0.92/ultralytics/yolo/v8/segment/
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/v8/segment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/v8/segment/predict.py
--rw-r--r--   0 runner    (1001) docker     (123)     8283 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/v8/segment/train.py
--rw-r--r--   0 runner    (1001) docker     (123)    12776 2023-05-03 23:27:16.000000 ultralytics-8.0.92/ultralytics/yolo/v8/segment/val.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:28:53.658922 ultralytics-8.0.92/ultralytics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    25796 2023-05-03 23:28:53.000000 ultralytics-8.0.92/ultralytics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5023 2023-05-03 23:28:53.000000 ultralytics-8.0.92/ultralytics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 23:28:53.000000 ultralytics-8.0.92/ultralytics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-03 23:28:53.000000 ultralytics-8.0.92/ultralytics.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-03 23:28:53.000000 ultralytics-8.0.92/ultralytics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-03 23:28:53.000000 ultralytics-8.0.92/ultralytics.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 23:14:31.110600 ultralytics-8.0.93/
+-rw-r--r--   0 runner    (1001) docker     (123)     5624 2023-05-05 23:12:57.000000 ultralytics-8.0.93/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-05 23:12:57.000000 ultralytics-8.0.93/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-05 23:12:57.000000 ultralytics-8.0.93/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    25796 2023-05-05 23:14:31.110600 ultralytics-8.0.93/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    24235 2023-05-05 23:12:57.000000 ultralytics-8.0.93/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    23225 2023-05-05 23:12:57.000000 ultralytics-8.0.93/README.zh-CN.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-05-05 23:12:57.000000 ultralytics-8.0.93/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-05 23:14:31.110600 ultralytics-8.0.93/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-05-05 23:12:57.000000 ultralytics-8.0.93/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 23:14:31.090600 ultralytics-8.0.93/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-05-05 23:12:57.000000 ultralytics-8.0.93/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-05-05 23:12:57.000000 ultralytics-8.0.93/tests/test_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7099 2023-05-05 23:12:57.000000 ultralytics-8.0.93/tests/test_python.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 23:14:31.090600 ultralytics-8.0.93/ultralytics/
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 23:14:31.090600 ultralytics-8.0.93/ultralytics/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)   137419 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/assets/bus.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    50427 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/assets/zidane.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 23:14:31.094600 ultralytics-8.0.93/ultralytics/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/datasets/Argoverse.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/datasets/GlobalWheat2020.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    42439 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/datasets/ImageNet.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     9270 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/datasets/Objects365.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/datasets/SKU-110K.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/datasets/VOC.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/datasets/VisDrone.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/datasets/coco-pose.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/datasets/coco.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/datasets/coco128-seg.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/datasets/coco128.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/datasets/coco8-pose.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/datasets/coco8-seg.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/datasets/coco8.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5178 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/datasets/xView.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 23:14:31.094600 ultralytics-8.0.93/ultralytics/hub/
+-rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/hub/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8479 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/hub/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9157 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/hub/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 23:14:31.086599 ultralytics-8.0.93/ultralytics/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 23:14:31.094600 ultralytics-8.0.93/ultralytics/models/v3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/models/v3/yolov3-spp.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/models/v3/yolov3-tiny.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/models/v3/yolov3.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 23:14:31.094600 ultralytics-8.0.93/ultralytics/models/v5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/models/v5/yolov5-p6.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/models/v5/yolov5.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 23:14:31.094600 ultralytics-8.0.93/ultralytics/models/v8/
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/models/v8/yolov8-cls.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/models/v8/yolov8-p2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/models/v8/yolov8-p6.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/models/v8/yolov8-pose-p6.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/models/v8/yolov8-pose.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/models/v8/yolov8-seg.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/models/v8/yolov8.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 23:14:31.098600 ultralytics-8.0.93/ultralytics/nn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/nn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24243 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/nn/autobackend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12509 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/nn/autoshape.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25079 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/nn/modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27170 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/nn/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 23:14:31.098600 ultralytics-8.0.93/ultralytics/tracker/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/tracker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 23:14:31.098600 ultralytics-8.0.93/ultralytics/tracker/cfg/
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/tracker/cfg/botsort.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/tracker/cfg/bytetrack.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/tracker/track.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 23:14:31.098600 ultralytics-8.0.93/ultralytics/tracker/trackers/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/tracker/trackers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/tracker/trackers/basetrack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/tracker/trackers/bot_sort.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14448 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/tracker/trackers/byte_tracker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 23:14:31.098600 ultralytics-8.0.93/ultralytics/tracker/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/tracker/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12214 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/tracker/utils/gmc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18420 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/tracker/utils/kalman_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8699 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/tracker/utils/matching.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 23:14:31.098600 ultralytics-8.0.93/ultralytics/vit/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/vit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 23:14:31.098600 ultralytics-8.0.93/ultralytics/vit/sam/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/vit/sam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13304 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/vit/sam/amg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/vit/sam/autosize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/vit/sam/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/vit/sam/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 23:14:31.102600 ultralytics-8.0.93/ultralytics/vit/sam/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/vit/sam/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6347 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/vit/sam/modules/decoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22502 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/vit/sam/modules/encoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15250 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/vit/sam/modules/mask_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11201 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/vit/sam/modules/prompt_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7116 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/vit/sam/modules/sam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8489 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/vit/sam/modules/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/vit/sam/predict.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 23:14:31.102600 ultralytics-8.0.93/ultralytics/yolo/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 23:14:31.102600 ultralytics-8.0.93/ultralytics/yolo/cfg/
+-rw-r--r--   0 runner    (1001) docker     (123)    17819 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/cfg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6168 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/cfg/default.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 23:14:31.102600 ultralytics-8.0.93/ultralytics/yolo/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/data/annotator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33512 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/data/augment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11763 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/data/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6556 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/data/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9190 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/data/converter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 23:14:31.102600 ultralytics-8.0.93/ultralytics/yolo/data/dataloaders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/data/dataloaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13777 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/data/dataloaders/stream_loaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17646 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/data/dataloaders/v5augmentations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51260 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/data/dataloaders/v5loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11980 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/data/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/data/dataset_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22741 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/data/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 23:14:31.102600 ultralytics-8.0.93/ultralytics/yolo/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40265 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/engine/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21937 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/engine/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15927 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/engine/predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20634 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/engine/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31310 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/engine/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11462 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/engine/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 23:14:31.106600 ultralytics-8.0.93/ultralytics/yolo/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)    27889 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/utils/autobatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6676 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/utils/benchmarks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 23:14:31.106600 ultralytics-8.0.93/ultralytics/yolo/utils/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/utils/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5544 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/utils/callbacks/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5831 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/utils/callbacks/clearml.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13190 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/utils/callbacks/comet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/utils/callbacks/hub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/utils/callbacks/mlflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3830 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/utils/callbacks/neptune.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/utils/callbacks/raytune.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/utils/callbacks/tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/utils/callbacks/wb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14881 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/utils/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/utils/dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11486 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/utils/downloads.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/utils/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/utils/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14176 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/utils/instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/utils/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41829 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/utils/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28191 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/utils/ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24037 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/utils/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13220 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/utils/tal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20019 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/utils/torch_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/utils/tuner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 23:14:31.106600 ultralytics-8.0.93/ultralytics/yolo/v8/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/v8/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 23:14:31.110600 ultralytics-8.0.93/ultralytics/yolo/v8/classify/
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/v8/classify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/v8/classify/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7194 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/v8/classify/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/v8/classify/val.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 23:14:31.110600 ultralytics-8.0.93/ultralytics/yolo/v8/detect/
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/v8/detect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/v8/detect/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12199 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/v8/detect/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14425 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/v8/detect/val.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 23:14:31.110600 ultralytics-8.0.93/ultralytics/yolo/v8/pose/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/v8/pose/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/v8/pose/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7836 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/v8/pose/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10840 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/v8/pose/val.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 23:14:31.110600 ultralytics-8.0.93/ultralytics/yolo/v8/segment/
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/v8/segment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/v8/segment/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8283 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/v8/segment/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12776 2023-05-05 23:12:57.000000 ultralytics-8.0.93/ultralytics/yolo/v8/segment/val.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 23:14:31.090600 ultralytics-8.0.93/ultralytics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    25796 2023-05-05 23:14:31.000000 ultralytics-8.0.93/ultralytics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-05-05 23:14:31.000000 ultralytics-8.0.93/ultralytics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 23:14:31.000000 ultralytics-8.0.93/ultralytics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-05 23:14:31.000000 ultralytics-8.0.93/ultralytics.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-05 23:14:31.000000 ultralytics-8.0.93/ultralytics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-05 23:14:31.000000 ultralytics-8.0.93/ultralytics.egg-info/top_level.txt
```

### Comparing `ultralytics-8.0.92/CONTRIBUTING.md` & `ultralytics-8.0.93/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.92/LICENSE` & `ultralytics-8.0.93/LICENSE`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.92/PKG-INFO` & `ultralytics-8.0.93/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ultralytics
-Version: 8.0.92
+Version: 8.0.93
 Summary: Ultralytics YOLOv8
 Home-page: https://github.com/ultralytics/ultralytics
 Author: Ultralytics
 Author-email: hello@ultralytics.com
 License: AGPL-3.0
 Project-URL: Bug Reports, https://github.com/ultralytics/ultralytics/issues
 Project-URL: Funding, https://ultralytics.com
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ultralytics Version: 8.0.92 Summary: Ultralytics
+Metadata-Version: 2.1 Name: ultralytics Version: 8.0.93 Summary: Ultralytics
 YOLOv8 Home-page: https://github.com/ultralytics/ultralytics Author:
 Ultralytics Author-email: hello@ultralytics.com License: AGPL-3.0 Project-URL:
 Bug Reports, https://github.com/ultralytics/ultralytics/issues Project-URL:
 Funding, https://ultralytics.com Project-URL: Source, https://github.com/
 ultralytics/ultralytics Keywords: machine-learning,deep-
 learning,vision,ML,DL,AI,YOLO,YOLOv3,YOLOv5,YOLOv8,HUB,Ultralytics Classifier:
 Development Status :: 4 - Beta Classifier: Intended Audience :: Developers
```

### Comparing `ultralytics-8.0.92/README.md` & `ultralytics-8.0.93/README.md`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.92/README.zh-CN.md` & `ultralytics-8.0.93/README.zh-CN.md`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.92/requirements.txt` & `ultralytics-8.0.93/requirements.txt`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.92/setup.cfg` & `ultralytics-8.0.93/setup.cfg`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.92/setup.py` & `ultralytics-8.0.93/setup.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.92/tests/test_cli.py` & `ultralytics-8.0.93/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.92/tests/test_engine.py` & `ultralytics-8.0.93/tests/test_engine.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.92/tests/test_python.py` & `ultralytics-8.0.93/tests/test_python.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.92/ultralytics/assets/bus.jpg` & `ultralytics-8.0.93/ultralytics/assets/bus.jpg`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.92/ultralytics/assets/zidane.jpg` & `ultralytics-8.0.93/ultralytics/assets/zidane.jpg`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.92/ultralytics/datasets/Argoverse.yaml` & `ultralytics-8.0.93/ultralytics/datasets/Argoverse.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.92/ultralytics/datasets/GlobalWheat2020.yaml` & `ultralytics-8.0.93/ultralytics/datasets/GlobalWheat2020.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.92/ultralytics/datasets/ImageNet.yaml` & `ultralytics-8.0.93/ultralytics/datasets/ImageNet.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.92/ultralytics/datasets/Objects365.yaml` & `ultralytics-8.0.93/ultralytics/datasets/Objects365.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.92/ultralytics/datasets/SKU-110K.yaml` & `ultralytics-8.0.93/ultralytics/datasets/SKU-110K.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.92/ultralytics/datasets/VOC.yaml` & `ultralytics-8.0.93/ultralytics/datasets/VOC.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.92/ultralytics/datasets/VisDrone.yaml` & `ultralytics-8.0.93/ultralytics/datasets/VisDrone.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.92/ultralytics/datasets/coco-pose.yaml` & `ultralytics-8.0.93/ultralytics/datasets/coco-pose.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.92/ultralytics/datasets/coco.yaml` & `ultralytics-8.0.93/ultralytics/datasets/coco.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.92/ultralytics/datasets/coco128-seg.yaml` & `ultralytics-8.0.93/ultralytics/datasets/coco128-seg.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.92/ultralytics/datasets/coco128.yaml` & `ultralytics-8.0.93/ultralytics/datasets/coco128.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.92/ultralytics/datasets/coco8-pose.yaml` & `ultralytics-8.0.93/ultralytics/datasets/coco8-pose.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.92/ultralytics/datasets/coco8-seg.yaml` & `ultralytics-8.0.93/ultralytics/datasets/coco8-seg.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.92/ultralytics/datasets/coco8.yaml` & `ultralytics-8.0.93/ultralytics/datasets/coco8.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.92/ultralytics/datasets/xView.yaml` & `ultralytics-8.0.93/ultralytics/datasets/xView.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.92/ultralytics/hub/__init__.py` & `ultralytics-8.0.93/ultralytics/hub/__init__.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.92/ultralytics/hub/auth.py` & `ultralytics-8.0.93/ultralytics/hub/auth.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.92/ultralytics/hub/session.py` & `ultralytics-8.0.93/ultralytics/hub/session.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.92/ultralytics/hub/utils.py` & `ultralytics-8.0.93/ultralytics/hub/utils.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.92/ultralytics/models/v3/yolov3-spp.yaml` & `ultralytics-8.0.93/ultralytics/models/v3/yolov3-spp.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.92/ultralytics/models/v3/yolov3-tiny.yaml` & `ultralytics-8.0.93/ultralytics/models/v3/yolov3-tiny.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.92/ultralytics/models/v3/yolov3.yaml` & `ultralytics-8.0.93/ultralytics/models/v3/yolov3.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.92/ultralytics/models/v5/yolov5-p6.yaml` & `ultralytics-8.0.93/ultralytics/models/v5/yolov5-p6.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.92/ultralytics/models/v5/yolov5.yaml` & `ultralytics-8.0.93/ultralytics/models/v5/yolov5.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.92/ultralytics/models/v8/yolov8-cls.yaml` & `ultralytics-8.0.93/ultralytics/models/v8/yolov8-cls.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.92/ultralytics/models/v8/yolov8-p2.yaml` & `ultralytics-8.0.93/ultralytics/models/v8/yolov8-p2.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.92/ultralytics/models/v8/yolov8-p6.yaml` & `ultralytics-8.0.93/ultralytics/models/v8/yolov8-p6.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.92/ultralytics/models/v8/yolov8-pose-p6.yaml` & `ultralytics-8.0.93/ultralytics/models/v8/yolov8-pose-p6.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.92/ultralytics/models/v8/yolov8-pose.yaml` & `ultralytics-8.0.93/ultralytics/models/v8/yolov8-pose.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.92/ultralytics/models/v8/yolov8-seg.yaml` & `ultralytics-8.0.93/ultralytics/models/v8/yolov8-seg.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.92/ultralytics/models/v8/yolov8.yaml` & `ultralytics-8.0.93/ultralytics/models/v8/yolov8.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.92/ultralytics/nn/autobackend.py` & `ultralytics-8.0.93/ultralytics/nn/autobackend.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.92/ultralytics/nn/autoshape.py` & `ultralytics-8.0.93/ultralytics/nn/autoshape.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.92/ultralytics/nn/modules.py` & `ultralytics-8.0.93/ultralytics/nn/modules.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.92/ultralytics/nn/tasks.py` & `ultralytics-8.0.93/ultralytics/nn/tasks.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.92/ultralytics/tracker/cfg/botsort.yaml` & `ultralytics-8.0.93/ultralytics/tracker/cfg/botsort.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.92/ultralytics/tracker/cfg/bytetrack.yaml` & `ultralytics-8.0.93/ultralytics/tracker/cfg/bytetrack.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.92/ultralytics/tracker/track.py` & `ultralytics-8.0.93/ultralytics/tracker/track.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.92/ultralytics/tracker/trackers/basetrack.py` & `ultralytics-8.0.93/ultralytics/tracker/trackers/basetrack.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.92/ultralytics/tracker/trackers/bot_sort.py` & `ultralytics-8.0.93/ultralytics/tracker/trackers/bot_sort.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.92/ultralytics/tracker/trackers/byte_tracker.py` & `ultralytics-8.0.93/ultralytics/tracker/trackers/byte_tracker.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.92/ultralytics/tracker/utils/gmc.py` & `ultralytics-8.0.93/ultralytics/tracker/utils/gmc.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.92/ultralytics/tracker/utils/kalman_filter.py` & `ultralytics-8.0.93/ultralytics/tracker/utils/kalman_filter.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.92/ultralytics/tracker/utils/matching.py` & `ultralytics-8.0.93/ultralytics/tracker/utils/matching.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.92/ultralytics/vit/sam/amg.py` & `ultralytics-8.0.93/ultralytics/vit/sam/amg.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.92/ultralytics/vit/sam/autosize.py` & `ultralytics-8.0.93/ultralytics/vit/sam/autosize.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.92/ultralytics/vit/sam/build.py` & `ultralytics-8.0.93/ultralytics/vit/sam/build.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.92/ultralytics/vit/sam/model.py` & `ultralytics-8.0.93/ultralytics/vit/sam/model.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.92/ultralytics/vit/sam/modules/decoders.py` & `ultralytics-8.0.93/ultralytics/vit/sam/modules/decoders.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.92/ultralytics/vit/sam/modules/encoders.py` & `ultralytics-8.0.93/ultralytics/vit/sam/modules/encoders.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.92/ultralytics/vit/sam/modules/mask_generator.py` & `ultralytics-8.0.93/ultralytics/vit/sam/modules/mask_generator.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.92/ultralytics/vit/sam/modules/prompt_predictor.py` & `ultralytics-8.0.93/ultralytics/vit/sam/modules/prompt_predictor.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.92/ultralytics/vit/sam/modules/sam.py` & `ultralytics-8.0.93/ultralytics/vit/sam/modules/sam.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.92/ultralytics/vit/sam/modules/transformer.py` & `ultralytics-8.0.93/ultralytics/vit/sam/modules/transformer.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.92/ultralytics/vit/sam/predict.py` & `ultralytics-8.0.93/ultralytics/vit/sam/predict.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.92/ultralytics/yolo/cfg/__init__.py` & `ultralytics-8.0.93/ultralytics/yolo/cfg/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 
 # Define keys for arg type checks
 CFG_FLOAT_KEYS = 'warmup_epochs', 'box', 'cls', 'dfl', 'degrees', 'shear'
 CFG_FRACTION_KEYS = ('dropout', 'iou', 'lr0', 'lrf', 'momentum', 'weight_decay', 'warmup_momentum', 'warmup_bias_lr',
                      'label_smoothing', 'hsv_h', 'hsv_s', 'hsv_v', 'translate', 'scale', 'perspective', 'flipud',
                      'fliplr', 'mosaic', 'mixup', 'copy_paste', 'conf', 'iou')  # fractional floats limited to 0.0 - 1.0
 CFG_INT_KEYS = ('epochs', 'patience', 'batch', 'workers', 'seed', 'close_mosaic', 'mask_ratio', 'max_det', 'vid_stride',
-                'line_thickness', 'workspace', 'nbs', 'save_period')
+                'line_width', 'workspace', 'nbs', 'save_period')
 CFG_BOOL_KEYS = ('save', 'exist_ok', 'verbose', 'deterministic', 'single_cls', 'rect', 'cos_lr', 'overlap_mask', 'val',
                  'save_json', 'save_hybrid', 'half', 'dnn', 'plots', 'show', 'save_txt', 'save_conf', 'save_crop',
                  'show_labels', 'show_conf', 'visualize', 'augment', 'agnostic_nms', 'retina_masks', 'boxes', 'keras',
                  'optimize', 'int8', 'dynamic', 'simplify', 'nms', 'v5loader')
 
 
 def cfg2dict(cfg):
@@ -148,14 +148,17 @@
     for key in custom.copy().keys():
         if key == 'hide_labels':
             deprecation_warn(key, 'show_labels')
             custom['show_labels'] = custom.pop('hide_labels') == 'False'
         if key == 'hide_conf':
             deprecation_warn(key, 'show_conf')
             custom['show_conf'] = custom.pop('hide_conf') == 'False'
+        if key == 'line_thickness':
+            deprecation_warn(key, 'line_width')
+            custom['line_width'] = custom.pop('line_thickness')
 
     return custom
 
 
 def check_cfg_mismatch(base: Dict, custom: Dict, e=None):
     """
     This function checks for any mismatched keys between a custom configuration list and a base configuration list.
```

### Comparing `ultralytics-8.0.92/ultralytics/yolo/cfg/default.yaml` & `ultralytics-8.0.93/ultralytics/yolo/cfg/default.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 show: False  # show results if possible
 save_txt: False  # save results as .txt file
 save_conf: False  # save results with confidence scores
 save_crop: False  # save cropped images with results
 show_labels: True  # show object labels in plots
 show_conf: True  # show object confidence scores in plots
 vid_stride: 1  # video frame-rate stride
-line_thickness: 3  # bounding box thickness (pixels)
+line_width:   # line width of the bounding boxes
 visualize: False  # visualize model features
 augment: False  # apply image augmentation to prediction sources
 agnostic_nms: False  # class-agnostic NMS
 classes:  # filter results by class, i.e. class=0, or class=[0,2,3]
 retina_masks: False  # use high-resolution segmentation masks
 boxes: True  # Show boxes in segmentation predictions
```

### Comparing `ultralytics-8.0.92/ultralytics/yolo/data/annotator.py` & `ultralytics-8.0.93/ultralytics/yolo/data/annotator.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,23 +4,21 @@
 from ultralytics.vit.sam import PromptPredictor, build_sam
 from ultralytics.yolo.utils.torch_utils import select_device
 
 
 def auto_annotate(data, det_model='yolov8x.pt', sam_model='sam_b.pt', device='', output_dir=None):
     """
     Automatically annotates images using a YOLO object detection model and a SAM segmentation model.
-
     Args:
         data (str): Path to a folder containing images to be annotated.
         det_model (str, optional): Pre-trained YOLO detection model. Defaults to 'yolov8x.pt'.
         sam_model (str, optional): Pre-trained SAM segmentation model. Defaults to 'sam_b.pt'.
         device (str, optional): Device to run the models on. Defaults to an empty string (CPU or GPU, if available).
         output_dir (str, None, optional): Directory to save the annotated results.
             Defaults to a 'labels' folder in the same directory as 'data'.
-
     """
     device = select_device(device)
     det_model = YOLO(det_model)
     sam_model = build_sam(sam_model)
     det_model.to(device)
     sam_model.to(device)
 
@@ -30,25 +28,26 @@
 
     prompt_predictor = PromptPredictor(sam_model)
     det_results = det_model(data, stream=True)
 
     for result in det_results:
         boxes = result.boxes.xyxy  # Boxes object for bbox outputs
         class_ids = result.boxes.cls.int().tolist()  # noqa
-        prompt_predictor.set_image(result.orig_img)
-        masks, _, _ = prompt_predictor.predict_torch(
-            point_coords=None,
-            point_labels=None,
-            boxes=prompt_predictor.transform.apply_boxes_torch(boxes, result.orig_shape[:2]),
-            multimask_output=False,
-        )
-
-        result.update(masks=masks.squeeze(1))
-        segments = result.masks.xyn  # noqa
-
-        with open(f'{str(Path(output_dir) / Path(result.path).stem)}.txt', 'w') as f:
-            for i in range(len(segments)):
-                s = segments[i]
-                if len(s) == 0:
-                    continue
-                segment = map(str, segments[i].reshape(-1).tolist())
-                f.write(f'{class_ids[i]} ' + ' '.join(segment) + '\n')
+        if len(class_ids):
+            prompt_predictor.set_image(result.orig_img)
+            masks, _, _ = prompt_predictor.predict_torch(
+                point_coords=None,
+                point_labels=None,
+                boxes=prompt_predictor.transform.apply_boxes_torch(boxes, result.orig_shape[:2]),
+                multimask_output=False,
+            )
+
+            result.update(masks=masks.squeeze(1))
+            segments = result.masks.xyn  # noqa
+
+            with open(str(Path(output_dir) / Path(result.path).stem) + '.txt', 'w') as f:
+                for i in range(len(segments)):
+                    s = segments[i]
+                    if len(s) == 0:
+                        continue
+                    segment = map(str, segments[i].reshape(-1).tolist())
+                    f.write(f'{class_ids[i]} ' + ' '.join(segment) + '\n')
```

### Comparing `ultralytics-8.0.92/ultralytics/yolo/data/augment.py` & `ultralytics-8.0.93/ultralytics/yolo/data/augment.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.92/ultralytics/yolo/data/base.py` & `ultralytics-8.0.93/ultralytics/yolo/data/base.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.92/ultralytics/yolo/data/build.py` & `ultralytics-8.0.93/ultralytics/yolo/data/build.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.92/ultralytics/yolo/data/dataloaders/stream_loaders.py` & `ultralytics-8.0.93/ultralytics/yolo/data/dataloaders/stream_loaders.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.92/ultralytics/yolo/data/dataloaders/v5augmentations.py` & `ultralytics-8.0.93/ultralytics/yolo/data/dataloaders/v5augmentations.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.92/ultralytics/yolo/data/dataloaders/v5loader.py` & `ultralytics-8.0.93/ultralytics/yolo/data/dataloaders/v5loader.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.92/ultralytics/yolo/data/dataset.py` & `ultralytics-8.0.93/ultralytics/yolo/data/dataset.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.92/ultralytics/yolo/data/dataset_wrappers.py` & `ultralytics-8.0.93/ultralytics/yolo/data/dataset_wrappers.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.92/ultralytics/yolo/data/utils.py` & `ultralytics-8.0.93/ultralytics/yolo/data/utils.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.92/ultralytics/yolo/engine/exporter.py` & `ultralytics-8.0.93/ultralytics/yolo/engine/exporter.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.92/ultralytics/yolo/engine/model.py` & `ultralytics-8.0.93/ultralytics/yolo/engine/model.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.92/ultralytics/yolo/engine/predictor.py` & `ultralytics-8.0.93/ultralytics/yolo/engine/predictor.py`

 * *Files 3% similar despite different names*

```diff
@@ -142,15 +142,15 @@
         self.data_path = p
         self.txt_path = str(self.save_dir / 'labels' / p.stem) + ('' if self.dataset.mode == 'image' else f'_{frame}')
         log_string += '%gx%g ' % im.shape[2:]  # print string
         result = results[idx]
         log_string += result.verbose()
 
         if self.args.save or self.args.show:  # Add bbox to image
-            plot_args = dict(line_width=self.args.line_thickness,
+            plot_args = dict(line_width=self.args.line_width,
                              boxes=self.args.boxes,
                              conf=self.args.show_conf,
                              labels=self.args.show_labels)
             if not self.args.retina_masks:
                 plot_args['im_gpu'] = im[idx]
             self.plotted_img = result.plot(**plot_args)
         # Write
@@ -208,43 +208,43 @@
         if self.args.save or self.args.save_txt:
             (self.save_dir / 'labels' if self.args.save_txt else self.save_dir).mkdir(parents=True, exist_ok=True)
         # Warmup model
         if not self.done_warmup:
             self.model.warmup(imgsz=(1 if self.model.pt or self.model.triton else self.dataset.bs, 3, *self.imgsz))
             self.done_warmup = True
 
-        self.seen, self.windows, self.dt, self.batch = 0, [], (ops.Profile(), ops.Profile(), ops.Profile()), None
+        self.seen, self.windows, self.batch, profilers = 0, [], None, (ops.Profile(), ops.Profile(), ops.Profile())
         self.run_callbacks('on_predict_start')
         for batch in self.dataset:
             self.run_callbacks('on_predict_batch_start')
             self.batch = batch
             path, im0s, vid_cap, s = batch
             visualize = increment_path(self.save_dir / Path(path[0]).stem,
                                        mkdir=True) if self.args.visualize and (not self.source_type.tensor) else False
 
             # Preprocess
-            with self.dt[0]:
+            with profilers[0]:
                 im = self.preprocess(im0s)
 
             # Inference
-            with self.dt[1]:
+            with profilers[1]:
                 preds = self.model(im, augment=self.args.augment, visualize=visualize)
 
             # Postprocess
-            with self.dt[2]:
+            with profilers[2]:
                 self.results = self.postprocess(preds, im, im0s)
             self.run_callbacks('on_predict_postprocess_end')
 
             # Visualize, save, write results
             n = len(im0s)
             for i in range(n):
                 self.results[i].speed = {
-                    'preprocess': self.dt[0].dt * 1E3 / n,
-                    'inference': self.dt[1].dt * 1E3 / n,
-                    'postprocess': self.dt[2].dt * 1E3 / n}
+                    'preprocess': profilers[0].dt * 1E3 / n,
+                    'inference': profilers[1].dt * 1E3 / n,
+                    'postprocess': profilers[2].dt * 1E3 / n}
                 if self.source_type.tensor:  # skip write, show and plot operations if input is raw tensor
                     continue
                 p, im0 = path[i], im0s[i].copy()
                 p = Path(p)
 
                 if self.args.verbose or self.args.save or self.args.save_txt or self.args.show:
                     s += self.write_results(i, self.results, (p, im, im0))
@@ -255,23 +255,23 @@
                 if self.args.save and self.plotted_img is not None:
                     self.save_preds(vid_cap, i, str(self.save_dir / p.name))
             self.run_callbacks('on_predict_batch_end')
             yield from self.results
 
             # Print time (inference-only)
             if self.args.verbose:
-                LOGGER.info(f'{s}{self.dt[1].dt * 1E3:.1f}ms')
+                LOGGER.info(f'{s}{profilers[1].dt * 1E3:.1f}ms')
 
         # Release assets
         if isinstance(self.vid_writer[-1], cv2.VideoWriter):
             self.vid_writer[-1].release()  # release final video writer
 
         # Print results
         if self.args.verbose and self.seen:
-            t = tuple(x.t / self.seen * 1E3 for x in self.dt)  # speeds per image
+            t = tuple(x.t / self.seen * 1E3 for x in profilers)  # speeds per image
             LOGGER.info(f'Speed: %.1fms preprocess, %.1fms inference, %.1fms postprocess per image at shape '
                         f'{(1, 3, *self.imgsz)}' % t)
         if self.args.save or self.args.save_txt or self.args.save_crop:
             nl = len(list(self.save_dir.glob('labels/*.txt')))  # number of labels
             s = f"\n{nl} label{'s' * (nl > 1)} saved to {self.save_dir / 'labels'}" if self.args.save_txt else ''
             LOGGER.info(f"Results saved to {colorstr('bold', self.save_dir)}{s}")
```

### Comparing `ultralytics-8.0.92/ultralytics/yolo/engine/results.py` & `ultralytics-8.0.93/ultralytics/yolo/engine/results.py`

 * *Files 2% similar despite different names*

```diff
@@ -193,14 +193,19 @@
         """
         # Deprecation warn TODO: remove in 8.2
         if 'show_conf' in kwargs:
             deprecation_warn('show_conf', 'conf')
             conf = kwargs['show_conf']
             assert type(conf) == bool, '`show_conf` should be of boolean type, i.e, show_conf=True/False'
 
+        if 'show_conf' in kwargs:
+            deprecation_warn('line_thickness', 'line_width')
+            line_width = kwargs['line_thickness']
+            assert type(line_width) == int, '`line_width` should be of int type, i.e, line_width=3'
+
         names = self.names
         annotator = Annotator(deepcopy(self.orig_img if img is None else img),
                               line_width,
                               font_size,
                               font,
                               pil,
                               example=names)
```

### Comparing `ultralytics-8.0.92/ultralytics/yolo/engine/trainer.py` & `ultralytics-8.0.93/ultralytics/yolo/engine/trainer.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.92/ultralytics/yolo/engine/validator.py` & `ultralytics-8.0.93/ultralytics/yolo/engine/validator.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.92/ultralytics/yolo/utils/__init__.py` & `ultralytics-8.0.93/ultralytics/yolo/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.92/ultralytics/yolo/utils/autobatch.py` & `ultralytics-8.0.93/ultralytics/yolo/utils/autobatch.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.92/ultralytics/yolo/utils/benchmarks.py` & `ultralytics-8.0.93/ultralytics/yolo/utils/benchmarks.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.92/ultralytics/yolo/utils/callbacks/base.py` & `ultralytics-8.0.93/ultralytics/yolo/utils/callbacks/base.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.92/ultralytics/yolo/utils/callbacks/clearml.py` & `ultralytics-8.0.93/ultralytics/yolo/utils/callbacks/clearml.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.92/ultralytics/yolo/utils/callbacks/comet.py` & `ultralytics-8.0.93/ultralytics/yolo/utils/callbacks/comet.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.92/ultralytics/yolo/utils/callbacks/hub.py` & `ultralytics-8.0.93/ultralytics/yolo/utils/callbacks/hub.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.92/ultralytics/yolo/utils/callbacks/mlflow.py` & `ultralytics-8.0.93/ultralytics/yolo/utils/callbacks/mlflow.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.92/ultralytics/yolo/utils/callbacks/neptune.py` & `ultralytics-8.0.93/ultralytics/yolo/utils/callbacks/neptune.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.92/ultralytics/yolo/utils/callbacks/tensorboard.py` & `ultralytics-8.0.93/ultralytics/yolo/utils/callbacks/tensorboard.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.92/ultralytics/yolo/utils/callbacks/wb.py` & `ultralytics-8.0.93/ultralytics/yolo/utils/callbacks/wb.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.92/ultralytics/yolo/utils/checks.py` & `ultralytics-8.0.93/ultralytics/yolo/utils/checks.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.92/ultralytics/yolo/utils/dist.py` & `ultralytics-8.0.93/ultralytics/yolo/utils/dist.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.92/ultralytics/yolo/utils/downloads.py` & `ultralytics-8.0.93/ultralytics/yolo/utils/downloads.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.92/ultralytics/yolo/utils/files.py` & `ultralytics-8.0.93/ultralytics/yolo/utils/files.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Ultralytics YOLO 🚀, AGPL-3.0 license
 
 import contextlib
 import glob
 import os
+import shutil
 from datetime import datetime
 from pathlib import Path
 
 
 class WorkingDirectory(contextlib.ContextDecorator):
     """Usage: @WorkingDirectory(dir) decorator or 'with WorkingDirectory(dir):' context manager."""
 
@@ -83,7 +84,17 @@
     return 0.0
 
 
 def get_latest_run(search_dir='.'):
     """Return path to most recent 'last.pt' in /runs (i.e. to --resume from)."""
     last_list = glob.glob(f'{search_dir}/**/last*.pt', recursive=True)
     return max(last_list, key=os.path.getctime) if last_list else ''
+
+
+def make_dirs(dir='new_dir/'):
+    # Create folders
+    dir = Path(dir)
+    if dir.exists():
+        shutil.rmtree(dir)  # delete dir
+    for p in dir, dir / 'labels', dir / 'images':
+        p.mkdir(parents=True, exist_ok=True)  # make dir
+    return dir
```

### Comparing `ultralytics-8.0.92/ultralytics/yolo/utils/instance.py` & `ultralytics-8.0.93/ultralytics/yolo/utils/instance.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.92/ultralytics/yolo/utils/loss.py` & `ultralytics-8.0.93/ultralytics/yolo/utils/loss.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.92/ultralytics/yolo/utils/metrics.py` & `ultralytics-8.0.93/ultralytics/yolo/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.92/ultralytics/yolo/utils/ops.py` & `ultralytics-8.0.93/ultralytics/yolo/utils/ops.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.92/ultralytics/yolo/utils/plotting.py` & `ultralytics-8.0.93/ultralytics/yolo/utils/plotting.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.92/ultralytics/yolo/utils/tal.py` & `ultralytics-8.0.93/ultralytics/yolo/utils/tal.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.92/ultralytics/yolo/utils/torch_utils.py` & `ultralytics-8.0.93/ultralytics/yolo/utils/torch_utils.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.92/ultralytics/yolo/utils/tuner.py` & `ultralytics-8.0.93/ultralytics/yolo/utils/tuner.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.92/ultralytics/yolo/v8/classify/predict.py` & `ultralytics-8.0.93/ultralytics/yolo/v8/classify/predict.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.92/ultralytics/yolo/v8/classify/train.py` & `ultralytics-8.0.93/ultralytics/yolo/v8/classify/train.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.92/ultralytics/yolo/v8/classify/val.py` & `ultralytics-8.0.93/ultralytics/yolo/v8/classify/val.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.92/ultralytics/yolo/v8/detect/predict.py` & `ultralytics-8.0.93/ultralytics/yolo/v8/detect/predict.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.92/ultralytics/yolo/v8/detect/train.py` & `ultralytics-8.0.93/ultralytics/yolo/v8/detect/train.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.92/ultralytics/yolo/v8/detect/val.py` & `ultralytics-8.0.93/ultralytics/yolo/v8/detect/val.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.92/ultralytics/yolo/v8/pose/predict.py` & `ultralytics-8.0.93/ultralytics/yolo/v8/pose/predict.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.92/ultralytics/yolo/v8/pose/train.py` & `ultralytics-8.0.93/ultralytics/yolo/v8/pose/train.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.92/ultralytics/yolo/v8/pose/val.py` & `ultralytics-8.0.93/ultralytics/yolo/v8/pose/val.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.92/ultralytics/yolo/v8/segment/predict.py` & `ultralytics-8.0.93/ultralytics/yolo/v8/segment/predict.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.92/ultralytics/yolo/v8/segment/train.py` & `ultralytics-8.0.93/ultralytics/yolo/v8/segment/train.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.92/ultralytics/yolo/v8/segment/val.py` & `ultralytics-8.0.93/ultralytics/yolo/v8/segment/val.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.92/ultralytics.egg-info/PKG-INFO` & `ultralytics-8.0.93/ultralytics.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ultralytics
-Version: 8.0.92
+Version: 8.0.93
 Summary: Ultralytics YOLOv8
 Home-page: https://github.com/ultralytics/ultralytics
 Author: Ultralytics
 Author-email: hello@ultralytics.com
 License: AGPL-3.0
 Project-URL: Bug Reports, https://github.com/ultralytics/ultralytics/issues
 Project-URL: Funding, https://ultralytics.com
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ultralytics Version: 8.0.92 Summary: Ultralytics
+Metadata-Version: 2.1 Name: ultralytics Version: 8.0.93 Summary: Ultralytics
 YOLOv8 Home-page: https://github.com/ultralytics/ultralytics Author:
 Ultralytics Author-email: hello@ultralytics.com License: AGPL-3.0 Project-URL:
 Bug Reports, https://github.com/ultralytics/ultralytics/issues Project-URL:
 Funding, https://ultralytics.com Project-URL: Source, https://github.com/
 ultralytics/ultralytics Keywords: machine-learning,deep-
 learning,vision,ML,DL,AI,YOLO,YOLOv3,YOLOv5,YOLOv8,HUB,Ultralytics Classifier:
 Development Status :: 4 - Beta Classifier: Intended Audience :: Developers
```

### Comparing `ultralytics-8.0.92/ultralytics.egg-info/SOURCES.txt` & `ultralytics-8.0.93/ultralytics.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -84,14 +84,15 @@
 ultralytics/yolo/cfg/__init__.py
 ultralytics/yolo/cfg/default.yaml
 ultralytics/yolo/data/__init__.py
 ultralytics/yolo/data/annotator.py
 ultralytics/yolo/data/augment.py
 ultralytics/yolo/data/base.py
 ultralytics/yolo/data/build.py
+ultralytics/yolo/data/converter.py
 ultralytics/yolo/data/dataset.py
 ultralytics/yolo/data/dataset_wrappers.py
 ultralytics/yolo/data/utils.py
 ultralytics/yolo/data/dataloaders/__init__.py
 ultralytics/yolo/data/dataloaders/stream_loaders.py
 ultralytics/yolo/data/dataloaders/v5augmentations.py
 ultralytics/yolo/data/dataloaders/v5loader.py
```

