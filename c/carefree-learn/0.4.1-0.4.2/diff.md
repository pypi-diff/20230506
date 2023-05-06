# Comparing `tmp/carefree-learn-0.4.1.tar.gz` & `tmp/carefree-learn-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "carefree-learn-0.4.1.tar", last modified: Wed Apr  5 06:44:21 2023, max compression
+gzip compressed data, was "carefree-learn-0.4.2.tar", last modified: Sat May  6 05:29:58 2023, max compression
```

## Comparing `carefree-learn-0.4.1.tar` & `carefree-learn-0.4.2.tar`

### file list

```diff
@@ -1,361 +1,361 @@
-drwxrwxrwx   0        0        0        0 2023-04-05 06:44:21.010144 carefree-learn-0.4.1/
--rw-rw-rw-   0        0        0     1090 2022-10-23 14:55:07.000000 carefree-learn-0.4.1/LICENSE
--rw-rw-rw-   0        0        0       75 2022-11-10 07:33:05.000000 carefree-learn-0.4.1/MANIFEST.in
--rw-rw-rw-   0        0        0     7575 2023-04-05 06:44:21.010144 carefree-learn-0.4.1/PKG-INFO
--rw-rw-rw-   0        0        0     7038 2023-04-04 02:24:07.000000 carefree-learn-0.4.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-05 06:44:20.794792 carefree-learn-0.4.1/carefree_learn.egg-info/
--rw-rw-rw-   0        0        0     7575 2023-04-05 06:44:20.000000 carefree-learn-0.4.1/carefree_learn.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    10736 2023-04-05 06:44:20.000000 carefree-learn-0.4.1/carefree_learn.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-05 06:44:20.000000 carefree-learn-0.4.1/carefree_learn.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      601 2023-04-05 06:44:20.000000 carefree-learn-0.4.1/carefree_learn.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-05 06:44:20.000000 carefree-learn-0.4.1/carefree_learn.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-05 06:44:20.798776 carefree-learn-0.4.1/cflearn/
--rw-rw-rw-   0        0        0      658 2023-04-04 02:24:07.000000 carefree-learn-0.4.1/cflearn/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-05 06:44:20.800770 carefree-learn-0.4.1/cflearn/api/
--rw-rw-rw-   0        0        0        0 2022-10-23 14:55:07.000000 carefree-learn-0.4.1/cflearn/api/__init__.py
--rw-rw-rw-   0        0        0    24147 2023-03-27 06:18:09.000000 carefree-learn-0.4.1/cflearn/api/api.py
-drwxrwxrwx   0        0        0        0 2023-04-05 06:44:20.801766 carefree-learn-0.4.1/cflearn/api/cv/
--rw-rw-rw-   0        0        0       81 2023-03-23 05:48:39.000000 carefree-learn-0.4.1/cflearn/api/cv/__init__.py
--rw-rw-rw-   0        0        0    56578 2023-04-05 06:11:06.000000 carefree-learn-0.4.1/cflearn/api/cv/diffusion.py
-drwxrwxrwx   0        0        0        0 2023-04-05 06:44:20.804757 carefree-learn-0.4.1/cflearn/api/cv/third_party/
--rw-rw-rw-   0        0        0      156 2023-03-22 01:51:15.000000 carefree-learn-0.4.1/cflearn/api/cv/third_party/__init__.py
--rw-rw-rw-   0        0        0     1069 2023-04-04 02:24:07.000000 carefree-learn-0.4.1/cflearn/api/cv/third_party/blip.py
-drwxrwxrwx   0        0        0        0 2023-04-05 06:44:20.805753 carefree-learn-0.4.1/cflearn/api/cv/third_party/iharm/
--rw-rw-rw-   0        0        0       20 2023-03-22 01:51:15.000000 carefree-learn-0.4.1/cflearn/api/cv/third_party/iharm/__init__.py
--rw-rw-rw-   0        0        0     1386 2023-04-04 02:24:07.000000 carefree-learn-0.4.1/cflearn/api/cv/third_party/iharm/api.py
-drwxrwxrwx   0        0        0        0 2023-04-05 06:44:20.807747 carefree-learn-0.4.1/cflearn/api/cv/third_party/iharm/inference/
--rw-rw-rw-   0        0        0        0 2023-03-22 01:51:15.000000 carefree-learn-0.4.1/cflearn/api/cv/third_party/iharm/inference/__init__.py
--rw-rw-rw-   0        0        0     1989 2023-03-22 01:51:15.000000 carefree-learn-0.4.1/cflearn/api/cv/third_party/iharm/inference/predictor.py
--rw-rw-rw-   0        0        0     4395 2023-03-22 01:51:15.000000 carefree-learn-0.4.1/cflearn/api/cv/third_party/iharm/inference/transforms.py
--rw-rw-rw-   0        0        0      341 2023-03-22 01:51:15.000000 carefree-learn-0.4.1/cflearn/api/cv/third_party/iharm/inference/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-05 06:44:20.808743 carefree-learn-0.4.1/cflearn/api/cv/third_party/iharm/mconfigs/
--rw-rw-rw-   0        0        0      112 2023-03-22 01:51:15.000000 carefree-learn-0.4.1/cflearn/api/cv/third_party/iharm/mconfigs/__init__.py
--rw-rw-rw-   0        0        0     1660 2023-03-22 01:51:15.000000 carefree-learn-0.4.1/cflearn/api/cv/third_party/iharm/mconfigs/backboned.py
--rw-rw-rw-   0        0        0     1953 2023-03-22 01:51:15.000000 carefree-learn-0.4.1/cflearn/api/cv/third_party/iharm/mconfigs/base.py
-drwxrwxrwx   0        0        0        0 2023-04-05 06:44:20.810736 carefree-learn-0.4.1/cflearn/api/cv/third_party/iharm/model/
--rw-rw-rw-   0        0        0        0 2023-03-22 01:51:15.000000 carefree-learn-0.4.1/cflearn/api/cv/third_party/iharm/model/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-05 06:44:20.812730 carefree-learn-0.4.1/cflearn/api/cv/third_party/iharm/model/backboned/
--rw-rw-rw-   0        0        0       70 2023-03-22 01:51:15.000000 carefree-learn-0.4.1/cflearn/api/cv/third_party/iharm/model/backboned/__init__.py
--rw-rw-rw-   0        0        0     4553 2023-03-22 01:51:15.000000 carefree-learn-0.4.1/cflearn/api/cv/third_party/iharm/model/backboned/deeplab.py
--rw-rw-rw-   0        0        0     6090 2023-03-22 01:51:15.000000 carefree-learn-0.4.1/cflearn/api/cv/third_party/iharm/model/backboned/hrnet.py
--rw-rw-rw-   0        0        0     3629 2023-03-22 01:51:15.000000 carefree-learn-0.4.1/cflearn/api/cv/third_party/iharm/model/backboned/ih_model.py
-drwxrwxrwx   0        0        0        0 2023-04-05 06:44:20.813726 carefree-learn-0.4.1/cflearn/api/cv/third_party/iharm/model/base/
--rw-rw-rw-   0        0        0      130 2023-03-22 01:51:15.000000 carefree-learn-0.4.1/cflearn/api/cv/third_party/iharm/model/base/__init__.py
--rw-rw-rw-   0        0        0     1236 2023-03-22 01:51:15.000000 carefree-learn-0.4.1/cflearn/api/cv/third_party/iharm/model/base/dih_model.py
--rw-rw-rw-   0        0        0     1353 2023-03-22 01:51:15.000000 carefree-learn-0.4.1/cflearn/api/cv/third_party/iharm/model/base/iseunet_v1.py
--rw-rw-rw-   0        0        0     3162 2023-03-22 01:51:15.000000 carefree-learn-0.4.1/cflearn/api/cv/third_party/iharm/model/base/ssam_model.py
-drwxrwxrwx   0        0        0        0 2023-04-05 06:44:20.818710 carefree-learn-0.4.1/cflearn/api/cv/third_party/iharm/model/modeling/
--rw-rw-rw-   0        0        0        0 2023-03-22 01:51:15.000000 carefree-learn-0.4.1/cflearn/api/cv/third_party/iharm/model/modeling/__init__.py
--rw-rw-rw-   0        0        0     8010 2023-03-22 01:51:15.000000 carefree-learn-0.4.1/cflearn/api/cv/third_party/iharm/model/modeling/basic_blocks.py
--rw-rw-rw-   0        0        0     5571 2023-03-22 01:51:15.000000 carefree-learn-0.4.1/cflearn/api/cv/third_party/iharm/model/modeling/conv_autoencoder.py
--rw-rw-rw-   0        0        0     7150 2023-03-22 01:51:15.000000 carefree-learn-0.4.1/cflearn/api/cv/third_party/iharm/model/modeling/deeplab_v3.py
--rw-rw-rw-   0        0        0    19814 2023-03-22 01:51:15.000000 carefree-learn-0.4.1/cflearn/api/cv/third_party/iharm/model/modeling/hrnet_ocr.py
--rw-rw-rw-   0        0        0     6392 2023-03-22 01:51:15.000000 carefree-learn-0.4.1/cflearn/api/cv/third_party/iharm/model/modeling/ocr.py
--rw-rw-rw-   0        0        0     1808 2023-03-22 01:51:15.000000 carefree-learn-0.4.1/cflearn/api/cv/third_party/iharm/model/modeling/resnet.py
--rw-rw-rw-   0        0        0    13493 2023-03-22 01:51:15.000000 carefree-learn-0.4.1/cflearn/api/cv/third_party/iharm/model/modeling/resnetv1b.py
--rw-rw-rw-   0        0        0     8229 2023-03-22 01:51:15.000000 carefree-learn-0.4.1/cflearn/api/cv/third_party/iharm/model/modeling/unet.py
--rw-rw-rw-   0        0        0      357 2023-03-22 01:51:15.000000 carefree-learn-0.4.1/cflearn/api/cv/third_party/iharm/model/modifiers.py
--rw-rw-rw-   0        0        0     4927 2023-03-22 01:51:15.000000 carefree-learn-0.4.1/cflearn/api/cv/third_party/iharm/model/ops.py
-drwxrwxrwx   0        0        0        0 2023-04-05 06:44:20.818710 carefree-learn-0.4.1/cflearn/api/cv/third_party/iharm/utils/
--rw-rw-rw-   0        0        0        0 2023-03-22 01:51:15.000000 carefree-learn-0.4.1/cflearn/api/cv/third_party/iharm/utils/__init__.py
--rw-rw-rw-   0        0        0      445 2023-03-22 01:51:15.000000 carefree-learn-0.4.1/cflearn/api/cv/third_party/iharm/utils/misc.py
--rw-rw-rw-   0        0        0    16017 2023-04-04 02:24:07.000000 carefree-learn-0.4.1/cflearn/api/cv/third_party/isnet.py
--rw-rw-rw-   0        0        0     9132 2023-04-04 02:24:07.000000 carefree-learn-0.4.1/cflearn/api/cv/third_party/lama.py
-drwxrwxrwx   0        0        0        0 2023-04-05 06:44:20.820703 carefree-learn-0.4.1/cflearn/api/cv/third_party/midas/
--rw-rw-rw-   0        0        0       20 2023-03-22 01:51:15.000000 carefree-learn-0.4.1/cflearn/api/cv/third_party/midas/__init__.py
--rw-rw-rw-   0        0        0     8006 2023-03-22 01:51:15.000000 carefree-learn-0.4.1/cflearn/api/cv/third_party/midas/api.py
-drwxrwxrwx   0        0        0        0 2023-04-05 06:44:20.824690 carefree-learn-0.4.1/cflearn/api/cv/third_party/midas/core/
--rw-rw-rw-   0        0        0        0 2023-03-22 01:51:15.000000 carefree-learn-0.4.1/cflearn/api/cv/third_party/midas/core/__init__.py
--rw-rw-rw-   0        0        0      383 2023-03-22 01:51:15.000000 carefree-learn-0.4.1/cflearn/api/cv/third_party/midas/core/base_model.py
--rw-rw-rw-   0        0        0    10222 2023-03-22 01:51:15.000000 carefree-learn-0.4.1/cflearn/api/cv/third_party/midas/core/blocks.py
--rw-rw-rw-   0        0        0     3259 2023-03-22 01:51:15.000000 carefree-learn-0.4.1/cflearn/api/cv/third_party/midas/core/dpt_depth.py
--rw-rw-rw-   0        0        0     2803 2023-03-22 01:51:15.000000 carefree-learn-0.4.1/cflearn/api/cv/third_party/midas/core/midas_net.py
--rw-rw-rw-   0        0        0     6071 2023-03-22 01:51:15.000000 carefree-learn-0.4.1/cflearn/api/cv/third_party/midas/core/midas_net_custom.py
--rw-rw-rw-   0        0        0     8096 2023-03-22 01:51:15.000000 carefree-learn-0.4.1/cflearn/api/cv/third_party/midas/core/transforms.py
--rw-rw-rw-   0        0        0    15154 2023-03-22 01:51:15.000000 carefree-learn-0.4.1/cflearn/api/cv/third_party/midas/core/vit.py
--rw-rw-rw-   0        0        0     4814 2023-03-22 01:51:15.000000 carefree-learn-0.4.1/cflearn/api/cv/third_party/midas/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-05 06:44:20.825686 carefree-learn-0.4.1/cflearn/api/cv/third_party/mlsd/
--rw-rw-rw-   0        0        0       20 2023-03-22 01:51:15.000000 carefree-learn-0.4.1/cflearn/api/cv/third_party/mlsd/__init__.py
--rw-rw-rw-   0        0        0     2106 2023-03-22 01:51:15.000000 carefree-learn-0.4.1/cflearn/api/cv/third_party/mlsd/api.py
-drwxrwxrwx   0        0        0        0 2023-04-05 06:44:20.827680 carefree-learn-0.4.1/cflearn/api/cv/third_party/mlsd/models/
--rw-rw-rw-   0        0        0        0 2023-03-22 01:51:15.000000 carefree-learn-0.4.1/cflearn/api/cv/third_party/mlsd/models/__init__.py
--rw-rw-rw-   0        0        0    10142 2023-03-22 01:51:15.000000 carefree-learn-0.4.1/cflearn/api/cv/third_party/mlsd/models/mbv2_mlsd_large.py
--rw-rw-rw-   0        0        0     9711 2023-03-22 01:51:15.000000 carefree-learn-0.4.1/cflearn/api/cv/third_party/mlsd/models/mbv2_mlsd_tiny.py
--rw-rw-rw-   0        0        0    26167 2023-03-22 01:51:15.000000 carefree-learn-0.4.1/cflearn/api/cv/third_party/mlsd/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-05 06:44:20.829673 carefree-learn-0.4.1/cflearn/api/cv/third_party/openpose/
--rw-rw-rw-   0        0        0       20 2023-03-22 01:51:15.000000 carefree-learn-0.4.1/cflearn/api/cv/third_party/openpose/__init__.py
--rw-rw-rw-   0        0        0     2392 2023-03-22 01:51:15.000000 carefree-learn-0.4.1/cflearn/api/cv/third_party/openpose/api.py
--rw-rw-rw-   0        0        0    14093 2023-03-22 01:51:15.000000 carefree-learn-0.4.1/cflearn/api/cv/third_party/openpose/body.py
--rw-rw-rw-   0        0        0     4271 2023-03-22 01:51:15.000000 carefree-learn-0.4.1/cflearn/api/cv/third_party/openpose/hand.py
--rw-rw-rw-   0        0        0     9090 2023-03-22 01:51:15.000000 carefree-learn-0.4.1/cflearn/api/cv/third_party/openpose/model.py
--rw-rw-rw-   0        0        0     8699 2023-03-22 01:51:15.000000 carefree-learn-0.4.1/cflearn/api/cv/third_party/openpose/util.py
--rw-rw-rw-   0        0        0     2053 2023-04-04 02:24:07.000000 carefree-learn-0.4.1/cflearn/api/cv/third_party/prompt.py
--rw-rw-rw-   0        0        0     2489 2023-03-23 09:35:16.000000 carefree-learn-0.4.1/cflearn/api/cv/translator.py
-drwxrwxrwx   0        0        0        0 2023-04-05 06:44:20.830669 carefree-learn-0.4.1/cflearn/api/ml/
--rw-rw-rw-   0        0        0       20 2023-03-23 05:48:39.000000 carefree-learn-0.4.1/cflearn/api/ml/__init__.py
--rw-rw-rw-   0        0        0     8678 2023-03-23 05:48:39.000000 carefree-learn-0.4.1/cflearn/api/ml/ddr.py
--rw-rw-rw-   0        0        0      524 2023-01-29 11:37:21.000000 carefree-learn-0.4.1/cflearn/api/schema.py
--rw-rw-rw-   0        0        0     5484 2023-04-04 06:12:57.000000 carefree-learn-0.4.1/cflearn/api/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-05 06:44:20.831667 carefree-learn-0.4.1/cflearn/api/zoo/
--rw-rw-rw-   0        0        0     6163 2023-03-29 08:24:36.000000 carefree-learn-0.4.1/cflearn/api/zoo/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-05 06:44:20.832663 carefree-learn-0.4.1/cflearn/callbacks/
--rw-rw-rw-   0        0        0       81 2023-03-23 05:48:39.000000 carefree-learn-0.4.1/cflearn/callbacks/__init__.py
--rw-rw-rw-   0        0        0     1118 2023-03-23 09:35:20.000000 carefree-learn-0.4.1/cflearn/callbacks/classification.py
--rw-rw-rw-   0        0        0     9649 2023-03-23 08:40:04.000000 carefree-learn-0.4.1/cflearn/callbacks/general.py
--rw-rw-rw-   0        0        0     4212 2023-03-23 09:35:26.000000 carefree-learn-0.4.1/cflearn/callbacks/generator.py
--rw-rw-rw-   0        0        0      656 2023-03-23 05:48:39.000000 carefree-learn-0.4.1/cflearn/constants.py
-drwxrwxrwx   0        0        0        0 2023-04-05 06:44:20.833660 carefree-learn-0.4.1/cflearn/data/
--rw-rw-rw-   0        0        0      247 2023-03-28 06:24:25.000000 carefree-learn-0.4.1/cflearn/data/__init__.py
--rw-rw-rw-   0        0        0     2798 2023-03-28 02:09:34.000000 carefree-learn-0.4.1/cflearn/data/array.py
-drwxrwxrwx   0        0        0        0 2023-04-05 06:44:20.834656 carefree-learn-0.4.1/cflearn/data/blocks/
--rw-rw-rw-   0        0        0       62 2023-03-23 05:48:39.000000 carefree-learn-0.4.1/cflearn/data/blocks/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-05 06:44:20.838644 carefree-learn-0.4.1/cflearn/data/blocks/cv/
--rw-rw-rw-   0        0        0      159 2023-03-29 09:56:34.000000 carefree-learn-0.4.1/cflearn/data/blocks/cv/__init__.py
--rw-rw-rw-   0        0        0     1447 2023-03-29 10:00:43.000000 carefree-learn-0.4.1/cflearn/data/blocks/cv/crop.py
--rw-rw-rw-   0        0        0      477 2023-03-23 05:48:39.000000 carefree-learn-0.4.1/cflearn/data/blocks/cv/hwc_to_chw.py
--rw-rw-rw-   0        0        0    31082 2023-03-29 07:34:59.000000 carefree-learn-0.4.1/cflearn/data/blocks/cv/image_folder.py
--rw-rw-rw-   0        0        0     2054 2023-03-29 07:34:59.000000 carefree-learn-0.4.1/cflearn/data/blocks/cv/normalize.py
--rw-rw-rw-   0        0        0     1002 2023-03-23 05:48:39.000000 carefree-learn-0.4.1/cflearn/data/blocks/cv/to_numpy.py
--rw-rw-rw-   0        0        0      609 2023-03-23 05:48:39.000000 carefree-learn-0.4.1/cflearn/data/blocks/cv/tuple_to_batch.py
--rw-rw-rw-   0        0        0      375 2023-03-23 05:48:39.000000 carefree-learn-0.4.1/cflearn/data/blocks/flatten.py
-drwxrwxrwx   0        0        0        0 2023-04-05 06:44:20.842630 carefree-learn-0.4.1/cflearn/data/blocks/ml/
--rw-rw-rw-   0        0        0      176 2023-03-23 05:48:39.000000 carefree-learn-0.4.1/cflearn/data/blocks/ml/__init__.py
--rw-rw-rw-   0        0        0    19260 2023-03-29 06:28:32.000000 carefree-learn-0.4.1/cflearn/data/blocks/ml/file.py
--rw-rw-rw-   0        0        0     1729 2023-03-29 06:29:22.000000 carefree-learn-0.4.1/cflearn/data/blocks/ml/gather.py
--rw-rw-rw-   0        0        0     7608 2023-03-29 06:29:31.000000 carefree-learn-0.4.1/cflearn/data/blocks/ml/nan_handler.py
--rw-rw-rw-   0        0        0     7327 2023-03-29 06:29:45.000000 carefree-learn-0.4.1/cflearn/data/blocks/ml/preprocessor.py
--rw-rw-rw-   0        0        0     6234 2023-03-29 06:30:03.000000 carefree-learn-0.4.1/cflearn/data/blocks/ml/recognizer.py
--rw-rw-rw-   0        0        0      416 2023-03-23 05:48:39.000000 carefree-learn-0.4.1/cflearn/data/blocks/ml/schema.py
--rw-rw-rw-   0        0        0    12175 2023-03-29 06:30:47.000000 carefree-learn-0.4.1/cflearn/data/blocks/ml/splitter.py
-drwxrwxrwx   0        0        0        0 2023-04-05 06:44:20.843627 carefree-learn-0.4.1/cflearn/data/ml/
--rw-rw-rw-   0        0        0       45 2023-03-23 05:48:39.000000 carefree-learn-0.4.1/cflearn/data/ml/__init__.py
--rw-rw-rw-   0        0        0     7741 2023-03-29 06:34:52.000000 carefree-learn-0.4.1/cflearn/data/ml/api.py
--rw-rw-rw-   0        0        0     1292 2023-03-23 05:48:39.000000 carefree-learn-0.4.1/cflearn/data/ml/datasets.py
-drwxrwxrwx   0        0        0        0 2023-04-05 06:44:20.845620 carefree-learn-0.4.1/cflearn/data/pytorch/
--rw-rw-rw-   0        0        0       45 2023-03-23 05:48:39.000000 carefree-learn-0.4.1/cflearn/data/pytorch/__init__.py
--rw-rw-rw-   0        0        0     8349 2023-03-27 12:47:27.000000 carefree-learn-0.4.1/cflearn/data/pytorch/api.py
--rw-rw-rw-   0        0        0     1406 2023-03-29 06:36:58.000000 carefree-learn-0.4.1/cflearn/data/pytorch/datasets.py
--rw-rw-rw-   0        0        0     7842 2023-03-28 02:09:41.000000 carefree-learn-0.4.1/cflearn/data/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-05 06:44:20.845620 carefree-learn-0.4.1/cflearn/dist/
--rw-rw-rw-   0        0        0       18 2022-10-23 14:55:07.000000 carefree-learn-0.4.1/cflearn/dist/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-05 06:44:20.847613 carefree-learn-0.4.1/cflearn/dist/ml/
--rw-rw-rw-   0        0        0      159 2022-10-23 14:55:07.000000 carefree-learn-0.4.1/cflearn/dist/ml/__init__.py
--rw-rw-rw-   0        0        0     8874 2023-03-23 05:48:39.000000 carefree-learn-0.4.1/cflearn/dist/ml/experiment.py
-drwxrwxrwx   0        0        0        0 2023-04-05 06:44:20.848610 carefree-learn-0.4.1/cflearn/dist/ml/runs/
--rw-rw-rw-   0        0        0        0 2022-10-23 14:55:07.000000 carefree-learn-0.4.1/cflearn/dist/ml/runs/__init__.py
--rw-rw-rw-   0        0        0     1320 2023-03-23 05:48:39.000000 carefree-learn-0.4.1/cflearn/dist/ml/runs/_utils.py
--rw-rw-rw-   0        0        0      291 2023-03-23 05:48:39.000000 carefree-learn-0.4.1/cflearn/dist/ml/runs/basic.py
--rw-rw-rw-   0        0        0     1709 2023-03-23 05:48:39.000000 carefree-learn-0.4.1/cflearn/dist/ml/task.py
--rw-rw-rw-   0        0        0     8910 2023-03-23 05:48:39.000000 carefree-learn-0.4.1/cflearn/inference.py
-drwxrwxrwx   0        0        0        0 2023-04-05 06:44:20.851600 carefree-learn-0.4.1/cflearn/losses/
--rw-rw-rw-   0        0        0       84 2022-10-23 14:55:07.000000 carefree-learn-0.4.1/cflearn/losses/__init__.py
--rw-rw-rw-   0        0        0     6391 2023-03-29 12:15:03.000000 carefree-learn-0.4.1/cflearn/losses/basic.py
--rw-rw-rw-   0        0        0     2546 2022-10-23 14:55:07.000000 carefree-learn-0.4.1/cflearn/losses/gan.py
--rw-rw-rw-   0        0        0     2812 2023-03-24 02:18:57.000000 carefree-learn-0.4.1/cflearn/losses/lpips.py
--rw-rw-rw-   0        0        0     3962 2023-03-23 05:48:39.000000 carefree-learn-0.4.1/cflearn/losses/vae.py
--rw-rw-rw-   0        0        0     5614 2023-03-23 05:48:39.000000 carefree-learn-0.4.1/cflearn/metrics.py
-drwxrwxrwx   0        0        0        0 2023-04-05 06:44:20.856584 carefree-learn-0.4.1/cflearn/misc/
--rw-rw-rw-   0        0        0        0 2023-02-14 02:22:11.000000 carefree-learn-0.4.1/cflearn/misc/__init__.py
--rw-rw-rw-   0        0        0    14696 2023-03-25 03:25:19.000000 carefree-learn-0.4.1/cflearn/misc/available.json
--rw-rw-rw-   0        0        0     1375 2023-03-23 05:48:39.000000 carefree-learn-0.4.1/cflearn/misc/mixins.py
--rw-rw-rw-   0        0        0    42403 2023-04-04 02:24:07.000000 carefree-learn-0.4.1/cflearn/misc/toolkit.py
-drwxrwxrwx   0        0        0        0 2023-04-05 06:44:20.857580 carefree-learn-0.4.1/cflearn/models/
--rw-rw-rw-   0        0        0       62 2023-03-23 05:48:39.000000 carefree-learn-0.4.1/cflearn/models/__init__.py
--rw-rw-rw-   0        0        0     5563 2023-01-29 11:37:21.000000 carefree-learn-0.4.1/cflearn/models/bases.py
-drwxrwxrwx   0        0        0        0 2023-04-05 06:44:20.858576 carefree-learn-0.4.1/cflearn/models/cv/
--rw-rw-rw-   0        0        0      167 2023-03-23 05:48:39.000000 carefree-learn-0.4.1/cflearn/models/cv/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-05 06:44:20.860570 carefree-learn-0.4.1/cflearn/models/cv/ae/
--rw-rw-rw-   0        0        0       38 2023-03-22 05:28:24.000000 carefree-learn-0.4.1/cflearn/models/cv/ae/__init__.py
--rw-rw-rw-   0        0        0    12091 2023-03-27 01:50:04.000000 carefree-learn-0.4.1/cflearn/models/cv/ae/common.py
--rw-rw-rw-   0        0        0     8409 2023-03-27 01:52:38.000000 carefree-learn-0.4.1/cflearn/models/cv/ae/kl.py
--rw-rw-rw-   0        0        0     7970 2023-03-27 01:52:49.000000 carefree-learn-0.4.1/cflearn/models/cv/ae/vq.py
-drwxrwxrwx   0        0        0        0 2023-04-05 06:44:20.863560 carefree-learn-0.4.1/cflearn/models/cv/classifier/
--rw-rw-rw-   0        0        0       24 2022-10-23 14:55:07.000000 carefree-learn-0.4.1/cflearn/models/cv/classifier/__init__.py
--rw-rw-rw-   0        0        0     4079 2023-01-29 11:37:21.000000 carefree-learn-0.4.1/cflearn/models/cv/classifier/vanilla.py
-drwxrwxrwx   0        0        0        0 2023-04-05 06:44:20.868548 carefree-learn-0.4.1/cflearn/models/cv/decoder/
--rw-rw-rw-   0        0        0      145 2023-01-29 11:37:21.000000 carefree-learn-0.4.1/cflearn/models/cv/decoder/__init__.py
--rw-rw-rw-   0        0        0     3619 2023-02-27 01:58:50.000000 carefree-learn-0.4.1/cflearn/models/cv/decoder/attn.py
--rw-rw-rw-   0        0        0     4162 2023-01-29 11:37:21.000000 carefree-learn-0.4.1/cflearn/models/cv/decoder/schema.py
--rw-rw-rw-   0        0        0     8739 2023-01-29 11:37:21.000000 carefree-learn-0.4.1/cflearn/models/cv/decoder/style_gan.py
--rw-rw-rw-   0        0        0    14508 2023-01-29 11:37:21.000000 carefree-learn-0.4.1/cflearn/models/cv/decoder/style_gan_v2.py
--rw-rw-rw-   0        0        0     9329 2023-01-29 11:37:21.000000 carefree-learn-0.4.1/cflearn/models/cv/decoder/vanilla.py
--rw-rw-rw-   0        0        0     3952 2023-01-29 11:37:21.000000 carefree-learn-0.4.1/cflearn/models/cv/decoder/vqgan.py
-drwxrwxrwx   0        0        0        0 2023-04-05 06:44:20.872535 carefree-learn-0.4.1/cflearn/models/cv/diffusion/
--rw-rw-rw-   0        0        0       87 2023-03-22 01:51:15.000000 carefree-learn-0.4.1/cflearn/models/cv/diffusion/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-05 06:44:20.874528 carefree-learn-0.4.1/cflearn/models/cv/diffusion/cond_models/
--rw-rw-rw-   0        0        0       69 2023-03-22 01:51:15.000000 carefree-learn-0.4.1/cflearn/models/cv/diffusion/cond_models/__init__.py
--rw-rw-rw-   0        0        0    10010 2023-03-23 05:48:39.000000 carefree-learn-0.4.1/cflearn/models/cv/diffusion/cond_models/clip.py
--rw-rw-rw-   0        0        0     1525 2023-03-24 02:19:09.000000 carefree-learn-0.4.1/cflearn/models/cv/diffusion/cond_models/rescaler.py
--rw-rw-rw-   0        0        0     1182 2023-03-23 05:48:39.000000 carefree-learn-0.4.1/cflearn/models/cv/diffusion/cond_models/schema.py
--rw-rw-rw-   0        0        0    29822 2023-04-04 03:36:26.000000 carefree-learn-0.4.1/cflearn/models/cv/diffusion/ddpm.py
--rw-rw-rw-   0        0        0    10395 2023-04-04 03:36:41.000000 carefree-learn-0.4.1/cflearn/models/cv/diffusion/ldm.py
-drwxrwxrwx   0        0        0        0 2023-04-05 06:44:20.878514 carefree-learn-0.4.1/cflearn/models/cv/diffusion/samplers/
--rw-rw-rw-   0        0        0      137 2023-03-22 01:51:15.000000 carefree-learn-0.4.1/cflearn/models/cv/diffusion/samplers/__init__.py
--rw-rw-rw-   0        0        0     2258 2023-03-22 01:51:15.000000 carefree-learn-0.4.1/cflearn/models/cv/diffusion/samplers/basic.py
--rw-rw-rw-   0        0        0     9817 2023-03-23 05:48:39.000000 carefree-learn-0.4.1/cflearn/models/cv/diffusion/samplers/ddim.py
--rw-rw-rw-   0        0        0    13157 2023-03-23 05:48:39.000000 carefree-learn-0.4.1/cflearn/models/cv/diffusion/samplers/k_samplers.py
--rw-rw-rw-   0        0        0     2593 2023-03-22 01:51:15.000000 carefree-learn-0.4.1/cflearn/models/cv/diffusion/samplers/plms.py
--rw-rw-rw-   0        0        0     7507 2023-03-29 11:33:58.000000 carefree-learn-0.4.1/cflearn/models/cv/diffusion/samplers/schema.py
--rw-rw-rw-   0        0        0    16613 2023-03-23 05:48:39.000000 carefree-learn-0.4.1/cflearn/models/cv/diffusion/samplers/solver.py
--rw-rw-rw-   0        0        0     2561 2023-03-22 01:51:15.000000 carefree-learn-0.4.1/cflearn/models/cv/diffusion/samplers/utils.py
--rw-rw-rw-   0        0        0    20269 2023-04-05 02:04:44.000000 carefree-learn-0.4.1/cflearn/models/cv/diffusion/unet.py
--rw-rw-rw-   0        0        0      737 2023-03-22 01:51:15.000000 carefree-learn-0.4.1/cflearn/models/cv/diffusion/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-05 06:44:20.883530 carefree-learn-0.4.1/cflearn/models/cv/encoder/
--rw-rw-rw-   0        0        0      240 2023-01-29 11:37:21.000000 carefree-learn-0.4.1/cflearn/models/cv/encoder/__init__.py
--rw-rw-rw-   0        0        0     3369 2023-02-27 01:58:50.000000 carefree-learn-0.4.1/cflearn/models/cv/encoder/attn.py
-drwxrwxrwx   0        0        0        0 2023-04-05 06:44:20.885523 carefree-learn-0.4.1/cflearn/models/cv/encoder/backbone/
--rw-rw-rw-   0        0        0       64 2022-10-23 14:55:07.000000 carefree-learn-0.4.1/cflearn/models/cv/encoder/backbone/__init__.py
--rw-rw-rw-   0        0        0     3109 2023-01-29 11:37:21.000000 carefree-learn-0.4.1/cflearn/models/cv/encoder/backbone/api.py
--rw-rw-rw-   0        0        0     4242 2022-10-23 14:55:07.000000 carefree-learn-0.4.1/cflearn/models/cv/encoder/backbone/core.py
-drwxrwxrwx   0        0        0        0 2023-04-05 06:44:20.887517 carefree-learn-0.4.1/cflearn/models/cv/encoder/backbone/models/
--rw-rw-rw-   0        0        0       97 2022-10-23 14:55:07.000000 carefree-learn-0.4.1/cflearn/models/cv/encoder/backbone/models/__init__.py
--rw-rw-rw-   0        0        0      430 2022-10-23 14:55:07.000000 carefree-learn-0.4.1/cflearn/models/cv/encoder/backbone/models/mobilenet.py
--rw-rw-rw-   0        0        0     1225 2022-10-23 14:55:07.000000 carefree-learn-0.4.1/cflearn/models/cv/encoder/backbone/models/resnet.py
--rw-rw-rw-   0        0        0     5392 2023-02-10 05:26:29.000000 carefree-learn-0.4.1/cflearn/models/cv/encoder/backbone/models/transformer.py
--rw-rw-rw-   0        0        0    13725 2022-10-23 14:55:07.000000 carefree-learn-0.4.1/cflearn/models/cv/encoder/backbone/models/vgg.py
--rw-rw-rw-   0        0        0      968 2022-10-23 14:55:07.000000 carefree-learn-0.4.1/cflearn/models/cv/encoder/backbone/register.py
--rw-rw-rw-   0        0        0     1133 2023-02-10 03:39:20.000000 carefree-learn-0.4.1/cflearn/models/cv/encoder/fnet.py
--rw-rw-rw-   0        0        0     1132 2023-02-10 03:39:20.000000 carefree-learn-0.4.1/cflearn/models/cv/encoder/mixer.py
--rw-rw-rw-   0        0        0     2336 2023-01-29 11:37:21.000000 carefree-learn-0.4.1/cflearn/models/cv/encoder/perceiver.py
--rw-rw-rw-   0        0        0     1149 2023-02-10 03:39:20.000000 carefree-learn-0.4.1/cflearn/models/cv/encoder/pool_former.py
--rw-rw-rw-   0        0        0     5124 2023-03-23 05:48:39.000000 carefree-learn-0.4.1/cflearn/models/cv/encoder/schema.py
--rw-rw-rw-   0        0        0     6125 2023-03-22 07:19:34.000000 carefree-learn-0.4.1/cflearn/models/cv/encoder/transformer.py
--rw-rw-rw-   0        0        0     5535 2023-01-29 11:37:21.000000 carefree-learn-0.4.1/cflearn/models/cv/encoder/vanilla.py
--rw-rw-rw-   0        0        0     5473 2023-01-29 11:37:21.000000 carefree-learn-0.4.1/cflearn/models/cv/encoder/vqgan.py
-drwxrwxrwx   0        0        0        0 2023-04-05 06:44:20.889510 carefree-learn-0.4.1/cflearn/models/cv/gan/
--rw-rw-rw-   0        0        0       55 2023-03-23 05:48:39.000000 carefree-learn-0.4.1/cflearn/models/cv/gan/__init__.py
--rw-rw-rw-   0        0        0     5920 2022-10-23 14:55:07.000000 carefree-learn-0.4.1/cflearn/models/cv/gan/discriminators.py
--rw-rw-rw-   0        0        0     7730 2023-03-29 11:05:45.000000 carefree-learn-0.4.1/cflearn/models/cv/gan/schema.py
--rw-rw-rw-   0        0        0     1913 2023-03-23 05:48:39.000000 carefree-learn-0.4.1/cflearn/models/cv/gan/vanilla.py
--rw-rw-rw-   0        0        0     6731 2023-03-23 05:48:39.000000 carefree-learn-0.4.1/cflearn/models/cv/general.py
-drwxrwxrwx   0        0        0        0 2023-04-05 06:44:20.890507 carefree-learn-0.4.1/cflearn/models/cv/translator/
--rw-rw-rw-   0        0        0       21 2023-03-22 01:51:15.000000 carefree-learn-0.4.1/cflearn/models/cv/translator/__init__.py
--rw-rw-rw-   0        0        0     4018 2023-03-23 05:48:39.000000 carefree-learn-0.4.1/cflearn/models/cv/translator/rrdb.py
-drwxrwxrwx   0        0        0        0 2023-04-05 06:44:20.891503 carefree-learn-0.4.1/cflearn/models/implicit/
--rw-rw-rw-   0        0        0       22 2022-10-23 14:55:07.000000 carefree-learn-0.4.1/cflearn/models/implicit/__init__.py
--rw-rw-rw-   0        0        0     7927 2022-10-23 14:55:07.000000 carefree-learn-0.4.1/cflearn/models/implicit/siren.py
-drwxrwxrwx   0        0        0        0 2023-04-05 06:44:20.895490 carefree-learn-0.4.1/cflearn/models/ml/
--rw-rw-rw-   0        0        0      165 2023-03-23 05:48:39.000000 carefree-learn-0.4.1/cflearn/models/ml/__init__.py
--rw-rw-rw-   0        0        0     1857 2023-03-23 05:48:39.000000 carefree-learn-0.4.1/cflearn/models/ml/base.py
--rw-rw-rw-   0        0        0    11624 2023-03-29 12:15:02.000000 carefree-learn-0.4.1/cflearn/models/ml/ddr.py
--rw-rw-rw-   0        0        0     8958 2023-03-28 02:09:49.000000 carefree-learn-0.4.1/cflearn/models/ml/encoders.py
--rw-rw-rw-   0        0        0     2392 2023-03-23 05:48:39.000000 carefree-learn-0.4.1/cflearn/models/ml/fcnn.py
--rw-rw-rw-   0        0        0     1100 2023-03-23 05:48:39.000000 carefree-learn-0.4.1/cflearn/models/ml/linear.py
--rw-rw-rw-   0        0        0     6980 2023-03-23 05:48:39.000000 carefree-learn-0.4.1/cflearn/models/ml/mixed_stacked.py
--rw-rw-rw-   0        0        0     7976 2023-03-23 05:48:39.000000 carefree-learn-0.4.1/cflearn/models/ml/nbm.py
--rw-rw-rw-   0        0        0     5272 2023-03-23 05:48:39.000000 carefree-learn-0.4.1/cflearn/models/ml/ndt.py
--rw-rw-rw-   0        0        0     3068 2023-03-23 05:48:39.000000 carefree-learn-0.4.1/cflearn/models/ml/rnn.py
--rw-rw-rw-   0        0        0     2798 2023-03-23 05:48:39.000000 carefree-learn-0.4.1/cflearn/models/ml/wnd.py
-drwxrwxrwx   0        0        0        0 2023-04-05 06:44:20.897482 carefree-learn-0.4.1/cflearn/models/multimodal/
--rw-rw-rw-   0        0        0       21 2023-03-23 05:48:39.000000 carefree-learn-0.4.1/cflearn/models/multimodal/__init__.py
--rw-rw-rw-   0        0        0    10260 2023-03-23 08:58:17.000000 carefree-learn-0.4.1/cflearn/models/multimodal/clip.py
--rw-rw-rw-   0        0        0       19 2023-03-22 01:51:15.000000 carefree-learn-0.4.1/cflearn/models/multimodal/constants.py
--rw-rw-rw-   0        0        0     1554 2023-03-29 11:05:45.000000 carefree-learn-0.4.1/cflearn/models/multimodal/schema.py
-drwxrwxrwx   0        0        0        0 2023-04-05 06:44:20.898480 carefree-learn-0.4.1/cflearn/models/nlp/
--rw-rw-rw-   0        0        0       80 2023-03-22 01:51:15.000000 carefree-learn-0.4.1/cflearn/models/nlp/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-05 06:44:20.899477 carefree-learn-0.4.1/cflearn/models/nlp/encoder/
--rw-rw-rw-   0        0        0       28 2023-03-22 01:51:15.000000 carefree-learn-0.4.1/cflearn/models/nlp/encoder/__init__.py
--rw-rw-rw-   0        0        0       19 2023-03-22 01:51:15.000000 carefree-learn-0.4.1/cflearn/models/nlp/encoder/constants.py
--rw-rw-rw-   0        0        0     3694 2023-03-22 01:51:15.000000 carefree-learn-0.4.1/cflearn/models/nlp/encoder/transformer.py
-drwxrwxrwx   0        0        0        0 2023-04-05 06:44:20.900473 carefree-learn-0.4.1/cflearn/models/nlp/tokenizers/
--rw-rw-rw-   0        0        0       44 2023-03-22 01:51:15.000000 carefree-learn-0.4.1/cflearn/models/nlp/tokenizers/__init__.py
--rw-rw-rw-   0        0        0     2371 2023-03-23 05:48:39.000000 carefree-learn-0.4.1/cflearn/models/nlp/tokenizers/clip.py
--rw-rw-rw-   0        0        0     1226 2023-03-22 01:51:15.000000 carefree-learn-0.4.1/cflearn/models/nlp/tokenizers/schema.py
-drwxrwxrwx   0        0        0        0 2023-04-05 06:44:20.902466 carefree-learn-0.4.1/cflearn/models/nlp/transformers/
--rw-rw-rw-   0        0        0       66 2023-03-22 01:51:15.000000 carefree-learn-0.4.1/cflearn/models/nlp/transformers/__init__.py
--rw-rw-rw-   0        0        0     3547 2023-03-27 13:58:44.000000 carefree-learn-0.4.1/cflearn/models/nlp/transformers/core.py
--rw-rw-rw-   0        0        0     1575 2023-03-22 01:51:15.000000 carefree-learn-0.4.1/cflearn/models/nlp/transformers/opus.py
--rw-rw-rw-   0        0        0      813 2023-03-22 01:51:15.000000 carefree-learn-0.4.1/cflearn/models/nlp/transformers/simbert.py
-drwxrwxrwx   0        0        0        0 2023-04-05 06:44:20.904461 carefree-learn-0.4.1/cflearn/models/schemas/
--rw-rw-rw-   0        0        0       42 2023-03-27 01:49:17.000000 carefree-learn-0.4.1/cflearn/models/schemas/__init__.py
--rw-rw-rw-   0        0        0    12838 2023-04-04 02:24:07.000000 carefree-learn-0.4.1/cflearn/models/schemas/custom.py
--rw-rw-rw-   0        0        0     4631 2023-03-23 05:48:39.000000 carefree-learn-0.4.1/cflearn/models/schemas/cv.py
-drwxrwxrwx   0        0        0        0 2023-04-05 06:44:20.905456 carefree-learn-0.4.1/cflearn/modules/
--rw-rw-rw-   0        0        0       54 2022-10-23 14:55:07.000000 carefree-learn-0.4.1/cflearn/modules/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-05 06:44:20.910440 carefree-learn-0.4.1/cflearn/modules/blocks/
--rw-rw-rw-   0        0        0      756 2023-03-24 08:39:05.000000 carefree-learn-0.4.1/cflearn/modules/blocks/__init__.py
--rw-rw-rw-   0        0        0     5165 2023-03-24 02:18:16.000000 carefree-learn-0.4.1/cflearn/modules/blocks/activations.py
--rw-rw-rw-   0        0        0    21921 2023-04-04 03:38:07.000000 carefree-learn-0.4.1/cflearn/modules/blocks/attentions.py
--rw-rw-rw-   0        0        0     6448 2022-11-09 12:05:57.000000 carefree-learn-0.4.1/cflearn/modules/blocks/common.py
-drwxrwxrwx   0        0        0        0 2023-04-05 06:44:20.911436 carefree-learn-0.4.1/cflearn/modules/blocks/convs/
--rw-rw-rw-   0        0        0       47 2022-10-23 14:55:07.000000 carefree-learn-0.4.1/cflearn/modules/blocks/convs/__init__.py
--rw-rw-rw-   0        0        0    19321 2023-03-24 02:29:08.000000 carefree-learn-0.4.1/cflearn/modules/blocks/convs/basic.py
--rw-rw-rw-   0        0        0     8836 2023-03-24 02:19:26.000000 carefree-learn-0.4.1/cflearn/modules/blocks/convs/residual.py
--rw-rw-rw-   0        0        0    18713 2023-03-25 03:37:31.000000 carefree-learn-0.4.1/cflearn/modules/blocks/customs.py
--rw-rw-rw-   0        0        0     8503 2023-03-23 05:48:39.000000 carefree-learn-0.4.1/cflearn/modules/blocks/high_level.py
--rw-rw-rw-   0        0        0    11952 2023-03-26 04:55:02.000000 carefree-learn-0.4.1/cflearn/modules/blocks/hijacks.py
--rw-rw-rw-   0        0        0      945 2023-03-25 03:55:38.000000 carefree-learn-0.4.1/cflearn/modules/blocks/hooks.py
-drwxrwxrwx   0        0        0        0 2023-04-05 06:44:20.912433 carefree-learn-0.4.1/cflearn/modules/blocks/implementations/
--rw-rw-rw-   0        0        0       26 2022-10-23 14:55:07.000000 carefree-learn-0.4.1/cflearn/modules/blocks/implementations/__init__.py
--rw-rw-rw-   0        0        0     4708 2022-10-23 14:55:07.000000 carefree-learn-0.4.1/cflearn/modules/blocks/implementations/perceiver.py
--rw-rw-rw-   0        0        0     6189 2023-01-29 11:37:21.000000 carefree-learn-0.4.1/cflearn/modules/blocks/mappings.py
-drwxrwxrwx   0        0        0        0 2023-04-05 06:44:20.915423 carefree-learn-0.4.1/cflearn/modules/blocks/mixed_stacks/
--rw-rw-rw-   0        0        0      127 2023-02-10 03:31:37.000000 carefree-learn-0.4.1/cflearn/modules/blocks/mixed_stacks/__init__.py
--rw-rw-rw-   0        0        0    28432 2023-04-05 02:26:17.000000 carefree-learn-0.4.1/cflearn/modules/blocks/mixed_stacks/api.py
--rw-rw-rw-   0        0        0     3774 2023-03-24 08:39:41.000000 carefree-learn-0.4.1/cflearn/modules/blocks/mixed_stacks/channel_mixers.py
--rw-rw-rw-   0        0        0     1179 2022-10-23 14:55:07.000000 carefree-learn-0.4.1/cflearn/modules/blocks/mixed_stacks/poolers.py
--rw-rw-rw-   0        0        0     1325 2023-02-10 05:18:20.000000 carefree-learn-0.4.1/cflearn/modules/blocks/mixed_stacks/schema.py
--rw-rw-rw-   0        0        0     6998 2023-02-10 10:31:50.000000 carefree-learn-0.4.1/cflearn/modules/blocks/mixed_stacks/token_mixers.py
--rw-rw-rw-   0        0        0     4682 2022-10-23 14:55:07.000000 carefree-learn-0.4.1/cflearn/modules/blocks/norms.py
--rw-rw-rw-   0        0        0      863 2023-02-27 01:58:50.000000 carefree-learn-0.4.1/cflearn/modules/blocks/utils.py
--rw-rw-rw-   0        0        0     4751 2022-10-23 14:55:07.000000 carefree-learn-0.4.1/cflearn/modules/optimizers.py
--rw-rw-rw-   0        0        0     9159 2022-11-09 12:09:28.000000 carefree-learn-0.4.1/cflearn/modules/schedulers.py
--rw-rw-rw-   0        0        0     4774 2023-03-23 05:48:39.000000 carefree-learn-0.4.1/cflearn/monitors.py
--rw-rw-rw-   0        0        0      634 2023-02-16 10:09:59.000000 carefree-learn-0.4.1/cflearn/parameters.py
-drwxrwxrwx   0        0        0        0 2023-04-05 06:44:20.917416 carefree-learn-0.4.1/cflearn/pipeline/
--rw-rw-rw-   0        0        0       92 2023-03-23 05:48:39.000000 carefree-learn-0.4.1/cflearn/pipeline/__init__.py
--rw-rw-rw-   0        0        0    23551 2023-03-29 11:32:53.000000 carefree-learn-0.4.1/cflearn/pipeline/api.py
-drwxrwxrwx   0        0        0        0 2023-04-05 06:44:20.920407 carefree-learn-0.4.1/cflearn/pipeline/blocks/
--rw-rw-rw-   0        0        0       41 2023-03-23 05:48:39.000000 carefree-learn-0.4.1/cflearn/pipeline/blocks/__init__.py
--rw-rw-rw-   0        0        0    36043 2023-03-27 01:51:03.000000 carefree-learn-0.4.1/cflearn/pipeline/blocks/basic.py
--rw-rw-rw-   0        0        0     2735 2023-03-23 05:48:39.000000 carefree-learn-0.4.1/cflearn/pipeline/blocks/ml.py
--rw-rw-rw-   0        0        0     1335 2023-03-23 05:48:39.000000 carefree-learn-0.4.1/cflearn/pipeline/blocks/utils.py
--rw-rw-rw-   0        0        0     3921 2023-03-23 08:46:39.000000 carefree-learn-0.4.1/cflearn/pipeline/core.py
--rw-rw-rw-   0        0        0      310 2023-03-23 05:48:39.000000 carefree-learn-0.4.1/cflearn/pipeline/schema.py
--rw-rw-rw-   0        0        0     1545 2023-03-23 05:48:39.000000 carefree-learn-0.4.1/cflearn/pipeline/third_party.py
--rw-rw-rw-   0        0        0      510 2023-03-23 05:48:39.000000 carefree-learn-0.4.1/cflearn/register.py
--rw-rw-rw-   0        0        0    60784 2023-03-29 15:41:28.000000 carefree-learn-0.4.1/cflearn/schema.py
-drwxrwxrwx   0        0        0        0 2023-04-05 06:44:20.921404 carefree-learn-0.4.1/cflearn/scripts/
--rw-rw-rw-   0        0        0       18 2023-03-24 10:59:16.000000 carefree-learn-0.4.1/cflearn/scripts/__init__.py
--rw-rw-rw-   0        0        0    12752 2023-04-04 02:24:07.000000 carefree-learn-0.4.1/cflearn/scripts/sd.py
--rw-rw-rw-   0        0        0    28526 2023-04-04 02:24:07.000000 carefree-learn-0.4.1/cflearn/trainer.py
--rw-rw-rw-   0        0        0     1053 2023-03-23 05:48:39.000000 carefree-learn-0.4.1/cflearn/types.py
-drwxrwxrwx   0        0        0        0 2023-04-05 06:44:20.923397 carefree-learn-0.4.1/cflearn/zoo/
--rw-rw-rw-   0        0        0       21 2023-03-22 01:51:15.000000 carefree-learn-0.4.1/cflearn/zoo/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-05 06:44:20.768359 carefree-learn-0.4.1/cflearn/zoo/configs/
-drwxrwxrwx   0        0        0        0 2023-04-05 06:44:20.767362 carefree-learn-0.4.1/cflearn/zoo/configs/ae/
-drwxrwxrwx   0        0        0        0 2023-04-05 06:44:20.940848 carefree-learn-0.4.1/cflearn/zoo/configs/ae/kl/
--rw-rw-rw-   0        0        0      201 2023-03-22 01:51:15.000000 carefree-learn-0.4.1/cflearn/zoo/configs/ae/kl/f16.json
--rw-rw-rw-   0        0        0      868 2023-03-23 05:48:39.000000 carefree-learn-0.4.1/cflearn/zoo/configs/ae/kl/f4.json
--rw-rw-rw-   0        0        0      160 2023-03-22 01:51:15.000000 carefree-learn-0.4.1/cflearn/zoo/configs/ae/kl/f8.json
-drwxrwxrwx   0        0        0        0 2023-04-05 06:44:20.954802 carefree-learn-0.4.1/cflearn/zoo/configs/ae/vq/
--rw-rw-rw-   0        0        0      205 2023-03-22 01:51:15.000000 carefree-learn-0.4.1/cflearn/zoo/configs/ae/vq/f4.json
--rw-rw-rw-   0        0        0       92 2023-03-22 01:51:15.000000 carefree-learn-0.4.1/cflearn/zoo/configs/ae/vq/f4_no_attn.json
--rw-rw-rw-   0        0        0      295 2023-03-22 01:51:15.000000 carefree-learn-0.4.1/cflearn/zoo/configs/ae/vq/f8.json
-drwxrwxrwx   0        0        0        0 2023-04-05 06:44:20.767362 carefree-learn-0.4.1/cflearn/zoo/configs/diffusion/
-drwxrwxrwx   0        0        0        0 2023-04-05 06:44:20.957795 carefree-learn-0.4.1/cflearn/zoo/configs/diffusion/ddpm/
--rw-rw-rw-   0        0        0     1155 2023-03-23 05:48:39.000000 carefree-learn-0.4.1/cflearn/zoo/configs/diffusion/ddpm/default.json
-drwxrwxrwx   0        0        0        0 2023-04-05 06:44:20.984232 carefree-learn-0.4.1/cflearn/zoo/configs/diffusion/ldm/
--rw-rw-rw-   0        0        0      513 2023-03-22 01:51:15.000000 carefree-learn-0.4.1/cflearn/zoo/configs/diffusion/ldm/default.json
--rw-rw-rw-   0        0        0      451 2023-04-04 04:59:57.000000 carefree-learn-0.4.1/cflearn/zoo/configs/diffusion/ldm/sd.json
--rw-rw-rw-   0        0        0      125 2023-03-22 01:51:15.000000 carefree-learn-0.4.1/cflearn/zoo/configs/diffusion/ldm/sd_inpainting.json
--rw-rw-rw-   0        0        0      344 2023-03-22 01:51:15.000000 carefree-learn-0.4.1/cflearn/zoo/configs/diffusion/ldm/sd_v2.json
--rw-rw-rw-   0        0        0      104 2023-03-22 01:51:15.000000 carefree-learn-0.4.1/cflearn/zoo/configs/diffusion/ldm/sd_v2_base.json
--rw-rw-rw-   0        0        0      600 2023-03-23 05:48:39.000000 carefree-learn-0.4.1/cflearn/zoo/configs/diffusion/ldm/vq.json
-drwxrwxrwx   0        0        0        0 2023-04-05 06:44:20.768359 carefree-learn-0.4.1/cflearn/zoo/configs/multimodal/
-drwxrwxrwx   0        0        0        0 2023-04-05 06:44:21.003166 carefree-learn-0.4.1/cflearn/zoo/configs/multimodal/clip/
--rw-rw-rw-   0        0        0      525 2023-03-22 01:51:15.000000 carefree-learn-0.4.1/cflearn/zoo/configs/multimodal/clip/chinese.json
--rw-rw-rw-   0        0        0       79 2023-03-23 05:48:39.000000 carefree-learn-0.4.1/cflearn/zoo/configs/multimodal/clip/default.json
--rw-rw-rw-   0        0        0      269 2023-03-22 01:51:15.000000 carefree-learn-0.4.1/cflearn/zoo/configs/multimodal/clip/large.json
--rw-rw-rw-   0        0        0      389 2023-03-22 01:51:15.000000 carefree-learn-0.4.1/cflearn/zoo/configs/multimodal/clip/open_clip_ViT_H_14.json
-drwxrwxrwx   0        0        0        0 2023-04-05 06:44:20.768359 carefree-learn-0.4.1/cflearn/zoo/configs/sr/
-drwxrwxrwx   0        0        0        0 2023-04-05 06:44:21.008156 carefree-learn-0.4.1/cflearn/zoo/configs/sr/esr/
--rw-rw-rw-   0        0        0       81 2023-03-22 01:51:15.000000 carefree-learn-0.4.1/cflearn/zoo/configs/sr/esr/anime.json
--rw-rw-rw-   0        0        0       79 2023-03-23 05:48:39.000000 carefree-learn-0.4.1/cflearn/zoo/configs/sr/esr/default.json
--rw-rw-rw-   0        0        0     7814 2023-03-29 11:34:44.000000 carefree-learn-0.4.1/cflearn/zoo/core.py
-drwxrwxrwx   0        0        0        0 2023-04-05 06:44:21.010144 carefree-learn-0.4.1/cflearn/zoo/models/
--rw-rw-rw-   0        0        0       44 2023-03-22 01:51:15.000000 carefree-learn-0.4.1/cflearn/zoo/models/__init__.py
--rw-rw-rw-   0        0        0     1606 2023-03-23 05:48:39.000000 carefree-learn-0.4.1/cflearn/zoo/models/clip.py
--rw-rw-rw-   0        0        0      506 2023-03-22 01:51:15.000000 carefree-learn-0.4.1/cflearn/zoo/models/schema.py
--rw-rw-rw-   0        0        0      383 2023-04-05 06:44:21.011140 carefree-learn-0.4.1/setup.cfg
--rw-rw-rw-   0        0        0     1702 2023-04-05 06:39:50.000000 carefree-learn-0.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.365221 carefree-learn-0.4.2/
+-rw-rw-rw-   0        0        0     1090 2022-10-23 14:55:07.000000 carefree-learn-0.4.2/LICENSE
+-rw-rw-rw-   0        0        0       75 2022-11-10 07:33:05.000000 carefree-learn-0.4.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     7575 2023-05-06 05:29:58.365221 carefree-learn-0.4.2/PKG-INFO
+-rw-rw-rw-   0        0        0     7038 2023-04-04 02:24:07.000000 carefree-learn-0.4.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.240707 carefree-learn-0.4.2/carefree_learn.egg-info/
+-rw-rw-rw-   0        0        0     7575 2023-05-06 05:29:58.000000 carefree-learn-0.4.2/carefree_learn.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    10736 2023-05-06 05:29:58.000000 carefree-learn-0.4.2/carefree_learn.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 05:29:58.000000 carefree-learn-0.4.2/carefree_learn.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      601 2023-05-06 05:29:58.000000 carefree-learn-0.4.2/carefree_learn.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-06 05:29:58.000000 carefree-learn-0.4.2/carefree_learn.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.244708 carefree-learn-0.4.2/cflearn/
+-rw-rw-rw-   0        0        0      658 2023-04-04 02:24:07.000000 carefree-learn-0.4.2/cflearn/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.246707 carefree-learn-0.4.2/cflearn/api/
+-rw-rw-rw-   0        0        0        0 2022-10-23 14:55:07.000000 carefree-learn-0.4.2/cflearn/api/__init__.py
+-rw-rw-rw-   0        0        0    24147 2023-03-27 06:18:09.000000 carefree-learn-0.4.2/cflearn/api/api.py
+drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.247707 carefree-learn-0.4.2/cflearn/api/cv/
+-rw-rw-rw-   0        0        0       81 2023-03-23 05:48:39.000000 carefree-learn-0.4.2/cflearn/api/cv/__init__.py
+-rw-rw-rw-   0        0        0    58260 2023-04-20 12:00:25.000000 carefree-learn-0.4.2/cflearn/api/cv/diffusion.py
+drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.249709 carefree-learn-0.4.2/cflearn/api/cv/third_party/
+-rw-rw-rw-   0        0        0      156 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/api/cv/third_party/__init__.py
+-rw-rw-rw-   0        0        0     1069 2023-04-04 02:24:07.000000 carefree-learn-0.4.2/cflearn/api/cv/third_party/blip.py
+drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.250708 carefree-learn-0.4.2/cflearn/api/cv/third_party/iharm/
+-rw-rw-rw-   0        0        0       20 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/api/cv/third_party/iharm/__init__.py
+-rw-rw-rw-   0        0        0     1386 2023-04-04 02:24:07.000000 carefree-learn-0.4.2/cflearn/api/cv/third_party/iharm/api.py
+drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.252708 carefree-learn-0.4.2/cflearn/api/cv/third_party/iharm/inference/
+-rw-rw-rw-   0        0        0        0 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/api/cv/third_party/iharm/inference/__init__.py
+-rw-rw-rw-   0        0        0     1989 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/api/cv/third_party/iharm/inference/predictor.py
+-rw-rw-rw-   0        0        0     4395 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/api/cv/third_party/iharm/inference/transforms.py
+-rw-rw-rw-   0        0        0      341 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/api/cv/third_party/iharm/inference/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.253707 carefree-learn-0.4.2/cflearn/api/cv/third_party/iharm/mconfigs/
+-rw-rw-rw-   0        0        0      112 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/api/cv/third_party/iharm/mconfigs/__init__.py
+-rw-rw-rw-   0        0        0     1660 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/api/cv/third_party/iharm/mconfigs/backboned.py
+-rw-rw-rw-   0        0        0     1953 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/api/cv/third_party/iharm/mconfigs/base.py
+drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.254708 carefree-learn-0.4.2/cflearn/api/cv/third_party/iharm/model/
+-rw-rw-rw-   0        0        0        0 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/api/cv/third_party/iharm/model/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.256708 carefree-learn-0.4.2/cflearn/api/cv/third_party/iharm/model/backboned/
+-rw-rw-rw-   0        0        0       70 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/api/cv/third_party/iharm/model/backboned/__init__.py
+-rw-rw-rw-   0        0        0     4553 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/api/cv/third_party/iharm/model/backboned/deeplab.py
+-rw-rw-rw-   0        0        0     6090 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/api/cv/third_party/iharm/model/backboned/hrnet.py
+-rw-rw-rw-   0        0        0     3629 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/api/cv/third_party/iharm/model/backboned/ih_model.py
+drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.258708 carefree-learn-0.4.2/cflearn/api/cv/third_party/iharm/model/base/
+-rw-rw-rw-   0        0        0      130 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/api/cv/third_party/iharm/model/base/__init__.py
+-rw-rw-rw-   0        0        0     1236 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/api/cv/third_party/iharm/model/base/dih_model.py
+-rw-rw-rw-   0        0        0     1353 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/api/cv/third_party/iharm/model/base/iseunet_v1.py
+-rw-rw-rw-   0        0        0     3162 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/api/cv/third_party/iharm/model/base/ssam_model.py
+drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.262708 carefree-learn-0.4.2/cflearn/api/cv/third_party/iharm/model/modeling/
+-rw-rw-rw-   0        0        0        0 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/api/cv/third_party/iharm/model/modeling/__init__.py
+-rw-rw-rw-   0        0        0     8010 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/api/cv/third_party/iharm/model/modeling/basic_blocks.py
+-rw-rw-rw-   0        0        0     5571 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/api/cv/third_party/iharm/model/modeling/conv_autoencoder.py
+-rw-rw-rw-   0        0        0     7150 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/api/cv/third_party/iharm/model/modeling/deeplab_v3.py
+-rw-rw-rw-   0        0        0    19814 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/api/cv/third_party/iharm/model/modeling/hrnet_ocr.py
+-rw-rw-rw-   0        0        0     6392 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/api/cv/third_party/iharm/model/modeling/ocr.py
+-rw-rw-rw-   0        0        0     1808 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/api/cv/third_party/iharm/model/modeling/resnet.py
+-rw-rw-rw-   0        0        0    13493 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/api/cv/third_party/iharm/model/modeling/resnetv1b.py
+-rw-rw-rw-   0        0        0     8229 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/api/cv/third_party/iharm/model/modeling/unet.py
+-rw-rw-rw-   0        0        0      357 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/api/cv/third_party/iharm/model/modifiers.py
+-rw-rw-rw-   0        0        0     4927 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/api/cv/third_party/iharm/model/ops.py
+drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.263707 carefree-learn-0.4.2/cflearn/api/cv/third_party/iharm/utils/
+-rw-rw-rw-   0        0        0        0 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/api/cv/third_party/iharm/utils/__init__.py
+-rw-rw-rw-   0        0        0      445 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/api/cv/third_party/iharm/utils/misc.py
+-rw-rw-rw-   0        0        0    16017 2023-04-04 02:24:07.000000 carefree-learn-0.4.2/cflearn/api/cv/third_party/isnet.py
+-rw-rw-rw-   0        0        0     9132 2023-04-04 02:24:07.000000 carefree-learn-0.4.2/cflearn/api/cv/third_party/lama.py
+drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.265708 carefree-learn-0.4.2/cflearn/api/cv/third_party/midas/
+-rw-rw-rw-   0        0        0       20 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/api/cv/third_party/midas/__init__.py
+-rw-rw-rw-   0        0        0     8006 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/api/cv/third_party/midas/api.py
+drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.269708 carefree-learn-0.4.2/cflearn/api/cv/third_party/midas/core/
+-rw-rw-rw-   0        0        0        0 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/api/cv/third_party/midas/core/__init__.py
+-rw-rw-rw-   0        0        0      383 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/api/cv/third_party/midas/core/base_model.py
+-rw-rw-rw-   0        0        0    10222 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/api/cv/third_party/midas/core/blocks.py
+-rw-rw-rw-   0        0        0     3259 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/api/cv/third_party/midas/core/dpt_depth.py
+-rw-rw-rw-   0        0        0     2803 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/api/cv/third_party/midas/core/midas_net.py
+-rw-rw-rw-   0        0        0     6071 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/api/cv/third_party/midas/core/midas_net_custom.py
+-rw-rw-rw-   0        0        0     8096 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/api/cv/third_party/midas/core/transforms.py
+-rw-rw-rw-   0        0        0    15154 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/api/cv/third_party/midas/core/vit.py
+-rw-rw-rw-   0        0        0     4814 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/api/cv/third_party/midas/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.270708 carefree-learn-0.4.2/cflearn/api/cv/third_party/mlsd/
+-rw-rw-rw-   0        0        0       20 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/api/cv/third_party/mlsd/__init__.py
+-rw-rw-rw-   0        0        0     2106 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/api/cv/third_party/mlsd/api.py
+drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.271708 carefree-learn-0.4.2/cflearn/api/cv/third_party/mlsd/models/
+-rw-rw-rw-   0        0        0        0 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/api/cv/third_party/mlsd/models/__init__.py
+-rw-rw-rw-   0        0        0    10142 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/api/cv/third_party/mlsd/models/mbv2_mlsd_large.py
+-rw-rw-rw-   0        0        0     9711 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/api/cv/third_party/mlsd/models/mbv2_mlsd_tiny.py
+-rw-rw-rw-   0        0        0    26167 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/api/cv/third_party/mlsd/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.274711 carefree-learn-0.4.2/cflearn/api/cv/third_party/openpose/
+-rw-rw-rw-   0        0        0       20 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/api/cv/third_party/openpose/__init__.py
+-rw-rw-rw-   0        0        0     2392 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/api/cv/third_party/openpose/api.py
+-rw-rw-rw-   0        0        0    14093 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/api/cv/third_party/openpose/body.py
+-rw-rw-rw-   0        0        0     4271 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/api/cv/third_party/openpose/hand.py
+-rw-rw-rw-   0        0        0     9090 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/api/cv/third_party/openpose/model.py
+-rw-rw-rw-   0        0        0     8699 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/api/cv/third_party/openpose/util.py
+-rw-rw-rw-   0        0        0     2053 2023-04-04 02:24:07.000000 carefree-learn-0.4.2/cflearn/api/cv/third_party/prompt.py
+-rw-rw-rw-   0        0        0     2489 2023-03-23 09:35:16.000000 carefree-learn-0.4.2/cflearn/api/cv/translator.py
+drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.274711 carefree-learn-0.4.2/cflearn/api/ml/
+-rw-rw-rw-   0        0        0       20 2023-03-23 05:48:39.000000 carefree-learn-0.4.2/cflearn/api/ml/__init__.py
+-rw-rw-rw-   0        0        0     8678 2023-03-23 05:48:39.000000 carefree-learn-0.4.2/cflearn/api/ml/ddr.py
+-rw-rw-rw-   0        0        0      524 2023-01-29 11:37:21.000000 carefree-learn-0.4.2/cflearn/api/schema.py
+-rw-rw-rw-   0        0        0     5513 2023-04-20 04:16:04.000000 carefree-learn-0.4.2/cflearn/api/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.275712 carefree-learn-0.4.2/cflearn/api/zoo/
+-rw-rw-rw-   0        0        0     6163 2023-03-29 08:24:36.000000 carefree-learn-0.4.2/cflearn/api/zoo/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.276711 carefree-learn-0.4.2/cflearn/callbacks/
+-rw-rw-rw-   0        0        0       81 2023-03-23 05:48:39.000000 carefree-learn-0.4.2/cflearn/callbacks/__init__.py
+-rw-rw-rw-   0        0        0     1118 2023-03-23 09:35:20.000000 carefree-learn-0.4.2/cflearn/callbacks/classification.py
+-rw-rw-rw-   0        0        0     9649 2023-03-23 08:40:04.000000 carefree-learn-0.4.2/cflearn/callbacks/general.py
+-rw-rw-rw-   0        0        0     4212 2023-03-23 09:35:26.000000 carefree-learn-0.4.2/cflearn/callbacks/generator.py
+-rw-rw-rw-   0        0        0      656 2023-03-23 05:48:39.000000 carefree-learn-0.4.2/cflearn/constants.py
+drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.277711 carefree-learn-0.4.2/cflearn/data/
+-rw-rw-rw-   0        0        0      247 2023-03-28 06:24:25.000000 carefree-learn-0.4.2/cflearn/data/__init__.py
+-rw-rw-rw-   0        0        0     2798 2023-03-28 02:09:34.000000 carefree-learn-0.4.2/cflearn/data/array.py
+drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.278711 carefree-learn-0.4.2/cflearn/data/blocks/
+-rw-rw-rw-   0        0        0       62 2023-03-23 05:48:39.000000 carefree-learn-0.4.2/cflearn/data/blocks/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.281711 carefree-learn-0.4.2/cflearn/data/blocks/cv/
+-rw-rw-rw-   0        0        0      159 2023-03-29 09:56:34.000000 carefree-learn-0.4.2/cflearn/data/blocks/cv/__init__.py
+-rw-rw-rw-   0        0        0     1447 2023-03-29 10:00:43.000000 carefree-learn-0.4.2/cflearn/data/blocks/cv/crop.py
+-rw-rw-rw-   0        0        0      477 2023-03-23 05:48:39.000000 carefree-learn-0.4.2/cflearn/data/blocks/cv/hwc_to_chw.py
+-rw-rw-rw-   0        0        0    31082 2023-03-29 07:34:59.000000 carefree-learn-0.4.2/cflearn/data/blocks/cv/image_folder.py
+-rw-rw-rw-   0        0        0     2054 2023-03-29 07:34:59.000000 carefree-learn-0.4.2/cflearn/data/blocks/cv/normalize.py
+-rw-rw-rw-   0        0        0     1002 2023-03-23 05:48:39.000000 carefree-learn-0.4.2/cflearn/data/blocks/cv/to_numpy.py
+-rw-rw-rw-   0        0        0      609 2023-03-23 05:48:39.000000 carefree-learn-0.4.2/cflearn/data/blocks/cv/tuple_to_batch.py
+-rw-rw-rw-   0        0        0      375 2023-03-23 05:48:39.000000 carefree-learn-0.4.2/cflearn/data/blocks/flatten.py
+drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.285712 carefree-learn-0.4.2/cflearn/data/blocks/ml/
+-rw-rw-rw-   0        0        0      176 2023-03-23 05:48:39.000000 carefree-learn-0.4.2/cflearn/data/blocks/ml/__init__.py
+-rw-rw-rw-   0        0        0    19260 2023-03-29 06:28:32.000000 carefree-learn-0.4.2/cflearn/data/blocks/ml/file.py
+-rw-rw-rw-   0        0        0     1729 2023-03-29 06:29:22.000000 carefree-learn-0.4.2/cflearn/data/blocks/ml/gather.py
+-rw-rw-rw-   0        0        0     7608 2023-03-29 06:29:31.000000 carefree-learn-0.4.2/cflearn/data/blocks/ml/nan_handler.py
+-rw-rw-rw-   0        0        0     7327 2023-03-29 06:29:45.000000 carefree-learn-0.4.2/cflearn/data/blocks/ml/preprocessor.py
+-rw-rw-rw-   0        0        0     6234 2023-03-29 06:30:03.000000 carefree-learn-0.4.2/cflearn/data/blocks/ml/recognizer.py
+-rw-rw-rw-   0        0        0      416 2023-03-23 05:48:39.000000 carefree-learn-0.4.2/cflearn/data/blocks/ml/schema.py
+-rw-rw-rw-   0        0        0    12175 2023-03-29 06:30:47.000000 carefree-learn-0.4.2/cflearn/data/blocks/ml/splitter.py
+drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.286712 carefree-learn-0.4.2/cflearn/data/ml/
+-rw-rw-rw-   0        0        0       45 2023-03-23 05:48:39.000000 carefree-learn-0.4.2/cflearn/data/ml/__init__.py
+-rw-rw-rw-   0        0        0     7741 2023-03-29 06:34:52.000000 carefree-learn-0.4.2/cflearn/data/ml/api.py
+-rw-rw-rw-   0        0        0     1292 2023-03-23 05:48:39.000000 carefree-learn-0.4.2/cflearn/data/ml/datasets.py
+drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.287711 carefree-learn-0.4.2/cflearn/data/pytorch/
+-rw-rw-rw-   0        0        0       45 2023-03-23 05:48:39.000000 carefree-learn-0.4.2/cflearn/data/pytorch/__init__.py
+-rw-rw-rw-   0        0        0     8349 2023-03-27 12:47:27.000000 carefree-learn-0.4.2/cflearn/data/pytorch/api.py
+-rw-rw-rw-   0        0        0     1406 2023-03-29 06:36:58.000000 carefree-learn-0.4.2/cflearn/data/pytorch/datasets.py
+-rw-rw-rw-   0        0        0     7842 2023-03-28 02:09:41.000000 carefree-learn-0.4.2/cflearn/data/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.287711 carefree-learn-0.4.2/cflearn/dist/
+-rw-rw-rw-   0        0        0       18 2022-10-23 14:55:07.000000 carefree-learn-0.4.2/cflearn/dist/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.289219 carefree-learn-0.4.2/cflearn/dist/ml/
+-rw-rw-rw-   0        0        0      159 2022-10-23 14:55:07.000000 carefree-learn-0.4.2/cflearn/dist/ml/__init__.py
+-rw-rw-rw-   0        0        0     8874 2023-03-23 05:48:39.000000 carefree-learn-0.4.2/cflearn/dist/ml/experiment.py
+drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.290223 carefree-learn-0.4.2/cflearn/dist/ml/runs/
+-rw-rw-rw-   0        0        0        0 2022-10-23 14:55:07.000000 carefree-learn-0.4.2/cflearn/dist/ml/runs/__init__.py
+-rw-rw-rw-   0        0        0     1320 2023-03-23 05:48:39.000000 carefree-learn-0.4.2/cflearn/dist/ml/runs/_utils.py
+-rw-rw-rw-   0        0        0      291 2023-03-23 05:48:39.000000 carefree-learn-0.4.2/cflearn/dist/ml/runs/basic.py
+-rw-rw-rw-   0        0        0     1709 2023-03-23 05:48:39.000000 carefree-learn-0.4.2/cflearn/dist/ml/task.py
+-rw-rw-rw-   0        0        0     8910 2023-03-23 05:48:39.000000 carefree-learn-0.4.2/cflearn/inference.py
+drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.292223 carefree-learn-0.4.2/cflearn/losses/
+-rw-rw-rw-   0        0        0       84 2022-10-23 14:55:07.000000 carefree-learn-0.4.2/cflearn/losses/__init__.py
+-rw-rw-rw-   0        0        0     6391 2023-03-29 12:15:03.000000 carefree-learn-0.4.2/cflearn/losses/basic.py
+-rw-rw-rw-   0        0        0     2546 2022-10-23 14:55:07.000000 carefree-learn-0.4.2/cflearn/losses/gan.py
+-rw-rw-rw-   0        0        0     2812 2023-03-24 02:18:57.000000 carefree-learn-0.4.2/cflearn/losses/lpips.py
+-rw-rw-rw-   0        0        0     3962 2023-03-23 05:48:39.000000 carefree-learn-0.4.2/cflearn/losses/vae.py
+-rw-rw-rw-   0        0        0     5614 2023-03-23 05:48:39.000000 carefree-learn-0.4.2/cflearn/metrics.py
+drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.293223 carefree-learn-0.4.2/cflearn/misc/
+-rw-rw-rw-   0        0        0        0 2023-02-14 02:22:11.000000 carefree-learn-0.4.2/cflearn/misc/__init__.py
+-rw-rw-rw-   0        0        0    14696 2023-04-20 10:57:14.000000 carefree-learn-0.4.2/cflearn/misc/available.json
+-rw-rw-rw-   0        0        0     1375 2023-03-23 05:48:39.000000 carefree-learn-0.4.2/cflearn/misc/mixins.py
+-rw-rw-rw-   0        0        0    42445 2023-04-12 11:55:25.000000 carefree-learn-0.4.2/cflearn/misc/toolkit.py
+drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.294223 carefree-learn-0.4.2/cflearn/models/
+-rw-rw-rw-   0        0        0       62 2023-03-23 05:48:39.000000 carefree-learn-0.4.2/cflearn/models/__init__.py
+-rw-rw-rw-   0        0        0     5563 2023-01-29 11:37:21.000000 carefree-learn-0.4.2/cflearn/models/bases.py
+drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.295223 carefree-learn-0.4.2/cflearn/models/cv/
+-rw-rw-rw-   0        0        0      167 2023-03-23 05:48:39.000000 carefree-learn-0.4.2/cflearn/models/cv/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.296223 carefree-learn-0.4.2/cflearn/models/cv/ae/
+-rw-rw-rw-   0        0        0       38 2023-03-22 05:28:24.000000 carefree-learn-0.4.2/cflearn/models/cv/ae/__init__.py
+-rw-rw-rw-   0        0        0    12091 2023-03-27 01:50:04.000000 carefree-learn-0.4.2/cflearn/models/cv/ae/common.py
+-rw-rw-rw-   0        0        0     8409 2023-03-27 01:52:38.000000 carefree-learn-0.4.2/cflearn/models/cv/ae/kl.py
+-rw-rw-rw-   0        0        0     7970 2023-03-27 01:52:49.000000 carefree-learn-0.4.2/cflearn/models/cv/ae/vq.py
+drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.297223 carefree-learn-0.4.2/cflearn/models/cv/classifier/
+-rw-rw-rw-   0        0        0       24 2022-10-23 14:55:07.000000 carefree-learn-0.4.2/cflearn/models/cv/classifier/__init__.py
+-rw-rw-rw-   0        0        0     4079 2023-01-29 11:37:21.000000 carefree-learn-0.4.2/cflearn/models/cv/classifier/vanilla.py
+drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.301226 carefree-learn-0.4.2/cflearn/models/cv/decoder/
+-rw-rw-rw-   0        0        0      145 2023-01-29 11:37:21.000000 carefree-learn-0.4.2/cflearn/models/cv/decoder/__init__.py
+-rw-rw-rw-   0        0        0     3619 2023-02-27 01:58:50.000000 carefree-learn-0.4.2/cflearn/models/cv/decoder/attn.py
+-rw-rw-rw-   0        0        0     4162 2023-01-29 11:37:21.000000 carefree-learn-0.4.2/cflearn/models/cv/decoder/schema.py
+-rw-rw-rw-   0        0        0     8739 2023-01-29 11:37:21.000000 carefree-learn-0.4.2/cflearn/models/cv/decoder/style_gan.py
+-rw-rw-rw-   0        0        0    14508 2023-01-29 11:37:21.000000 carefree-learn-0.4.2/cflearn/models/cv/decoder/style_gan_v2.py
+-rw-rw-rw-   0        0        0     9329 2023-01-29 11:37:21.000000 carefree-learn-0.4.2/cflearn/models/cv/decoder/vanilla.py
+-rw-rw-rw-   0        0        0     3952 2023-01-29 11:37:21.000000 carefree-learn-0.4.2/cflearn/models/cv/decoder/vqgan.py
+drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.303223 carefree-learn-0.4.2/cflearn/models/cv/diffusion/
+-rw-rw-rw-   0        0        0       87 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/models/cv/diffusion/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.305222 carefree-learn-0.4.2/cflearn/models/cv/diffusion/cond_models/
+-rw-rw-rw-   0        0        0       69 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/models/cv/diffusion/cond_models/__init__.py
+-rw-rw-rw-   0        0        0    10010 2023-03-23 05:48:39.000000 carefree-learn-0.4.2/cflearn/models/cv/diffusion/cond_models/clip.py
+-rw-rw-rw-   0        0        0     1525 2023-03-24 02:19:09.000000 carefree-learn-0.4.2/cflearn/models/cv/diffusion/cond_models/rescaler.py
+-rw-rw-rw-   0        0        0     1182 2023-03-23 05:48:39.000000 carefree-learn-0.4.2/cflearn/models/cv/diffusion/cond_models/schema.py
+-rw-rw-rw-   0        0        0    28538 2023-05-06 05:26:10.000000 carefree-learn-0.4.2/cflearn/models/cv/diffusion/ddpm.py
+-rw-rw-rw-   0        0        0    10395 2023-04-20 06:47:39.000000 carefree-learn-0.4.2/cflearn/models/cv/diffusion/ldm.py
+drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.309223 carefree-learn-0.4.2/cflearn/models/cv/diffusion/samplers/
+-rw-rw-rw-   0        0        0      137 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/models/cv/diffusion/samplers/__init__.py
+-rw-rw-rw-   0        0        0     2258 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/models/cv/diffusion/samplers/basic.py
+-rw-rw-rw-   0        0        0     9817 2023-03-23 05:48:39.000000 carefree-learn-0.4.2/cflearn/models/cv/diffusion/samplers/ddim.py
+-rw-rw-rw-   0        0        0    13157 2023-04-20 02:12:01.000000 carefree-learn-0.4.2/cflearn/models/cv/diffusion/samplers/k_samplers.py
+-rw-rw-rw-   0        0        0     2593 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/models/cv/diffusion/samplers/plms.py
+-rw-rw-rw-   0        0        0     7804 2023-05-04 11:20:31.000000 carefree-learn-0.4.2/cflearn/models/cv/diffusion/samplers/schema.py
+-rw-rw-rw-   0        0        0    16613 2023-03-23 05:48:39.000000 carefree-learn-0.4.2/cflearn/models/cv/diffusion/samplers/solver.py
+-rw-rw-rw-   0        0        0     2561 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/models/cv/diffusion/samplers/utils.py
+-rw-rw-rw-   0        0        0    20269 2023-04-20 03:26:15.000000 carefree-learn-0.4.2/cflearn/models/cv/diffusion/unet.py
+-rw-rw-rw-   0        0        0      737 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/models/cv/diffusion/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.313223 carefree-learn-0.4.2/cflearn/models/cv/encoder/
+-rw-rw-rw-   0        0        0      240 2023-01-29 11:37:21.000000 carefree-learn-0.4.2/cflearn/models/cv/encoder/__init__.py
+-rw-rw-rw-   0        0        0     3369 2023-02-27 01:58:50.000000 carefree-learn-0.4.2/cflearn/models/cv/encoder/attn.py
+drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.315224 carefree-learn-0.4.2/cflearn/models/cv/encoder/backbone/
+-rw-rw-rw-   0        0        0       64 2022-10-23 14:55:07.000000 carefree-learn-0.4.2/cflearn/models/cv/encoder/backbone/__init__.py
+-rw-rw-rw-   0        0        0     3109 2023-01-29 11:37:21.000000 carefree-learn-0.4.2/cflearn/models/cv/encoder/backbone/api.py
+-rw-rw-rw-   0        0        0     4242 2022-10-23 14:55:07.000000 carefree-learn-0.4.2/cflearn/models/cv/encoder/backbone/core.py
+drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.317223 carefree-learn-0.4.2/cflearn/models/cv/encoder/backbone/models/
+-rw-rw-rw-   0        0        0       97 2022-10-23 14:55:07.000000 carefree-learn-0.4.2/cflearn/models/cv/encoder/backbone/models/__init__.py
+-rw-rw-rw-   0        0        0      430 2022-10-23 14:55:07.000000 carefree-learn-0.4.2/cflearn/models/cv/encoder/backbone/models/mobilenet.py
+-rw-rw-rw-   0        0        0     1225 2022-10-23 14:55:07.000000 carefree-learn-0.4.2/cflearn/models/cv/encoder/backbone/models/resnet.py
+-rw-rw-rw-   0        0        0     5392 2023-02-10 05:26:29.000000 carefree-learn-0.4.2/cflearn/models/cv/encoder/backbone/models/transformer.py
+-rw-rw-rw-   0        0        0    13725 2022-10-23 14:55:07.000000 carefree-learn-0.4.2/cflearn/models/cv/encoder/backbone/models/vgg.py
+-rw-rw-rw-   0        0        0      968 2022-10-23 14:55:07.000000 carefree-learn-0.4.2/cflearn/models/cv/encoder/backbone/register.py
+-rw-rw-rw-   0        0        0     1133 2023-02-10 03:39:20.000000 carefree-learn-0.4.2/cflearn/models/cv/encoder/fnet.py
+-rw-rw-rw-   0        0        0     1132 2023-02-10 03:39:20.000000 carefree-learn-0.4.2/cflearn/models/cv/encoder/mixer.py
+-rw-rw-rw-   0        0        0     2336 2023-01-29 11:37:21.000000 carefree-learn-0.4.2/cflearn/models/cv/encoder/perceiver.py
+-rw-rw-rw-   0        0        0     1149 2023-02-10 03:39:20.000000 carefree-learn-0.4.2/cflearn/models/cv/encoder/pool_former.py
+-rw-rw-rw-   0        0        0     5124 2023-03-23 05:48:39.000000 carefree-learn-0.4.2/cflearn/models/cv/encoder/schema.py
+-rw-rw-rw-   0        0        0     6125 2023-03-22 07:19:34.000000 carefree-learn-0.4.2/cflearn/models/cv/encoder/transformer.py
+-rw-rw-rw-   0        0        0     5535 2023-01-29 11:37:21.000000 carefree-learn-0.4.2/cflearn/models/cv/encoder/vanilla.py
+-rw-rw-rw-   0        0        0     5473 2023-01-29 11:37:21.000000 carefree-learn-0.4.2/cflearn/models/cv/encoder/vqgan.py
+drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.319223 carefree-learn-0.4.2/cflearn/models/cv/gan/
+-rw-rw-rw-   0        0        0       55 2023-03-23 05:48:39.000000 carefree-learn-0.4.2/cflearn/models/cv/gan/__init__.py
+-rw-rw-rw-   0        0        0     5920 2022-10-23 14:55:07.000000 carefree-learn-0.4.2/cflearn/models/cv/gan/discriminators.py
+-rw-rw-rw-   0        0        0     7730 2023-03-29 11:05:45.000000 carefree-learn-0.4.2/cflearn/models/cv/gan/schema.py
+-rw-rw-rw-   0        0        0     1913 2023-03-23 05:48:39.000000 carefree-learn-0.4.2/cflearn/models/cv/gan/vanilla.py
+-rw-rw-rw-   0        0        0     6731 2023-03-23 05:48:39.000000 carefree-learn-0.4.2/cflearn/models/cv/general.py
+drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.320223 carefree-learn-0.4.2/cflearn/models/cv/translator/
+-rw-rw-rw-   0        0        0       21 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/models/cv/translator/__init__.py
+-rw-rw-rw-   0        0        0     4018 2023-03-23 05:48:39.000000 carefree-learn-0.4.2/cflearn/models/cv/translator/rrdb.py
+drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.321223 carefree-learn-0.4.2/cflearn/models/implicit/
+-rw-rw-rw-   0        0        0       22 2022-10-23 14:55:07.000000 carefree-learn-0.4.2/cflearn/models/implicit/__init__.py
+-rw-rw-rw-   0        0        0     7927 2022-10-23 14:55:07.000000 carefree-learn-0.4.2/cflearn/models/implicit/siren.py
+drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.325223 carefree-learn-0.4.2/cflearn/models/ml/
+-rw-rw-rw-   0        0        0      165 2023-03-23 05:48:39.000000 carefree-learn-0.4.2/cflearn/models/ml/__init__.py
+-rw-rw-rw-   0        0        0     1857 2023-03-23 05:48:39.000000 carefree-learn-0.4.2/cflearn/models/ml/base.py
+-rw-rw-rw-   0        0        0    11624 2023-03-29 12:15:02.000000 carefree-learn-0.4.2/cflearn/models/ml/ddr.py
+-rw-rw-rw-   0        0        0     8958 2023-03-28 02:09:49.000000 carefree-learn-0.4.2/cflearn/models/ml/encoders.py
+-rw-rw-rw-   0        0        0     2392 2023-03-23 05:48:39.000000 carefree-learn-0.4.2/cflearn/models/ml/fcnn.py
+-rw-rw-rw-   0        0        0     1100 2023-03-23 05:48:39.000000 carefree-learn-0.4.2/cflearn/models/ml/linear.py
+-rw-rw-rw-   0        0        0     6980 2023-03-23 05:48:39.000000 carefree-learn-0.4.2/cflearn/models/ml/mixed_stacked.py
+-rw-rw-rw-   0        0        0     7976 2023-03-23 05:48:39.000000 carefree-learn-0.4.2/cflearn/models/ml/nbm.py
+-rw-rw-rw-   0        0        0     5272 2023-03-23 05:48:39.000000 carefree-learn-0.4.2/cflearn/models/ml/ndt.py
+-rw-rw-rw-   0        0        0     3068 2023-03-23 05:48:39.000000 carefree-learn-0.4.2/cflearn/models/ml/rnn.py
+-rw-rw-rw-   0        0        0     2798 2023-03-23 05:48:39.000000 carefree-learn-0.4.2/cflearn/models/ml/wnd.py
+drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.326223 carefree-learn-0.4.2/cflearn/models/multimodal/
+-rw-rw-rw-   0        0        0       21 2023-03-23 05:48:39.000000 carefree-learn-0.4.2/cflearn/models/multimodal/__init__.py
+-rw-rw-rw-   0        0        0    10260 2023-03-23 08:58:17.000000 carefree-learn-0.4.2/cflearn/models/multimodal/clip.py
+-rw-rw-rw-   0        0        0       19 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/models/multimodal/constants.py
+-rw-rw-rw-   0        0        0     1554 2023-03-29 11:05:45.000000 carefree-learn-0.4.2/cflearn/models/multimodal/schema.py
+drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.327223 carefree-learn-0.4.2/cflearn/models/nlp/
+-rw-rw-rw-   0        0        0       80 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/models/nlp/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.328223 carefree-learn-0.4.2/cflearn/models/nlp/encoder/
+-rw-rw-rw-   0        0        0       28 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/models/nlp/encoder/__init__.py
+-rw-rw-rw-   0        0        0       19 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/models/nlp/encoder/constants.py
+-rw-rw-rw-   0        0        0     3694 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/models/nlp/encoder/transformer.py
+drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.329222 carefree-learn-0.4.2/cflearn/models/nlp/tokenizers/
+-rw-rw-rw-   0        0        0       44 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/models/nlp/tokenizers/__init__.py
+-rw-rw-rw-   0        0        0     2371 2023-03-23 05:48:39.000000 carefree-learn-0.4.2/cflearn/models/nlp/tokenizers/clip.py
+-rw-rw-rw-   0        0        0     1226 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/models/nlp/tokenizers/schema.py
+drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.331223 carefree-learn-0.4.2/cflearn/models/nlp/transformers/
+-rw-rw-rw-   0        0        0       66 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/models/nlp/transformers/__init__.py
+-rw-rw-rw-   0        0        0     3547 2023-03-27 13:58:44.000000 carefree-learn-0.4.2/cflearn/models/nlp/transformers/core.py
+-rw-rw-rw-   0        0        0     1575 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/models/nlp/transformers/opus.py
+-rw-rw-rw-   0        0        0      813 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/models/nlp/transformers/simbert.py
+drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.332224 carefree-learn-0.4.2/cflearn/models/schemas/
+-rw-rw-rw-   0        0        0       42 2023-03-27 01:49:17.000000 carefree-learn-0.4.2/cflearn/models/schemas/__init__.py
+-rw-rw-rw-   0        0        0    12838 2023-04-04 02:24:07.000000 carefree-learn-0.4.2/cflearn/models/schemas/custom.py
+-rw-rw-rw-   0        0        0     4631 2023-03-23 05:48:39.000000 carefree-learn-0.4.2/cflearn/models/schemas/cv.py
+drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.334223 carefree-learn-0.4.2/cflearn/modules/
+-rw-rw-rw-   0        0        0       54 2022-10-23 14:55:07.000000 carefree-learn-0.4.2/cflearn/modules/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.341222 carefree-learn-0.4.2/cflearn/modules/blocks/
+-rw-rw-rw-   0        0        0      756 2023-03-24 08:39:05.000000 carefree-learn-0.4.2/cflearn/modules/blocks/__init__.py
+-rw-rw-rw-   0        0        0     5165 2023-03-24 02:18:16.000000 carefree-learn-0.4.2/cflearn/modules/blocks/activations.py
+-rw-rw-rw-   0        0        0    22018 2023-04-12 11:14:32.000000 carefree-learn-0.4.2/cflearn/modules/blocks/attentions.py
+-rw-rw-rw-   0        0        0     6448 2022-11-09 12:05:57.000000 carefree-learn-0.4.2/cflearn/modules/blocks/common.py
+drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.343222 carefree-learn-0.4.2/cflearn/modules/blocks/convs/
+-rw-rw-rw-   0        0        0       47 2022-10-23 14:55:07.000000 carefree-learn-0.4.2/cflearn/modules/blocks/convs/__init__.py
+-rw-rw-rw-   0        0        0    19321 2023-03-24 02:29:08.000000 carefree-learn-0.4.2/cflearn/modules/blocks/convs/basic.py
+-rw-rw-rw-   0        0        0     8836 2023-03-24 02:19:26.000000 carefree-learn-0.4.2/cflearn/modules/blocks/convs/residual.py
+-rw-rw-rw-   0        0        0    18802 2023-04-12 11:14:59.000000 carefree-learn-0.4.2/cflearn/modules/blocks/customs.py
+-rw-rw-rw-   0        0        0     8503 2023-03-23 05:48:39.000000 carefree-learn-0.4.2/cflearn/modules/blocks/high_level.py
+-rw-rw-rw-   0        0        0    14999 2023-04-12 13:33:59.000000 carefree-learn-0.4.2/cflearn/modules/blocks/hijacks.py
+-rw-rw-rw-   0        0        0     1304 2023-04-12 13:32:32.000000 carefree-learn-0.4.2/cflearn/modules/blocks/hooks.py
+drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.345223 carefree-learn-0.4.2/cflearn/modules/blocks/implementations/
+-rw-rw-rw-   0        0        0       26 2022-10-23 14:55:07.000000 carefree-learn-0.4.2/cflearn/modules/blocks/implementations/__init__.py
+-rw-rw-rw-   0        0        0     4708 2022-10-23 14:55:07.000000 carefree-learn-0.4.2/cflearn/modules/blocks/implementations/perceiver.py
+-rw-rw-rw-   0        0        0     6189 2023-01-29 11:37:21.000000 carefree-learn-0.4.2/cflearn/modules/blocks/mappings.py
+drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.349223 carefree-learn-0.4.2/cflearn/modules/blocks/mixed_stacks/
+-rw-rw-rw-   0        0        0      127 2023-02-10 03:31:37.000000 carefree-learn-0.4.2/cflearn/modules/blocks/mixed_stacks/__init__.py
+-rw-rw-rw-   0        0        0    28432 2023-04-12 08:04:35.000000 carefree-learn-0.4.2/cflearn/modules/blocks/mixed_stacks/api.py
+-rw-rw-rw-   0        0        0     3774 2023-03-24 08:39:41.000000 carefree-learn-0.4.2/cflearn/modules/blocks/mixed_stacks/channel_mixers.py
+-rw-rw-rw-   0        0        0     1179 2022-10-23 14:55:07.000000 carefree-learn-0.4.2/cflearn/modules/blocks/mixed_stacks/poolers.py
+-rw-rw-rw-   0        0        0     1325 2023-02-10 05:18:20.000000 carefree-learn-0.4.2/cflearn/modules/blocks/mixed_stacks/schema.py
+-rw-rw-rw-   0        0        0     6998 2023-02-10 10:31:50.000000 carefree-learn-0.4.2/cflearn/modules/blocks/mixed_stacks/token_mixers.py
+-rw-rw-rw-   0        0        0     4682 2022-10-23 14:55:07.000000 carefree-learn-0.4.2/cflearn/modules/blocks/norms.py
+-rw-rw-rw-   0        0        0      863 2023-02-27 01:58:50.000000 carefree-learn-0.4.2/cflearn/modules/blocks/utils.py
+-rw-rw-rw-   0        0        0     4751 2022-10-23 14:55:07.000000 carefree-learn-0.4.2/cflearn/modules/optimizers.py
+-rw-rw-rw-   0        0        0     9159 2022-11-09 12:09:28.000000 carefree-learn-0.4.2/cflearn/modules/schedulers.py
+-rw-rw-rw-   0        0        0     4774 2023-03-23 05:48:39.000000 carefree-learn-0.4.2/cflearn/monitors.py
+-rw-rw-rw-   0        0        0      634 2023-02-16 10:09:59.000000 carefree-learn-0.4.2/cflearn/parameters.py
+drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.351223 carefree-learn-0.4.2/cflearn/pipeline/
+-rw-rw-rw-   0        0        0       92 2023-03-23 05:48:39.000000 carefree-learn-0.4.2/cflearn/pipeline/__init__.py
+-rw-rw-rw-   0        0        0    23551 2023-03-29 11:32:53.000000 carefree-learn-0.4.2/cflearn/pipeline/api.py
+drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.353222 carefree-learn-0.4.2/cflearn/pipeline/blocks/
+-rw-rw-rw-   0        0        0       41 2023-03-23 05:48:39.000000 carefree-learn-0.4.2/cflearn/pipeline/blocks/__init__.py
+-rw-rw-rw-   0        0        0    36043 2023-03-27 01:51:03.000000 carefree-learn-0.4.2/cflearn/pipeline/blocks/basic.py
+-rw-rw-rw-   0        0        0     2735 2023-03-23 05:48:39.000000 carefree-learn-0.4.2/cflearn/pipeline/blocks/ml.py
+-rw-rw-rw-   0        0        0     1335 2023-03-23 05:48:39.000000 carefree-learn-0.4.2/cflearn/pipeline/blocks/utils.py
+-rw-rw-rw-   0        0        0     3921 2023-03-23 08:46:39.000000 carefree-learn-0.4.2/cflearn/pipeline/core.py
+-rw-rw-rw-   0        0        0      310 2023-03-23 05:48:39.000000 carefree-learn-0.4.2/cflearn/pipeline/schema.py
+-rw-rw-rw-   0        0        0     1545 2023-03-23 05:48:39.000000 carefree-learn-0.4.2/cflearn/pipeline/third_party.py
+-rw-rw-rw-   0        0        0      510 2023-03-23 05:48:39.000000 carefree-learn-0.4.2/cflearn/register.py
+-rw-rw-rw-   0        0        0    60784 2023-03-29 15:41:28.000000 carefree-learn-0.4.2/cflearn/schema.py
+drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.354221 carefree-learn-0.4.2/cflearn/scripts/
+-rw-rw-rw-   0        0        0       18 2023-03-24 10:59:16.000000 carefree-learn-0.4.2/cflearn/scripts/__init__.py
+-rw-rw-rw-   0        0        0    12752 2023-04-04 02:24:07.000000 carefree-learn-0.4.2/cflearn/scripts/sd.py
+-rw-rw-rw-   0        0        0    28526 2023-04-04 02:24:07.000000 carefree-learn-0.4.2/cflearn/trainer.py
+-rw-rw-rw-   0        0        0     1053 2023-03-23 05:48:39.000000 carefree-learn-0.4.2/cflearn/types.py
+drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.354221 carefree-learn-0.4.2/cflearn/zoo/
+-rw-rw-rw-   0        0        0       21 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/zoo/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.225708 carefree-learn-0.4.2/cflearn/zoo/configs/
+drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.224708 carefree-learn-0.4.2/cflearn/zoo/configs/ae/
+drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.356221 carefree-learn-0.4.2/cflearn/zoo/configs/ae/kl/
+-rw-rw-rw-   0        0        0      201 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/zoo/configs/ae/kl/f16.json
+-rw-rw-rw-   0        0        0      868 2023-03-23 05:48:39.000000 carefree-learn-0.4.2/cflearn/zoo/configs/ae/kl/f4.json
+-rw-rw-rw-   0        0        0      160 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/zoo/configs/ae/kl/f8.json
+drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.358222 carefree-learn-0.4.2/cflearn/zoo/configs/ae/vq/
+-rw-rw-rw-   0        0        0      205 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/zoo/configs/ae/vq/f4.json
+-rw-rw-rw-   0        0        0       92 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/zoo/configs/ae/vq/f4_no_attn.json
+-rw-rw-rw-   0        0        0      295 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/zoo/configs/ae/vq/f8.json
+drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.224708 carefree-learn-0.4.2/cflearn/zoo/configs/diffusion/
+drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.358222 carefree-learn-0.4.2/cflearn/zoo/configs/diffusion/ddpm/
+-rw-rw-rw-   0        0        0     1155 2023-03-23 05:48:39.000000 carefree-learn-0.4.2/cflearn/zoo/configs/diffusion/ddpm/default.json
+drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.361222 carefree-learn-0.4.2/cflearn/zoo/configs/diffusion/ldm/
+-rw-rw-rw-   0        0        0      513 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/zoo/configs/diffusion/ldm/default.json
+-rw-rw-rw-   0        0        0      451 2023-04-04 04:59:57.000000 carefree-learn-0.4.2/cflearn/zoo/configs/diffusion/ldm/sd.json
+-rw-rw-rw-   0        0        0      125 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/zoo/configs/diffusion/ldm/sd_inpainting.json
+-rw-rw-rw-   0        0        0      344 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/zoo/configs/diffusion/ldm/sd_v2.json
+-rw-rw-rw-   0        0        0      104 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/zoo/configs/diffusion/ldm/sd_v2_base.json
+-rw-rw-rw-   0        0        0      600 2023-03-23 05:48:39.000000 carefree-learn-0.4.2/cflearn/zoo/configs/diffusion/ldm/vq.json
+drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.224708 carefree-learn-0.4.2/cflearn/zoo/configs/multimodal/
+drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.363222 carefree-learn-0.4.2/cflearn/zoo/configs/multimodal/clip/
+-rw-rw-rw-   0        0        0      525 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/zoo/configs/multimodal/clip/chinese.json
+-rw-rw-rw-   0        0        0       79 2023-03-23 05:48:39.000000 carefree-learn-0.4.2/cflearn/zoo/configs/multimodal/clip/default.json
+-rw-rw-rw-   0        0        0      269 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/zoo/configs/multimodal/clip/large.json
+-rw-rw-rw-   0        0        0      389 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/zoo/configs/multimodal/clip/open_clip_ViT_H_14.json
+drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.225708 carefree-learn-0.4.2/cflearn/zoo/configs/sr/
+drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.364222 carefree-learn-0.4.2/cflearn/zoo/configs/sr/esr/
+-rw-rw-rw-   0        0        0       81 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/zoo/configs/sr/esr/anime.json
+-rw-rw-rw-   0        0        0       79 2023-03-23 05:48:39.000000 carefree-learn-0.4.2/cflearn/zoo/configs/sr/esr/default.json
+-rw-rw-rw-   0        0        0     7814 2023-03-29 11:34:44.000000 carefree-learn-0.4.2/cflearn/zoo/core.py
+drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.365221 carefree-learn-0.4.2/cflearn/zoo/models/
+-rw-rw-rw-   0        0        0       44 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/zoo/models/__init__.py
+-rw-rw-rw-   0        0        0     1606 2023-03-23 05:48:39.000000 carefree-learn-0.4.2/cflearn/zoo/models/clip.py
+-rw-rw-rw-   0        0        0      506 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/zoo/models/schema.py
+-rw-rw-rw-   0        0        0      383 2023-05-06 05:29:58.370221 carefree-learn-0.4.2/setup.cfg
+-rw-rw-rw-   0        0        0     1702 2023-05-06 05:22:46.000000 carefree-learn-0.4.2/setup.py
```

### Comparing `carefree-learn-0.4.1/LICENSE` & `carefree-learn-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/PKG-INFO` & `carefree-learn-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: carefree-learn
-Version: 0.4.1
+Version: 0.4.2
 Summary: Deep Learning with PyTorch made easy
 Home-page: https://github.com/carefree0910/carefree-learn
-Download-URL: https://github.com/carefree0910/carefree-learn/archive/v0.4.1.tar.gz
+Download-URL: https://github.com/carefree0910/carefree-learn/archive/v0.4.2.tar.gz
 Author: carefree0910
 Author-email: syameimaru.saki@gmail.com
 Keywords: python machine-learning deep-learning solution PyTorch
 Description-Content-Type: text/markdown
 Provides-Extra: onnx
 Provides-Extra: cv
 Provides-Extra: cv_full
```

### Comparing `carefree-learn-0.4.1/README.md` & `carefree-learn-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/carefree_learn.egg-info/PKG-INFO` & `carefree-learn-0.4.2/carefree_learn.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: carefree-learn
-Version: 0.4.1
+Version: 0.4.2
 Summary: Deep Learning with PyTorch made easy
 Home-page: https://github.com/carefree0910/carefree-learn
-Download-URL: https://github.com/carefree0910/carefree-learn/archive/v0.4.1.tar.gz
+Download-URL: https://github.com/carefree0910/carefree-learn/archive/v0.4.2.tar.gz
 Author: carefree0910
 Author-email: syameimaru.saki@gmail.com
 Keywords: python machine-learning deep-learning solution PyTorch
 Description-Content-Type: text/markdown
 Provides-Extra: onnx
 Provides-Extra: cv
 Provides-Extra: cv_full
```

### Comparing `carefree-learn-0.4.1/carefree_learn.egg-info/SOURCES.txt` & `carefree-learn-0.4.2/carefree_learn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/carefree_learn.egg-info/requires.txt` & `carefree-learn-0.4.2/carefree_learn.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/__init__.py` & `carefree-learn-0.4.2/cflearn/__init__.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/api/api.py` & `carefree-learn-0.4.2/cflearn/api/api.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/api/cv/diffusion.py` & `carefree-learn-0.4.2/cflearn/api/cv/diffusion.py`

 * *Files 2% similar despite different names*

```diff
@@ -577,25 +577,27 @@
     def txt2img_inpainting(
         self,
         txt: Union[str, List[str]],
         image: Union[str, Image.Image],
         mask: Union[str, Image.Image],
         export_path: Optional[str] = None,
         *,
+        seed: Optional[int] = None,
         reference: Optional[Union[str, Image.Image]] = None,
         reference_fidelity: float = 0.2,
         anchor: int = 64,
         max_wh: int = 512,
         num_samples: Optional[int] = None,
         num_steps: Optional[int] = None,
         clip_output: bool = True,
         keep_original: bool = False,
         use_raw_inpainting: bool = False,
         raw_inpainting_fidelity: float = 0.2,
         callback: Optional[Callable[[Tensor], Tensor]] = None,
+        use_latent_guidance: bool = False,
         verbose: bool = True,
         **kwargs: Any,
     ) -> Tensor:
         if use_raw_inpainting:
             image_res = read_image(image, max_wh, anchor=anchor)
             mask = read_image(mask, max_wh, anchor=anchor, to_mask=True).image
             z = z_ref = self._get_z(image_res.image)
@@ -625,35 +627,58 @@
             max_wh,
             anchor,
             lambda remained_mask, img: np.where(remained_mask, img, 0.5),
             lambda bool_mask: torch.from_numpy(bool_mask),
         )
         # sampling
         with switch_sampler_context(self, kwargs.get("sampler")):
+            # calculate `z_ref` stuffs based on `use_image_guidance`
+            if not use_latent_guidance:
+                z_ref = z_ref_mask = z_ref_noise = None
+            else:
+                z_ref = self._get_z(res.image_res.image)
+                z_ref_mask = 1.0 - F.interpolate(
+                    torch.from_numpy(res.mask).to(z_ref),
+                    z_ref.shape[-2:],
+                    mode="bicubic",
+                )
+                if seed is not None:
+                    seed_everything(seed)
+                z_ref_noise = torch.randn_like(z_ref)
+                reference = res.image_res.original
+            # calculate `z` based on `reference`
             if reference is None:
                 z = None
                 size = tuple(
                     map(
                         lambda n: n * self.size_info.factor,
                         res.remained_image_cond.shape[-2:][::-1],
                     )
                 )
             else:
                 size = None
                 z = self._get_z(read_image(reference, max_wh, anchor=anchor).image)
+                if z_ref_mask is not None and z_ref_noise is not None:
+                    z = z * z_ref_mask + z_ref_noise * (1.0 - z_ref_mask)
                 z, _, kwargs = self._q_sample(
                     z,
                     num_steps,
                     reference_fidelity,
+                    seed,
                     **kwargs,
                 )
+            # core
             sampled = self.sample(
                 num_samples,
                 export_path,
+                seed=seed,
                 z=z,
+                z_ref=z_ref,
+                z_ref_mask=z_ref_mask,
+                z_ref_noise=z_ref_noise,
                 size=size,  # type: ignore
                 original_size=res.image_res.original_size,
                 alpha=res.image_res.alpha,
                 cond=txt_list,
                 cond_concat=torch.cat([res.mask_cond, res.remained_image_cond], dim=1),
                 num_steps=num_steps,
                 clip_output=clip_output,
@@ -910,19 +935,19 @@
                         self.lora_checkpoints = api.m.get_lora_checkpoints()
                         api.m.cleanup_lora()
 
             def __enter__(self) -> DDPM:
                 return self.api.m
 
             def __exit__(self, exc_type: Any, exc_val: Any, exc_tb: Any) -> None:
-                self.api.m.control_model = self.m_ctrl
-                self.api.m.condition_model = self.m_cond
                 if self.lora_checkpoints is not None:
                     assert isinstance(self.api.m, StableDiffusion)
                     self.api.m.restore_lora_from(self.lora_checkpoints)
+                self.api.m.control_model = self.m_ctrl
+                self.api.m.condition_model = self.m_cond
 
         return _(self)
 
     # lora
 
     def load_sd_lora(self, key: str, *, path: str) -> None:
         if not isinstance(self.m, StableDiffusion):
@@ -1148,24 +1173,25 @@
         mask_image_fn: Callable[[np.ndarray, np.ndarray], np.ndarray],
         mask_cond_fn: Callable[[np.ndarray], Tensor],
     ) -> MaskedCond:
         # handle mask stuffs
         image_res = read_image(image, max_wh, anchor=anchor)
         mask_res = read_image(mask, max_wh, anchor=anchor, to_mask=True)
         mask = mask_res.image
-        bool_mask = mask >= 0.5
+        bool_mask = np.round(mask) >= 0.5
         remained_mask = (~bool_mask).astype(np.float16 if self.use_half else np.float32)
         remained_image = mask_image_fn(remained_mask, image_res.image)
         # construct condition tensor
         remained_cond = self._get_z(remained_image)
         latent_shape = remained_cond.shape[-2:]
-        mask_cond = mask_cond_fn(bool_mask)
-        mask_cond = mask_cond.to(torch.float16 if self.use_half else torch.float32)
-        mask_cond = mask_cond.to(self.device)
+        mask_cond = mask_cond_fn(bool_mask).to(torch.float32)
         mask_cond = F.interpolate(mask_cond, size=latent_shape)
+        if self.use_half:
+            mask_cond = mask_cond.half()
+        mask_cond = mask_cond.to(self.device)
         return MaskedCond(
             image_res,
             mask_res,
             mask,
             remained_image,
             remained_mask,
             mask_cond,
@@ -1173,15 +1199,15 @@
         )
 
     def _q_sample(
         self,
         z: Tensor,
         num_steps: Optional[int],
         fidelity: float,
-        seed: int,
+        seed: Optional[int],
         variations: Optional[List[Tuple[int, float]]] = None,
         variation_seed: Optional[int] = None,
         variation_strength: Optional[float] = None,
         **kwargs: Any,
     ) -> Tuple[Tensor, Tensor, Dict[str, Any]]:
         if num_steps is None:
             num_steps = self.sampler.default_steps
@@ -1232,32 +1258,40 @@
                 num_steps=num_steps,
                 clip_output=clip_output,
                 verbose=verbose,
                 **kwargs,
             )
 
 
-def offset_cnet_weights(d: tensor_dict_type, api: DiffusionAPI) -> tensor_dict_type:
+def offset_cnet_weights(
+    d: tensor_dict_type,
+    *,
+    api: Optional[DiffusionAPI] = None,
+    base_md: Optional[tensor_dict_type] = None,
+) -> tensor_dict_type:
     with open(download_static("sd_mapping", extension="json"), "r") as f:
         mapping = json.load(f)
     with open(download_static("sd_controlnet_mapping", extension="json"), "r") as f:
         c_mapping = json.load(f)
     rev_c_mapping = {v: k for k, v in c_mapping.items()}
     nd = shallow_copy_dict(d)
-    with api.load_context() as m:
-        md = m.state_dict()
-    device = list(md.values())[0].device
+    if base_md is None:
+        if api is None:
+            raise ValueError("Either `api` or `md` must be provided.")
+        with api.load_context() as m:
+            base_md = m.state_dict()
+    device = list(base_md.values())[0].device
     nd = {k: v.to(device) for k, v in nd.items()}
     for k, v in nd.items():
         rev_k = rev_c_mapping[k]
         original_k = f"model.diffusion_model.{rev_k.split('.', 1)[1]}"
         mk = mapping.get(original_k)
         if mk is None:
             continue
-        mv = md[mk].to(v)
+        mv = base_md[mk].to(v)
         # inpainting workaround
         if k == "input_blocks.0.0.weight" and mv.shape[1] == 9:
             mv = mv[:, :4]
         nd[k] = v + mv
     return nd
 
 
@@ -1419,15 +1453,19 @@
         root = os.path.join(OPT.cache_dir, DLZoo.model_dir)
         for hint, tag in hints2tags.items():
             self.controlnet_weights[hint] = torch.load(download_model(tag, root=root))
 
     def prepare_control_defaults(self) -> None:
         self.prepare_control(self.control_defaults)
 
-    def switch_control(self, *hints: ControlNetHints) -> None:
+    def switch_control(
+        self,
+        *hints: ControlNetHints,
+        base_md: Optional[tensor_dict_type] = None,
+    ) -> None:
         if self.m.control_model is None:
             raise ValueError("`control_model` is not built yet")
 
         hints_list = list(hints)
         if len(hints_list) > self.num_pool:
             print_warning(
                 f"number of target hints ({len(hints_list)}) exceeds "
@@ -1450,14 +1488,15 @@
 
         sorted_target = sorted(target)
         loaded_list = [self.loaded[hint] for hint in sorted_target]
         base_list = [self.base_sd_versions.get(hint) for hint in sorted_target]
         need_offset_list = [
             base is None
             or self.current_sd_version is None
+            or base_md is not None
             or get_sd_tag(base) != get_sd_tag(self.current_sd_version)
             for base in base_list
         ]
         if all(loaded_list) and not any(need_offset_list):
             return
         iterator = zip(loaded_list, sorted_target, need_offset_list)
         for loaded, hint, need_offset in iterator:
@@ -1466,19 +1505,23 @@
             d = self.controlnet_weights.get(hint)
             if d is None:
                 raise ValueError(
                     f"cannot find ControlNet weights called '{hint}', "
                     f"available weights are: {', '.join(self.available_control_hints)}"
                 )
             if need_offset:
-                d = offset_cnet_weights(d, self)
+                d = offset_cnet_weights(d, api=self, base_md=base_md)
             self.m.load_control_net_with(hint, d)
             self.loaded[hint] = True
-            if self.current_sd_version is not None:
-                self.base_sd_versions[hint] = self.current_sd_version
+            # if `base_md` is provided, should reset cache settings
+            if base_md is not None:
+                self.base_sd_versions.pop(hint, None)
+            else:
+                if self.current_sd_version is not None:
+                    self.base_sd_versions[hint] = self.current_sd_version
 
     def prepare_annotator(self, hint: ControlNetHints) -> None:
         if hint not in self.annotators:
             annotator_class = self.annotator_classes.get(hint)
             if annotator_class is None:
                 raise ValueError(f"annotator for '{hint}' is not implemented")
             annotator = annotator_class(self.device)
```

### Comparing `carefree-learn-0.4.1/cflearn/api/cv/third_party/blip.py` & `carefree-learn-0.4.2/cflearn/api/cv/third_party/blip.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/api/cv/third_party/iharm/api.py` & `carefree-learn-0.4.2/cflearn/api/cv/third_party/iharm/api.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/api/cv/third_party/iharm/inference/predictor.py` & `carefree-learn-0.4.2/cflearn/api/cv/third_party/iharm/inference/predictor.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/api/cv/third_party/iharm/inference/transforms.py` & `carefree-learn-0.4.2/cflearn/api/cv/third_party/iharm/inference/transforms.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/api/cv/third_party/iharm/mconfigs/backboned.py` & `carefree-learn-0.4.2/cflearn/api/cv/third_party/iharm/mconfigs/backboned.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/api/cv/third_party/iharm/mconfigs/base.py` & `carefree-learn-0.4.2/cflearn/api/cv/third_party/iharm/mconfigs/base.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/api/cv/third_party/iharm/model/backboned/deeplab.py` & `carefree-learn-0.4.2/cflearn/api/cv/third_party/iharm/model/backboned/deeplab.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/api/cv/third_party/iharm/model/backboned/hrnet.py` & `carefree-learn-0.4.2/cflearn/api/cv/third_party/iharm/model/backboned/hrnet.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/api/cv/third_party/iharm/model/backboned/ih_model.py` & `carefree-learn-0.4.2/cflearn/api/cv/third_party/iharm/model/backboned/ih_model.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/api/cv/third_party/iharm/model/base/dih_model.py` & `carefree-learn-0.4.2/cflearn/api/cv/third_party/iharm/model/base/dih_model.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/api/cv/third_party/iharm/model/base/iseunet_v1.py` & `carefree-learn-0.4.2/cflearn/api/cv/third_party/iharm/model/base/iseunet_v1.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/api/cv/third_party/iharm/model/base/ssam_model.py` & `carefree-learn-0.4.2/cflearn/api/cv/third_party/iharm/model/base/ssam_model.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/api/cv/third_party/iharm/model/modeling/basic_blocks.py` & `carefree-learn-0.4.2/cflearn/api/cv/third_party/iharm/model/modeling/basic_blocks.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/api/cv/third_party/iharm/model/modeling/conv_autoencoder.py` & `carefree-learn-0.4.2/cflearn/api/cv/third_party/iharm/model/modeling/conv_autoencoder.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/api/cv/third_party/iharm/model/modeling/deeplab_v3.py` & `carefree-learn-0.4.2/cflearn/api/cv/third_party/iharm/model/modeling/deeplab_v3.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/api/cv/third_party/iharm/model/modeling/hrnet_ocr.py` & `carefree-learn-0.4.2/cflearn/api/cv/third_party/iharm/model/modeling/hrnet_ocr.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/api/cv/third_party/iharm/model/modeling/ocr.py` & `carefree-learn-0.4.2/cflearn/api/cv/third_party/iharm/model/modeling/ocr.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/api/cv/third_party/iharm/model/modeling/resnet.py` & `carefree-learn-0.4.2/cflearn/api/cv/third_party/iharm/model/modeling/resnet.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/api/cv/third_party/iharm/model/modeling/resnetv1b.py` & `carefree-learn-0.4.2/cflearn/api/cv/third_party/iharm/model/modeling/resnetv1b.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/api/cv/third_party/iharm/model/modeling/unet.py` & `carefree-learn-0.4.2/cflearn/api/cv/third_party/iharm/model/modeling/unet.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/api/cv/third_party/iharm/model/ops.py` & `carefree-learn-0.4.2/cflearn/api/cv/third_party/iharm/model/ops.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/api/cv/third_party/isnet.py` & `carefree-learn-0.4.2/cflearn/api/cv/third_party/isnet.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/api/cv/third_party/lama.py` & `carefree-learn-0.4.2/cflearn/api/cv/third_party/lama.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/api/cv/third_party/midas/api.py` & `carefree-learn-0.4.2/cflearn/api/cv/third_party/midas/api.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/api/cv/third_party/midas/core/blocks.py` & `carefree-learn-0.4.2/cflearn/api/cv/third_party/midas/core/blocks.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/api/cv/third_party/midas/core/dpt_depth.py` & `carefree-learn-0.4.2/cflearn/api/cv/third_party/midas/core/dpt_depth.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/api/cv/third_party/midas/core/midas_net.py` & `carefree-learn-0.4.2/cflearn/api/cv/third_party/midas/core/midas_net.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/api/cv/third_party/midas/core/midas_net_custom.py` & `carefree-learn-0.4.2/cflearn/api/cv/third_party/midas/core/midas_net_custom.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/api/cv/third_party/midas/core/transforms.py` & `carefree-learn-0.4.2/cflearn/api/cv/third_party/midas/core/transforms.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/api/cv/third_party/midas/core/vit.py` & `carefree-learn-0.4.2/cflearn/api/cv/third_party/midas/core/vit.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/api/cv/third_party/midas/utils.py` & `carefree-learn-0.4.2/cflearn/api/cv/third_party/midas/utils.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/api/cv/third_party/mlsd/api.py` & `carefree-learn-0.4.2/cflearn/api/cv/third_party/mlsd/api.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/api/cv/third_party/mlsd/models/mbv2_mlsd_large.py` & `carefree-learn-0.4.2/cflearn/api/cv/third_party/mlsd/models/mbv2_mlsd_large.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/api/cv/third_party/mlsd/models/mbv2_mlsd_tiny.py` & `carefree-learn-0.4.2/cflearn/api/cv/third_party/mlsd/models/mbv2_mlsd_tiny.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/api/cv/third_party/mlsd/utils.py` & `carefree-learn-0.4.2/cflearn/api/cv/third_party/mlsd/utils.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/api/cv/third_party/openpose/api.py` & `carefree-learn-0.4.2/cflearn/api/cv/third_party/openpose/api.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/api/cv/third_party/openpose/body.py` & `carefree-learn-0.4.2/cflearn/api/cv/third_party/openpose/body.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/api/cv/third_party/openpose/hand.py` & `carefree-learn-0.4.2/cflearn/api/cv/third_party/openpose/hand.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/api/cv/third_party/openpose/model.py` & `carefree-learn-0.4.2/cflearn/api/cv/third_party/openpose/model.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/api/cv/third_party/openpose/util.py` & `carefree-learn-0.4.2/cflearn/api/cv/third_party/openpose/util.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/api/cv/third_party/prompt.py` & `carefree-learn-0.4.2/cflearn/api/cv/third_party/prompt.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/api/cv/translator.py` & `carefree-learn-0.4.2/cflearn/api/cv/translator.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/api/ml/ddr.py` & `carefree-learn-0.4.2/cflearn/api/ml/ddr.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/api/schema.py` & `carefree-learn-0.4.2/cflearn/api/schema.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/api/utils.py` & `carefree-learn-0.4.2/cflearn/api/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
         device: torch.device,
         *,
         use_amp: bool = False,
         use_half: bool = False,
     ):
         if use_amp and use_half:
             raise ValueError("`use_amp` & `use_half` should not be True simultaneously")
-        self.m = m
+        self.m = m.eval().requires_grad_(False)
         self.device = device
         self.use_amp = use_amp
         self.use_half = use_half
 
     def to(
         self,
         device: torch.device,
```

### Comparing `carefree-learn-0.4.1/cflearn/api/zoo/__init__.py` & `carefree-learn-0.4.2/cflearn/api/zoo/__init__.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/callbacks/classification.py` & `carefree-learn-0.4.2/cflearn/callbacks/classification.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/callbacks/general.py` & `carefree-learn-0.4.2/cflearn/callbacks/general.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/callbacks/generator.py` & `carefree-learn-0.4.2/cflearn/callbacks/generator.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/constants.py` & `carefree-learn-0.4.2/cflearn/constants.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/data/array.py` & `carefree-learn-0.4.2/cflearn/data/array.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/data/blocks/cv/crop.py` & `carefree-learn-0.4.2/cflearn/data/blocks/cv/crop.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/data/blocks/cv/image_folder.py` & `carefree-learn-0.4.2/cflearn/data/blocks/cv/image_folder.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/data/blocks/cv/normalize.py` & `carefree-learn-0.4.2/cflearn/data/blocks/cv/normalize.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/data/blocks/cv/to_numpy.py` & `carefree-learn-0.4.2/cflearn/data/blocks/cv/to_numpy.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/data/blocks/cv/tuple_to_batch.py` & `carefree-learn-0.4.2/cflearn/data/blocks/cv/tuple_to_batch.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/data/blocks/ml/file.py` & `carefree-learn-0.4.2/cflearn/data/blocks/ml/file.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/data/blocks/ml/gather.py` & `carefree-learn-0.4.2/cflearn/data/blocks/ml/gather.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/data/blocks/ml/nan_handler.py` & `carefree-learn-0.4.2/cflearn/data/blocks/ml/nan_handler.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/data/blocks/ml/preprocessor.py` & `carefree-learn-0.4.2/cflearn/data/blocks/ml/preprocessor.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/data/blocks/ml/recognizer.py` & `carefree-learn-0.4.2/cflearn/data/blocks/ml/recognizer.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/data/blocks/ml/splitter.py` & `carefree-learn-0.4.2/cflearn/data/blocks/ml/splitter.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/data/ml/api.py` & `carefree-learn-0.4.2/cflearn/data/ml/api.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/data/ml/datasets.py` & `carefree-learn-0.4.2/cflearn/data/ml/datasets.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/data/pytorch/api.py` & `carefree-learn-0.4.2/cflearn/data/pytorch/api.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/data/pytorch/datasets.py` & `carefree-learn-0.4.2/cflearn/data/pytorch/datasets.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/data/utils.py` & `carefree-learn-0.4.2/cflearn/data/utils.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/dist/ml/experiment.py` & `carefree-learn-0.4.2/cflearn/dist/ml/experiment.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/dist/ml/runs/_utils.py` & `carefree-learn-0.4.2/cflearn/dist/ml/runs/_utils.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/dist/ml/task.py` & `carefree-learn-0.4.2/cflearn/dist/ml/task.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/inference.py` & `carefree-learn-0.4.2/cflearn/inference.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/losses/basic.py` & `carefree-learn-0.4.2/cflearn/losses/basic.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/losses/gan.py` & `carefree-learn-0.4.2/cflearn/losses/gan.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/losses/lpips.py` & `carefree-learn-0.4.2/cflearn/losses/lpips.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/losses/vae.py` & `carefree-learn-0.4.2/cflearn/losses/vae.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/metrics.py` & `carefree-learn-0.4.2/cflearn/metrics.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/misc/available.json` & `carefree-learn-0.4.2/cflearn/misc/available.json`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/misc/mixins.py` & `carefree-learn-0.4.2/cflearn/misc/mixins.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/misc/toolkit.py` & `carefree-learn-0.4.2/cflearn/misc/toolkit.py`

 * *Files 0% similar despite different names*

```diff
@@ -929,15 +929,16 @@
         if self._to_train is not None:
             self._module.train(mode=self._training)
         if self._inference_context is not None:
             self._inference_context.__exit__(exc_type, exc_val, exc_tb)
         if self._grad_context is not None:
             self._grad_context.__exit__(exc_type, exc_val, exc_tb)
         for p, v in self._cache.items():
-            p.requires_grad_(v)
+            if p.requires_grad != v:
+                p.requires_grad_(v)
 
 
 class train_context(mode_context):
     """
     Useful when we need to get gradients with our PyTorch model during evaluating.
     """
```

### Comparing `carefree-learn-0.4.1/cflearn/models/bases.py` & `carefree-learn-0.4.2/cflearn/models/bases.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/models/cv/ae/common.py` & `carefree-learn-0.4.2/cflearn/models/cv/ae/common.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/models/cv/ae/kl.py` & `carefree-learn-0.4.2/cflearn/models/cv/ae/kl.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/models/cv/ae/vq.py` & `carefree-learn-0.4.2/cflearn/models/cv/ae/vq.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/models/cv/classifier/vanilla.py` & `carefree-learn-0.4.2/cflearn/models/cv/classifier/vanilla.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/models/cv/decoder/attn.py` & `carefree-learn-0.4.2/cflearn/models/cv/decoder/attn.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/models/cv/decoder/schema.py` & `carefree-learn-0.4.2/cflearn/models/cv/decoder/schema.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/models/cv/decoder/style_gan.py` & `carefree-learn-0.4.2/cflearn/models/cv/decoder/style_gan.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/models/cv/decoder/style_gan_v2.py` & `carefree-learn-0.4.2/cflearn/models/cv/decoder/style_gan_v2.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/models/cv/decoder/vanilla.py` & `carefree-learn-0.4.2/cflearn/models/cv/decoder/vanilla.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/models/cv/decoder/vqgan.py` & `carefree-learn-0.4.2/cflearn/models/cv/decoder/vqgan.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/models/cv/diffusion/cond_models/clip.py` & `carefree-learn-0.4.2/cflearn/models/cv/diffusion/cond_models/clip.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/models/cv/diffusion/cond_models/rescaler.py` & `carefree-learn-0.4.2/cflearn/models/cv/diffusion/cond_models/rescaler.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/models/cv/diffusion/cond_models/schema.py` & `carefree-learn-0.4.2/cflearn/models/cv/diffusion/cond_models/schema.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/models/cv/diffusion/ddpm.py` & `carefree-learn-0.4.2/cflearn/models/cv/diffusion/ddpm.py`

 * *Files 6% similar despite different names*

```diff
@@ -163,28 +163,24 @@
         batch: tensor_dict_type,
         forward_results: Union[tensor_dict_type, List[tensor_dict_type]],
     ) -> None:
         if m.training and m.unet_ema is not None:
             m.unet_ema()
 
 
-TControlScales = Union[float, List[float]]
-TTControlScales = Union[TControlScales, Dict[str, TControlScales]]
-
-
 @ModelWithCustomSteps.register("ddpm")
 class DDPM(ModelWithCustomSteps, GaussianGeneratorMixin):
     cond_key = "cond"
     noise_key = "noise"
     timesteps_key = "timesteps"
     identity_condition_model = "identity"
 
     sampler: ISampler
     control_model: Optional[Union[ControlNet, nn.ModuleDict]]
-    control_scales: Optional[Union[List[float], Dict[str, List[float]]]]
+    control_scales: Optional[Union[List[float], List[List[float]]]]
 
     def __init__(
         self,
         img_size: int,
         # unet
         in_channels: int,
         out_channels: int,
@@ -511,49 +507,49 @@
                 if not check_hint_start(hint_start):
                     ctrl = None
                 else:
                     ctrl = self.control_model(net, hint, timesteps=timesteps, **cond_kw)
                     if self.control_scales is None:
                         scales = [1.0] * self.num_control_scales
                     else:
-                        if isinstance(self.control_scales, dict):
-                            raise ValueError("`control_scales` should not be dict")
-                        scales = self.control_scales
+                        if isinstance(self.control_scales[0], list):
+                            raise ValueError("`control_scales` should be list of float")
+                        scales = self.control_scales  # type: ignore
                     ctrl = [c * scale for c, scale in zip(ctrl, scales)]
             else:
-                if not isinstance(hint, dict):
-                    raise ValueError("`hint` should be a dict for multi control")
+                if not isinstance(hint, list):
+                    raise ValueError("`hint` should be a list for control settings")
+                if not isinstance(hint_start, list):
+                    raise ValueError("`hint_start` should be a list of Optional[float]")
                 target_keys = set(self.control_model.keys())
-                if set(hint) - target_keys:
-                    msg = f"`hint` should not exceed following keys: {', '.join(sorted(target_keys))}"
+                hint_types = set(pair[0] for pair in hint)
+                if hint_types - target_keys:
+                    msg = f"`hint` ({hint_types}) should not exceed following keys: {', '.join(sorted(target_keys))}"
                     raise ValueError(msg)
-                if hint_start is not None and not isinstance(hint_start, dict):
-                    hint_start = {k: hint_start for k in hint}
                 ctrl = [0.0] * self.num_control_scales
                 any_activated = False
-                for k, k_hint in hint.items():
-                    k_hint_start = None if hint_start is None else hint_start.get(k)
-                    if not check_hint_start(k_hint_start):
+                for i, ((i_type, i_hint), i_start) in enumerate(zip(hint, hint_start)):
+                    if not check_hint_start(i_start):
                         continue
                     any_activated = True
-                    k_cmodel = self.control_model[k]
+                    i_cmodel = self.control_model[i_type]
                     # inpainting workaround
-                    if k_cmodel.in_channels == net.shape[1]:
+                    if i_cmodel.in_channels == net.shape[1]:
                         cnet = net
                     else:
-                        cnet = net[:, : k_cmodel.in_channels]
-                    k_control = k_cmodel(cnet, k_hint, timesteps=timesteps, **cond_kw)
-                    if self.control_scales is not None:
-                        if not isinstance(self.control_scales, dict):
-                            raise ValueError("`control_scales` should be a dict")
-                        k_scales = self.control_scales[k]
+                        cnet = net[:, : i_cmodel.in_channels]
+                    i_control = i_cmodel(cnet, i_hint, timesteps=timesteps, **cond_kw)
+                    if self.control_scales is None:
+                        i_scales = [1.0] * self.num_control_scales
                     else:
-                        k_scales = [1.0] * self.num_control_scales
-                    for i, (k_c, k_scale) in enumerate(zip(k_control, k_scales)):
-                        ctrl[i] += k_c * k_scale
+                        if not isinstance(self.control_scales[i], list):
+                            raise ValueError("`control_scales` should be list of list")
+                        i_scales = self.control_scales[i]  # type: ignore
+                    for j, (j_c, j_scale) in enumerate(zip(i_control, i_scales)):
+                        ctrl[j] += j_c * j_scale
                 if not any_activated:
                     ctrl = None
             cond_kw["control"] = ctrl
             cond_kw["only_mid_control"] = self.only_mid_control
         return self.unet(net, timesteps=timesteps, **cond_kw)
 
     def predict_eps_from_z_and_v(
@@ -613,40 +609,14 @@
         if not isinstance(self.control_model, nn.ModuleDict):
             msg = "`load_control_net_with` is only available when multiple `ControlNet` are used"
             raise ValueError(msg)
         if name not in self.control_model:
             raise ValueError(f"cannot find '{name}' in current models")
         self.control_model[name].load_state_dict(d)
 
-    def set_control_scales(self, scales: TTControlScales) -> None:
-        def _parse(ss: TControlScales) -> List[float]:
-            if isinstance(ss, float):
-                ss = [ss] * self.num_control_scales
-            return ss
-
-        if not isinstance(scales, dict):
-            scales = _parse(scales)
-        else:
-            scales = {k: _parse(v) for k, v in scales.items()}
-        if isinstance(self.control_model, ControlNet):
-            if isinstance(scales, dict):
-                msg = "`scales` should not be dict when only one `ControlNet` is used"
-                raise ValueError(msg)
-            self.control_scales = scales
-        else:
-            if not isinstance(scales, dict):
-                msg = "`scales` should be dict when multiple `ControlNet` are used"
-                raise ValueError(msg)
-            if self.control_model is not None:
-                target_keys = set(self.control_model.keys())
-                if set(scales) != target_keys:
-                    msg = f"`scales` should (exactly) have following keys: {', '.join(sorted(target_keys))}"
-                    raise ValueError(msg)
-            self.control_scales = {k: _parse(v) for k, v in scales.items()}
-
     def detach_control_net(self) -> None:
         if self.control_model is not None:
             self.control_model.to("cpu")
             del self.control_model
             self.control_model = None
 
     # internal
```

### Comparing `carefree-learn-0.4.1/cflearn/models/cv/diffusion/ldm.py` & `carefree-learn-0.4.2/cflearn/models/cv/diffusion/ldm.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/models/cv/diffusion/samplers/basic.py` & `carefree-learn-0.4.2/cflearn/models/cv/diffusion/samplers/basic.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/models/cv/diffusion/samplers/ddim.py` & `carefree-learn-0.4.2/cflearn/models/cv/diffusion/samplers/ddim.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/models/cv/diffusion/samplers/k_samplers.py` & `carefree-learn-0.4.2/cflearn/models/cv/diffusion/samplers/k_samplers.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/models/cv/diffusion/samplers/plms.py` & `carefree-learn-0.4.2/cflearn/models/cv/diffusion/samplers/plms.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/models/cv/diffusion/samplers/schema.py` & `carefree-learn-0.4.2/cflearn/models/cv/diffusion/samplers/schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from typing import Any
 from typing import Dict
 from typing import Type
 from typing import Callable
 from typing import Optional
 from typing import Protocol
 from cftool.misc import update_dict
+from cftool.misc import safe_execute
 from cftool.misc import shallow_copy_dict
 from cftool.misc import WithRegister
 
 from ..utils import cond_type
 from ..utils import extract_to
 from ..utils import get_timesteps
 from ..utils import CONCAT_KEY
@@ -167,14 +168,19 @@
         if verbose:
             iterator = tqdm(iterator, desc=f"sampling ({self.__identifier__})")
         # execute
         image = z
         if cond is not None and self.model.condition_model is not None:
             cond = self.model._get_cond(cond)
         for step in iterator:
+            callback = kwargs.get("step_callback")
+            if callback is not None:
+                callback_kw = dict(step=step, num_steps=num_steps, image=image)
+                if not safe_execute(callback, callback_kw):
+                    break
             kw = shallow_copy_dict(self.sample_kwargs)
             update_dict(shallow_copy_dict(kwargs), kw)
             image = self.sample_step(image, cond, step, num_steps, **kw)
             if ref is not None and ref_mask is not None and ref_noise is not None:
                 ref_ts = get_timesteps(num_steps - step - 1, ref.shape[0], z.device)
                 ref_noisy = self.q_sample(ref, ref_ts, ref_noise)
                 image = ref_noisy * ref_mask + image * (1.0 - ref_mask)
```

### Comparing `carefree-learn-0.4.1/cflearn/models/cv/diffusion/samplers/solver.py` & `carefree-learn-0.4.2/cflearn/models/cv/diffusion/samplers/solver.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/models/cv/diffusion/samplers/utils.py` & `carefree-learn-0.4.2/cflearn/models/cv/diffusion/samplers/utils.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/models/cv/diffusion/unet.py` & `carefree-learn-0.4.2/cflearn/models/cv/diffusion/unet.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/models/cv/diffusion/utils.py` & `carefree-learn-0.4.2/cflearn/models/cv/diffusion/utils.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/models/cv/encoder/attn.py` & `carefree-learn-0.4.2/cflearn/models/cv/encoder/attn.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/models/cv/encoder/backbone/api.py` & `carefree-learn-0.4.2/cflearn/models/cv/encoder/backbone/api.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/models/cv/encoder/backbone/core.py` & `carefree-learn-0.4.2/cflearn/models/cv/encoder/backbone/core.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/models/cv/encoder/backbone/models/resnet.py` & `carefree-learn-0.4.2/cflearn/models/cv/encoder/backbone/models/resnet.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/models/cv/encoder/backbone/models/transformer.py` & `carefree-learn-0.4.2/cflearn/models/cv/encoder/backbone/models/transformer.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/models/cv/encoder/backbone/models/vgg.py` & `carefree-learn-0.4.2/cflearn/models/cv/encoder/backbone/models/vgg.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/models/cv/encoder/backbone/register.py` & `carefree-learn-0.4.2/cflearn/models/cv/encoder/backbone/register.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/models/cv/encoder/fnet.py` & `carefree-learn-0.4.2/cflearn/models/cv/encoder/fnet.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/models/cv/encoder/mixer.py` & `carefree-learn-0.4.2/cflearn/models/cv/encoder/mixer.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/models/cv/encoder/perceiver.py` & `carefree-learn-0.4.2/cflearn/models/cv/encoder/perceiver.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/models/cv/encoder/pool_former.py` & `carefree-learn-0.4.2/cflearn/models/cv/encoder/pool_former.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/models/cv/encoder/schema.py` & `carefree-learn-0.4.2/cflearn/models/cv/encoder/schema.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/models/cv/encoder/transformer.py` & `carefree-learn-0.4.2/cflearn/models/cv/encoder/transformer.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/models/cv/encoder/vanilla.py` & `carefree-learn-0.4.2/cflearn/models/cv/encoder/vanilla.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/models/cv/encoder/vqgan.py` & `carefree-learn-0.4.2/cflearn/models/cv/encoder/vqgan.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/models/cv/gan/discriminators.py` & `carefree-learn-0.4.2/cflearn/models/cv/gan/discriminators.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/models/cv/gan/schema.py` & `carefree-learn-0.4.2/cflearn/models/cv/gan/schema.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/models/cv/gan/vanilla.py` & `carefree-learn-0.4.2/cflearn/models/cv/gan/vanilla.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/models/cv/general.py` & `carefree-learn-0.4.2/cflearn/models/cv/general.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/models/cv/translator/rrdb.py` & `carefree-learn-0.4.2/cflearn/models/cv/translator/rrdb.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/models/implicit/siren.py` & `carefree-learn-0.4.2/cflearn/models/implicit/siren.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/models/ml/base.py` & `carefree-learn-0.4.2/cflearn/models/ml/base.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/models/ml/ddr.py` & `carefree-learn-0.4.2/cflearn/models/ml/ddr.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/models/ml/encoders.py` & `carefree-learn-0.4.2/cflearn/models/ml/encoders.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/models/ml/fcnn.py` & `carefree-learn-0.4.2/cflearn/models/ml/fcnn.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/models/ml/linear.py` & `carefree-learn-0.4.2/cflearn/models/ml/linear.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/models/ml/mixed_stacked.py` & `carefree-learn-0.4.2/cflearn/models/ml/mixed_stacked.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/models/ml/nbm.py` & `carefree-learn-0.4.2/cflearn/models/ml/nbm.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/models/ml/ndt.py` & `carefree-learn-0.4.2/cflearn/models/ml/ndt.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/models/ml/rnn.py` & `carefree-learn-0.4.2/cflearn/models/ml/rnn.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/models/ml/wnd.py` & `carefree-learn-0.4.2/cflearn/models/ml/wnd.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/models/multimodal/clip.py` & `carefree-learn-0.4.2/cflearn/models/multimodal/clip.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/models/multimodal/schema.py` & `carefree-learn-0.4.2/cflearn/models/multimodal/schema.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/models/nlp/encoder/transformer.py` & `carefree-learn-0.4.2/cflearn/models/nlp/encoder/transformer.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/models/nlp/tokenizers/clip.py` & `carefree-learn-0.4.2/cflearn/models/nlp/tokenizers/clip.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/models/nlp/tokenizers/schema.py` & `carefree-learn-0.4.2/cflearn/models/nlp/tokenizers/schema.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/models/nlp/transformers/core.py` & `carefree-learn-0.4.2/cflearn/models/nlp/transformers/core.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/models/nlp/transformers/opus.py` & `carefree-learn-0.4.2/cflearn/models/nlp/transformers/opus.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/models/nlp/transformers/simbert.py` & `carefree-learn-0.4.2/cflearn/models/nlp/transformers/simbert.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/models/schemas/custom.py` & `carefree-learn-0.4.2/cflearn/models/schemas/custom.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/models/schemas/cv.py` & `carefree-learn-0.4.2/cflearn/models/schemas/cv.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/modules/blocks/__init__.py` & `carefree-learn-0.4.2/cflearn/modules/blocks/__init__.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/modules/blocks/activations.py` & `carefree-learn-0.4.2/cflearn/modules/blocks/activations.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/modules/blocks/attentions.py` & `carefree-learn-0.4.2/cflearn/modules/blocks/attentions.py`

 * *Files 1% similar despite different names*

```diff
@@ -189,14 +189,16 @@
         *,
         hw: Optional[Tuple[int, int]] = None,
         mask: Optional[Tensor] = None,
         require_weights: bool = False,
         determinate: bool = False,
     ) -> AttentionOutput:
         qkv_inp = q, k, v
+        if self.hook is not None:
+            qkv_inp = self.hook.before_forward(qkv_inp)
         # `mask` represents slots which will be zeroed
         if self.qkv_same:
             qkv = F.linear(q, self.in_w, self.qkv_bias)
             if not determinate:
                 q, k, v = qkv.chunk(3, dim=-1)
             else:
                 qkv = qkv.view(-1, int(q.shape[1]), 3, self.embed_dim)
@@ -223,15 +225,15 @@
             # B, Nk, Dk -> B, Nk, D
             k = F.linear(self._reduce(k, hw), self.k_w, k_bias)
             # B, Nv, Dv -> B, Nv, D
             v = F.linear(self._reduce(v, hw), self.v_w, v_bias)
         if self.hook is not None:
             if self.reduction is not None:
                 raise ValueError("currently `hook` does not support `reduction`")
-            q, k, v = self.hook.callback(qkv_inp, (q, k, v))
+            q, k, v = self.hook.after_forward(qkv_inp, (q, k, v))
         q, k, v = map(self.activation, [q, k, v])
         # B, N*, D -> B * N_head, N*, D_head
         q, k, v = map(self._to_heads, [q, k, v], [determinate] * 3)
         if mask is not None:
             # B, Nq, Nk -> B, N_head, Nq, Nk
             mask = mask.repeat(self.num_heads, 1, 1)
             mask = mask.view(-1, self.num_heads, *mask.shape[1:])
```

### Comparing `carefree-learn-0.4.1/cflearn/modules/blocks/common.py` & `carefree-learn-0.4.2/cflearn/modules/blocks/common.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/modules/blocks/convs/basic.py` & `carefree-learn-0.4.2/cflearn/modules/blocks/convs/basic.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/modules/blocks/convs/residual.py` & `carefree-learn-0.4.2/cflearn/modules/blocks/convs/residual.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/modules/blocks/customs.py` & `carefree-learn-0.4.2/cflearn/modules/blocks/customs.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,29 +76,31 @@
 
     @property
     def bias(self) -> Optional[Tensor]:
         return self.b if self.linear is None else self.linear.bias
 
     def forward(self, net: Tensor) -> Tensor:
         inp = net
+        if self.hook is not None:
+            inp = self.hook.before_forward(inp)
         if self.linear is not None:
             weight = self.linear.weight
             if self.pruner is not None:
                 weight = self.pruner(weight)
             net = F.linear(net, weight, self.linear.bias)
         else:
             w1, w2 = self.w1, self.w2
             if self.pruner1 is not None:
                 w1 = self.pruner1(w1)
             if self.pruner2 is not None:
                 w2 = self.pruner2(w2)
             net = F.linear(net, w1)
             net = F.linear(net, w2, self.b)
         if self.hook is not None:
-            net = self.hook.callback(inp, net)
+            net = self.hook.after_forward(inp, net)
         return net
 
     def init_weights_with(self, w_init_fn: Callable[[Tensor], None]) -> None:
         with torch.no_grad():
             if self.linear is not None:
                 w_init_fn(self.linear.weight.data)
             elif self.w1 is not None and self.w2 is not None:
```

### Comparing `carefree-learn-0.4.1/cflearn/modules/blocks/high_level.py` & `carefree-learn-0.4.2/cflearn/modules/blocks/high_level.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/modules/blocks/hijacks.py` & `carefree-learn-0.4.2/cflearn/modules/blocks/hijacks.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,20 +3,23 @@
 from torch import nn
 from torch import Tensor
 from typing import Any
 from typing import Set
 from typing import Dict
 from typing import List
 from typing import Union
+from typing import Generic
+from typing import TypeVar
 from typing import Optional
 from typing import NamedTuple
+from cftool.misc import print_info
+from cftool.misc import print_warning
 from cftool.misc import shallow_copy_dict
 from cftool.array import tensor_dict_type
 
-from .hooks import TQKV
 from .hooks import IHook
 from .hooks import IBasicHook
 from .hooks import IAttentionHook
 from .hooks import MultiHooks
 from .customs import Linear
 
 
@@ -34,17 +37,19 @@
         self.args = args
         self.kwargs = shallow_copy_dict(kwargs)
         super().__init__(*args, **kwargs)
         self.hook = hook
 
     def forward(self, net: Tensor) -> Tensor:
         inp = net
+        if self.hook is not None:
+            inp = self.hook.before_forward(inp)
         net = super().forward(net)  # type: ignore
         if self.hook is not None:
-            net = self.hook.callback(inp, net)
+            net = self.hook.after_forward(inp, net)
         return net
 
 
 class HijackLinear(IBasicHijackMixin, nn.Linear):
     pass
 
 
@@ -64,50 +69,89 @@
     pass
 
 
 # attention hijacks
 
 
 class IAttention:
+    in_w: Optional[nn.Parameter]
     hook: Optional[IAttentionHook]
     input_dim: int
     embed_dim: int
 
 
 # LoRA
 ## input -> lora_down -> selector -> lora_up -> dropout -> alpha (scale)
 
 
-class ILoRAHook(IBasicHook):
+TLoRA = TypeVar("TLoRA")
+
+
+class ILoRAHook(Generic[TLoRA]):
+    _ms: List[TLoRA]
+    backup: Optional[Tensor] = None
+    injected: bool = False
+
+    @property
+    def m(self) -> TLoRA:
+        return self._ms[0]
+
+    def inject(self, w: nn.Parameter, updown: Tensor, index: Optional[int]) -> None:
+        if self.backup is None and (index is None or index == 0):
+            self.backup = w.data
+        if self.backup is None:
+            w.data = w.data + updown
+        else:
+            w.data = self.backup + updown
+        self.injected = True
+
+
+class ILoRAMappingHook(ILoRAHook[Union[nn.Linear, nn.Conv2d]], IBasicHook):
     rank: int
     lora_down: Union[nn.Linear, nn.Conv2d]
     selector: Union[nn.Identity, nn.Linear, nn.Conv2d]
     lora_up: Union[nn.Linear, nn.Conv2d]
     dropout: nn.Dropout
     alpha: nn.Parameter
+    scale: float = 1.0
 
     @property
-    def scale(self) -> float:
+    def alpha_scale(self) -> float:
         return self.alpha.item() / self.lora_down.weight.shape[0]
 
     def set_scale(self, scale: float) -> None:
-        self.alpha.data.fill_(scale * self.lora_down.weight.shape[0])
+        self.scale = scale
+        self.injected = False
 
-    def callback(self, inp: Tensor, out: Tensor) -> Tensor:
-        lora = self.dropout(self.lora_up(self.selector(self.lora_down(inp))))
-        return out + self.scale * lora
+    def get_updown(self) -> Tensor:
+        up = self.lora_up.weight
+        down = self.lora_down.weight
+        if len(up.shape) == 2 and len(down.shape) == 2:
+            updown = up @ down
+        else:
+            updown = (up[..., 0, 0] @ down[..., 0, 0])[..., None, None]
+        updown = self.scale * self.alpha_scale * updown
+        return updown
+
+    def before_forward(self, inp: Tensor, index: Optional[int] = None) -> Tensor:
+        if not self.injected:
+            weight = self.m.weight
+            updown = self.get_updown()
+            self.inject(weight, updown, index)
+        return inp
 
     @classmethod
-    def create_with(cls, m: IBasicHijackMixin, rank: int) -> "ILoRAHook":
+    def create_with(cls, m: IBasicHijackMixin, rank: int) -> "ILoRAMappingHook":
         self = cls(*m.args, rank=rank, **m.kwargs)
         self.to(m.weight)
+        self._ms = [m]
         return self
 
 
-class LoRALinearHook(ILoRAHook):
+class LoRALinearHook(ILoRAMappingHook):
     def __init__(
         self,
         in_features: int,
         out_features: int,
         *args: Any,
         rank: int = 4,
         dropout: float = 0.1,
@@ -132,15 +176,15 @@
 
     def set_selector(self, diag: Tensor) -> None:
         assert diag.shape == (self.rank,)
         self.selector = nn.Linear(self.rank, self.rank, bias=False)
         self.selector.weight.data = torch.diag(diag).to(self.lora_up.weight.data)
 
 
-class LoRAConvHook(ILoRAHook):
+class LoRAConvHook(ILoRAMappingHook):
     def __init__(
         self,
         in_channels: int,
         out_channels: int,
         kernel_size: int,
         stride: int = 1,
         padding: int = 0,
@@ -193,42 +237,46 @@
             stride=1,
             padding=0,
             bias=False,
         )
         self.selector.weight.data = torch.diag(diag).to(self.lora_up.weight.data)
 
 
-class LoRAAttentionHook(IAttentionHook):
+class LoRAAttentionHook(ILoRAHook[IAttention], IAttentionHook):
     def __init__(self, in_features: int, out_features: int, *, rank: int) -> None:
         super().__init__()
         self.to_q = LoRALinearHook(in_features, out_features, rank=rank)
         self.to_k = LoRALinearHook(in_features, out_features, rank=rank)
         self.to_v = LoRALinearHook(in_features, out_features, rank=rank)
 
     def set_scale(self, scale: float) -> None:
         self.to_q.set_scale(scale)
         self.to_k.set_scale(scale)
         self.to_v.set_scale(scale)
+        self.injected = False
 
-    def callback(self, qkv_inp: TQKV, qkv_out: TQKV) -> TQKV:
-        q_in, k_in, v_in = qkv_inp
-        q, k, v = qkv_out
-        q = self.to_q.callback(q_in, q)
-        k = self.to_k.callback(k_in, k)
-        v = self.to_v.callback(v_in, v)
-        return q, k, v
+    def before_forward(self, inp: Tensor, index: Optional[int] = None) -> Tensor:
+        if not self.injected:
+            in_w = self.m.in_w
+            hooks = [self.to_q, self.to_k, self.to_v]
+            updown = torch.vstack([h.get_updown() for h in hooks])
+            assert in_w is not None, "should be self_attn in lora"
+            self.inject(in_w, updown, index)
+        return inp
 
     @classmethod
     def create_with(cls, m: IAttention, rank: int) -> "LoRAAttentionHook":
-        return cls(m.input_dim, m.embed_dim, rank=rank)
+        self = cls(m.input_dim, m.embed_dim, rank=rank)
+        self._ms = [m]
+        return self
 
 
 class LoRAPack(NamedTuple):
     rank: int
-    hooks: Dict[str, Union[ILoRAHook, LoRAAttentionHook]]
+    hooks: Dict[str, Union[ILoRAMappingHook, LoRAAttentionHook]]
 
 
 class LoRAManager:
     def __init__(self) -> None:
         self.m = None
         self.injected = False
         self.lora_packs: Dict[str, LoRAPack] = {}
@@ -255,19 +303,29 @@
         merged = {k: v[0] if len(v) == 1 else MultiHooks(v) for k, v in hooks.items()}
         return LoRAPack(rank, merged)
 
     def load_pack_with(self, key: str, d: tensor_dict_type) -> None:
         pack = self.lora_packs.get(key)
         if pack is None:
             raise ValueError(f"cannot find '{key}' pack")
+        num_source = len(d)
+        num_prepared = 0
         for k, v in pack.hooks.items():
             for n, p in v.named_parameters():
                 tp = d[f"{k}.{n}"]
                 assert p.data.shape == tp.shape
                 p.data = tp.to(p.data)
+                num_prepared += 1
+        if num_source == num_prepared:
+            print_info(f"{num_prepared} weights are loaded")
+        else:
+            print_warning(
+                f"only {num_prepared}/{num_source} weights are loaded, "
+                "which could lead to unexpected behaviours"
+            )
 
     def prepare(
         self,
         m: nn.Module,
         *,
         key: str,
         rank: int,
@@ -297,32 +355,57 @@
         if m is not self.m:
             raise ValueError("prepared module does not match the incoming module.")
         pack = self.build_pack(*keys)
         if pack is None:
             raise ValueError(f"cannot build LoRAPack with {', '.join(keys)}")
         hooks = pack.hooks
         pivot = list(m.parameters())[0]
+        num_hooks = len(hooks)
+        num_injected = 0
         for name, module in m.named_modules():
             hook = hooks.get(name)
             if hook is not None:
                 if not isinstance(module, IHijackMixin):
                     msg = f"`hook` is found for '{name}' but it is not a Hijack module"
                     raise ValueError(msg)
                 hook.to(pivot)
                 module.hook = hook
+                num_injected += 1
+        if num_hooks == num_injected:
+            print_info(f"{num_injected} hooks are injected")
+        else:
+            print_warning(
+                f"only {num_injected}/{num_hooks} hooks are injected, "
+                "which could lead to unexpected behaviours"
+            )
         self.injected = True
 
     def cleanup(self, m: nn.Module) -> None:
         if not self.injected:
             raise ValueError("LoRA is not injected, please call `inject` first.")
         if m is not self.m:
             raise ValueError("injected module does not match the incoming module.")
         for module in m.modules():  # type: ignore
             if isinstance(module, IHijackMixin):
-                module.hook = None
+                hook = module.hook
+                if not isinstance(hook, MultiHooks):
+                    hooks = [hook]
+                else:
+                    hooks = hook.hooks
+                for h in hooks:
+                    if not isinstance(h, ILoRAHook):
+                        continue
+                    h.injected = False
+                    module.hook = None
+                    if h.backup is not None:
+                        if isinstance(module, IAttention):
+                            module.in_w.data = h.backup  # type: ignore
+                        else:
+                            module.weight.data = h.backup  # type: ignore
+                        h.backup = None
         self.injected = False
         torch.cuda.empty_cache()
 
     def set_scale(self, key: str, scale: float) -> None:
         pack = self.lora_packs.get(key)
         if pack is None:
             raise ValueError(f"cannot find LoRAPack '{key}'")
```

### Comparing `carefree-learn-0.4.1/cflearn/modules/blocks/hooks.py` & `carefree-learn-0.4.2/cflearn/modules/blocks/hooks.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,40 +1,47 @@
-from abc import abstractmethod
-from abc import ABCMeta
 from torch import nn
 from torch import Tensor
 from typing import Any
 from typing import List
 from typing import Tuple
+from typing import Optional
 from torch.nn import Module
 
 
 TQKV = Tuple[Tensor, Tensor, Tensor]
 
 
-class IHook(Module, metaclass=ABCMeta):
-    @abstractmethod
-    def callback(self, inp: Any, out: Any) -> Any:
-        pass
+class IHook(Module):
+    # modify the `input`
+    ## when `index` is provided, it means the hook is inside a `MultiHooks`
+    def before_forward(self, inp: Any, index: Optional[int] = None) -> Any:
+        return inp
+
+    # modify the `output`
+    def after_forward(self, inp: Any, out: Any) -> Any:
+        return out
 
 
 class IBasicHook(IHook):
-    @abstractmethod
-    def callback(self, inp: Tensor, out: Tensor) -> Tensor:
-        pass
+    def after_forward(self, inp: Tensor, out: Tensor) -> Tensor:
+        return out
 
 
 class IAttentionHook(IHook):
-    @abstractmethod
-    def callback(self, qkv_inp: TQKV, qkv_out: TQKV) -> TQKV:
-        pass
+    def after_forward(self, qkv_inp: TQKV, qkv_out: TQKV) -> TQKV:
+        return qkv_out
 
 
 class MultiHooks(IHook):
     def __init__(self, hooks: List[IHook]) -> None:
         super().__init__()
         self.hooks = nn.ModuleList(hooks)
 
-    def callback(self, inp: Any, out: Any) -> Any:
+    def before_forward(self, inp: Any, index: Optional[int] = None) -> Any:
+        for i, hook in enumerate(self.hooks):
+            inp = hook.before_forward(inp, i)
+        return inp
+
+    def after_forward(self, inp: Any, out: Any) -> Any:
         for hook in self.hooks:
-            out = hook.callback(inp, out)
+            out = hook.after_forward(inp, out)
         return out
```

### Comparing `carefree-learn-0.4.1/cflearn/modules/blocks/implementations/perceiver.py` & `carefree-learn-0.4.2/cflearn/modules/blocks/implementations/perceiver.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/modules/blocks/mappings.py` & `carefree-learn-0.4.2/cflearn/modules/blocks/mappings.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/modules/blocks/mixed_stacks/api.py` & `carefree-learn-0.4.2/cflearn/modules/blocks/mixed_stacks/api.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/modules/blocks/mixed_stacks/channel_mixers.py` & `carefree-learn-0.4.2/cflearn/modules/blocks/mixed_stacks/channel_mixers.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/modules/blocks/mixed_stacks/poolers.py` & `carefree-learn-0.4.2/cflearn/modules/blocks/mixed_stacks/poolers.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/modules/blocks/mixed_stacks/schema.py` & `carefree-learn-0.4.2/cflearn/modules/blocks/mixed_stacks/schema.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/modules/blocks/mixed_stacks/token_mixers.py` & `carefree-learn-0.4.2/cflearn/modules/blocks/mixed_stacks/token_mixers.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/modules/blocks/norms.py` & `carefree-learn-0.4.2/cflearn/modules/blocks/norms.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/modules/blocks/utils.py` & `carefree-learn-0.4.2/cflearn/modules/blocks/utils.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/modules/optimizers.py` & `carefree-learn-0.4.2/cflearn/modules/optimizers.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/modules/schedulers.py` & `carefree-learn-0.4.2/cflearn/modules/schedulers.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/monitors.py` & `carefree-learn-0.4.2/cflearn/monitors.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/parameters.py` & `carefree-learn-0.4.2/cflearn/parameters.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/pipeline/api.py` & `carefree-learn-0.4.2/cflearn/pipeline/api.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/pipeline/blocks/basic.py` & `carefree-learn-0.4.2/cflearn/pipeline/blocks/basic.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/pipeline/blocks/ml.py` & `carefree-learn-0.4.2/cflearn/pipeline/blocks/ml.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/pipeline/blocks/utils.py` & `carefree-learn-0.4.2/cflearn/pipeline/blocks/utils.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/pipeline/core.py` & `carefree-learn-0.4.2/cflearn/pipeline/core.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/pipeline/third_party.py` & `carefree-learn-0.4.2/cflearn/pipeline/third_party.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/schema.py` & `carefree-learn-0.4.2/cflearn/schema.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/scripts/sd.py` & `carefree-learn-0.4.2/cflearn/scripts/sd.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/trainer.py` & `carefree-learn-0.4.2/cflearn/trainer.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/types.py` & `carefree-learn-0.4.2/cflearn/types.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/zoo/configs/ae/kl/f4.json` & `carefree-learn-0.4.2/cflearn/zoo/configs/ae/kl/f4.json`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/zoo/configs/diffusion/ddpm/default.json` & `carefree-learn-0.4.2/cflearn/zoo/configs/diffusion/ddpm/default.json`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/zoo/configs/diffusion/ldm/default.json` & `carefree-learn-0.4.2/cflearn/zoo/configs/diffusion/ldm/default.json`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/zoo/configs/diffusion/ldm/vq.json` & `carefree-learn-0.4.2/cflearn/zoo/configs/diffusion/ldm/vq.json`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/zoo/configs/multimodal/clip/chinese.json` & `carefree-learn-0.4.2/cflearn/zoo/configs/multimodal/clip/chinese.json`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/zoo/core.py` & `carefree-learn-0.4.2/cflearn/zoo/core.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/cflearn/zoo/models/clip.py` & `carefree-learn-0.4.2/cflearn/zoo/models/clip.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.1/setup.py` & `carefree-learn-0.4.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 from setuptools import find_packages
 
 
-VERSION = "0.4.1"
+VERSION = "0.4.2"
 DESCRIPTION = "Deep Learning with PyTorch made easy"
 with open("README.md", encoding="utf-8") as f:
     LONG_DESCRIPTION = f.read()
 
 cv_requires = [
     "ftfy",
     "lmdb",
```

