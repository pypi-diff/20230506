# Comparing `tmp/hcpdiff-0.2.2.tar.gz` & `tmp/hcpdiff-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hcpdiff-0.2.2.tar", last modified: Sat Apr 29 03:57:22 2023, max compression
+gzip compressed data, was "hcpdiff-0.3.0.tar", last modified: Sat May  6 03:28:25 2023, max compression
```

## Comparing `hcpdiff-0.2.2.tar` & `hcpdiff-0.3.0.tar`

### file list

```diff
@@ -1,94 +1,100 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 03:57:22.328503 hcpdiff-0.2.2/
--rw-rw-rw-   0        0        0    11558 2023-04-11 12:44:40.000000 hcpdiff-0.2.2/LICENSE
--rw-rw-rw-   0        0        0     5507 2023-04-29 03:57:22.328503 hcpdiff-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     4770 2023-04-29 03:26:53.000000 hcpdiff-0.2.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-29 03:57:22.271138 hcpdiff-0.2.2/cfgs/
-drwxrwxrwx   0        0        0        0 2023-04-29 03:57:22.275220 hcpdiff-0.2.2/cfgs/infer/
--rw-rw-rw-   0        0        0      179 2023-04-11 09:59:00.000000 hcpdiff-0.2.2/cfgs/infer/change_vae.yaml
--rw-rw-rw-   0        0        0      672 2023-04-12 10:04:24.000000 hcpdiff-0.2.2/cfgs/infer/euler_a.yaml
--rw-rw-rw-   0        0        0     1659 2023-04-25 10:11:05.000000 hcpdiff-0.2.2/cfgs/infer/img2img.yaml
--rw-rw-rw-   0        0        0     1003 2023-04-29 03:26:21.000000 hcpdiff-0.2.2/cfgs/infer/img2img_controlnet.yaml
--rw-rw-rw-   0        0        0     1581 2023-04-29 03:26:21.000000 hcpdiff-0.2.2/cfgs/infer/text2img.yaml
-drwxrwxrwx   0        0        0        0 2023-04-29 03:57:22.276221 hcpdiff-0.2.2/cfgs/plugins/
--rw-rw-rw-   0        0        0      442 2023-04-29 03:26:21.000000 hcpdiff-0.2.2/cfgs/plugins/plugin_controlnet.yaml
--rw-rw-rw-   0        0        0     9971 2023-03-22 01:36:55.000000 hcpdiff-0.2.2/cfgs/te_struct.txt
-drwxrwxrwx   0        0        0        0 2023-04-29 03:57:22.278221 hcpdiff-0.2.2/cfgs/train/
-drwxrwxrwx   0        0        0        0 2023-04-29 03:57:22.284222 hcpdiff-0.2.2/cfgs/train/examples/
--rw-rw-rw-   0        0        0     1846 2023-04-11 12:30:15.000000 hcpdiff-0.2.2/cfgs/train/examples/CustomDiffusion.yaml
--rw-rw-rw-   0        0        0     2815 2023-04-15 14:19:44.000000 hcpdiff-0.2.2/cfgs/train/examples/DreamArtist++.yaml
--rw-rw-rw-   0        0        0     1334 2023-04-12 06:39:19.000000 hcpdiff-0.2.2/cfgs/train/examples/DreamArtist.yaml
--rw-rw-rw-   0        0        0     1644 2023-04-11 12:30:15.000000 hcpdiff-0.2.2/cfgs/train/examples/DreamBooth.yaml
--rw-rw-rw-   0        0        0     1124 2023-04-11 12:30:15.000000 hcpdiff-0.2.2/cfgs/train/examples/TextualInversion.yaml
--rw-rw-rw-   0        0        0     1046 2023-04-29 03:26:21.000000 hcpdiff-0.2.2/cfgs/train/examples/controlnet.yaml
--rw-rw-rw-   0        0        0     1178 2023-04-11 12:30:15.000000 hcpdiff-0.2.2/cfgs/train/examples/fine-tuning.yaml
--rw-rw-rw-   0        0        0     1397 2023-04-11 12:30:15.000000 hcpdiff-0.2.2/cfgs/train/examples/locon.yaml
--rw-rw-rw-   0        0        0     1228 2023-04-11 12:30:15.000000 hcpdiff-0.2.2/cfgs/train/examples/lora_conventional.yaml
--rw-rw-rw-   0        0        0     3158 2023-04-29 03:26:21.000000 hcpdiff-0.2.2/cfgs/train/train_base.yaml
--rw-rw-rw-   0        0        0     1025 2023-04-29 03:26:21.000000 hcpdiff-0.2.2/cfgs/train/tuning_base.yaml
--rw-rw-rw-   0        0        0    46121 2023-03-22 01:36:55.000000 hcpdiff-0.2.2/cfgs/unet_struct.txt
-drwxrwxrwx   0        0        0        0 2023-04-29 03:57:22.288404 hcpdiff-0.2.2/hcpdiff/
--rw-rw-rw-   0        0        0        0 2023-04-11 12:30:15.000000 hcpdiff-0.2.2/hcpdiff/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-29 03:57:22.297401 hcpdiff-0.2.2/hcpdiff/data/
--rw-rw-rw-   0        0        0      195 2023-04-29 03:26:21.000000 hcpdiff-0.2.2/hcpdiff/data/__init__.py
--rw-rw-rw-   0        0        0     8773 2023-04-29 03:26:21.000000 hcpdiff-0.2.2/hcpdiff/data/bucket.py
--rw-rw-rw-   0        0        0     2390 2023-04-29 03:26:21.000000 hcpdiff-0.2.2/hcpdiff/data/cond_pair_dataset.py
--rw-rw-rw-   0        0        0     5782 2023-04-29 03:26:21.000000 hcpdiff-0.2.2/hcpdiff/data/pair_dataset.py
--rw-rw-rw-   0        0        0     2416 2023-04-29 03:26:21.000000 hcpdiff-0.2.2/hcpdiff/data/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-29 03:57:22.305503 hcpdiff-0.2.2/hcpdiff/models/
--rw-rw-rw-   0        0        0      295 2023-04-15 14:19:44.000000 hcpdiff-0.2.2/hcpdiff/models/__init__.py
--rw-rw-rw-   0        0        0     1422 2023-04-11 12:30:15.000000 hcpdiff-0.2.2/hcpdiff/models/cfg_context.py
--rw-rw-rw-   0        0        0     7931 2023-04-29 03:26:21.000000 hcpdiff-0.2.2/hcpdiff/models/controlnet.py
--rw-rw-rw-   0        0        0     3068 2023-04-11 12:47:28.000000 hcpdiff-0.2.2/hcpdiff/models/layers.py
--rw-rw-rw-   0        0        0     6815 2023-04-29 03:26:21.000000 hcpdiff-0.2.2/hcpdiff/models/lora_base.py
--rw-rw-rw-   0        0        0     7801 2023-04-29 03:26:21.000000 hcpdiff-0.2.2/hcpdiff/models/lora_layers.py
--rw-rw-rw-   0        0        0     8973 2023-04-29 03:26:21.000000 hcpdiff-0.2.2/hcpdiff/models/plugin.py
--rw-rw-rw-   0        0        0     3922 2023-04-29 03:26:21.000000 hcpdiff-0.2.2/hcpdiff/models/text_emb_ex.py
--rw-rw-rw-   0        0        0     5807 2023-04-29 03:26:21.000000 hcpdiff-0.2.2/hcpdiff/models/textencoder_ex.py
--rw-rw-rw-   0        0        0     2440 2023-04-14 04:04:05.000000 hcpdiff-0.2.2/hcpdiff/models/tokenizer_ex.py
-drwxrwxrwx   0        0        0        0 2023-04-29 03:57:22.309504 hcpdiff-0.2.2/hcpdiff/tools/
--rw-rw-rw-   0        0        0        0 2023-04-12 06:39:19.000000 hcpdiff-0.2.2/hcpdiff/tools/__init__.py
--rw-rw-rw-   0        0        0      753 2023-04-12 08:25:47.000000 hcpdiff-0.2.2/hcpdiff/tools/convert_caption_txt2json.py
--rw-rw-rw-   0        0        0     1916 2023-04-29 03:26:21.000000 hcpdiff-0.2.2/hcpdiff/tools/create_embedding.py
--rw-rw-rw-   0        0        0     1738 2023-04-29 03:26:21.000000 hcpdiff-0.2.2/hcpdiff/tools/gen_from_ptlist.py
--rw-rw-rw-   0        0        0      658 2023-04-29 03:26:21.000000 hcpdiff-0.2.2/hcpdiff/tools/init_proj.py
--rw-rw-rw-   0        0        0     8536 2023-04-25 10:11:05.000000 hcpdiff-0.2.2/hcpdiff/tools/sd2diffusers.py
--rw-rw-rw-   0        0        0    26567 2023-04-29 03:26:21.000000 hcpdiff-0.2.2/hcpdiff/train_ac.py
--rw-rw-rw-   0        0        0     4284 2023-04-29 03:26:21.000000 hcpdiff-0.2.2/hcpdiff/train_ac_single.py
--rw-rw-rw-   0        0        0    10421 2023-04-29 03:26:21.000000 hcpdiff-0.2.2/hcpdiff/train_colo.py
-drwxrwxrwx   0        0        0        0 2023-04-29 03:57:22.315503 hcpdiff-0.2.2/hcpdiff/utils/
--rw-rw-rw-   0        0        0        0 2023-04-11 12:30:15.000000 hcpdiff-0.2.2/hcpdiff/utils/__init__.py
--rw-rw-rw-   0        0        0     2865 2023-04-12 06:39:19.000000 hcpdiff-0.2.2/hcpdiff/utils/caption_tools.py
--rw-rw-rw-   0        0        0    13041 2023-04-29 03:48:15.000000 hcpdiff-0.2.2/hcpdiff/utils/cfg_net_tools.py
-drwxrwxrwx   0        0        0        0 2023-04-29 03:57:22.318514 hcpdiff-0.2.2/hcpdiff/utils/ckpt_manager/
--rw-rw-rw-   0        0        0       82 2023-04-11 12:30:15.000000 hcpdiff-0.2.2/hcpdiff/utils/ckpt_manager/__init__.py
--rw-rw-rw-   0        0        0     4266 2023-04-29 03:26:21.000000 hcpdiff-0.2.2/hcpdiff/utils/ckpt_manager/ckpt_pkl.py
--rw-rw-rw-   0        0        0     1884 2023-04-25 10:11:05.000000 hcpdiff-0.2.2/hcpdiff/utils/ckpt_manager/ckpt_safetensor.py
--rw-rw-rw-   0        0        0      860 2023-04-11 12:30:15.000000 hcpdiff-0.2.2/hcpdiff/utils/colo_utils.py
--rw-rw-rw-   0        0        0     3065 2023-04-11 12:30:15.000000 hcpdiff-0.2.2/hcpdiff/utils/ema.py
--rw-rw-rw-   0        0        0     8680 2023-04-11 12:30:15.000000 hcpdiff-0.2.2/hcpdiff/utils/img_size_tool.py
--rw-rw-rw-   0        0        0     5937 2023-04-29 03:26:21.000000 hcpdiff-0.2.2/hcpdiff/utils/net_utils.py
--rw-rw-rw-   0        0        0     2741 2023-04-29 03:26:21.000000 hcpdiff-0.2.2/hcpdiff/utils/utils.py
--rw-rw-rw-   0        0        0     7365 2023-04-27 13:09:44.000000 hcpdiff-0.2.2/hcpdiff/visualizer.py
-drwxrwxrwx   0        0        0        0 2023-04-29 03:57:22.293402 hcpdiff-0.2.2/hcpdiff.egg-info/
--rw-rw-rw-   0        0        0     5507 2023-04-29 03:57:22.000000 hcpdiff-0.2.2/hcpdiff.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2277 2023-04-29 03:57:22.000000 hcpdiff-0.2.2/hcpdiff.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 03:57:22.000000 hcpdiff-0.2.2/hcpdiff.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2023-04-29 03:57:22.000000 hcpdiff-0.2.2/hcpdiff.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      225 2023-04-29 03:57:22.000000 hcpdiff-0.2.2/hcpdiff.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-29 03:57:22.000000 hcpdiff-0.2.2/hcpdiff.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-29 03:57:22.324504 hcpdiff-0.2.2/prompt_tuning_template/
--rw-rw-rw-   0        0        0       14 2023-04-03 03:15:56.000000 hcpdiff-0.2.2/prompt_tuning_template/caption.txt
--rw-rw-rw-   0        0        0       14 2023-02-21 02:34:54.000000 hcpdiff-0.2.2/prompt_tuning_template/name.txt
--rw-rw-rw-   0        0        0       55 2023-02-21 02:36:10.000000 hcpdiff-0.2.2/prompt_tuning_template/name_2pt_caption.txt
--rw-rw-rw-   0        0        0       25 2023-03-22 03:52:13.000000 hcpdiff-0.2.2/prompt_tuning_template/name_caption.txt
--rw-rw-rw-   0        0        0      915 2023-04-02 01:48:02.000000 hcpdiff-0.2.2/prompt_tuning_template/object.txt
--rw-rw-rw-   0        0        0     1212 2023-04-17 05:27:11.000000 hcpdiff-0.2.2/prompt_tuning_template/object_caption.txt
--rw-rw-rw-   0        0        0      890 2023-04-11 08:41:31.000000 hcpdiff-0.2.2/prompt_tuning_template/style.txt
--rw-rw-rw-   0        0        0     1099 2023-04-17 05:27:11.000000 hcpdiff-0.2.2/prompt_tuning_template/style_caption.txt
--rw-rw-rw-   0        0        0       42 2023-04-29 03:57:22.329503 hcpdiff-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0     1833 2023-04-29 03:57:13.000000 hcpdiff-0.2.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-29 03:57:22.327503 hcpdiff-0.2.2/test/
--rw-rw-rw-   0        0        0     1062 2023-04-19 08:08:17.000000 hcpdiff-0.2.2/test/test_combine.py
--rw-rw-rw-   0        0        0      717 2023-04-25 06:44:29.000000 hcpdiff-0.2.2/test/test_ctnet.py
--rw-rw-rw-   0        0        0      918 2023-04-20 07:07:20.000000 hcpdiff-0.2.2/test/test_paradict.py
--rw-rw-rw-   0        0        0      592 2023-04-13 07:54:04.000000 hcpdiff-0.2.2/test/test_plugin_param.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:28:25.861787 hcpdiff-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5407 2023-05-06 03:28:25.861787 hcpdiff-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4690 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:28:25.845787 hcpdiff-0.3.0/cfgs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:28:25.849787 hcpdiff-0.3.0/cfgs/infer/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/cfgs/infer/change_vae.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/cfgs/infer/euler_a.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/cfgs/infer/img2img.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/cfgs/infer/img2img_controlnet.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/cfgs/infer/text2img.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:28:25.849787 hcpdiff-0.3.0/cfgs/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/cfgs/plugins/plugin_controlnet.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     9778 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/cfgs/te_struct.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:28:25.849787 hcpdiff-0.3.0/cfgs/train/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:28:25.849787 hcpdiff-0.3.0/cfgs/train/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/cfgs/train/examples/CustomDiffusion.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/cfgs/train/examples/DreamArtist++.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/cfgs/train/examples/DreamArtist.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/cfgs/train/examples/DreamBooth.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/cfgs/train/examples/TextualInversion.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/cfgs/train/examples/controlnet.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/cfgs/train/examples/fine-tuning.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/cfgs/train/examples/locon.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/cfgs/train/examples/lora_conventional.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/cfgs/train/examples/min_snr.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/cfgs/train/train_base.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/cfgs/train/tuning_base.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    45190 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/cfgs/unet_struct.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:28:25.849787 hcpdiff-0.3.0/hcpdiff/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/hcpdiff/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:28:25.853787 hcpdiff-0.3.0/hcpdiff/ckpt_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/hcpdiff/ckpt_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/hcpdiff/ckpt_manager/ckpt_pkl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/hcpdiff/ckpt_manager/ckpt_safetensor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:28:25.853787 hcpdiff-0.3.0/hcpdiff/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/hcpdiff/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8554 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/hcpdiff/data/bucket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/hcpdiff/data/cond_pair_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6104 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/hcpdiff/data/pair_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/hcpdiff/data/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:28:25.853787 hcpdiff-0.3.0/hcpdiff/loggers/
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/hcpdiff/loggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/hcpdiff/loggers/base_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/hcpdiff/loggers/cli_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/hcpdiff/loggers/tensorboard_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/hcpdiff/loggers/wandb_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:28:25.857787 hcpdiff-0.3.0/hcpdiff/loss/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/hcpdiff/loss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/hcpdiff/loss/min_snr_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/hcpdiff/loss/mse_loss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:28:25.857787 hcpdiff-0.3.0/hcpdiff/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/hcpdiff/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/hcpdiff/models/cfg_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7744 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/hcpdiff/models/controlnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/hcpdiff/models/layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6677 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/hcpdiff/models/lora_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7832 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/hcpdiff/models/lora_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8754 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/hcpdiff/models/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/hcpdiff/models/text_emb_ex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5674 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/hcpdiff/models/textencoder_ex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/hcpdiff/models/tokenizer_ex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:28:25.857787 hcpdiff-0.3.0/hcpdiff/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/hcpdiff/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/hcpdiff/tools/convert_caption_txt2json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/hcpdiff/tools/create_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/hcpdiff/tools/gen_from_ptlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/hcpdiff/tools/init_proj.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8326 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/hcpdiff/tools/sd2diffusers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26244 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/hcpdiff/train_ac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4785 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/hcpdiff/train_ac_single.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9319 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/hcpdiff/train_colo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:28:25.861787 hcpdiff-0.3.0/hcpdiff/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/hcpdiff/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/hcpdiff/utils/caption_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12819 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/hcpdiff/utils/cfg_net_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/hcpdiff/utils/colo_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/hcpdiff/utils/ema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8433 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/hcpdiff/utils/img_size_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7052 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/hcpdiff/utils/net_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/hcpdiff/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7221 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/hcpdiff/visualizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:28:25.853787 hcpdiff-0.3.0/hcpdiff.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5407 2023-05-06 03:28:25.000000 hcpdiff-0.3.0/hcpdiff.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-05-06 03:28:25.000000 hcpdiff-0.3.0/hcpdiff.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 03:28:25.000000 hcpdiff-0.3.0/hcpdiff.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-06 03:28:25.000000 hcpdiff-0.3.0/hcpdiff.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-06 03:28:25.000000 hcpdiff-0.3.0/hcpdiff.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-06 03:28:25.000000 hcpdiff-0.3.0/hcpdiff.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:28:25.861787 hcpdiff-0.3.0/prompt_tuning_template/
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/prompt_tuning_template/caption.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/prompt_tuning_template/name.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/prompt_tuning_template/name_2pt_caption.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/prompt_tuning_template/name_caption.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/prompt_tuning_template/object.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/prompt_tuning_template/object_caption.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/prompt_tuning_template/style.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/prompt_tuning_template/style_caption.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 03:28:25.861787 hcpdiff-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/setup.py
```

### Comparing `hcpdiff-0.2.2/LICENSE` & `hcpdiff-0.3.0/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,201 +1,201 @@
-                                 Apache License
-                           Version 2.0, January 2004
-                        http://www.apache.org/licenses/
-
-   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      "License" shall mean the terms and conditions for use, reproduction,
-      and distribution as defined by Sections 1 through 9 of this document.
-
-      "Licensor" shall mean the copyright owner or entity authorized by
-      the copyright owner that is granting the License.
-
-      "Legal Entity" shall mean the union of the acting entity and all
-      other entities that control, are controlled by, or are under common
-      control with that entity. For the purposes of this definition,
-      "control" means (i) the power, direct or indirect, to cause the
-      direction or management of such entity, whether by contract or
-      otherwise, or (ii) ownership of fifty percent (50%) or more of the
-      outstanding shares, or (iii) beneficial ownership of such entity.
-
-      "You" (or "Your") shall mean an individual or Legal Entity
-      exercising permissions granted by this License.
-
-      "Source" form shall mean the preferred form for making modifications,
-      including but not limited to software source code, documentation
-      source, and configuration files.
-
-      "Object" form shall mean any form resulting from mechanical
-      transformation or translation of a Source form, including but
-      not limited to compiled object code, generated documentation,
-      and conversions to other media types.
-
-      "Work" shall mean the work of authorship, whether in Source or
-      Object form, made available under the License, as indicated by a
-      copyright notice that is included in or attached to the work
-      (an example is provided in the Appendix below).
-
-      "Derivative Works" shall mean any work, whether in Source or Object
-      form, that is based on (or derived from) the Work and for which the
-      editorial revisions, annotations, elaborations, or other modifications
-      represent, as a whole, an original work of authorship. For the purposes
-      of this License, Derivative Works shall not include works that remain
-      separable from, or merely link (or bind by name) to the interfaces of,
-      the Work and Derivative Works thereof.
-
-      "Contribution" shall mean any work of authorship, including
-      the original version of the Work and any modifications or additions
-      to that Work or Derivative Works thereof, that is intentionally
-      submitted to Licensor for inclusion in the Work by the copyright owner
-      or by an individual or Legal Entity authorized to submit on behalf of
-      the copyright owner. For the purposes of this definition, "submitted"
-      means any form of electronic, verbal, or written communication sent
-      to the Licensor or its representatives, including but not limited to
-      communication on electronic mailing lists, source code control systems,
-      and issue tracking systems that are managed by, or on behalf of, the
-      Licensor for the purpose of discussing and improving the Work, but
-      excluding communication that is conspicuously marked or otherwise
-      designated in writing by the copyright owner as "Not a Contribution."
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity
-      on behalf of whom a Contribution has been received by Licensor and
-      subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      copyright license to reproduce, prepare Derivative Works of,
-      publicly display, publicly perform, sublicense, and distribute the
-      Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      (except as stated in this section) patent license to make, have made,
-      use, offer to sell, sell, import, and otherwise transfer the Work,
-      where such license applies only to those patent claims licensable
-      by such Contributor that are necessarily infringed by their
-      Contribution(s) alone or by combination of their Contribution(s)
-      with the Work to which such Contribution(s) was submitted. If You
-      institute patent litigation against any entity (including a
-      cross-claim or counterclaim in a lawsuit) alleging that the Work
-      or a Contribution incorporated within the Work constitutes direct
-      or contributory patent infringement, then any patent licenses
-      granted to You under this License for that Work shall terminate
-      as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the
-      Work or Derivative Works thereof in any medium, with or without
-      modifications, and in Source or Object form, provided that You
-      meet the following conditions:
-
-      (a) You must give any other recipients of the Work or
-          Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices
-          stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works
-          that You distribute, all copyright, patent, trademark, and
-          attribution notices from the Source form of the Work,
-          excluding those notices that do not pertain to any part of
-          the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its
-          distribution, then any Derivative Works that You distribute must
-          include a readable copy of the attribution notices contained
-          within such NOTICE file, excluding those notices that do not
-          pertain to any part of the Derivative Works, in at least one
-          of the following places: within a NOTICE text file distributed
-          as part of the Derivative Works; within the Source form or
-          documentation, if provided along with the Derivative Works; or,
-          within a display generated by the Derivative Works, if and
-          wherever such third-party notices normally appear. The contents
-          of the NOTICE file are for informational purposes only and
-          do not modify the License. You may add Your own attribution
-          notices within Derivative Works that You distribute, alongside
-          or as an addendum to the NOTICE text from the Work, provided
-          that such additional attribution notices cannot be construed
-          as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and
-      may provide additional or different license terms and conditions
-      for use, reproduction, or distribution of Your modifications, or
-      for any such Derivative Works as a whole, provided Your use,
-      reproduction, and distribution of the Work otherwise complies with
-      the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise,
-      any Contribution intentionally submitted for inclusion in the Work
-      by You to the Licensor shall be under the terms and conditions of
-      this License, without any additional terms or conditions.
-      Notwithstanding the above, nothing herein shall supersede or modify
-      the terms of any separate license agreement you may have executed
-      with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade
-      names, trademarks, service marks, or product names of the Licensor,
-      except as required for reasonable and customary use in describing the
-      origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or
-      agreed to in writing, Licensor provides the Work (and each
-      Contributor provides its Contributions) on an "AS IS" BASIS,
-      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-      implied, including, without limitation, any warranties or conditions
-      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-      PARTICULAR PURPOSE. You are solely responsible for determining the
-      appropriateness of using or redistributing the Work and assume any
-      risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory,
-      whether in tort (including negligence), contract, or otherwise,
-      unless required by applicable law (such as deliberate and grossly
-      negligent acts) or agreed to in writing, shall any Contributor be
-      liable to You for damages, including any direct, indirect, special,
-      incidental, or consequential damages of any character arising as a
-      result of this License or out of the use or inability to use the
-      Work (including but not limited to damages for loss of goodwill,
-      work stoppage, computer failure or malfunction, or any and all
-      other commercial damages or losses), even if such Contributor
-      has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing
-      the Work or Derivative Works thereof, You may choose to offer,
-      and charge a fee for, acceptance of support, warranty, indemnity,
-      or other liability obligations and/or rights consistent with this
-      License. However, in accepting such obligations, You may act only
-      on Your own behalf and on Your sole responsibility, not on behalf
-      of any other Contributor, and only if You agree to indemnify,
-      defend, and hold each Contributor harmless for any liability
-      incurred by, or claims asserted against, such Contributor by reason
-      of your accepting any such warranty or additional liability.
-
-   END OF TERMS AND CONDITIONS
-
-   APPENDIX: How to apply the Apache License to your work.
-
-      To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "[]"
-      replaced with your own identifying information. (Don't include
-      the brackets!)  The text should be enclosed in the appropriate
-      comment syntax for the file format. We also recommend that a
-      file or class name and description of purpose be included on the
-      same "printed page" as the copyright notice for easier
-      identification within third-party archives.
-
-   Copyright [yyyy] [name of copyright owner]
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
+                                 Apache License
+                           Version 2.0, January 2004
+                        http://www.apache.org/licenses/
+
+   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+   1. Definitions.
+
+      "License" shall mean the terms and conditions for use, reproduction,
+      and distribution as defined by Sections 1 through 9 of this document.
+
+      "Licensor" shall mean the copyright owner or entity authorized by
+      the copyright owner that is granting the License.
+
+      "Legal Entity" shall mean the union of the acting entity and all
+      other entities that control, are controlled by, or are under common
+      control with that entity. For the purposes of this definition,
+      "control" means (i) the power, direct or indirect, to cause the
+      direction or management of such entity, whether by contract or
+      otherwise, or (ii) ownership of fifty percent (50%) or more of the
+      outstanding shares, or (iii) beneficial ownership of such entity.
+
+      "You" (or "Your") shall mean an individual or Legal Entity
+      exercising permissions granted by this License.
+
+      "Source" form shall mean the preferred form for making modifications,
+      including but not limited to software source code, documentation
+      source, and configuration files.
+
+      "Object" form shall mean any form resulting from mechanical
+      transformation or translation of a Source form, including but
+      not limited to compiled object code, generated documentation,
+      and conversions to other media types.
+
+      "Work" shall mean the work of authorship, whether in Source or
+      Object form, made available under the License, as indicated by a
+      copyright notice that is included in or attached to the work
+      (an example is provided in the Appendix below).
+
+      "Derivative Works" shall mean any work, whether in Source or Object
+      form, that is based on (or derived from) the Work and for which the
+      editorial revisions, annotations, elaborations, or other modifications
+      represent, as a whole, an original work of authorship. For the purposes
+      of this License, Derivative Works shall not include works that remain
+      separable from, or merely link (or bind by name) to the interfaces of,
+      the Work and Derivative Works thereof.
+
+      "Contribution" shall mean any work of authorship, including
+      the original version of the Work and any modifications or additions
+      to that Work or Derivative Works thereof, that is intentionally
+      submitted to Licensor for inclusion in the Work by the copyright owner
+      or by an individual or Legal Entity authorized to submit on behalf of
+      the copyright owner. For the purposes of this definition, "submitted"
+      means any form of electronic, verbal, or written communication sent
+      to the Licensor or its representatives, including but not limited to
+      communication on electronic mailing lists, source code control systems,
+      and issue tracking systems that are managed by, or on behalf of, the
+      Licensor for the purpose of discussing and improving the Work, but
+      excluding communication that is conspicuously marked or otherwise
+      designated in writing by the copyright owner as "Not a Contribution."
+
+      "Contributor" shall mean Licensor and any individual or Legal Entity
+      on behalf of whom a Contribution has been received by Licensor and
+      subsequently incorporated within the Work.
+
+   2. Grant of Copyright License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      copyright license to reproduce, prepare Derivative Works of,
+      publicly display, publicly perform, sublicense, and distribute the
+      Work and such Derivative Works in Source or Object form.
+
+   3. Grant of Patent License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      (except as stated in this section) patent license to make, have made,
+      use, offer to sell, sell, import, and otherwise transfer the Work,
+      where such license applies only to those patent claims licensable
+      by such Contributor that are necessarily infringed by their
+      Contribution(s) alone or by combination of their Contribution(s)
+      with the Work to which such Contribution(s) was submitted. If You
+      institute patent litigation against any entity (including a
+      cross-claim or counterclaim in a lawsuit) alleging that the Work
+      or a Contribution incorporated within the Work constitutes direct
+      or contributory patent infringement, then any patent licenses
+      granted to You under this License for that Work shall terminate
+      as of the date such litigation is filed.
+
+   4. Redistribution. You may reproduce and distribute copies of the
+      Work or Derivative Works thereof in any medium, with or without
+      modifications, and in Source or Object form, provided that You
+      meet the following conditions:
+
+      (a) You must give any other recipients of the Work or
+          Derivative Works a copy of this License; and
+
+      (b) You must cause any modified files to carry prominent notices
+          stating that You changed the files; and
+
+      (c) You must retain, in the Source form of any Derivative Works
+          that You distribute, all copyright, patent, trademark, and
+          attribution notices from the Source form of the Work,
+          excluding those notices that do not pertain to any part of
+          the Derivative Works; and
+
+      (d) If the Work includes a "NOTICE" text file as part of its
+          distribution, then any Derivative Works that You distribute must
+          include a readable copy of the attribution notices contained
+          within such NOTICE file, excluding those notices that do not
+          pertain to any part of the Derivative Works, in at least one
+          of the following places: within a NOTICE text file distributed
+          as part of the Derivative Works; within the Source form or
+          documentation, if provided along with the Derivative Works; or,
+          within a display generated by the Derivative Works, if and
+          wherever such third-party notices normally appear. The contents
+          of the NOTICE file are for informational purposes only and
+          do not modify the License. You may add Your own attribution
+          notices within Derivative Works that You distribute, alongside
+          or as an addendum to the NOTICE text from the Work, provided
+          that such additional attribution notices cannot be construed
+          as modifying the License.
+
+      You may add Your own copyright statement to Your modifications and
+      may provide additional or different license terms and conditions
+      for use, reproduction, or distribution of Your modifications, or
+      for any such Derivative Works as a whole, provided Your use,
+      reproduction, and distribution of the Work otherwise complies with
+      the conditions stated in this License.
+
+   5. Submission of Contributions. Unless You explicitly state otherwise,
+      any Contribution intentionally submitted for inclusion in the Work
+      by You to the Licensor shall be under the terms and conditions of
+      this License, without any additional terms or conditions.
+      Notwithstanding the above, nothing herein shall supersede or modify
+      the terms of any separate license agreement you may have executed
+      with Licensor regarding such Contributions.
+
+   6. Trademarks. This License does not grant permission to use the trade
+      names, trademarks, service marks, or product names of the Licensor,
+      except as required for reasonable and customary use in describing the
+      origin of the Work and reproducing the content of the NOTICE file.
+
+   7. Disclaimer of Warranty. Unless required by applicable law or
+      agreed to in writing, Licensor provides the Work (and each
+      Contributor provides its Contributions) on an "AS IS" BASIS,
+      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+      implied, including, without limitation, any warranties or conditions
+      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+      PARTICULAR PURPOSE. You are solely responsible for determining the
+      appropriateness of using or redistributing the Work and assume any
+      risks associated with Your exercise of permissions under this License.
+
+   8. Limitation of Liability. In no event and under no legal theory,
+      whether in tort (including negligence), contract, or otherwise,
+      unless required by applicable law (such as deliberate and grossly
+      negligent acts) or agreed to in writing, shall any Contributor be
+      liable to You for damages, including any direct, indirect, special,
+      incidental, or consequential damages of any character arising as a
+      result of this License or out of the use or inability to use the
+      Work (including but not limited to damages for loss of goodwill,
+      work stoppage, computer failure or malfunction, or any and all
+      other commercial damages or losses), even if such Contributor
+      has been advised of the possibility of such damages.
+
+   9. Accepting Warranty or Additional Liability. While redistributing
+      the Work or Derivative Works thereof, You may choose to offer,
+      and charge a fee for, acceptance of support, warranty, indemnity,
+      or other liability obligations and/or rights consistent with this
+      License. However, in accepting such obligations, You may act only
+      on Your own behalf and on Your sole responsibility, not on behalf
+      of any other Contributor, and only if You agree to indemnify,
+      defend, and hold each Contributor harmless for any liability
+      incurred by, or claims asserted against, such Contributor by reason
+      of your accepting any such warranty or additional liability.
+
+   END OF TERMS AND CONDITIONS
+
+   APPENDIX: How to apply the Apache License to your work.
+
+      To apply the Apache License to your work, attach the following
+      boilerplate notice, with the fields enclosed by brackets "[]"
+      replaced with your own identifying information. (Don't include
+      the brackets!)  The text should be enclosed in the appropriate
+      comment syntax for the file format. We also recommend that a
+      file or class name and description of purpose be included on the
+      same "printed page" as the copyright notice for easier
+      identification within third-party archives.
+
+   Copyright [yyyy] [name of copyright owner]
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
```

### Comparing `hcpdiff-0.2.2/PKG-INFO` & `hcpdiff-0.3.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,148 +1,130 @@
-Metadata-Version: 2.1
-Name: hcpdiff
-Version: 0.2.2
-Summary: A universal Stable-Diffusion toolbox
-Home-page: https://github.com/7eu7d7/HCP-Diffusion
-Author: Ziyi Dong
-Author-email: dzy7eu7d7@gmail.com
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# HCP-Diffusion
-
-[![PyPI](https://img.shields.io/pypi/v/hcpdiff)](https://pypi.org/project/hcpdiff/)
-[![GitHub stars](https://img.shields.io/github/stars/7eu7d7/HCP-Diffusion)](https://github.com/7eu7d7/HCP-Diffusion/stargazers)
-[![GitHub license](https://img.shields.io/github/license/7eu7d7/HCP-Diffusion)](https://github.com/7eu7d7/HCP-Diffusion/blob/master/LICENSE)
-[![codecov](https://codecov.io/gh/7eu7d7/HCP-Diffusion/branch/main/graph/badge.svg)](https://codecov.io/gh/7eu7d7/HCP-Diffusion)
-[![open issues](https://isitmaintained.com/badge/open/7eu7d7/HCP-Diffusion.svg)](https://github.com/7eu7d7/HCP-Diffusion/issues)
-
-[📘中文说明](./README_cn.md)
-
-## Introduction
-HCP-Diffusion is a toolbox for stable diffusion models based on diffusers.
-It facilitates flexiable configurations and component support for training, in comparison with webui and sd-scripts.
-
-This toolbox supports **colossal-AI**, which can significantly reduce GPU memory usage.
-
-HCP-Diffusion can unify existing training methods for text-to-image generation (e.g., Prompt-tuning, Textual Inversion, DreamArtist, Fine-tuning, DreamBooth, LoRA, ControlNet, etc) and model structures through a single ```.yaml``` configuration file.
-
-The toolbox has also implemented an upgraded version of DreamArtist with LoRA, named DreamArtist++, for one-shot text-to-image generation.
-Compared to DreamArtist, DreamArtist++ is more stable with higher image quality and generation controllability, and faster training speed.
-
-## Features
-
-* Layer-wise LoRA (with Conv2d)
-* Layer-wise fine-tuning
-* Layer-wise model ensemble
-* Prompt-tuning with multiple words
-* DreamArtist and DreamArtist++
-* Aspect Ratio Bucket (ARB) with automatic clustering
-* Priori data
-* Image attention mask
-* Word attention multiplier
-* Custom words that occupy multiple words
-* Maximum sentence length expansion
-* colossal-AI
-* xformers for unet and text-encoder
-* CLIP skip
-* Tag shuffle and dropout
-* safetensors support
-* Controlnet (support train)
-
-## Install
-
-Install with pip:
-```bash
-pip install hcpdiff
-# Start a new project and make initialization
-hcpinit
-```
-
-Install from source:
-```bash
-git clone https://github.com/7eu7d7/HCP-Diffusion.git
-cd HCP-Diffusion
-pip install -e .
-# Modified based on this project or start a new project and make initialization
-## hcpinit
-```
-
-## User guidance
-
-Training:
-```yaml
-# with accelerate
-accelerate launch -m hcpdiff.train_ac --cfg cfgs/train/cfg_file.yaml
-# with accelerate and only one gpu
-accelerate launch -m hcpdiff.train_ac_single --cfg cfgs/train/cfg_file.yaml
-# with colossal-AI
-torchrun --nproc_per_node 1 -m hcpdiff.train_colo --cfg cfgs/train/cfg_file.yaml
-```
-
-Inference:
-```yaml
-python -m hcpdiff.visualizer --cfg cfgs/infer/cfg.yaml pretrained_model=pretrained_model_path \
-        prompt='positive_prompt' \
-        neg_prompt='negative_prompt' \
-        seed=42
-```
-
-The framework is based on diffusers. So it needs to convert the original stable diffusion model into a supported format using the [scripts provided by diffusers](https://github.com/huggingface/diffusers/blob/main/scripts/convert_original_stable_diffusion_to_diffusers.py).
-+ Download the [config file](https://huggingface.co/runwayml/stable-diffusion-v1-5/blob/main/v1-inference.yaml)
-+ Convert models based on config file
-
-```bash
-python -m hcpdiff.tools.sd2diffusers \
-    --checkpoint_path "path_to_stable_diffusion_model" \
-    --original_config_file "path_to_config_file" \
-    --dump_path "save_directory" \
-    [--extract_ema] # Extract ema model
-    [--from_safetensors] # Whether the original model is in safetensors format
-    [--to_safetensors] # Whether to save to safetensors format
-```
-
-+ [Model Training Tutorial](doc/guide_train.md)
-+ [DreamArtist++ Tutorial](doc/guide_DA.md)
-+ [Model Inference Tutorial](doc/guide_infer.md)
-+ [Configuration file explanation](doc/guide_cfg.md)
-
-Use xformer to reduce VRAM usage and accelerate training:
-```bash
-# use conda
-conda install xformers -c xformers
-
-# use pip
-pip install xfromers>=0.0.17
-```
-
-## Team
-
-This toolbox is maintained by [HCP-Lab, SYSU](https://www.sysu-hcp.net/).
-More models and features are welcome to contribute to this toolbox.
-
-## Citation
-
-```
-@article{DBLP:journals/corr/abs-2211-11337,
-  author    = {Ziyi Dong and
-               Pengxu Wei and
-               Liang Lin},
-  title     = {DreamArtist: Towards Controllable One-Shot Text-to-Image Generation
-               via Positive-Negative Prompt-Tuning},
-  journal   = {CoRR},
-  volume    = {abs/2211.11337},
-  year      = {2022},
-  doi       = {10.48550/arXiv.2211.11337},
-  eprinttype = {arXiv},
-  eprint    = {2211.11337},
-}
-```
+# HCP-Diffusion
+
+[![PyPI](https://img.shields.io/pypi/v/hcpdiff)](https://pypi.org/project/hcpdiff/)
+[![GitHub stars](https://img.shields.io/github/stars/7eu7d7/HCP-Diffusion)](https://github.com/7eu7d7/HCP-Diffusion/stargazers)
+[![GitHub license](https://img.shields.io/github/license/7eu7d7/HCP-Diffusion)](https://github.com/7eu7d7/HCP-Diffusion/blob/master/LICENSE)
+[![codecov](https://codecov.io/gh/7eu7d7/HCP-Diffusion/branch/main/graph/badge.svg)](https://codecov.io/gh/7eu7d7/HCP-Diffusion)
+[![open issues](https://isitmaintained.com/badge/open/7eu7d7/HCP-Diffusion.svg)](https://github.com/7eu7d7/HCP-Diffusion/issues)
+
+[📘中文说明](./README_cn.md)
+
+## Introduction
+HCP-Diffusion is a toolbox for stable diffusion models based on diffusers.
+It facilitates flexiable configurations and component support for training, in comparison with webui and sd-scripts.
+
+This toolbox supports **colossal-AI**, which can significantly reduce GPU memory usage.
+
+HCP-Diffusion can unify existing training methods for text-to-image generation (e.g., Prompt-tuning, Textual Inversion, DreamArtist, Fine-tuning, DreamBooth, LoRA, ControlNet, etc) and model structures through a single ```.yaml``` configuration file.
+
+The toolbox has also implemented an upgraded version of DreamArtist with LoRA, named DreamArtist++, for one-shot text-to-image generation.
+Compared to DreamArtist, DreamArtist++ is more stable with higher image quality and generation controllability, and faster training speed.
+
+## Features
+
+* Layer-wise LoRA (with Conv2d)
+* Layer-wise fine-tuning
+* Layer-wise model ensemble
+* Prompt-tuning with multiple words
+* DreamArtist and DreamArtist++
+* Aspect Ratio Bucket (ARB) with automatic clustering
+* Multiple datasets with multiple data sources
+* Image attention mask
+* Word attention multiplier
+* Custom words that occupy multiple words
+* Maximum sentence length expansion
+* colossal-AI
+* xformers for unet and text-encoder
+* CLIP skip
+* Tag shuffle and dropout
+* safetensors support
+* Controlnet (support train)
+* Min-SNR loss
+
+## Install
+
+Install with pip:
+```bash
+pip install hcpdiff
+# Start a new project and make initialization
+hcpinit
+```
+
+Install from source:
+```bash
+git clone https://github.com/7eu7d7/HCP-Diffusion.git
+cd HCP-Diffusion
+pip install -e .
+# Modified based on this project or start a new project and make initialization
+## hcpinit
+```
+
+## User guidance
+
+Training:
+```yaml
+# with accelerate
+accelerate launch -m hcpdiff.train_ac --cfg cfgs/train/cfg_file.yaml
+# with accelerate and only one gpu
+accelerate launch -m hcpdiff.train_ac_single --cfg cfgs/train/cfg_file.yaml
+# with colossal-AI
+torchrun --nproc_per_node 1 -m hcpdiff.train_colo --cfg cfgs/train/cfg_file.yaml
+```
+
+Inference:
+```yaml
+python -m hcpdiff.visualizer --cfg cfgs/infer/cfg.yaml pretrained_model=pretrained_model_path \
+        prompt='positive_prompt' \
+        neg_prompt='negative_prompt' \
+        seed=42
+```
+
+The framework is based on diffusers. So it needs to convert the original stable diffusion model into a supported format using the [scripts provided by diffusers](https://github.com/huggingface/diffusers/blob/main/scripts/convert_original_stable_diffusion_to_diffusers.py).
++ Download the [config file](https://huggingface.co/runwayml/stable-diffusion-v1-5/blob/main/v1-inference.yaml)
++ Convert models based on config file
+
+```bash
+python -m hcpdiff.tools.sd2diffusers \
+    --checkpoint_path "path_to_stable_diffusion_model" \
+    --original_config_file "path_to_config_file" \
+    --dump_path "save_directory" \
+    [--extract_ema] # Extract ema model
+    [--from_safetensors] # Whether the original model is in safetensors format
+    [--to_safetensors] # Whether to save to safetensors format
+```
+
++ [Model Training Tutorial](doc/guide_train.md)
++ [DreamArtist++ Tutorial](doc/guide_DA.md)
++ [Model Inference Tutorial](doc/guide_infer.md)
++ [Configuration file explanation](doc/guide_cfg.md)
+
+Use xformer to reduce VRAM usage and accelerate training:
+```bash
+# use conda
+conda install xformers -c xformers
+
+# use pip
+pip install xfromers>=0.0.17
+```
+
+## Team
+
+This toolbox is maintained by [HCP-Lab, SYSU](https://www.sysu-hcp.net/).
+More models and features are welcome to contribute to this toolbox.
+
+## Citation
+
+```
+@article{DBLP:journals/corr/abs-2211-11337,
+  author    = {Ziyi Dong and
+               Pengxu Wei and
+               Liang Lin},
+  title     = {DreamArtist: Towards Controllable One-Shot Text-to-Image Generation
+               via Positive-Negative Prompt-Tuning},
+  journal   = {CoRR},
+  volume    = {abs/2211.11337},
+  year      = {2022},
+  doi       = {10.48550/arXiv.2211.11337},
+  eprinttype = {arXiv},
+  eprint    = {2211.11337},
+}
+```
```

### Comparing `hcpdiff-0.2.2/cfgs/infer/img2img.yaml` & `hcpdiff-0.3.0/cfgs/infer/text2img.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -1,65 +1,62 @@
-# base_state*base_model_alpha + (lora_state[i]*lora_scale[i]*lora_alpha[i]) + (part_state[k]*part_alpha[k])
-
-pretrained_model: ''
-prompt: ''
-neg_prompt: 'lowres, bad anatomy, bad hands, text, error, missing fingers, extra digit, fewer digits, cropped, worst quality, low quality, normal quality, jpeg artifacts, signature, watermark, username, blurry'
-out_dir: 'output/'
-emb_dir: 'embs/'
-N_repeats: 1
-bs: 4
-num: 1
-seed: null
-fp16: True
-
-condition:
-  type: i2i
-  image: 'cond_img.png'
-
-save:
-  save_cfg: True
-  image_type: png
-  quality: 95
-#  image_type: webp
-#  quality: 75
-
-infer_args:
-  num_inference_steps: 30
-  strength: 0.75
-  guidance_scale: 7.5
-
-new_components: {}
-
-merge: # can be null
-  exp_dir: '2023-04-03-10-10-36'
-  alpha: 0.8
-  plugin_cfg: null
-
-  group1:
-    type: 'unet'
-    base_model_alpha: 1.0 # base model weight to merge with lora or part
-    lora:
-      - path: 'exps/${....exp_dir}/ckpts/unet-600.safetensors'
-        alpha: ${....alpha}
-        layers: 'all'
-        mask: [0.5, 1]
-      - path: 'exps/${....exp_dir}/ckpts/unet-neg-600.safetensors'
-        alpha: 0.65
-        layers: 'all'
-        mask: [0, 0.5]
-    part: null
-    plugin: null
-
-  group2:
-    type: 'TE'
-    base_model_alpha: 1.0 # base model weight to infer with lora or part
-    lora:
-      - path: 'exps/${....exp_dir}/ckpts/text_encoder-600.safetensors'
-        alpha: ${....alpha}
-        layers: 'all'
-        mask: [0.5, 1]
-      - path: 'exps/${....exp_dir}/ckpts/text_encoder-neg-600.safetensors'
-        alpha: 0.65
-        layers: 'all'
-        mask: [0, 0.5]
-    part: null
-    plugin: null
+# base_state*base_model_alpha + (lora_state[i]*lora_scale[i]*lora_alpha[i]) + (part_state[k]*part_alpha[k])
+
+pretrained_model: ''
+prompt: ''
+neg_prompt: 'lowres, bad anatomy, bad hands, text, error, missing fingers, extra digit, fewer digits, cropped, worst quality, low quality, normal quality, jpeg artifacts, signature, watermark, username, blurry'
+out_dir: 'output/'
+emb_dir: 'embs/'
+N_repeats: 1
+clip_skip: 0
+bs: 4
+num: 1
+seed: null
+fp16: True
+
+condition: null
+
+save:
+  save_cfg: True
+  image_type: png
+  quality: 95
+#  image_type: webp
+#  quality: 75
+
+infer_args:
+  width: 512
+  height: 512
+  guidance_scale: 7.5
+  num_inference_steps: 50
+
+new_components: {}
+
+merge: # can be null
+  exp_dir: '2023-04-03-10-10-36'
+  alpha: 0.8
+
+  group1:
+    type: 'unet'
+    base_model_alpha: 1.0 # base model weight to merge with lora or part
+    lora:
+      - path: 'exps/${....exp_dir}/ckpts/unet-600.safetensors'
+        alpha: ${....alpha}
+        layers: 'all'
+        mask: [0.5, 1]
+      - path: 'exps/${....exp_dir}/ckpts/unet-neg-600.safetensors'
+        alpha: 0.65
+        layers: 'all'
+        mask: [0, 0.5]
+    part: null
+
+  group2:
+    type: 'TE'
+    base_model_alpha: 1.0 # base model weight to infer with lora or part
+    lora:
+      - path: 'exps/${....exp_dir}/ckpts/text_encoder-600.safetensors'
+        alpha: ${....alpha}
+        layers: 'all'
+        mask: [0.5, 1]
+      - path: 'exps/${....exp_dir}/ckpts/text_encoder-neg-600.safetensors'
+        alpha: 0.65
+        layers: 'all'
+        mask: [0, 0.5]
+    part: null
```

### Comparing `hcpdiff-0.2.2/cfgs/infer/img2img_controlnet.yaml` & `hcpdiff-0.3.0/cfgs/infer/img2img_controlnet.yaml`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,44 +1,44 @@
-# base_state*base_model_alpha + (lora_state[i]*lora_scale[i]*lora_alpha[i]) + (part_state[k]*part_alpha[k])
-
-pretrained_model: ''
-prompt: ''
-neg_prompt: 'lowres, bad anatomy, bad hands, text, error, missing fingers, extra digit, fewer digits, cropped, worst quality, low quality, normal quality, jpeg artifacts, signature, watermark, username, blurry'
-out_dir: 'output/'
-emb_dir: 'embs/'
-N_repeats: 1
-clip_skip: 0
-bs: 4
-num: 1
-seed: null
-fp16: True
-
-condition:
-  type: controlnet
-  image: 'cond_img.png'
-
-save:
-  save_cfg: True
-  image_type: png
-  quality: 95
-#  image_type: webp
-#  quality: 75
-
-infer_args:
-  width: 512
-  height: 512
-  num_inference_steps: 30
-
-new_components: {}
-
-merge:
-  plugin_cfg: cfgs/plugins/plugin_controlnet.yaml
-
-  group1:
-    type: 'unet'
-    base_model_alpha: 1.0 # base model weight to merge with lora or part
-    lora: null
-    part: null
-    plugin:
-      controlnet1:
-        path: 'ckpts/controlnet.ckpt'
+# base_state*base_model_alpha + (lora_state[i]*lora_scale[i]*lora_alpha[i]) + (part_state[k]*part_alpha[k])
+
+pretrained_model: ''
+prompt: ''
+neg_prompt: 'lowres, bad anatomy, bad hands, text, error, missing fingers, extra digit, fewer digits, cropped, worst quality, low quality, normal quality, jpeg artifacts, signature, watermark, username, blurry'
+out_dir: 'output/'
+emb_dir: 'embs/'
+N_repeats: 1
+clip_skip: 0
+bs: 4
+num: 1
+seed: null
+fp16: True
+
+condition:
+  type: controlnet
+  image: 'cond_img.png'
+
+save:
+  save_cfg: True
+  image_type: png
+  quality: 95
+#  image_type: webp
+#  quality: 75
+
+infer_args:
+  width: 512
+  height: 512
+  num_inference_steps: 30
+
+new_components: {}
+
+merge:
+  plugin_cfg: cfgs/plugins/plugin_controlnet.yaml
+
+  group1:
+    type: 'unet'
+    base_model_alpha: 1.0 # base model weight to merge with lora or part
+    lora: null
+    part: null
+    plugin:
+      controlnet1:
+        path: 'ckpts/controlnet.ckpt'
         layers: 'all'
```

### Comparing `hcpdiff-0.2.2/cfgs/infer/text2img.yaml` & `hcpdiff-0.3.0/cfgs/infer/img2img.yaml`

 * *Files 19% similar despite different names*

```diff
@@ -1,61 +1,66 @@
-# base_state*base_model_alpha + (lora_state[i]*lora_scale[i]*lora_alpha[i]) + (part_state[k]*part_alpha[k])
-
-pretrained_model: ''
-prompt: ''
-neg_prompt: 'lowres, bad anatomy, bad hands, text, error, missing fingers, extra digit, fewer digits, cropped, worst quality, low quality, normal quality, jpeg artifacts, signature, watermark, username, blurry'
-out_dir: 'output/'
-emb_dir: 'embs/'
-N_repeats: 1
-bs: 4
-num: 1
-seed: null
-fp16: True
-
-condition: null
-
-save:
-  save_cfg: True
-  image_type: png
-  quality: 95
-#  image_type: webp
-#  quality: 75
-
-infer_args:
-  width: 512
-  height: 512
-  guidance_scale: 7.5
-  num_inference_steps: 50
-
-new_components: {}
-
-merge: # can be null
-  exp_dir: '2023-04-03-10-10-36'
-  alpha: 0.8
-
-  group1:
-    type: 'unet'
-    base_model_alpha: 1.0 # base model weight to merge with lora or part
-    lora:
-      - path: 'exps/${....exp_dir}/ckpts/unet-600.safetensors'
-        alpha: ${....alpha}
-        layers: 'all'
-        mask: [0.5, 1]
-      - path: 'exps/${....exp_dir}/ckpts/unet-neg-600.safetensors'
-        alpha: 0.65
-        layers: 'all'
-        mask: [0, 0.5]
-    part: null
-
-  group2:
-    type: 'TE'
-    base_model_alpha: 1.0 # base model weight to infer with lora or part
-    lora:
-      - path: 'exps/${....exp_dir}/ckpts/text_encoder-600.safetensors'
-        alpha: ${....alpha}
-        layers: 'all'
-        mask: [0.5, 1]
-      - path: 'exps/${....exp_dir}/ckpts/text_encoder-neg-600.safetensors'
-        alpha: 0.65
-        layers: 'all'
-        mask: [0, 0.5]
-    part: null
+# base_state*base_model_alpha + (lora_state[i]*lora_scale[i]*lora_alpha[i]) + (part_state[k]*part_alpha[k])
+
+pretrained_model: ''
+prompt: ''
+neg_prompt: 'lowres, bad anatomy, bad hands, text, error, missing fingers, extra digit, fewer digits, cropped, worst quality, low quality, normal quality, jpeg artifacts, signature, watermark, username, blurry'
+out_dir: 'output/'
+emb_dir: 'embs/'
+N_repeats: 1
+clip_skip: 0
+bs: 4
+num: 1
+seed: null
+fp16: True
+
+condition:
+  type: i2i
+  image: 'cond_img.png'
+
+save:
+  save_cfg: True
+  image_type: png
+  quality: 95
+#  image_type: webp
+#  quality: 75
+
+infer_args:
+  num_inference_steps: 30
+  strength: 0.75
+  guidance_scale: 7.5
+
+new_components: {}
+
+merge: # can be null
+  exp_dir: '2023-04-03-10-10-36'
+  alpha: 0.8
+  plugin_cfg: null
+
+  group1:
+    type: 'unet'
+    base_model_alpha: 1.0 # base model weight to merge with lora or part
+    lora:
+      - path: 'exps/${....exp_dir}/ckpts/unet-600.safetensors'
+        alpha: ${....alpha}
+        layers: 'all'
+        mask: [0.5, 1]
+      - path: 'exps/${....exp_dir}/ckpts/unet-neg-600.safetensors'
+        alpha: 0.65
+        layers: 'all'
+        mask: [0, 0.5]
+    part: null
+    plugin: null
+
+  group2:
+    type: 'TE'
+    base_model_alpha: 1.0 # base model weight to infer with lora or part
+    lora:
+      - path: 'exps/${....exp_dir}/ckpts/text_encoder-600.safetensors'
+        alpha: ${....alpha}
+        layers: 'all'
+        mask: [0.5, 1]
+      - path: 'exps/${....exp_dir}/ckpts/text_encoder-neg-600.safetensors'
+        alpha: 0.65
+        layers: 'all'
+        mask: [0, 0.5]
+    part: null
+    plugin: null
```

### Comparing `hcpdiff-0.2.2/cfgs/te_struct.txt` & `hcpdiff-0.3.0/cfgs/te_struct.txt`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,193 +1,193 @@
-CLIPTextModel(
-  (text_model): CLIPTextTransformer(
-    (embeddings): CLIPTextEmbeddings(
-      (token_embedding): Embedding(49408, 768)
-      (position_embedding): Embedding(77, 768)
-    )
-    (encoder): CLIPEncoder(
-      (layers): ModuleList(
-        (0): CLIPEncoderLayer(
-          (self_attn): CLIPAttention(
-            (k_proj): Linear(in_features=768, out_features=768, bias=True)
-            (v_proj): Linear(in_features=768, out_features=768, bias=True)
-            (q_proj): Linear(in_features=768, out_features=768, bias=True)
-            (out_proj): Linear(in_features=768, out_features=768, bias=True)
-          )
-          (layer_norm1): LayerNorm((768,), eps=1e-05, elementwise_affine=True)
-          (mlp): CLIPMLP(
-            (activation_fn): QuickGELUActivation()
-            (fc1): Linear(in_features=768, out_features=3072, bias=True)
-            (fc2): Linear(in_features=3072, out_features=768, bias=True)
-          )
-          (layer_norm2): LayerNorm((768,), eps=1e-05, elementwise_affine=True)
-        )
-        (1): CLIPEncoderLayer(
-          (self_attn): CLIPAttention(
-            (k_proj): Linear(in_features=768, out_features=768, bias=True)
-            (v_proj): Linear(in_features=768, out_features=768, bias=True)
-            (q_proj): Linear(in_features=768, out_features=768, bias=True)
-            (out_proj): Linear(in_features=768, out_features=768, bias=True)
-          )
-          (layer_norm1): LayerNorm((768,), eps=1e-05, elementwise_affine=True)
-          (mlp): CLIPMLP(
-            (activation_fn): QuickGELUActivation()
-            (fc1): Linear(in_features=768, out_features=3072, bias=True)
-            (fc2): Linear(in_features=3072, out_features=768, bias=True)
-          )
-          (layer_norm2): LayerNorm((768,), eps=1e-05, elementwise_affine=True)
-        )
-        (2): CLIPEncoderLayer(
-          (self_attn): CLIPAttention(
-            (k_proj): Linear(in_features=768, out_features=768, bias=True)
-            (v_proj): Linear(in_features=768, out_features=768, bias=True)
-            (q_proj): Linear(in_features=768, out_features=768, bias=True)
-            (out_proj): Linear(in_features=768, out_features=768, bias=True)
-          )
-          (layer_norm1): LayerNorm((768,), eps=1e-05, elementwise_affine=True)
-          (mlp): CLIPMLP(
-            (activation_fn): QuickGELUActivation()
-            (fc1): Linear(in_features=768, out_features=3072, bias=True)
-            (fc2): Linear(in_features=3072, out_features=768, bias=True)
-          )
-          (layer_norm2): LayerNorm((768,), eps=1e-05, elementwise_affine=True)
-        )
-        (3): CLIPEncoderLayer(
-          (self_attn): CLIPAttention(
-            (k_proj): Linear(in_features=768, out_features=768, bias=True)
-            (v_proj): Linear(in_features=768, out_features=768, bias=True)
-            (q_proj): Linear(in_features=768, out_features=768, bias=True)
-            (out_proj): Linear(in_features=768, out_features=768, bias=True)
-          )
-          (layer_norm1): LayerNorm((768,), eps=1e-05, elementwise_affine=True)
-          (mlp): CLIPMLP(
-            (activation_fn): QuickGELUActivation()
-            (fc1): Linear(in_features=768, out_features=3072, bias=True)
-            (fc2): Linear(in_features=3072, out_features=768, bias=True)
-          )
-          (layer_norm2): LayerNorm((768,), eps=1e-05, elementwise_affine=True)
-        )
-        (4): CLIPEncoderLayer(
-          (self_attn): CLIPAttention(
-            (k_proj): Linear(in_features=768, out_features=768, bias=True)
-            (v_proj): Linear(in_features=768, out_features=768, bias=True)
-            (q_proj): Linear(in_features=768, out_features=768, bias=True)
-            (out_proj): Linear(in_features=768, out_features=768, bias=True)
-          )
-          (layer_norm1): LayerNorm((768,), eps=1e-05, elementwise_affine=True)
-          (mlp): CLIPMLP(
-            (activation_fn): QuickGELUActivation()
-            (fc1): Linear(in_features=768, out_features=3072, bias=True)
-            (fc2): Linear(in_features=3072, out_features=768, bias=True)
-          )
-          (layer_norm2): LayerNorm((768,), eps=1e-05, elementwise_affine=True)
-        )
-        (5): CLIPEncoderLayer(
-          (self_attn): CLIPAttention(
-            (k_proj): Linear(in_features=768, out_features=768, bias=True)
-            (v_proj): Linear(in_features=768, out_features=768, bias=True)
-            (q_proj): Linear(in_features=768, out_features=768, bias=True)
-            (out_proj): Linear(in_features=768, out_features=768, bias=True)
-          )
-          (layer_norm1): LayerNorm((768,), eps=1e-05, elementwise_affine=True)
-          (mlp): CLIPMLP(
-            (activation_fn): QuickGELUActivation()
-            (fc1): Linear(in_features=768, out_features=3072, bias=True)
-            (fc2): Linear(in_features=3072, out_features=768, bias=True)
-          )
-          (layer_norm2): LayerNorm((768,), eps=1e-05, elementwise_affine=True)
-        )
-        (6): CLIPEncoderLayer(
-          (self_attn): CLIPAttention(
-            (k_proj): Linear(in_features=768, out_features=768, bias=True)
-            (v_proj): Linear(in_features=768, out_features=768, bias=True)
-            (q_proj): Linear(in_features=768, out_features=768, bias=True)
-            (out_proj): Linear(in_features=768, out_features=768, bias=True)
-          )
-          (layer_norm1): LayerNorm((768,), eps=1e-05, elementwise_affine=True)
-          (mlp): CLIPMLP(
-            (activation_fn): QuickGELUActivation()
-            (fc1): Linear(in_features=768, out_features=3072, bias=True)
-            (fc2): Linear(in_features=3072, out_features=768, bias=True)
-          )
-          (layer_norm2): LayerNorm((768,), eps=1e-05, elementwise_affine=True)
-        )
-        (7): CLIPEncoderLayer(
-          (self_attn): CLIPAttention(
-            (k_proj): Linear(in_features=768, out_features=768, bias=True)
-            (v_proj): Linear(in_features=768, out_features=768, bias=True)
-            (q_proj): Linear(in_features=768, out_features=768, bias=True)
-            (out_proj): Linear(in_features=768, out_features=768, bias=True)
-          )
-          (layer_norm1): LayerNorm((768,), eps=1e-05, elementwise_affine=True)
-          (mlp): CLIPMLP(
-            (activation_fn): QuickGELUActivation()
-            (fc1): Linear(in_features=768, out_features=3072, bias=True)
-            (fc2): Linear(in_features=3072, out_features=768, bias=True)
-          )
-          (layer_norm2): LayerNorm((768,), eps=1e-05, elementwise_affine=True)
-        )
-        (8): CLIPEncoderLayer(
-          (self_attn): CLIPAttention(
-            (k_proj): Linear(in_features=768, out_features=768, bias=True)
-            (v_proj): Linear(in_features=768, out_features=768, bias=True)
-            (q_proj): Linear(in_features=768, out_features=768, bias=True)
-            (out_proj): Linear(in_features=768, out_features=768, bias=True)
-          )
-          (layer_norm1): LayerNorm((768,), eps=1e-05, elementwise_affine=True)
-          (mlp): CLIPMLP(
-            (activation_fn): QuickGELUActivation()
-            (fc1): Linear(in_features=768, out_features=3072, bias=True)
-            (fc2): Linear(in_features=3072, out_features=768, bias=True)
-          )
-          (layer_norm2): LayerNorm((768,), eps=1e-05, elementwise_affine=True)
-        )
-        (9): CLIPEncoderLayer(
-          (self_attn): CLIPAttention(
-            (k_proj): Linear(in_features=768, out_features=768, bias=True)
-            (v_proj): Linear(in_features=768, out_features=768, bias=True)
-            (q_proj): Linear(in_features=768, out_features=768, bias=True)
-            (out_proj): Linear(in_features=768, out_features=768, bias=True)
-          )
-          (layer_norm1): LayerNorm((768,), eps=1e-05, elementwise_affine=True)
-          (mlp): CLIPMLP(
-            (activation_fn): QuickGELUActivation()
-            (fc1): Linear(in_features=768, out_features=3072, bias=True)
-            (fc2): Linear(in_features=3072, out_features=768, bias=True)
-          )
-          (layer_norm2): LayerNorm((768,), eps=1e-05, elementwise_affine=True)
-        )
-        (10): CLIPEncoderLayer(
-          (self_attn): CLIPAttention(
-            (k_proj): Linear(in_features=768, out_features=768, bias=True)
-            (v_proj): Linear(in_features=768, out_features=768, bias=True)
-            (q_proj): Linear(in_features=768, out_features=768, bias=True)
-            (out_proj): Linear(in_features=768, out_features=768, bias=True)
-          )
-          (layer_norm1): LayerNorm((768,), eps=1e-05, elementwise_affine=True)
-          (mlp): CLIPMLP(
-            (activation_fn): QuickGELUActivation()
-            (fc1): Linear(in_features=768, out_features=3072, bias=True)
-            (fc2): Linear(in_features=3072, out_features=768, bias=True)
-          )
-          (layer_norm2): LayerNorm((768,), eps=1e-05, elementwise_affine=True)
-        )
-        (11): CLIPEncoderLayer(
-          (self_attn): CLIPAttention(
-            (k_proj): Linear(in_features=768, out_features=768, bias=True)
-            (v_proj): Linear(in_features=768, out_features=768, bias=True)
-            (q_proj): Linear(in_features=768, out_features=768, bias=True)
-            (out_proj): Linear(in_features=768, out_features=768, bias=True)
-          )
-          (layer_norm1): LayerNorm((768,), eps=1e-05, elementwise_affine=True)
-          (mlp): CLIPMLP(
-            (activation_fn): QuickGELUActivation()
-            (fc1): Linear(in_features=768, out_features=3072, bias=True)
-            (fc2): Linear(in_features=3072, out_features=768, bias=True)
-          )
-          (layer_norm2): LayerNorm((768,), eps=1e-05, elementwise_affine=True)
-        )
-      )
-    )
-    (final_layer_norm): LayerNorm((768,), eps=1e-05, elementwise_affine=True)
-  )
-)
+CLIPTextModel(
+  (text_model): CLIPTextTransformer(
+    (embeddings): CLIPTextEmbeddings(
+      (token_embedding): Embedding(49408, 768)
+      (position_embedding): Embedding(77, 768)
+    )
+    (encoder): CLIPEncoder(
+      (layers): ModuleList(
+        (0): CLIPEncoderLayer(
+          (self_attn): CLIPAttention(
+            (k_proj): Linear(in_features=768, out_features=768, bias=True)
+            (v_proj): Linear(in_features=768, out_features=768, bias=True)
+            (q_proj): Linear(in_features=768, out_features=768, bias=True)
+            (out_proj): Linear(in_features=768, out_features=768, bias=True)
+          )
+          (layer_norm1): LayerNorm((768,), eps=1e-05, elementwise_affine=True)
+          (mlp): CLIPMLP(
+            (activation_fn): QuickGELUActivation()
+            (fc1): Linear(in_features=768, out_features=3072, bias=True)
+            (fc2): Linear(in_features=3072, out_features=768, bias=True)
+          )
+          (layer_norm2): LayerNorm((768,), eps=1e-05, elementwise_affine=True)
+        )
+        (1): CLIPEncoderLayer(
+          (self_attn): CLIPAttention(
+            (k_proj): Linear(in_features=768, out_features=768, bias=True)
+            (v_proj): Linear(in_features=768, out_features=768, bias=True)
+            (q_proj): Linear(in_features=768, out_features=768, bias=True)
+            (out_proj): Linear(in_features=768, out_features=768, bias=True)
+          )
+          (layer_norm1): LayerNorm((768,), eps=1e-05, elementwise_affine=True)
+          (mlp): CLIPMLP(
+            (activation_fn): QuickGELUActivation()
+            (fc1): Linear(in_features=768, out_features=3072, bias=True)
+            (fc2): Linear(in_features=3072, out_features=768, bias=True)
+          )
+          (layer_norm2): LayerNorm((768,), eps=1e-05, elementwise_affine=True)
+        )
+        (2): CLIPEncoderLayer(
+          (self_attn): CLIPAttention(
+            (k_proj): Linear(in_features=768, out_features=768, bias=True)
+            (v_proj): Linear(in_features=768, out_features=768, bias=True)
+            (q_proj): Linear(in_features=768, out_features=768, bias=True)
+            (out_proj): Linear(in_features=768, out_features=768, bias=True)
+          )
+          (layer_norm1): LayerNorm((768,), eps=1e-05, elementwise_affine=True)
+          (mlp): CLIPMLP(
+            (activation_fn): QuickGELUActivation()
+            (fc1): Linear(in_features=768, out_features=3072, bias=True)
+            (fc2): Linear(in_features=3072, out_features=768, bias=True)
+          )
+          (layer_norm2): LayerNorm((768,), eps=1e-05, elementwise_affine=True)
+        )
+        (3): CLIPEncoderLayer(
+          (self_attn): CLIPAttention(
+            (k_proj): Linear(in_features=768, out_features=768, bias=True)
+            (v_proj): Linear(in_features=768, out_features=768, bias=True)
+            (q_proj): Linear(in_features=768, out_features=768, bias=True)
+            (out_proj): Linear(in_features=768, out_features=768, bias=True)
+          )
+          (layer_norm1): LayerNorm((768,), eps=1e-05, elementwise_affine=True)
+          (mlp): CLIPMLP(
+            (activation_fn): QuickGELUActivation()
+            (fc1): Linear(in_features=768, out_features=3072, bias=True)
+            (fc2): Linear(in_features=3072, out_features=768, bias=True)
+          )
+          (layer_norm2): LayerNorm((768,), eps=1e-05, elementwise_affine=True)
+        )
+        (4): CLIPEncoderLayer(
+          (self_attn): CLIPAttention(
+            (k_proj): Linear(in_features=768, out_features=768, bias=True)
+            (v_proj): Linear(in_features=768, out_features=768, bias=True)
+            (q_proj): Linear(in_features=768, out_features=768, bias=True)
+            (out_proj): Linear(in_features=768, out_features=768, bias=True)
+          )
+          (layer_norm1): LayerNorm((768,), eps=1e-05, elementwise_affine=True)
+          (mlp): CLIPMLP(
+            (activation_fn): QuickGELUActivation()
+            (fc1): Linear(in_features=768, out_features=3072, bias=True)
+            (fc2): Linear(in_features=3072, out_features=768, bias=True)
+          )
+          (layer_norm2): LayerNorm((768,), eps=1e-05, elementwise_affine=True)
+        )
+        (5): CLIPEncoderLayer(
+          (self_attn): CLIPAttention(
+            (k_proj): Linear(in_features=768, out_features=768, bias=True)
+            (v_proj): Linear(in_features=768, out_features=768, bias=True)
+            (q_proj): Linear(in_features=768, out_features=768, bias=True)
+            (out_proj): Linear(in_features=768, out_features=768, bias=True)
+          )
+          (layer_norm1): LayerNorm((768,), eps=1e-05, elementwise_affine=True)
+          (mlp): CLIPMLP(
+            (activation_fn): QuickGELUActivation()
+            (fc1): Linear(in_features=768, out_features=3072, bias=True)
+            (fc2): Linear(in_features=3072, out_features=768, bias=True)
+          )
+          (layer_norm2): LayerNorm((768,), eps=1e-05, elementwise_affine=True)
+        )
+        (6): CLIPEncoderLayer(
+          (self_attn): CLIPAttention(
+            (k_proj): Linear(in_features=768, out_features=768, bias=True)
+            (v_proj): Linear(in_features=768, out_features=768, bias=True)
+            (q_proj): Linear(in_features=768, out_features=768, bias=True)
+            (out_proj): Linear(in_features=768, out_features=768, bias=True)
+          )
+          (layer_norm1): LayerNorm((768,), eps=1e-05, elementwise_affine=True)
+          (mlp): CLIPMLP(
+            (activation_fn): QuickGELUActivation()
+            (fc1): Linear(in_features=768, out_features=3072, bias=True)
+            (fc2): Linear(in_features=3072, out_features=768, bias=True)
+          )
+          (layer_norm2): LayerNorm((768,), eps=1e-05, elementwise_affine=True)
+        )
+        (7): CLIPEncoderLayer(
+          (self_attn): CLIPAttention(
+            (k_proj): Linear(in_features=768, out_features=768, bias=True)
+            (v_proj): Linear(in_features=768, out_features=768, bias=True)
+            (q_proj): Linear(in_features=768, out_features=768, bias=True)
+            (out_proj): Linear(in_features=768, out_features=768, bias=True)
+          )
+          (layer_norm1): LayerNorm((768,), eps=1e-05, elementwise_affine=True)
+          (mlp): CLIPMLP(
+            (activation_fn): QuickGELUActivation()
+            (fc1): Linear(in_features=768, out_features=3072, bias=True)
+            (fc2): Linear(in_features=3072, out_features=768, bias=True)
+          )
+          (layer_norm2): LayerNorm((768,), eps=1e-05, elementwise_affine=True)
+        )
+        (8): CLIPEncoderLayer(
+          (self_attn): CLIPAttention(
+            (k_proj): Linear(in_features=768, out_features=768, bias=True)
+            (v_proj): Linear(in_features=768, out_features=768, bias=True)
+            (q_proj): Linear(in_features=768, out_features=768, bias=True)
+            (out_proj): Linear(in_features=768, out_features=768, bias=True)
+          )
+          (layer_norm1): LayerNorm((768,), eps=1e-05, elementwise_affine=True)
+          (mlp): CLIPMLP(
+            (activation_fn): QuickGELUActivation()
+            (fc1): Linear(in_features=768, out_features=3072, bias=True)
+            (fc2): Linear(in_features=3072, out_features=768, bias=True)
+          )
+          (layer_norm2): LayerNorm((768,), eps=1e-05, elementwise_affine=True)
+        )
+        (9): CLIPEncoderLayer(
+          (self_attn): CLIPAttention(
+            (k_proj): Linear(in_features=768, out_features=768, bias=True)
+            (v_proj): Linear(in_features=768, out_features=768, bias=True)
+            (q_proj): Linear(in_features=768, out_features=768, bias=True)
+            (out_proj): Linear(in_features=768, out_features=768, bias=True)
+          )
+          (layer_norm1): LayerNorm((768,), eps=1e-05, elementwise_affine=True)
+          (mlp): CLIPMLP(
+            (activation_fn): QuickGELUActivation()
+            (fc1): Linear(in_features=768, out_features=3072, bias=True)
+            (fc2): Linear(in_features=3072, out_features=768, bias=True)
+          )
+          (layer_norm2): LayerNorm((768,), eps=1e-05, elementwise_affine=True)
+        )
+        (10): CLIPEncoderLayer(
+          (self_attn): CLIPAttention(
+            (k_proj): Linear(in_features=768, out_features=768, bias=True)
+            (v_proj): Linear(in_features=768, out_features=768, bias=True)
+            (q_proj): Linear(in_features=768, out_features=768, bias=True)
+            (out_proj): Linear(in_features=768, out_features=768, bias=True)
+          )
+          (layer_norm1): LayerNorm((768,), eps=1e-05, elementwise_affine=True)
+          (mlp): CLIPMLP(
+            (activation_fn): QuickGELUActivation()
+            (fc1): Linear(in_features=768, out_features=3072, bias=True)
+            (fc2): Linear(in_features=3072, out_features=768, bias=True)
+          )
+          (layer_norm2): LayerNorm((768,), eps=1e-05, elementwise_affine=True)
+        )
+        (11): CLIPEncoderLayer(
+          (self_attn): CLIPAttention(
+            (k_proj): Linear(in_features=768, out_features=768, bias=True)
+            (v_proj): Linear(in_features=768, out_features=768, bias=True)
+            (q_proj): Linear(in_features=768, out_features=768, bias=True)
+            (out_proj): Linear(in_features=768, out_features=768, bias=True)
+          )
+          (layer_norm1): LayerNorm((768,), eps=1e-05, elementwise_affine=True)
+          (mlp): CLIPMLP(
+            (activation_fn): QuickGELUActivation()
+            (fc1): Linear(in_features=768, out_features=3072, bias=True)
+            (fc2): Linear(in_features=3072, out_features=768, bias=True)
+          )
+          (layer_norm2): LayerNorm((768,), eps=1e-05, elementwise_affine=True)
+        )
+      )
+    )
+    (final_layer_norm): LayerNorm((768,), eps=1e-05, elementwise_affine=True)
+  )
+)
```

### Comparing `hcpdiff-0.2.2/cfgs/train/examples/CustomDiffusion.yaml` & `hcpdiff-0.3.0/cfgs/train/examples/TextualInversion.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -1,73 +1,43 @@
-_base_: [cfgs/train/train_base.yaml, cfgs/train/tuning_base.yaml]
-
-unet:
-  -
-    lr: 1e-6
-    layers:
-      - 're:.*\.to_k$'
-      - 're:.*\.to_v$'
-
-## lora version of CustomDiffusion
-#lora_unet:
-#  -
-#    lr: 1e-4
-#    layers:
-#      - 're:.*\.to_k$'
-#      - 're:.*\.to_v$'
-
-tokenizer_pt:
-  train: # prompt tuning embeddings, needs to be created in advance
-    - { name: 'pt-dog1', lr: 0.003 }
-
-train:
-  gradient_accumulation_steps: 1
-  save_step: 100
-
-  scheduler:
-    name: 'constant_with_warmup'
-    num_warmup_steps: 50
-    num_training_steps: 600
-
-model:
-  pretrained_model_name_or_path: 'runwayml/stable-diffusion-v1-5'
-  tokenizer_repeats: 1
-  ema_unet: 0
-  ema_text_encoder: 0
-
-data:
-  batch_size: 4
-  prompt_template: 'prompt_tuning_template/object.txt'
-  caption_file: null
-  cache_latents: True
-  tag_transforms:
-    transforms:
-      - _target_: hcpdiff.utils.caption_tools.TagShuffle
-      - _target_: hcpdiff.utils.caption_tools.TagDropout
-        p: 0.1
-      - _target_: hcpdiff.utils.caption_tools.TemplateFill
-        word_names:
-          pt1: pt-dog1
-          class: dog
-  bucket:
-    _target_: hcpdiff.data.bucket.RatioBucket.from_files
-    img_root: 'imgs/'
-    target_area: {_target_: "builtins.eval", _args_: ['512*512']}
-    num_bucket: 1
-
-data_class:
-  batch_size: 1
-  prompt_template: 'prompt_tuning_template/object.txt'
-  caption_file: null
-  cache_latents: True
-  tag_transforms:
-    transforms:
-      - _target_: hcpdiff.utils.caption_tools.TagShuffle
-      - _target_: hcpdiff.utils.caption_tools.TagDropout
-        p: 0.1
-      - _target_: hcpdiff.utils.caption_tools.TemplateFill
-        word_names: # class word only
-          class: dog
-  bucket:
-    _target_: hcpdiff.data.bucket.FixedBucket
-    img_root: 'db/dog'
-    target_size: 512
+_base_: [cfgs/train/train_base.yaml, cfgs/train/tuning_base.yaml]
+
+tokenizer_pt:
+  train: # prompt tuning embeddings, needs to be created in advance
+    - { name: 'pt-catgirl1', lr: 0.003 }
+
+train:
+  gradient_accumulation_steps: 1
+  save_step: 100
+
+  scheduler:
+    name: 'constant_with_warmup'
+    num_warmup_steps: 50
+    num_training_steps: 600
+
+model:
+  pretrained_model_name_or_path: 'runwayml/stable-diffusion-v1-5'
+  tokenizer_repeats: 1
+  ema_unet: 0
+  ema_text_encoder: 0
+
+data:
+  dataset1:
+    batch_size: 4
+    cache_latents: True
+
+    source:
+      data_source1:
+        img_root: 'imgs/'
+        prompt_template: 'prompt_tuning_template/object.txt'
+        caption_file: null # path to image captions (file_words)
+        tag_transforms:
+          transforms:
+            - _target_: hcpdiff.utils.caption_tools.TagShuffle
+            - _target_: hcpdiff.utils.caption_tools.TagDropout
+              p: 0.1
+            - _target_: hcpdiff.utils.caption_tools.TemplateFill
+              word_names:
+                pt1: pt-catgirl1
+    bucket:
+      _target_: hcpdiff.data.bucket.RatioBucket.from_files # aspect ratio bucket
+      target_area: {_target_: "builtins.eval", _args_: ['512*512']}
+      num_bucket: 5
```

### Comparing `hcpdiff-0.2.2/cfgs/train/examples/DreamArtist.yaml` & `hcpdiff-0.3.0/cfgs/train/examples/DreamArtist.yaml`

 * *Files 23% similar despite different names*

```diff
@@ -1,45 +1,47 @@
-_base_: [cfgs/train/train_base.yaml, cfgs/train/tuning_base.yaml]
-
-tokenizer_pt:
-  train: # prompt tuning embeddings, needs to be created in advance
-    - { name: 'pt-catgirl1', lr: 0.003 }
-    - { name: 'pt-catgirl1-neg', lr: 0.003 }
-
-train:
-  gradient_accumulation_steps: 1
-  save_step: 100
-
-  #cfg_scale: '1.0-3.0:cos' # dynamic CFG with timestamp
-  cfg_scale: '3.0'
-
-  scheduler:
-    name: 'constant_with_warmup'
-    num_warmup_steps: 50
-    num_training_steps: 600
-
-model:
-  pretrained_model_name_or_path: 'runwayml/stable-diffusion-v1-5'
-  tokenizer_repeats: 1
-  ema_unet: 0
-  ema_text_encoder: 0
-
-data:
-  batch_size: 4
-  prompt_template: 'prompt_tuning_template/object.txt'
-  caption_file: null
-  cache_latents: True
-  tag_transforms:
-    transforms:
-      - _target_: hcpdiff.utils.caption_tools.TagShuffle
-      - _target_: hcpdiff.utils.caption_tools.TagDropout
-        p: 0.1
-      - _target_: hcpdiff.utils.caption_tools.TemplateFill
-        word_names:
-          pt1: [pt-catgirl1, pt-catgirl1-neg] # A pair of word for positive and negative branches respectively.
-  bucket:
-    _target_: hcpdiff.data.bucket.RatioBucket.from_files # aspect ratio bucket
-    img_root: 'imgs/'
-    target_area: {_target_: "builtins.eval", _args_: ['512*512']}
-    num_bucket: 1
-
-data_class: null
+_base_: [cfgs/train/train_base.yaml, cfgs/train/tuning_base.yaml]
+
+tokenizer_pt:
+  train: # prompt tuning embeddings, needs to be created in advance
+    - { name: 'pt-catgirl1', lr: 0.003 }
+    - { name: 'pt-catgirl1-neg', lr: 0.003 }
+
+train:
+  gradient_accumulation_steps: 1
+  save_step: 100
+
+  #cfg_scale: '1.0-3.0:cos' # dynamic CFG with timestamp
+  cfg_scale: '3.0'
+
+  scheduler:
+    name: 'constant_with_warmup'
+    num_warmup_steps: 50
+    num_training_steps: 600
+
+model:
+  pretrained_model_name_or_path: 'runwayml/stable-diffusion-v1-5'
+  tokenizer_repeats: 1
+  ema_unet: 0
+  ema_text_encoder: 0
+
+data:
+  dataset1:
+    batch_size: 4
+    cache_latents: True
+
+    source:
+      data_source1:
+        img_root: 'imgs/'
+        prompt_template: 'prompt_tuning_template/object.txt'
+        caption_file: null # path to image captions (file_words)
+        tag_transforms:
+          transforms:
+            - _target_: hcpdiff.utils.caption_tools.TagShuffle
+            - _target_: hcpdiff.utils.caption_tools.TagDropout
+              p: 0.1
+            - _target_: hcpdiff.utils.caption_tools.TemplateFill
+              word_names:
+                pt1: [pt-catgirl1, pt-catgirl1-neg] # A pair of word for positive and negative branches respectively.
+    bucket:
+      _target_: hcpdiff.data.bucket.RatioBucket.from_files # aspect ratio bucket
+      target_area: {_target_: "builtins.eval", _args_: ['512*512']}
+      num_bucket: 5
```

### Comparing `hcpdiff-0.2.2/cfgs/train/examples/controlnet.yaml` & `hcpdiff-0.3.0/cfgs/train/examples/min_snr.yaml`

 * *Files 24% similar despite different names*

```diff
@@ -1,41 +1,58 @@
-_base_:
-  - cfgs/train/train_base.yaml
-  - cfgs/plugins/plugin_controlnet.yaml # include controlnet plugin
-
-tokenizer_pt:
-  train: null
-
-train:
-  gradient_accumulation_steps: 1
-  save_step: 100
-
-  scheduler:
-    name: 'constant_with_warmup'
-    num_warmup_steps: 50
-    num_training_steps: 600
-
-model:
-  pretrained_model_name_or_path: 'runwayml/stable-diffusion-v1-5'
-  tokenizer_repeats: 1
-  ema_unet: 0
-  ema_text_encoder: 0
-
-data:
-  batch_size: 4
-  prompt_template: 'prompt_tuning_template/object.txt'
-  caption_file: null
-  cache_latents: True
-  tag_transforms:
-    transforms:
-      - _target_: hcpdiff.utils.caption_tools.TagShuffle
-      - _target_: hcpdiff.utils.caption_tools.TagDropout
-        p: 0.1
-      - _target_: hcpdiff.utils.caption_tools.TemplateFill
-        word_names: {}
-  bucket:
-    _target_: hcpdiff.data.bucket.RatioBucket.from_files # aspect ratio bucket
-    img_root: 'imgs/'
-    target_area: {_target_: "builtins.eval", _args_: ['512*512']}
-    num_bucket: 10
-
-data_class: null
+_base_: [cfgs/train/train_base.yaml, cfgs/train/tuning_base.yaml]
+
+unet:
+  -
+    lr: 1e-6
+    layers:
+      - '' # fine-tuning all layers in unet
+
+## fine-tuning text-encoder
+#text_encoder:
+#  - lr: 1e-6
+#    layers:
+#      - ''
+
+tokenizer_pt:
+  train: null
+
+train:
+  gradient_accumulation_steps: 1
+  save_step: 100
+
+  loss:
+    criterion: # min SNR loss
+      _target_: hcpdiff.loss.MinSNRLoss
+      gamma: 2.0
+
+  scheduler:
+    name: 'constant_with_warmup'
+    num_warmup_steps: 50
+    num_training_steps: 600
+
+model:
+  pretrained_model_name_or_path: 'runwayml/stable-diffusion-v1-5'
+  tokenizer_repeats: 1
+  ema_unet: 0
+  ema_text_encoder: 0
+
+data:
+  dataset1:
+    batch_size: 4
+    cache_latents: True
+
+    source:
+      data_source1:
+        img_root: 'imgs/'
+        prompt_template: 'prompt_tuning_template/object.txt'
+        caption_file: null # path to image captions (file_words)
+        tag_transforms:
+          transforms:
+            - _target_: hcpdiff.utils.caption_tools.TagShuffle
+            - _target_: hcpdiff.utils.caption_tools.TagDropout
+              p: 0.1
+            - _target_: hcpdiff.utils.caption_tools.TemplateFill
+              word_names: { }
+    bucket:
+      _target_: hcpdiff.data.bucket.RatioBucket.from_files # aspect ratio bucket
+      target_area: {_target_: "builtins.eval", _args_: ['512*512']}
+      num_bucket: 5
```

### Comparing `hcpdiff-0.2.2/cfgs/train/examples/fine-tuning.yaml` & `hcpdiff-0.3.0/cfgs/train/examples/controlnet.yaml`

 * *Files 19% similar despite different names*

```diff
@@ -1,51 +1,43 @@
-_base_: [cfgs/train/train_base.yaml, cfgs/train/tuning_base.yaml]
-
-unet:
-  -
-    lr: 1e-6
-    layers:
-      - '' # fine-tuning all layers in unet
-
-## fine-tuning text-encoder
-#text_encoder:
-#  - lr: 1e-6
-#    layers:
-#      - ''
-
-tokenizer_pt:
-  train: null
-
-train:
-  gradient_accumulation_steps: 1
-  save_step: 100
-
-  scheduler:
-    name: 'constant_with_warmup'
-    num_warmup_steps: 50
-    num_training_steps: 600
-
-model:
-  pretrained_model_name_or_path: 'runwayml/stable-diffusion-v1-5'
-  tokenizer_repeats: 1
-  ema_unet: 0
-  ema_text_encoder: 0
-
-data:
-  batch_size: 4
-  prompt_template: 'prompt_tuning_template/object.txt'
-  caption_file: null
-  cache_latents: True
-  tag_transforms:
-    transforms:
-      - _target_: hcpdiff.utils.caption_tools.TagShuffle
-      - _target_: hcpdiff.utils.caption_tools.TagDropout
-        p: 0.1
-      - _target_: hcpdiff.utils.caption_tools.TemplateFill
-        word_names: {}
-  bucket:
-    _target_: hcpdiff.data.bucket.RatioBucket.from_files # aspect ratio bucket
-    img_root: 'imgs/'
-    target_area: {_target_: "builtins.eval", _args_: ['512*512']}
-    num_bucket: 10
-
-data_class: null
+_base_:
+  - cfgs/train/train_base.yaml
+  - cfgs/plugins/plugin_controlnet.yaml # include controlnet plugin
+
+tokenizer_pt:
+  train: null
+
+train:
+  gradient_accumulation_steps: 1
+  save_step: 100
+
+  scheduler:
+    name: 'constant_with_warmup'
+    num_warmup_steps: 50
+    num_training_steps: 600
+
+model:
+  pretrained_model_name_or_path: 'runwayml/stable-diffusion-v1-5'
+  tokenizer_repeats: 1
+  ema_unet: 0
+  ema_text_encoder: 0
+
+data:
+  dataset1:
+    batch_size: 4
+    cache_latents: True
+
+    source:
+      data_source1:
+        img_root: 'imgs/'
+        prompt_template: 'prompt_tuning_template/object.txt'
+        caption_file: null # path to image captions (file_words)
+        tag_transforms:
+          transforms:
+            - _target_: hcpdiff.utils.caption_tools.TagShuffle
+            - _target_: hcpdiff.utils.caption_tools.TagDropout
+              p: 0.1
+            - _target_: hcpdiff.utils.caption_tools.TemplateFill
+              word_names: { }
+    bucket:
+      _target_: hcpdiff.data.bucket.RatioBucket.from_files # aspect ratio bucket
+      target_area: {_target_: "builtins.eval", _args_: ['512*512']}
+      num_bucket: 5
```

### Comparing `hcpdiff-0.2.2/cfgs/train/examples/lora_conventional.yaml` & `hcpdiff-0.3.0/cfgs/train/examples/lora_conventional.yaml`

 * *Files 17% similar despite different names*

```diff
@@ -1,54 +1,56 @@
-_base_: [cfgs/train/train_base.yaml, cfgs/train/tuning_base.yaml]
-
-lora_unet:
-  -
-    lr: 1e-4
-    rank: 8
-    layers:
-      - 're:.*\.attn.?$'
-      - 're:.*\.ff\.net\.0$'
-
-lora_text_encoder:
-  - lr: 1e-5
-    rank: 4
-    layers:
-      - 're:.*self_attn$'
-      - 're:.*mlp$'
-
-tokenizer_pt:
-  train: null
-
-train:
-  gradient_accumulation_steps: 1
-  save_step: 100
-
-  scheduler:
-    name: 'constant_with_warmup'
-    num_warmup_steps: 50
-    num_training_steps: 600
-
-model:
-  pretrained_model_name_or_path: 'runwayml/stable-diffusion-v1-5'
-  tokenizer_repeats: 1
-  ema_unet: 0
-  ema_text_encoder: 0
-
-data:
-  batch_size: 4
-  prompt_template: 'prompt_tuning_template/object.txt'
-  caption_file: null
-  cache_latents: True
-  tag_transforms:
-    transforms:
-      - _target_: hcpdiff.utils.caption_tools.TagShuffle
-      - _target_: hcpdiff.utils.caption_tools.TagDropout
-        p: 0.1
-      - _target_: hcpdiff.utils.caption_tools.TemplateFill
-        word_names: {}
-  bucket:
-    _target_: hcpdiff.data.bucket.RatioBucket.from_files # aspect ratio bucket
-    img_root: 'imgs/'
-    target_area: {_target_: "builtins.eval", _args_: ['512*512']}
-    num_bucket: 10
-
-data_class: null
+_base_: [cfgs/train/train_base.yaml, cfgs/train/tuning_base.yaml]
+
+lora_unet:
+  -
+    lr: 1e-4
+    rank: 8
+    layers:
+      - 're:.*\.attn.?$'
+      - 're:.*\.ff\.net\.0$'
+
+lora_text_encoder:
+  - lr: 1e-5
+    rank: 4
+    layers:
+      - 're:.*self_attn$'
+      - 're:.*mlp$'
+
+tokenizer_pt:
+  train: null
+
+train:
+  gradient_accumulation_steps: 1
+  save_step: 100
+
+  scheduler:
+    name: 'constant_with_warmup'
+    num_warmup_steps: 50
+    num_training_steps: 600
+
+model:
+  pretrained_model_name_or_path: 'runwayml/stable-diffusion-v1-5'
+  tokenizer_repeats: 1
+  ema_unet: 0
+  ema_text_encoder: 0
+
+data:
+  dataset1:
+    batch_size: 4
+    cache_latents: True
+
+    source:
+      data_source1:
+        img_root: 'imgs/'
+        prompt_template: 'prompt_tuning_template/object.txt'
+        caption_file: null # path to image captions (file_words)
+        tag_transforms:
+          transforms:
+            - _target_: hcpdiff.utils.caption_tools.TagShuffle
+            - _target_: hcpdiff.utils.caption_tools.TagDropout
+              p: 0.1
+            - _target_: hcpdiff.utils.caption_tools.TemplateFill
+              word_names: { }
+    bucket:
+      _target_: hcpdiff.data.bucket.RatioBucket.from_files # aspect ratio bucket
+      target_area: {_target_: "builtins.eval", _args_: ['512*512']}
+      num_bucket: 5
```

### Comparing `hcpdiff-0.2.2/cfgs/train/train_base.yaml` & `hcpdiff-0.3.0/cfgs/train/train_base.yaml`

 * *Files 22% similar despite different names*

```diff
@@ -1,109 +1,104 @@
-
-exp_dir: exps/
-mixed_precision: 'fp16'
-allow_tf32: False
-seed: 114514
-ckpt_type: 'safetensors' # [torch, safetensors]
-
-vis_info:
-  prompt: null
-  negative_prompt: ''
-
-train:
-  gradient_accumulation_steps: 1
-  workers: 4
-  max_grad_norm: 1.0
-  set_grads_to_none: False
-  save_step: 100
-  log_step: 20
-  cfg_scale: '1.0' # for DreamArtist
-
-  resume: null
-#  resume:
-#    ckpt_path:
-#      unet: []
-#      TE: []
-#      words: {}
-#    start_step: 0
-
-  loss:
-    criterion:
-      _target_: torch.nn.MSELoss
-      reduction: 'none' # support for attention mask
-    prior_loss_weight: 1.0
-    type: 'eps' # 'eps' or 'sample'
-
-  optimizer:
-    type: adamw
-    weight_decay: 1e-3
-    weight_decay_pt: 5e-4
-
-  scale_lr: True # auto scale lr with total batch size
-  scheduler:
-    name: 'one_cycle'
-    num_warmup_steps: 200
-    num_training_steps: 1000
-    scheduler_kwargs: {} # args for scheduler
-
-  scale_lr_pt: True
-  scheduler_pt: ${.scheduler}
-
-model:
-  revision: null
-  pretrained_model_name_or_path: null
-  tokenizer_name: null
-  tokenizer_repeats: 3
-  enable_xformers: True
-  gradient_checkpointing: True
-  ema_unet: 0 # 0 to disable
-  ema_text_encoder: 0 # 0 to disable
-  clip_skip: 0
-
-  noise_scheduler: DDPMScheduler
-
-data:
-  _target_: hcpdiff.data.TextImagePairDataset
-  _partial_: True # Not directly instantiate the object here. There are other parameters to be added in the runtime.
-  batch_size: 4
-  prompt_template: 'prompt_tuning_template/name.txt'
-  caption_file: null # path to image captions (file_words)
-  cache_latents: True
-  att_mask: null
-  att_mask_encode: False
-  bg_color: [255, 255, 255] # RGB; for ARGB -> RGB
-  image_transforms:
-    _target_: torchvision.transforms.Compose # "_target_" for hydra.utils.instantiate
-    transforms:
-      - _target_: torchvision.transforms.ToTensor
-      - _target_: torchvision.transforms.Normalize
-        _args_: [[0.5], [0.5]]
-  tag_transforms:
-    _target_: torchvision.transforms.Compose
-    transforms:
-      - _target_: hcpdiff.utils.caption_tools.TagShuffle
-      - _target_: hcpdiff.utils.caption_tools.TagDropout
-        p: 0.1
-      - _target_: hcpdiff.utils.caption_tools.TemplateFill
-        word_names: {} # Replace placeholders with specific words or embeddings
-  bucket:
-    _target_: hcpdiff.data.bucket.RatioBucket.from_files # aspect ratio bucket
-    img_root: 'imgs/train' # images directory of train images
-    target_area: {_target_: "builtins.eval", _args_: ['512*512']} # Expected area of training images: width * height
-    num_bucket: 5
-
-data_class: # for DreamBooth
-  _target_: hcpdiff.data.TextImagePairDataset
-  _partial_: True
-  batch_size: 1
-  prompt_template: 'prompt_tuning_template/name.txt'
-  caption_file: null
-  cache_latents: True
-  att_mask: null
-  att_mask_encode: False
-  bg_color: [255, 255, 255] # RGB; for ARGB -> RGB
-  image_transforms: ${..data.image_transforms}
-  tag_transforms: ${..data.tag_transforms}
-  bucket:
-    _target_: hcpdiff.data.bucket.FixedBucket # aspect ratio bucket
-    img_root: 'imgs/train_class'
-    target_size: [512, 512]
+
+exp_dir: exps/
+mixed_precision: 'fp16'
+allow_tf32: False
+seed: 114514
+ckpt_type: 'safetensors' # [torch, safetensors]
+
+vis_info:
+  prompt: null
+  negative_prompt: ''
+
+train:
+  gradient_accumulation_steps: 1
+  workers: 4
+  max_grad_norm: 1.0
+  set_grads_to_none: False
+  save_step: 100
+  cfg_scale: '1.0' # for DreamArtist
+
+  resume: null
+#  resume:
+#    ckpt_path:
+#      unet: []
+#      TE: []
+#      words: {}
+#    start_step: 0
+
+  loss:
+    criterion:
+      _target_: hcpdiff.loss.MSELoss
+      _partial_: True
+      reduction: 'none' # support for attention mask
+    type: 'eps' # 'eps' or 'sample'
+
+  optimizer:
+    type: adamw
+    weight_decay: 1e-3
+    weight_decay_pt: 5e-4
+
+  scale_lr: True # auto scale lr with total batch size
+  scheduler:
+    name: 'one_cycle'
+    num_warmup_steps: 200
+    num_training_steps: 1000
+    scheduler_kwargs: {} # args for scheduler
+
+  scale_lr_pt: True
+  scheduler_pt: ${.scheduler}
+
+logger:
+  -
+    _target_: hcpdiff.loggers.CLILogger
+    _partial_: True
+    out_path: 'train.log'
+    log_step: 20
+
+model:
+  revision: null
+  pretrained_model_name_or_path: null
+  tokenizer_name: null
+  tokenizer_repeats: 3
+  enable_xformers: True
+  gradient_checkpointing: True
+  ema_unet: 0 # 0 to disable
+  ema_text_encoder: 0 # 0 to disable
+  clip_skip: 0
+  noise_scheduler: DDPMScheduler
+
+data:
+  dataset1:
+    _target_: hcpdiff.data.TextImagePairDataset
+    _partial_: True # Not directly instantiate the object here. There are other parameters to be added in the runtime.
+    batch_size: 4
+    cache_latents: True
+    att_mask_encode: False
+    loss_weight: 1.0
+
+    image_transforms:
+      _target_: torchvision.transforms.Compose # "_target_" for hydra.utils.instantiate
+      transforms:
+        - _target_: torchvision.transforms.ToTensor
+        - _target_: torchvision.transforms.Normalize
+          _args_: [ [ 0.5 ], [ 0.5 ] ]
+
+    source:
+      data_source1:
+        img_root: 'imgs/train' # images directory of train images
+        prompt_template: 'prompt_tuning_template/object.txt'
+        caption_file: null # path to image captions (file_words)
+        att_mask: null
+        bg_color: [255, 255, 255] # RGB; for ARGB -> RGB
+        image_transforms: ${...image_transforms}
+        tag_transforms:
+          _target_: torchvision.transforms.Compose
+          transforms:
+            - _target_: hcpdiff.utils.caption_tools.TagShuffle
+            - _target_: hcpdiff.utils.caption_tools.TagDropout
+              p: 0.1
+            - _target_: hcpdiff.utils.caption_tools.TemplateFill
+              word_names: {} # Replace placeholders with specific words or embeddings
+    bucket:
+      _target_: hcpdiff.data.bucket.RatioBucket.from_files # aspect ratio bucket
+      target_area: {_target_: "builtins.eval", _args_: ['512*512']} # Expected area of training images: width * height
+      num_bucket: 5
```

### Comparing `hcpdiff-0.2.2/cfgs/unet_struct.txt` & `hcpdiff-0.3.0/cfgs/unet_struct.txt`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,932 +1,932 @@
-UNet2DConditionModel(
-  (conv_in): Conv2d(4, 320, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1))
-  (time_proj): Timesteps()
-  (time_embedding): TimestepEmbedding(
-    (linear_1): Linear(in_features=320, out_features=1280, bias=True)
-    (act): SiLU()
-    (linear_2): Linear(in_features=1280, out_features=1280, bias=True)
-  )
-  (down_blocks): ModuleList(
-    (0): CrossAttnDownBlock2D(
-      (attentions): ModuleList(
-        (0): Transformer2DModel(
-          (norm): GroupNorm(32, 320, eps=1e-06, affine=True)
-          (proj_in): Conv2d(320, 320, kernel_size=(1, 1), stride=(1, 1))
-          (transformer_blocks): ModuleList(
-            (0): BasicTransformerBlock(
-              (attn1): CrossAttention(
-                (to_q): Linear(in_features=320, out_features=320, bias=False)
-                (to_k): Linear(in_features=320, out_features=320, bias=False)
-                (to_v): Linear(in_features=320, out_features=320, bias=False)
-                (to_out): ModuleList(
-                  (0): Linear(in_features=320, out_features=320, bias=True)
-                  (1): Dropout(p=0.0, inplace=False)
-                )
-              )
-              (ff): FeedForward(
-                (net): ModuleList(
-                  (0): GEGLU(
-                    (proj): Linear(in_features=320, out_features=2560, bias=True)
-                  )
-                  (1): Dropout(p=0.0, inplace=False)
-                  (2): Linear(in_features=1280, out_features=320, bias=True)
-                )
-              )
-              (attn2): CrossAttention(
-                (to_q): Linear(in_features=320, out_features=320, bias=False)
-                (to_k): Linear(in_features=768, out_features=320, bias=False)
-                (to_v): Linear(in_features=768, out_features=320, bias=False)
-                (to_out): ModuleList(
-                  (0): Linear(in_features=320, out_features=320, bias=True)
-                  (1): Dropout(p=0.0, inplace=False)
-                )
-              )
-              (norm1): LayerNorm((320,), eps=1e-05, elementwise_affine=True)
-              (norm2): LayerNorm((320,), eps=1e-05, elementwise_affine=True)
-              (norm3): LayerNorm((320,), eps=1e-05, elementwise_affine=True)
-            )
-          )
-          (proj_out): Conv2d(320, 320, kernel_size=(1, 1), stride=(1, 1))
-        )
-        (1): Transformer2DModel(
-          (norm): GroupNorm(32, 320, eps=1e-06, affine=True)
-          (proj_in): Conv2d(320, 320, kernel_size=(1, 1), stride=(1, 1))
-          (transformer_blocks): ModuleList(
-            (0): BasicTransformerBlock(
-              (attn1): CrossAttention(
-                (to_q): Linear(in_features=320, out_features=320, bias=False)
-                (to_k): Linear(in_features=320, out_features=320, bias=False)
-                (to_v): Linear(in_features=320, out_features=320, bias=False)
-                (to_out): ModuleList(
-                  (0): Linear(in_features=320, out_features=320, bias=True)
-                  (1): Dropout(p=0.0, inplace=False)
-                )
-              )
-              (ff): FeedForward(
-                (net): ModuleList(
-                  (0): GEGLU(
-                    (proj): Linear(in_features=320, out_features=2560, bias=True)
-                  )
-                  (1): Dropout(p=0.0, inplace=False)
-                  (2): Linear(in_features=1280, out_features=320, bias=True)
-                )
-              )
-              (attn2): CrossAttention(
-                (to_q): Linear(in_features=320, out_features=320, bias=False)
-                (to_k): Linear(in_features=768, out_features=320, bias=False)
-                (to_v): Linear(in_features=768, out_features=320, bias=False)
-                (to_out): ModuleList(
-                  (0): Linear(in_features=320, out_features=320, bias=True)
-                  (1): Dropout(p=0.0, inplace=False)
-                )
-              )
-              (norm1): LayerNorm((320,), eps=1e-05, elementwise_affine=True)
-              (norm2): LayerNorm((320,), eps=1e-05, elementwise_affine=True)
-              (norm3): LayerNorm((320,), eps=1e-05, elementwise_affine=True)
-            )
-          )
-          (proj_out): Conv2d(320, 320, kernel_size=(1, 1), stride=(1, 1))
-        )
-      )
-      (resnets): ModuleList(
-        (0): ResnetBlock2D(
-          (norm1): GroupNorm(32, 320, eps=1e-05, affine=True)
-          (conv1): Conv2d(320, 320, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1))
-          (time_emb_proj): Linear(in_features=1280, out_features=320, bias=True)
-          (norm2): GroupNorm(32, 320, eps=1e-05, affine=True)
-          (dropout): Dropout(p=0.0, inplace=False)
-          (conv2): Conv2d(320, 320, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1))
-          (nonlinearity): SiLU()
-        )
-        (1): ResnetBlock2D(
-          (norm1): GroupNorm(32, 320, eps=1e-05, affine=True)
-          (conv1): Conv2d(320, 320, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1))
-          (time_emb_proj): Linear(in_features=1280, out_features=320, bias=True)
-          (norm2): GroupNorm(32, 320, eps=1e-05, affine=True)
-          (dropout): Dropout(p=0.0, inplace=False)
-          (conv2): Conv2d(320, 320, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1))
-          (nonlinearity): SiLU()
-        )
-      )
-      (downsamplers): ModuleList(
-        (0): Downsample2D(
-          (conv): Conv2d(320, 320, kernel_size=(3, 3), stride=(2, 2), padding=(1, 1))
-        )
-      )
-    )
-    (1): CrossAttnDownBlock2D(
-      (attentions): ModuleList(
-        (0): Transformer2DModel(
-          (norm): GroupNorm(32, 640, eps=1e-06, affine=True)
-          (proj_in): Conv2d(640, 640, kernel_size=(1, 1), stride=(1, 1))
-          (transformer_blocks): ModuleList(
-            (0): BasicTransformerBlock(
-              (attn1): CrossAttention(
-                (to_q): Linear(in_features=640, out_features=640, bias=False)
-                (to_k): Linear(in_features=640, out_features=640, bias=False)
-                (to_v): Linear(in_features=640, out_features=640, bias=False)
-                (to_out): ModuleList(
-                  (0): Linear(in_features=640, out_features=640, bias=True)
-                  (1): Dropout(p=0.0, inplace=False)
-                )
-              )
-              (ff): FeedForward(
-                (net): ModuleList(
-                  (0): GEGLU(
-                    (proj): Linear(in_features=640, out_features=5120, bias=True)
-                  )
-                  (1): Dropout(p=0.0, inplace=False)
-                  (2): Linear(in_features=2560, out_features=640, bias=True)
-                )
-              )
-              (attn2): CrossAttention(
-                (to_q): Linear(in_features=640, out_features=640, bias=False)
-                (to_k): Linear(in_features=768, out_features=640, bias=False)
-                (to_v): Linear(in_features=768, out_features=640, bias=False)
-                (to_out): ModuleList(
-                  (0): Linear(in_features=640, out_features=640, bias=True)
-                  (1): Dropout(p=0.0, inplace=False)
-                )
-              )
-              (norm1): LayerNorm((640,), eps=1e-05, elementwise_affine=True)
-              (norm2): LayerNorm((640,), eps=1e-05, elementwise_affine=True)
-              (norm3): LayerNorm((640,), eps=1e-05, elementwise_affine=True)
-            )
-          )
-          (proj_out): Conv2d(640, 640, kernel_size=(1, 1), stride=(1, 1))
-        )
-        (1): Transformer2DModel(
-          (norm): GroupNorm(32, 640, eps=1e-06, affine=True)
-          (proj_in): Conv2d(640, 640, kernel_size=(1, 1), stride=(1, 1))
-          (transformer_blocks): ModuleList(
-            (0): BasicTransformerBlock(
-              (attn1): CrossAttention(
-                (to_q): Linear(in_features=640, out_features=640, bias=False)
-                (to_k): Linear(in_features=640, out_features=640, bias=False)
-                (to_v): Linear(in_features=640, out_features=640, bias=False)
-                (to_out): ModuleList(
-                  (0): Linear(in_features=640, out_features=640, bias=True)
-                  (1): Dropout(p=0.0, inplace=False)
-                )
-              )
-              (ff): FeedForward(
-                (net): ModuleList(
-                  (0): GEGLU(
-                    (proj): Linear(in_features=640, out_features=5120, bias=True)
-                  )
-                  (1): Dropout(p=0.0, inplace=False)
-                  (2): Linear(in_features=2560, out_features=640, bias=True)
-                )
-              )
-              (attn2): CrossAttention(
-                (to_q): Linear(in_features=640, out_features=640, bias=False)
-                (to_k): Linear(in_features=768, out_features=640, bias=False)
-                (to_v): Linear(in_features=768, out_features=640, bias=False)
-                (to_out): ModuleList(
-                  (0): Linear(in_features=640, out_features=640, bias=True)
-                  (1): Dropout(p=0.0, inplace=False)
-                )
-              )
-              (norm1): LayerNorm((640,), eps=1e-05, elementwise_affine=True)
-              (norm2): LayerNorm((640,), eps=1e-05, elementwise_affine=True)
-              (norm3): LayerNorm((640,), eps=1e-05, elementwise_affine=True)
-            )
-          )
-          (proj_out): Conv2d(640, 640, kernel_size=(1, 1), stride=(1, 1))
-        )
-      )
-      (resnets): ModuleList(
-        (0): ResnetBlock2D(
-          (norm1): GroupNorm(32, 320, eps=1e-05, affine=True)
-          (conv1): Conv2d(320, 640, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1))
-          (time_emb_proj): Linear(in_features=1280, out_features=640, bias=True)
-          (norm2): GroupNorm(32, 640, eps=1e-05, affine=True)
-          (dropout): Dropout(p=0.0, inplace=False)
-          (conv2): Conv2d(640, 640, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1))
-          (nonlinearity): SiLU()
-          (conv_shortcut): Conv2d(320, 640, kernel_size=(1, 1), stride=(1, 1))
-        )
-        (1): ResnetBlock2D(
-          (norm1): GroupNorm(32, 640, eps=1e-05, affine=True)
-          (conv1): Conv2d(640, 640, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1))
-          (time_emb_proj): Linear(in_features=1280, out_features=640, bias=True)
-          (norm2): GroupNorm(32, 640, eps=1e-05, affine=True)
-          (dropout): Dropout(p=0.0, inplace=False)
-          (conv2): Conv2d(640, 640, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1))
-          (nonlinearity): SiLU()
-        )
-      )
-      (downsamplers): ModuleList(
-        (0): Downsample2D(
-          (conv): Conv2d(640, 640, kernel_size=(3, 3), stride=(2, 2), padding=(1, 1))
-        )
-      )
-    )
-    (2): CrossAttnDownBlock2D(
-      (attentions): ModuleList(
-        (0): Transformer2DModel(
-          (norm): GroupNorm(32, 1280, eps=1e-06, affine=True)
-          (proj_in): Conv2d(1280, 1280, kernel_size=(1, 1), stride=(1, 1))
-          (transformer_blocks): ModuleList(
-            (0): BasicTransformerBlock(
-              (attn1): CrossAttention(
-                (to_q): Linear(in_features=1280, out_features=1280, bias=False)
-                (to_k): Linear(in_features=1280, out_features=1280, bias=False)
-                (to_v): Linear(in_features=1280, out_features=1280, bias=False)
-                (to_out): ModuleList(
-                  (0): Linear(in_features=1280, out_features=1280, bias=True)
-                  (1): Dropout(p=0.0, inplace=False)
-                )
-              )
-              (ff): FeedForward(
-                (net): ModuleList(
-                  (0): GEGLU(
-                    (proj): Linear(in_features=1280, out_features=10240, bias=True)
-                  )
-                  (1): Dropout(p=0.0, inplace=False)
-                  (2): Linear(in_features=5120, out_features=1280, bias=True)
-                )
-              )
-              (attn2): CrossAttention(
-                (to_q): Linear(in_features=1280, out_features=1280, bias=False)
-                (to_k): Linear(in_features=768, out_features=1280, bias=False)
-                (to_v): Linear(in_features=768, out_features=1280, bias=False)
-                (to_out): ModuleList(
-                  (0): Linear(in_features=1280, out_features=1280, bias=True)
-                  (1): Dropout(p=0.0, inplace=False)
-                )
-              )
-              (norm1): LayerNorm((1280,), eps=1e-05, elementwise_affine=True)
-              (norm2): LayerNorm((1280,), eps=1e-05, elementwise_affine=True)
-              (norm3): LayerNorm((1280,), eps=1e-05, elementwise_affine=True)
-            )
-          )
-          (proj_out): Conv2d(1280, 1280, kernel_size=(1, 1), stride=(1, 1))
-        )
-        (1): Transformer2DModel(
-          (norm): GroupNorm(32, 1280, eps=1e-06, affine=True)
-          (proj_in): Conv2d(1280, 1280, kernel_size=(1, 1), stride=(1, 1))
-          (transformer_blocks): ModuleList(
-            (0): BasicTransformerBlock(
-              (attn1): CrossAttention(
-                (to_q): Linear(in_features=1280, out_features=1280, bias=False)
-                (to_k): Linear(in_features=1280, out_features=1280, bias=False)
-                (to_v): Linear(in_features=1280, out_features=1280, bias=False)
-                (to_out): ModuleList(
-                  (0): Linear(in_features=1280, out_features=1280, bias=True)
-                  (1): Dropout(p=0.0, inplace=False)
-                )
-              )
-              (ff): FeedForward(
-                (net): ModuleList(
-                  (0): GEGLU(
-                    (proj): Linear(in_features=1280, out_features=10240, bias=True)
-                  )
-                  (1): Dropout(p=0.0, inplace=False)
-                  (2): Linear(in_features=5120, out_features=1280, bias=True)
-                )
-              )
-              (attn2): CrossAttention(
-                (to_q): Linear(in_features=1280, out_features=1280, bias=False)
-                (to_k): Linear(in_features=768, out_features=1280, bias=False)
-                (to_v): Linear(in_features=768, out_features=1280, bias=False)
-                (to_out): ModuleList(
-                  (0): Linear(in_features=1280, out_features=1280, bias=True)
-                  (1): Dropout(p=0.0, inplace=False)
-                )
-              )
-              (norm1): LayerNorm((1280,), eps=1e-05, elementwise_affine=True)
-              (norm2): LayerNorm((1280,), eps=1e-05, elementwise_affine=True)
-              (norm3): LayerNorm((1280,), eps=1e-05, elementwise_affine=True)
-            )
-          )
-          (proj_out): Conv2d(1280, 1280, kernel_size=(1, 1), stride=(1, 1))
-        )
-      )
-      (resnets): ModuleList(
-        (0): ResnetBlock2D(
-          (norm1): GroupNorm(32, 640, eps=1e-05, affine=True)
-          (conv1): Conv2d(640, 1280, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1))
-          (time_emb_proj): Linear(in_features=1280, out_features=1280, bias=True)
-          (norm2): GroupNorm(32, 1280, eps=1e-05, affine=True)
-          (dropout): Dropout(p=0.0, inplace=False)
-          (conv2): Conv2d(1280, 1280, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1))
-          (nonlinearity): SiLU()
-          (conv_shortcut): Conv2d(640, 1280, kernel_size=(1, 1), stride=(1, 1))
-        )
-        (1): ResnetBlock2D(
-          (norm1): GroupNorm(32, 1280, eps=1e-05, affine=True)
-          (conv1): Conv2d(1280, 1280, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1))
-          (time_emb_proj): Linear(in_features=1280, out_features=1280, bias=True)
-          (norm2): GroupNorm(32, 1280, eps=1e-05, affine=True)
-          (dropout): Dropout(p=0.0, inplace=False)
-          (conv2): Conv2d(1280, 1280, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1))
-          (nonlinearity): SiLU()
-        )
-      )
-      (downsamplers): ModuleList(
-        (0): Downsample2D(
-          (conv): Conv2d(1280, 1280, kernel_size=(3, 3), stride=(2, 2), padding=(1, 1))
-        )
-      )
-    )
-    (3): DownBlock2D(
-      (resnets): ModuleList(
-        (0): ResnetBlock2D(
-          (norm1): GroupNorm(32, 1280, eps=1e-05, affine=True)
-          (conv1): Conv2d(1280, 1280, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1))
-          (time_emb_proj): Linear(in_features=1280, out_features=1280, bias=True)
-          (norm2): GroupNorm(32, 1280, eps=1e-05, affine=True)
-          (dropout): Dropout(p=0.0, inplace=False)
-          (conv2): Conv2d(1280, 1280, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1))
-          (nonlinearity): SiLU()
-        )
-        (1): ResnetBlock2D(
-          (norm1): GroupNorm(32, 1280, eps=1e-05, affine=True)
-          (conv1): Conv2d(1280, 1280, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1))
-          (time_emb_proj): Linear(in_features=1280, out_features=1280, bias=True)
-          (norm2): GroupNorm(32, 1280, eps=1e-05, affine=True)
-          (dropout): Dropout(p=0.0, inplace=False)
-          (conv2): Conv2d(1280, 1280, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1))
-          (nonlinearity): SiLU()
-        )
-      )
-    )
-  )
-  (up_blocks): ModuleList(
-    (0): UpBlock2D(
-      (resnets): ModuleList(
-        (0): ResnetBlock2D(
-          (norm1): GroupNorm(32, 2560, eps=1e-05, affine=True)
-          (conv1): Conv2d(2560, 1280, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1))
-          (time_emb_proj): Linear(in_features=1280, out_features=1280, bias=True)
-          (norm2): GroupNorm(32, 1280, eps=1e-05, affine=True)
-          (dropout): Dropout(p=0.0, inplace=False)
-          (conv2): Conv2d(1280, 1280, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1))
-          (nonlinearity): SiLU()
-          (conv_shortcut): Conv2d(2560, 1280, kernel_size=(1, 1), stride=(1, 1))
-        )
-        (1): ResnetBlock2D(
-          (norm1): GroupNorm(32, 2560, eps=1e-05, affine=True)
-          (conv1): Conv2d(2560, 1280, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1))
-          (time_emb_proj): Linear(in_features=1280, out_features=1280, bias=True)
-          (norm2): GroupNorm(32, 1280, eps=1e-05, affine=True)
-          (dropout): Dropout(p=0.0, inplace=False)
-          (conv2): Conv2d(1280, 1280, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1))
-          (nonlinearity): SiLU()
-          (conv_shortcut): Conv2d(2560, 1280, kernel_size=(1, 1), stride=(1, 1))
-        )
-        (2): ResnetBlock2D(
-          (norm1): GroupNorm(32, 2560, eps=1e-05, affine=True)
-          (conv1): Conv2d(2560, 1280, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1))
-          (time_emb_proj): Linear(in_features=1280, out_features=1280, bias=True)
-          (norm2): GroupNorm(32, 1280, eps=1e-05, affine=True)
-          (dropout): Dropout(p=0.0, inplace=False)
-          (conv2): Conv2d(1280, 1280, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1))
-          (nonlinearity): SiLU()
-          (conv_shortcut): Conv2d(2560, 1280, kernel_size=(1, 1), stride=(1, 1))
-        )
-      )
-      (upsamplers): ModuleList(
-        (0): Upsample2D(
-          (conv): Conv2d(1280, 1280, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1))
-        )
-      )
-    )
-    (1): CrossAttnUpBlock2D(
-      (attentions): ModuleList(
-        (0): Transformer2DModel(
-          (norm): GroupNorm(32, 1280, eps=1e-06, affine=True)
-          (proj_in): Conv2d(1280, 1280, kernel_size=(1, 1), stride=(1, 1))
-          (transformer_blocks): ModuleList(
-            (0): BasicTransformerBlock(
-              (attn1): CrossAttention(
-                (to_q): Linear(in_features=1280, out_features=1280, bias=False)
-                (to_k): Linear(in_features=1280, out_features=1280, bias=False)
-                (to_v): Linear(in_features=1280, out_features=1280, bias=False)
-                (to_out): ModuleList(
-                  (0): Linear(in_features=1280, out_features=1280, bias=True)
-                  (1): Dropout(p=0.0, inplace=False)
-                )
-              )
-              (ff): FeedForward(
-                (net): ModuleList(
-                  (0): GEGLU(
-                    (proj): Linear(in_features=1280, out_features=10240, bias=True)
-                  )
-                  (1): Dropout(p=0.0, inplace=False)
-                  (2): Linear(in_features=5120, out_features=1280, bias=True)
-                )
-              )
-              (attn2): CrossAttention(
-                (to_q): Linear(in_features=1280, out_features=1280, bias=False)
-                (to_k): Linear(in_features=768, out_features=1280, bias=False)
-                (to_v): Linear(in_features=768, out_features=1280, bias=False)
-                (to_out): ModuleList(
-                  (0): Linear(in_features=1280, out_features=1280, bias=True)
-                  (1): Dropout(p=0.0, inplace=False)
-                )
-              )
-              (norm1): LayerNorm((1280,), eps=1e-05, elementwise_affine=True)
-              (norm2): LayerNorm((1280,), eps=1e-05, elementwise_affine=True)
-              (norm3): LayerNorm((1280,), eps=1e-05, elementwise_affine=True)
-            )
-          )
-          (proj_out): Conv2d(1280, 1280, kernel_size=(1, 1), stride=(1, 1))
-        )
-        (1): Transformer2DModel(
-          (norm): GroupNorm(32, 1280, eps=1e-06, affine=True)
-          (proj_in): Conv2d(1280, 1280, kernel_size=(1, 1), stride=(1, 1))
-          (transformer_blocks): ModuleList(
-            (0): BasicTransformerBlock(
-              (attn1): CrossAttention(
-                (to_q): Linear(in_features=1280, out_features=1280, bias=False)
-                (to_k): Linear(in_features=1280, out_features=1280, bias=False)
-                (to_v): Linear(in_features=1280, out_features=1280, bias=False)
-                (to_out): ModuleList(
-                  (0): Linear(in_features=1280, out_features=1280, bias=True)
-                  (1): Dropout(p=0.0, inplace=False)
-                )
-              )
-              (ff): FeedForward(
-                (net): ModuleList(
-                  (0): GEGLU(
-                    (proj): Linear(in_features=1280, out_features=10240, bias=True)
-                  )
-                  (1): Dropout(p=0.0, inplace=False)
-                  (2): Linear(in_features=5120, out_features=1280, bias=True)
-                )
-              )
-              (attn2): CrossAttention(
-                (to_q): Linear(in_features=1280, out_features=1280, bias=False)
-                (to_k): Linear(in_features=768, out_features=1280, bias=False)
-                (to_v): Linear(in_features=768, out_features=1280, bias=False)
-                (to_out): ModuleList(
-                  (0): Linear(in_features=1280, out_features=1280, bias=True)
-                  (1): Dropout(p=0.0, inplace=False)
-                )
-              )
-              (norm1): LayerNorm((1280,), eps=1e-05, elementwise_affine=True)
-              (norm2): LayerNorm((1280,), eps=1e-05, elementwise_affine=True)
-              (norm3): LayerNorm((1280,), eps=1e-05, elementwise_affine=True)
-            )
-          )
-          (proj_out): Conv2d(1280, 1280, kernel_size=(1, 1), stride=(1, 1))
-        )
-        (2): Transformer2DModel(
-          (norm): GroupNorm(32, 1280, eps=1e-06, affine=True)
-          (proj_in): Conv2d(1280, 1280, kernel_size=(1, 1), stride=(1, 1))
-          (transformer_blocks): ModuleList(
-            (0): BasicTransformerBlock(
-              (attn1): CrossAttention(
-                (to_q): Linear(in_features=1280, out_features=1280, bias=False)
-                (to_k): Linear(in_features=1280, out_features=1280, bias=False)
-                (to_v): Linear(in_features=1280, out_features=1280, bias=False)
-                (to_out): ModuleList(
-                  (0): Linear(in_features=1280, out_features=1280, bias=True)
-                  (1): Dropout(p=0.0, inplace=False)
-                )
-              )
-              (ff): FeedForward(
-                (net): ModuleList(
-                  (0): GEGLU(
-                    (proj): Linear(in_features=1280, out_features=10240, bias=True)
-                  )
-                  (1): Dropout(p=0.0, inplace=False)
-                  (2): Linear(in_features=5120, out_features=1280, bias=True)
-                )
-              )
-              (attn2): CrossAttention(
-                (to_q): Linear(in_features=1280, out_features=1280, bias=False)
-                (to_k): Linear(in_features=768, out_features=1280, bias=False)
-                (to_v): Linear(in_features=768, out_features=1280, bias=False)
-                (to_out): ModuleList(
-                  (0): Linear(in_features=1280, out_features=1280, bias=True)
-                  (1): Dropout(p=0.0, inplace=False)
-                )
-              )
-              (norm1): LayerNorm((1280,), eps=1e-05, elementwise_affine=True)
-              (norm2): LayerNorm((1280,), eps=1e-05, elementwise_affine=True)
-              (norm3): LayerNorm((1280,), eps=1e-05, elementwise_affine=True)
-            )
-          )
-          (proj_out): Conv2d(1280, 1280, kernel_size=(1, 1), stride=(1, 1))
-        )
-      )
-      (resnets): ModuleList(
-        (0): ResnetBlock2D(
-          (norm1): GroupNorm(32, 2560, eps=1e-05, affine=True)
-          (conv1): Conv2d(2560, 1280, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1))
-          (time_emb_proj): Linear(in_features=1280, out_features=1280, bias=True)
-          (norm2): GroupNorm(32, 1280, eps=1e-05, affine=True)
-          (dropout): Dropout(p=0.0, inplace=False)
-          (conv2): Conv2d(1280, 1280, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1))
-          (nonlinearity): SiLU()
-          (conv_shortcut): Conv2d(2560, 1280, kernel_size=(1, 1), stride=(1, 1))
-        )
-        (1): ResnetBlock2D(
-          (norm1): GroupNorm(32, 2560, eps=1e-05, affine=True)
-          (conv1): Conv2d(2560, 1280, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1))
-          (time_emb_proj): Linear(in_features=1280, out_features=1280, bias=True)
-          (norm2): GroupNorm(32, 1280, eps=1e-05, affine=True)
-          (dropout): Dropout(p=0.0, inplace=False)
-          (conv2): Conv2d(1280, 1280, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1))
-          (nonlinearity): SiLU()
-          (conv_shortcut): Conv2d(2560, 1280, kernel_size=(1, 1), stride=(1, 1))
-        )
-        (2): ResnetBlock2D(
-          (norm1): GroupNorm(32, 1920, eps=1e-05, affine=True)
-          (conv1): Conv2d(1920, 1280, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1))
-          (time_emb_proj): Linear(in_features=1280, out_features=1280, bias=True)
-          (norm2): GroupNorm(32, 1280, eps=1e-05, affine=True)
-          (dropout): Dropout(p=0.0, inplace=False)
-          (conv2): Conv2d(1280, 1280, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1))
-          (nonlinearity): SiLU()
-          (conv_shortcut): Conv2d(1920, 1280, kernel_size=(1, 1), stride=(1, 1))
-        )
-      )
-      (upsamplers): ModuleList(
-        (0): Upsample2D(
-          (conv): Conv2d(1280, 1280, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1))
-        )
-      )
-    )
-    (2): CrossAttnUpBlock2D(
-      (attentions): ModuleList(
-        (0): Transformer2DModel(
-          (norm): GroupNorm(32, 640, eps=1e-06, affine=True)
-          (proj_in): Conv2d(640, 640, kernel_size=(1, 1), stride=(1, 1))
-          (transformer_blocks): ModuleList(
-            (0): BasicTransformerBlock(
-              (attn1): CrossAttention(
-                (to_q): Linear(in_features=640, out_features=640, bias=False)
-                (to_k): Linear(in_features=640, out_features=640, bias=False)
-                (to_v): Linear(in_features=640, out_features=640, bias=False)
-                (to_out): ModuleList(
-                  (0): Linear(in_features=640, out_features=640, bias=True)
-                  (1): Dropout(p=0.0, inplace=False)
-                )
-              )
-              (ff): FeedForward(
-                (net): ModuleList(
-                  (0): GEGLU(
-                    (proj): Linear(in_features=640, out_features=5120, bias=True)
-                  )
-                  (1): Dropout(p=0.0, inplace=False)
-                  (2): Linear(in_features=2560, out_features=640, bias=True)
-                )
-              )
-              (attn2): CrossAttention(
-                (to_q): Linear(in_features=640, out_features=640, bias=False)
-                (to_k): Linear(in_features=768, out_features=640, bias=False)
-                (to_v): Linear(in_features=768, out_features=640, bias=False)
-                (to_out): ModuleList(
-                  (0): Linear(in_features=640, out_features=640, bias=True)
-                  (1): Dropout(p=0.0, inplace=False)
-                )
-              )
-              (norm1): LayerNorm((640,), eps=1e-05, elementwise_affine=True)
-              (norm2): LayerNorm((640,), eps=1e-05, elementwise_affine=True)
-              (norm3): LayerNorm((640,), eps=1e-05, elementwise_affine=True)
-            )
-          )
-          (proj_out): Conv2d(640, 640, kernel_size=(1, 1), stride=(1, 1))
-        )
-        (1): Transformer2DModel(
-          (norm): GroupNorm(32, 640, eps=1e-06, affine=True)
-          (proj_in): Conv2d(640, 640, kernel_size=(1, 1), stride=(1, 1))
-          (transformer_blocks): ModuleList(
-            (0): BasicTransformerBlock(
-              (attn1): CrossAttention(
-                (to_q): Linear(in_features=640, out_features=640, bias=False)
-                (to_k): Linear(in_features=640, out_features=640, bias=False)
-                (to_v): Linear(in_features=640, out_features=640, bias=False)
-                (to_out): ModuleList(
-                  (0): Linear(in_features=640, out_features=640, bias=True)
-                  (1): Dropout(p=0.0, inplace=False)
-                )
-              )
-              (ff): FeedForward(
-                (net): ModuleList(
-                  (0): GEGLU(
-                    (proj): Linear(in_features=640, out_features=5120, bias=True)
-                  )
-                  (1): Dropout(p=0.0, inplace=False)
-                  (2): Linear(in_features=2560, out_features=640, bias=True)
-                )
-              )
-              (attn2): CrossAttention(
-                (to_q): Linear(in_features=640, out_features=640, bias=False)
-                (to_k): Linear(in_features=768, out_features=640, bias=False)
-                (to_v): Linear(in_features=768, out_features=640, bias=False)
-                (to_out): ModuleList(
-                  (0): Linear(in_features=640, out_features=640, bias=True)
-                  (1): Dropout(p=0.0, inplace=False)
-                )
-              )
-              (norm1): LayerNorm((640,), eps=1e-05, elementwise_affine=True)
-              (norm2): LayerNorm((640,), eps=1e-05, elementwise_affine=True)
-              (norm3): LayerNorm((640,), eps=1e-05, elementwise_affine=True)
-            )
-          )
-          (proj_out): Conv2d(640, 640, kernel_size=(1, 1), stride=(1, 1))
-        )
-        (2): Transformer2DModel(
-          (norm): GroupNorm(32, 640, eps=1e-06, affine=True)
-          (proj_in): Conv2d(640, 640, kernel_size=(1, 1), stride=(1, 1))
-          (transformer_blocks): ModuleList(
-            (0): BasicTransformerBlock(
-              (attn1): CrossAttention(
-                (to_q): Linear(in_features=640, out_features=640, bias=False)
-                (to_k): Linear(in_features=640, out_features=640, bias=False)
-                (to_v): Linear(in_features=640, out_features=640, bias=False)
-                (to_out): ModuleList(
-                  (0): Linear(in_features=640, out_features=640, bias=True)
-                  (1): Dropout(p=0.0, inplace=False)
-                )
-              )
-              (ff): FeedForward(
-                (net): ModuleList(
-                  (0): GEGLU(
-                    (proj): Linear(in_features=640, out_features=5120, bias=True)
-                  )
-                  (1): Dropout(p=0.0, inplace=False)
-                  (2): Linear(in_features=2560, out_features=640, bias=True)
-                )
-              )
-              (attn2): CrossAttention(
-                (to_q): Linear(in_features=640, out_features=640, bias=False)
-                (to_k): Linear(in_features=768, out_features=640, bias=False)
-                (to_v): Linear(in_features=768, out_features=640, bias=False)
-                (to_out): ModuleList(
-                  (0): Linear(in_features=640, out_features=640, bias=True)
-                  (1): Dropout(p=0.0, inplace=False)
-                )
-              )
-              (norm1): LayerNorm((640,), eps=1e-05, elementwise_affine=True)
-              (norm2): LayerNorm((640,), eps=1e-05, elementwise_affine=True)
-              (norm3): LayerNorm((640,), eps=1e-05, elementwise_affine=True)
-            )
-          )
-          (proj_out): Conv2d(640, 640, kernel_size=(1, 1), stride=(1, 1))
-        )
-      )
-      (resnets): ModuleList(
-        (0): ResnetBlock2D(
-          (norm1): GroupNorm(32, 1920, eps=1e-05, affine=True)
-          (conv1): Conv2d(1920, 640, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1))
-          (time_emb_proj): Linear(in_features=1280, out_features=640, bias=True)
-          (norm2): GroupNorm(32, 640, eps=1e-05, affine=True)
-          (dropout): Dropout(p=0.0, inplace=False)
-          (conv2): Conv2d(640, 640, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1))
-          (nonlinearity): SiLU()
-          (conv_shortcut): Conv2d(1920, 640, kernel_size=(1, 1), stride=(1, 1))
-        )
-        (1): ResnetBlock2D(
-          (norm1): GroupNorm(32, 1280, eps=1e-05, affine=True)
-          (conv1): Conv2d(1280, 640, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1))
-          (time_emb_proj): Linear(in_features=1280, out_features=640, bias=True)
-          (norm2): GroupNorm(32, 640, eps=1e-05, affine=True)
-          (dropout): Dropout(p=0.0, inplace=False)
-          (conv2): Conv2d(640, 640, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1))
-          (nonlinearity): SiLU()
-          (conv_shortcut): Conv2d(1280, 640, kernel_size=(1, 1), stride=(1, 1))
-        )
-        (2): ResnetBlock2D(
-          (norm1): GroupNorm(32, 960, eps=1e-05, affine=True)
-          (conv1): Conv2d(960, 640, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1))
-          (time_emb_proj): Linear(in_features=1280, out_features=640, bias=True)
-          (norm2): GroupNorm(32, 640, eps=1e-05, affine=True)
-          (dropout): Dropout(p=0.0, inplace=False)
-          (conv2): Conv2d(640, 640, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1))
-          (nonlinearity): SiLU()
-          (conv_shortcut): Conv2d(960, 640, kernel_size=(1, 1), stride=(1, 1))
-        )
-      )
-      (upsamplers): ModuleList(
-        (0): Upsample2D(
-          (conv): Conv2d(640, 640, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1))
-        )
-      )
-    )
-    (3): CrossAttnUpBlock2D(
-      (attentions): ModuleList(
-        (0): Transformer2DModel(
-          (norm): GroupNorm(32, 320, eps=1e-06, affine=True)
-          (proj_in): Conv2d(320, 320, kernel_size=(1, 1), stride=(1, 1))
-          (transformer_blocks): ModuleList(
-            (0): BasicTransformerBlock(
-              (attn1): CrossAttention(
-                (to_q): Linear(in_features=320, out_features=320, bias=False)
-                (to_k): Linear(in_features=320, out_features=320, bias=False)
-                (to_v): Linear(in_features=320, out_features=320, bias=False)
-                (to_out): ModuleList(
-                  (0): Linear(in_features=320, out_features=320, bias=True)
-                  (1): Dropout(p=0.0, inplace=False)
-                )
-              )
-              (ff): FeedForward(
-                (net): ModuleList(
-                  (0): GEGLU(
-                    (proj): Linear(in_features=320, out_features=2560, bias=True)
-                  )
-                  (1): Dropout(p=0.0, inplace=False)
-                  (2): Linear(in_features=1280, out_features=320, bias=True)
-                )
-              )
-              (attn2): CrossAttention(
-                (to_q): Linear(in_features=320, out_features=320, bias=False)
-                (to_k): Linear(in_features=768, out_features=320, bias=False)
-                (to_v): Linear(in_features=768, out_features=320, bias=False)
-                (to_out): ModuleList(
-                  (0): Linear(in_features=320, out_features=320, bias=True)
-                  (1): Dropout(p=0.0, inplace=False)
-                )
-              )
-              (norm1): LayerNorm((320,), eps=1e-05, elementwise_affine=True)
-              (norm2): LayerNorm((320,), eps=1e-05, elementwise_affine=True)
-              (norm3): LayerNorm((320,), eps=1e-05, elementwise_affine=True)
-            )
-          )
-          (proj_out): Conv2d(320, 320, kernel_size=(1, 1), stride=(1, 1))
-        )
-        (1): Transformer2DModel(
-          (norm): GroupNorm(32, 320, eps=1e-06, affine=True)
-          (proj_in): Conv2d(320, 320, kernel_size=(1, 1), stride=(1, 1))
-          (transformer_blocks): ModuleList(
-            (0): BasicTransformerBlock(
-              (attn1): CrossAttention(
-                (to_q): Linear(in_features=320, out_features=320, bias=False)
-                (to_k): Linear(in_features=320, out_features=320, bias=False)
-                (to_v): Linear(in_features=320, out_features=320, bias=False)
-                (to_out): ModuleList(
-                  (0): Linear(in_features=320, out_features=320, bias=True)
-                  (1): Dropout(p=0.0, inplace=False)
-                )
-              )
-              (ff): FeedForward(
-                (net): ModuleList(
-                  (0): GEGLU(
-                    (proj): Linear(in_features=320, out_features=2560, bias=True)
-                  )
-                  (1): Dropout(p=0.0, inplace=False)
-                  (2): Linear(in_features=1280, out_features=320, bias=True)
-                )
-              )
-              (attn2): CrossAttention(
-                (to_q): Linear(in_features=320, out_features=320, bias=False)
-                (to_k): Linear(in_features=768, out_features=320, bias=False)
-                (to_v): Linear(in_features=768, out_features=320, bias=False)
-                (to_out): ModuleList(
-                  (0): Linear(in_features=320, out_features=320, bias=True)
-                  (1): Dropout(p=0.0, inplace=False)
-                )
-              )
-              (norm1): LayerNorm((320,), eps=1e-05, elementwise_affine=True)
-              (norm2): LayerNorm((320,), eps=1e-05, elementwise_affine=True)
-              (norm3): LayerNorm((320,), eps=1e-05, elementwise_affine=True)
-            )
-          )
-          (proj_out): Conv2d(320, 320, kernel_size=(1, 1), stride=(1, 1))
-        )
-        (2): Transformer2DModel(
-          (norm): GroupNorm(32, 320, eps=1e-06, affine=True)
-          (proj_in): Conv2d(320, 320, kernel_size=(1, 1), stride=(1, 1))
-          (transformer_blocks): ModuleList(
-            (0): BasicTransformerBlock(
-              (attn1): CrossAttention(
-                (to_q): Linear(in_features=320, out_features=320, bias=False)
-                (to_k): Linear(in_features=320, out_features=320, bias=False)
-                (to_v): Linear(in_features=320, out_features=320, bias=False)
-                (to_out): ModuleList(
-                  (0): Linear(in_features=320, out_features=320, bias=True)
-                  (1): Dropout(p=0.0, inplace=False)
-                )
-              )
-              (ff): FeedForward(
-                (net): ModuleList(
-                  (0): GEGLU(
-                    (proj): Linear(in_features=320, out_features=2560, bias=True)
-                  )
-                  (1): Dropout(p=0.0, inplace=False)
-                  (2): Linear(in_features=1280, out_features=320, bias=True)
-                )
-              )
-              (attn2): CrossAttention(
-                (to_q): Linear(in_features=320, out_features=320, bias=False)
-                (to_k): Linear(in_features=768, out_features=320, bias=False)
-                (to_v): Linear(in_features=768, out_features=320, bias=False)
-                (to_out): ModuleList(
-                  (0): Linear(in_features=320, out_features=320, bias=True)
-                  (1): Dropout(p=0.0, inplace=False)
-                )
-              )
-              (norm1): LayerNorm((320,), eps=1e-05, elementwise_affine=True)
-              (norm2): LayerNorm((320,), eps=1e-05, elementwise_affine=True)
-              (norm3): LayerNorm((320,), eps=1e-05, elementwise_affine=True)
-            )
-          )
-          (proj_out): Conv2d(320, 320, kernel_size=(1, 1), stride=(1, 1))
-        )
-      )
-      (resnets): ModuleList(
-        (0): ResnetBlock2D(
-          (norm1): GroupNorm(32, 960, eps=1e-05, affine=True)
-          (conv1): Conv2d(960, 320, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1))
-          (time_emb_proj): Linear(in_features=1280, out_features=320, bias=True)
-          (norm2): GroupNorm(32, 320, eps=1e-05, affine=True)
-          (dropout): Dropout(p=0.0, inplace=False)
-          (conv2): Conv2d(320, 320, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1))
-          (nonlinearity): SiLU()
-          (conv_shortcut): Conv2d(960, 320, kernel_size=(1, 1), stride=(1, 1))
-        )
-        (1): ResnetBlock2D(
-          (norm1): GroupNorm(32, 640, eps=1e-05, affine=True)
-          (conv1): Conv2d(640, 320, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1))
-          (time_emb_proj): Linear(in_features=1280, out_features=320, bias=True)
-          (norm2): GroupNorm(32, 320, eps=1e-05, affine=True)
-          (dropout): Dropout(p=0.0, inplace=False)
-          (conv2): Conv2d(320, 320, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1))
-          (nonlinearity): SiLU()
-          (conv_shortcut): Conv2d(640, 320, kernel_size=(1, 1), stride=(1, 1))
-        )
-        (2): ResnetBlock2D(
-          (norm1): GroupNorm(32, 640, eps=1e-05, affine=True)
-          (conv1): Conv2d(640, 320, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1))
-          (time_emb_proj): Linear(in_features=1280, out_features=320, bias=True)
-          (norm2): GroupNorm(32, 320, eps=1e-05, affine=True)
-          (dropout): Dropout(p=0.0, inplace=False)
-          (conv2): Conv2d(320, 320, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1))
-          (nonlinearity): SiLU()
-          (conv_shortcut): Conv2d(640, 320, kernel_size=(1, 1), stride=(1, 1))
-        )
-      )
-    )
-  )
-  (mid_block): UNetMidBlock2DCrossAttn(
-    (attentions): ModuleList(
-      (0): Transformer2DModel(
-        (norm): GroupNorm(32, 1280, eps=1e-06, affine=True)
-        (proj_in): Conv2d(1280, 1280, kernel_size=(1, 1), stride=(1, 1))
-        (transformer_blocks): ModuleList(
-          (0): BasicTransformerBlock(
-            (attn1): CrossAttention(
-              (to_q): Linear(in_features=1280, out_features=1280, bias=False)
-              (to_k): Linear(in_features=1280, out_features=1280, bias=False)
-              (to_v): Linear(in_features=1280, out_features=1280, bias=False)
-              (to_out): ModuleList(
-                (0): Linear(in_features=1280, out_features=1280, bias=True)
-                (1): Dropout(p=0.0, inplace=False)
-              )
-            )
-            (ff): FeedForward(
-              (net): ModuleList(
-                (0): GEGLU(
-                  (proj): Linear(in_features=1280, out_features=10240, bias=True)
-                )
-                (1): Dropout(p=0.0, inplace=False)
-                (2): Linear(in_features=5120, out_features=1280, bias=True)
-              )
-            )
-            (attn2): CrossAttention(
-              (to_q): Linear(in_features=1280, out_features=1280, bias=False)
-              (to_k): Linear(in_features=768, out_features=1280, bias=False)
-              (to_v): Linear(in_features=768, out_features=1280, bias=False)
-              (to_out): ModuleList(
-                (0): Linear(in_features=1280, out_features=1280, bias=True)
-                (1): Dropout(p=0.0, inplace=False)
-              )
-            )
-            (norm1): LayerNorm((1280,), eps=1e-05, elementwise_affine=True)
-            (norm2): LayerNorm((1280,), eps=1e-05, elementwise_affine=True)
-            (norm3): LayerNorm((1280,), eps=1e-05, elementwise_affine=True)
-          )
-        )
-        (proj_out): Conv2d(1280, 1280, kernel_size=(1, 1), stride=(1, 1))
-      )
-    )
-    (resnets): ModuleList(
-      (0): ResnetBlock2D(
-        (norm1): GroupNorm(32, 1280, eps=1e-05, affine=True)
-        (conv1): Conv2d(1280, 1280, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1))
-        (time_emb_proj): Linear(in_features=1280, out_features=1280, bias=True)
-        (norm2): GroupNorm(32, 1280, eps=1e-05, affine=True)
-        (dropout): Dropout(p=0.0, inplace=False)
-        (conv2): Conv2d(1280, 1280, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1))
-        (nonlinearity): SiLU()
-      )
-      (1): ResnetBlock2D(
-        (norm1): GroupNorm(32, 1280, eps=1e-05, affine=True)
-        (conv1): Conv2d(1280, 1280, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1))
-        (time_emb_proj): Linear(in_features=1280, out_features=1280, bias=True)
-        (norm2): GroupNorm(32, 1280, eps=1e-05, affine=True)
-        (dropout): Dropout(p=0.0, inplace=False)
-        (conv2): Conv2d(1280, 1280, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1))
-        (nonlinearity): SiLU()
-      )
-    )
-  )
-  (conv_norm_out): GroupNorm(32, 320, eps=1e-05, affine=True)
-  (conv_act): SiLU()
-  (conv_out): Conv2d(320, 4, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1))
+UNet2DConditionModel(
+  (conv_in): Conv2d(4, 320, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1))
+  (time_proj): Timesteps()
+  (time_embedding): TimestepEmbedding(
+    (linear_1): Linear(in_features=320, out_features=1280, bias=True)
+    (act): SiLU()
+    (linear_2): Linear(in_features=1280, out_features=1280, bias=True)
+  )
+  (down_blocks): ModuleList(
+    (0): CrossAttnDownBlock2D(
+      (attentions): ModuleList(
+        (0): Transformer2DModel(
+          (norm): GroupNorm(32, 320, eps=1e-06, affine=True)
+          (proj_in): Conv2d(320, 320, kernel_size=(1, 1), stride=(1, 1))
+          (transformer_blocks): ModuleList(
+            (0): BasicTransformerBlock(
+              (attn1): CrossAttention(
+                (to_q): Linear(in_features=320, out_features=320, bias=False)
+                (to_k): Linear(in_features=320, out_features=320, bias=False)
+                (to_v): Linear(in_features=320, out_features=320, bias=False)
+                (to_out): ModuleList(
+                  (0): Linear(in_features=320, out_features=320, bias=True)
+                  (1): Dropout(p=0.0, inplace=False)
+                )
+              )
+              (ff): FeedForward(
+                (net): ModuleList(
+                  (0): GEGLU(
+                    (proj): Linear(in_features=320, out_features=2560, bias=True)
+                  )
+                  (1): Dropout(p=0.0, inplace=False)
+                  (2): Linear(in_features=1280, out_features=320, bias=True)
+                )
+              )
+              (attn2): CrossAttention(
+                (to_q): Linear(in_features=320, out_features=320, bias=False)
+                (to_k): Linear(in_features=768, out_features=320, bias=False)
+                (to_v): Linear(in_features=768, out_features=320, bias=False)
+                (to_out): ModuleList(
+                  (0): Linear(in_features=320, out_features=320, bias=True)
+                  (1): Dropout(p=0.0, inplace=False)
+                )
+              )
+              (norm1): LayerNorm((320,), eps=1e-05, elementwise_affine=True)
+              (norm2): LayerNorm((320,), eps=1e-05, elementwise_affine=True)
+              (norm3): LayerNorm((320,), eps=1e-05, elementwise_affine=True)
+            )
+          )
+          (proj_out): Conv2d(320, 320, kernel_size=(1, 1), stride=(1, 1))
+        )
+        (1): Transformer2DModel(
+          (norm): GroupNorm(32, 320, eps=1e-06, affine=True)
+          (proj_in): Conv2d(320, 320, kernel_size=(1, 1), stride=(1, 1))
+          (transformer_blocks): ModuleList(
+            (0): BasicTransformerBlock(
+              (attn1): CrossAttention(
+                (to_q): Linear(in_features=320, out_features=320, bias=False)
+                (to_k): Linear(in_features=320, out_features=320, bias=False)
+                (to_v): Linear(in_features=320, out_features=320, bias=False)
+                (to_out): ModuleList(
+                  (0): Linear(in_features=320, out_features=320, bias=True)
+                  (1): Dropout(p=0.0, inplace=False)
+                )
+              )
+              (ff): FeedForward(
+                (net): ModuleList(
+                  (0): GEGLU(
+                    (proj): Linear(in_features=320, out_features=2560, bias=True)
+                  )
+                  (1): Dropout(p=0.0, inplace=False)
+                  (2): Linear(in_features=1280, out_features=320, bias=True)
+                )
+              )
+              (attn2): CrossAttention(
+                (to_q): Linear(in_features=320, out_features=320, bias=False)
+                (to_k): Linear(in_features=768, out_features=320, bias=False)
+                (to_v): Linear(in_features=768, out_features=320, bias=False)
+                (to_out): ModuleList(
+                  (0): Linear(in_features=320, out_features=320, bias=True)
+                  (1): Dropout(p=0.0, inplace=False)
+                )
+              )
+              (norm1): LayerNorm((320,), eps=1e-05, elementwise_affine=True)
+              (norm2): LayerNorm((320,), eps=1e-05, elementwise_affine=True)
+              (norm3): LayerNorm((320,), eps=1e-05, elementwise_affine=True)
+            )
+          )
+          (proj_out): Conv2d(320, 320, kernel_size=(1, 1), stride=(1, 1))
+        )
+      )
+      (resnets): ModuleList(
+        (0): ResnetBlock2D(
+          (norm1): GroupNorm(32, 320, eps=1e-05, affine=True)
+          (conv1): Conv2d(320, 320, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1))
+          (time_emb_proj): Linear(in_features=1280, out_features=320, bias=True)
+          (norm2): GroupNorm(32, 320, eps=1e-05, affine=True)
+          (dropout): Dropout(p=0.0, inplace=False)
+          (conv2): Conv2d(320, 320, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1))
+          (nonlinearity): SiLU()
+        )
+        (1): ResnetBlock2D(
+          (norm1): GroupNorm(32, 320, eps=1e-05, affine=True)
+          (conv1): Conv2d(320, 320, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1))
+          (time_emb_proj): Linear(in_features=1280, out_features=320, bias=True)
+          (norm2): GroupNorm(32, 320, eps=1e-05, affine=True)
+          (dropout): Dropout(p=0.0, inplace=False)
+          (conv2): Conv2d(320, 320, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1))
+          (nonlinearity): SiLU()
+        )
+      )
+      (downsamplers): ModuleList(
+        (0): Downsample2D(
+          (conv): Conv2d(320, 320, kernel_size=(3, 3), stride=(2, 2), padding=(1, 1))
+        )
+      )
+    )
+    (1): CrossAttnDownBlock2D(
+      (attentions): ModuleList(
+        (0): Transformer2DModel(
+          (norm): GroupNorm(32, 640, eps=1e-06, affine=True)
+          (proj_in): Conv2d(640, 640, kernel_size=(1, 1), stride=(1, 1))
+          (transformer_blocks): ModuleList(
+            (0): BasicTransformerBlock(
+              (attn1): CrossAttention(
+                (to_q): Linear(in_features=640, out_features=640, bias=False)
+                (to_k): Linear(in_features=640, out_features=640, bias=False)
+                (to_v): Linear(in_features=640, out_features=640, bias=False)
+                (to_out): ModuleList(
+                  (0): Linear(in_features=640, out_features=640, bias=True)
+                  (1): Dropout(p=0.0, inplace=False)
+                )
+              )
+              (ff): FeedForward(
+                (net): ModuleList(
+                  (0): GEGLU(
+                    (proj): Linear(in_features=640, out_features=5120, bias=True)
+                  )
+                  (1): Dropout(p=0.0, inplace=False)
+                  (2): Linear(in_features=2560, out_features=640, bias=True)
+                )
+              )
+              (attn2): CrossAttention(
+                (to_q): Linear(in_features=640, out_features=640, bias=False)
+                (to_k): Linear(in_features=768, out_features=640, bias=False)
+                (to_v): Linear(in_features=768, out_features=640, bias=False)
+                (to_out): ModuleList(
+                  (0): Linear(in_features=640, out_features=640, bias=True)
+                  (1): Dropout(p=0.0, inplace=False)
+                )
+              )
+              (norm1): LayerNorm((640,), eps=1e-05, elementwise_affine=True)
+              (norm2): LayerNorm((640,), eps=1e-05, elementwise_affine=True)
+              (norm3): LayerNorm((640,), eps=1e-05, elementwise_affine=True)
+            )
+          )
+          (proj_out): Conv2d(640, 640, kernel_size=(1, 1), stride=(1, 1))
+        )
+        (1): Transformer2DModel(
+          (norm): GroupNorm(32, 640, eps=1e-06, affine=True)
+          (proj_in): Conv2d(640, 640, kernel_size=(1, 1), stride=(1, 1))
+          (transformer_blocks): ModuleList(
+            (0): BasicTransformerBlock(
+              (attn1): CrossAttention(
+                (to_q): Linear(in_features=640, out_features=640, bias=False)
+                (to_k): Linear(in_features=640, out_features=640, bias=False)
+                (to_v): Linear(in_features=640, out_features=640, bias=False)
+                (to_out): ModuleList(
+                  (0): Linear(in_features=640, out_features=640, bias=True)
+                  (1): Dropout(p=0.0, inplace=False)
+                )
+              )
+              (ff): FeedForward(
+                (net): ModuleList(
+                  (0): GEGLU(
+                    (proj): Linear(in_features=640, out_features=5120, bias=True)
+                  )
+                  (1): Dropout(p=0.0, inplace=False)
+                  (2): Linear(in_features=2560, out_features=640, bias=True)
+                )
+              )
+              (attn2): CrossAttention(
+                (to_q): Linear(in_features=640, out_features=640, bias=False)
+                (to_k): Linear(in_features=768, out_features=640, bias=False)
+                (to_v): Linear(in_features=768, out_features=640, bias=False)
+                (to_out): ModuleList(
+                  (0): Linear(in_features=640, out_features=640, bias=True)
+                  (1): Dropout(p=0.0, inplace=False)
+                )
+              )
+              (norm1): LayerNorm((640,), eps=1e-05, elementwise_affine=True)
+              (norm2): LayerNorm((640,), eps=1e-05, elementwise_affine=True)
+              (norm3): LayerNorm((640,), eps=1e-05, elementwise_affine=True)
+            )
+          )
+          (proj_out): Conv2d(640, 640, kernel_size=(1, 1), stride=(1, 1))
+        )
+      )
+      (resnets): ModuleList(
+        (0): ResnetBlock2D(
+          (norm1): GroupNorm(32, 320, eps=1e-05, affine=True)
+          (conv1): Conv2d(320, 640, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1))
+          (time_emb_proj): Linear(in_features=1280, out_features=640, bias=True)
+          (norm2): GroupNorm(32, 640, eps=1e-05, affine=True)
+          (dropout): Dropout(p=0.0, inplace=False)
+          (conv2): Conv2d(640, 640, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1))
+          (nonlinearity): SiLU()
+          (conv_shortcut): Conv2d(320, 640, kernel_size=(1, 1), stride=(1, 1))
+        )
+        (1): ResnetBlock2D(
+          (norm1): GroupNorm(32, 640, eps=1e-05, affine=True)
+          (conv1): Conv2d(640, 640, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1))
+          (time_emb_proj): Linear(in_features=1280, out_features=640, bias=True)
+          (norm2): GroupNorm(32, 640, eps=1e-05, affine=True)
+          (dropout): Dropout(p=0.0, inplace=False)
+          (conv2): Conv2d(640, 640, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1))
+          (nonlinearity): SiLU()
+        )
+      )
+      (downsamplers): ModuleList(
+        (0): Downsample2D(
+          (conv): Conv2d(640, 640, kernel_size=(3, 3), stride=(2, 2), padding=(1, 1))
+        )
+      )
+    )
+    (2): CrossAttnDownBlock2D(
+      (attentions): ModuleList(
+        (0): Transformer2DModel(
+          (norm): GroupNorm(32, 1280, eps=1e-06, affine=True)
+          (proj_in): Conv2d(1280, 1280, kernel_size=(1, 1), stride=(1, 1))
+          (transformer_blocks): ModuleList(
+            (0): BasicTransformerBlock(
+              (attn1): CrossAttention(
+                (to_q): Linear(in_features=1280, out_features=1280, bias=False)
+                (to_k): Linear(in_features=1280, out_features=1280, bias=False)
+                (to_v): Linear(in_features=1280, out_features=1280, bias=False)
+                (to_out): ModuleList(
+                  (0): Linear(in_features=1280, out_features=1280, bias=True)
+                  (1): Dropout(p=0.0, inplace=False)
+                )
+              )
+              (ff): FeedForward(
+                (net): ModuleList(
+                  (0): GEGLU(
+                    (proj): Linear(in_features=1280, out_features=10240, bias=True)
+                  )
+                  (1): Dropout(p=0.0, inplace=False)
+                  (2): Linear(in_features=5120, out_features=1280, bias=True)
+                )
+              )
+              (attn2): CrossAttention(
+                (to_q): Linear(in_features=1280, out_features=1280, bias=False)
+                (to_k): Linear(in_features=768, out_features=1280, bias=False)
+                (to_v): Linear(in_features=768, out_features=1280, bias=False)
+                (to_out): ModuleList(
+                  (0): Linear(in_features=1280, out_features=1280, bias=True)
+                  (1): Dropout(p=0.0, inplace=False)
+                )
+              )
+              (norm1): LayerNorm((1280,), eps=1e-05, elementwise_affine=True)
+              (norm2): LayerNorm((1280,), eps=1e-05, elementwise_affine=True)
+              (norm3): LayerNorm((1280,), eps=1e-05, elementwise_affine=True)
+            )
+          )
+          (proj_out): Conv2d(1280, 1280, kernel_size=(1, 1), stride=(1, 1))
+        )
+        (1): Transformer2DModel(
+          (norm): GroupNorm(32, 1280, eps=1e-06, affine=True)
+          (proj_in): Conv2d(1280, 1280, kernel_size=(1, 1), stride=(1, 1))
+          (transformer_blocks): ModuleList(
+            (0): BasicTransformerBlock(
+              (attn1): CrossAttention(
+                (to_q): Linear(in_features=1280, out_features=1280, bias=False)
+                (to_k): Linear(in_features=1280, out_features=1280, bias=False)
+                (to_v): Linear(in_features=1280, out_features=1280, bias=False)
+                (to_out): ModuleList(
+                  (0): Linear(in_features=1280, out_features=1280, bias=True)
+                  (1): Dropout(p=0.0, inplace=False)
+                )
+              )
+              (ff): FeedForward(
+                (net): ModuleList(
+                  (0): GEGLU(
+                    (proj): Linear(in_features=1280, out_features=10240, bias=True)
+                  )
+                  (1): Dropout(p=0.0, inplace=False)
+                  (2): Linear(in_features=5120, out_features=1280, bias=True)
+                )
+              )
+              (attn2): CrossAttention(
+                (to_q): Linear(in_features=1280, out_features=1280, bias=False)
+                (to_k): Linear(in_features=768, out_features=1280, bias=False)
+                (to_v): Linear(in_features=768, out_features=1280, bias=False)
+                (to_out): ModuleList(
+                  (0): Linear(in_features=1280, out_features=1280, bias=True)
+                  (1): Dropout(p=0.0, inplace=False)
+                )
+              )
+              (norm1): LayerNorm((1280,), eps=1e-05, elementwise_affine=True)
+              (norm2): LayerNorm((1280,), eps=1e-05, elementwise_affine=True)
+              (norm3): LayerNorm((1280,), eps=1e-05, elementwise_affine=True)
+            )
+          )
+          (proj_out): Conv2d(1280, 1280, kernel_size=(1, 1), stride=(1, 1))
+        )
+      )
+      (resnets): ModuleList(
+        (0): ResnetBlock2D(
+          (norm1): GroupNorm(32, 640, eps=1e-05, affine=True)
+          (conv1): Conv2d(640, 1280, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1))
+          (time_emb_proj): Linear(in_features=1280, out_features=1280, bias=True)
+          (norm2): GroupNorm(32, 1280, eps=1e-05, affine=True)
+          (dropout): Dropout(p=0.0, inplace=False)
+          (conv2): Conv2d(1280, 1280, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1))
+          (nonlinearity): SiLU()
+          (conv_shortcut): Conv2d(640, 1280, kernel_size=(1, 1), stride=(1, 1))
+        )
+        (1): ResnetBlock2D(
+          (norm1): GroupNorm(32, 1280, eps=1e-05, affine=True)
+          (conv1): Conv2d(1280, 1280, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1))
+          (time_emb_proj): Linear(in_features=1280, out_features=1280, bias=True)
+          (norm2): GroupNorm(32, 1280, eps=1e-05, affine=True)
+          (dropout): Dropout(p=0.0, inplace=False)
+          (conv2): Conv2d(1280, 1280, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1))
+          (nonlinearity): SiLU()
+        )
+      )
+      (downsamplers): ModuleList(
+        (0): Downsample2D(
+          (conv): Conv2d(1280, 1280, kernel_size=(3, 3), stride=(2, 2), padding=(1, 1))
+        )
+      )
+    )
+    (3): DownBlock2D(
+      (resnets): ModuleList(
+        (0): ResnetBlock2D(
+          (norm1): GroupNorm(32, 1280, eps=1e-05, affine=True)
+          (conv1): Conv2d(1280, 1280, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1))
+          (time_emb_proj): Linear(in_features=1280, out_features=1280, bias=True)
+          (norm2): GroupNorm(32, 1280, eps=1e-05, affine=True)
+          (dropout): Dropout(p=0.0, inplace=False)
+          (conv2): Conv2d(1280, 1280, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1))
+          (nonlinearity): SiLU()
+        )
+        (1): ResnetBlock2D(
+          (norm1): GroupNorm(32, 1280, eps=1e-05, affine=True)
+          (conv1): Conv2d(1280, 1280, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1))
+          (time_emb_proj): Linear(in_features=1280, out_features=1280, bias=True)
+          (norm2): GroupNorm(32, 1280, eps=1e-05, affine=True)
+          (dropout): Dropout(p=0.0, inplace=False)
+          (conv2): Conv2d(1280, 1280, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1))
+          (nonlinearity): SiLU()
+        )
+      )
+    )
+  )
+  (up_blocks): ModuleList(
+    (0): UpBlock2D(
+      (resnets): ModuleList(
+        (0): ResnetBlock2D(
+          (norm1): GroupNorm(32, 2560, eps=1e-05, affine=True)
+          (conv1): Conv2d(2560, 1280, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1))
+          (time_emb_proj): Linear(in_features=1280, out_features=1280, bias=True)
+          (norm2): GroupNorm(32, 1280, eps=1e-05, affine=True)
+          (dropout): Dropout(p=0.0, inplace=False)
+          (conv2): Conv2d(1280, 1280, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1))
+          (nonlinearity): SiLU()
+          (conv_shortcut): Conv2d(2560, 1280, kernel_size=(1, 1), stride=(1, 1))
+        )
+        (1): ResnetBlock2D(
+          (norm1): GroupNorm(32, 2560, eps=1e-05, affine=True)
+          (conv1): Conv2d(2560, 1280, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1))
+          (time_emb_proj): Linear(in_features=1280, out_features=1280, bias=True)
+          (norm2): GroupNorm(32, 1280, eps=1e-05, affine=True)
+          (dropout): Dropout(p=0.0, inplace=False)
+          (conv2): Conv2d(1280, 1280, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1))
+          (nonlinearity): SiLU()
+          (conv_shortcut): Conv2d(2560, 1280, kernel_size=(1, 1), stride=(1, 1))
+        )
+        (2): ResnetBlock2D(
+          (norm1): GroupNorm(32, 2560, eps=1e-05, affine=True)
+          (conv1): Conv2d(2560, 1280, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1))
+          (time_emb_proj): Linear(in_features=1280, out_features=1280, bias=True)
+          (norm2): GroupNorm(32, 1280, eps=1e-05, affine=True)
+          (dropout): Dropout(p=0.0, inplace=False)
+          (conv2): Conv2d(1280, 1280, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1))
+          (nonlinearity): SiLU()
+          (conv_shortcut): Conv2d(2560, 1280, kernel_size=(1, 1), stride=(1, 1))
+        )
+      )
+      (upsamplers): ModuleList(
+        (0): Upsample2D(
+          (conv): Conv2d(1280, 1280, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1))
+        )
+      )
+    )
+    (1): CrossAttnUpBlock2D(
+      (attentions): ModuleList(
+        (0): Transformer2DModel(
+          (norm): GroupNorm(32, 1280, eps=1e-06, affine=True)
+          (proj_in): Conv2d(1280, 1280, kernel_size=(1, 1), stride=(1, 1))
+          (transformer_blocks): ModuleList(
+            (0): BasicTransformerBlock(
+              (attn1): CrossAttention(
+                (to_q): Linear(in_features=1280, out_features=1280, bias=False)
+                (to_k): Linear(in_features=1280, out_features=1280, bias=False)
+                (to_v): Linear(in_features=1280, out_features=1280, bias=False)
+                (to_out): ModuleList(
+                  (0): Linear(in_features=1280, out_features=1280, bias=True)
+                  (1): Dropout(p=0.0, inplace=False)
+                )
+              )
+              (ff): FeedForward(
+                (net): ModuleList(
+                  (0): GEGLU(
+                    (proj): Linear(in_features=1280, out_features=10240, bias=True)
+                  )
+                  (1): Dropout(p=0.0, inplace=False)
+                  (2): Linear(in_features=5120, out_features=1280, bias=True)
+                )
+              )
+              (attn2): CrossAttention(
+                (to_q): Linear(in_features=1280, out_features=1280, bias=False)
+                (to_k): Linear(in_features=768, out_features=1280, bias=False)
+                (to_v): Linear(in_features=768, out_features=1280, bias=False)
+                (to_out): ModuleList(
+                  (0): Linear(in_features=1280, out_features=1280, bias=True)
+                  (1): Dropout(p=0.0, inplace=False)
+                )
+              )
+              (norm1): LayerNorm((1280,), eps=1e-05, elementwise_affine=True)
+              (norm2): LayerNorm((1280,), eps=1e-05, elementwise_affine=True)
+              (norm3): LayerNorm((1280,), eps=1e-05, elementwise_affine=True)
+            )
+          )
+          (proj_out): Conv2d(1280, 1280, kernel_size=(1, 1), stride=(1, 1))
+        )
+        (1): Transformer2DModel(
+          (norm): GroupNorm(32, 1280, eps=1e-06, affine=True)
+          (proj_in): Conv2d(1280, 1280, kernel_size=(1, 1), stride=(1, 1))
+          (transformer_blocks): ModuleList(
+            (0): BasicTransformerBlock(
+              (attn1): CrossAttention(
+                (to_q): Linear(in_features=1280, out_features=1280, bias=False)
+                (to_k): Linear(in_features=1280, out_features=1280, bias=False)
+                (to_v): Linear(in_features=1280, out_features=1280, bias=False)
+                (to_out): ModuleList(
+                  (0): Linear(in_features=1280, out_features=1280, bias=True)
+                  (1): Dropout(p=0.0, inplace=False)
+                )
+              )
+              (ff): FeedForward(
+                (net): ModuleList(
+                  (0): GEGLU(
+                    (proj): Linear(in_features=1280, out_features=10240, bias=True)
+                  )
+                  (1): Dropout(p=0.0, inplace=False)
+                  (2): Linear(in_features=5120, out_features=1280, bias=True)
+                )
+              )
+              (attn2): CrossAttention(
+                (to_q): Linear(in_features=1280, out_features=1280, bias=False)
+                (to_k): Linear(in_features=768, out_features=1280, bias=False)
+                (to_v): Linear(in_features=768, out_features=1280, bias=False)
+                (to_out): ModuleList(
+                  (0): Linear(in_features=1280, out_features=1280, bias=True)
+                  (1): Dropout(p=0.0, inplace=False)
+                )
+              )
+              (norm1): LayerNorm((1280,), eps=1e-05, elementwise_affine=True)
+              (norm2): LayerNorm((1280,), eps=1e-05, elementwise_affine=True)
+              (norm3): LayerNorm((1280,), eps=1e-05, elementwise_affine=True)
+            )
+          )
+          (proj_out): Conv2d(1280, 1280, kernel_size=(1, 1), stride=(1, 1))
+        )
+        (2): Transformer2DModel(
+          (norm): GroupNorm(32, 1280, eps=1e-06, affine=True)
+          (proj_in): Conv2d(1280, 1280, kernel_size=(1, 1), stride=(1, 1))
+          (transformer_blocks): ModuleList(
+            (0): BasicTransformerBlock(
+              (attn1): CrossAttention(
+                (to_q): Linear(in_features=1280, out_features=1280, bias=False)
+                (to_k): Linear(in_features=1280, out_features=1280, bias=False)
+                (to_v): Linear(in_features=1280, out_features=1280, bias=False)
+                (to_out): ModuleList(
+                  (0): Linear(in_features=1280, out_features=1280, bias=True)
+                  (1): Dropout(p=0.0, inplace=False)
+                )
+              )
+              (ff): FeedForward(
+                (net): ModuleList(
+                  (0): GEGLU(
+                    (proj): Linear(in_features=1280, out_features=10240, bias=True)
+                  )
+                  (1): Dropout(p=0.0, inplace=False)
+                  (2): Linear(in_features=5120, out_features=1280, bias=True)
+                )
+              )
+              (attn2): CrossAttention(
+                (to_q): Linear(in_features=1280, out_features=1280, bias=False)
+                (to_k): Linear(in_features=768, out_features=1280, bias=False)
+                (to_v): Linear(in_features=768, out_features=1280, bias=False)
+                (to_out): ModuleList(
+                  (0): Linear(in_features=1280, out_features=1280, bias=True)
+                  (1): Dropout(p=0.0, inplace=False)
+                )
+              )
+              (norm1): LayerNorm((1280,), eps=1e-05, elementwise_affine=True)
+              (norm2): LayerNorm((1280,), eps=1e-05, elementwise_affine=True)
+              (norm3): LayerNorm((1280,), eps=1e-05, elementwise_affine=True)
+            )
+          )
+          (proj_out): Conv2d(1280, 1280, kernel_size=(1, 1), stride=(1, 1))
+        )
+      )
+      (resnets): ModuleList(
+        (0): ResnetBlock2D(
+          (norm1): GroupNorm(32, 2560, eps=1e-05, affine=True)
+          (conv1): Conv2d(2560, 1280, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1))
+          (time_emb_proj): Linear(in_features=1280, out_features=1280, bias=True)
+          (norm2): GroupNorm(32, 1280, eps=1e-05, affine=True)
+          (dropout): Dropout(p=0.0, inplace=False)
+          (conv2): Conv2d(1280, 1280, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1))
+          (nonlinearity): SiLU()
+          (conv_shortcut): Conv2d(2560, 1280, kernel_size=(1, 1), stride=(1, 1))
+        )
+        (1): ResnetBlock2D(
+          (norm1): GroupNorm(32, 2560, eps=1e-05, affine=True)
+          (conv1): Conv2d(2560, 1280, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1))
+          (time_emb_proj): Linear(in_features=1280, out_features=1280, bias=True)
+          (norm2): GroupNorm(32, 1280, eps=1e-05, affine=True)
+          (dropout): Dropout(p=0.0, inplace=False)
+          (conv2): Conv2d(1280, 1280, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1))
+          (nonlinearity): SiLU()
+          (conv_shortcut): Conv2d(2560, 1280, kernel_size=(1, 1), stride=(1, 1))
+        )
+        (2): ResnetBlock2D(
+          (norm1): GroupNorm(32, 1920, eps=1e-05, affine=True)
+          (conv1): Conv2d(1920, 1280, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1))
+          (time_emb_proj): Linear(in_features=1280, out_features=1280, bias=True)
+          (norm2): GroupNorm(32, 1280, eps=1e-05, affine=True)
+          (dropout): Dropout(p=0.0, inplace=False)
+          (conv2): Conv2d(1280, 1280, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1))
+          (nonlinearity): SiLU()
+          (conv_shortcut): Conv2d(1920, 1280, kernel_size=(1, 1), stride=(1, 1))
+        )
+      )
+      (upsamplers): ModuleList(
+        (0): Upsample2D(
+          (conv): Conv2d(1280, 1280, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1))
+        )
+      )
+    )
+    (2): CrossAttnUpBlock2D(
+      (attentions): ModuleList(
+        (0): Transformer2DModel(
+          (norm): GroupNorm(32, 640, eps=1e-06, affine=True)
+          (proj_in): Conv2d(640, 640, kernel_size=(1, 1), stride=(1, 1))
+          (transformer_blocks): ModuleList(
+            (0): BasicTransformerBlock(
+              (attn1): CrossAttention(
+                (to_q): Linear(in_features=640, out_features=640, bias=False)
+                (to_k): Linear(in_features=640, out_features=640, bias=False)
+                (to_v): Linear(in_features=640, out_features=640, bias=False)
+                (to_out): ModuleList(
+                  (0): Linear(in_features=640, out_features=640, bias=True)
+                  (1): Dropout(p=0.0, inplace=False)
+                )
+              )
+              (ff): FeedForward(
+                (net): ModuleList(
+                  (0): GEGLU(
+                    (proj): Linear(in_features=640, out_features=5120, bias=True)
+                  )
+                  (1): Dropout(p=0.0, inplace=False)
+                  (2): Linear(in_features=2560, out_features=640, bias=True)
+                )
+              )
+              (attn2): CrossAttention(
+                (to_q): Linear(in_features=640, out_features=640, bias=False)
+                (to_k): Linear(in_features=768, out_features=640, bias=False)
+                (to_v): Linear(in_features=768, out_features=640, bias=False)
+                (to_out): ModuleList(
+                  (0): Linear(in_features=640, out_features=640, bias=True)
+                  (1): Dropout(p=0.0, inplace=False)
+                )
+              )
+              (norm1): LayerNorm((640,), eps=1e-05, elementwise_affine=True)
+              (norm2): LayerNorm((640,), eps=1e-05, elementwise_affine=True)
+              (norm3): LayerNorm((640,), eps=1e-05, elementwise_affine=True)
+            )
+          )
+          (proj_out): Conv2d(640, 640, kernel_size=(1, 1), stride=(1, 1))
+        )
+        (1): Transformer2DModel(
+          (norm): GroupNorm(32, 640, eps=1e-06, affine=True)
+          (proj_in): Conv2d(640, 640, kernel_size=(1, 1), stride=(1, 1))
+          (transformer_blocks): ModuleList(
+            (0): BasicTransformerBlock(
+              (attn1): CrossAttention(
+                (to_q): Linear(in_features=640, out_features=640, bias=False)
+                (to_k): Linear(in_features=640, out_features=640, bias=False)
+                (to_v): Linear(in_features=640, out_features=640, bias=False)
+                (to_out): ModuleList(
+                  (0): Linear(in_features=640, out_features=640, bias=True)
+                  (1): Dropout(p=0.0, inplace=False)
+                )
+              )
+              (ff): FeedForward(
+                (net): ModuleList(
+                  (0): GEGLU(
+                    (proj): Linear(in_features=640, out_features=5120, bias=True)
+                  )
+                  (1): Dropout(p=0.0, inplace=False)
+                  (2): Linear(in_features=2560, out_features=640, bias=True)
+                )
+              )
+              (attn2): CrossAttention(
+                (to_q): Linear(in_features=640, out_features=640, bias=False)
+                (to_k): Linear(in_features=768, out_features=640, bias=False)
+                (to_v): Linear(in_features=768, out_features=640, bias=False)
+                (to_out): ModuleList(
+                  (0): Linear(in_features=640, out_features=640, bias=True)
+                  (1): Dropout(p=0.0, inplace=False)
+                )
+              )
+              (norm1): LayerNorm((640,), eps=1e-05, elementwise_affine=True)
+              (norm2): LayerNorm((640,), eps=1e-05, elementwise_affine=True)
+              (norm3): LayerNorm((640,), eps=1e-05, elementwise_affine=True)
+            )
+          )
+          (proj_out): Conv2d(640, 640, kernel_size=(1, 1), stride=(1, 1))
+        )
+        (2): Transformer2DModel(
+          (norm): GroupNorm(32, 640, eps=1e-06, affine=True)
+          (proj_in): Conv2d(640, 640, kernel_size=(1, 1), stride=(1, 1))
+          (transformer_blocks): ModuleList(
+            (0): BasicTransformerBlock(
+              (attn1): CrossAttention(
+                (to_q): Linear(in_features=640, out_features=640, bias=False)
+                (to_k): Linear(in_features=640, out_features=640, bias=False)
+                (to_v): Linear(in_features=640, out_features=640, bias=False)
+                (to_out): ModuleList(
+                  (0): Linear(in_features=640, out_features=640, bias=True)
+                  (1): Dropout(p=0.0, inplace=False)
+                )
+              )
+              (ff): FeedForward(
+                (net): ModuleList(
+                  (0): GEGLU(
+                    (proj): Linear(in_features=640, out_features=5120, bias=True)
+                  )
+                  (1): Dropout(p=0.0, inplace=False)
+                  (2): Linear(in_features=2560, out_features=640, bias=True)
+                )
+              )
+              (attn2): CrossAttention(
+                (to_q): Linear(in_features=640, out_features=640, bias=False)
+                (to_k): Linear(in_features=768, out_features=640, bias=False)
+                (to_v): Linear(in_features=768, out_features=640, bias=False)
+                (to_out): ModuleList(
+                  (0): Linear(in_features=640, out_features=640, bias=True)
+                  (1): Dropout(p=0.0, inplace=False)
+                )
+              )
+              (norm1): LayerNorm((640,), eps=1e-05, elementwise_affine=True)
+              (norm2): LayerNorm((640,), eps=1e-05, elementwise_affine=True)
+              (norm3): LayerNorm((640,), eps=1e-05, elementwise_affine=True)
+            )
+          )
+          (proj_out): Conv2d(640, 640, kernel_size=(1, 1), stride=(1, 1))
+        )
+      )
+      (resnets): ModuleList(
+        (0): ResnetBlock2D(
+          (norm1): GroupNorm(32, 1920, eps=1e-05, affine=True)
+          (conv1): Conv2d(1920, 640, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1))
+          (time_emb_proj): Linear(in_features=1280, out_features=640, bias=True)
+          (norm2): GroupNorm(32, 640, eps=1e-05, affine=True)
+          (dropout): Dropout(p=0.0, inplace=False)
+          (conv2): Conv2d(640, 640, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1))
+          (nonlinearity): SiLU()
+          (conv_shortcut): Conv2d(1920, 640, kernel_size=(1, 1), stride=(1, 1))
+        )
+        (1): ResnetBlock2D(
+          (norm1): GroupNorm(32, 1280, eps=1e-05, affine=True)
+          (conv1): Conv2d(1280, 640, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1))
+          (time_emb_proj): Linear(in_features=1280, out_features=640, bias=True)
+          (norm2): GroupNorm(32, 640, eps=1e-05, affine=True)
+          (dropout): Dropout(p=0.0, inplace=False)
+          (conv2): Conv2d(640, 640, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1))
+          (nonlinearity): SiLU()
+          (conv_shortcut): Conv2d(1280, 640, kernel_size=(1, 1), stride=(1, 1))
+        )
+        (2): ResnetBlock2D(
+          (norm1): GroupNorm(32, 960, eps=1e-05, affine=True)
+          (conv1): Conv2d(960, 640, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1))
+          (time_emb_proj): Linear(in_features=1280, out_features=640, bias=True)
+          (norm2): GroupNorm(32, 640, eps=1e-05, affine=True)
+          (dropout): Dropout(p=0.0, inplace=False)
+          (conv2): Conv2d(640, 640, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1))
+          (nonlinearity): SiLU()
+          (conv_shortcut): Conv2d(960, 640, kernel_size=(1, 1), stride=(1, 1))
+        )
+      )
+      (upsamplers): ModuleList(
+        (0): Upsample2D(
+          (conv): Conv2d(640, 640, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1))
+        )
+      )
+    )
+    (3): CrossAttnUpBlock2D(
+      (attentions): ModuleList(
+        (0): Transformer2DModel(
+          (norm): GroupNorm(32, 320, eps=1e-06, affine=True)
+          (proj_in): Conv2d(320, 320, kernel_size=(1, 1), stride=(1, 1))
+          (transformer_blocks): ModuleList(
+            (0): BasicTransformerBlock(
+              (attn1): CrossAttention(
+                (to_q): Linear(in_features=320, out_features=320, bias=False)
+                (to_k): Linear(in_features=320, out_features=320, bias=False)
+                (to_v): Linear(in_features=320, out_features=320, bias=False)
+                (to_out): ModuleList(
+                  (0): Linear(in_features=320, out_features=320, bias=True)
+                  (1): Dropout(p=0.0, inplace=False)
+                )
+              )
+              (ff): FeedForward(
+                (net): ModuleList(
+                  (0): GEGLU(
+                    (proj): Linear(in_features=320, out_features=2560, bias=True)
+                  )
+                  (1): Dropout(p=0.0, inplace=False)
+                  (2): Linear(in_features=1280, out_features=320, bias=True)
+                )
+              )
+              (attn2): CrossAttention(
+                (to_q): Linear(in_features=320, out_features=320, bias=False)
+                (to_k): Linear(in_features=768, out_features=320, bias=False)
+                (to_v): Linear(in_features=768, out_features=320, bias=False)
+                (to_out): ModuleList(
+                  (0): Linear(in_features=320, out_features=320, bias=True)
+                  (1): Dropout(p=0.0, inplace=False)
+                )
+              )
+              (norm1): LayerNorm((320,), eps=1e-05, elementwise_affine=True)
+              (norm2): LayerNorm((320,), eps=1e-05, elementwise_affine=True)
+              (norm3): LayerNorm((320,), eps=1e-05, elementwise_affine=True)
+            )
+          )
+          (proj_out): Conv2d(320, 320, kernel_size=(1, 1), stride=(1, 1))
+        )
+        (1): Transformer2DModel(
+          (norm): GroupNorm(32, 320, eps=1e-06, affine=True)
+          (proj_in): Conv2d(320, 320, kernel_size=(1, 1), stride=(1, 1))
+          (transformer_blocks): ModuleList(
+            (0): BasicTransformerBlock(
+              (attn1): CrossAttention(
+                (to_q): Linear(in_features=320, out_features=320, bias=False)
+                (to_k): Linear(in_features=320, out_features=320, bias=False)
+                (to_v): Linear(in_features=320, out_features=320, bias=False)
+                (to_out): ModuleList(
+                  (0): Linear(in_features=320, out_features=320, bias=True)
+                  (1): Dropout(p=0.0, inplace=False)
+                )
+              )
+              (ff): FeedForward(
+                (net): ModuleList(
+                  (0): GEGLU(
+                    (proj): Linear(in_features=320, out_features=2560, bias=True)
+                  )
+                  (1): Dropout(p=0.0, inplace=False)
+                  (2): Linear(in_features=1280, out_features=320, bias=True)
+                )
+              )
+              (attn2): CrossAttention(
+                (to_q): Linear(in_features=320, out_features=320, bias=False)
+                (to_k): Linear(in_features=768, out_features=320, bias=False)
+                (to_v): Linear(in_features=768, out_features=320, bias=False)
+                (to_out): ModuleList(
+                  (0): Linear(in_features=320, out_features=320, bias=True)
+                  (1): Dropout(p=0.0, inplace=False)
+                )
+              )
+              (norm1): LayerNorm((320,), eps=1e-05, elementwise_affine=True)
+              (norm2): LayerNorm((320,), eps=1e-05, elementwise_affine=True)
+              (norm3): LayerNorm((320,), eps=1e-05, elementwise_affine=True)
+            )
+          )
+          (proj_out): Conv2d(320, 320, kernel_size=(1, 1), stride=(1, 1))
+        )
+        (2): Transformer2DModel(
+          (norm): GroupNorm(32, 320, eps=1e-06, affine=True)
+          (proj_in): Conv2d(320, 320, kernel_size=(1, 1), stride=(1, 1))
+          (transformer_blocks): ModuleList(
+            (0): BasicTransformerBlock(
+              (attn1): CrossAttention(
+                (to_q): Linear(in_features=320, out_features=320, bias=False)
+                (to_k): Linear(in_features=320, out_features=320, bias=False)
+                (to_v): Linear(in_features=320, out_features=320, bias=False)
+                (to_out): ModuleList(
+                  (0): Linear(in_features=320, out_features=320, bias=True)
+                  (1): Dropout(p=0.0, inplace=False)
+                )
+              )
+              (ff): FeedForward(
+                (net): ModuleList(
+                  (0): GEGLU(
+                    (proj): Linear(in_features=320, out_features=2560, bias=True)
+                  )
+                  (1): Dropout(p=0.0, inplace=False)
+                  (2): Linear(in_features=1280, out_features=320, bias=True)
+                )
+              )
+              (attn2): CrossAttention(
+                (to_q): Linear(in_features=320, out_features=320, bias=False)
+                (to_k): Linear(in_features=768, out_features=320, bias=False)
+                (to_v): Linear(in_features=768, out_features=320, bias=False)
+                (to_out): ModuleList(
+                  (0): Linear(in_features=320, out_features=320, bias=True)
+                  (1): Dropout(p=0.0, inplace=False)
+                )
+              )
+              (norm1): LayerNorm((320,), eps=1e-05, elementwise_affine=True)
+              (norm2): LayerNorm((320,), eps=1e-05, elementwise_affine=True)
+              (norm3): LayerNorm((320,), eps=1e-05, elementwise_affine=True)
+            )
+          )
+          (proj_out): Conv2d(320, 320, kernel_size=(1, 1), stride=(1, 1))
+        )
+      )
+      (resnets): ModuleList(
+        (0): ResnetBlock2D(
+          (norm1): GroupNorm(32, 960, eps=1e-05, affine=True)
+          (conv1): Conv2d(960, 320, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1))
+          (time_emb_proj): Linear(in_features=1280, out_features=320, bias=True)
+          (norm2): GroupNorm(32, 320, eps=1e-05, affine=True)
+          (dropout): Dropout(p=0.0, inplace=False)
+          (conv2): Conv2d(320, 320, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1))
+          (nonlinearity): SiLU()
+          (conv_shortcut): Conv2d(960, 320, kernel_size=(1, 1), stride=(1, 1))
+        )
+        (1): ResnetBlock2D(
+          (norm1): GroupNorm(32, 640, eps=1e-05, affine=True)
+          (conv1): Conv2d(640, 320, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1))
+          (time_emb_proj): Linear(in_features=1280, out_features=320, bias=True)
+          (norm2): GroupNorm(32, 320, eps=1e-05, affine=True)
+          (dropout): Dropout(p=0.0, inplace=False)
+          (conv2): Conv2d(320, 320, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1))
+          (nonlinearity): SiLU()
+          (conv_shortcut): Conv2d(640, 320, kernel_size=(1, 1), stride=(1, 1))
+        )
+        (2): ResnetBlock2D(
+          (norm1): GroupNorm(32, 640, eps=1e-05, affine=True)
+          (conv1): Conv2d(640, 320, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1))
+          (time_emb_proj): Linear(in_features=1280, out_features=320, bias=True)
+          (norm2): GroupNorm(32, 320, eps=1e-05, affine=True)
+          (dropout): Dropout(p=0.0, inplace=False)
+          (conv2): Conv2d(320, 320, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1))
+          (nonlinearity): SiLU()
+          (conv_shortcut): Conv2d(640, 320, kernel_size=(1, 1), stride=(1, 1))
+        )
+      )
+    )
+  )
+  (mid_block): UNetMidBlock2DCrossAttn(
+    (attentions): ModuleList(
+      (0): Transformer2DModel(
+        (norm): GroupNorm(32, 1280, eps=1e-06, affine=True)
+        (proj_in): Conv2d(1280, 1280, kernel_size=(1, 1), stride=(1, 1))
+        (transformer_blocks): ModuleList(
+          (0): BasicTransformerBlock(
+            (attn1): CrossAttention(
+              (to_q): Linear(in_features=1280, out_features=1280, bias=False)
+              (to_k): Linear(in_features=1280, out_features=1280, bias=False)
+              (to_v): Linear(in_features=1280, out_features=1280, bias=False)
+              (to_out): ModuleList(
+                (0): Linear(in_features=1280, out_features=1280, bias=True)
+                (1): Dropout(p=0.0, inplace=False)
+              )
+            )
+            (ff): FeedForward(
+              (net): ModuleList(
+                (0): GEGLU(
+                  (proj): Linear(in_features=1280, out_features=10240, bias=True)
+                )
+                (1): Dropout(p=0.0, inplace=False)
+                (2): Linear(in_features=5120, out_features=1280, bias=True)
+              )
+            )
+            (attn2): CrossAttention(
+              (to_q): Linear(in_features=1280, out_features=1280, bias=False)
+              (to_k): Linear(in_features=768, out_features=1280, bias=False)
+              (to_v): Linear(in_features=768, out_features=1280, bias=False)
+              (to_out): ModuleList(
+                (0): Linear(in_features=1280, out_features=1280, bias=True)
+                (1): Dropout(p=0.0, inplace=False)
+              )
+            )
+            (norm1): LayerNorm((1280,), eps=1e-05, elementwise_affine=True)
+            (norm2): LayerNorm((1280,), eps=1e-05, elementwise_affine=True)
+            (norm3): LayerNorm((1280,), eps=1e-05, elementwise_affine=True)
+          )
+        )
+        (proj_out): Conv2d(1280, 1280, kernel_size=(1, 1), stride=(1, 1))
+      )
+    )
+    (resnets): ModuleList(
+      (0): ResnetBlock2D(
+        (norm1): GroupNorm(32, 1280, eps=1e-05, affine=True)
+        (conv1): Conv2d(1280, 1280, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1))
+        (time_emb_proj): Linear(in_features=1280, out_features=1280, bias=True)
+        (norm2): GroupNorm(32, 1280, eps=1e-05, affine=True)
+        (dropout): Dropout(p=0.0, inplace=False)
+        (conv2): Conv2d(1280, 1280, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1))
+        (nonlinearity): SiLU()
+      )
+      (1): ResnetBlock2D(
+        (norm1): GroupNorm(32, 1280, eps=1e-05, affine=True)
+        (conv1): Conv2d(1280, 1280, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1))
+        (time_emb_proj): Linear(in_features=1280, out_features=1280, bias=True)
+        (norm2): GroupNorm(32, 1280, eps=1e-05, affine=True)
+        (dropout): Dropout(p=0.0, inplace=False)
+        (conv2): Conv2d(1280, 1280, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1))
+        (nonlinearity): SiLU()
+      )
+    )
+  )
+  (conv_norm_out): GroupNorm(32, 320, eps=1e-05, affine=True)
+  (conv_act): SiLU()
+  (conv_out): Conv2d(320, 4, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1))
 )
```

### Comparing `hcpdiff-0.2.2/hcpdiff/data/cond_pair_dataset.py` & `hcpdiff-0.3.0/hcpdiff/data/cond_pair_dataset.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,51 +1,49 @@
-"""
-pair_dataset.py
-====================
-    :Name:        text-image pair dataset
-    :Author:      Dong Ziyi
-    :Affiliation: HCP Lab, SYSU
-    :Created:     10/03/2023
-    :Licence:     Apache-2.0
-"""
-
-from typing import Callable, Iterable
-from .bucket import BaseBucket
-import os.path
-
-import torch
-import cv2
-from .pair_dataset import TextImagePairDataset
-from hcpdiff.utils.utils import get_file_name
-from torchvision import transforms
-
-class TextImageCondPairDataset(TextImagePairDataset):
-    """
-    A dataset to prepare the instance and class images with the prompts for fine-tuning the model.
-    It pre-processes the images and the tokenizes prompts.
-    """
-
-    def __init__(self, prompt_template: str, tokenizer, tokenizer_repeats: int = 1, caption_file: str = None,
-                 att_mask: str = None, att_mask_encode: bool = False, bg_color: Iterable[int] = (255, 255, 255),
-                 image_transforms: Callable = None, tag_transforms: Callable = None, bucket: BaseBucket = None, return_path: bool = False,
-                 cond_dir: str = None):
-        super().__init__(prompt_template, tokenizer, tokenizer_repeats, caption_file, att_mask, att_mask_encode, bg_color, image_transforms,
-                         tag_transforms, bucket, return_path)
-        self.cond_dir = cond_dir
-        self.cond_transform = transforms.ToTensor()
-
-    def load_data(self, path, size):
-        img_name = os.path.basename(path)
-        image = self.load_image(path)
-        img_cond = self.load_image(os.path.join(self.cond_dir, img_name))
-        att_mask = self.get_att_map(get_file_name(img_name))
-        if att_mask is None:
-            data = self.bucket.crop_resize({"img": image, "cond":img_cond}, size)
-            image = self.image_transforms(data['img'])  # resize to bucket size
-            img_cond = self.cond_transform(data['cond'])
-            att_mask = torch.ones((size[1] // 8, size[0] // 8))
-        else:
-            data = self.bucket.crop_resize({"img": image, "mask": att_mask, "cond":img_cond}, size)
-            image = self.image_transforms(data['img'])
-            img_cond = self.cond_transform(data['cond'])
-            att_mask = torch.tensor(cv2.resize(att_mask, (size[0] // 8, size[1] // 8), interpolation=cv2.INTER_LINEAR))
-        return {'img': image, 'mask': att_mask, "cond":img_cond}
+"""
+pair_dataset.py
+====================
+    :Name:        text-image pair dataset
+    :Author:      Dong Ziyi
+    :Affiliation: HCP Lab, SYSU
+    :Created:     10/03/2023
+    :Licence:     Apache-2.0
+"""
+
+from typing import Callable, Iterable, Dict
+from .bucket import BaseBucket
+import os.path
+
+import torch
+import cv2
+from .pair_dataset import TextImagePairDataset
+from hcpdiff.utils.utils import get_file_name
+from torchvision import transforms
+
+class TextImageCondPairDataset(TextImagePairDataset):
+    """
+    A dataset to prepare the instance and class images with the prompts for fine-tuning the model.
+    It pre-processes the images and the tokenizes prompts.
+    """
+
+    def __init__(self, tokenizer, tokenizer_repeats: int = 1, att_mask_encode: bool = False,
+                 bucket: BaseBucket = None, source: Dict = None, return_path: bool = False, **kwargs):
+        super().__init__(tokenizer, tokenizer_repeats, att_mask_encode, bucket, source, return_path)
+        for data_source in source.values():
+            self.source_dict[data_source.img_root].cond_dir = data_source.cond_dir
+        self.cond_transform = transforms.ToTensor()
+
+    def load_data(self, path, size):
+        img_root, img_name = os.path.split(path)
+        image = self.load_image(path)
+        img_cond = self.load_image(os.path.join(self.source_dict[img_root].cond_dir, img_name))
+        att_mask = self.get_att_map(img_root, get_file_name(img_name))
+        if att_mask is None:
+            data = self.bucket.crop_resize({"img": image, "cond":img_cond}, size)
+            image = self.source_dict[img_root].image_transforms(data['img'])  # resize to bucket size
+            img_cond = self.cond_transform(data['cond'])
+            att_mask = torch.ones((size[1] // 8, size[0] // 8))
+        else:
+            data = self.bucket.crop_resize({"img": image, "mask": att_mask, "cond":img_cond}, size)
+            image = self.source_dict[img_root].image_transforms(data['img'])
+            img_cond = self.cond_transform(data['cond'])
+            att_mask = torch.tensor(cv2.resize(att_mask, (size[0] // 8, size[1] // 8), interpolation=cv2.INTER_LINEAR))
+        return {'img': image, 'mask': att_mask, "cond":img_cond}
```

### Comparing `hcpdiff-0.2.2/hcpdiff/data/pair_dataset.py` & `hcpdiff-0.3.0/hcpdiff/data/pair_dataset.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,142 +1,150 @@
-"""
-pair_dataset.py
-====================
-    :Name:        text-image pair dataset
-    :Author:      Dong Ziyi
-    :Affiliation: HCP Lab, SYSU
-    :Created:     10/03/2023
-    :Licence:     Apache-2.0
-"""
-
-from typing import Tuple, Callable, Iterable
-import os.path
-
-import torch
-from PIL import Image
-import cv2
-from torch.utils.data import Dataset
-from .bucket import BaseBucket
-from hcpdiff.utils.caption_tools import *
-from hcpdiff.utils.utils import _default, get_file_name, get_file_ext
-from hcpdiff.utils.img_size_tool import types_support
-from tqdm.auto import tqdm
-
-import json
-import yaml
-
-
-class TextImagePairDataset(Dataset):
-    """
-    A dataset to prepare the instance and class images with the prompts for fine-tuning the model.
-    It pre-processes the images and the tokenizes prompts.
-    """
-
-    def __init__(self, prompt_template: str, tokenizer, tokenizer_repeats: int = 1, caption_file: str = None,
-                 att_mask: str = None, att_mask_encode: bool = False, bg_color: Iterable[int] = (255, 255, 255),
-                 image_transforms: Callable = None, tag_transforms: Callable = None, bucket: BaseBucket = None, return_path: bool = False):
-        self.return_path = return_path
-
-        self.tokenizer = tokenizer
-        self.tokenizer_repeats = tokenizer_repeats
-
-        self.bucket: BaseBucket = bucket
-        self.caption_dict = self.load_captions(caption_file)
-        self.att_mask_path = {} if att_mask is None else \
-            {get_file_name(file): os.path.join(att_mask, file) for file in os.listdir(att_mask) if
-             get_file_ext(file) in types_support}
-        self.att_mask_encode = att_mask_encode
-
-        self.prompt_template = self.load_template(prompt_template)
-
-        self.image_transforms = _default(image_transforms, image_transforms)
-        self.tag_transforms = _default(tag_transforms, tag_transforms)
-        self.bg_color = tuple(bg_color)
-
-        self.latents = None  # Cache latents for faster training. Works only without image argumentations.
-
-    def load_image(self, path):
-        image = Image.open(path)
-        if image.mode == 'RGBA':
-            x, y = image.size
-            canvas = Image.new('RGBA', image.size, self.bg_color)
-            canvas.paste(image, (0, 0, x, y), image)
-            image = canvas
-        return image.convert("RGB")
-
-    def load_captions(self, caption_file):
-        if caption_file is None:
-            return dict()
-        elif caption_file.endswith('.json'):
-            with open(caption_file, 'r', encoding='utf-8') as f:
-                return json.loads(f.read())
-        elif caption_file.endswith('.yaml'):
-            with open(caption_file, 'r', encoding='utf-8') as f:
-                return yaml.load(f.read(), Loader=yaml.FullLoader)
-        else:
-            return dict()
-
-    def load_template(self, template_file):
-        with open(template_file, 'r', encoding='utf-8') as f:
-            return f.read().strip().split('\n')
-
-    @torch.no_grad()
-    def cache_latents(self, vae, weight_dtype, device, show_prog=True):
-        self.latents = {}
-        self.bucket.rest(0)
-
-        for path, size in tqdm(self.bucket, disable=not show_prog):
-            img_name = os.path.basename(path)
-            if img_name not in self.latents:
-                data = self.load_data(path, size)
-                image = data['img'].unsqueeze(0).to(device, dtype=weight_dtype)
-                latents = vae.encode(image).latent_dist.sample().squeeze(0)
-                data['img'] = (latents * 0.18215).cpu()
-                self.latents[img_name] = data
-
-    def get_att_map(self, img_name):
-        if img_name not in self.att_mask_path:
-            return None
-        att_mask = Image.open(self.att_mask_path[img_name]).convert("L")
-        np_mask = np.array(att_mask).astype(float)
-        np_mask[np_mask <= 127 + 0.1] = (np_mask[np_mask <= 127 + 0.1] / 127.)
-        np_mask[np_mask > 127] = ((np_mask[np_mask > 127] - 127) / 128.) * 4 + 1
-        return np_mask
-
-    def load_data(self, path, size):
-        img_name = os.path.basename(path)
-        image = self.load_image(path)
-        att_mask = self.get_att_map(get_file_name(img_name))
-        if att_mask is None:
-            data = self.bucket.crop_resize({"img": image}, size)
-            image = self.image_transforms(data['img'])  # resize to bucket size
-            att_mask = torch.ones((size[1] // 8, size[0] // 8))
-        else:
-            data = self.bucket.crop_resize({"img": image, "mask": att_mask}, size)
-            image = self.image_transforms(data['img'])
-            att_mask = torch.tensor(cv2.resize(att_mask, (size[0] // 8, size[1] // 8), interpolation=cv2.INTER_LINEAR))
-        return {'img': image, 'mask': att_mask}
-
-    def __len__(self):
-        return len(self.bucket)
-
-    def __getitem__(self, index):
-        path, size = self.bucket[index]
-        img_name = os.path.basename(path)
-
-        if self.latents is None:
-            data = self.load_data(path, size)
-        else:
-            data = self.latents[img_name]
-
-        caption_ist = self.caption_dict[img_name] if img_name in self.caption_dict else None
-        prompt_ist = self.tag_transforms({'prompt': random.choice(self.prompt_template), 'caption': caption_ist})['prompt']
-
-        # tokenize Sp or (Sn, Sp)
-        prompt_ids = self.tokenizer(
-            prompt_ist, truncation=True, padding="max_length", return_tensors="pt",
-            max_length=self.tokenizer.model_max_length * self.tokenizer_repeats).input_ids.squeeze()
-
-        if self.return_path:
-            return data, prompt_ids, path
-        else:
-            return data, prompt_ids
+"""
+pair_dataset.py
+====================
+    :Name:        text-image pair dataset
+    :Author:      Dong Ziyi
+    :Affiliation: HCP Lab, SYSU
+    :Created:     10/03/2023
+    :Licence:     Apache-2.0
+"""
+
+import json
+import os.path
+from argparse import Namespace
+
+import cv2
+import torch
+import yaml
+from PIL import Image
+from torch.utils.data import Dataset
+from tqdm.auto import tqdm
+
+from hcpdiff.utils.caption_tools import *
+from hcpdiff.utils.img_size_tool import types_support
+from hcpdiff.utils.utils import get_file_name, get_file_ext
+from .bucket import BaseBucket
+
+
+class TextImagePairDataset(Dataset):
+    """
+    A dataset to prepare the instance and class images with the prompts for fine-tuning the model.
+    It pre-processes the images and the tokenizes prompts.
+    """
+
+    def __init__(self, tokenizer, tokenizer_repeats: int = 1, att_mask_encode: bool = False,
+                 bucket: BaseBucket = None, source: Dict = None, return_path: bool = False, **kwargs):
+        self.return_path = return_path
+
+        self.tokenizer = tokenizer
+        self.tokenizer_repeats = tokenizer_repeats
+
+        self.bucket: BaseBucket = bucket
+        self.att_mask_encode = att_mask_encode
+
+        self.source_dict = {}
+        for data_source in source.values():
+            source_metas = Namespace()
+            source_metas.caption_dict = self.load_captions(data_source.caption_file)
+            source_metas.att_mask_path = {} if data_source.att_mask is None else \
+                {get_file_name(file): os.path.join(data_source.att_mask, file)
+                 for file in os.listdir(data_source.att_mask) if get_file_ext(file) in types_support}
+            source_metas.prompt_template = self.load_template(data_source.prompt_template)
+            source_metas.image_transforms = data_source.image_transforms
+            source_metas.tag_transforms = data_source.tag_transforms
+            source_metas.bg_color = tuple(data_source.bg_color)
+
+            self.source_dict[os.path.dirname(data_source.img_root+'/')] = source_metas
+
+        self.latents = None  # Cache latents for faster training. Works only without image argumentations.
+
+    def load_image(self, path):
+        image = Image.open(path)
+        if image.mode == 'RGBA':
+            img_root = os.path.dirname(path)
+            x, y = image.size
+            canvas = Image.new('RGBA', image.size, self.source_dict[img_root].bg_color)
+            canvas.paste(image, (0, 0, x, y), image)
+            image = canvas
+        return image.convert("RGB")
+
+    def load_captions(self, caption_file):
+        if caption_file is None:
+            return dict()
+        elif caption_file.endswith('.json'):
+            with open(caption_file, 'r', encoding='utf-8') as f:
+                return json.loads(f.read())
+        elif caption_file.endswith('.yaml'):
+            with open(caption_file, 'r', encoding='utf-8') as f:
+                return yaml.load(f.read(), Loader=yaml.FullLoader)
+        else:
+            return dict()
+
+    def load_template(self, template_file):
+        with open(template_file, 'r', encoding='utf-8') as f:
+            return f.read().strip().split('\n')
+
+    @torch.no_grad()
+    def cache_latents(self, vae, weight_dtype, device, show_prog=True):
+        self.latents = {}
+        self.bucket.rest(0)
+
+        for path, size in tqdm(self.bucket, disable=not show_prog):
+            img_name = os.path.basename(path)
+            if img_name not in self.latents:
+                data = self.load_data(path, size)
+                image = data['img'].unsqueeze(0).to(device, dtype=weight_dtype)
+                latents = vae.encode(image).latent_dist.sample().squeeze(0)
+                data['img'] = (latents * 0.18215).cpu()
+                self.latents[img_name] = data
+
+    def get_att_map(self, img_root, img_name):
+        if img_name not in self.source_dict[img_root].att_mask_path:
+            return None
+        att_mask = Image.open(self.source_dict[img_root].att_mask_path[img_name]).convert("L")
+        np_mask = np.array(att_mask).astype(float)
+        np_mask[np_mask <= 127 + 0.1] = (np_mask[np_mask <= 127 + 0.1] / 127.)
+        np_mask[np_mask > 127] = ((np_mask[np_mask > 127] - 127) / 128.) * 4 + 1
+        return np_mask
+
+    def load_data(self, path, size):
+        img_root, img_name = os.path.split(path)
+        image = self.load_image(path)
+        att_mask = self.get_att_map(img_root, get_file_name(img_name))
+        if att_mask is None:
+            data = self.bucket.crop_resize({"img": image}, size)
+            image = self.source_dict[img_root].image_transforms(data['img'])  # resize to bucket size
+            att_mask = torch.ones((size[1] // 8, size[0] // 8))
+        else:
+            data = self.bucket.crop_resize({"img": image, "mask": att_mask}, size)
+            image = self.source_dict[img_root].image_transforms(data['img'])
+            att_mask = torch.tensor(cv2.resize(att_mask, (size[0] // 8, size[1] // 8), interpolation=cv2.INTER_LINEAR))
+        return {'img': image, 'mask': att_mask}
+
+    def __len__(self):
+        return len(self.bucket)
+
+    def __getitem__(self, index):
+        path, size = self.bucket[index]
+        img_root, img_name = os.path.split(path)
+
+        if self.latents is None:
+            data = self.load_data(path, size)
+        else:
+            data = self.latents[img_name]
+
+        caption_ist = self.source_dict[img_root].caption_dict[img_name] if img_name in \
+                            self.source_dict[img_root].caption_dict else None
+        prompt_ist = self.source_dict[img_root].tag_transforms(
+            {'prompt': random.choice(self.source_dict[img_root].prompt_template), 'caption': caption_ist})['prompt']
+
+        # tokenize Sp or (Sn, Sp)
+        prompt_ids = self.tokenizer(
+            prompt_ist, truncation=True, padding="max_length", return_tensors="pt",
+            max_length=self.tokenizer.model_max_length * self.tokenizer_repeats).input_ids.squeeze()
+
+        data['prompt'] = prompt_ids
+
+        if self.return_path:
+            return data, path
+        else:
+            return data
```

### Comparing `hcpdiff-0.2.2/hcpdiff/data/utils.py` & `hcpdiff-0.3.0/hcpdiff/data/utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,76 +1,86 @@
-from PIL import Image
-import torch
-import cv2
-
-from torchvision import transforms as T
-from torchvision.transforms import functional as F
-
-
-class DualRandomCrop(object):
-    def __init__(self, size):
-        self.size = size
-
-    def __call__(self, img):
-        crop_params = T.RandomCrop.get_params(img['img'], self.size)
-        img['img'] = F.crop(img['img'], *crop_params)
-        if "mask" in img:
-            img['mask'] = F.crop(img['mask'], *crop_params)
-        if "cond" in img:
-            img['cond'] = F.crop(img['cond'], *crop_params)
-        return img
-
-def resize_crop_fix(img, target_size):
-    w,h=img['img'].size
-    if w==target_size[0] and h==target_size[1]:
-        return img
-
-    ratio_img=w/h
-    if ratio_img > target_size[0]/target_size[1]:
-        new_size = (int(ratio_img*target_size[1]), target_size[1])
-        interp_type = Image.ANTIALIAS if h>target_size[1] else Image.BICUBIC
-    else:
-        new_size = (target_size[0], int(target_size[0]/ratio_img))
-        interp_type = Image.ANTIALIAS if w>target_size[0] else Image.BICUBIC
-    img['img'] = img['img'].resize(new_size, interp_type)
-    if "mask" in img:
-        img['mask'] = cv2.resize(img['mask'], new_size, interpolation=cv2.INTER_CUBIC)
-    if "cond" in img:
-        img['cond'] = img['cond'].resize(new_size, interp_type)
-
-    return DualRandomCrop(target_size[::-1])(img)
-
-def collate_fn_ft(batch):
-    datas, sn_list, sp_list = {'img':[]}, [], []
-
-    data0 = batch[0][0]
-    if 'mask' in data0:
-        datas['mask']=[]
-    if 'cond' in data0:
-        datas['cond']=[]
-
-    for data, target in batch:
-        datas['img'].append(data['img'])
-        datas['mask'].append(data['mask'])
-        if 'cond' in data:
-            datas['cond'].append(data['cond'])
-        if len(target.shape)==2:
-            sn_list.append(target[0])
-            sp_list.append(target[1])
-        else:
-            sp_list.append(target)
-    sn_list += sp_list
-
-    datas['img'] = torch.stack(datas['img'])
-    datas['mask'] = torch.stack(datas['mask']).unsqueeze(1)
-    if 'cond' in data0:
-        datas['cond'] = torch.stack(datas['cond'])
-
-    return datas, torch.stack(sn_list)
-
-def cycle_data(data_loader):
-    epoch=0
-    while True:
-        data_loader.dataset.bucket.rest(epoch)
-        for data in data_loader:
-            yield data
-        epoch+=1
+from PIL import Image
+import torch
+import cv2
+
+from torchvision import transforms as T
+from torchvision.transforms import functional as F
+
+
+class DualRandomCrop(object):
+    def __init__(self, size):
+        self.size = size
+
+    def __call__(self, img):
+        crop_params = T.RandomCrop.get_params(img['img'], self.size)
+        img['img'] = F.crop(img['img'], *crop_params)
+        if "mask" in img:
+            img['mask'] = F.crop(img['mask'], *crop_params)
+        if "cond" in img:
+            img['cond'] = F.crop(img['cond'], *crop_params)
+        return img
+
+def resize_crop_fix(img, target_size):
+    w,h=img['img'].size
+    if w==target_size[0] and h==target_size[1]:
+        return img
+
+    ratio_img=w/h
+    if ratio_img > target_size[0]/target_size[1]:
+        new_size = (int(ratio_img*target_size[1]), target_size[1])
+        interp_type = Image.ANTIALIAS if h>target_size[1] else Image.BICUBIC
+    else:
+        new_size = (target_size[0], int(target_size[0]/ratio_img))
+        interp_type = Image.ANTIALIAS if w>target_size[0] else Image.BICUBIC
+    img['img'] = img['img'].resize(new_size, interp_type)
+    if "mask" in img:
+        img['mask'] = cv2.resize(img['mask'], new_size, interpolation=cv2.INTER_CUBIC)
+    if "cond" in img:
+        img['cond'] = img['cond'].resize(new_size, interp_type)
+
+    return DualRandomCrop(target_size[::-1])(img)
+
+def collate_fn_ft(batch):
+    datas, sn_list, sp_list = {'img':[]}, [], []
+
+    data0 = batch[0]
+    if 'mask' in data0:
+        datas['mask']=[]
+    if 'cond' in data0:
+        datas['cond']=[]
+
+    for data in batch:
+        datas['img'].append(data['img'])
+        datas['mask'].append(data['mask'])
+        if 'cond' in data:
+            datas['cond'].append(data['cond'])
+
+        target = data['prompt']
+        if len(target.shape)==2:
+            sn_list.append(target[0])
+            sp_list.append(target[1])
+        else:
+            sp_list.append(target)
+    sn_list += sp_list
+
+    datas['img'] = torch.stack(datas['img'])
+    datas['mask'] = torch.stack(datas['mask']).unsqueeze(1)
+    if 'cond' in data0:
+        datas['cond'] = torch.stack(datas['cond'])
+    datas['prompt'] = torch.stack(sn_list)
+
+    return datas
+
+class CycleData():
+    def __init__(self, data_loader):
+        print(data_loader)
+        self.data_loader = data_loader
+
+    def __iter__(self):
+        self.epoch = 0
+        def cycle():
+            while True:
+                self.data_loader.dataset.bucket.rest(self.epoch)
+                for data in self.data_loader:
+                    yield data
+                self.epoch+=1
+        return cycle()
```

### Comparing `hcpdiff-0.2.2/hcpdiff/models/cfg_context.py` & `hcpdiff-0.3.0/hcpdiff/models/cfg_context.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-import torch
-from einops import repeat
-import math
-
-class CFGContext:
-    def pre(self, noisy_latents, timesteps):
-        return noisy_latents, timesteps
-
-    def post(self, model_pred):
-        return model_pred
-
-class DreamArtistPTContext(CFGContext):
-    def __init__(self, cfg_scale, num_train_timesteps):
-        self.cfg_scale=cfg_scale
-        self.num_train_timesteps=num_train_timesteps
-
-    def pre(self, noisy_latents, timesteps):
-        self.t_raw = timesteps
-        noisy_latents = repeat(noisy_latents, 'b c h w -> (pn b) c h w', pn=2)
-        timesteps = timesteps.repeat(2)
-        return noisy_latents, timesteps
-
-    def post(self, model_pred):
-        e_t_uncond, e_t = model_pred.chunk(2)
-        if self.cfg_scale[0] != self.cfg_scale[1]:
-            rate = self.t_raw / (self.num_train_timesteps - 1)
-            if self.cfg_scale[2] == 'cos':
-                rate = torch.cos((rate - 1) * math.pi / 2)
-            elif self.cfg_scale[2] == 'cos2':
-                rate = 1 - torch.cos(rate * math.pi / 2)
-            elif self.cfg_scale[2] == 'ln':
-                pass
-            else:
-                rate = eval(self.cfg_scale[2])
-            rate = rate.view(-1,1,1,1)
-        else:
-            rate = 1
-        model_pred = e_t_uncond + ((self.cfg_scale[1] - self.cfg_scale[0]) * rate + self.cfg_scale[0]) * (e_t - e_t_uncond)
+import torch
+from einops import repeat
+import math
+
+class CFGContext:
+    def pre(self, noisy_latents, timesteps):
+        return noisy_latents, timesteps
+
+    def post(self, model_pred):
+        return model_pred
+
+class DreamArtistPTContext(CFGContext):
+    def __init__(self, cfg_scale, num_train_timesteps):
+        self.cfg_scale=cfg_scale
+        self.num_train_timesteps=num_train_timesteps
+
+    def pre(self, noisy_latents, timesteps):
+        self.t_raw = timesteps
+        noisy_latents = repeat(noisy_latents, 'b c h w -> (pn b) c h w', pn=2)
+        timesteps = timesteps.repeat(2)
+        return noisy_latents, timesteps
+
+    def post(self, model_pred):
+        e_t_uncond, e_t = model_pred.chunk(2)
+        if self.cfg_scale[0] != self.cfg_scale[1]:
+            rate = self.t_raw / (self.num_train_timesteps - 1)
+            if self.cfg_scale[2] == 'cos':
+                rate = torch.cos((rate - 1) * math.pi / 2)
+            elif self.cfg_scale[2] == 'cos2':
+                rate = 1 - torch.cos(rate * math.pi / 2)
+            elif self.cfg_scale[2] == 'ln':
+                pass
+            else:
+                rate = eval(self.cfg_scale[2])
+            rate = rate.view(-1,1,1,1)
+        else:
+            rate = 1
+        model_pred = e_t_uncond + ((self.cfg_scale[1] - self.cfg_scale[0]) * rate + self.cfg_scale[0]) * (e_t - e_t_uncond)
         return model_pred
```

### Comparing `hcpdiff-0.2.2/hcpdiff/models/controlnet.py` & `hcpdiff-0.3.0/hcpdiff/models/controlnet.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,187 +1,187 @@
-from typing import List, Tuple, Union, Optional, Dict, Any
-
-from diffusers import UNet2DConditionModel
-import torch
-from torch import nn
-from copy import deepcopy
-
-from .plugin import MultiPluginBlock, BasePluginBlock
-from hcpdiff.utils.net_utils import remove_all_hooks, remove_layers
-
-class ControlNetPlugin(MultiPluginBlock):
-    def __init__(self, name:str, from_layers: List[Dict[str, Any]], to_layers: List[Dict[str, Any]], host_model: UNet2DConditionModel=None,
-                 cond_block_channels=(3, 16, 32, 96, 256, 320),
-                 layers_per_block=2, block_out_channels: Tuple[int] = (320, 640, 1280, 1280)):
-        super().__init__(name, from_layers, to_layers, host_model=host_model)
-
-        self.register_input_feeder_to(host_model)
-
-        self.conv_in = self.copy_block(host_model.conv_in)
-        self.time_proj = self.copy_block(host_model.time_proj)
-        self.time_embedding = self.copy_block(host_model.time_embedding)
-        self.class_embedding = self.copy_block(host_model.class_embedding)
-        self.down_blocks = self.copy_block(host_model.down_blocks)
-        self.mid_block = self.copy_block(host_model.mid_block)
-        self.dtype = host_model.dtype
-
-        self.build_head(cond_block_channels)
-
-        self.controlnet_down_blocks = nn.ModuleList(
-            [nn.Conv2d(block_out_channels[0], block_out_channels[0], kernel_size=1)]+
-            [nn.Conv2d(out_ch, out_ch, kernel_size=1) for out_ch in block_out_channels for _ in range(layers_per_block+1)]
-        )
-        self.controlnet_mid_block = self.controlnet_down_blocks[-1]
-        del self.controlnet_down_blocks[-1]
-
-        self.reset_parameters()
-
-    def copy_block(self, block):
-        if block is None:
-            return block
-        block = deepcopy(block)
-        remove_all_hooks(block)
-        remove_layers(block, BasePluginBlock)
-        return block
-
-    def build_head(self, cond_block_channels):
-        cond_head = [
-            nn.Conv2d(cond_block_channels[0], cond_block_channels[1], kernel_size=3, padding=1),
-            nn.SiLU(),
-        ]
-        for i in range(2, (len(cond_block_channels) - 2) * 2):
-            cond_head.append(nn.Conv2d(cond_block_channels[i // 2], cond_block_channels[(i + 1) // 2], kernel_size=3, padding=1, stride=1 + i % 2))
-            cond_head.append(nn.SiLU())
-        cond_head.append(nn.Conv2d(cond_block_channels[-2], cond_block_channels[-1], kernel_size=3, padding=1))
-        self.cond_head = nn.Sequential(*cond_head)
-
-    def reset_parameters(self) -> None:
-        def weight_init(m):
-            if isinstance(m, nn.Conv2d):
-                nn.init.constant_(m.weight, 0)
-        self.controlnet_down_blocks.apply(weight_init)
-        self.controlnet_mid_block.apply(weight_init)
-        self.cond_head[-1].apply(weight_init)
-
-    def from_layer_hook(self, host, fea_in:Tuple[torch.Tensor], fea_out:Tuple[torch.Tensor], idx: int):
-        if idx==0:
-            self.data_input = fea_in
-        elif idx==1:
-            self.feat_to = self(*self.data_input)
-
-    def to_layer_hook(self, host, fea_in:Tuple[torch.Tensor], fea_out:Tuple[torch.Tensor], idx: int):
-        if idx == 5:
-            sp = fea_in[0].shape[1]//2
-            new_feat = fea_in[0].clone()
-            new_feat[:, sp:, ...] = fea_in[0][:, sp:, ...] + self.feat_to[0]
-            return (new_feat, fea_in[1])
-        elif idx == 3:
-            return (fea_out[0], tuple(fea_out[1][i] + self.feat_to[(idx) * 3 + i+1] for i in range(2)))
-        elif idx == 4:
-            return fea_out + self.feat_to[11+1]
-        else:
-            return (fea_out[0], tuple(fea_out[1][i]+self.feat_to[(idx)*3+i+1] for i in range(3)))
-
-    def feed_input_data(self, data): # get the control image
-        if isinstance(data, dict):
-            self.cond = data['cond']
-
-    def forward(
-            self,
-            sample: torch.FloatTensor,
-            timestep: Union[torch.Tensor, float, int],
-            encoder_hidden_states: torch.Tensor,
-            class_labels: Optional[torch.Tensor] = None,
-            timestep_cond: Optional[torch.Tensor] = None,
-            attention_mask: Optional[torch.Tensor] = None,
-            cross_attention_kwargs: Optional[Dict[str, Any]] = None,
-    ) -> Tuple:
-
-        # prepare attention_mask
-        if attention_mask is not None:
-            attention_mask = (1 - attention_mask.to(sample.dtype)) * -10000.0
-            attention_mask = attention_mask.unsqueeze(1)
-
-        # 1. time
-        timesteps = timestep
-        if not torch.is_tensor(timesteps):
-            # TODO: this requires sync between CPU and GPU. So try to pass timesteps as tensors if you can
-            # This would be a good case for the `match` statement (Python 3.10+)
-            is_mps = sample.device.type == "mps"
-            if isinstance(timestep, float):
-                dtype = torch.float32 if is_mps else torch.float64
-            else:
-                dtype = torch.int32 if is_mps else torch.int64
-            timesteps = torch.tensor([timesteps], dtype=dtype, device=sample.device)
-        elif len(timesteps.shape) == 0:
-            timesteps = timesteps[None].to(sample.device)
-
-        # broadcast to batch dimension in a way that's compatible with ONNX/Core ML
-        timesteps = timesteps.expand(sample.shape[0])
-
-        t_emb = self.time_proj(timesteps)
-
-        # timesteps does not contain any weights and will always return f32 tensors
-        # but time_embedding might actually be running in fp16. so we need to cast here.
-        # there might be better ways to encapsulate this.
-        t_emb = t_emb.to(dtype=self.dtype)
-
-        emb = self.time_embedding(t_emb, timestep_cond)
-
-        if self.class_embedding is not None:
-            if class_labels is None:
-                raise ValueError("class_labels should be provided when num_class_embeds > 0")
-
-            if self.config.class_embed_type == "timestep":
-                class_labels = self.time_proj(class_labels)
-
-            class_emb = self.class_embedding(class_labels).to(dtype=self.dtype)
-            emb = emb + class_emb
-
-        # 2. pre-process
-        sample = self.conv_in(sample)
-
-        controlnet_cond = self.cond_head(self.cond)
-
-        sample += controlnet_cond
-
-        # 3. down
-        down_block_res_samples = (sample,)
-        for downsample_block in self.down_blocks:
-            if hasattr(downsample_block, "has_cross_attention") and downsample_block.has_cross_attention:
-                sample, res_samples = downsample_block(
-                    hidden_states=sample,
-                    temb=emb,
-                    encoder_hidden_states=encoder_hidden_states,
-                    attention_mask=attention_mask,
-                    cross_attention_kwargs=cross_attention_kwargs,
-                )
-            else:
-                sample, res_samples = downsample_block(hidden_states=sample, temb=emb)
-
-            down_block_res_samples += res_samples
-
-        # 4. mid
-        if self.mid_block is not None:
-            sample = self.mid_block(
-                sample,
-                emb,
-                encoder_hidden_states=encoder_hidden_states,
-                attention_mask=attention_mask,
-                cross_attention_kwargs=cross_attention_kwargs,
-            )
-
-        # 5. Control net blocks
-
-        controlnet_down_block_res_samples = ()
-
-        for down_block_res_sample, controlnet_block in zip(down_block_res_samples, self.controlnet_down_blocks):
-            down_block_res_sample = controlnet_block(down_block_res_sample)
-            controlnet_down_block_res_samples += (down_block_res_sample,)
-
-        mid_block_res_sample = self.controlnet_mid_block(sample)
-
-        return controlnet_down_block_res_samples + (mid_block_res_sample,)
-
-
-
-
+from typing import List, Tuple, Union, Optional, Dict, Any
+
+from diffusers import UNet2DConditionModel
+import torch
+from torch import nn
+from copy import deepcopy
+
+from .plugin import MultiPluginBlock, BasePluginBlock
+from hcpdiff.utils.net_utils import remove_all_hooks, remove_layers
+
+class ControlNetPlugin(MultiPluginBlock):
+    def __init__(self, name:str, from_layers: List[Dict[str, Any]], to_layers: List[Dict[str, Any]], host_model: UNet2DConditionModel=None,
+                 cond_block_channels=(3, 16, 32, 96, 256, 320),
+                 layers_per_block=2, block_out_channels: Tuple[int] = (320, 640, 1280, 1280)):
+        super().__init__(name, from_layers, to_layers, host_model=host_model)
+
+        self.register_input_feeder_to(host_model)
+
+        self.conv_in = self.copy_block(host_model.conv_in)
+        self.time_proj = self.copy_block(host_model.time_proj)
+        self.time_embedding = self.copy_block(host_model.time_embedding)
+        self.class_embedding = self.copy_block(host_model.class_embedding)
+        self.down_blocks = self.copy_block(host_model.down_blocks)
+        self.mid_block = self.copy_block(host_model.mid_block)
+        self.dtype = host_model.dtype
+
+        self.build_head(cond_block_channels)
+
+        self.controlnet_down_blocks = nn.ModuleList(
+            [nn.Conv2d(block_out_channels[0], block_out_channels[0], kernel_size=1)]+
+            [nn.Conv2d(out_ch, out_ch, kernel_size=1) for out_ch in block_out_channels for _ in range(layers_per_block+1)]
+        )
+        self.controlnet_mid_block = self.controlnet_down_blocks[-1]
+        del self.controlnet_down_blocks[-1]
+
+        self.reset_parameters()
+
+    def copy_block(self, block):
+        if block is None:
+            return block
+        block = deepcopy(block)
+        remove_all_hooks(block)
+        remove_layers(block, BasePluginBlock)
+        return block
+
+    def build_head(self, cond_block_channels):
+        cond_head = [
+            nn.Conv2d(cond_block_channels[0], cond_block_channels[1], kernel_size=3, padding=1),
+            nn.SiLU(),
+        ]
+        for i in range(2, (len(cond_block_channels) - 2) * 2):
+            cond_head.append(nn.Conv2d(cond_block_channels[i // 2], cond_block_channels[(i + 1) // 2], kernel_size=3, padding=1, stride=1 + i % 2))
+            cond_head.append(nn.SiLU())
+        cond_head.append(nn.Conv2d(cond_block_channels[-2], cond_block_channels[-1], kernel_size=3, padding=1))
+        self.cond_head = nn.Sequential(*cond_head)
+
+    def reset_parameters(self) -> None:
+        def weight_init(m):
+            if isinstance(m, nn.Conv2d):
+                nn.init.constant_(m.weight, 0)
+        self.controlnet_down_blocks.apply(weight_init)
+        self.controlnet_mid_block.apply(weight_init)
+        self.cond_head[-1].apply(weight_init)
+
+    def from_layer_hook(self, host, fea_in:Tuple[torch.Tensor], fea_out:Tuple[torch.Tensor], idx: int):
+        if idx==0:
+            self.data_input = fea_in
+        elif idx==1:
+            self.feat_to = self(*self.data_input)
+
+    def to_layer_hook(self, host, fea_in:Tuple[torch.Tensor], fea_out:Tuple[torch.Tensor], idx: int):
+        if idx == 5:
+            sp = fea_in[0].shape[1]//2
+            new_feat = fea_in[0].clone()
+            new_feat[:, sp:, ...] = fea_in[0][:, sp:, ...] + self.feat_to[0]
+            return (new_feat, fea_in[1])
+        elif idx == 3:
+            return (fea_out[0], tuple(fea_out[1][i] + self.feat_to[(idx) * 3 + i+1] for i in range(2)))
+        elif idx == 4:
+            return fea_out + self.feat_to[11+1]
+        else:
+            return (fea_out[0], tuple(fea_out[1][i]+self.feat_to[(idx)*3+i+1] for i in range(3)))
+
+    def feed_input_data(self, data): # get the control image
+        if isinstance(data, dict):
+            self.cond = data['cond']
+
+    def forward(
+            self,
+            sample: torch.FloatTensor,
+            timestep: Union[torch.Tensor, float, int],
+            encoder_hidden_states: torch.Tensor,
+            class_labels: Optional[torch.Tensor] = None,
+            timestep_cond: Optional[torch.Tensor] = None,
+            attention_mask: Optional[torch.Tensor] = None,
+            cross_attention_kwargs: Optional[Dict[str, Any]] = None,
+    ) -> Tuple:
+
+        # prepare attention_mask
+        if attention_mask is not None:
+            attention_mask = (1 - attention_mask.to(sample.dtype)) * -10000.0
+            attention_mask = attention_mask.unsqueeze(1)
+
+        # 1. time
+        timesteps = timestep
+        if not torch.is_tensor(timesteps):
+            # TODO: this requires sync between CPU and GPU. So try to pass timesteps as tensors if you can
+            # This would be a good case for the `match` statement (Python 3.10+)
+            is_mps = sample.device.type == "mps"
+            if isinstance(timestep, float):
+                dtype = torch.float32 if is_mps else torch.float64
+            else:
+                dtype = torch.int32 if is_mps else torch.int64
+            timesteps = torch.tensor([timesteps], dtype=dtype, device=sample.device)
+        elif len(timesteps.shape) == 0:
+            timesteps = timesteps[None].to(sample.device)
+
+        # broadcast to batch dimension in a way that's compatible with ONNX/Core ML
+        timesteps = timesteps.expand(sample.shape[0])
+
+        t_emb = self.time_proj(timesteps)
+
+        # timesteps does not contain any weights and will always return f32 tensors
+        # but time_embedding might actually be running in fp16. so we need to cast here.
+        # there might be better ways to encapsulate this.
+        t_emb = t_emb.to(dtype=self.dtype)
+
+        emb = self.time_embedding(t_emb, timestep_cond)
+
+        if self.class_embedding is not None:
+            if class_labels is None:
+                raise ValueError("class_labels should be provided when num_class_embeds > 0")
+
+            if self.config.class_embed_type == "timestep":
+                class_labels = self.time_proj(class_labels)
+
+            class_emb = self.class_embedding(class_labels).to(dtype=self.dtype)
+            emb = emb + class_emb
+
+        # 2. pre-process
+        sample = self.conv_in(sample)
+
+        controlnet_cond = self.cond_head(self.cond)
+
+        sample += controlnet_cond
+
+        # 3. down
+        down_block_res_samples = (sample,)
+        for downsample_block in self.down_blocks:
+            if hasattr(downsample_block, "has_cross_attention") and downsample_block.has_cross_attention:
+                sample, res_samples = downsample_block(
+                    hidden_states=sample,
+                    temb=emb,
+                    encoder_hidden_states=encoder_hidden_states,
+                    attention_mask=attention_mask,
+                    cross_attention_kwargs=cross_attention_kwargs,
+                )
+            else:
+                sample, res_samples = downsample_block(hidden_states=sample, temb=emb)
+
+            down_block_res_samples += res_samples
+
+        # 4. mid
+        if self.mid_block is not None:
+            sample = self.mid_block(
+                sample,
+                emb,
+                encoder_hidden_states=encoder_hidden_states,
+                attention_mask=attention_mask,
+                cross_attention_kwargs=cross_attention_kwargs,
+            )
+
+        # 5. Control net blocks
+
+        controlnet_down_block_res_samples = ()
+
+        for down_block_res_sample, controlnet_block in zip(down_block_res_samples, self.controlnet_down_blocks):
+            down_block_res_sample = controlnet_block(down_block_res_sample)
+            controlnet_down_block_res_samples += (down_block_res_sample,)
+
+        mid_block_res_sample = self.controlnet_mid_block(sample)
+
+        return controlnet_down_block_res_samples + (mid_block_res_sample,)
+
+
+
+
```

### Comparing `hcpdiff-0.2.2/hcpdiff/models/layers.py` & `hcpdiff-0.3.0/hcpdiff/models/layers.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,78 +1,78 @@
-"""
-layers.py
-====================
-    :Name:        GroupLinear and other layers
-    :Author:      Dong Ziyi
-    :Affiliation: HCP Lab, SYSU
-    :Created:     09/04/2023
-    :Licence:     Apache-2.0
-"""
-
-import torch
-from torch import nn
-import math
-from einops import rearrange
-
-class GroupLinear(nn.Module):
-    def __init__(self, in_features: int, out_features: int, groups: int, bias: bool = True,
-                 device=None, dtype=None):
-        super().__init__()
-        assert in_features%groups == 0
-        assert out_features%groups == 0
-
-        factory_kwargs = {'device': device, 'dtype': dtype}
-
-        self.groups = groups
-        self.in_features = in_features
-        self.out_features = out_features
-
-        self.weight = nn.Parameter(torch.empty((groups, in_features//groups, out_features//groups), **factory_kwargs))
-        if bias:
-            self.bias = nn.Parameter(torch.empty(groups, 1, out_features//groups, **factory_kwargs))
-        else:
-            self.register_parameter('bias', None)
-        self.reset_parameters()
-
-    def reset_parameters(self) -> None:
-        # Setting a=sqrt(5) in kaiming_uniform is the same as initializing with
-        # uniform(-1/sqrt(in_features), 1/sqrt(in_features)). For details, see
-        # https://github.com/pytorch/pytorch/issues/57109
-        self.kaiming_uniform_group(self.weight, a=math.sqrt(5))
-        if self.bias is not None:
-            fan_in, _ = self._calculate_fan_in_and_fan_out(self.weight)
-            bound = 1 / math.sqrt(fan_in) if fan_in > 0 else 0
-            nn.init.uniform_(self.bias, -bound, bound)
-
-    @staticmethod
-    def _calculate_fan_in_and_fan_out(tensor):
-        receptive_field_size = 1
-        num_input_fmaps = tensor.size(-2)
-        num_output_fmaps = tensor.size(-1)
-        fan_in = num_input_fmaps * receptive_field_size
-        fan_out = num_output_fmaps * receptive_field_size
-
-        return fan_in, fan_out
-
-    @staticmethod
-    def kaiming_uniform_group(tensor: torch.Tensor, a: float = 0, mode: str = 'fan_in', nonlinearity: str = 'leaky_relu') -> torch.Tensor:
-        def _calculate_correct_fan(tensor, mode):
-            mode = mode.lower()
-            valid_modes = ['fan_in', 'fan_out']
-            if mode not in valid_modes:
-                raise ValueError("Mode {} not supported, please use one of {}".format(mode, valid_modes))
-
-            fan_in, fan_out = GroupLinear._calculate_fan_in_and_fan_out(tensor)
-            return fan_in if mode == 'fan_in' else fan_out
-
-        fan = _calculate_correct_fan(tensor, mode)
-        gain = nn.init.calculate_gain(nonlinearity, a)
-        std = gain / math.sqrt(fan)
-        bound = math.sqrt(3.0) * std  # Calculate uniform bounds from standard deviation
-        with torch.no_grad():
-            return tensor.uniform_(-bound, bound)
-
-    def forward(self, x: torch.Tensor): # x: [B,G,L,C]
-        out = x @ self.weight
-        if self.bias is not None:
-            out = out + self.bias
+"""
+layers.py
+====================
+    :Name:        GroupLinear and other layers
+    :Author:      Dong Ziyi
+    :Affiliation: HCP Lab, SYSU
+    :Created:     09/04/2023
+    :Licence:     Apache-2.0
+"""
+
+import torch
+from torch import nn
+import math
+from einops import rearrange
+
+class GroupLinear(nn.Module):
+    def __init__(self, in_features: int, out_features: int, groups: int, bias: bool = True,
+                 device=None, dtype=None):
+        super().__init__()
+        assert in_features%groups == 0
+        assert out_features%groups == 0
+
+        factory_kwargs = {'device': device, 'dtype': dtype}
+
+        self.groups = groups
+        self.in_features = in_features
+        self.out_features = out_features
+
+        self.weight = nn.Parameter(torch.empty((groups, in_features//groups, out_features//groups), **factory_kwargs))
+        if bias:
+            self.bias = nn.Parameter(torch.empty(groups, 1, out_features//groups, **factory_kwargs))
+        else:
+            self.register_parameter('bias', None)
+        self.reset_parameters()
+
+    def reset_parameters(self) -> None:
+        # Setting a=sqrt(5) in kaiming_uniform is the same as initializing with
+        # uniform(-1/sqrt(in_features), 1/sqrt(in_features)). For details, see
+        # https://github.com/pytorch/pytorch/issues/57109
+        self.kaiming_uniform_group(self.weight, a=math.sqrt(5))
+        if self.bias is not None:
+            fan_in, _ = self._calculate_fan_in_and_fan_out(self.weight)
+            bound = 1 / math.sqrt(fan_in) if fan_in > 0 else 0
+            nn.init.uniform_(self.bias, -bound, bound)
+
+    @staticmethod
+    def _calculate_fan_in_and_fan_out(tensor):
+        receptive_field_size = 1
+        num_input_fmaps = tensor.size(-2)
+        num_output_fmaps = tensor.size(-1)
+        fan_in = num_input_fmaps * receptive_field_size
+        fan_out = num_output_fmaps * receptive_field_size
+
+        return fan_in, fan_out
+
+    @staticmethod
+    def kaiming_uniform_group(tensor: torch.Tensor, a: float = 0, mode: str = 'fan_in', nonlinearity: str = 'leaky_relu') -> torch.Tensor:
+        def _calculate_correct_fan(tensor, mode):
+            mode = mode.lower()
+            valid_modes = ['fan_in', 'fan_out']
+            if mode not in valid_modes:
+                raise ValueError("Mode {} not supported, please use one of {}".format(mode, valid_modes))
+
+            fan_in, fan_out = GroupLinear._calculate_fan_in_and_fan_out(tensor)
+            return fan_in if mode == 'fan_in' else fan_out
+
+        fan = _calculate_correct_fan(tensor, mode)
+        gain = nn.init.calculate_gain(nonlinearity, a)
+        std = gain / math.sqrt(fan)
+        bound = math.sqrt(3.0) * std  # Calculate uniform bounds from standard deviation
+        with torch.no_grad():
+            return tensor.uniform_(-bound, bound)
+
+    def forward(self, x: torch.Tensor): # x: [B,G,L,C]
+        out = x @ self.weight
+        if self.bias is not None:
+            out = out + self.bias
         return out
```

### Comparing `hcpdiff-0.2.2/hcpdiff/models/lora_base.py` & `hcpdiff-0.3.0/hcpdiff/models/lora_base.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,170 +1,170 @@
-"""
-lora.py
-====================
-    :Name:        lora tools
-    :Author:      Dong Ziyi
-    :Affiliation: HCP Lab, SYSU
-    :Created:     10/03/2023
-    :Licence:     Apache-2.0
-"""
-
-import torch
-from torch import nn
-
-from hcpdiff.utils.utils import make_mask, low_rank_approximate, isinstance_list
-from .plugin import SinglePluginBlock, PluginGroup, BasePluginBlock
-
-from typing import Union, Tuple, Dict, Type
-
-class LoraBlock(SinglePluginBlock):
-    wrapable_classes = [nn.Linear, nn.Conv2d]
-
-    def __init__(self, lora_id:int, host:Union[nn.Linear, nn.Conv2d], rank, dropout=0.1, scale=1.0, bias=False,
-                 inplace=True, hook_param=None, **kwargs):
-        super().__init__(f'lora_block_{lora_id}', host, hook_param)
-
-        self.mask_range = None
-        self.inplace=inplace
-        self.bias=bias
-
-        if isinstance(host, nn.Linear):
-            self.host_type = 'linear'
-            self.layer = self.LinearLayer(host, rank, bias, dropout, self)
-        elif isinstance(host, nn.Conv2d):
-            self.host_type = 'conv'
-            self.layer = self.Conv2dLayer(host, rank, bias, dropout, self)
-        else:
-            raise NotImplementedError(f'No lora for {type(host)}')
-        self.rank = self.layer.rank
-
-        self.register_buffer('scale', torch.tensor(1.0 if scale == 0 else scale / self.rank))
-
-    def set_mask(self, mask_range):
-        self.mask_range = mask_range
-
-    def init_weights(self, svd_init=False):
-        host = self.host()
-        if svd_init:
-            U, V = low_rank_approximate(host.weight, self.rank)
-            self.feed_svd(U, V, host.weight)
-        else:
-            self.layer.lora_down.reset_parameters()
-            nn.init.zeros_(self.layer.lora_up.weight)
-
-    def forward(self, fea_in:Tuple[torch.Tensor], fea_out:torch.Tensor):
-        if self.mask_range is None:
-            return fea_out + self.layer(fea_in[0]) * self.scale
-        else:
-            # for DreamArtist-lora
-            batch_mask = slice(int(self.mask_range[0]*fea_out.shape[0]), int(self.mask_range[1]*fea_out.shape[0]))
-            if self.inplace:
-                fea_out[batch_mask, ...] = fea_out[batch_mask, ...] + self.layer(fea_in[0][batch_mask, ...]) * self.scale
-                return fea_out
-            else: # colossal-AI dose not support inplace+view
-                new_out = fea_out.clone()
-                new_out[batch_mask, ...] = fea_out[batch_mask, ...] + self.layer(fea_in[0][batch_mask, ...]) * self.scale
-                return new_out
-
-    def collapse_to_host(self, alpha=None, base_alpha=1.0):
-        if alpha is None:
-            alpha = self.scale
-
-        host = self.host()
-        re_w, re_b = self.get_collapsed_param()
-        host.weight = nn.Parameter(
-            host.weight.data * base_alpha + alpha * re_w.to(host.weight.device, dtype=host.weight.dtype)
-        )
-
-        if self.lora_up.bias is not None:
-            if host.bias is None:
-                host.bias = nn.Parameter(re_b.to(host.weight.device, dtype=host.weight.dtype))
-            else:
-                host.bias = nn.Parameter(
-                    host.bias.data * base_alpha + alpha * re_b.to(host.weight.device, dtype=host.weight.dtype))
-
-    class LinearLayer(nn.Module):
-        def __init__(self, host, rank, bias, dropout, block):
-            super().__init__()
-            self.rank=rank
-            if isinstance(self.rank, float):
-                self.rank = max(round(host.out_features * self.rank), 1)
-            self.dropout = nn.Dropout(dropout)
-
-        def feed_svd(self, U, V, weight):
-            self.lora_up.weight.data = U.to(device=weight.device, dtype=weight.dtype)
-            self.lora_down.weight.data = V.to(device=weight.device, dtype=weight.dtype)
-
-        def forward(self, x):
-            return self.dropout(self.lora_up(self.lora_down(x)))
-
-        def get_collapsed_param(self) -> Tuple[torch.Tensor, torch.Tensor]:
-            pass
-
-    class Conv2dLayer(nn.Module):
-        def __init__(self, host, rank, bias, dropout, block):
-            super().__init__()
-            self.rank = rank
-            if isinstance(self.rank, float):
-                self.rank = max(round(host.out_channels * self.rank), 1)
-            self.dropout = nn.Dropout(dropout)
-
-        def feed_svd(self, U, V, weight):
-            self.lora_up.weight.data = U.to(device=weight.device, dtype=weight.dtype)
-            self.lora_down.weight.data = V.to(device=weight.device, dtype=weight.dtype)
-
-        def forward(self, x):
-            return self.dropout(self.lora_up(self.lora_down(x)))
-
-        def get_collapsed_param(self) -> Tuple[torch.Tensor, torch.Tensor]:
-            pass
-
-    @classmethod
-    def wrap_layer(cls, lora_id:int, layer: Union[nn.Linear, nn.Conv2d], rank=1, dropout=0.0, scale=1.0, svd_init=False,
-                   bias=False, mask=None, **kwargs):# -> LoraBlock:
-        lora_block = cls(lora_id, layer, rank, dropout, scale, bias=bias, **kwargs)
-        lora_block.init_weights(svd_init)
-        lora_block.set_mask(mask)
-        return lora_block
-
-    @classmethod
-    def wrap_model(cls, lora_id:int, model: nn.Module, **kwargs):# -> Dict[str, LoraBlock]:
-        return super(LoraBlock, cls).wrap_model(lora_id, model, exclude_key='lora_block_', **kwargs)
-
-    @staticmethod
-    def extract_lora_state(model:nn.Module):
-        return {k:v for k,v in model.state_dict().items() if 'lora_block_' in k}
-
-    @staticmethod
-    def extract_state_without_lora(model:nn.Module):
-        return {k:v for k,v in model.state_dict().items() if 'lora_block_' not in k}
-
-    @staticmethod
-    def extract_param_without_lora(model:nn.Module):
-        return {k:v for k,v in model.named_parameters() if 'lora_block_' not in k}
-
-    @staticmethod
-    def extract_trainable_state_without_lora(model:nn.Module):
-        trainable_keys = {k for k,v in model.named_parameters() if ('lora_block_' not in k) and v.requires_grad}
-        return {k: v for k, v in model.state_dict().items() if k in trainable_keys}
-
-class LoraGroup(PluginGroup):
-    def set_mask(self, batch_mask):
-        for item in self.plugin_dict.values():
-            item.set_mask(batch_mask)
-
-    def collapse_to_host(self, alpha=None, base_alpha=1.0):
-        for item in self.plugin_dict.values():
-            item.collapse_to_host(alpha, base_alpha)
-
-    def set_inplace(self, inplace):
-        for item in self.plugin_dict.values():
-            item.inplace = inplace
-
-def split_state(state_dict):
-    sd_base, sd_lora={}, {}
-    for k, v in state_dict.items():
-        if 'lora_block_' in k:
-            sd_lora[k]=v
-        else:
-            sd_base[k]=v
+"""
+lora.py
+====================
+    :Name:        lora tools
+    :Author:      Dong Ziyi
+    :Affiliation: HCP Lab, SYSU
+    :Created:     10/03/2023
+    :Licence:     Apache-2.0
+"""
+
+import torch
+from torch import nn
+
+from hcpdiff.utils.utils import make_mask, low_rank_approximate, isinstance_list
+from .plugin import SinglePluginBlock, PluginGroup, BasePluginBlock
+
+from typing import Union, Tuple, Dict, Type
+
+class LoraBlock(SinglePluginBlock):
+    wrapable_classes = [nn.Linear, nn.Conv2d]
+
+    def __init__(self, lora_id:int, host:Union[nn.Linear, nn.Conv2d], rank, dropout=0.1, scale=1.0, bias=False,
+                 inplace=True, hook_param=None, alpha_auto_scale=True, **kwargs):
+        super().__init__(f'lora_block_{lora_id}', host, hook_param)
+
+        self.mask_range = None
+        self.inplace=inplace
+        self.bias=bias
+
+        if isinstance(host, nn.Linear):
+            self.host_type = 'linear'
+            self.layer = self.LinearLayer(host, rank, bias, dropout, self)
+        elif isinstance(host, nn.Conv2d):
+            self.host_type = 'conv'
+            self.layer = self.Conv2dLayer(host, rank, bias, dropout, self)
+        else:
+            raise NotImplementedError(f'No lora for {type(host)}')
+        self.rank = self.layer.rank
+
+        self.register_buffer('scale', torch.tensor(scale / self.rank if alpha_auto_scale else scale))
+
+    def set_mask(self, mask_range):
+        self.mask_range = mask_range
+
+    def init_weights(self, svd_init=False):
+        host = self.host()
+        if svd_init:
+            U, V = low_rank_approximate(host.weight, self.rank)
+            self.feed_svd(U, V, host.weight)
+        else:
+            self.layer.lora_down.reset_parameters()
+            nn.init.zeros_(self.layer.lora_up.weight)
+
+    def forward(self, fea_in:Tuple[torch.Tensor], fea_out:torch.Tensor):
+        if self.mask_range is None:
+            return fea_out + self.layer(fea_in[0]) * self.scale
+        else:
+            # for DreamArtist-lora
+            batch_mask = slice(int(self.mask_range[0]*fea_out.shape[0]), int(self.mask_range[1]*fea_out.shape[0]))
+            if self.inplace:
+                fea_out[batch_mask, ...] = fea_out[batch_mask, ...] + self.layer(fea_in[0][batch_mask, ...]) * self.scale
+                return fea_out
+            else: # colossal-AI dose not support inplace+view
+                new_out = fea_out.clone()
+                new_out[batch_mask, ...] = fea_out[batch_mask, ...] + self.layer(fea_in[0][batch_mask, ...]) * self.scale
+                return new_out
+
+    def collapse_to_host(self, alpha=None, base_alpha=1.0):
+        if alpha is None:
+            alpha = self.scale
+
+        host = self.host()
+        re_w, re_b = self.get_collapsed_param()
+        host.weight = nn.Parameter(
+            host.weight.data * base_alpha + alpha * re_w.to(host.weight.device, dtype=host.weight.dtype)
+        )
+
+        if self.lora_up.bias is not None:
+            if host.bias is None:
+                host.bias = nn.Parameter(re_b.to(host.weight.device, dtype=host.weight.dtype))
+            else:
+                host.bias = nn.Parameter(
+                    host.bias.data * base_alpha + alpha * re_b.to(host.weight.device, dtype=host.weight.dtype))
+
+    class LinearLayer(nn.Module):
+        def __init__(self, host, rank, bias, dropout, block):
+            super().__init__()
+            self.rank=rank
+            if isinstance(self.rank, float):
+                self.rank = max(round(host.out_features * self.rank), 1)
+            self.dropout = nn.Dropout(dropout)
+
+        def feed_svd(self, U, V, weight):
+            self.lora_up.weight.data = U.to(device=weight.device, dtype=weight.dtype)
+            self.lora_down.weight.data = V.to(device=weight.device, dtype=weight.dtype)
+
+        def forward(self, x):
+            return self.dropout(self.lora_up(self.lora_down(x)))
+
+        def get_collapsed_param(self) -> Tuple[torch.Tensor, torch.Tensor]:
+            pass
+
+    class Conv2dLayer(nn.Module):
+        def __init__(self, host, rank, bias, dropout, block):
+            super().__init__()
+            self.rank = rank
+            if isinstance(self.rank, float):
+                self.rank = max(round(host.out_channels * self.rank), 1)
+            self.dropout = nn.Dropout(dropout)
+
+        def feed_svd(self, U, V, weight):
+            self.lora_up.weight.data = U.to(device=weight.device, dtype=weight.dtype)
+            self.lora_down.weight.data = V.to(device=weight.device, dtype=weight.dtype)
+
+        def forward(self, x):
+            return self.dropout(self.lora_up(self.lora_down(x)))
+
+        def get_collapsed_param(self) -> Tuple[torch.Tensor, torch.Tensor]:
+            pass
+
+    @classmethod
+    def wrap_layer(cls, lora_id:int, layer: Union[nn.Linear, nn.Conv2d], rank=1, dropout=0.0, scale=1.0, svd_init=False,
+                   bias=False, mask=None, **kwargs):# -> LoraBlock:
+        lora_block = cls(lora_id, layer, rank, dropout, scale, bias=bias, **kwargs)
+        lora_block.init_weights(svd_init)
+        lora_block.set_mask(mask)
+        return lora_block
+
+    @classmethod
+    def wrap_model(cls, lora_id:int, model: nn.Module, **kwargs):# -> Dict[str, LoraBlock]:
+        return super(LoraBlock, cls).wrap_model(lora_id, model, exclude_key='lora_block_', **kwargs)
+
+    @staticmethod
+    def extract_lora_state(model:nn.Module):
+        return {k:v for k,v in model.state_dict().items() if 'lora_block_' in k}
+
+    @staticmethod
+    def extract_state_without_lora(model:nn.Module):
+        return {k:v for k,v in model.state_dict().items() if 'lora_block_' not in k}
+
+    @staticmethod
+    def extract_param_without_lora(model:nn.Module):
+        return {k:v for k,v in model.named_parameters() if 'lora_block_' not in k}
+
+    @staticmethod
+    def extract_trainable_state_without_lora(model:nn.Module):
+        trainable_keys = {k for k,v in model.named_parameters() if ('lora_block_' not in k) and v.requires_grad}
+        return {k: v for k, v in model.state_dict().items() if k in trainable_keys}
+
+class LoraGroup(PluginGroup):
+    def set_mask(self, batch_mask):
+        for item in self.plugin_dict.values():
+            item.set_mask(batch_mask)
+
+    def collapse_to_host(self, alpha=None, base_alpha=1.0):
+        for item in self.plugin_dict.values():
+            item.collapse_to_host(alpha, base_alpha)
+
+    def set_inplace(self, inplace):
+        for item in self.plugin_dict.values():
+            item.inplace = inplace
+
+def split_state(state_dict):
+    sd_base, sd_lora={}, {}
+    for k, v in state_dict.items():
+        if 'lora_block_' in k:
+            sd_lora[k]=v
+        else:
+            sd_base[k]=v
     return sd_base, sd_lora
```

### Comparing `hcpdiff-0.2.2/hcpdiff/models/lora_layers.py` & `hcpdiff-0.3.0/hcpdiff/models/lora_layers.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,143 +1,143 @@
-"""
-lora_layers.py
-====================
-    :Name:        lora layers
-    :Author:      Dong Ziyi
-    :Affiliation: HCP Lab, SYSU
-    :Created:     09/04/2023
-    :Licence:     Apache-2.0
-"""
-
-from typing import Union
-
-import torch
-from einops import repeat, rearrange, einsum
-from torch import nn
-
-from .lora_base import LoraBlock
-from .layers import GroupLinear
-
-class LoraLayer(LoraBlock):
-    def __init__(self, lora_id:int, host, rank=1, dropout=0.1, scale=1.0, bias=False, inplace=True, **kwargs):
-        super().__init__(lora_id, host, rank, dropout, scale, bias, inplace)
-
-    class LinearLayer(LoraBlock.LinearLayer):
-        def __init__(self, host, rank, bias, dropout, block):
-            super().__init__(host, rank, bias, dropout, block)
-            self.lora_down = nn.Linear(host.in_features, self.rank, bias=False)
-            self.lora_up = nn.Linear(self.rank, host.out_features, bias=bias)
-
-        def get_collapsed_param(self):
-            w = self.lora_up.weight.data @ self.lora_down.weight.data
-            b = self.lora_up.bias.data if self.bias else None
-            return w, b
-
-    class Conv2dLayer(LoraBlock.Conv2dLayer):
-        def __init__(self, host, rank, bias, dropout, block):
-            super().__init__(host, rank, bias, dropout, block)
-            self.lora_down = nn.Conv2d(host.in_channels, self.rank, kernel_size=host.kernel_size, stride=host.stride,
-                                       padding=host.padding, dilation=host.dilation, groups=host.groups, bias=False)
-            self.lora_up = nn.Conv2d(self.rank, host.out_channels, kernel_size=1, stride=1, padding=0,
-                                     groups=host.groups, bias=bias)
-
-        def get_collapsed_param(self):
-            w = einsum(self.lora_up.weight.data, self.lora_down.weight.data, 'o r ..., r i ... -> o i ...')
-            b = self.lora_up.bias.data if self.bias else None
-            return w, b
-
-class LoraLayerGroup(LoraBlock):
-    def __init__(self, lora_id:int, host, rank=1, dropout=0.1, scale=1.0, bias=False, inplace=True, rank_groups=1, **kwargs):
-        self.rank_groups_raw = rank_groups
-        super().__init__(lora_id, host, rank, dropout, scale, bias, inplace)
-
-    def collapse_to_host(self, alpha=None, base_alpha=1.0):
-        raise NotImplementedError('LoraLayerGroup not support reparameterization.')
-
-    class LinearLayer(LoraBlock.LinearLayer):
-        def __init__(self, host, rank, bias, dropout, block):
-            super().__init__(host, rank, bias, dropout, block)
-            self.register_buffer('rank_groups', torch.tensor(block.rank_groups_raw, dtype=torch.int))
-            self.lora_down = GroupLinear(host.in_features*self.rank_groups, self.rank, groups=self.rank_groups, bias=False)
-            self.lora_up = GroupLinear(self.rank, host.out_features*self.rank_groups, groups=self.rank_groups, bias=bias)
-
-        def feed_svd(self, U, V, weight):
-            self.lora_up.weight.data = rearrange(U, 'o (g ri) -> g ri o', g=self.rank_groups).to(device=weight.device, dtype=weight.dtype)
-            self.lora_down.weight.data = rearrange(V, '(g ri) i -> g i ri', g=self.rank_groups).to(device=weight.device, dtype=weight.dtype)
-
-        def forward(self, x):
-            x = repeat(x, 'b l c -> b l (g c)', g=self.rank_groups)
-            x = rearrange(x, 'b l (g c) -> b g l c', g=self.rank_groups)
-            x = self.dropout(self.lora_up(self.lora_down(x)))
-            x = torch.prod(x, dim=1, dtype=torch.float16)**(1/self.rank_groups).to(dtype=x.dtype)
-            return x
-
-    class Conv2dLayer(LoraBlock.Conv2dLayer):
-        def __init__(self, host, rank, bias, dropout, block):
-            super().__init__(host, rank, bias, dropout, block)
-            self.register_buffer('rank_groups', torch.tensor(block.rank_groups_raw))
-            self.lora_down = nn.Conv2d(host.in_channels * self.rank_groups, self.rank, kernel_size=host.kernel_size, stride=host.stride,
-                                       padding=host.padding, dilation=host.dilation, groups=self.rank_groups, bias=False)
-            self.lora_up = nn.Conv2d(self.rank, host.out_channels * self.rank_groups, kernel_size=1, stride=1,
-                                     padding=0, groups=self.rank_groups, bias=bias)
-
-        def feed_svd(self, U, V, weight):
-            self.lora_up.weight.data = rearrange(U, 'o (g ri) ... -> (g o) ri ...', g=self.rank_groups).to(device=weight.device, dtype=weight.dtype)
-            self.lora_down.weight.data = rearrange(V, '(g ri) i ... -> g i ri ...', g=self.rank_groups).to(device=weight.device, dtype=weight.dtype)
-
-        def forward(self, x):
-            x = self.dropout(self.lora_up(self.lora_down(x)))
-            x = torch.prod(rearrange(x, 'b (g c) h w -> b g c h w'), dim=1, dtype=torch.float16) ** (1 / self.rank_groups).to(dtype=x.dtype)
-            return x
-
-class LohaLayer(LoraBlock):
-    def __init__(self, lora_id:int, host, rank=1, dropout=0.1, scale=1.0, bias=False, inplace=True, rank_groups=2, **kwargs):
-        self.rank_groups_raw = rank_groups
-        super().__init__(lora_id, host, rank, dropout, scale, bias, inplace, hook_param='weight')
-
-    def forward(self, host_param: nn.Parameter):
-        return host_param + self.layer(host_param) * self.scale
-
-    class LinearLayer(LoraBlock.LinearLayer):
-        def __init__(self, host, rank, bias, dropout, block):
-            super().__init__(host, rank, bias, dropout, block)
-            self.register_buffer('rank_groups', torch.tensor(block.rank_groups_raw))
-            self.W_down = nn.Parameter(torch.empty((block.rank_groups_raw, self.rank//block.rank_groups_raw, host.in_features)))
-            self.W_up = nn.Parameter(torch.empty((block.rank_groups_raw, host.out_features, self.rank//block.rank_groups_raw)))
-
-        def forward(self, x):
-            return torch.prod(self.W_up @ self.W_down, dim=0)
-
-        def feed_svd(self, U, V, weight):
-            self.W_up.data = rearrange(U, 'o (g ri) -> g ri o', g=self.rank_groups).to(device=weight.device, dtype=weight.dtype)
-            self.W_down.data = rearrange(V, '(g ri) i -> g i ri', g=self.rank_groups).to(device=weight.device, dtype=weight.dtype)
-
-        def get_collapsed_param(self):
-            w = torch.prod(self.W_up.data @ self.W_down.data, dim=0)
-            b = None
-            return w, b
-
-    class Conv2dLayer(LoraBlock.Conv2dLayer):
-        def __init__(self, host, rank, bias, dropout, block):
-            super().__init__(host, rank, bias, dropout, block)
-            self.W_down = nn.Parameter( torch.empty((block.rank_groups_raw, self.rank // block.rank_groups_raw,
-                                                     host.in_features, *host.kernel_size)))
-            self.W_up = nn.Parameter(torch.empty((block.rank_groups_raw, host.out_features,
-                                                    self.rank//block.rank_groups_raw, *([1]*len(host.kernel_size)))))
-
-        def forward(self, x):
-            return torch.prod(einsum(self.W_up, self.W_down, 'g o r ..., g r i ... -> g o i ...'), dim=0)
-
-        def feed_svd(self, U, V, weight):
-            self.W_up.data = rearrange(U, 'o (g ri) ... -> (g o) ri ...', g=self.rank_groups).to(device=weight.device, dtype=weight.dtype)
-            self.W_down.data = rearrange(V, '(g ri) i ... -> g i ri ...', g=self.rank_groups).to(device=weight.device, dtype=weight.dtype)
-
-        def get_collapsed_param(self):
-            w = torch.prod(einsum(self.W_up.data, self.W_down.data, 'g o r ..., g r i ... -> g o i ...'), dim=0)
-            b = None
-            return w, b
-
-layer_map={
-    'lora': LoraLayer,
-    'loha_group': LoraLayerGroup,
-    'loha': LohaLayer,
-}
+"""
+lora_layers.py
+====================
+    :Name:        lora layers
+    :Author:      Dong Ziyi
+    :Affiliation: HCP Lab, SYSU
+    :Created:     09/04/2023
+    :Licence:     Apache-2.0
+"""
+
+from typing import Union
+
+import torch
+from einops import repeat, rearrange, einsum
+from torch import nn
+
+from .lora_base import LoraBlock
+from .layers import GroupLinear
+
+class LoraLayer(LoraBlock):
+    def __init__(self, lora_id:int, host, rank=1, dropout=0.1, scale=1.0, bias=False, inplace=True, alpha_auto_scale=True, **kwargs):
+        super().__init__(lora_id, host, rank, dropout, scale, bias, inplace, alpha_auto_scale=alpha_auto_scale)
+
+    class LinearLayer(LoraBlock.LinearLayer):
+        def __init__(self, host, rank, bias, dropout, block):
+            super().__init__(host, rank, bias, dropout, block)
+            self.lora_down = nn.Linear(host.in_features, self.rank, bias=False)
+            self.lora_up = nn.Linear(self.rank, host.out_features, bias=bias)
+
+        def get_collapsed_param(self):
+            w = self.lora_up.weight.data @ self.lora_down.weight.data
+            b = self.lora_up.bias.data if self.bias else None
+            return w, b
+
+    class Conv2dLayer(LoraBlock.Conv2dLayer):
+        def __init__(self, host, rank, bias, dropout, block):
+            super().__init__(host, rank, bias, dropout, block)
+            self.lora_down = nn.Conv2d(host.in_channels, self.rank, kernel_size=host.kernel_size, stride=host.stride,
+                                       padding=host.padding, dilation=host.dilation, groups=host.groups, bias=False)
+            self.lora_up = nn.Conv2d(self.rank, host.out_channels, kernel_size=1, stride=1, padding=0,
+                                     groups=host.groups, bias=bias)
+
+        def get_collapsed_param(self):
+            w = einsum(self.lora_up.weight.data, self.lora_down.weight.data, 'o r ..., r i ... -> o i ...')
+            b = self.lora_up.bias.data if self.bias else None
+            return w, b
+
+class LoraLayerGroup(LoraBlock):
+    def __init__(self, lora_id:int, host, rank=1, dropout=0.1, scale=1.0, bias=False, inplace=True, rank_groups=1, alpha_auto_scale=True, **kwargs):
+        self.rank_groups_raw = rank_groups
+        super().__init__(lora_id, host, rank, dropout, scale, bias, inplace, alpha_auto_scale=alpha_auto_scale)
+
+    def collapse_to_host(self, alpha=None, base_alpha=1.0):
+        raise NotImplementedError('LoraLayerGroup not support reparameterization.')
+
+    class LinearLayer(LoraBlock.LinearLayer):
+        def __init__(self, host, rank, bias, dropout, block):
+            super().__init__(host, rank, bias, dropout, block)
+            self.register_buffer('rank_groups', torch.tensor(block.rank_groups_raw, dtype=torch.int))
+            self.lora_down = GroupLinear(host.in_features*self.rank_groups, self.rank, groups=self.rank_groups, bias=False)
+            self.lora_up = GroupLinear(self.rank, host.out_features*self.rank_groups, groups=self.rank_groups, bias=bias)
+
+        def feed_svd(self, U, V, weight):
+            self.lora_up.weight.data = rearrange(U, 'o (g ri) -> g ri o', g=self.rank_groups).to(device=weight.device, dtype=weight.dtype)
+            self.lora_down.weight.data = rearrange(V, '(g ri) i -> g i ri', g=self.rank_groups).to(device=weight.device, dtype=weight.dtype)
+
+        def forward(self, x):
+            x = repeat(x, 'b l c -> b l (g c)', g=self.rank_groups)
+            x = rearrange(x, 'b l (g c) -> b g l c', g=self.rank_groups)
+            x = self.dropout(self.lora_up(self.lora_down(x)))
+            x = torch.prod(x, dim=1, dtype=torch.float16)**(1/self.rank_groups).to(dtype=x.dtype)
+            return x
+
+    class Conv2dLayer(LoraBlock.Conv2dLayer):
+        def __init__(self, host, rank, bias, dropout, block):
+            super().__init__(host, rank, bias, dropout, block)
+            self.register_buffer('rank_groups', torch.tensor(block.rank_groups_raw))
+            self.lora_down = nn.Conv2d(host.in_channels * self.rank_groups, self.rank, kernel_size=host.kernel_size, stride=host.stride,
+                                       padding=host.padding, dilation=host.dilation, groups=self.rank_groups, bias=False)
+            self.lora_up = nn.Conv2d(self.rank, host.out_channels * self.rank_groups, kernel_size=1, stride=1,
+                                     padding=0, groups=self.rank_groups, bias=bias)
+
+        def feed_svd(self, U, V, weight):
+            self.lora_up.weight.data = rearrange(U, 'o (g ri) ... -> (g o) ri ...', g=self.rank_groups).to(device=weight.device, dtype=weight.dtype)
+            self.lora_down.weight.data = rearrange(V, '(g ri) i ... -> g i ri ...', g=self.rank_groups).to(device=weight.device, dtype=weight.dtype)
+
+        def forward(self, x):
+            x = self.dropout(self.lora_up(self.lora_down(x)))
+            x = torch.prod(rearrange(x, 'b (g c) h w -> b g c h w'), dim=1, dtype=torch.float16) ** (1 / self.rank_groups).to(dtype=x.dtype)
+            return x
+
+class LohaLayer(LoraBlock):
+    def __init__(self, lora_id:int, host, rank=1, dropout=0.1, scale=1.0, bias=False, inplace=True, rank_groups=2, alpha_auto_scale=True, **kwargs):
+        self.rank_groups_raw = rank_groups
+        super().__init__(lora_id, host, rank, dropout, scale, bias, inplace, hook_param='weight', alpha_auto_scale=alpha_auto_scale)
+
+    def forward(self, host_param: nn.Parameter):
+        return host_param + self.layer(host_param) * self.scale
+
+    class LinearLayer(LoraBlock.LinearLayer):
+        def __init__(self, host, rank, bias, dropout, block):
+            super().__init__(host, rank, bias, dropout, block)
+            self.register_buffer('rank_groups', torch.tensor(block.rank_groups_raw))
+            self.W_down = nn.Parameter(torch.empty((block.rank_groups_raw, self.rank//block.rank_groups_raw, host.in_features)))
+            self.W_up = nn.Parameter(torch.empty((block.rank_groups_raw, host.out_features, self.rank//block.rank_groups_raw)))
+
+        def forward(self, x):
+            return torch.prod(self.W_up @ self.W_down, dim=0)
+
+        def feed_svd(self, U, V, weight):
+            self.W_up.data = rearrange(U, 'o (g ri) -> g ri o', g=self.rank_groups).to(device=weight.device, dtype=weight.dtype)
+            self.W_down.data = rearrange(V, '(g ri) i -> g i ri', g=self.rank_groups).to(device=weight.device, dtype=weight.dtype)
+
+        def get_collapsed_param(self):
+            w = torch.prod(self.W_up.data @ self.W_down.data, dim=0)
+            b = None
+            return w, b
+
+    class Conv2dLayer(LoraBlock.Conv2dLayer):
+        def __init__(self, host, rank, bias, dropout, block):
+            super().__init__(host, rank, bias, dropout, block)
+            self.W_down = nn.Parameter( torch.empty((block.rank_groups_raw, self.rank // block.rank_groups_raw,
+                                                     host.in_features, *host.kernel_size)))
+            self.W_up = nn.Parameter(torch.empty((block.rank_groups_raw, host.out_features,
+                                                    self.rank//block.rank_groups_raw, *([1]*len(host.kernel_size)))))
+
+        def forward(self, x):
+            return torch.prod(einsum(self.W_up, self.W_down, 'g o r ..., g r i ... -> g o i ...'), dim=0)
+
+        def feed_svd(self, U, V, weight):
+            self.W_up.data = rearrange(U, 'o (g ri) ... -> (g o) ri ...', g=self.rank_groups).to(device=weight.device, dtype=weight.dtype)
+            self.W_down.data = rearrange(V, '(g ri) i ... -> g i ri ...', g=self.rank_groups).to(device=weight.device, dtype=weight.dtype)
+
+        def get_collapsed_param(self):
+            w = torch.prod(einsum(self.W_up.data, self.W_down.data, 'g o r ..., g r i ... -> g o i ...'), dim=0)
+            b = None
+            return w, b
+
+layer_map={
+    'lora': LoraLayer,
+    'loha_group': LoraLayerGroup,
+    'loha': LohaLayer,
+}
```

### Comparing `hcpdiff-0.2.2/hcpdiff/models/plugin.py` & `hcpdiff-0.3.0/hcpdiff/models/plugin.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,219 +1,219 @@
-"""
-plugin.py
-====================
-    :Name:        model plugin
-    :Author:      Dong Ziyi
-    :Affiliation: HCP Lab, SYSU
-    :Created:     10/03/2023
-    :Licence:     Apache-2.0
-"""
-
-from typing import Tuple, List, Dict, Any
-
-import torch
-from torch import nn
-import weakref
-
-from hcpdiff.utils.utils import isinstance_list
-
-class BasePluginBlock(nn.Module):
-    def __init__(self, name: str):
-        super().__init__()
-        self.name = name
-
-    def forward(self, host:nn.Module, fea_in:Tuple[torch.Tensor], fea_out:torch.Tensor):
-        return fea_out
-
-    def remove(self):
-        pass
-
-    def feed_input_data(self, data):
-        self.input_data = data
-
-    def register_input_feeder_to(self, host_model):
-        if not hasattr(host_model, 'input_feeder'):
-            host_model.input_feeder = []
-        host_model.input_feeder.append(self.feed_input_data)
-
-    def set_hyper_params(self, **kwargs):
-        for k,v in kwargs.items():
-            setattr(self, k, v)
-
-    @staticmethod
-    def extract_state_without_plugin(model: nn.Module, trainable=False):
-        plugin_names = {k for k,v in model.named_modules() if isinstance(v, BasePluginBlock)}
-        model_sd = {}
-        for k, v in model.state_dict().items():
-            if (not trainable) or v.requires_grad:
-                for name in plugin_names:
-                    if k.startswith(name):
-                        break
-                else:
-                    model_sd[k]=v
-        return model_sd
-
-class SinglePluginBlock(BasePluginBlock):
-    wrapable_classes=[]
-
-    def __init__(self, name:str, host:nn.Module, hook_param=None, host_model=None):
-        super().__init__(name)
-        self.host = weakref.ref(host)
-        setattr(host, name, self)
-
-        if hook_param is None:
-            self.hook_handle = host.register_forward_hook(self.layer_hook)
-        else: # hook for model parameters
-            self.backup = getattr(host, hook_param)
-            self.target = hook_param
-            self.handle_pre = host.register_forward_pre_hook(self.pre_hook)
-            self.handle_post = host.register_forward_hook(self.post_hook)
-
-    def layer_hook(self, host, fea_in:Tuple[torch.Tensor], fea_out:torch.Tensor):
-        return self(fea_in, fea_out)
-
-    def pre_hook(self, host, fea_in:torch.Tensor):
-        host.weight_restored = False
-        host_param = getattr(host, self.target)
-        delattr(host, self.target)
-        setattr(host, self.target, self(host_param))
-        return fea_in
-
-    def post_hook(self, host, fea_int, fea_out):
-        if not getattr(host, 'weight_restored', False):
-            setattr(host, self.target, self.backup)
-            host.weight_restored = True
-
-    def remove(self):
-        host = self.host()
-        delattr(host, self.name)
-        if hasattr(self, 'hook_handle'):
-            self.hook_handle.remove()
-        else:
-            self.handle_pre.remove()
-            self.handle_post.remove()
-
-    @classmethod
-    def wrap_layer(cls, name: str, layer: nn.Module, **kwargs):  # -> SinglePluginBlock:
-        raise NotImplementedError(f'wrap_layer of {cls} is not implemented.')
-
-    @classmethod
-    def wrap_model(cls, plugin_name: str, model: nn.Module, exclude_key=None, **kwargs):  # -> Dict[str, SinglePluginBlock]:
-        plugin_block_dict = {}
-        if isinstance_list(model, cls.wrapable_classes):
-            plugin_block_dict[''] = cls.wrap_layer(plugin_name, model, **kwargs)
-        else:
-            if exclude_key:
-                # there maybe multiple single plugin block, avoid insert plugin into plugin blocks with exclude_key
-                named_modules = {name: layer for name, layer in model.named_modules() if exclude_key not in name}
-            else:
-                named_modules = {name: layer for name, layer in model.named_modules()}
-            for name, layer in named_modules.items():
-                if isinstance_list(layer, cls.wrapable_classes):
-                    plugin_block_dict[name] = cls.wrap_layer(plugin_name, layer, **kwargs)
-        return plugin_block_dict
-
-class PluginBlock(BasePluginBlock):
-    def __init__(self, name, from_layer:Dict[str, Any], to_layer:Dict[str, Any], host_model=None):
-        super().__init__(name)
-        self.host_from = weakref.ref(from_layer['layer'])
-        self.host_to = weakref.ref(to_layer['layer'])
-        setattr(from_layer['layer'], name, self)
-
-        if from_layer['pre_hook']:
-            self.hook_handle_from = from_layer['layer'].register_forward_pre_hook(lambda host, fea_in: self.from_layer_hook(host, fea_in, None))
-        else:
-            self.hook_handle_from = from_layer['layer'].register_forward_hook(lambda host, fea_in, fea_out: self.from_layer_hook(host, fea_in, fea_out))
-        if to_layer['pre_hook']:
-            self.hook_handle_to = to_layer['layer'].register_forward_pre_hook(lambda host, fea_in: self.to_layer_hook(host, fea_in, None))
-        else:
-            self.hook_handle_to = to_layer['layer'].register_forward_hook(lambda host, fea_in, fea_out: self.to_layer_hook(host, fea_in, fea_out))
-
-    def from_layer_hook(self, host, fea_in:Tuple[torch.Tensor], fea_out:torch.Tensor):
-        self.feat_from = fea_in
-
-    def to_layer_hook(self, host, fea_in:Tuple[torch.Tensor], fea_out:torch.Tensor):
-        return self(self.feat_from, fea_in, fea_out)
-
-    def remove(self):
-        host_from = self.host_from()
-        delattr(host_from, self.name)
-        self.hook_handle_from.remove()
-        self.hook_handle_to.remove()
-
-class MultiPluginBlock(BasePluginBlock):
-    def __init__(self, name:str, from_layers:List[Dict[str, Any]], to_layers:List[Dict[str, Any]], host_model=None):
-        super().__init__(name)
-        assert host_model is not None
-        self.host_from = [weakref.ref(x['layer']) for x in from_layers]
-        self.host_to = [weakref.ref(x['layer']) for x in to_layers]
-        self.host_model = weakref.ref(host_model)
-        setattr(host_model, name, self)
-
-        self.feat_from=[None for _ in range(len(from_layers))]
-
-        self.hook_handle_from = []
-        self.hook_handle_to = []
-
-        for idx, layer in enumerate(from_layers):
-            if layer['pre_hook']:
-                handle_from = layer['layer'].register_forward_pre_hook(lambda host, fea_in, idx=idx:self.from_layer_hook(host, fea_in, None, idx))
-            else:
-                handle_from = layer['layer'].register_forward_hook(lambda host, fea_in, fea_out, idx=idx: self.from_layer_hook(host, fea_in, fea_out, idx))
-            self.hook_handle_from.append(handle_from)
-        for idx, layer in enumerate(to_layers):
-            if layer['pre_hook']:
-                handle_to = layer['layer'].register_forward_pre_hook(lambda host, fea_in, idx=idx:self.to_layer_hook(host, fea_in, None, idx))
-            else:
-                handle_to = layer['layer'].register_forward_hook(lambda host, fea_in, fea_out, idx=idx:self.to_layer_hook(host, fea_in, fea_out, idx))
-            self.hook_handle_to.append(handle_to)
-
-        self.record_count=0
-
-    def from_layer_hook(self, host, fea_in:Tuple[torch.Tensor], fea_out:Tuple[torch.Tensor], idx: int):
-        self.feat_from[idx] = fea_in
-        self.record_count+=1
-        if self.record_count==len(self.feat_from): # call forward when all feat is record
-            self.record_count = 0
-            self.feat_to = self(self.feat_from)
-
-    def to_layer_hook(self, host, fea_in:Tuple[torch.Tensor], fea_out:Tuple[torch.Tensor], idx: int):
-        return self.feat_to[idx] + fea_out
-
-    def remove(self):
-        host_model = self.host_model()
-        delattr(host_model, self.name)
-        for handle_from in self.hook_handle_from:
-            handle_from.remove()
-        for handle_to in self.hook_handle_to:
-            handle_to.remove()
-
-class PluginGroup:
-    def __init__(self, plugin_dict:Dict[str, BasePluginBlock]):
-        self.plugin_dict = plugin_dict # {host_model_path: plugin_object}
-
-    def __setitem__(self, k, v):
-        self.plugin_dict[k]=v
-
-    def __getitem__(self, k):
-        return self.plugin_dict[k]
-
-    @property
-    def plugin_name(self):
-        if self.empty():
-            return None
-        return next(iter(self.plugin_dict.values())).name
-
-    def remove(self):
-        for plugin in self.plugin_dict.values():
-            plugin.remove()
-
-    def state_dict(self, model=None):
-        if model is None:
-            return {f'{k}.___.{ks}':vs for k,v in self.plugin_dict.items() for ks,vs in v.state_dict().items()}
-        else:
-            sd_model = model.state_dict()
-            return {f'{k}.___.{ks}':sd_model[f'{k}.{v.name}.{ks}'] for k,v in self.plugin_dict.items() for ks,vs in v.state_dict().items()}
-
-    def empty(self):
-        return len(self.plugin_dict)==0
-
+"""
+plugin.py
+====================
+    :Name:        model plugin
+    :Author:      Dong Ziyi
+    :Affiliation: HCP Lab, SYSU
+    :Created:     10/03/2023
+    :Licence:     Apache-2.0
+"""
+
+from typing import Tuple, List, Dict, Any
+
+import torch
+from torch import nn
+import weakref
+
+from hcpdiff.utils.utils import isinstance_list
+
+class BasePluginBlock(nn.Module):
+    def __init__(self, name: str):
+        super().__init__()
+        self.name = name
+
+    def forward(self, host:nn.Module, fea_in:Tuple[torch.Tensor], fea_out:torch.Tensor):
+        return fea_out
+
+    def remove(self):
+        pass
+
+    def feed_input_data(self, data):
+        self.input_data = data
+
+    def register_input_feeder_to(self, host_model):
+        if not hasattr(host_model, 'input_feeder'):
+            host_model.input_feeder = []
+        host_model.input_feeder.append(self.feed_input_data)
+
+    def set_hyper_params(self, **kwargs):
+        for k,v in kwargs.items():
+            setattr(self, k, v)
+
+    @staticmethod
+    def extract_state_without_plugin(model: nn.Module, trainable=False):
+        plugin_names = {k for k,v in model.named_modules() if isinstance(v, BasePluginBlock)}
+        model_sd = {}
+        for k, v in model.state_dict().items():
+            if (not trainable) or v.requires_grad:
+                for name in plugin_names:
+                    if k.startswith(name):
+                        break
+                else:
+                    model_sd[k]=v
+        return model_sd
+
+class SinglePluginBlock(BasePluginBlock):
+    wrapable_classes=[]
+
+    def __init__(self, name:str, host:nn.Module, hook_param=None, host_model=None):
+        super().__init__(name)
+        self.host = weakref.ref(host)
+        setattr(host, name, self)
+
+        if hook_param is None:
+            self.hook_handle = host.register_forward_hook(self.layer_hook)
+        else: # hook for model parameters
+            self.backup = getattr(host, hook_param)
+            self.target = hook_param
+            self.handle_pre = host.register_forward_pre_hook(self.pre_hook)
+            self.handle_post = host.register_forward_hook(self.post_hook)
+
+    def layer_hook(self, host, fea_in:Tuple[torch.Tensor], fea_out:torch.Tensor):
+        return self(fea_in, fea_out)
+
+    def pre_hook(self, host, fea_in:torch.Tensor):
+        host.weight_restored = False
+        host_param = getattr(host, self.target)
+        delattr(host, self.target)
+        setattr(host, self.target, self(host_param))
+        return fea_in
+
+    def post_hook(self, host, fea_int, fea_out):
+        if not getattr(host, 'weight_restored', False):
+            setattr(host, self.target, self.backup)
+            host.weight_restored = True
+
+    def remove(self):
+        host = self.host()
+        delattr(host, self.name)
+        if hasattr(self, 'hook_handle'):
+            self.hook_handle.remove()
+        else:
+            self.handle_pre.remove()
+            self.handle_post.remove()
+
+    @classmethod
+    def wrap_layer(cls, name: str, layer: nn.Module, **kwargs):  # -> SinglePluginBlock:
+        raise NotImplementedError(f'wrap_layer of {cls} is not implemented.')
+
+    @classmethod
+    def wrap_model(cls, plugin_name: str, model: nn.Module, exclude_key=None, **kwargs):  # -> Dict[str, SinglePluginBlock]:
+        plugin_block_dict = {}
+        if isinstance_list(model, cls.wrapable_classes):
+            plugin_block_dict[''] = cls.wrap_layer(plugin_name, model, **kwargs)
+        else:
+            if exclude_key:
+                # there maybe multiple single plugin block, avoid insert plugin into plugin blocks with exclude_key
+                named_modules = {name: layer for name, layer in model.named_modules() if exclude_key not in name}
+            else:
+                named_modules = {name: layer for name, layer in model.named_modules()}
+            for name, layer in named_modules.items():
+                if isinstance_list(layer, cls.wrapable_classes):
+                    plugin_block_dict[name] = cls.wrap_layer(plugin_name, layer, **kwargs)
+        return plugin_block_dict
+
+class PluginBlock(BasePluginBlock):
+    def __init__(self, name, from_layer:Dict[str, Any], to_layer:Dict[str, Any], host_model=None):
+        super().__init__(name)
+        self.host_from = weakref.ref(from_layer['layer'])
+        self.host_to = weakref.ref(to_layer['layer'])
+        setattr(from_layer['layer'], name, self)
+
+        if from_layer['pre_hook']:
+            self.hook_handle_from = from_layer['layer'].register_forward_pre_hook(lambda host, fea_in: self.from_layer_hook(host, fea_in, None))
+        else:
+            self.hook_handle_from = from_layer['layer'].register_forward_hook(lambda host, fea_in, fea_out: self.from_layer_hook(host, fea_in, fea_out))
+        if to_layer['pre_hook']:
+            self.hook_handle_to = to_layer['layer'].register_forward_pre_hook(lambda host, fea_in: self.to_layer_hook(host, fea_in, None))
+        else:
+            self.hook_handle_to = to_layer['layer'].register_forward_hook(lambda host, fea_in, fea_out: self.to_layer_hook(host, fea_in, fea_out))
+
+    def from_layer_hook(self, host, fea_in:Tuple[torch.Tensor], fea_out:torch.Tensor):
+        self.feat_from = fea_in
+
+    def to_layer_hook(self, host, fea_in:Tuple[torch.Tensor], fea_out:torch.Tensor):
+        return self(self.feat_from, fea_in, fea_out)
+
+    def remove(self):
+        host_from = self.host_from()
+        delattr(host_from, self.name)
+        self.hook_handle_from.remove()
+        self.hook_handle_to.remove()
+
+class MultiPluginBlock(BasePluginBlock):
+    def __init__(self, name:str, from_layers:List[Dict[str, Any]], to_layers:List[Dict[str, Any]], host_model=None):
+        super().__init__(name)
+        assert host_model is not None
+        self.host_from = [weakref.ref(x['layer']) for x in from_layers]
+        self.host_to = [weakref.ref(x['layer']) for x in to_layers]
+        self.host_model = weakref.ref(host_model)
+        setattr(host_model, name, self)
+
+        self.feat_from=[None for _ in range(len(from_layers))]
+
+        self.hook_handle_from = []
+        self.hook_handle_to = []
+
+        for idx, layer in enumerate(from_layers):
+            if layer['pre_hook']:
+                handle_from = layer['layer'].register_forward_pre_hook(lambda host, fea_in, idx=idx:self.from_layer_hook(host, fea_in, None, idx))
+            else:
+                handle_from = layer['layer'].register_forward_hook(lambda host, fea_in, fea_out, idx=idx: self.from_layer_hook(host, fea_in, fea_out, idx))
+            self.hook_handle_from.append(handle_from)
+        for idx, layer in enumerate(to_layers):
+            if layer['pre_hook']:
+                handle_to = layer['layer'].register_forward_pre_hook(lambda host, fea_in, idx=idx:self.to_layer_hook(host, fea_in, None, idx))
+            else:
+                handle_to = layer['layer'].register_forward_hook(lambda host, fea_in, fea_out, idx=idx:self.to_layer_hook(host, fea_in, fea_out, idx))
+            self.hook_handle_to.append(handle_to)
+
+        self.record_count=0
+
+    def from_layer_hook(self, host, fea_in:Tuple[torch.Tensor], fea_out:Tuple[torch.Tensor], idx: int):
+        self.feat_from[idx] = fea_in
+        self.record_count+=1
+        if self.record_count==len(self.feat_from): # call forward when all feat is record
+            self.record_count = 0
+            self.feat_to = self(self.feat_from)
+
+    def to_layer_hook(self, host, fea_in:Tuple[torch.Tensor], fea_out:Tuple[torch.Tensor], idx: int):
+        return self.feat_to[idx] + fea_out
+
+    def remove(self):
+        host_model = self.host_model()
+        delattr(host_model, self.name)
+        for handle_from in self.hook_handle_from:
+            handle_from.remove()
+        for handle_to in self.hook_handle_to:
+            handle_to.remove()
+
+class PluginGroup:
+    def __init__(self, plugin_dict:Dict[str, BasePluginBlock]):
+        self.plugin_dict = plugin_dict # {host_model_path: plugin_object}
+
+    def __setitem__(self, k, v):
+        self.plugin_dict[k]=v
+
+    def __getitem__(self, k):
+        return self.plugin_dict[k]
+
+    @property
+    def plugin_name(self):
+        if self.empty():
+            return None
+        return next(iter(self.plugin_dict.values())).name
+
+    def remove(self):
+        for plugin in self.plugin_dict.values():
+            plugin.remove()
+
+    def state_dict(self, model=None):
+        if model is None:
+            return {f'{k}.___.{ks}':vs for k,v in self.plugin_dict.items() for ks,vs in v.state_dict().items()}
+        else:
+            sd_model = model.state_dict()
+            return {f'{k}.___.{ks}':sd_model[f'{k}.{v.name}.{ks}'] for k,v in self.plugin_dict.items() for ks,vs in v.state_dict().items()}
+
+    def empty(self):
+        return len(self.plugin_dict)==0
+
```

### Comparing `hcpdiff-0.2.2/hcpdiff/models/text_emb_ex.py` & `hcpdiff-0.3.0/hcpdiff/models/text_emb_ex.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,91 +1,91 @@
-"""
-text_emb_ex.py
-====================
-    :Name:        hook for embedding
-    :Author:      Dong Ziyi
-    :Affiliation: HCP Lab, SYSU
-    :Created:     10/03/2023
-    :Licence:     Apache-2.0
-"""
-from typing import Tuple
-
-import torch
-from torch import nn
-import os
-from loguru import logger
-from einops import rearrange, repeat
-
-from ..utils.net_utils import load_emb
-from .plugin import SinglePluginBlock
-
-class EmbeddingPTHook(SinglePluginBlock):
-    def __init__(self, token_embedding:nn.Module, N_word=75, N_repeats=3):
-        super().__init__('emb_ex', token_embedding)
-        self.handle_pre = token_embedding.register_forward_pre_hook(self.pre_hook)
-
-        self.N_word=N_word
-        self.N_repeats=N_repeats
-        self.num_embeddings=token_embedding.num_embeddings
-        self.emb={}
-        self.emb_train=nn.ParameterList()
-
-    def add_emb(self, emb:nn.Parameter, token_id:int):
-        self.emb[token_id]=emb
-
-    def pre_hook(self, host, input_ids: Tuple[torch.Tensor]):
-        self.input_ids = rearrange(input_ids[0], '(b r) w -> b (r w)', r=self.N_repeats)  # 兼容Attention mask
-        return self.input_ids.clip(0, self.num_embeddings-1)
-
-    def forward(self, fea_in:Tuple[torch.Tensor], inputs_embeds:torch.Tensor): # inputs_embeds:[B, N_word+2, N_emb]
-        '''
-        :param input_ids: [B, N_ids]
-        :return: [B, N_repeat, N_word+2, N_emb]
-        '''
-        rep_idxs_B = self.input_ids >= self.num_embeddings
-        BOS = repeat(inputs_embeds[0,0,:], 'e -> r 1 e', r=self.N_repeats)
-        EOS = repeat(inputs_embeds[0,-1,:], 'e -> r 1 e', r=self.N_repeats)
-
-        replaced_embeds = []
-        for item, rep_idxs, ids_raw in zip(inputs_embeds, rep_idxs_B, self.input_ids):
-            # insert pt to embeddings
-            rep_idxs=torch.where(rep_idxs)[0]
-            item_new=[]
-            rep_idx_last=0
-            for rep_idx in rep_idxs:
-                rep_idx=rep_idx.item()
-                item_new.append(item[rep_idx_last:rep_idx, :])
-                item_new.append(self.emb[ids_raw[rep_idx].item()].to(dtype=item.dtype))
-                rep_idx_last=rep_idx+1
-            item_new.append(item[rep_idx_last:, :])
-
-            # split to N_repeat sentence
-            replaced_item = torch.cat(item_new, dim=0)[1:self.N_word*self.N_repeats+1, :]
-            replaced_item = rearrange(replaced_item, '(r w) e -> r w e', r=self.N_repeats, w=self.N_word)
-            replaced_item = torch.cat([BOS, replaced_item, EOS], dim=1) # [N_repeat, N_word+2, N_emb]
-
-            replaced_embeds.append(replaced_item)
-        return torch.cat(replaced_embeds, dim=0) # [B*N_repeat, N_word+2, N_emb]
-
-    def remove(self):
-        super(EmbeddingPTHook, self).remove()
-        self.handle_pre.remove()
-
-    @classmethod
-    def hook(cls, ex_words_emb, tokenizer, text_encoder, log=False, **kwargs):
-        word_list = list(ex_words_emb.keys())
-        tokenizer.add_tokens(word_list)
-        token_ids = tokenizer(' '.join(word_list)).input_ids[1:-1]
-
-        embedding_hook = cls(text_encoder.text_model.embeddings.token_embedding, **kwargs)
-        #text_encoder.text_model.embeddings.token_embedding = embedding_hook
-        for tid, word in zip(token_ids, word_list):
-            embedding_hook.add_emb(ex_words_emb[word], tid)
-            if log:
-                logger.info(f'hook: {word}, len: {ex_words_emb[word].shape[0]}, id: {tid}')
-        return embedding_hook
-
-    @classmethod
-    def hook_from_dir(cls, emb_dir, tokenizer, text_encoder, log=True, device='cuda:0', **kwargs):
-        ex_words_emb = {file[:-3]: nn.Parameter(load_emb(os.path.join(emb_dir, file)).to(device), requires_grad=False)
-                        for file in os.listdir(emb_dir) if file.endswith('.pt')}
-        return cls.hook(ex_words_emb, tokenizer, text_encoder, log, **kwargs), ex_words_emb
+"""
+text_emb_ex.py
+====================
+    :Name:        hook for embedding
+    :Author:      Dong Ziyi
+    :Affiliation: HCP Lab, SYSU
+    :Created:     10/03/2023
+    :Licence:     Apache-2.0
+"""
+from typing import Tuple
+
+import torch
+from torch import nn
+import os
+from loguru import logger
+from einops import rearrange, repeat
+
+from ..utils.net_utils import load_emb
+from .plugin import SinglePluginBlock
+
+class EmbeddingPTHook(SinglePluginBlock):
+    def __init__(self, token_embedding:nn.Module, N_word=75, N_repeats=3):
+        super().__init__('emb_ex', token_embedding)
+        self.handle_pre = token_embedding.register_forward_pre_hook(self.pre_hook)
+
+        self.N_word=N_word
+        self.N_repeats=N_repeats
+        self.num_embeddings=token_embedding.num_embeddings
+        self.emb={}
+        self.emb_train=nn.ParameterList()
+
+    def add_emb(self, emb:nn.Parameter, token_id:int):
+        self.emb[token_id]=emb
+
+    def pre_hook(self, host, input_ids: Tuple[torch.Tensor]):
+        self.input_ids = rearrange(input_ids[0], '(b r) w -> b (r w)', r=self.N_repeats)  # 兼容Attention mask
+        return self.input_ids.clip(0, self.num_embeddings-1)
+
+    def forward(self, fea_in:Tuple[torch.Tensor], inputs_embeds:torch.Tensor): # inputs_embeds:[B, N_word+2, N_emb]
+        '''
+        :param input_ids: [B, N_ids]
+        :return: [B, N_repeat, N_word+2, N_emb]
+        '''
+        rep_idxs_B = self.input_ids >= self.num_embeddings
+        BOS = repeat(inputs_embeds[0,0,:], 'e -> r 1 e', r=self.N_repeats)
+        EOS = repeat(inputs_embeds[0,-1,:], 'e -> r 1 e', r=self.N_repeats)
+
+        replaced_embeds = []
+        for item, rep_idxs, ids_raw in zip(inputs_embeds, rep_idxs_B, self.input_ids):
+            # insert pt to embeddings
+            rep_idxs=torch.where(rep_idxs)[0]
+            item_new=[]
+            rep_idx_last=0
+            for rep_idx in rep_idxs:
+                rep_idx=rep_idx.item()
+                item_new.append(item[rep_idx_last:rep_idx, :])
+                item_new.append(self.emb[ids_raw[rep_idx].item()].to(dtype=item.dtype))
+                rep_idx_last=rep_idx+1
+            item_new.append(item[rep_idx_last:, :])
+
+            # split to N_repeat sentence
+            replaced_item = torch.cat(item_new, dim=0)[1:self.N_word*self.N_repeats+1, :]
+            replaced_item = rearrange(replaced_item, '(r w) e -> r w e', r=self.N_repeats, w=self.N_word)
+            replaced_item = torch.cat([BOS, replaced_item, EOS], dim=1) # [N_repeat, N_word+2, N_emb]
+
+            replaced_embeds.append(replaced_item)
+        return torch.cat(replaced_embeds, dim=0) # [B*N_repeat, N_word+2, N_emb]
+
+    def remove(self):
+        super(EmbeddingPTHook, self).remove()
+        self.handle_pre.remove()
+
+    @classmethod
+    def hook(cls, ex_words_emb, tokenizer, text_encoder, log=False, **kwargs):
+        word_list = list(ex_words_emb.keys())
+        tokenizer.add_tokens(word_list)
+        token_ids = tokenizer(' '.join(word_list)).input_ids[1:-1]
+
+        embedding_hook = cls(text_encoder.text_model.embeddings.token_embedding, **kwargs)
+        #text_encoder.text_model.embeddings.token_embedding = embedding_hook
+        for tid, word in zip(token_ids, word_list):
+            embedding_hook.add_emb(ex_words_emb[word], tid)
+            if log:
+                logger.info(f'hook: {word}, len: {ex_words_emb[word].shape[0]}, id: {tid}')
+        return embedding_hook
+
+    @classmethod
+    def hook_from_dir(cls, emb_dir, tokenizer, text_encoder, log=True, device='cuda:0', **kwargs):
+        ex_words_emb = {file[:-3]: nn.Parameter(load_emb(os.path.join(emb_dir, file)).to(device), requires_grad=False)
+                        for file in os.listdir(emb_dir) if file.endswith('.pt')}
+        return cls.hook(ex_words_emb, tokenizer, text_encoder, log, **kwargs), ex_words_emb
```

### Comparing `hcpdiff-0.2.2/hcpdiff/models/textencoder_ex.py` & `hcpdiff-0.3.0/hcpdiff/models/textencoder_ex.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,134 +1,134 @@
-"""
-textencoder_ex.py
-====================
-    :Name:        extend text encoder
-    :Author:      Dong Ziyi
-    :Affiliation: HCP Lab, SYSU
-    :Created:     10/03/2023
-    :Licence:     Apache-2.0
-"""
-
-import torch
-from torch import nn
-from typing import Tuple, Optional
-from transformers.models.clip.modeling_clip import CLIPAttention
-from einops import repeat, rearrange
-from einops.layers.torch import Rearrange
-from collections import deque
-
-class TEEXHook:
-    def __init__(self, text_enc:nn.Module, tokenizer, N_repeats=3, clip_skip=0, device='cuda'):
-        self.text_enc = text_enc
-        self.tokenizer = tokenizer
-
-        self.N_repeats = N_repeats
-        self.clip_skip = clip_skip
-        self.device = device
-        self.attn_mult = None
-
-        text_enc.register_forward_hook(self.forward_hook)
-        text_enc.register_forward_pre_hook(self.forward_hook_input)
-
-    def encode_prompt_to_emb(self, prompt):
-        text_inputs = self.tokenizer(
-            prompt,
-            padding="max_length",
-            max_length=self.tokenizer.model_max_length * self.N_repeats,
-            truncation=True,
-            return_tensors="pt",
-        )
-        text_input_ids = text_inputs.input_ids
-
-        if hasattr(self.text_enc.config, "use_attention_mask") and self.text_enc.config.use_attention_mask:
-            attention_mask = text_inputs.attention_mask.to(self.device)
-        else:
-            attention_mask = None
-
-        prompt_embeds = self.text_enc(
-            text_input_ids.to(self.device),
-            attention_mask=attention_mask,
-            output_hidden_states=True,
-        )
-        return prompt_embeds
-
-    def forward_hook_input(self, host, feat_in):
-        feat_re = rearrange(feat_in[0], 'b (r w) -> (b r) w', r=self.N_repeats) # 使Attention mask的尺寸为N_word+2
-        return (feat_re,) if len(feat_in)==1 else (feat_re, *feat_in[1:])
-
-    def forward_hook(self, host, feat_in:Tuple[torch.Tensor], feat_out):
-        if self.clip_skip>0:
-            encoder_hidden_states = feat_out['hidden_states'][-self.clip_skip-1]
-            encoder_hidden_states = self.text_enc.text_model.final_layer_norm(encoder_hidden_states)
-            encoder_hidden_states = encoder_hidden_states + 0*feat_out['last_hidden_state'] # avoid unused parameters, make gradient checkpointing happy
-        else:
-            encoder_hidden_states = feat_out['last_hidden_state']  # Get the text embedding for conditioning
-
-        encoder_hidden_states = rearrange(encoder_hidden_states, '(b r) ... -> b r ...', r=self.N_repeats)  # [B, N_repeat, N_word+2, N_emb]
-        BOS, EOS = encoder_hidden_states[:, 0, :1, :], encoder_hidden_states[:, -1, -1:, :]
-        encoder_hidden_states = torch.cat([BOS, encoder_hidden_states[:, :, 1:-1, :].flatten(1, 2), EOS], dim=1)  # [B, N_repeat*N_word+2, N_emb]
-
-        return encoder_hidden_states
-
-    @staticmethod
-    def mult_attn(prompt_embeds, attn_mult):
-        if attn_mult!=None:
-            for i, item in enumerate(attn_mult):
-                if len(item)>0:
-                    original_mean = prompt_embeds[i, ...].mean()
-                    prompt_embeds[i, 1:len(item) + 1, :] *= item.view(-1, 1).to(prompt_embeds.device)
-                    new_mean = prompt_embeds[i, ...].mean()
-                    prompt_embeds[i, ...] *= original_mean / new_mean
-        return prompt_embeds
-
-    def enable_xformers(self):
-        try:
-            from xformers.components import build_attention
-            my_config = {
-                "name": 'scaled_dot_product',
-                "dropout": 0.0,
-            }
-            self.clip_attention = build_attention(my_config)
-
-            for k,v in self.text_enc.named_modules():
-                if isinstance(v, CLIPAttention):
-                    self.apply_xformers_attention_clip(v)
-        except:
-            print('xformers not find')
-
-    def apply_xformers_attention_clip(self, layer):
-        re_qkv = Rearrange('b l (h hd) -> b h l hd', h=layer.num_heads, hd=layer.head_dim)
-
-        def forward(hidden_states: torch.Tensor,
-                    attention_mask: Optional[torch.Tensor] = None,
-                    causal_attention_mask: Optional[torch.Tensor] = None,
-                    output_attentions: Optional[bool] = False,
-                    ) -> Tuple[torch.Tensor, Optional[torch.Tensor], Optional[Tuple[torch.Tensor]]]:
-            """Input shape: Batch x Time x Channel"""
-
-            # get query proj
-            query_states = re_qkv(layer.q_proj(hidden_states)) #* layer.scale
-            key_states = re_qkv(layer.k_proj(hidden_states))
-            value_states = re_qkv(layer.v_proj(hidden_states))
-
-            att_mask=None
-            if attention_mask is not None:
-                att_mask = repeat(attention_mask, 'b 1 x y -> (b h) x y', h=layer.num_heads)
-
-            if causal_attention_mask is not None:
-                causal_attention_mask = repeat(causal_attention_mask, 'b 1 x y -> (b h) x y', h=layer.num_heads)
-                if att_mask is None:
-                    att_mask = causal_attention_mask
-                else:
-                    att_mask += causal_attention_mask
-
-            attn_output = self.clip_attention(query_states, key_states, value_states, att_mask=att_mask)
-            attn_output = rearrange(attn_output, 'b h l hd -> b l (h hd)', h=layer.num_heads)
-
-            attn_output = layer.out_proj(attn_output)
-
-            return attn_output, None
-        layer.forward = forward
-
-    @classmethod
-    def hook_pipe(cls, pipe, N_repeats=3, clip_skip=0):
+"""
+textencoder_ex.py
+====================
+    :Name:        extend text encoder
+    :Author:      Dong Ziyi
+    :Affiliation: HCP Lab, SYSU
+    :Created:     10/03/2023
+    :Licence:     Apache-2.0
+"""
+
+import torch
+from torch import nn
+from typing import Tuple, Optional
+from transformers.models.clip.modeling_clip import CLIPAttention
+from einops import repeat, rearrange
+from einops.layers.torch import Rearrange
+from collections import deque
+
+class TEEXHook:
+    def __init__(self, text_enc:nn.Module, tokenizer, N_repeats=3, clip_skip=0, device='cuda'):
+        self.text_enc = text_enc
+        self.tokenizer = tokenizer
+
+        self.N_repeats = N_repeats
+        self.clip_skip = clip_skip
+        self.device = device
+        self.attn_mult = None
+
+        text_enc.register_forward_hook(self.forward_hook)
+        text_enc.register_forward_pre_hook(self.forward_hook_input)
+
+    def encode_prompt_to_emb(self, prompt):
+        text_inputs = self.tokenizer(
+            prompt,
+            padding="max_length",
+            max_length=self.tokenizer.model_max_length * self.N_repeats,
+            truncation=True,
+            return_tensors="pt",
+        )
+        text_input_ids = text_inputs.input_ids
+
+        if hasattr(self.text_enc.config, "use_attention_mask") and self.text_enc.config.use_attention_mask:
+            attention_mask = text_inputs.attention_mask.to(self.device)
+        else:
+            attention_mask = None
+
+        prompt_embeds = self.text_enc(
+            text_input_ids.to(self.device),
+            attention_mask=attention_mask,
+            output_hidden_states=True,
+        )
+        return prompt_embeds
+
+    def forward_hook_input(self, host, feat_in):
+        feat_re = rearrange(feat_in[0], 'b (r w) -> (b r) w', r=self.N_repeats) # 使Attention mask的尺寸为N_word+2
+        return (feat_re,) if len(feat_in)==1 else (feat_re, *feat_in[1:])
+
+    def forward_hook(self, host, feat_in:Tuple[torch.Tensor], feat_out):
+        if self.clip_skip>0:
+            encoder_hidden_states = feat_out['hidden_states'][-self.clip_skip-1]
+            encoder_hidden_states = self.text_enc.text_model.final_layer_norm(encoder_hidden_states)
+            encoder_hidden_states = encoder_hidden_states + 0*feat_out['last_hidden_state'] # avoid unused parameters, make gradient checkpointing happy
+        else:
+            encoder_hidden_states = feat_out['last_hidden_state']  # Get the text embedding for conditioning
+
+        encoder_hidden_states = rearrange(encoder_hidden_states, '(b r) ... -> b r ...', r=self.N_repeats)  # [B, N_repeat, N_word+2, N_emb]
+        BOS, EOS = encoder_hidden_states[:, 0, :1, :], encoder_hidden_states[:, -1, -1:, :]
+        encoder_hidden_states = torch.cat([BOS, encoder_hidden_states[:, :, 1:-1, :].flatten(1, 2), EOS], dim=1)  # [B, N_repeat*N_word+2, N_emb]
+
+        return encoder_hidden_states
+
+    @staticmethod
+    def mult_attn(prompt_embeds, attn_mult):
+        if attn_mult!=None:
+            for i, item in enumerate(attn_mult):
+                if len(item)>0:
+                    original_mean = prompt_embeds[i, ...].mean()
+                    prompt_embeds[i, 1:len(item) + 1, :] *= item.view(-1, 1).to(prompt_embeds.device)
+                    new_mean = prompt_embeds[i, ...].mean()
+                    prompt_embeds[i, ...] *= original_mean / new_mean
+        return prompt_embeds
+
+    def enable_xformers(self):
+        try:
+            from xformers.components import build_attention
+            my_config = {
+                "name": 'scaled_dot_product',
+                "dropout": 0.0,
+            }
+            self.clip_attention = build_attention(my_config)
+
+            for k,v in self.text_enc.named_modules():
+                if isinstance(v, CLIPAttention):
+                    self.apply_xformers_attention_clip(v)
+        except:
+            print('xformers not find')
+
+    def apply_xformers_attention_clip(self, layer):
+        re_qkv = Rearrange('b l (h hd) -> b h l hd', h=layer.num_heads, hd=layer.head_dim)
+
+        def forward(hidden_states: torch.Tensor,
+                    attention_mask: Optional[torch.Tensor] = None,
+                    causal_attention_mask: Optional[torch.Tensor] = None,
+                    output_attentions: Optional[bool] = False,
+                    ) -> Tuple[torch.Tensor, Optional[torch.Tensor], Optional[Tuple[torch.Tensor]]]:
+            """Input shape: Batch x Time x Channel"""
+
+            # get query proj
+            query_states = re_qkv(layer.q_proj(hidden_states)) #* layer.scale
+            key_states = re_qkv(layer.k_proj(hidden_states))
+            value_states = re_qkv(layer.v_proj(hidden_states))
+
+            att_mask=None
+            if attention_mask is not None:
+                att_mask = repeat(attention_mask, 'b 1 x y -> (b h) x y', h=layer.num_heads)
+
+            if causal_attention_mask is not None:
+                causal_attention_mask = repeat(causal_attention_mask, 'b 1 x y -> (b h) x y', h=layer.num_heads)
+                if att_mask is None:
+                    att_mask = causal_attention_mask
+                else:
+                    att_mask += causal_attention_mask
+
+            attn_output = self.clip_attention(query_states, key_states, value_states, att_mask=att_mask)
+            attn_output = rearrange(attn_output, 'b h l hd -> b l (h hd)', h=layer.num_heads)
+
+            attn_output = layer.out_proj(attn_output)
+
+            return attn_output, None
+        layer.forward = forward
+
+    @classmethod
+    def hook_pipe(cls, pipe, N_repeats=3, clip_skip=0):
         return cls(pipe.text_encoder, pipe.tokenizer, N_repeats=N_repeats, device=pipe._execution_device, clip_skip=clip_skip)
```

### Comparing `hcpdiff-0.2.2/hcpdiff/tools/convert_caption_txt2json.py` & `hcpdiff-0.3.0/hcpdiff/tools/convert_caption_txt2json.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-import argparse
-import json
-import os
-
-from hcpdiff.utils.img_size_tool import types_support
-
-parser = argparse.ArgumentParser(description='Stable Diffusion Training')
-parser.add_argument('--data_root', type=str, default='')
-args = parser.parse_args()
-
-
-def get_txt_caption(path):
-    with open(path, encoding='utf8') as f:
-        return f.read().strip()
-
-
-captions = {}
-for file in os.listdir(args.data_root):
-    ext_idx = file.rfind('.')
-    file_name = file[:ext_idx]
-    if file[ext_idx + 1:] in types_support:
-        captions[file] = get_txt_caption(os.path.join(args.data_root, f'{file_name}.txt'))
-
-with open(os.path.join(args.data_root, f'image_captions.json'), "w", encoding='utf8') as f:
-    json.dump(captions, f)
+import argparse
+import json
+import os
+
+from hcpdiff.utils.img_size_tool import types_support
+
+parser = argparse.ArgumentParser(description='Stable Diffusion Training')
+parser.add_argument('--data_root', type=str, default='')
+args = parser.parse_args()
+
+
+def get_txt_caption(path):
+    with open(path, encoding='utf8') as f:
+        return f.read().strip()
+
+
+captions = {}
+for file in os.listdir(args.data_root):
+    ext_idx = file.rfind('.')
+    file_name = file[:ext_idx]
+    if file[ext_idx + 1:] in types_support:
+        captions[file] = get_txt_caption(os.path.join(args.data_root, f'{file_name}.txt'))
+
+with open(os.path.join(args.data_root, f'image_captions.json'), "w", encoding='utf8') as f:
+    json.dump(captions, f)
```

### Comparing `hcpdiff-0.2.2/hcpdiff/tools/gen_from_ptlist.py` & `hcpdiff-0.3.0/hcpdiff/tools/gen_from_ptlist.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,47 +1,47 @@
-import os.path
-
-import torch
-from diffusers import StableDiffusionPipeline
-from PIL import Image
-import pyarrow.parquet as pq
-import argparse
-import json
-from tqdm.auto import tqdm
-
-parser = argparse.ArgumentParser(description='Stable Diffusion Training')
-parser.add_argument('--prompt_file', type=str, default='')
-parser.add_argument('--model', type=str, default='runwayml/stable-diffusion-v1-5')
-parser.add_argument('--out_dir', type=str, default=r'./prompt_ds')
-parser.add_argument('--negative_prompt', type=str, default='')
-parser.add_argument('--num', type=int, default=200)
-parser.add_argument('--bs', type=int, default=4)
-args = parser.parse_args()
-
-torch.backends.cudnn.benchmark = True
-
-
-def split_batch(data, bs):
-    return [data[i:i + bs] for i in range(0, len(data), bs)]
-
-
-data = pq.read_table(args.prompt_file).to_batches(args.bs)
-pipeline = StableDiffusionPipeline.from_pretrained(args.model, torch_dtype=torch.float16)
-pipeline.requires_safety_checker = False
-pipeline.safety_checker = None
-pipeline.to("cuda")
-pipeline.unet.to(memory_format=torch.channels_last)
-pipeline.enable_xformers_memory_efficient_attention()
-
-count = 0
-captions = {}
-with torch.inference_mode():
-    for i in tqdm(range(args.num)):
-        p_batch = data[i][0].to_pylist()
-        imgs = pipeline(p_batch, negative_prompt=[args.negative_prompt] * len(p_batch)).images
-        for prompt, img in zip(p_batch, imgs):
-            img.resize((512, 512), Image.BILINEAR).save(os.path.join(args.out_dir, f'{count}.png'), format='PNG')
-            captions[f'{count}.png'] = prompt
-            count += 1
-
-with open(os.path.join(args.out_dir, f'image_captions.json'), "w") as f:
-    json.dump(captions, f)
+import os.path
+
+import torch
+from diffusers import StableDiffusionPipeline
+from PIL import Image
+import pyarrow.parquet as pq
+import argparse
+import json
+from tqdm.auto import tqdm
+
+parser = argparse.ArgumentParser(description='Stable Diffusion Training')
+parser.add_argument('--prompt_file', type=str, default='')
+parser.add_argument('--model', type=str, default='runwayml/stable-diffusion-v1-5')
+parser.add_argument('--out_dir', type=str, default=r'./prompt_ds')
+parser.add_argument('--negative_prompt', type=str, default='')
+parser.add_argument('--num', type=int, default=200)
+parser.add_argument('--bs', type=int, default=4)
+args = parser.parse_args()
+
+torch.backends.cudnn.benchmark = True
+
+
+def split_batch(data, bs):
+    return [data[i:i + bs] for i in range(0, len(data), bs)]
+
+
+data = pq.read_table(args.prompt_file).to_batches(args.bs)
+pipeline = StableDiffusionPipeline.from_pretrained(args.model, torch_dtype=torch.float16)
+pipeline.requires_safety_checker = False
+pipeline.safety_checker = None
+pipeline.to("cuda")
+pipeline.unet.to(memory_format=torch.channels_last)
+pipeline.enable_xformers_memory_efficient_attention()
+
+count = 0
+captions = {}
+with torch.inference_mode():
+    for i in tqdm(range(args.num)):
+        p_batch = data[i][0].to_pylist()
+        imgs = pipeline(p_batch, negative_prompt=[args.negative_prompt] * len(p_batch)).images
+        for prompt, img in zip(p_batch, imgs):
+            img.resize((512, 512), Image.BILINEAR).save(os.path.join(args.out_dir, f'{count}.png'), format='PNG')
+            captions[f'{count}.png'] = prompt
+            count += 1
+
+with open(os.path.join(args.out_dir, f'image_captions.json'), "w") as f:
+    json.dump(captions, f)
```

### Comparing `hcpdiff-0.2.2/hcpdiff/tools/init_proj.py` & `hcpdiff-0.3.0/hcpdiff/tools/init_proj.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-import sys
-import shutil
-import os
-
-
-def main():
-    try:
-        if os.path.exists(r'./cfgs'):
-            shutil.rmtree(r'./cfgs')
-        if os.path.exists(r'./prompt_tuning_template'):
-            shutil.rmtree(r'./prompt_tuning_template')
-        shutil.copytree(os.path.join(sys.prefix, 'hcpdiff/cfgs'), r'./cfgs')
-        shutil.copytree(os.path.join(sys.prefix, 'hcpdiff/prompt_tuning_template'), r'./prompt_tuning_template')
-    except:
-        shutil.copytree(os.path.join(sys.prefix, '../hcpdiff/cfgs'), r'./cfgs')
-        shutil.copytree(os.path.join(sys.prefix, '../hcpdiff/prompt_tuning_template'), r'./prompt_tuning_template')
+import sys
+import shutil
+import os
+
+
+def main():
+    try:
+        if os.path.exists(r'./cfgs'):
+            shutil.rmtree(r'./cfgs')
+        if os.path.exists(r'./prompt_tuning_template'):
+            shutil.rmtree(r'./prompt_tuning_template')
+        shutil.copytree(os.path.join(sys.prefix, 'hcpdiff/cfgs'), r'./cfgs')
+        shutil.copytree(os.path.join(sys.prefix, 'hcpdiff/prompt_tuning_template'), r'./prompt_tuning_template')
+    except:
+        shutil.copytree(os.path.join(sys.prefix, '../hcpdiff/cfgs'), r'./cfgs')
+        shutil.copytree(os.path.join(sys.prefix, '../hcpdiff/prompt_tuning_template'), r'./prompt_tuning_template')
```

### Comparing `hcpdiff-0.2.2/hcpdiff/train_ac.py` & `hcpdiff-0.3.0/hcpdiff/train_ac.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,549 +1,543 @@
-"""
-train_ac.py
-====================
-    :Name:        train with accelerate
-    :Author:      Dong Ziyi
-    :Affiliation: HCP Lab, SYSU
-    :Created:     10/03/2023
-    :Licence:     Apache-2.0
-"""
-
-
-import argparse
-import itertools
-import os
-import sys
-
-import torch
-import torch.utils.checkpoint
-import torch.utils.data
-import transformers
-from accelerate import Accelerator, DistributedDataParallelKwargs
-from accelerate.utils import set_seed
-from transformers import AutoTokenizer
-from omegaconf import OmegaConf
-import hydra
-from loguru import logger
-import time
-from functools import partial
-
-import diffusers
-from diffusers import AutoencoderKL, UNet2DConditionModel
-from diffusers.utils.import_utils import is_xformers_available
-
-from hcpdiff.data import RatioBucket
-from hcpdiff.utils.utils import load_config_with_cli, get_cfg_range
-from hcpdiff.data.utils import cycle_data
-from hcpdiff.utils.net_utils import get_scheduler, import_text_encoder_class, TEUnetWrapper, load_emb
-from hcpdiff.models import EmbeddingPTHook, TEEXHook, CFGContext, DreamArtistPTContext
-from hcpdiff.utils.ema import ModelEMA
-from hcpdiff.utils.cfg_net_tools import make_hcpdiff, make_plugin
-from hcpdiff.data import collate_fn_ft
-from hcpdiff.visualizer import Visualizer
-from hcpdiff.utils.ckpt_manager import CkptManagerPKL, CkptManagerSafe
-
-class Trainer:
-    def __init__(self, cfgs_raw):
-        cfgs = hydra.utils.instantiate(cfgs_raw)
-        self.cfgs=cfgs
-
-        self.init_context(cfgs_raw)
-
-        if self.is_local_main_process:
-            self.exp_dir = os.path.join(self.cfgs.exp_dir, f'{time.strftime("%Y-%m-%d-%H-%M-%S")}')
-            os.makedirs(os.path.join(self.exp_dir, 'ckpts/'), exist_ok=True)
-            logger.add(os.path.join(self.exp_dir, 'train.log'))
-            with open(os.path.join(self.exp_dir, 'cfg.yaml'), 'w', encoding='utf-8') as f:
-                f.write(OmegaConf.to_yaml(cfgs_raw))
-        else:
-            logger.disable("__main__")
-
-        logger.info(f'world_size: {self.world_size}')
-        logger.info(f'accumulation: {self.cfgs.train.gradient_accumulation_steps}')
-
-        if self.is_local_main_process:
-            transformers.utils.logging.set_verbosity_warning()
-            diffusers.utils.logging.set_verbosity_warning()
-        else:
-            transformers.utils.logging.set_verbosity_error()
-            diffusers.utils.logging.set_verbosity_error()
-
-        self.lr=1e-5 # no usage, place set lr in cfgs
-        self.train_TE = (cfgs.text_encoder is not None) or (cfgs.lora_text_encoder is not None) or (cfgs.plugin_TE is not None)
-
-        self.build_ckpt_manager()
-        self.build_model()
-        self.make_hooks()
-        self.config_model()
-        self.cache_latents=False
-        self.batch_size_list = []
-        self.train_loader=self.build_data(cfgs.data)
-        if cfgs.data_class is None:
-            self.train_loader_class=None # without DreamBooth
-        else:
-            self.train_loader_class=self.build_data(cfgs.data_class)
-        if self.cache_latents:
-            self.vae = self.vae.to('cpu')
-        self.build_optimizer_scheduler()
-        self.criterion = cfgs.train.loss.criterion
-
-        self.cfg_scale = get_cfg_range(cfgs.train.cfg_scale)
-        if self.cfg_scale[1]==1.0:
-            self.cfg_context = CFGContext()
-        else: # DreamArtist
-            self.cfg_context = DreamArtistPTContext(self.cfg_scale, self.num_train_timesteps)
-
-        with torch.no_grad():
-            self.build_ema()
-
-        self.load_resume()
-
-        if cfgs.allow_tf32:
-            torch.backends.cuda.matmul.allow_tf32 = True
-
-        self.prepare()
-
-    @property
-    def device(self):
-        return self.accelerator.device
-
-    @property
-    def is_local_main_process(self):
-        return self.accelerator.is_local_main_process
-
-    def init_context(self, cfgs_raw):
-        ddp_kwargs = DistributedDataParallelKwargs(broadcast_buffers=False)
-        self.accelerator = Accelerator(
-            gradient_accumulation_steps=self.cfgs.train.gradient_accumulation_steps,
-            mixed_precision=self.cfgs.mixed_precision,
-            step_scheduler_with_optimizer=False,
-            kwargs_handlers=[ddp_kwargs], # fix inplace bug in DDP while use data_class
-        )
-
-        self.local_rank = int(os.environ.get("LOCAL_RANK", -1))
-        self.world_size = self.accelerator.num_processes
-
-        set_seed(self.cfgs.seed + self.local_rank)
-
-    def prepare(self):
-        # Prepare everything with accelerator.
-        if self.train_TE:
-            prepare_obj_list = [self.TE_unet, self.train_loader]
-            prepare_name_list = ['TE_unet', 'train_loader']
-        else:
-            prepare_obj_list = [self.unet, self.train_loader]
-            prepare_name_list = ['unet', 'train_loader']
-        if hasattr(self, 'optimizer'):
-            prepare_obj_list.extend([self.optimizer, self.lr_scheduler])
-            prepare_name_list.extend(['optimizer', 'lr_scheduler'])
-        if hasattr(self, 'optimizer_pt'):
-            prepare_obj_list.extend([self.optimizer_pt, self.lr_scheduler_pt])
-            prepare_name_list.extend(['optimizer_pt', 'lr_scheduler_pt'])
-
-        prepared_obj = self.accelerator.prepare(*prepare_obj_list)
-        for name, obj in zip(prepare_name_list, prepared_obj):
-            setattr(self, name, obj)
-
-    def scale_lr(self, parameters):
-        bs = sum(self.batch_size_list)
-        scale_factor = bs * self.world_size * self.cfgs.train.gradient_accumulation_steps
-        for param in parameters:
-            if 'lr' in param:
-                param['lr'] *= scale_factor
-
-    def build_model(self):
-        # Load the tokenizer
-        if self.cfgs.model.tokenizer_name:
-            self.tokenizer = AutoTokenizer.from_pretrained(self.cfgs.model.tokenizer_name, revision=self.cfgs.model.revision, use_fast=False)
-        elif self.cfgs.model.pretrained_model_name_or_path:
-            self.tokenizer = AutoTokenizer.from_pretrained(
-                self.cfgs.model.pretrained_model_name_or_path, subfolder="tokenizer",
-                revision=self.cfgs.model.revision, use_fast=False,
-            )
-
-        # Load scheduler and models
-        self.noise_scheduler = getattr(diffusers, self.cfgs.model.noise_scheduler).from_pretrained(self.cfgs.model.pretrained_model_name_or_path, subfolder="scheduler")
-        self.num_train_timesteps = len(self.noise_scheduler.timesteps)
-        self.vae: AutoencoderKL = AutoencoderKL.from_pretrained(self.cfgs.model.pretrained_model_name_or_path, subfolder="vae",
-                                            revision=self.cfgs.model.revision)
-        self.build_unet_and_TE()
-
-    def build_unet_and_TE(self): # for easy to use colossalAI
-        self.unet = UNet2DConditionModel.from_pretrained(
-            self.cfgs.model.pretrained_model_name_or_path, subfolder="unet", revision=self.cfgs.model.revision
-        )
-        # import correct text encoder class
-        text_encoder_cls = import_text_encoder_class(self.cfgs.model.pretrained_model_name_or_path, self.cfgs.model.revision)
-        self.text_encoder = text_encoder_cls.from_pretrained(
-            self.cfgs.model.pretrained_model_name_or_path, subfolder="text_encoder", revision=self.cfgs.model.revision
-        )
-
-        if self.train_TE:
-            # Wrap unet and text_encoder to make DDP happy. Multiple DDP has soooooo many fxxking bugs!
-            self.TE_unet = TEUnetWrapper(self.unet, self.text_encoder)
-
-
-    def build_ema(self):
-        if self.cfgs.model.ema_unet>0:
-            self.ema_unet = ModelEMA(self.unet.named_parameters(), self.cfgs.model.ema_unet)
-        if self.train_TE and self.cfgs.model.ema_text_encoder>0:
-            self.ema_text_encoder = ModelEMA(self.text_encoder.named_parameters(), self.cfgs.model.ema_text_encoder)
-
-    def build_ckpt_manager(self):
-        if self.cfgs.ckpt_type=='torch':
-            self.ckpt_manager = CkptManagerPKL()
-        elif self.cfgs.ckpt_type=='safetensors':
-            self.ckpt_manager = CkptManagerSafe()
-        else:
-            raise NotImplementedError(f'Not support ckpt type: {self.cfgs.ckpt_type}')
-        if self.is_local_main_process:
-            self.ckpt_manager.set_save_dir(os.path.join(self.exp_dir, 'ckpts'), emb_dir=self.cfgs.tokenizer_pt.emb_dir)
-
-    @property
-    def unet_raw(self):
-        return self.TE_unet.module.unet if self.train_TE else self.unet.module
-
-    @property
-    def text_encoder_raw(self):
-        return self.TE_unet.module.TE if self.train_TE else self.text_encoder
-
-    def config_model(self):
-        if self.cfgs.model.enable_xformers:
-            if is_xformers_available():
-                self.unet.enable_xformers_memory_efficient_attention()
-                #self.text_enc_hook.enable_xformers()
-            else:
-                raise ValueError("xformers is not available. Make sure it is installed correctly")
-
-        self.vae.requires_grad_(False)
-        self.unet.requires_grad_(False)
-        self.text_encoder.requires_grad_(False)
-
-        self.unet.eval()
-        self.text_encoder.eval()
-
-        if self.cfgs.model.gradient_checkpointing:
-            self.unet.enable_gradient_checkpointing()
-            if self.train_TE:
-                self.text_encoder.gradient_checkpointing_enable()
-
-        weight_dtype = torch.float32
-        if self.cfgs.mixed_precision == "fp16":
-            weight_dtype = torch.float16
-        elif self.cfgs.mixed_precision == "bf16":
-            weight_dtype = torch.bfloat16
-        self.weight_dtype = weight_dtype
-
-        # Move vae and text_encoder to device and cast to weight_dtype
-        self.vae = self.vae.to(self.device, dtype=weight_dtype)
-        if not self.train_TE:
-            self.text_encoder = self.text_encoder.to(self.device, dtype=weight_dtype)
-
-    @torch.no_grad()
-    def load_resume(self):
-        if self.cfgs.train.resume is not None:
-            for ckpt in self.cfgs.train.resume.ckpt_path.unet:
-                self.ckpt_manager.load_ckpt_to_model(self.unet, ckpt, model_ema=getattr(self, 'ema_unet', None))
-            for ckpt in self.cfgs.train.resume.ckpt_path.TE:
-                self.ckpt_manager.load_ckpt_to_model(self.text_encoder, ckpt, model_ema=getattr(self, 'ema_text_encoder', None))
-            for name, ckpt in self.cfgs.train.resume.ckpt_path.words:
-                self.ex_words_emb[name].data = load_emb(ckpt)
-
-    def make_hooks(self):
-        # Hook tokenizer and embedding to support pt
-        self.embedding_hook, self.ex_words_emb = EmbeddingPTHook.hook_from_dir(
-                        self.cfgs.tokenizer_pt.emb_dir, self.tokenizer, self.text_encoder, log=self.is_local_main_process,
-                        N_repeats=self.cfgs.model.tokenizer_repeats, device=self.device)
-
-        self.text_enc_hook = TEEXHook(self.text_encoder, self.tokenizer, N_repeats=self.cfgs.model.tokenizer_repeats, device=self.device,
-                                      clip_skip=self.cfgs.model.clip_skip)
-
-
-    def build_data(self, data_builder:partial) -> torch.utils.data.DataLoader:
-        batch_size = data_builder.keywords.pop('batch_size')
-        cache_latents = data_builder.keywords.pop('cache_latents')
-        self.batch_size_list.append(batch_size)
-
-        train_dataset = data_builder(tokenizer=self.tokenizer, tokenizer_repeats=self.cfgs.model.tokenizer_repeats)
-        train_dataset.bucket.build(batch_size * self.world_size)
-        arb = isinstance(train_dataset.bucket, RatioBucket)
-        logger.info(f"len(train_dataset): {len(train_dataset)}")
-
-        if cache_latents:
-            self.cache_latents = True
-            train_dataset.cache_latents(self.vae, self.weight_dtype, self.device, show_prog=self.is_local_main_process)
-
-        # Pytorch Data loader
-        train_sampler = torch.utils.data.distributed.DistributedSampler(train_dataset, num_replicas=self.world_size,
-                                                                        rank=self.local_rank, shuffle=not arb)
-        train_loader = torch.utils.data.DataLoader(train_dataset, batch_size=batch_size,
-            num_workers=self.cfgs.train.workers, sampler=train_sampler, collate_fn=collate_fn_ft)
-        return train_loader
-
-    def get_param_group_train(self):
-        # make miniFT and warp with lora
-        self.DA_lora = False
-        train_params_unet, self.lora_unet = make_hcpdiff(self.unet, self.cfgs.unet, self.cfgs.lora_unet)
-        if isinstance(self.lora_unet, tuple): # creat negative lora
-            self.DA_lora = True
-            self.lora_unet, self.lora_unet_neg = self.lora_unet
-        train_params_unet_plugin, self.all_plugin_unet = make_plugin(self.unet, self.cfgs.plugin_unet)
-        train_params_unet += train_params_unet_plugin
-
-        if self.train_TE:
-            train_params_text_encoder, self.lora_TE = make_hcpdiff(self.text_encoder, self.cfgs.text_encoder, self.cfgs.lora_text_encoder)
-            if isinstance(self.lora_TE, tuple):  # creat negative lora
-                self.DA_lora = True
-                self.lora_TE, self.lora_TE_neg = self.lora_TE
-            train_params_TE_plugin, self.all_plugin_TE = make_plugin(self.text_encoder, self.cfgs.plugin_TE)
-            train_params_text_encoder += train_params_TE_plugin
-        else:
-            train_params_text_encoder=[]
-
-        # params for embedding
-        train_params_emb = []
-        self.train_pts = {}
-        if self.cfgs.tokenizer_pt.train is not None:
-            for v in self.cfgs.tokenizer_pt.train:
-                self.train_pts[v.name]=self.ex_words_emb[v.name]
-                self.ex_words_emb[v.name].requires_grad=True
-                self.embedding_hook.emb_train.append(self.ex_words_emb[v.name])
-                train_params_emb.append({'params':self.ex_words_emb[v.name], 'lr':v.lr})
-
-        return train_params_unet + train_params_text_encoder, train_params_emb
-
-    def build_optimizer_scheduler(self):
-        # set optimizer
-        parameters, parameters_pt = self.get_param_group_train()
-
-        cfg_opt = self.cfgs.train.optimizer
-        if len(parameters)>0: # do fine-tuning
-            if self.cfgs.train.scale_lr:
-                self.scale_lr(parameters)
-
-            if cfg_opt.type=='adamw_8bit':
-                import bitsandbytes as bnb
-                self.optimizer = bnb.optim.AdamW8bit(params=parameters, lr=self.lr, weight_decay=cfg_opt.weight_decay)
-            elif cfg_opt.type=='deepspeed' and self.accelerator.state.deepspeed_plugin is not None:
-                from deepspeed.ops.adam import FusedAdam
-                self.optimizer = FusedAdam(params=parameters, lr=self.lr, weight_decay=cfg_opt.weight_decay)
-            elif cfg_opt.type=='adamw':
-                self.optimizer = torch.optim.AdamW(params=parameters, lr=self.lr, weight_decay=cfg_opt.weight_decay)
-            else:
-                self.optimizer = cfg_opt.optimizer.opt(parameters, lr=self.lr)
-
-            self.lr_scheduler = get_scheduler(optimizer=self.optimizer, **self.cfgs.train.scheduler)
-
-        if len(parameters_pt)>0: # do prompt-tuning
-            if self.cfgs.train.scale_lr_pt:
-                self.scale_lr(parameters_pt)
-
-            self.optimizer_pt = torch.optim.AdamW(params=parameters_pt, lr=self.lr, weight_decay=cfg_opt.weight_decay_pt)
-            self.lr_scheduler_pt = get_scheduler(optimizer=self.optimizer_pt, **self.cfgs.train.scheduler_pt)
-
-    def train(self):
-        total_batch_size = sum(self.batch_size_list) * self.world_size * self.cfgs.train.gradient_accumulation_steps
-
-        logger.info("***** Running training *****")
-        logger.info(f"  Num batches each epoch = {len(self.train_loader)}")
-        logger.info(f"  Num Steps = {self.cfgs.train.scheduler.num_training_steps}")
-        logger.info(f"  Instantaneous batch size per device = {sum(self.batch_size_list)}")
-        logger.info(f"  Total train batch size (w. parallel, distributed & accumulation) = {total_batch_size}")
-        logger.info(f"  Gradient Accumulation steps = {self.cfgs.train.gradient_accumulation_steps}")
-        self.global_step = 0
-        if self.cfgs.train.resume is not None:
-            self.global_step = self.cfgs.train.resume.start_step
-
-        if self.train_loader_class is not None:
-            self.data_iter_class = iter(cycle_data(self.train_loader_class))
-
-        loss_sum=0
-        for data, prompt_ids in cycle_data(self.train_loader):
-            loss=self.train_one_step(data, prompt_ids)
-            loss_sum+=loss
-
-            self.global_step += 1
-            if self.is_local_main_process:
-                if self.global_step % self.cfgs.train.save_step == 0:
-                    self.save_model()
-                if self.global_step % self.cfgs.train.log_step == 0:
-                    lr_model = self.lr_scheduler.get_last_lr()[0] if hasattr(self, 'lr_scheduler') else 0.
-                    lr_word = self.lr_scheduler_pt.get_last_lr()[0] if hasattr(self, 'lr_scheduler_pt') else 0.
-                    logger.info('Step [{}/{}], LR_model: {:.2e}, LR_word: {:.2e}, Loss: {:.5f}'
-                                .format(self.global_step, self.cfgs.train.scheduler.num_training_steps,
-                                        lr_model, lr_word, loss_sum / self.cfgs.train.log_step))
-                    loss_sum = 0
-
-            if self.global_step >= self.cfgs.train.scheduler.num_training_steps:
-                break
-
-        self.wait_for_everyone()
-        if self.is_local_main_process:
-            self.save_model()
-
-    def wait_for_everyone(self):
-        self.accelerator.wait_for_everyone()
-
-    @torch.no_grad()
-    def get_latents(self, image, dataset):
-        if dataset.latents is None:
-            latents = self.vae.encode(image).latent_dist.sample()
-            latents = latents * 0.18215
-        else:
-            latents = image  # Cached latents
-        return latents
-
-    def make_noise(self, latents):
-        # Sample noise that we'll add to the latents
-        noise = torch.randn_like(latents)
-        bsz = latents.shape[0]
-        # Sample a random timestep for each image
-        timesteps = torch.randint(0, self.noise_scheduler.config.num_train_timesteps, (bsz,), device=latents.device)
-        timesteps = timesteps.long()
-
-        # Add noise to the latents according to the noise magnitude at each timestep
-        # (this is the forward diffusion process)
-        return self.noise_scheduler.add_noise(latents, noise, timesteps), noise, timesteps
-
-    def encode_decode(self, prompt_ids, noisy_latents, timesteps, **kwargs):
-        # for DDP support
-        if self.train_TE:
-            model_pred = self.TE_unet(prompt_ids, noisy_latents, timesteps, **kwargs)
-        else:
-            input_all = dict(prompt_ids=prompt_ids, noisy_latents=noisy_latents, timesteps=timesteps, **kwargs)
-            if hasattr(self.text_encoder, 'input_feeder'):
-                for feeder in self.text_encoder.input_feeder:
-                    feeder(input_all)
-            if hasattr(self.unet_raw, 'input_feeder'):
-                for feeder in self.unet_raw.input_feeder:
-                    feeder(input_all)
-
-            encoder_hidden_states = self.text_encoder(prompt_ids, output_hidden_states=True)  # Get the text embedding for conditioning
-            model_pred = self.unet(noisy_latents, timesteps, encoder_hidden_states).sample  # Predict the noise residual
-        return model_pred
-
-    def forward(self, latents, prompt_ids, **kwargs):
-        noisy_latents, noise, timesteps = self.make_noise(latents)
-
-        # CFG context for DreamArtist
-        noisy_latents, timesteps = self.cfg_context.pre(noisy_latents, timesteps)
-        model_pred = self.encode_decode(prompt_ids, noisy_latents, timesteps, **kwargs)
-        model_pred = self.cfg_context.post(model_pred)
-
-        # Get the target for loss depending on the prediction type
-        if self.cfgs.train.loss.type == "eps":
-            target = noise
-        elif self.cfgs.train.loss.type == "sample":
-            target = self.noise_scheduler.step(noise, timesteps, noisy_latents)
-            model_pred = self.noise_scheduler.step(model_pred, timesteps, noisy_latents)
-        else:
-            raise ValueError(f"Unknown loss type {self.cfgs.train.loss.type}")
-        return model_pred, target
-
-    def train_one_step(self, data, prompt_ids):
-        image = data['img'].to(self.device, dtype=self.weight_dtype)
-        att_mask = data['mask'].to(self.device)
-        prompt_ids=prompt_ids.to(self.device)
-        other_datas = {k:v.to(self.device, dtype=self.weight_dtype) for k,v in data.items() if k!='img' and k!='mask'}
-
-        with self.accelerator.accumulate(self.unet):
-            latents = self.get_latents(image, self.train_loader.dataset)
-            model_pred, target = self.forward(latents, prompt_ids, **other_datas)
-
-            if self.train_loader_class is not None:
-                loss = self.get_loss(model_pred, target, att_mask) # Compute instance loss
-                self.accelerator.backward(loss)
-
-                #DreamBooth prior forward
-                data_cls, prompt_ids_cls = next(self.data_iter_class)
-                image_cls = data_cls['img'].to(self.device, dtype=self.weight_dtype)
-                att_mask_cls = data_cls['mask'].to(self.device)
-                prompt_ids_cls = prompt_ids_cls.to(self.device)
-                other_datas_cls = {k: v.to(self.device, dtype=self.weight_dtype) for k, v in data_cls.items() if k != 'img' and k != 'mask'}
-                latents_cls = self.get_latents(image_cls, self.train_loader_class.dataset)
-                model_pred_prior, target_prior = self.forward(latents_cls, prompt_ids_cls, **other_datas_cls)
-
-                prior_loss = self.get_loss(model_pred_prior, target_prior, att_mask_cls) # Compute prior loss
-                loss = self.cfgs.train.loss.prior_loss_weight * prior_loss
-                self.accelerator.backward(loss)
-            else:
-                loss = self.get_loss(model_pred, target, att_mask)
-                self.accelerator.backward(loss)
-
-            if hasattr(self, 'optimizer'):
-                if self.accelerator.sync_gradients: # fine-tuning
-                    params_to_clip = (
-                        itertools.chain(self.unet.parameters(), self.text_encoder.parameters())
-                        if self.train_TE else self.unet.parameters()
-                    )
-                    self.accelerator.clip_grad_norm_(params_to_clip, self.cfgs.train.max_grad_norm)
-                self.optimizer.step()
-                self.lr_scheduler.step()
-                self.optimizer.zero_grad(set_to_none=self.cfgs.train.set_grads_to_none)
-
-            if hasattr(self, 'optimizer_pt'): # prompt tuning
-                self.optimizer_pt.step()
-                self.lr_scheduler_pt.step()
-                self.optimizer_pt.zero_grad(set_to_none=self.cfgs.train.set_grads_to_none)
-
-            self.update_ema()
-        return loss.item()
-
-    def get_loss(self, model_pred, target, att_mask):
-        if len(self.embedding_hook.emb_train)>0:
-            return (self.criterion(model_pred.float(), target.float()) * att_mask).mean() \
-               + 0*sum(self.embedding_hook.emb_train).mean() # avoid unused parameters, make gradient checkpointing happy
-        else:
-            return (self.criterion(model_pred.float(), target.float()) * att_mask).mean()
-
-    def update_ema(self):
-        if hasattr(self, 'ema_unet'):
-            self.ema_unet.step(self.unet_raw.named_parameters())
-        if hasattr(self, 'ema_text_encoder'):
-            self.ema_text_encoder.step(self.text_encoder_raw.named_parameters())
-
-    def save_model(self, from_raw=False):
-        unet_raw=self.unet_raw
-        self.ckpt_manager.save_model_with_lora(unet_raw, self.lora_unet, model_ema=getattr(self, 'ema_unet', None),
-                                               name='unet', step=self.global_step)
-        self.ckpt_manager.save_plugins(unet_raw, self.all_plugin_unet, name='unet', step=self.global_step,
-                                       model_ema=getattr(self, 'ema_unet', None))
-        if self.train_TE:
-            TE_raw = self.text_encoder_raw
-            # exclude_key: embeddings should not save with text-encoder
-            self.ckpt_manager.save_model_with_lora(TE_raw, self.lora_TE, model_ema=getattr(self, 'ema_text_encoder', None),
-                                                   name='text_encoder', step=self.global_step, exclude_key='emb_ex.')
-            self.ckpt_manager.save_plugins(TE_raw, self.all_plugin_TE, name='text_encoder', step=self.global_step,
-                                           model_ema=getattr(self, 'ema_text_encoder', None))
-
-        if self.DA_lora:
-            self.ckpt_manager.save_model_with_lora(None, self.lora_unet_neg, name='unet-neg', step=self.global_step)
-            if self.train_TE:
-                self.ckpt_manager.save_model_with_lora(None, self.lora_TE_neg, name='text_encoder-neg', step=self.global_step)
-
-        self.ckpt_manager.save_embedding(self.train_pts, self.global_step, self.cfgs.tokenizer_pt.replace)
-
-        logger.info(f"Saved state, step: {self.global_step}")
-
-    def make_vis(self):
-        vis_dir = os.path.join(self.exp_dir ,f'vis-{self.global_step}')
-        new_components={
-            'unet': self.unet_raw,
-            'text_encoder': self.text_encoder_raw,
-            'tokenizer': self.tokenizer,
-            'vae': self.vae,
-        }
-        viser = Visualizer(self.cfgs.model.pretrained_model_name_or_path, new_components=new_components)
-        if self.cfgs.vis_info.prompt:
-            raise ValueError('vis_info.prompt is None. cannot generate without prompt.')
-        viser.vis_to_dir(vis_dir, self.cfgs.vis_prompt)
-
-
-if __name__ == '__main__':
-    parser = argparse.ArgumentParser(description='Stable Diffusion Training')
-    parser.add_argument('--cfg', type=str, default=None, required=True)
-    args, _ = parser.parse_known_args()
-
-    conf = load_config_with_cli(args.cfg, args_list=sys.argv[3:]) # skip --cfg
-    trainer=Trainer(conf)
-    trainer.train()
+"""
+train_ac.py
+====================
+    :Name:        train with accelerate
+    :Author:      Dong Ziyi
+    :Affiliation: HCP Lab, SYSU
+    :Created:     10/03/2023
+    :Licence:     Apache-2.0
+"""
+
+import argparse
+import itertools
+import os
+import sys
+import time
+from functools import partial
+
+import diffusers
+import hydra
+import numpy as np
+import torch
+import torch.utils.checkpoint
+import torch.utils.data
+import transformers
+from accelerate import Accelerator, DistributedDataParallelKwargs
+from accelerate.utils import set_seed
+from diffusers import AutoencoderKL, UNet2DConditionModel
+from diffusers.utils.import_utils import is_xformers_available
+from omegaconf import OmegaConf
+from transformers import AutoTokenizer
+
+from hcpdiff.ckpt_manager import CkptManagerPKL, CkptManagerSafe
+from hcpdiff.data import RatioBucket, DataGroup, collate_fn_ft
+from hcpdiff.loggers import LoggerGroup
+from hcpdiff.models import EmbeddingPTHook, TEEXHook, CFGContext, DreamArtistPTContext
+from hcpdiff.utils.cfg_net_tools import make_hcpdiff, make_plugin
+from hcpdiff.utils.ema import ModelEMA
+from hcpdiff.utils.net_utils import get_scheduler, import_text_encoder_class, TEUnetWrapper, load_emb
+from hcpdiff.utils.utils import load_config_with_cli, get_cfg_range, mgcd
+from hcpdiff.visualizer import Visualizer
+
+class Trainer:
+    def __init__(self, cfgs_raw):
+        cfgs = hydra.utils.instantiate(cfgs_raw)
+        self.cfgs = cfgs
+
+        self.init_context(cfgs_raw)
+
+        if self.is_local_main_process:
+            self.exp_dir = os.path.join(self.cfgs.exp_dir, f'{time.strftime("%Y-%m-%d-%H-%M-%S")}')
+            os.makedirs(os.path.join(self.exp_dir, 'ckpts/'), exist_ok=True)
+            self.loggers: LoggerGroup = LoggerGroup([builder(exp_dir=self.exp_dir) for builder in self.cfgs.logger])
+            with open(os.path.join(self.exp_dir, 'cfg.yaml'), 'w', encoding='utf-8') as f:
+                f.write(OmegaConf.to_yaml(cfgs_raw))
+        else:
+            self.loggers: LoggerGroup = LoggerGroup([builder(exp_dir=None) for builder in self.cfgs.logger])
+
+        self.min_log_step = mgcd(*[item.log_step for item in self.loggers.logger_list])
+
+        self.loggers.info(f'world_size: {self.world_size}')
+        self.loggers.info(f'accumulation: {self.cfgs.train.gradient_accumulation_steps}')
+
+        if self.is_local_main_process:
+            transformers.utils.logging.set_verbosity_warning()
+            diffusers.utils.logging.set_verbosity_warning()
+        else:
+            transformers.utils.logging.set_verbosity_error()
+            diffusers.utils.logging.set_verbosity_error()
+
+        self.lr = 1e-5  # no usage, place set lr in cfgs
+        self.train_TE = (cfgs.text_encoder is not None) or (cfgs.lora_text_encoder is not None) or (cfgs.plugin_TE is not None)
+
+        self.build_ckpt_manager()
+        self.build_model()
+        self.make_hooks()
+        self.config_model()
+        self.cache_latents = False
+
+        self.batch_size_list = []
+        assert len(cfgs.data)>0
+        loss_weights = [dataset.keywords['loss_weight'] for name, dataset in cfgs.data.items()]
+        self.train_loader_group = DataGroup([self.build_data(dataset) for name, dataset in cfgs.data.items()], loss_weights)
+
+        if self.cache_latents:
+            self.vae = self.vae.to('cpu')
+        self.build_optimizer_scheduler()
+        self.criterion = cfgs.train.loss.criterion(noise_scheduler=self.noise_scheduler, device=self.device)
+
+        self.cfg_scale = get_cfg_range(cfgs.train.cfg_scale)
+        if self.cfg_scale[1] == 1.0:
+            self.cfg_context = CFGContext()
+        else:  # DreamArtist
+            self.cfg_context = DreamArtistPTContext(self.cfg_scale, self.num_train_timesteps)
+
+        with torch.no_grad():
+            self.build_ema()
+
+        self.load_resume()
+
+        if cfgs.allow_tf32:
+            torch.backends.cuda.matmul.allow_tf32 = True
+
+        self.prepare()
+
+    @property
+    def device(self):
+        return self.accelerator.device
+
+    @property
+    def is_local_main_process(self):
+        return self.accelerator.is_local_main_process
+
+    def init_context(self, cfgs_raw):
+        ddp_kwargs = DistributedDataParallelKwargs(broadcast_buffers=False)
+        self.accelerator = Accelerator(
+            gradient_accumulation_steps=self.cfgs.train.gradient_accumulation_steps,
+            mixed_precision=self.cfgs.mixed_precision,
+            step_scheduler_with_optimizer=False,
+            kwargs_handlers=[ddp_kwargs],  # fix inplace bug in DDP while use data_class
+        )
+
+        self.local_rank = int(os.environ.get("LOCAL_RANK", -1))
+        self.world_size = self.accelerator.num_processes
+
+        set_seed(self.cfgs.seed+self.local_rank)
+
+    def prepare(self):
+        # Prepare everything with accelerator.
+        if self.train_TE:
+            # try:
+            #     self.TE_unet = torch.compile(self.TE_unet)
+            # except:
+            #     print('cannot compile model')
+            prepare_obj_list = [self.TE_unet]
+            prepare_name_list = ['TE_unet']
+        else:
+            # try:
+            #     self.unet = torch.compile(self.unet)
+            #     self.text_encoder = torch.compile(self.text_encoder)
+            # except:
+            #     print('cannot compile model')
+            prepare_obj_list = [self.unet]
+            prepare_name_list = ['unet']
+        if hasattr(self, 'optimizer'):
+            prepare_obj_list.extend([self.optimizer, self.lr_scheduler])
+            prepare_name_list.extend(['optimizer', 'lr_scheduler'])
+        if hasattr(self, 'optimizer_pt'):
+            prepare_obj_list.extend([self.optimizer_pt, self.lr_scheduler_pt])
+            prepare_name_list.extend(['optimizer_pt', 'lr_scheduler_pt'])
+
+        prepared_obj = self.accelerator.prepare(*prepare_obj_list)
+        for name, obj in zip(prepare_name_list, prepared_obj):
+            setattr(self, name, obj)
+
+        if len(self.train_loader_group) > 1:
+            self.train_loader_group.loader_list = list(self.accelerator.prepare(*self.train_loader_group.loader_list))
+        else:
+            self.train_loader_group.loader_list = [self.accelerator.prepare(*self.train_loader_group.loader_list)]
+
+    def scale_lr(self, parameters):
+        bs = sum(self.batch_size_list)
+        scale_factor = bs*self.world_size*self.cfgs.train.gradient_accumulation_steps
+        for param in parameters:
+            if 'lr' in param:
+                param['lr'] *= scale_factor
+
+    def build_model(self):
+        # Load the tokenizer
+        if self.cfgs.model.tokenizer_name:
+            self.tokenizer = AutoTokenizer.from_pretrained(self.cfgs.model.tokenizer_name, revision=self.cfgs.model.revision, use_fast=False)
+        elif self.cfgs.model.pretrained_model_name_or_path:
+            self.tokenizer = AutoTokenizer.from_pretrained(
+                self.cfgs.model.pretrained_model_name_or_path, subfolder="tokenizer",
+                revision=self.cfgs.model.revision, use_fast=False,
+            )
+
+        # Load scheduler and models
+        self.noise_scheduler = getattr(diffusers, self.cfgs.model.noise_scheduler) \
+            .from_pretrained(self.cfgs.model.pretrained_model_name_or_path, subfolder="scheduler")
+        self.num_train_timesteps = len(self.noise_scheduler.timesteps)
+        self.vae: AutoencoderKL = AutoencoderKL.from_pretrained(self.cfgs.model.pretrained_model_name_or_path, subfolder="vae",
+                                                                revision=self.cfgs.model.revision)
+        self.build_unet_and_TE()
+
+    def build_unet_and_TE(self):  # for easy to use colossalAI
+        self.unet = UNet2DConditionModel.from_pretrained(
+            self.cfgs.model.pretrained_model_name_or_path, subfolder="unet", revision=self.cfgs.model.revision
+        )
+        # import correct text encoder class
+        text_encoder_cls = import_text_encoder_class(self.cfgs.model.pretrained_model_name_or_path, self.cfgs.model.revision)
+        self.text_encoder = text_encoder_cls.from_pretrained(
+            self.cfgs.model.pretrained_model_name_or_path, subfolder="text_encoder", revision=self.cfgs.model.revision
+        )
+
+        if self.train_TE:
+            # Wrap unet and text_encoder to make DDP happy. Multiple DDP has soooooo many fxxking bugs!
+            self.TE_unet = TEUnetWrapper(self.unet, self.text_encoder)
+
+    def build_ema(self):
+        if self.cfgs.model.ema_unet>0:
+            self.ema_unet = ModelEMA(self.unet.named_parameters(), self.cfgs.model.ema_unet)
+        if self.train_TE and self.cfgs.model.ema_text_encoder>0:
+            self.ema_text_encoder = ModelEMA(self.text_encoder.named_parameters(), self.cfgs.model.ema_text_encoder)
+
+    def build_ckpt_manager(self):
+        if self.cfgs.ckpt_type == 'torch':
+            self.ckpt_manager = CkptManagerPKL()
+        elif self.cfgs.ckpt_type == 'safetensors':
+            self.ckpt_manager = CkptManagerSafe()
+        else:
+            raise NotImplementedError(f'Not support ckpt type: {self.cfgs.ckpt_type}')
+        if self.is_local_main_process:
+            self.ckpt_manager.set_save_dir(os.path.join(self.exp_dir, 'ckpts'), emb_dir=self.cfgs.tokenizer_pt.emb_dir)
+
+    @property
+    def unet_raw(self):
+        return self.TE_unet.module.unet if self.train_TE else self.unet.module
+
+    @property
+    def text_encoder_raw(self):
+        return self.TE_unet.module.TE if self.train_TE else self.text_encoder
+
+    def config_model(self):
+        if self.cfgs.model.enable_xformers:
+            if is_xformers_available():
+                self.unet.enable_xformers_memory_efficient_attention()
+                # self.text_enc_hook.enable_xformers()
+            else:
+                raise ValueError("xformers is not available. Make sure it is installed correctly")
+
+        self.vae.requires_grad_(False)
+        self.unet.requires_grad_(False)
+        self.text_encoder.requires_grad_(False)
+
+        self.unet.eval()
+        self.text_encoder.eval()
+
+        if self.cfgs.model.gradient_checkpointing:
+            self.unet.enable_gradient_checkpointing()
+            if self.train_TE:
+                self.text_encoder.gradient_checkpointing_enable()
+
+        weight_dtype = torch.float32
+        if self.cfgs.mixed_precision == "fp16":
+            weight_dtype = torch.float16
+        elif self.cfgs.mixed_precision == "bf16":
+            weight_dtype = torch.bfloat16
+        self.weight_dtype = weight_dtype
+
+        # Move vae and text_encoder to device and cast to weight_dtype
+        self.vae = self.vae.to(self.device, dtype=weight_dtype)
+        if not self.train_TE:
+            self.text_encoder = self.text_encoder.to(self.device, dtype=weight_dtype)
+
+    @torch.no_grad()
+    def load_resume(self):
+        if self.cfgs.train.resume is not None:
+            for ckpt in self.cfgs.train.resume.ckpt_path.unet:
+                self.ckpt_manager.load_ckpt_to_model(self.unet, ckpt, model_ema=getattr(self, 'ema_unet', None))
+            for ckpt in self.cfgs.train.resume.ckpt_path.TE:
+                self.ckpt_manager.load_ckpt_to_model(self.text_encoder, ckpt, model_ema=getattr(self, 'ema_text_encoder', None))
+            for name, ckpt in self.cfgs.train.resume.ckpt_path.words:
+                self.ex_words_emb[name].data = load_emb(ckpt)
+
+    def make_hooks(self):
+        # Hook tokenizer and embedding to support pt
+        self.embedding_hook, self.ex_words_emb = EmbeddingPTHook.hook_from_dir(
+            self.cfgs.tokenizer_pt.emb_dir, self.tokenizer, self.text_encoder, log=self.is_local_main_process,
+            N_repeats=self.cfgs.model.tokenizer_repeats, device=self.device)
+
+        self.text_enc_hook = TEEXHook(self.text_encoder, self.tokenizer, N_repeats=self.cfgs.model.tokenizer_repeats, device=self.device,
+                                      clip_skip=self.cfgs.model.clip_skip)
+
+    def build_data(self, data_builder: partial) -> torch.utils.data.DataLoader:
+        batch_size = data_builder.keywords.pop('batch_size')
+        cache_latents = data_builder.keywords.pop('cache_latents')
+        self.batch_size_list.append(batch_size)
+
+        train_dataset = data_builder(tokenizer=self.tokenizer, tokenizer_repeats=self.cfgs.model.tokenizer_repeats)
+        train_dataset.bucket.build(batch_size*self.world_size,
+                                   img_root_list=[source.img_root for source in data_builder.keywords['source'].values()])
+        arb = isinstance(train_dataset.bucket, RatioBucket)
+        self.loggers.info(f"len(train_dataset): {len(train_dataset)}")
+
+        if cache_latents:
+            self.cache_latents = True
+            train_dataset.cache_latents(self.vae, self.weight_dtype, self.device, show_prog=self.is_local_main_process)
+
+        # Pytorch Data loader
+        train_sampler = torch.utils.data.distributed.DistributedSampler(train_dataset, num_replicas=self.world_size,
+                                                                        rank=self.local_rank, shuffle=not arb)
+        train_loader = torch.utils.data.DataLoader(train_dataset, batch_size=batch_size,
+                                                   num_workers=self.cfgs.train.workers, sampler=train_sampler, collate_fn=collate_fn_ft)
+        return train_loader
+
+    def get_param_group_train(self):
+        # make miniFT and warp with lora
+        self.DA_lora = False
+        train_params_unet, self.lora_unet = make_hcpdiff(self.unet, self.cfgs.unet, self.cfgs.lora_unet)
+        if isinstance(self.lora_unet, tuple):  # creat negative lora
+            self.DA_lora = True
+            self.lora_unet, self.lora_unet_neg = self.lora_unet
+        train_params_unet_plugin, self.all_plugin_unet = make_plugin(self.unet, self.cfgs.plugin_unet)
+        train_params_unet += train_params_unet_plugin
+
+        if self.train_TE:
+            train_params_text_encoder, self.lora_TE = make_hcpdiff(self.text_encoder, self.cfgs.text_encoder, self.cfgs.lora_text_encoder)
+            if isinstance(self.lora_TE, tuple):  # creat negative lora
+                self.DA_lora = True
+                self.lora_TE, self.lora_TE_neg = self.lora_TE
+            train_params_TE_plugin, self.all_plugin_TE = make_plugin(self.text_encoder, self.cfgs.plugin_TE)
+            train_params_text_encoder += train_params_TE_plugin
+        else:
+            train_params_text_encoder = []
+
+        # params for embedding
+        train_params_emb = []
+        self.train_pts = {}
+        if self.cfgs.tokenizer_pt.train is not None:
+            for v in self.cfgs.tokenizer_pt.train:
+                self.train_pts[v.name] = self.ex_words_emb[v.name]
+                self.ex_words_emb[v.name].requires_grad = True
+                self.embedding_hook.emb_train.append(self.ex_words_emb[v.name])
+                train_params_emb.append({'params':self.ex_words_emb[v.name], 'lr':v.lr})
+
+        return train_params_unet+train_params_text_encoder, train_params_emb
+
+    def build_optimizer_scheduler(self):
+        # set optimizer
+        parameters, parameters_pt = self.get_param_group_train()
+
+        cfg_opt = self.cfgs.train.optimizer
+        if len(parameters)>0:  # do fine-tuning
+            if self.cfgs.train.scale_lr:
+                self.scale_lr(parameters)
+
+            if cfg_opt.type == 'adamw_8bit':
+                import bitsandbytes as bnb
+                self.optimizer = bnb.optim.AdamW8bit(params=parameters, lr=self.lr, weight_decay=cfg_opt.weight_decay)
+            elif cfg_opt.type == 'deepspeed' and self.accelerator.state.deepspeed_plugin is not None:
+                from deepspeed.ops.adam import FusedAdam
+                self.optimizer = FusedAdam(params=parameters, lr=self.lr, weight_decay=cfg_opt.weight_decay)
+            elif cfg_opt.type == 'adamw':
+                self.optimizer = torch.optim.AdamW(params=parameters, lr=self.lr, weight_decay=cfg_opt.weight_decay)
+            else:
+                self.optimizer = cfg_opt.optimizer.opt(parameters, lr=self.lr)
+
+            self.lr_scheduler = get_scheduler(optimizer=self.optimizer, **self.cfgs.train.scheduler)
+
+        if len(parameters_pt)>0:  # do prompt-tuning
+            if self.cfgs.train.scale_lr_pt:
+                self.scale_lr(parameters_pt)
+
+            self.optimizer_pt = torch.optim.AdamW(params=parameters_pt, lr=self.lr, weight_decay=cfg_opt.weight_decay_pt)
+            self.lr_scheduler_pt = get_scheduler(optimizer=self.optimizer_pt, **self.cfgs.train.scheduler_pt)
+
+    def train(self):
+        total_batch_size = sum(self.batch_size_list)*self.world_size*self.cfgs.train.gradient_accumulation_steps
+
+        self.loggers.info("***** Running training *****")
+        self.loggers.info(f"  Num batches each epoch = {len(self.train_loader_group.loader_list[0])}")
+        self.loggers.info(f"  Num Steps = {self.cfgs.train.scheduler.num_training_steps}")
+        self.loggers.info(f"  Instantaneous batch size per device = {sum(self.batch_size_list)}")
+        self.loggers.info(f"  Total train batch size (w. parallel, distributed & accumulation) = {total_batch_size}")
+        self.loggers.info(f"  Gradient Accumulation steps = {self.cfgs.train.gradient_accumulation_steps}")
+        self.global_step = 0
+        if self.cfgs.train.resume is not None:
+            self.global_step = self.cfgs.train.resume.start_step
+
+        loss_sum = np.ones(30)
+        for data_list in self.train_loader_group:
+            loss = self.train_one_step(data_list)
+            loss_sum[self.global_step%len(loss_sum)] = loss
+
+            self.global_step += 1
+            if self.is_local_main_process:
+                if self.global_step%self.cfgs.train.save_step == 0:
+                    self.save_model()
+                if self.global_step%self.min_log_step == 0:
+                    lr_model = self.lr_scheduler.get_last_lr()[0] if hasattr(self, 'lr_scheduler') else 0.
+                    lr_word = self.lr_scheduler_pt.get_last_lr()[0] if hasattr(self, 'lr_scheduler_pt') else 0.
+                    self.loggers.log(datas={
+                        'Step':{'format':'[{}/{}]', 'data':[self.global_step, self.cfgs.train.scheduler.num_training_steps]},
+                        'LR_model':{'format':'{:.2e}', 'data':[lr_model]},
+                        'LR_word':{'format':'{:.2e}', 'data':[lr_word]},
+                        'Loss':{'format':'{:.5f}', 'data':[loss_sum.mean()]},
+                    }, step=self.global_step)
+
+            if self.global_step>=self.cfgs.train.scheduler.num_training_steps:
+                break
+
+        self.wait_for_everyone()
+        if self.is_local_main_process:
+            self.save_model()
+
+    def wait_for_everyone(self):
+        self.accelerator.wait_for_everyone()
+
+    @torch.no_grad()
+    def get_latents(self, image, dataset):
+        if dataset.latents is None:
+            latents = self.vae.encode(image).latent_dist.sample()
+            latents = latents*0.18215
+        else:
+            latents = image  # Cached latents
+        return latents
+
+    def make_noise(self, latents):
+        # Sample noise that we'll add to the latents
+        noise = torch.randn_like(latents)
+        bsz = latents.shape[0]
+        # Sample a random timestep for each image
+        timesteps = torch.randint(0, self.noise_scheduler.config.num_train_timesteps, (bsz,), device=latents.device)
+        timesteps = timesteps.long()
+
+        # Add noise to the latents according to the noise magnitude at each timestep
+        # (this is the forward diffusion process)
+        return self.noise_scheduler.add_noise(latents, noise, timesteps), noise, timesteps
+
+    def encode_decode(self, prompt_ids, noisy_latents, timesteps, **kwargs):
+        # for DDP support
+        if self.train_TE:
+            model_pred = self.TE_unet(prompt_ids, noisy_latents, timesteps, **kwargs)
+        else:
+            input_all = dict(prompt_ids=prompt_ids, noisy_latents=noisy_latents, timesteps=timesteps, **kwargs)
+            if hasattr(self.text_encoder, 'input_feeder'):
+                for feeder in self.text_encoder.input_feeder:
+                    feeder(input_all)
+            if hasattr(self.unet_raw, 'input_feeder'):
+                for feeder in self.unet_raw.input_feeder:
+                    feeder(input_all)
+
+            encoder_hidden_states = self.text_encoder(prompt_ids, output_hidden_states=True)  # Get the text embedding for conditioning
+            model_pred = self.unet(noisy_latents, timesteps, encoder_hidden_states).sample  # Predict the noise residual
+        return model_pred
+
+    def forward(self, latents, prompt_ids, **kwargs):
+        noisy_latents, noise, timesteps = self.make_noise(latents)
+
+        # CFG context for DreamArtist
+        noisy_latents, timesteps = self.cfg_context.pre(noisy_latents, timesteps)
+        model_pred = self.encode_decode(prompt_ids, noisy_latents, timesteps, **kwargs)
+        model_pred = self.cfg_context.post(model_pred)
+
+        # Get the target for loss depending on the prediction type
+        if self.cfgs.train.loss.type == "eps":
+            target = noise
+        elif self.cfgs.train.loss.type == "sample":
+            target = self.noise_scheduler.step(noise, timesteps, noisy_latents)
+            model_pred = self.noise_scheduler.step(model_pred, timesteps, noisy_latents)
+        else:
+            raise ValueError(f"Unknown loss type {self.cfgs.train.loss.type}")
+        return model_pred, target, timesteps
+
+    def train_one_step(self, data_list):
+        with self.accelerator.accumulate(self.unet):
+            for idx, data in enumerate(data_list):
+                image = data.pop('img').to(self.device, dtype=self.weight_dtype)
+                att_mask = data.pop('mask').to(self.device)
+                prompt_ids = data.pop('prompt').to(self.device)
+                other_datas = {k:v.to(self.device, dtype=self.weight_dtype) for k, v in data.items()}
+
+                latents = self.get_latents(image, self.train_loader_group.get_dataset(idx))
+                model_pred, target, timesteps = self.forward(latents, prompt_ids, **other_datas)
+                loss = self.get_loss(model_pred, target, timesteps, att_mask) * self.train_loader_group.get_loss_weights(idx)
+                self.accelerator.backward(loss)
+
+            if hasattr(self, 'optimizer'):
+                if self.accelerator.sync_gradients:  # fine-tuning
+                    params_to_clip = (
+                        itertools.chain(self.unet.parameters(), self.text_encoder.parameters())
+                        if self.train_TE else self.unet.parameters()
+                    )
+                    self.accelerator.clip_grad_norm_(params_to_clip, self.cfgs.train.max_grad_norm)
+                self.optimizer.step()
+                self.lr_scheduler.step()
+                self.optimizer.zero_grad(set_to_none=self.cfgs.train.set_grads_to_none)
+
+            if hasattr(self, 'optimizer_pt'):  # prompt tuning
+                self.optimizer_pt.step()
+                self.lr_scheduler_pt.step()
+                self.optimizer_pt.zero_grad(set_to_none=self.cfgs.train.set_grads_to_none)
+
+            self.update_ema()
+        return loss.item()
+
+    def get_loss(self, model_pred, target, timesteps, att_mask):
+        if len(self.embedding_hook.emb_train)>0:
+            return (self.criterion(model_pred.float(), target.float(), timesteps)*att_mask).mean() \
+                   +0*sum(self.embedding_hook.emb_train).mean()  # avoid unused parameters, make gradient checkpointing happy
+        else:
+            return (self.criterion(model_pred.float(), target.float(), timesteps)*att_mask).mean()
+
+    def update_ema(self):
+        if hasattr(self, 'ema_unet'):
+            self.ema_unet.step(self.unet_raw.named_parameters())
+        if hasattr(self, 'ema_text_encoder'):
+            self.ema_text_encoder.step(self.text_encoder_raw.named_parameters())
+
+    def save_model(self, from_raw=False):
+        unet_raw = self.unet_raw
+        self.ckpt_manager.save_model_with_lora(unet_raw, self.lora_unet, model_ema=getattr(self, 'ema_unet', None),
+                                               name='unet', step=self.global_step)
+        self.ckpt_manager.save_plugins(unet_raw, self.all_plugin_unet, name='unet', step=self.global_step,
+                                       model_ema=getattr(self, 'ema_unet', None))
+        if self.train_TE:
+            TE_raw = self.text_encoder_raw
+            # exclude_key: embeddings should not save with text-encoder
+            self.ckpt_manager.save_model_with_lora(TE_raw, self.lora_TE, model_ema=getattr(self, 'ema_text_encoder', None),
+                                                   name='text_encoder', step=self.global_step, exclude_key='emb_ex.')
+            self.ckpt_manager.save_plugins(TE_raw, self.all_plugin_TE, name='text_encoder', step=self.global_step,
+                                           model_ema=getattr(self, 'ema_text_encoder', None))
+
+        if self.DA_lora:
+            self.ckpt_manager.save_model_with_lora(None, self.lora_unet_neg, name='unet-neg', step=self.global_step)
+            if self.train_TE:
+                self.ckpt_manager.save_model_with_lora(None, self.lora_TE_neg, name='text_encoder-neg', step=self.global_step)
+
+        self.ckpt_manager.save_embedding(self.train_pts, self.global_step, self.cfgs.tokenizer_pt.replace)
+
+        self.loggers.info(f"Saved state, step: {self.global_step}")
+
+    def make_vis(self):
+        vis_dir = os.path.join(self.exp_dir, f'vis-{self.global_step}')
+        new_components = {
+            'unet':self.unet_raw,
+            'text_encoder':self.text_encoder_raw,
+            'tokenizer':self.tokenizer,
+            'vae':self.vae,
+        }
+        viser = Visualizer(self.cfgs.model.pretrained_model_name_or_path, new_components=new_components)
+        if self.cfgs.vis_info.prompt:
+            raise ValueError('vis_info.prompt is None. cannot generate without prompt.')
+        viser.vis_to_dir(vis_dir, self.cfgs.vis_prompt)
+
+if __name__ == '__main__':
+    parser = argparse.ArgumentParser(description='Stable Diffusion Training')
+    parser.add_argument('--cfg', type=str, default=None, required=True)
+    args, _ = parser.parse_known_args()
+
+    conf = load_config_with_cli(args.cfg, args_list=sys.argv[3:])  # skip --cfg
+    trainer = Trainer(conf)
+    trainer.train()
```

### Comparing `hcpdiff-0.2.2/hcpdiff/train_ac_single.py` & `hcpdiff-0.3.0/hcpdiff/train_ac_single.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,98 +1,110 @@
-import argparse
-import sys
-import torch
-from loguru import logger
-from functools import partial
-
-from accelerate import Accelerator
-from hcpdiff.train_ac import Trainer, RatioBucket, load_config_with_cli, set_seed
-from hcpdiff.data import collate_fn_ft
-
-class TrainerSingleCard(Trainer):
-    def init_context(self, cfgs_raw):
-        self.accelerator = Accelerator(
-            gradient_accumulation_steps=self.cfgs.train.gradient_accumulation_steps,
-            mixed_precision=self.cfgs.mixed_precision,
-            step_scheduler_with_optimizer=False,
-        )
-
-        self.local_rank = 0
-        self.world_size = self.accelerator.num_processes
-
-        set_seed(self.cfgs.seed + self.local_rank)
-
-    def prepare(self):
-        # Prepare everything with accelerator.
-        prepare_obj_list = [self.unet, self.train_loader]
-        prepare_name_list = ['unet', 'train_loader']
-        if hasattr(self, 'optimizer'):
-            prepare_obj_list.extend([self.optimizer, self.lr_scheduler])
-            prepare_name_list.extend(['optimizer', 'lr_scheduler'])
-        if hasattr(self, 'optimizer_pt'):
-            prepare_obj_list.extend([self.optimizer_pt, self.lr_scheduler_pt])
-            prepare_name_list.extend(['optimizer_pt', 'lr_scheduler_pt'])
-        if self.train_TE:
-            prepare_obj_list.append(self.text_encoder)
-            prepare_name_list.append('text_encoder')
-
-        prepared_obj = self.accelerator.prepare(*prepare_obj_list)
-        for name, obj in zip(prepare_name_list, prepared_obj):
-            setattr(self, name, obj)
-
-    def build_data(self, data_builder:partial) -> torch.utils.data.DataLoader:
-        batch_size = data_builder.keywords.pop('batch_size')
-        cache_latents = data_builder.keywords.pop('cache_latents')
-        self.batch_size_list.append(batch_size)
-
-        train_dataset = data_builder(tokenizer=self.tokenizer, tokenizer_repeats=self.cfgs.model.tokenizer_repeats)
-        train_dataset.bucket.build(batch_size * self.world_size)
-        arb = isinstance(train_dataset.bucket, RatioBucket)
-        logger.info(f"len(train_dataset): {len(train_dataset)}")
-
-        if cache_latents:
-            self.cache_latents = True
-            train_dataset.cache_latents(self.vae, self.weight_dtype, self.device, show_prog=self.is_local_main_process)
-
-        # Pytorch Data loader
-        train_loader = torch.utils.data.DataLoader(train_dataset, batch_size=batch_size,
-            num_workers=self.cfgs.train.workers, shuffle=not arb, collate_fn=collate_fn_ft)
-        return train_loader
-
-    def encode_decode(self, prompt_ids, noisy_latents, timesteps, **kwargs):
-        input_all = dict(prompt_ids=prompt_ids, noisy_latents=noisy_latents, timesteps=timesteps, **kwargs)
-        if hasattr(self.text_encoder, 'input_feeder'):
-            for feeder in self.text_encoder.input_feeder:
-                feeder(input_all)
-        if hasattr(self.unet_raw, 'input_feeder'):
-            for feeder in self.unet_raw.input_feeder:
-                feeder(input_all)
-
-        encoder_hidden_states = self.text_encoder(prompt_ids, output_hidden_states=True)  # Get the text embedding for conditioning
-        model_pred = self.unet(noisy_latents, timesteps, encoder_hidden_states).sample  # Predict the noise residual
-        return model_pred
-
-    def get_loss(self, model_pred, target, att_mask):
-        return (self.criterion(model_pred.float(), target.float()) * att_mask).mean()
-
-    def update_ema(self):
-        if hasattr(self, 'ema_unet'):
-            self.ema_unet.step(self.unet.named_parameters())
-        if hasattr(self, 'ema_text_encoder'):
-            self.ema_text_encoder.step(self.text_encoder.named_parameters())
-
-    @property
-    def unet_raw(self):
-        return self.unet
-
-    @property
-    def text_encoder_raw(self):
-        return self.text_encoder
-
-if __name__ == '__main__':
-    parser = argparse.ArgumentParser(description='Stable Diffusion Training')
-    parser.add_argument('--cfg', type=str, default='cfg/train/demo.yaml')
-    args, _ = parser.parse_known_args()
-
-    conf = load_config_with_cli(args.cfg, args_list=sys.argv[3:]) # skip --cfg
-    trainer=TrainerSingleCard(conf)
+import argparse
+import sys
+import torch
+from loguru import logger
+from functools import partial
+
+from accelerate import Accelerator
+from hcpdiff.train_ac import Trainer, RatioBucket, load_config_with_cli, set_seed
+from hcpdiff.data import collate_fn_ft
+
+class TrainerSingleCard(Trainer):
+    def init_context(self, cfgs_raw):
+        self.accelerator = Accelerator(
+            gradient_accumulation_steps=self.cfgs.train.gradient_accumulation_steps,
+            mixed_precision=self.cfgs.mixed_precision,
+            step_scheduler_with_optimizer=False,
+        )
+
+        self.local_rank = 0
+        self.world_size = self.accelerator.num_processes
+
+        set_seed(self.cfgs.seed + self.local_rank)
+
+    def prepare(self):
+        # try:
+        #     self.unet = torch.compile(self.unet)
+        #     self.text_encoder = torch.compile(self.text_encoder)
+        # except:
+        #     print('cannot compile model')
+
+        # Prepare everything with accelerator.
+        prepare_obj_list = [self.unet]
+        prepare_name_list = ['unet']
+        if hasattr(self, 'optimizer'):
+            prepare_obj_list.extend([self.optimizer, self.lr_scheduler])
+            prepare_name_list.extend(['optimizer', 'lr_scheduler'])
+        if hasattr(self, 'optimizer_pt'):
+            prepare_obj_list.extend([self.optimizer_pt, self.lr_scheduler_pt])
+            prepare_name_list.extend(['optimizer_pt', 'lr_scheduler_pt'])
+        if self.train_TE:
+            prepare_obj_list.append(self.text_encoder)
+            prepare_name_list.append('text_encoder')
+
+        prepared_obj = self.accelerator.prepare(*prepare_obj_list)
+        for name, obj in zip(prepare_name_list, prepared_obj):
+            setattr(self, name, obj)
+
+        if len(self.train_loader_group)>1:
+            self.train_loader_group.loader_list = list(self.accelerator.prepare(*self.train_loader_group.loader_list))
+        else:
+            self.train_loader_group.loader_list = [self.accelerator.prepare(*self.train_loader_group.loader_list)]
+
+    def build_data(self, data_builder:partial) -> torch.utils.data.DataLoader:
+        batch_size = data_builder.keywords.pop('batch_size')
+        cache_latents = data_builder.keywords.pop('cache_latents')
+        self.batch_size_list.append(batch_size)
+
+        train_dataset = data_builder(tokenizer=self.tokenizer, tokenizer_repeats=self.cfgs.model.tokenizer_repeats)
+        train_dataset.bucket.build(batch_size * self.world_size,
+                                   img_root_list=[source.img_root for source in data_builder.keywords['source'].values()])
+        arb = isinstance(train_dataset.bucket, RatioBucket)
+        logger.info(f"len(train_dataset): {len(train_dataset)}")
+
+        if cache_latents:
+            self.cache_latents = True
+            train_dataset.cache_latents(self.vae, self.weight_dtype, self.device, show_prog=self.is_local_main_process)
+
+        # Pytorch Data loader
+        train_loader = torch.utils.data.DataLoader(train_dataset, batch_size=batch_size,
+            num_workers=self.cfgs.train.workers, shuffle=not arb, collate_fn=collate_fn_ft)
+        return train_loader
+
+    def encode_decode(self, prompt_ids, noisy_latents, timesteps, **kwargs):
+        input_all = dict(prompt_ids=prompt_ids, noisy_latents=noisy_latents, timesteps=timesteps, **kwargs)
+        if hasattr(self.text_encoder, 'input_feeder'):
+            for feeder in self.text_encoder.input_feeder:
+                feeder(input_all)
+        if hasattr(self.unet_raw, 'input_feeder'):
+            for feeder in self.unet_raw.input_feeder:
+                feeder(input_all)
+
+        encoder_hidden_states = self.text_encoder(prompt_ids, output_hidden_states=True)  # Get the text embedding for conditioning
+        model_pred = self.unet(noisy_latents, timesteps, encoder_hidden_states).sample  # Predict the noise residual
+        return model_pred
+
+    def get_loss(self, model_pred, target, timesteps, att_mask):
+        return (self.criterion(model_pred.float(), target.float(), timesteps) * att_mask).mean()
+
+    def update_ema(self):
+        if hasattr(self, 'ema_unet'):
+            self.ema_unet.step(self.unet.named_parameters())
+        if hasattr(self, 'ema_text_encoder'):
+            self.ema_text_encoder.step(self.text_encoder.named_parameters())
+
+    @property
+    def unet_raw(self):
+        return self.unet
+
+    @property
+    def text_encoder_raw(self):
+        return self.text_encoder
+
+if __name__ == '__main__':
+    parser = argparse.ArgumentParser(description='Stable Diffusion Training')
+    parser.add_argument('--cfg', type=str, default='cfg/train/demo.yaml')
+    args, _ = parser.parse_known_args()
+
+    conf = load_config_with_cli(args.cfg, args_list=sys.argv[3:]) # skip --cfg
+    trainer=TrainerSingleCard(conf)
     trainer.train()
```

### Comparing `hcpdiff-0.2.2/hcpdiff/train_colo.py` & `hcpdiff-0.3.0/hcpdiff/train_colo.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,235 +1,223 @@
-"""
-train_colo.py
-====================
-    :Name:        train with colossal-AI
-    :Author:      Dong Ziyi
-    :Affiliation: HCP Lab, SYSU
-    :Created:     10/03/2023
-    :Licence:     Apache-2.0
-"""
-
-import argparse
-import sys
-import torch
-from torch import nn
-
-import colossalai
-import colossalai.tensor
-from colossalai.context.parallel_mode import ParallelMode
-from colossalai.core import global_context as gpc
-from colossalai.nn.parallel.utils import get_static_torch_model
-from colossalai.utils import get_current_device
-from colossalai.utils.model.colo_init_context import ColoInitContext
-from colossalai.utils.model.colo_init_context import _convert_to_coloparam
-from colossalai.tensor import ColoParameter
-
-from hcpdiff.train_ac import Trainer, get_scheduler, ModelEMA
-from diffusers import UNet2DConditionModel
-from hcpdiff.utils.colo_utils import gemini_zero_dpp, GeminiAdamOptimizerP
-from hcpdiff.utils.utils import load_config_with_cli
-from hcpdiff.utils.net_utils import import_text_encoder_class, TEUnetWrapper
-
-class TrainerColo(Trainer):
-    def init_context(self, cfgs_raw):
-        # If passed along, set the training seed now.
-        if self.cfgs.seed is None:
-            colossalai.launch_from_torch(config='./config.py')
-        else:
-            # set_seed(args.seed)
-            colossalai.launch_from_torch(config='./config.py', seed=self.cfgs.seed)
-
-        self.local_rank = gpc.get_local_rank(ParallelMode.DATA)
-        self.world_size = gpc.get_world_size(ParallelMode.DATA)
-
-    @property
-    def device(self):
-        return get_current_device()
-
-    @property
-    def is_local_main_process(self):
-        return self.local_rank in [0,-1]
-
-    def prepare(self):
-        pass
-
-    def wait_for_everyone(self):
-        torch.cuda.synchronize()
-
-    def build_unet_and_TE(self):
-        # import correct text encoder class
-        text_encoder_cls = import_text_encoder_class(self.cfgs.model.pretrained_model_name_or_path,
-                                                     self.cfgs.model.revision)
-        with ColoInitContext(device=self.device):
-            self.unet = UNet2DConditionModel.from_pretrained(
-                self.cfgs.model.pretrained_model_name_or_path, subfolder="unet", revision=self.cfgs.model.revision,
-                low_cpu_mem_usage=False
-            )
-            if self.train_TE:
-                self.text_encoder = text_encoder_cls.from_pretrained(
-                    self.cfgs.model.pretrained_model_name_or_path, subfolder="text_encoder", revision=self.cfgs.model.revision
-                )
-                self.TE_unet = TEUnetWrapper(self.unet, self.text_encoder)
-        if not self.train_TE:
-            self.text_encoder = text_encoder_cls.from_pretrained(
-                self.cfgs.model.pretrained_model_name_or_path, subfolder="text_encoder", revision=self.cfgs.model.revision
-            )
-
-    def build_ema(self):
-        if self.cfgs.model.ema_unet>0:
-            self.ema_unet = ModelEMA(get_static_torch_model(self.unet).named_parameters(), self.cfgs.model.ema_unet)
-        if self.train_TE and self.cfgs.model.ema_text_encoder>0:
-            self.ema_text_encoder = ModelEMA(self.text_encoder.named_parameters(), self.cfgs.model.ema_text_encoder)
-
-    def convert_emb_param(self, cinit):
-        name_list = []
-        for name, param in self.embedding_hook.named_parameters():
-            if type(param) is ColoParameter:
-                continue
-
-            split = name.rfind('.')
-            if split >= 0:  # param in submodule
-                module_name = name[:split]
-                param_name = name[split + 1:]
-            else:
-                module_name = ''  # param in current module
-                param_name = name
-            name_list.append((module_name, param_name))
-
-        replaced_tensors = dict(
-        )  # record mapping between (torch.Tensor, ColoTensor) to distinguish the same reference
-        for module_name, param_name in name_list:
-            submodule = self.embedding_hook.get_submodule(module_name)
-            param = submodule.get_parameter(param_name)
-            if param in replaced_tensors:
-                colo_param = replaced_tensors[param]
-            else:
-                colo_param = _convert_to_coloparam(param, cinit._device, cinit._dtype, cinit._default_pg,
-                                                   cinit._default_dist_spec)
-                replaced_tensors[param] = colo_param
-            delattr(submodule, param_name)
-            setattr(submodule, param_name, colo_param)
-            colo_param.shared_param_modules.append(submodule)
-
-    def get_param_group_train(self):
-        with ColoInitContext(device=self.device) as cinit:
-            params = super().get_param_group_train()
-            self.convert_emb_param(cinit)
-
-        self.lora_unet.set_inplace(False)
-        if self.DA_lora:
-            self.lora_unet_neg.set_inplace(False)
-        if self.train_TE:
-            self.lora_TE.set_inplace(False)
-            if self.DA_lora:
-                self.lora_TE_neg.set_inplace(False)
-            self.TE_unet = gemini_zero_dpp(self.TE_unet)
-        else:
-            self.unet = gemini_zero_dpp(self.unet)
-        return params
-
-    def build_optimizer_scheduler(self):
-        # set optimizer
-        parameters, parameters_pt = self.get_param_group_train()
-
-        cfg_opt = self.cfgs.train.optimizer
-        if len(parameters)>0: # do fine-tuning
-            if self.cfgs.train.scale_lr:
-                self.scale_lr(parameters)
-            self.optimizer = GeminiAdamOptimizerP(self.TE_unet if self.train_TE else self.unet, parameters, lr=self.lr,
-                                                  initial_scale=2 ** 5, clipping_norm=self.cfgs.train.max_grad_norm)
-
-            self.lr_scheduler = get_scheduler(optimizer=self.optimizer, **self.cfgs.train.scheduler)
-
-        if len(parameters_pt)>0: # do prompt-tuning
-            if self.cfgs.train.scale_lr_pt:
-                self.scale_lr(parameters_pt)
-
-            self.optimizer_pt = torch.optim.AdamW(params=parameters_pt, lr=self.lr, weight_decay=cfg_opt.weight_decay_pt)
-            self.lr_scheduler_pt = get_scheduler(optimizer=self.optimizer_pt, **self.cfgs.train.scheduler_pt)
-
-    def train_one_step(self, data, prompt_ids):
-        torch.cuda.reset_peak_memory_stats()
-        image = data['img'].to(self.device, dtype=self.weight_dtype, non_blocking=True)
-        att_mask = data['mask'].to(self.device, non_blocking=True)
-        prompt_ids = prompt_ids.to(self.device, non_blocking=True)
-        other_datas = {k: v.to(self.device, dtype=self.weight_dtype, non_blocking=True) for k, v in data.items() if k != 'img' and k != 'mask'}
-
-        latents = self.get_latents(image, self.train_loader.dataset)
-        model_pred, target = self.forward(latents, prompt_ids, **other_datas)
-
-        if self.train_loader_class is not None:
-            # DreamBooth prior forward
-            data_cls, prompt_ids_cls = next(self.data_iter_class)
-            image_cls = data_cls['img'].to(self.device, dtype=self.weight_dtype, non_blocking=True)
-            att_mask_cls = data_cls['mask'].to(self.device, non_blocking=True)
-            prompt_ids_cls = prompt_ids_cls.to(self.device, non_blocking=True)
-            other_datas_cls = {k: v.to(self.device, dtype=self.weight_dtype, non_blocking=True) for k, v in data_cls.items() if k != 'img' and k != 'mask'}
-            latents_cls = self.get_latents(image_cls, self.train_loader_class.dataset)
-            model_pred_prior, target_prior = self.forward(latents_cls, prompt_ids_cls, **other_datas_cls)
-
-            loss = self.get_loss(model_pred, target, att_mask)  # Compute instance loss
-            prior_loss = self.get_loss(model_pred_prior, target_prior, att_mask_cls)  # Compute prior loss
-            loss = loss + self.cfgs.train.loss.prior_loss_weight * prior_loss
-        else:
-            loss = self.get_loss(model_pred, target, att_mask)
-
-        if hasattr(self, 'optimizer'):
-            self.optimizer.backward(loss)
-        else:
-            loss.backward()
-
-        if hasattr(self, 'optimizer'):
-            self.optimizer.step()
-            self.lr_scheduler.step()
-            self.optimizer.zero_grad(set_to_none=self.cfgs.train.set_grads_to_none)
-
-        if hasattr(self, 'optimizer_pt'): # prompt tuning
-            self.optimizer_pt.step()
-            self.lr_scheduler_pt.step()
-            self.optimizer_pt.zero_grad(set_to_none=self.cfgs.train.set_grads_to_none)
-
-        self.update_ema()
-        return loss.item()
-
-    def update_ema(self):
-        if hasattr(self, 'ema_unet'):
-            self.ema_unet.step(get_static_torch_model(self.unet).named_parameters())
-        if hasattr(self, 'ema_text_encoder'):
-            self.ema_text_encoder.step(self.text_encoder.named_parameters())
-
-    @property
-    def unet_raw(self):
-        if self.train_TE:
-            unet = get_static_torch_model(self.TE_unet).unet
-        else:
-            unet = get_static_torch_model(self.unet)
-        req_grad_dict = {k:v.requires_grad for k,v in self.unet.named_parameters()}
-        for k,v in unet.named_parameters():
-            v.requires_grad = req_grad_dict[k]
-        return unet
-
-    @property
-    def text_encoder_raw(self):
-        if self.train_TE:
-            TE = get_static_torch_model(self.TE_unet).TE
-            req_grad_dict = {k: v.requires_grad for k, v in self.text_encoder.named_parameters()}
-            for k, v in TE.named_parameters():
-                v.requires_grad = req_grad_dict[k]
-        else:
-            TE = self.text_encoder
-        return TE
-
-    def save_model(self, from_raw=True):
-        super(TrainerColo, self).save_model(from_raw)
-
-
-if __name__ == '__main__':
-    parser = argparse.ArgumentParser(description='Stable Diffusion Training')
-    parser.add_argument('--cfg', type=str, default='cfg/train/demo.yaml')
-    parser.add_argument( "--placement", type=str, default="cpu",
-        help="Placement Policy for Gemini. Valid when using colossalai as dist plan.")
-    args, _ = parser.parse_known_args()
-
-    conf = load_config_with_cli(args.cfg, args_list=sys.argv[3:]) # skip --cfg
-    trainer=TrainerColo(conf)
+"""
+train_colo.py
+====================
+    :Name:        train with colossal-AI
+    :Author:      Dong Ziyi
+    :Affiliation: HCP Lab, SYSU
+    :Created:     10/03/2023
+    :Licence:     Apache-2.0
+"""
+
+import argparse
+import sys
+import torch
+from torch import nn
+
+import colossalai
+import colossalai.tensor
+from colossalai.context.parallel_mode import ParallelMode
+from colossalai.core import global_context as gpc
+from colossalai.nn.parallel.utils import get_static_torch_model
+from colossalai.utils import get_current_device
+from colossalai.utils.model.colo_init_context import ColoInitContext
+from colossalai.utils.model.colo_init_context import _convert_to_coloparam
+from colossalai.tensor import ColoParameter
+
+from hcpdiff.train_ac import Trainer, get_scheduler, ModelEMA
+from diffusers import UNet2DConditionModel
+from hcpdiff.utils.colo_utils import gemini_zero_dpp, GeminiAdamOptimizerP
+from hcpdiff.utils.utils import load_config_with_cli
+from hcpdiff.utils.net_utils import import_text_encoder_class, TEUnetWrapper
+
+class TrainerColo(Trainer):
+    def init_context(self, cfgs_raw):
+        # If passed along, set the training seed now.
+        if self.cfgs.seed is None:
+            colossalai.launch_from_torch(config='./config.py')
+        else:
+            # set_seed(args.seed)
+            colossalai.launch_from_torch(config='./config.py', seed=self.cfgs.seed)
+
+        self.local_rank = gpc.get_local_rank(ParallelMode.DATA)
+        self.world_size = gpc.get_world_size(ParallelMode.DATA)
+
+    @property
+    def device(self):
+        return get_current_device()
+
+    @property
+    def is_local_main_process(self):
+        return self.local_rank in [0,-1]
+
+    def prepare(self):
+        pass
+
+    def wait_for_everyone(self):
+        torch.cuda.synchronize()
+
+    def build_unet_and_TE(self):
+        # import correct text encoder class
+        text_encoder_cls = import_text_encoder_class(self.cfgs.model.pretrained_model_name_or_path,
+                                                     self.cfgs.model.revision)
+        with ColoInitContext(device=self.device):
+            self.unet = UNet2DConditionModel.from_pretrained(
+                self.cfgs.model.pretrained_model_name_or_path, subfolder="unet", revision=self.cfgs.model.revision,
+                low_cpu_mem_usage=False
+            )
+            if self.train_TE:
+                self.text_encoder = text_encoder_cls.from_pretrained(
+                    self.cfgs.model.pretrained_model_name_or_path, subfolder="text_encoder", revision=self.cfgs.model.revision
+                )
+                self.TE_unet = TEUnetWrapper(self.unet, self.text_encoder)
+        if not self.train_TE:
+            self.text_encoder = text_encoder_cls.from_pretrained(
+                self.cfgs.model.pretrained_model_name_or_path, subfolder="text_encoder", revision=self.cfgs.model.revision
+            )
+
+    def build_ema(self):
+        if self.cfgs.model.ema_unet>0:
+            self.ema_unet = ModelEMA(get_static_torch_model(self.unet).named_parameters(), self.cfgs.model.ema_unet)
+        if self.train_TE and self.cfgs.model.ema_text_encoder>0:
+            self.ema_text_encoder = ModelEMA(self.text_encoder.named_parameters(), self.cfgs.model.ema_text_encoder)
+
+    def convert_emb_param(self, cinit):
+        name_list = []
+        for name, param in self.embedding_hook.named_parameters():
+            if type(param) is ColoParameter:
+                continue
+
+            split = name.rfind('.')
+            if split >= 0:  # param in submodule
+                module_name = name[:split]
+                param_name = name[split + 1:]
+            else:
+                module_name = ''  # param in current module
+                param_name = name
+            name_list.append((module_name, param_name))
+
+        replaced_tensors = dict(
+        )  # record mapping between (torch.Tensor, ColoTensor) to distinguish the same reference
+        for module_name, param_name in name_list:
+            submodule = self.embedding_hook.get_submodule(module_name)
+            param = submodule.get_parameter(param_name)
+            if param in replaced_tensors:
+                colo_param = replaced_tensors[param]
+            else:
+                colo_param = _convert_to_coloparam(param, cinit._device, cinit._dtype, cinit._default_pg,
+                                                   cinit._default_dist_spec)
+                replaced_tensors[param] = colo_param
+            delattr(submodule, param_name)
+            setattr(submodule, param_name, colo_param)
+            colo_param.shared_param_modules.append(submodule)
+
+    def get_param_group_train(self):
+        with ColoInitContext(device=self.device) as cinit:
+            params = super().get_param_group_train()
+            self.convert_emb_param(cinit)
+
+        self.lora_unet.set_inplace(False)
+        if self.DA_lora:
+            self.lora_unet_neg.set_inplace(False)
+        if self.train_TE:
+            self.lora_TE.set_inplace(False)
+            if self.DA_lora:
+                self.lora_TE_neg.set_inplace(False)
+            self.TE_unet = gemini_zero_dpp(self.TE_unet)
+        else:
+            self.unet = gemini_zero_dpp(self.unet)
+        return params
+
+    def build_optimizer_scheduler(self):
+        # set optimizer
+        parameters, parameters_pt = self.get_param_group_train()
+
+        cfg_opt = self.cfgs.train.optimizer
+        if len(parameters)>0: # do fine-tuning
+            if self.cfgs.train.scale_lr:
+                self.scale_lr(parameters)
+            self.optimizer = GeminiAdamOptimizerP(self.TE_unet if self.train_TE else self.unet, parameters, lr=self.lr,
+                                                  initial_scale=2 ** 5, clipping_norm=self.cfgs.train.max_grad_norm)
+
+            self.lr_scheduler = get_scheduler(optimizer=self.optimizer, **self.cfgs.train.scheduler)
+
+        if len(parameters_pt)>0: # do prompt-tuning
+            if self.cfgs.train.scale_lr_pt:
+                self.scale_lr(parameters_pt)
+
+            self.optimizer_pt = torch.optim.AdamW(params=parameters_pt, lr=self.lr, weight_decay=cfg_opt.weight_decay_pt)
+            self.lr_scheduler_pt = get_scheduler(optimizer=self.optimizer_pt, **self.cfgs.train.scheduler_pt)
+
+    def train_one_step(self, data_list):
+        torch.cuda.reset_peak_memory_stats()
+        loss = []
+        for idx, data in enumerate(data_list):
+            image = data.pop('img').to(self.device, dtype=self.weight_dtype, non_blocking=True)
+            att_mask = data.pop('mask').to(self.device, non_blocking=True)
+            prompt_ids = data.pop('prompt').to(self.device, non_blocking=True)
+            other_datas = {k:v.to(self.device, dtype=self.weight_dtype, non_blocking=True) for k, v in data.items()}
+
+            latents = self.get_latents(image, self.train_loader_group.get_dataset(idx))
+            model_pred, target, timesteps = self.forward(latents, prompt_ids, **other_datas)
+            loss.append(self.get_loss(model_pred, target, timesteps, att_mask)*self.train_loader_group.get_loss_weights(idx))
+        loss = sum(loss)
+
+        if hasattr(self, 'optimizer'):
+            self.optimizer.backward(loss)
+        else:
+            loss.backward()
+
+        if hasattr(self, 'optimizer'):
+            self.optimizer.step()
+            self.lr_scheduler.step()
+            self.optimizer.zero_grad(set_to_none=self.cfgs.train.set_grads_to_none)
+
+        if hasattr(self, 'optimizer_pt'): # prompt tuning
+            self.optimizer_pt.step()
+            self.lr_scheduler_pt.step()
+            self.optimizer_pt.zero_grad(set_to_none=self.cfgs.train.set_grads_to_none)
+
+        self.update_ema()
+        return loss.item()
+
+    def update_ema(self):
+        if hasattr(self, 'ema_unet'):
+            self.ema_unet.step(get_static_torch_model(self.unet).named_parameters())
+        if hasattr(self, 'ema_text_encoder'):
+            self.ema_text_encoder.step(self.text_encoder.named_parameters())
+
+    @property
+    def unet_raw(self):
+        if self.train_TE:
+            unet = get_static_torch_model(self.TE_unet).unet
+        else:
+            unet = get_static_torch_model(self.unet)
+        req_grad_dict = {k:v.requires_grad for k,v in self.unet.named_parameters()}
+        for k,v in unet.named_parameters():
+            v.requires_grad = req_grad_dict[k]
+        return unet
+
+    @property
+    def text_encoder_raw(self):
+        if self.train_TE:
+            TE = get_static_torch_model(self.TE_unet).TE
+            req_grad_dict = {k: v.requires_grad for k, v in self.text_encoder.named_parameters()}
+            for k, v in TE.named_parameters():
+                v.requires_grad = req_grad_dict[k]
+        else:
+            TE = self.text_encoder
+        return TE
+
+    def save_model(self, from_raw=True):
+        super(TrainerColo, self).save_model(from_raw)
+
+
+if __name__ == '__main__':
+    parser = argparse.ArgumentParser(description='Stable Diffusion Training')
+    parser.add_argument('--cfg', type=str, default='cfg/train/demo.yaml')
+    parser.add_argument( "--placement", type=str, default="cpu",
+        help="Placement Policy for Gemini. Valid when using colossalai as dist plan.")
+    args, _ = parser.parse_known_args()
+
+    conf = load_config_with_cli(args.cfg, args_list=sys.argv[3:]) # skip --cfg
+    trainer=TrainerColo(conf)
     trainer.train()
```

### Comparing `hcpdiff-0.2.2/hcpdiff/utils/caption_tools.py` & `hcpdiff-0.3.0/hcpdiff/utils/caption_tools.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,87 +1,87 @@
-"""
-caption_tools.py
-====================
-    :Name:        process prompts
-    :Author:      Dong Ziyi
-    :Affiliation: HCP Lab, SYSU
-    :Created:     10/03/2023
-    :Licence:     Apache-2.0
-"""
-
-import random
-from string import Formatter
-from typing import List, Dict, Union
-
-import numpy as np
-
-
-class TagShuffle:
-    def __call__(self, data):
-        if 'caption' in data:
-            text = data['caption']
-            if text is not None:
-                tags = text.split(',')
-                random.shuffle(tags)
-                data['caption'] = ','.join(tags)
-            return data
-        else:
-            for i, item in enumerate(data['prompt']):
-                tags = item.split(',')
-                random.shuffle(tags)
-                data['prompt'][i] = ','.join(tags)
-            return data
-
-    def __repr__(self):
-        return 'TagShuffle()'
-
-
-class TagDropout:
-    def __init__(self, p=0.1):
-        self.p = p
-
-    def __call__(self, data):
-        if 'caption' in data:
-            text = data['caption']
-            if text is not None:
-                tags = np.array(text.split(','))
-                data['caption'] = ','.join(tags[np.random.random(len(tags)) > self.p])
-            return data
-        else:
-            for i, item in enumerate(data['prompt']):
-                tags = item.split(',')
-                data['prompt'][i] = ','.join(tags[np.random.random(len(tags)) > self.p])
-            return data
-
-    def __repr__(self):
-        return f'TagDropout(p={self.p})'
-
-
-class TemplateFill:
-    def __init__(self, word_names: Dict[str, Union[str, List[str]]]):
-        self.word_names = word_names
-        self.DA_names = {k: v for k, v in word_names.items() if not isinstance(v, str)}
-        self.dream_artist = len(self.DA_names) > 0
-
-    def __call__(self, data):
-        template, caption = data['prompt'], data['caption']
-
-        keys_need = {i[1] for i in Formatter().parse(template) if i[1] is not None}
-        fill_dict = {k: v for k, v in self.word_names.items() if k in keys_need}
-
-        if (caption is not None) and ('caption' in keys_need):
-            fill_dict.update(caption=caption)
-
-        # skip keys that not provide
-        for k in keys_need:
-            if k not in fill_dict:
-                fill_dict[k] = ''
-
-        if self.dream_artist:
-            fill_dict_pos = {k: (v if isinstance(v, str) else v[0]) for k, v in fill_dict.items()}
-            fill_dict_neg = {k: (v if isinstance(v, str) else v[1]) for k, v in fill_dict.items()}
-            return {'prompt':[template.format(**fill_dict_neg), template.format(**fill_dict_pos)]}
-        else:
-            return {'prompt':[template.format(**fill_dict)]}
-
-    def __repr__(self):
-        return f'TemplateFill(\nword_names={self.word_names}\n)'
+"""
+caption_tools.py
+====================
+    :Name:        process prompts
+    :Author:      Dong Ziyi
+    :Affiliation: HCP Lab, SYSU
+    :Created:     10/03/2023
+    :Licence:     Apache-2.0
+"""
+
+import random
+from string import Formatter
+from typing import List, Dict, Union
+
+import numpy as np
+
+
+class TagShuffle:
+    def __call__(self, data):
+        if 'caption' in data:
+            text = data['caption']
+            if text is not None:
+                tags = text.split(',')
+                random.shuffle(tags)
+                data['caption'] = ','.join(tags)
+            return data
+        else:
+            for i, item in enumerate(data['prompt']):
+                tags = item.split(',')
+                random.shuffle(tags)
+                data['prompt'][i] = ','.join(tags)
+            return data
+
+    def __repr__(self):
+        return 'TagShuffle()'
+
+
+class TagDropout:
+    def __init__(self, p=0.1):
+        self.p = p
+
+    def __call__(self, data):
+        if 'caption' in data:
+            text = data['caption']
+            if text is not None:
+                tags = np.array(text.split(','))
+                data['caption'] = ','.join(tags[np.random.random(len(tags)) > self.p])
+            return data
+        else:
+            for i, item in enumerate(data['prompt']):
+                tags = item.split(',')
+                data['prompt'][i] = ','.join(tags[np.random.random(len(tags)) > self.p])
+            return data
+
+    def __repr__(self):
+        return f'TagDropout(p={self.p})'
+
+
+class TemplateFill:
+    def __init__(self, word_names: Dict[str, Union[str, List[str]]]):
+        self.word_names = word_names
+        self.DA_names = {k: v for k, v in word_names.items() if not isinstance(v, str)}
+        self.dream_artist = len(self.DA_names) > 0
+
+    def __call__(self, data):
+        template, caption = data['prompt'], data['caption']
+
+        keys_need = {i[1] for i in Formatter().parse(template) if i[1] is not None}
+        fill_dict = {k: v for k, v in self.word_names.items() if k in keys_need}
+
+        if (caption is not None) and ('caption' in keys_need):
+            fill_dict.update(caption=caption)
+
+        # skip keys that not provide
+        for k in keys_need:
+            if k not in fill_dict:
+                fill_dict[k] = ''
+
+        if self.dream_artist:
+            fill_dict_pos = {k: (v if isinstance(v, str) else v[0]) for k, v in fill_dict.items()}
+            fill_dict_neg = {k: (v if isinstance(v, str) else v[1]) for k, v in fill_dict.items()}
+            return {'prompt':[template.format(**fill_dict_neg), template.format(**fill_dict_pos)]}
+        else:
+            return {'prompt':[template.format(**fill_dict)]}
+
+    def __repr__(self):
+        return f'TemplateFill(\nword_names={self.word_names}\n)'
```

### Comparing `hcpdiff-0.2.2/hcpdiff/utils/cfg_net_tools.py` & `hcpdiff-0.3.0/hcpdiff/utils/cfg_net_tools.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,278 +1,278 @@
-"""
-cfg_net_tools.py
-====================
-    :Name:        creat model and plugin from config
-    :Author:      Dong Ziyi
-    :Affiliation: HCP Lab, SYSU
-    :Created:     10/03/2023
-    :Licence:     Apache-2.0
-"""
-
-
-from typing import Dict, List, Iterable, Tuple, Union, Any
-
-import re
-import torch
-from torch import nn
-
-from .utils import net_path_join
-from hcpdiff.models.lora_base import LoraBlock, LoraGroup
-from hcpdiff.models import lora_layers
-from hcpdiff.models.plugin import SinglePluginBlock, MultiPluginBlock, PluginBlock, PluginGroup
-from .ckpt_manager import CkptManagerPKL, CkptManagerSafe
-
-def get_class_match_layer(class_name, block:nn.Module):
-    if type(block).__name__==class_name:
-        return ['']
-    else:
-        return ['.'+name for name, layer in block.named_modules() if type(layer).__name__==class_name]
-
-def get_match_layers(layers, all_layers, return_metas=False) -> Union[List[str], List[Dict[str, Any]]]:
-    res=[]
-    for name in layers:
-        metas = name.split(':')
-
-        use_re = False
-        pre_hook = False
-        cls_filter = None
-        for meta in metas[:-1]:
-            if meta=='re':
-                use_re=True
-            elif meta=='pre_hook':
-                pre_hook=True
-            elif meta.startswith('cls('):
-                cls_filter=meta[4:-1]
-
-        name = metas[-1]
-        if use_re:
-            pattern = re.compile(name)
-            match_layers = filter(lambda x: pattern.match(x) != None, all_layers.keys())
-        else:
-            match_layers = [name]
-
-        if cls_filter is not None:
-            match_layers_new = []
-            for layer in match_layers:
-                match_layers_new.extend([layer + x for x in get_class_match_layer(name[1], all_layers[layer])])
-            match_layers = match_layers_new
-
-        for layer in match_layers:
-            if return_metas:
-                res.append({'layer': layer, 'pre_hook': pre_hook})
-            else:
-                res.append(layer)
-
-    # Remove duplicates and keep the original order
-    if return_metas:
-        layer_set=set()
-        res_unique = []
-        for item in res:
-            if item['layer'] not in layer_set:
-                layer_set.add(item['layer'])
-                res_unique.append(item)
-        return res_unique
-    else:
-        return sorted(set(res), key=res.index)
-
-def get_lora_rank_and_cls(lora_state):
-    rank_groups = getattr(lora_state, 'layer.rank_groups', 1)
-    if rank_groups > 1:
-        if len(lora_state['layer.lora_down.weight'].shape) == 3:
-            rank = rank_groups * lora_state['layer.lora_down.weight'].shape[2]
-        else:
-            rank = lora_state['layer.lora_down.weight'].shape[0]
-        lora_layer_cls = lora_layers.layer_map['loha_group']
-    else:
-        rank = lora_state['layer.lora_down.weight'].shape[0]
-        lora_layer_cls = lora_layers.layer_map['lora']
-    return lora_layer_cls, rank, rank_groups
-
-def make_hcpdiff(model, cfg_model, cfg_lora, default_lr=1e-5) -> Tuple[List[Dict], Union[LoraGroup, Tuple[LoraGroup, LoraGroup]]]:
-    named_modules = {k:v for k,v in model.named_modules()}
-
-    train_params=[]
-    all_lora_blocks={}
-    all_lora_blocks_neg={}
-
-    if cfg_model is not None:
-        for item in cfg_model:
-            for layer_name in get_match_layers(item.layers, named_modules):
-                layer = named_modules[layer_name]
-                layer.requires_grad_(True)
-                layer.train()
-                train_params.append({'params':list(LoraBlock.extract_param_without_lora(layer).values()), 'lr':getattr(item, 'lr', default_lr)})
-
-    if cfg_lora is not None:
-        for lora_id, item in enumerate(cfg_lora):
-            for layer_name in get_match_layers(item.layers, named_modules):
-                layer = named_modules[layer_name]
-                arg_dict = {k:v for k,v in item.items() if k!='layers'}
-                lora_block_dict = lora_layers.layer_map[getattr(arg_dict, 'type', 'lora')].wrap_model(lora_id, layer, **arg_dict)
-
-                params_group = []
-                block_branch = getattr(item, 'branch', None) # for DreamArtist-lora
-                for k,v in lora_block_dict.items():
-                    block_path = net_path_join(layer_name, k)
-                    if block_branch is None:
-                        all_lora_blocks[block_path] = v
-                    elif block_branch=='p':
-                        all_lora_blocks[block_path] = v
-                        v.set_mask((0.5, 1))
-                    elif block_branch == 'n':
-                        all_lora_blocks_neg[block_path]=v
-                        v.set_mask((0, 0.5))
-                    else:
-                        raise NotImplementedError(f'Unsupported branch "{block_branch}"')
-                    v.requires_grad_(True)
-                    v.train()
-                    params_group.extend(v.parameters())
-
-                train_params.append({'params': params_group, 'lr':getattr(item, 'lr', default_lr)})
-
-    if len(all_lora_blocks_neg)>0:
-        return train_params, (LoraGroup(all_lora_blocks), LoraGroup(all_lora_blocks_neg))
-    else:
-        return train_params, LoraGroup(all_lora_blocks)
-
-def make_plugin(model, cfg_plugin, default_lr=1e-5) -> Tuple[List, Dict[str, PluginGroup]]:
-    train_params=[]
-    all_plugin_group={}
-
-    if cfg_plugin is None:
-        return train_params, all_plugin_group
-
-    named_modules = {k: v for k, v in model.named_modules()}
-
-    # builder: functools.partial
-    for plugin_name, builder in cfg_plugin.items():
-        all_plugin_blocks={}
-
-        lr = builder.keywords.pop('lr') if 'lr' in builder.keywords else default_lr
-        train_plugin = builder.keywords.pop('train') if 'train' in builder.keywords else True
-        plugin_class = getattr(builder.func, '__self__', builder.func) # support static or class method
-
-        if issubclass(plugin_class, MultiPluginBlock):
-            from_layers = [{**item, 'layer':named_modules[item['layer']]} for item in get_match_layers(builder.keywords.pop('from_layers'), named_modules, return_metas=True)]
-            to_layers = [{**item, 'layer':named_modules[item['layer']]} for item in get_match_layers(builder.keywords.pop('to_layers'), named_modules, return_metas=True)]
-
-            layer = builder(name=plugin_name, host_model=model, from_layers=from_layers, to_layers=to_layers)
-            if train_plugin:
-                layer.requires_grad_(True)
-                layer.train()
-                train_params.append({'params': layer.parameters(), 'lr': lr})
-            else:
-                layer.requires_grad_(False)
-                layer.eval()
-            all_plugin_blocks[''] = layer
-        elif issubclass(plugin_class, SinglePluginBlock):
-            layers_name = builder.keywords.pop('layers')
-            for layer_name in get_match_layers(layers_name, named_modules):
-                blocks = builder(name=plugin_name, host_model=model, host=named_modules[layer_name])
-                if not isinstance(blocks, dict):
-                    blocks={'':blocks}
-
-                params_group = []
-                for k,v in blocks.items():
-                    all_plugin_blocks[net_path_join(layer_name, k)] = v
-                    if train_plugin:
-                        v.requires_grad_(True)
-                        v.train()
-                        params_group.extend(v.parameters())
-                    else:
-                        v.requires_grad_(False)
-                        v.eval()
-                if train_plugin:
-                    train_params.append({'params': params_group, 'lr': lr})
-        elif issubclass(plugin_class, PluginBlock):
-            from_layer = get_match_layers(builder.keywords.pop('from_layer'), named_modules, return_metas=True)
-            to_layer = get_match_layers(builder.keywords.pop('to_layer'), named_modules, return_metas=True)
-
-            for from_layer_meta, to_layer_meta in zip(from_layer, to_layer):
-                from_layer_name=from_layer_meta['layer']
-                from_layer_meta['layer']=named_modules[from_layer_name]
-                to_layer_meta['layer']=named_modules[to_layer_meta['layer']]
-                layer = builder(name=plugin_name, host_model=model, from_layer=from_layer_meta, to_layer=to_layer_meta)
-                if train_plugin:
-                    layer.requires_grad_(True)
-                    layer.train()
-                    train_params.append({'params': layer.parameters(), 'lr': lr})
-                else:
-                    layer.requires_grad_(False)
-                    layer.eval()
-                all_plugin_blocks[from_layer_name] = layer
-        else:
-            raise NotImplementedError(f'Unknown plugin {plugin_class}')
-        all_plugin_group[plugin_name] = PluginGroup(all_plugin_blocks)
-    return train_params, all_plugin_group
-
-@torch.no_grad()
-def load_hcpdiff(model:nn.Module, cfg_merge):
-    named_modules = {k: v for k, v in model.named_modules()}
-    named_params = {k: v for k, v in model.named_parameters()}
-    all_lora_blocks = {}
-
-    ckpt_manager_torch = CkptManagerPKL()
-    ckpt_manager_safe = CkptManagerSafe()
-
-    def get_ckpt_manager(path:str):
-        return ckpt_manager_safe if path.endswith('.safetensors') else ckpt_manager_torch
-
-    if "lora" in cfg_merge and cfg_merge.lora is not None:
-        for lora_id, item in enumerate(cfg_merge.lora):
-            lora_state = get_ckpt_manager(item.path).load_ckpt(item.path, map_location='cpu')['lora']
-            lora_block_state = {}
-            # get all layers in the lora_state
-            for name, p in lora_state.items():
-                # lora_block. is the old format
-                prefix, block_name = name.split('.___.' if name.rfind('lora_block.')==-1 else '.lora_block.', 1)
-                if prefix not in lora_block_state:
-                    lora_block_state[prefix] = {}
-                lora_block_state[prefix][block_name] = p
-            # get selected layers
-            if item.layers != 'all':
-                match_blocks = get_match_layers(item.layers, named_modules)
-                lora_state_new = {}
-                for k, v in lora_block_state.items():
-                    for mk in match_blocks:
-                        if k.startswith(mk):
-                            lora_state_new[k]=v
-                            break
-                lora_block_state = lora_state_new
-            # add lora to host and load weights
-            for host_name, lora_state in lora_block_state.items():
-                lora_layer_cls, rank, rank_groups = get_lora_rank_and_cls(lora_state)
-                del lora_state['scale']
-
-                lora_block = lora_layer_cls.wrap_layer(lora_id, named_modules[host_name], rank=rank, dropout=getattr(item, 'dropout', 0.0),
-                                                        scale=getattr(item, 'alpha', 1.0), bias='layer.lora_up.bias' in lora_state,
-                                                        rank_groups=rank_groups)
-                all_lora_blocks[f'{host_name}.{lora_block.name}'] = lora_block
-                lora_block.load_state_dict(lora_state, strict=False)
-                lora_block.set_mask(getattr(item, 'mask', None))
-                lora_block.to(model.device)
-
-    if "part" in cfg_merge and cfg_merge.part is not None:
-        for item in cfg_merge.part:
-            part_state = get_ckpt_manager(item.path).load_ckpt(item.path, map_location='cpu')['base']
-            if item.layers == 'all':
-                for k, v in part_state.items():
-                    named_params[k].data = cfg_merge.base_model_alpha * named_params[k].data + item.alpha * v
-            else:
-                match_blocks = get_match_layers(item.layers, named_modules)
-                state_add = {k:v for blk in match_blocks for k,v in part_state.items() if k.startswith(blk)}
-                for k, v in state_add.items():
-                    named_params[k].data = cfg_merge.base_model_alpha * named_params[k].data + item.alpha * v
-
-    if "plugin" in cfg_merge and cfg_merge.plugin is not None:
-        for name, item in cfg_merge.plugin.items():
-            plugin_state = get_ckpt_manager(item.path).load_ckpt(item.path, map_location='cpu')
-            if item.layers != 'all':
-                match_blocks = get_match_layers(item.layers, named_modules)
-                plugin_state = {k: v for blk in match_blocks for k, v in plugin_state.items() if k.startswith(blk)}
-            plugin_state = {k.replace('___', name):v for k, v in plugin_state.items()} # replace placeholder to target plugin name
-            model.load_state_dict(plugin_state, strict=False)
-            del item.layers
-            del item.path
-            getattr(model, name).set_hyper_params(**item)
-
+"""
+cfg_net_tools.py
+====================
+    :Name:        creat model and plugin from config
+    :Author:      Dong Ziyi
+    :Affiliation: HCP Lab, SYSU
+    :Created:     10/03/2023
+    :Licence:     Apache-2.0
+"""
+
+
+from typing import Dict, List, Tuple, Union, Any
+
+import re
+import torch
+from torch import nn
+
+from .utils import net_path_join
+from hcpdiff.models.lora_base import LoraBlock, LoraGroup
+from hcpdiff.models import lora_layers
+from hcpdiff.models.plugin import SinglePluginBlock, MultiPluginBlock, PluginBlock, PluginGroup
+from hcpdiff.ckpt_manager import CkptManagerPKL, CkptManagerSafe
+
+def get_class_match_layer(class_name, block:nn.Module):
+    if type(block).__name__==class_name:
+        return ['']
+    else:
+        return ['.'+name for name, layer in block.named_modules() if type(layer).__name__==class_name]
+
+def get_match_layers(layers, all_layers, return_metas=False) -> Union[List[str], List[Dict[str, Any]]]:
+    res=[]
+    for name in layers:
+        metas = name.split(':')
+
+        use_re = False
+        pre_hook = False
+        cls_filter = None
+        for meta in metas[:-1]:
+            if meta=='re':
+                use_re=True
+            elif meta=='pre_hook':
+                pre_hook=True
+            elif meta.startswith('cls('):
+                cls_filter=meta[4:-1]
+
+        name = metas[-1]
+        if use_re:
+            pattern = re.compile(name)
+            match_layers = filter(lambda x: pattern.match(x) != None, all_layers.keys())
+        else:
+            match_layers = [name]
+
+        if cls_filter is not None:
+            match_layers_new = []
+            for layer in match_layers:
+                match_layers_new.extend([layer + x for x in get_class_match_layer(name[1], all_layers[layer])])
+            match_layers = match_layers_new
+
+        for layer in match_layers:
+            if return_metas:
+                res.append({'layer': layer, 'pre_hook': pre_hook})
+            else:
+                res.append(layer)
+
+    # Remove duplicates and keep the original order
+    if return_metas:
+        layer_set=set()
+        res_unique = []
+        for item in res:
+            if item['layer'] not in layer_set:
+                layer_set.add(item['layer'])
+                res_unique.append(item)
+        return res_unique
+    else:
+        return sorted(set(res), key=res.index)
+
+def get_lora_rank_and_cls(lora_state):
+    rank_groups = getattr(lora_state, 'layer.rank_groups', 1)
+    if rank_groups > 1:
+        if len(lora_state['layer.lora_down.weight'].shape) == 3:
+            rank = rank_groups * lora_state['layer.lora_down.weight'].shape[2]
+        else:
+            rank = lora_state['layer.lora_down.weight'].shape[0]
+        lora_layer_cls = lora_layers.layer_map['loha_group']
+    else:
+        rank = lora_state['layer.lora_down.weight'].shape[0]
+        lora_layer_cls = lora_layers.layer_map['lora']
+    return lora_layer_cls, rank, rank_groups
+
+def make_hcpdiff(model, cfg_model, cfg_lora, default_lr=1e-5) -> Tuple[List[Dict], Union[LoraGroup, Tuple[LoraGroup, LoraGroup]]]:
+    named_modules = {k:v for k,v in model.named_modules()}
+
+    train_params=[]
+    all_lora_blocks={}
+    all_lora_blocks_neg={}
+
+    if cfg_model is not None:
+        for item in cfg_model:
+            for layer_name in get_match_layers(item.layers, named_modules):
+                layer = named_modules[layer_name]
+                layer.requires_grad_(True)
+                layer.train()
+                train_params.append({'params':list(LoraBlock.extract_param_without_lora(layer).values()), 'lr':getattr(item, 'lr', default_lr)})
+
+    if cfg_lora is not None:
+        for lora_id, item in enumerate(cfg_lora):
+            for layer_name in get_match_layers(item.layers, named_modules):
+                layer = named_modules[layer_name]
+                arg_dict = {k:v for k,v in item.items() if k!='layers'}
+                lora_block_dict = lora_layers.layer_map[getattr(arg_dict, 'type', 'lora')].wrap_model(lora_id, layer, **arg_dict)
+
+                params_group = []
+                block_branch = getattr(item, 'branch', None) # for DreamArtist-lora
+                for k,v in lora_block_dict.items():
+                    block_path = net_path_join(layer_name, k)
+                    if block_branch is None:
+                        all_lora_blocks[block_path] = v
+                    elif block_branch=='p':
+                        all_lora_blocks[block_path] = v
+                        v.set_mask((0.5, 1))
+                    elif block_branch == 'n':
+                        all_lora_blocks_neg[block_path]=v
+                        v.set_mask((0, 0.5))
+                    else:
+                        raise NotImplementedError(f'Unsupported branch "{block_branch}"')
+                    v.requires_grad_(True)
+                    v.train()
+                    params_group.extend(v.parameters())
+
+                train_params.append({'params': params_group, 'lr':getattr(item, 'lr', default_lr)})
+
+    if len(all_lora_blocks_neg)>0:
+        return train_params, (LoraGroup(all_lora_blocks), LoraGroup(all_lora_blocks_neg))
+    else:
+        return train_params, LoraGroup(all_lora_blocks)
+
+def make_plugin(model, cfg_plugin, default_lr=1e-5) -> Tuple[List, Dict[str, PluginGroup]]:
+    train_params=[]
+    all_plugin_group={}
+
+    if cfg_plugin is None:
+        return train_params, all_plugin_group
+
+    named_modules = {k: v for k, v in model.named_modules()}
+
+    # builder: functools.partial
+    for plugin_name, builder in cfg_plugin.items():
+        all_plugin_blocks={}
+
+        lr = builder.keywords.pop('lr') if 'lr' in builder.keywords else default_lr
+        train_plugin = builder.keywords.pop('train') if 'train' in builder.keywords else True
+        plugin_class = getattr(builder.func, '__self__', builder.func) # support static or class method
+
+        if issubclass(plugin_class, MultiPluginBlock):
+            from_layers = [{**item, 'layer':named_modules[item['layer']]} for item in get_match_layers(builder.keywords.pop('from_layers'), named_modules, return_metas=True)]
+            to_layers = [{**item, 'layer':named_modules[item['layer']]} for item in get_match_layers(builder.keywords.pop('to_layers'), named_modules, return_metas=True)]
+
+            layer = builder(name=plugin_name, host_model=model, from_layers=from_layers, to_layers=to_layers)
+            if train_plugin:
+                layer.requires_grad_(True)
+                layer.train()
+                train_params.append({'params': layer.parameters(), 'lr': lr})
+            else:
+                layer.requires_grad_(False)
+                layer.eval()
+            all_plugin_blocks[''] = layer
+        elif issubclass(plugin_class, SinglePluginBlock):
+            layers_name = builder.keywords.pop('layers')
+            for layer_name in get_match_layers(layers_name, named_modules):
+                blocks = builder(name=plugin_name, host_model=model, host=named_modules[layer_name])
+                if not isinstance(blocks, dict):
+                    blocks={'':blocks}
+
+                params_group = []
+                for k,v in blocks.items():
+                    all_plugin_blocks[net_path_join(layer_name, k)] = v
+                    if train_plugin:
+                        v.requires_grad_(True)
+                        v.train()
+                        params_group.extend(v.parameters())
+                    else:
+                        v.requires_grad_(False)
+                        v.eval()
+                if train_plugin:
+                    train_params.append({'params': params_group, 'lr': lr})
+        elif issubclass(plugin_class, PluginBlock):
+            from_layer = get_match_layers(builder.keywords.pop('from_layer'), named_modules, return_metas=True)
+            to_layer = get_match_layers(builder.keywords.pop('to_layer'), named_modules, return_metas=True)
+
+            for from_layer_meta, to_layer_meta in zip(from_layer, to_layer):
+                from_layer_name=from_layer_meta['layer']
+                from_layer_meta['layer']=named_modules[from_layer_name]
+                to_layer_meta['layer']=named_modules[to_layer_meta['layer']]
+                layer = builder(name=plugin_name, host_model=model, from_layer=from_layer_meta, to_layer=to_layer_meta)
+                if train_plugin:
+                    layer.requires_grad_(True)
+                    layer.train()
+                    train_params.append({'params': layer.parameters(), 'lr': lr})
+                else:
+                    layer.requires_grad_(False)
+                    layer.eval()
+                all_plugin_blocks[from_layer_name] = layer
+        else:
+            raise NotImplementedError(f'Unknown plugin {plugin_class}')
+        all_plugin_group[plugin_name] = PluginGroup(all_plugin_blocks)
+    return train_params, all_plugin_group
+
+@torch.no_grad()
+def load_hcpdiff(model:nn.Module, cfg_merge):
+    named_modules = {k: v for k, v in model.named_modules()}
+    named_params = {k: v for k, v in model.named_parameters()}
+    all_lora_blocks = {}
+
+    ckpt_manager_torch = CkptManagerPKL()
+    ckpt_manager_safe = CkptManagerSafe()
+
+    def get_ckpt_manager(path:str):
+        return ckpt_manager_safe if path.endswith('.safetensors') else ckpt_manager_torch
+
+    if "lora" in cfg_merge and cfg_merge.lora is not None:
+        for lora_id, item in enumerate(cfg_merge.lora):
+            lora_state = get_ckpt_manager(item.path).load_ckpt(item.path, map_location='cpu')['lora']
+            lora_block_state = {}
+            # get all layers in the lora_state
+            for name, p in lora_state.items():
+                # lora_block. is the old format
+                prefix, block_name = name.split('.___.' if name.rfind('lora_block.')==-1 else '.lora_block.', 1)
+                if prefix not in lora_block_state:
+                    lora_block_state[prefix] = {}
+                lora_block_state[prefix][block_name] = p
+            # get selected layers
+            if item.layers != 'all':
+                match_blocks = get_match_layers(item.layers, named_modules)
+                lora_state_new = {}
+                for k, v in lora_block_state.items():
+                    for mk in match_blocks:
+                        if k.startswith(mk):
+                            lora_state_new[k]=v
+                            break
+                lora_block_state = lora_state_new
+            # add lora to host and load weights
+            for host_name, lora_state in lora_block_state.items():
+                lora_layer_cls, rank, rank_groups = get_lora_rank_and_cls(lora_state)
+                del lora_state['scale']
+
+                lora_block = lora_layer_cls.wrap_layer(lora_id, named_modules[host_name], rank=rank, dropout=getattr(item, 'dropout', 0.0),
+                                                        scale=getattr(item, 'alpha', 1.0), bias='layer.lora_up.bias' in lora_state,
+                                                        rank_groups=rank_groups, alpha_auto_scale=getattr(item, 'alpha_auto_scale', True))
+                all_lora_blocks[f'{host_name}.{lora_block.name}'] = lora_block
+                lora_block.load_state_dict(lora_state, strict=False)
+                lora_block.set_mask(getattr(item, 'mask', None))
+                lora_block.to(model.device)
+
+    if "part" in cfg_merge and cfg_merge.part is not None:
+        for item in cfg_merge.part:
+            part_state = get_ckpt_manager(item.path).load_ckpt(item.path, map_location='cpu')['base']
+            if item.layers == 'all':
+                for k, v in part_state.items():
+                    named_params[k].data = cfg_merge.base_model_alpha * named_params[k].data + item.alpha * v
+            else:
+                match_blocks = get_match_layers(item.layers, named_modules)
+                state_add = {k:v for blk in match_blocks for k,v in part_state.items() if k.startswith(blk)}
+                for k, v in state_add.items():
+                    named_params[k].data = cfg_merge.base_model_alpha * named_params[k].data + item.alpha * v
+
+    if "plugin" in cfg_merge and cfg_merge.plugin is not None:
+        for name, item in cfg_merge.plugin.items():
+            plugin_state = get_ckpt_manager(item.path).load_ckpt(item.path, map_location='cpu')
+            if item.layers != 'all':
+                match_blocks = get_match_layers(item.layers, named_modules)
+                plugin_state = {k: v for blk in match_blocks for k, v in plugin_state.items() if k.startswith(blk)}
+            plugin_state = {k.replace('___', name):v for k, v in plugin_state.items()} # replace placeholder to target plugin name
+            model.load_state_dict(plugin_state, strict=False)
+            del item.layers
+            del item.path
+            getattr(model, name).set_hyper_params(**item)
+
     return LoraGroup(all_lora_blocks)
```

### Comparing `hcpdiff-0.2.2/hcpdiff/utils/ckpt_manager/ckpt_pkl.py` & `hcpdiff-0.3.0/hcpdiff/ckpt_manager/ckpt_pkl.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,103 +1,103 @@
-"""
-ckpt_pkl.py
-====================
-    :Name:        save model with torch
-    :Author:      Dong Ziyi
-    :Affiliation: HCP Lab, SYSU
-    :Created:     8/04/2023
-    :Licence:     MIT
-"""
-
-from typing import Dict
-import os
-
-import torch
-from torch import nn
-
-from hcpdiff.models.lora_base import LoraBlock, LoraGroup, split_state
-from hcpdiff.models.plugin import PluginGroup, BasePluginBlock
-from hcpdiff.utils.net_utils import save_emb
-
-
-class CkptManagerPKL:
-    def __init__(self, plugin_from_raw=False):
-        self.plugin_from_raw = plugin_from_raw
-
-    def set_save_dir(self, save_dir, emb_dir=None):
-        os.makedirs(save_dir, exist_ok=True)
-        self.save_dir = save_dir
-        self.emb_dir = emb_dir
-
-    def exclude_state(self, state, key):
-        if key is None:
-            return state
-        else:
-            return {k: v for k, v in state.items() if key in k}
-
-    def save_model(self, model: nn.Module, name, step, model_ema=None, exclude_key=None):
-        sd_model = {
-            'base': self.exclude_state(LoraBlock.extract_trainable_state_without_lora(model), exclude_key),
-        }
-        if model_ema is not None:
-            sd_ema, sd_ema_lora = split_state(model_ema.state_dict())
-            sd_model['base_ema'] = self.exclude_state(sd_ema, exclude_key)
-        self._save_ckpt(sd_model, name, step)
-
-    def save_plugins(self, host_model: nn.Module, plugins: Dict[str, PluginGroup], name:str, step:int, model_ema=None):
-        if len(plugins)>0:
-            sd_plugin={}
-            for plugin_name, plugin in plugins.items():
-                sd_plugin['plugin'] = plugin.state_dict(host_model if self.plugin_from_raw else None)
-                if model_ema is not None:
-                    sd_plugin['plugin_ema'] = plugin.state_dict(model_ema)
-                self._save_ckpt(sd_plugin, f'{name}-{plugin_name}', step)
-
-    def save_model_with_lora(self, model: nn.Module, lora_blocks: LoraGroup, name:str, step:int, model_ema=None,
-                             exclude_key=None):
-        sd_model = {
-            'base': self.exclude_state(BasePluginBlock.extract_state_without_plugin(model, trainable=True), exclude_key),
-        } if model is not None else {}
-        if (lora_blocks is not None) and (not lora_blocks.empty()):
-            sd_model['lora'] = lora_blocks.state_dict(model if self.plugin_from_raw else None)
-
-        if model_ema is not None:
-            ema_state = model_ema.state_dict()
-            if model is not None:
-                sd_ema = {k:ema_state[k] for k in sd_model['base'].keys()}
-                sd_model['base_ema'] = self.exclude_state(sd_ema, exclude_key)
-            if (lora_blocks is not None) and (not lora_blocks.empty()):
-                sd_model['lora_ema'] = {k:ema_state[k] for k in sd_model['lora'].keys()}
-
-        self._save_ckpt(sd_model, name, step)
-
-    def _save_ckpt(self, sd_model, name, step, save_path=None):
-        if save_path is None:
-            save_path = os.path.join(self.save_dir, f"{name}-{step}.ckpt")
-        torch.save(sd_model, save_path)
-
-    def load_ckpt(self, ckpt_path, map_location='cpu'):
-        return torch.load(ckpt_path, map_location=map_location)
-
-    def load_ckpt_to_model(self, model: nn.Module, ckpt_path, model_ema=None):
-        sd = self.load_ckpt(ckpt_path)
-        if 'base' in sd:
-            model.load_state_dict(sd['base'], strict=False)
-        if 'lora' in sd:
-            model.load_state_dict(sd['lora'], strict=False)
-        if 'plugin' in sd:
-            model.load_state_dict(sd['plugin'], strict=False)
-
-        if model_ema is not None:
-            if 'base' in sd:
-                model_ema.load_state_dict(sd['base_ema'])
-            if 'lora' in sd:
-                model_ema.load_state_dict(sd['lora_ema'])
-            if 'plugin' in sd:
-                model_ema.load_state_dict(sd['plugin_ema'])
-
-    def save_embedding(self, train_pts, step, replace):
-        for k, v in train_pts.items():
-            save_path = os.path.join(self.save_dir, f"{k}-{step}.pt")
-            save_emb(save_path, v.data, replace=True)
-            if replace:
-                save_emb(f'{k}.pt', v.data, replace=True)
+"""
+ckpt_pkl.py
+====================
+    :Name:        save model with torch
+    :Author:      Dong Ziyi
+    :Affiliation: HCP Lab, SYSU
+    :Created:     8/04/2023
+    :Licence:     MIT
+"""
+
+from typing import Dict
+import os
+
+import torch
+from torch import nn
+
+from hcpdiff.models.lora_base import LoraBlock, LoraGroup, split_state
+from hcpdiff.models.plugin import PluginGroup, BasePluginBlock
+from hcpdiff.utils.net_utils import save_emb
+
+
+class CkptManagerPKL:
+    def __init__(self, plugin_from_raw=False):
+        self.plugin_from_raw = plugin_from_raw
+
+    def set_save_dir(self, save_dir, emb_dir=None):
+        os.makedirs(save_dir, exist_ok=True)
+        self.save_dir = save_dir
+        self.emb_dir = emb_dir
+
+    def exclude_state(self, state, key):
+        if key is None:
+            return state
+        else:
+            return {k: v for k, v in state.items() if key in k}
+
+    def save_model(self, model: nn.Module, name, step, model_ema=None, exclude_key=None):
+        sd_model = {
+            'base': self.exclude_state(LoraBlock.extract_trainable_state_without_lora(model), exclude_key),
+        }
+        if model_ema is not None:
+            sd_ema, sd_ema_lora = split_state(model_ema.state_dict())
+            sd_model['base_ema'] = self.exclude_state(sd_ema, exclude_key)
+        self._save_ckpt(sd_model, name, step)
+
+    def save_plugins(self, host_model: nn.Module, plugins: Dict[str, PluginGroup], name:str, step:int, model_ema=None):
+        if len(plugins)>0:
+            sd_plugin={}
+            for plugin_name, plugin in plugins.items():
+                sd_plugin['plugin'] = plugin.state_dict(host_model if self.plugin_from_raw else None)
+                if model_ema is not None:
+                    sd_plugin['plugin_ema'] = plugin.state_dict(model_ema)
+                self._save_ckpt(sd_plugin, f'{name}-{plugin_name}', step)
+
+    def save_model_with_lora(self, model: nn.Module, lora_blocks: LoraGroup, name:str, step:int, model_ema=None,
+                             exclude_key=None):
+        sd_model = {
+            'base': self.exclude_state(BasePluginBlock.extract_state_without_plugin(model, trainable=True), exclude_key),
+        } if model is not None else {}
+        if (lora_blocks is not None) and (not lora_blocks.empty()):
+            sd_model['lora'] = lora_blocks.state_dict(model if self.plugin_from_raw else None)
+
+        if model_ema is not None:
+            ema_state = model_ema.state_dict()
+            if model is not None:
+                sd_ema = {k:ema_state[k] for k in sd_model['base'].keys()}
+                sd_model['base_ema'] = self.exclude_state(sd_ema, exclude_key)
+            if (lora_blocks is not None) and (not lora_blocks.empty()):
+                sd_model['lora_ema'] = {k:ema_state[k] for k in sd_model['lora'].keys()}
+
+        self._save_ckpt(sd_model, name, step)
+
+    def _save_ckpt(self, sd_model, name, step, save_path=None):
+        if save_path is None:
+            save_path = os.path.join(self.save_dir, f"{name}-{step}.ckpt")
+        torch.save(sd_model, save_path)
+
+    def load_ckpt(self, ckpt_path, map_location='cpu'):
+        return torch.load(ckpt_path, map_location=map_location)
+
+    def load_ckpt_to_model(self, model: nn.Module, ckpt_path, model_ema=None):
+        sd = self.load_ckpt(ckpt_path)
+        if 'base' in sd:
+            model.load_state_dict(sd['base'], strict=False)
+        if 'lora' in sd:
+            model.load_state_dict(sd['lora'], strict=False)
+        if 'plugin' in sd:
+            model.load_state_dict(sd['plugin'], strict=False)
+
+        if model_ema is not None:
+            if 'base' in sd:
+                model_ema.load_state_dict(sd['base_ema'])
+            if 'lora' in sd:
+                model_ema.load_state_dict(sd['lora_ema'])
+            if 'plugin' in sd:
+                model_ema.load_state_dict(sd['plugin_ema'])
+
+    def save_embedding(self, train_pts, step, replace):
+        for k, v in train_pts.items():
+            save_path = os.path.join(self.save_dir, f"{k}-{step}.pt")
+            save_emb(save_path, v.data, replace=True)
+            if replace:
+                save_emb(f'{k}.pt', v.data, replace=True)
```

### Comparing `hcpdiff-0.2.2/hcpdiff/utils/ema.py` & `hcpdiff-0.3.0/hcpdiff/utils/ema.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,72 +1,72 @@
-import torch
-from torch import nn
-from copy import deepcopy
-from typing import Iterable, Tuple, Dict
-
-'''class ModelEma(nn.Module):
-    def __init__(self, model, decay=0.9997, device=None):
-        super(ModelEma, self).__init__()
-        # make a copy of the model for accumulating moving average of weights
-        self.module = deepcopy(model)
-        self.module.eval()
-        self.decay = decay
-        self.device = device  # perform ema on different device from model if set
-        if self.device is not None:
-            self.module.to(device=device)
-
-    def _update(self, model, update_fn):
-        with torch.no_grad():
-            for ema_v, model_v in zip(self.module.state_dict().values(), model.state_dict().values()):
-                if self.device is not None:
-                    model_v = model_v.to(device=self.device)
-                ema_v.copy_(update_fn(ema_v, model_v))
-
-    def update(self, model):
-        self._update(model, update_fn=lambda e, m: self.decay * e + (1. - self.decay) * m)
-
-    def set(self, model):
-        self._update(model, update_fn=lambda e, m: m)'''
-
-class ModelEMA:
-    def __init__(self, parameters: Iterable[Tuple[str, torch.nn.Parameter]], decay_max=0.997, decay_factor=(1,5), optimization_step=0):
-        self.train_params = {name:p.data.clone().detach() for name, p in parameters}
-        self.decay_max = decay_max
-        self.decay_factor = decay_factor
-        self.optimization_step = optimization_step
-
-    @torch.no_grad()
-    def step(self, parameters: Iterable[Tuple[str, torch.nn.Parameter]]):
-        self.optimization_step += 1
-        # Compute the decay factor for the exponential moving average.
-        if self.decay_factor[0]==self.decay_factor[1]:
-            one_minus_decay = 1-self.decay_max
-        else:
-            value = (self.decay_factor[0] + self.optimization_step) / (self.decay_factor[1] + self.optimization_step)
-            one_minus_decay = 1 - min(self.decay_max, value)
-
-        for name, param in parameters:
-            if name in self.train_params:
-                s_param=self.train_params[name]
-                s_param.sub_(one_minus_decay * (s_param - param.data.to(s_param.device)))
-
-        #torch.cuda.empty_cache()
-
-    def copy_to(self, parameters: Iterable[Tuple[str, torch.nn.Parameter]]) -> None:
-        for name, param in parameters:
-            if name in self.train_params:
-                param.data.copy_(self.train_params[name])
-
-    def to(self, device=None, dtype=None):
-        # .to() on the tensors handles None correctly
-        self.train_params = {
-            name:(p.to(device=device, dtype=dtype) if p.is_floating_point() else p.to(device=device)) for name, p in self.train_params
-        }
-        return self
-
-    def state_dict(self) -> Dict[str, torch.Tensor]:
-        return self.train_params
-
-    def load_state_dict(self, state: Dict[str, torch.Tensor]):
-        for k, v in state:
-            if k in self.train_params:
-                self.train_params[k]=v
+import torch
+from torch import nn
+from copy import deepcopy
+from typing import Iterable, Tuple, Dict
+
+'''class ModelEma(nn.Module):
+    def __init__(self, model, decay=0.9997, device=None):
+        super(ModelEma, self).__init__()
+        # make a copy of the model for accumulating moving average of weights
+        self.module = deepcopy(model)
+        self.module.eval()
+        self.decay = decay
+        self.device = device  # perform ema on different device from model if set
+        if self.device is not None:
+            self.module.to(device=device)
+
+    def _update(self, model, update_fn):
+        with torch.no_grad():
+            for ema_v, model_v in zip(self.module.state_dict().values(), model.state_dict().values()):
+                if self.device is not None:
+                    model_v = model_v.to(device=self.device)
+                ema_v.copy_(update_fn(ema_v, model_v))
+
+    def update(self, model):
+        self._update(model, update_fn=lambda e, m: self.decay * e + (1. - self.decay) * m)
+
+    def set(self, model):
+        self._update(model, update_fn=lambda e, m: m)'''
+
+class ModelEMA:
+    def __init__(self, parameters: Iterable[Tuple[str, torch.nn.Parameter]], decay_max=0.997, decay_factor=(1,5), optimization_step=0):
+        self.train_params = {name:p.data.clone().detach() for name, p in parameters}
+        self.decay_max = decay_max
+        self.decay_factor = decay_factor
+        self.optimization_step = optimization_step
+
+    @torch.no_grad()
+    def step(self, parameters: Iterable[Tuple[str, torch.nn.Parameter]]):
+        self.optimization_step += 1
+        # Compute the decay factor for the exponential moving average.
+        if self.decay_factor[0]==self.decay_factor[1]:
+            one_minus_decay = 1-self.decay_max
+        else:
+            value = (self.decay_factor[0] + self.optimization_step) / (self.decay_factor[1] + self.optimization_step)
+            one_minus_decay = 1 - min(self.decay_max, value)
+
+        for name, param in parameters:
+            if name in self.train_params:
+                s_param=self.train_params[name]
+                s_param.sub_(one_minus_decay * (s_param - param.data.to(s_param.device)))
+
+        #torch.cuda.empty_cache()
+
+    def copy_to(self, parameters: Iterable[Tuple[str, torch.nn.Parameter]]) -> None:
+        for name, param in parameters:
+            if name in self.train_params:
+                param.data.copy_(self.train_params[name])
+
+    def to(self, device=None, dtype=None):
+        # .to() on the tensors handles None correctly
+        self.train_params = {
+            name:(p.to(device=device, dtype=dtype) if p.is_floating_point() else p.to(device=device)) for name, p in self.train_params
+        }
+        return self
+
+    def state_dict(self) -> Dict[str, torch.Tensor]:
+        return self.train_params
+
+    def load_state_dict(self, state: Dict[str, torch.Tensor]):
+        for k, v in state:
+            if k in self.train_params:
+                self.train_params[k]=v
```

### Comparing `hcpdiff-0.2.2/hcpdiff/utils/img_size_tool.py` & `hcpdiff-0.3.0/hcpdiff/utils/img_size_tool.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,248 +1,248 @@
-"""
-
-img_size_tool.py
-====================
-
-    :Name:        get_image_size
-    :Purpose:     extract image dimensions given a file path
-
-    :Author:      Paulo Scardine (based on code from Emmanuel VAÏSSE)
-                  Dong Ziyi, add webp support
-
-    :Created:     26/09/2013
-    :Modified:    02/03/2023
-    :Copyright:   (c) Paulo Scardine 2013
-    :Licence:     MIT
-
-"""
-
-import collections
-import os
-import io
-import struct
-from PIL import Image
-
-FILE_UNKNOWN = "Sorry, don't know how to get size for this file."
-
-class UnknownImageFormat(Exception):
-    pass
-
-types_support = ['bmp', 'gif', 'ico', 'jpeg', 'jpg', 'png', 'tiff', 'webp']
-
-def get_image_size(file_path):
-    """
-    Return (width, height) for a given img file content - no external
-    dependencies except the os and struct builtin modules
-    """
-    width, height = get_image_metadata(file_path)
-    return width, height
-
-
-def get_image_size_from_bytesio(input, size):
-    """
-    Return (width, height) for a given img file content - no external
-    dependencies except the os and struct builtin modules
-
-    Args:
-        input (io.IOBase): io object support read & seek
-        size (int): size of buffer in byte
-    """
-    width, height = get_image_metadata_from_bytesio(input, size)
-    return width, height
-
-
-def get_image_metadata(file_path):
-    """
-    Return an `Image` object for a given img file content - no external
-    dependencies except the os and struct builtin modules
-
-    Args:
-        file_path (str): path to an image file
-
-    Returns:
-        (width, height)
-    """
-    size = os.path.getsize(file_path)
-
-    # be explicit with open arguments - we need binary mode
-    with io.open(file_path, "rb") as input:
-        return get_image_metadata_from_bytesio(input, size, file_path)
-
-
-def get_image_metadata_from_bytesio(input, size, file_path=None):
-    """
-    Return an `Image` object for a given img file content - no external
-    dependencies except the os and struct builtin modules
-
-    Args:
-        input (io.IOBase): io object support read & seek
-        size (int): size of buffer in byte
-        file_path (str): path to an image file
-
-    Returns:
-        (width, height)
-    """
-    height = -1
-    width = -1
-    data = input.read(30)
-    msg = " raised while trying to decode as JPEG."
-
-    if (size >= 10) and data[:6] in (b'GIF87a', b'GIF89a'):
-        # GIFs
-        #imgtype = GIF
-        w, h = struct.unpack("<HH", data[6:10])
-        width = int(w)
-        height = int(h)
-    elif (size >= 24) and data[8:12] == b'WEBP':
-        # WEBPs
-        #imgtype = WEBP
-        if data[15]==b'X': #VP8X
-            w = int.from_bytes(data[24:27], 'little')+1
-            h = int.from_bytes(data[27:30], 'little')+1
-        elif data[15]==b' ': #VP8
-            w, h = struct.unpack("<HH", data[0x1A:0x1E])
-        else:
-            w, h = Image.open(file_path).size
-
-        width = int(w)
-        height = int(h)
-    elif ((size >= 24) and data.startswith(b'\211PNG\r\n\032\n')
-            and (data[12:16] == b'IHDR')):
-        # PNGs
-        #imgtype = PNG
-        w, h = struct.unpack(">LL", data[16:24])
-        width = int(w)
-        height = int(h)
-    elif (size >= 16) and data.startswith(b'\211PNG\r\n\032\n'):
-        # older PNGs
-        #imgtype = PNG
-        w, h = struct.unpack(">LL", data[8:16])
-        width = int(w)
-        height = int(h)
-    elif (size >= 2) and data.startswith(b'\377\330'):
-        # JPEG
-        #imgtype = JPEG
-        input.seek(0)
-        input.read(2)
-        b = input.read(1)
-        try:
-            while (b and ord(b) != 0xDA):
-                while (ord(b) != 0xFF):
-                    b = input.read(1)
-                while (ord(b) == 0xFF):
-                    b = input.read(1)
-                if (ord(b) >= 0xC0 and ord(b) <= 0xC3):
-                    input.read(3)
-                    h, w = struct.unpack(">HH", input.read(4))
-                    break
-                else:
-                    input.read(
-                        int(struct.unpack(">H", input.read(2))[0]) - 2)
-                b = input.read(1)
-            width = int(w)
-            height = int(h)
-        except struct.error:
-            raise UnknownImageFormat("StructError" + msg)
-        except ValueError:
-            raise UnknownImageFormat("ValueError" + msg)
-        except Exception as e:
-            raise UnknownImageFormat(e.__class__.__name__ + msg)
-    elif (size >= 26) and data.startswith(b'BM'):
-        # BMP
-        #imgtype = BMP
-        headersize = struct.unpack("<I", data[14:18])[0]
-        if headersize == 12:
-            w, h = struct.unpack("<HH", data[18:22])
-            width = int(w)
-            height = int(h)
-        elif headersize >= 40:
-            w, h = struct.unpack("<ii", data[18:26])
-            width = int(w)
-            # as h is negative when stored upside down
-            height = abs(int(h))
-        else:
-            raise UnknownImageFormat(
-                "Unkown DIB header size:" +
-                str(headersize))
-    elif (size >= 8) and data[:4] in (b"II\052\000", b"MM\000\052"):
-        # Standard TIFF, big- or little-endian
-        # BigTIFF and other different but TIFF-like formats are not
-        # supported currently
-        #imgtype = TIFF
-        byteOrder = data[:2]
-        boChar = ">" if byteOrder == "MM" else "<"
-        # maps TIFF type id to size (in bytes)
-        # and python format char for struct
-        tiffTypes = {
-            1: (1, boChar + "B"),  # BYTE
-            2: (1, boChar + "c"),  # ASCII
-            3: (2, boChar + "H"),  # SHORT
-            4: (4, boChar + "L"),  # LONG
-            5: (8, boChar + "LL"),  # RATIONAL
-            6: (1, boChar + "b"),  # SBYTE
-            7: (1, boChar + "c"),  # UNDEFINED
-            8: (2, boChar + "h"),  # SSHORT
-            9: (4, boChar + "l"),  # SLONG
-            10: (8, boChar + "ll"),  # SRATIONAL
-            11: (4, boChar + "f"),  # FLOAT
-            12: (8, boChar + "d")   # DOUBLE
-        }
-        ifdOffset = struct.unpack(boChar + "L", data[4:8])[0]
-        try:
-            countSize = 2
-            input.seek(ifdOffset)
-            ec = input.read(countSize)
-            ifdEntryCount = struct.unpack(boChar + "H", ec)[0]
-            # 2 bytes: TagId + 2 bytes: type + 4 bytes: count of values + 4
-            # bytes: value offset
-            ifdEntrySize = 12
-            for i in range(ifdEntryCount):
-                entryOffset = ifdOffset + countSize + i * ifdEntrySize
-                input.seek(entryOffset)
-                tag = input.read(2)
-                tag = struct.unpack(boChar + "H", tag)[0]
-                if(tag == 256 or tag == 257):
-                    # if type indicates that value fits into 4 bytes, value
-                    # offset is not an offset but value itself
-                    type = input.read(2)
-                    type = struct.unpack(boChar + "H", type)[0]
-                    if type not in tiffTypes:
-                        raise UnknownImageFormat(
-                            "Unkown TIFF field type:" +
-                            str(type))
-                    typeSize = tiffTypes[type][0]
-                    typeChar = tiffTypes[type][1]
-                    input.seek(entryOffset + 8)
-                    value = input.read(typeSize)
-                    value = int(struct.unpack(typeChar, value)[0])
-                    if tag == 256:
-                        width = value
-                    else:
-                        height = value
-                if width > -1 and height > -1:
-                    break
-        except Exception as e:
-            raise UnknownImageFormat(str(e))
-    elif size >= 2:
-            # see http://en.wikipedia.org/wiki/ICO_(file_format)
-        #imgtype = 'ICO'
-        input.seek(0)
-        reserved = input.read(2)
-        if 0 != struct.unpack("<H", reserved)[0]:
-            raise UnknownImageFormat(FILE_UNKNOWN)
-        format = input.read(2)
-        assert 1 == struct.unpack("<H", format)[0]
-        num = input.read(2)
-        num = struct.unpack("<H", num)[0]
-        if num > 1:
-            import warnings
-            warnings.warn("ICO File contains more than one image")
-        # http://msdn.microsoft.com/en-us/library/ms997538.aspx
-        w = input.read(1)
-        h = input.read(1)
-        width = ord(w)
-        height = ord(h)
-    else:
-        raise UnknownImageFormat(FILE_UNKNOWN)
-
+"""
+
+img_size_tool.py
+====================
+
+    :Name:        get_image_size
+    :Purpose:     extract image dimensions given a file path
+
+    :Author:      Paulo Scardine (based on code from Emmanuel VAÏSSE)
+                  Dong Ziyi, add webp support
+
+    :Created:     26/09/2013
+    :Modified:    02/03/2023
+    :Copyright:   (c) Paulo Scardine 2013
+    :Licence:     MIT
+
+"""
+
+import collections
+import os
+import io
+import struct
+from PIL import Image
+
+FILE_UNKNOWN = "Sorry, don't know how to get size for this file."
+
+class UnknownImageFormat(Exception):
+    pass
+
+types_support = ['bmp', 'gif', 'ico', 'jpeg', 'jpg', 'png', 'tiff', 'webp']
+
+def get_image_size(file_path):
+    """
+    Return (width, height) for a given img file content - no external
+    dependencies except the os and struct builtin modules
+    """
+    width, height = get_image_metadata(file_path)
+    return width, height
+
+
+def get_image_size_from_bytesio(input, size):
+    """
+    Return (width, height) for a given img file content - no external
+    dependencies except the os and struct builtin modules
+
+    Args:
+        input (io.IOBase): io object support read & seek
+        size (int): size of buffer in byte
+    """
+    width, height = get_image_metadata_from_bytesio(input, size)
+    return width, height
+
+
+def get_image_metadata(file_path):
+    """
+    Return an `Image` object for a given img file content - no external
+    dependencies except the os and struct builtin modules
+
+    Args:
+        file_path (str): path to an image file
+
+    Returns:
+        (width, height)
+    """
+    size = os.path.getsize(file_path)
+
+    # be explicit with open arguments - we need binary mode
+    with io.open(file_path, "rb") as input:
+        return get_image_metadata_from_bytesio(input, size, file_path)
+
+
+def get_image_metadata_from_bytesio(input, size, file_path=None):
+    """
+    Return an `Image` object for a given img file content - no external
+    dependencies except the os and struct builtin modules
+
+    Args:
+        input (io.IOBase): io object support read & seek
+        size (int): size of buffer in byte
+        file_path (str): path to an image file
+
+    Returns:
+        (width, height)
+    """
+    height = -1
+    width = -1
+    data = input.read(30)
+    msg = " raised while trying to decode as JPEG."
+
+    if (size >= 10) and data[:6] in (b'GIF87a', b'GIF89a'):
+        # GIFs
+        #imgtype = GIF
+        w, h = struct.unpack("<HH", data[6:10])
+        width = int(w)
+        height = int(h)
+    elif (size >= 24) and data[8:12] == b'WEBP':
+        # WEBPs
+        #imgtype = WEBP
+        if data[15]==b'X': #VP8X
+            w = int.from_bytes(data[24:27], 'little')+1
+            h = int.from_bytes(data[27:30], 'little')+1
+        elif data[15]==b' ': #VP8
+            w, h = struct.unpack("<HH", data[0x1A:0x1E])
+        else:
+            w, h = Image.open(file_path).size
+
+        width = int(w)
+        height = int(h)
+    elif ((size >= 24) and data.startswith(b'\211PNG\r\n\032\n')
+            and (data[12:16] == b'IHDR')):
+        # PNGs
+        #imgtype = PNG
+        w, h = struct.unpack(">LL", data[16:24])
+        width = int(w)
+        height = int(h)
+    elif (size >= 16) and data.startswith(b'\211PNG\r\n\032\n'):
+        # older PNGs
+        #imgtype = PNG
+        w, h = struct.unpack(">LL", data[8:16])
+        width = int(w)
+        height = int(h)
+    elif (size >= 2) and data.startswith(b'\377\330'):
+        # JPEG
+        #imgtype = JPEG
+        input.seek(0)
+        input.read(2)
+        b = input.read(1)
+        try:
+            while (b and ord(b) != 0xDA):
+                while (ord(b) != 0xFF):
+                    b = input.read(1)
+                while (ord(b) == 0xFF):
+                    b = input.read(1)
+                if (ord(b) >= 0xC0 and ord(b) <= 0xC3):
+                    input.read(3)
+                    h, w = struct.unpack(">HH", input.read(4))
+                    break
+                else:
+                    input.read(
+                        int(struct.unpack(">H", input.read(2))[0]) - 2)
+                b = input.read(1)
+            width = int(w)
+            height = int(h)
+        except struct.error:
+            raise UnknownImageFormat("StructError" + msg)
+        except ValueError:
+            raise UnknownImageFormat("ValueError" + msg)
+        except Exception as e:
+            raise UnknownImageFormat(e.__class__.__name__ + msg)
+    elif (size >= 26) and data.startswith(b'BM'):
+        # BMP
+        #imgtype = BMP
+        headersize = struct.unpack("<I", data[14:18])[0]
+        if headersize == 12:
+            w, h = struct.unpack("<HH", data[18:22])
+            width = int(w)
+            height = int(h)
+        elif headersize >= 40:
+            w, h = struct.unpack("<ii", data[18:26])
+            width = int(w)
+            # as h is negative when stored upside down
+            height = abs(int(h))
+        else:
+            raise UnknownImageFormat(
+                "Unkown DIB header size:" +
+                str(headersize))
+    elif (size >= 8) and data[:4] in (b"II\052\000", b"MM\000\052"):
+        # Standard TIFF, big- or little-endian
+        # BigTIFF and other different but TIFF-like formats are not
+        # supported currently
+        #imgtype = TIFF
+        byteOrder = data[:2]
+        boChar = ">" if byteOrder == "MM" else "<"
+        # maps TIFF type id to size (in bytes)
+        # and python format char for struct
+        tiffTypes = {
+            1: (1, boChar + "B"),  # BYTE
+            2: (1, boChar + "c"),  # ASCII
+            3: (2, boChar + "H"),  # SHORT
+            4: (4, boChar + "L"),  # LONG
+            5: (8, boChar + "LL"),  # RATIONAL
+            6: (1, boChar + "b"),  # SBYTE
+            7: (1, boChar + "c"),  # UNDEFINED
+            8: (2, boChar + "h"),  # SSHORT
+            9: (4, boChar + "l"),  # SLONG
+            10: (8, boChar + "ll"),  # SRATIONAL
+            11: (4, boChar + "f"),  # FLOAT
+            12: (8, boChar + "d")   # DOUBLE
+        }
+        ifdOffset = struct.unpack(boChar + "L", data[4:8])[0]
+        try:
+            countSize = 2
+            input.seek(ifdOffset)
+            ec = input.read(countSize)
+            ifdEntryCount = struct.unpack(boChar + "H", ec)[0]
+            # 2 bytes: TagId + 2 bytes: type + 4 bytes: count of values + 4
+            # bytes: value offset
+            ifdEntrySize = 12
+            for i in range(ifdEntryCount):
+                entryOffset = ifdOffset + countSize + i * ifdEntrySize
+                input.seek(entryOffset)
+                tag = input.read(2)
+                tag = struct.unpack(boChar + "H", tag)[0]
+                if(tag == 256 or tag == 257):
+                    # if type indicates that value fits into 4 bytes, value
+                    # offset is not an offset but value itself
+                    type = input.read(2)
+                    type = struct.unpack(boChar + "H", type)[0]
+                    if type not in tiffTypes:
+                        raise UnknownImageFormat(
+                            "Unkown TIFF field type:" +
+                            str(type))
+                    typeSize = tiffTypes[type][0]
+                    typeChar = tiffTypes[type][1]
+                    input.seek(entryOffset + 8)
+                    value = input.read(typeSize)
+                    value = int(struct.unpack(typeChar, value)[0])
+                    if tag == 256:
+                        width = value
+                    else:
+                        height = value
+                if width > -1 and height > -1:
+                    break
+        except Exception as e:
+            raise UnknownImageFormat(str(e))
+    elif size >= 2:
+            # see http://en.wikipedia.org/wiki/ICO_(file_format)
+        #imgtype = 'ICO'
+        input.seek(0)
+        reserved = input.read(2)
+        if 0 != struct.unpack("<H", reserved)[0]:
+            raise UnknownImageFormat(FILE_UNKNOWN)
+        format = input.read(2)
+        assert 1 == struct.unpack("<H", format)[0]
+        num = input.read(2)
+        num = struct.unpack("<H", num)[0]
+        if num > 1:
+            import warnings
+            warnings.warn("ICO File contains more than one image")
+        # http://msdn.microsoft.com/en-us/library/ms997538.aspx
+        w = input.read(1)
+        h = input.read(1)
+        width = ord(w)
+        height = ord(h)
+    else:
+        raise UnknownImageFormat(FILE_UNKNOWN)
+
     return width, height
```

### Comparing `hcpdiff-0.2.2/hcpdiff/visualizer.py` & `hcpdiff-0.3.0/hcpdiff/visualizer.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,167 +1,167 @@
-import argparse
-import os
-import sys
-
-import hydra
-import torch
-from diffusers import StableDiffusionPipeline, StableDiffusionImg2ImgPipeline, UNet2DConditionModel
-from diffusers.utils.import_utils import is_xformers_available
-from diffusers.utils import PIL_INTERPOLATION
-from matplotlib import pyplot as plt
-from omegaconf import OmegaConf
-
-from hcpdiff.models import EmbeddingPTHook, TEEXHook, TokenizerHook
-from hcpdiff.utils.cfg_net_tools import load_hcpdiff, make_plugin
-from hcpdiff.utils.utils import to_validate_file, load_config_with_cli, load_config
-from hcpdiff.utils.img_size_tool import types_support
-from torch.cuda.amp import autocast
-from PIL import Image
-import numpy as np
-
-class UnetHook(): # for controlnet
-    def __init__(self, unet):
-        self.unet = unet
-        self.call_raw = UNet2DConditionModel.__call__
-        UNet2DConditionModel.__call__ = self.unet_call
-
-    def unet_call(self, sample, timestep, encoder_hidden_states, **kwargs):
-        return self.call_raw(self.unet, sample, timestep, encoder_hidden_states)
-
-class Visualizer:
-    def __init__(self, cfgs):
-        self.cfgs_raw = cfgs
-        self.cfgs = hydra.utils.instantiate(self.cfgs_raw)
-        self.cfg_merge = self.cfgs.merge
-
-        pipeline = self.get_pipeline()
-        comp = pipeline.from_pretrained(self.cfgs.pretrained_model, safety_checker=None, requires_safety_checker=False).components
-        comp.update(self.cfgs.new_components)
-        self.pipe = pipeline(**comp)
-
-        if self.cfg_merge:
-            self.merge_model()
-
-        self.pipe = self.pipe.to("cuda")
-        emb, _ = EmbeddingPTHook.hook_from_dir(self.cfgs.emb_dir, self.pipe.tokenizer, self.pipe.text_encoder, N_repeats=self.cfgs.N_repeats)
-        self.te_hook = TEEXHook.hook_pipe(self.pipe, N_repeats=self.cfgs.N_repeats, clip_skip=self.cfgs.clip_skip)
-        self.token_ex = TokenizerHook(self.pipe.tokenizer)
-        UnetHook(self.pipe.unet)
-
-        if is_xformers_available():
-            self.pipe.unet.enable_xformers_memory_efficient_attention()
-            # self.te_hook.enable_xformers()
-
-    def get_pipeline(self):
-        if self.cfgs.condition is None:
-            return StableDiffusionPipeline
-        else:
-            if self.cfgs.condition.type=='i2i':
-                return StableDiffusionImg2ImgPipeline
-            elif self.cfgs.condition.type=='controlnet':
-                return StableDiffusionPipeline
-            else:
-                raise NotImplementedError(f'No condition type named {self.cfgs.condition.type}')
-
-    def merge_model(self):
-        if 'plugin_cfg' in self.cfg_merge: # Build plugins
-            plugin_cfg = hydra.utils.instantiate(load_config(self.cfg_merge.plugin_cfg))
-            make_plugin(self.pipe.unet, plugin_cfg.plugin_unet)
-            make_plugin(self.pipe.text_encoder, plugin_cfg.plugin_TE)
-
-        for cfg_group in self.cfg_merge.values():
-            if hasattr(cfg_group, 'type'):
-                if cfg_group.type == 'unet':
-                    load_hcpdiff(self.pipe.unet, cfg_group)
-                elif cfg_group.type == 'TE':
-                    load_hcpdiff(self.pipe.text_encoder, cfg_group)
-
-    def set_scheduler(self, scheduler):
-        self.pipe.scheduler = scheduler
-
-    def prepare_cond_image(self, image, width, height, batch_size, device):
-        if not isinstance(image, torch.Tensor):
-            if isinstance(image, Image.Image):
-                image = [image]
-
-            if isinstance(image[0], Image.Image):
-                image = [
-                    np.array(i.resize((width, height), resample=PIL_INTERPOLATION["lanczos"]))[None, :] for i in image
-                ]
-                image = np.concatenate(image, axis=0)
-                image = np.array(image).astype(np.float32) / 255.0
-                image = image.transpose(0, 3, 1, 2)
-                image = torch.from_numpy(image)
-            elif isinstance(image[0], torch.Tensor):
-                image = torch.cat(image, dim=0)
-
-        image = image.repeat_interleave(batch_size, dim=0)
-        image = image.to(device=device)
-
-        return image
-
-    def get_ex_input(self):
-        ex_input_dict = {}
-        if self.cfgs.condition is not None:
-            img = Image.open(self.cfgs.condition.image).convert('RGB')
-            ex_input_dict['cond'] = self.prepare_cond_image(img, self.cfgs.infer_args.width, self.cfgs.infer_args.height, self.cfgs.bs*2, 'cuda')
-        return ex_input_dict
-
-    @torch.no_grad()
-    def vis_to_dir(self, root, prompt, negative_prompt='', save_cfg=True, **kwargs):
-        os.makedirs(root, exist_ok=True)
-        num_img_exist = len([x for x in os.listdir(root) if x.rsplit('.', 1)[-1] in types_support])
-
-        ex_input_dict = self.get_ex_input()
-
-        mult_p, clean_text_p = self.token_ex.parse_attn_mult(prompt)
-        mult_n, clean_text_n = self.token_ex.parse_attn_mult(negative_prompt)
-        with autocast(enabled=self.cfgs.fp16):
-            emb_n, emb_p = self.te_hook.encode_prompt_to_emb(clean_text_n + clean_text_p).chunk(2)
-            emb_p = self.te_hook.mult_attn(emb_p, mult_p)
-            emb_n = self.te_hook.mult_attn(emb_n, mult_n)
-
-            if hasattr(self.pipe.unet, 'input_feeder'):
-                for feeder in self.pipe.unet.input_feeder:
-                    feeder(ex_input_dict)
-
-            images = self.pipe(prompt_embeds=emb_p, negative_prompt_embeds=emb_n, **kwargs).images
-
-        for p, pn, img in zip(prompt, negative_prompt, images):
-            img.save(os.path.join(root, f"{num_img_exist}-{to_validate_file(prompt[0])}.{self.cfgs.save.image_type}"), quality=self.cfgs.save.quality)
-
-            if save_cfg:
-                with open(os.path.join(root, f"{num_img_exist}-info.yaml"), 'w', encoding='utf-8') as f:
-                    f.write(OmegaConf.to_yaml(self.cfgs_raw))
-            num_img_exist += 1
-
-    def show_latent(self, prompt, negative_prompt='', **kwargs):
-        emb_n, emb_p = self.te_hook.encode_prompt_to_emb(negative_prompt + prompt).chunk(2)
-        emb_p = self.te_hook.mult_attn(emb_p, self.token_ex.parse_attn_mult(prompt))
-        emb_n = self.te_hook.mult_attn(emb_n, self.token_ex.parse_attn_mult(negative_prompt))
-        images = self.pipe(prompt_embeds=emb_p, negative_prompt_embeds=emb_n, output_type='latent', **kwargs).images
-
-        for img in images:
-            plt.figure()
-            for i, feat in enumerate(img):
-                plt.subplot(221 + i)
-                plt.imshow(feat)
-            plt.show()
-
-
-if __name__ == '__main__':
-    parser = argparse.ArgumentParser(description='Stable Diffusion Training')
-    parser.add_argument('--cfg', type=str, default='')
-    args, _ = parser.parse_known_args()
-    cfgs = load_config_with_cli(args.cfg, args_list=sys.argv[3:])  # skip --cfg
-
-    os.makedirs(cfgs.out_dir, exist_ok=True)
-    if cfgs.seed is not None:
-        G = torch.Generator()
-        G.manual_seed(cfgs.seed)
-    else:
-        G = None
-
-    viser = Visualizer(cfgs)
-    for i in range(cfgs.num):
-        viser.vis_to_dir(cfgs.out_dir, prompt=[cfgs.prompt] * cfgs.bs, negative_prompt=[cfgs.neg_prompt] * cfgs.bs,
-                         generator=G, save_cfg=cfgs.save.save_cfg, **cfgs.infer_args)
+import argparse
+import os
+import sys
+
+import hydra
+import torch
+from diffusers import StableDiffusionPipeline, StableDiffusionImg2ImgPipeline, UNet2DConditionModel
+from diffusers.utils.import_utils import is_xformers_available
+from diffusers.utils import PIL_INTERPOLATION
+from matplotlib import pyplot as plt
+from omegaconf import OmegaConf
+
+from hcpdiff.models import EmbeddingPTHook, TEEXHook, TokenizerHook
+from hcpdiff.utils.cfg_net_tools import load_hcpdiff, make_plugin
+from hcpdiff.utils.utils import to_validate_file, load_config_with_cli, load_config
+from hcpdiff.utils.img_size_tool import types_support
+from torch.cuda.amp import autocast
+from PIL import Image
+import numpy as np
+
+class UnetHook(): # for controlnet
+    def __init__(self, unet):
+        self.unet = unet
+        self.call_raw = UNet2DConditionModel.__call__
+        UNet2DConditionModel.__call__ = self.unet_call
+
+    def unet_call(self, sample, timestep, encoder_hidden_states, **kwargs):
+        return self.call_raw(self.unet, sample, timestep, encoder_hidden_states)
+
+class Visualizer:
+    def __init__(self, cfgs):
+        self.cfgs_raw = cfgs
+        self.cfgs = hydra.utils.instantiate(self.cfgs_raw)
+        self.cfg_merge = self.cfgs.merge
+
+        pipeline = self.get_pipeline()
+        comp = pipeline.from_pretrained(self.cfgs.pretrained_model, safety_checker=None, requires_safety_checker=False).components
+        comp.update(self.cfgs.new_components)
+        self.pipe = pipeline(**comp)
+
+        if self.cfg_merge:
+            self.merge_model()
+
+        self.pipe = self.pipe.to("cuda")
+        emb, _ = EmbeddingPTHook.hook_from_dir(self.cfgs.emb_dir, self.pipe.tokenizer, self.pipe.text_encoder, N_repeats=self.cfgs.N_repeats)
+        self.te_hook = TEEXHook.hook_pipe(self.pipe, N_repeats=self.cfgs.N_repeats, clip_skip=self.cfgs.clip_skip)
+        self.token_ex = TokenizerHook(self.pipe.tokenizer)
+        UnetHook(self.pipe.unet)
+
+        if is_xformers_available():
+            self.pipe.unet.enable_xformers_memory_efficient_attention()
+            # self.te_hook.enable_xformers()
+
+    def get_pipeline(self):
+        if self.cfgs.condition is None:
+            return StableDiffusionPipeline
+        else:
+            if self.cfgs.condition.type=='i2i':
+                return StableDiffusionImg2ImgPipeline
+            elif self.cfgs.condition.type=='controlnet':
+                return StableDiffusionPipeline
+            else:
+                raise NotImplementedError(f'No condition type named {self.cfgs.condition.type}')
+
+    def merge_model(self):
+        if 'plugin_cfg' in self.cfg_merge: # Build plugins
+            plugin_cfg = hydra.utils.instantiate(load_config(self.cfg_merge.plugin_cfg))
+            make_plugin(self.pipe.unet, plugin_cfg.plugin_unet)
+            make_plugin(self.pipe.text_encoder, plugin_cfg.plugin_TE)
+
+        for cfg_group in self.cfg_merge.values():
+            if hasattr(cfg_group, 'type'):
+                if cfg_group.type == 'unet':
+                    load_hcpdiff(self.pipe.unet, cfg_group)
+                elif cfg_group.type == 'TE':
+                    load_hcpdiff(self.pipe.text_encoder, cfg_group)
+
+    def set_scheduler(self, scheduler):
+        self.pipe.scheduler = scheduler
+
+    def prepare_cond_image(self, image, width, height, batch_size, device):
+        if not isinstance(image, torch.Tensor):
+            if isinstance(image, Image.Image):
+                image = [image]
+
+            if isinstance(image[0], Image.Image):
+                image = [
+                    np.array(i.resize((width, height), resample=PIL_INTERPOLATION["lanczos"]))[None, :] for i in image
+                ]
+                image = np.concatenate(image, axis=0)
+                image = np.array(image).astype(np.float32) / 255.0
+                image = image.transpose(0, 3, 1, 2)
+                image = torch.from_numpy(image)
+            elif isinstance(image[0], torch.Tensor):
+                image = torch.cat(image, dim=0)
+
+        image = image.repeat_interleave(batch_size, dim=0)
+        image = image.to(device=device)
+
+        return image
+
+    def get_ex_input(self):
+        ex_input_dict = {}
+        if self.cfgs.condition is not None:
+            img = Image.open(self.cfgs.condition.image).convert('RGB')
+            ex_input_dict['cond'] = self.prepare_cond_image(img, self.cfgs.infer_args.width, self.cfgs.infer_args.height, self.cfgs.bs*2, 'cuda')
+        return ex_input_dict
+
+    @torch.no_grad()
+    def vis_to_dir(self, root, prompt, negative_prompt='', save_cfg=True, **kwargs):
+        os.makedirs(root, exist_ok=True)
+        num_img_exist = max([int(x.split('-',1)[0]) for x in os.listdir(root) if x.rsplit('.', 1)[-1] in types_support])+1
+
+        ex_input_dict = self.get_ex_input()
+
+        mult_p, clean_text_p = self.token_ex.parse_attn_mult(prompt)
+        mult_n, clean_text_n = self.token_ex.parse_attn_mult(negative_prompt)
+        with autocast(enabled=self.cfgs.fp16):
+            emb_n, emb_p = self.te_hook.encode_prompt_to_emb(clean_text_n + clean_text_p).chunk(2)
+            emb_p = self.te_hook.mult_attn(emb_p, mult_p)
+            emb_n = self.te_hook.mult_attn(emb_n, mult_n)
+
+            if hasattr(self.pipe.unet, 'input_feeder'):
+                for feeder in self.pipe.unet.input_feeder:
+                    feeder(ex_input_dict)
+
+            images = self.pipe(prompt_embeds=emb_p, negative_prompt_embeds=emb_n, **kwargs).images
+
+        for p, pn, img in zip(prompt, negative_prompt, images):
+            img.save(os.path.join(root, f"{num_img_exist}-{to_validate_file(prompt[0])}.{self.cfgs.save.image_type}"), quality=self.cfgs.save.quality)
+
+            if save_cfg:
+                with open(os.path.join(root, f"{num_img_exist}-info.yaml"), 'w', encoding='utf-8') as f:
+                    f.write(OmegaConf.to_yaml(self.cfgs_raw))
+            num_img_exist += 1
+
+    def show_latent(self, prompt, negative_prompt='', **kwargs):
+        emb_n, emb_p = self.te_hook.encode_prompt_to_emb(negative_prompt + prompt).chunk(2)
+        emb_p = self.te_hook.mult_attn(emb_p, self.token_ex.parse_attn_mult(prompt))
+        emb_n = self.te_hook.mult_attn(emb_n, self.token_ex.parse_attn_mult(negative_prompt))
+        images = self.pipe(prompt_embeds=emb_p, negative_prompt_embeds=emb_n, output_type='latent', **kwargs).images
+
+        for img in images:
+            plt.figure()
+            for i, feat in enumerate(img):
+                plt.subplot(221 + i)
+                plt.imshow(feat)
+            plt.show()
+
+
+if __name__ == '__main__':
+    parser = argparse.ArgumentParser(description='Stable Diffusion Training')
+    parser.add_argument('--cfg', type=str, default='')
+    args, _ = parser.parse_known_args()
+    cfgs = load_config_with_cli(args.cfg, args_list=sys.argv[3:])  # skip --cfg
+
+    os.makedirs(cfgs.out_dir, exist_ok=True)
+    if cfgs.seed is not None:
+        G = torch.Generator()
+        G.manual_seed(cfgs.seed)
+    else:
+        G = None
+
+    viser = Visualizer(cfgs)
+    for i in range(cfgs.num):
+        viser.vis_to_dir(cfgs.out_dir, prompt=[cfgs.prompt] * cfgs.bs, negative_prompt=[cfgs.neg_prompt] * cfgs.bs,
+                         generator=G, save_cfg=cfgs.save.save_cfg, **cfgs.infer_args)
```

### Comparing `hcpdiff-0.2.2/hcpdiff.egg-info/SOURCES.txt` & `hcpdiff-0.3.0/hcpdiff.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -16,30 +16,42 @@
 cfgs/train/examples/DreamArtist.yaml
 cfgs/train/examples/DreamBooth.yaml
 cfgs/train/examples/TextualInversion.yaml
 cfgs/train/examples/controlnet.yaml
 cfgs/train/examples/fine-tuning.yaml
 cfgs/train/examples/locon.yaml
 cfgs/train/examples/lora_conventional.yaml
+cfgs/train/examples/min_snr.yaml
 hcpdiff/__init__.py
 hcpdiff/train_ac.py
 hcpdiff/train_ac_single.py
 hcpdiff/train_colo.py
 hcpdiff/visualizer.py
 hcpdiff.egg-info/PKG-INFO
 hcpdiff.egg-info/SOURCES.txt
 hcpdiff.egg-info/dependency_links.txt
 hcpdiff.egg-info/entry_points.txt
 hcpdiff.egg-info/requires.txt
 hcpdiff.egg-info/top_level.txt
+hcpdiff/ckpt_manager/__init__.py
+hcpdiff/ckpt_manager/ckpt_pkl.py
+hcpdiff/ckpt_manager/ckpt_safetensor.py
 hcpdiff/data/__init__.py
 hcpdiff/data/bucket.py
 hcpdiff/data/cond_pair_dataset.py
 hcpdiff/data/pair_dataset.py
 hcpdiff/data/utils.py
+hcpdiff/loggers/__init__.py
+hcpdiff/loggers/base_logger.py
+hcpdiff/loggers/cli_logger.py
+hcpdiff/loggers/tensorboard_logger.py
+hcpdiff/loggers/wandb_logger.py
+hcpdiff/loss/__init__.py
+hcpdiff/loss/min_snr_loss.py
+hcpdiff/loss/mse_loss.py
 hcpdiff/models/__init__.py
 hcpdiff/models/cfg_context.py
 hcpdiff/models/controlnet.py
 hcpdiff/models/layers.py
 hcpdiff/models/lora_base.py
 hcpdiff/models/lora_layers.py
 hcpdiff/models/plugin.py
@@ -56,22 +68,15 @@
 hcpdiff/utils/caption_tools.py
 hcpdiff/utils/cfg_net_tools.py
 hcpdiff/utils/colo_utils.py
 hcpdiff/utils/ema.py
 hcpdiff/utils/img_size_tool.py
 hcpdiff/utils/net_utils.py
 hcpdiff/utils/utils.py
-hcpdiff/utils/ckpt_manager/__init__.py
-hcpdiff/utils/ckpt_manager/ckpt_pkl.py
-hcpdiff/utils/ckpt_manager/ckpt_safetensor.py
 prompt_tuning_template/caption.txt
 prompt_tuning_template/name.txt
 prompt_tuning_template/name_2pt_caption.txt
 prompt_tuning_template/name_caption.txt
 prompt_tuning_template/object.txt
 prompt_tuning_template/object_caption.txt
 prompt_tuning_template/style.txt
-prompt_tuning_template/style_caption.txt
-test/test_combine.py
-test/test_ctnet.py
-test/test_paradict.py
-test/test_plugin_param.py
+prompt_tuning_template/style_caption.txt
```

### Comparing `hcpdiff-0.2.2/prompt_tuning_template/object.txt` & `hcpdiff-0.3.0/prompt_tuning_template/object.txt`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-a photo of a {pt1} {class}
-a rendering of a {pt1} {class}
-a cropped photo of the {pt1} {class}
-the photo of a {pt1} {class}
-a photo of a clean {pt1} {class}
-a photo of a dirty {pt1} {class}
-a dark photo of the {pt1} {class}
-a photo of my {pt1} {class}
-a photo of the cool {pt1} {class}
-a close-up photo of a {pt1} {class}
-a bright photo of the {pt1} {class}
-a cropped photo of a {pt1} {class}
-a photo of the {pt1} {class}
-a good photo of the {pt1} {class}
-a photo of one {pt1} {class}
-a close-up photo of the {pt1} {class}
-a rendition of the {pt1} {class}
-a photo of the clean {pt1} {class}
-a rendition of a {pt1} {class}
-a photo of a nice {pt1} {class}
-a good photo of a {pt1} {class}
-a photo of the nice {pt1} {class}
-a photo of the small {pt1} {class}
-a photo of the weird {pt1} {class}
-a photo of the large {pt1} {class}
-a photo of a cool {pt1} {class}
+a photo of a {pt1} {class}
+a rendering of a {pt1} {class}
+a cropped photo of the {pt1} {class}
+the photo of a {pt1} {class}
+a photo of a clean {pt1} {class}
+a photo of a dirty {pt1} {class}
+a dark photo of the {pt1} {class}
+a photo of my {pt1} {class}
+a photo of the cool {pt1} {class}
+a close-up photo of a {pt1} {class}
+a bright photo of the {pt1} {class}
+a cropped photo of a {pt1} {class}
+a photo of the {pt1} {class}
+a good photo of the {pt1} {class}
+a photo of one {pt1} {class}
+a close-up photo of the {pt1} {class}
+a rendition of the {pt1} {class}
+a photo of the clean {pt1} {class}
+a rendition of a {pt1} {class}
+a photo of a nice {pt1} {class}
+a good photo of a {pt1} {class}
+a photo of the nice {pt1} {class}
+a photo of the small {pt1} {class}
+a photo of the weird {pt1} {class}
+a photo of the large {pt1} {class}
+a photo of a cool {pt1} {class}
 a photo of a small {pt1} {class}
```

### Comparing `hcpdiff-0.2.2/prompt_tuning_template/object_caption.txt` & `hcpdiff-0.3.0/prompt_tuning_template/object_caption.txt`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-a photo of a {pt1} {class}, {caption}
-a rendering of a {pt1} {class}, {caption}
-a cropped photo of the {pt1} {class}, {caption}
-the photo of a {pt1} {class}, {caption}
-a photo of a clean {pt1} {class}, {caption}
-a photo of a dirty {pt1} {class}, {caption}
-a dark photo of the {pt1} {class}, {caption}
-a photo of my {pt1} {class}, {caption}
-a photo of the cool {pt1} {class}, {caption}
-a close-up photo of a {pt1} {class}, {caption}
-a bright photo of the {pt1} {class}, {caption}
-a cropped photo of a {pt1} {class}, {caption}
-a photo of the {pt1} {class}, {caption}
-a good photo of the {pt1} {class}, {caption}
-a photo of one {pt1} {class}, {caption}
-a close-up photo of the {pt1} {class}, {caption}
-a rendition of the {pt1} {class}, {caption}
-a photo of the clean {pt1} {class}, {caption}
-a rendition of a {pt1} {class}, {caption}
-a photo of a nice {pt1} {class}, {caption}
-a good photo of a {pt1} {class}, {caption}
-a photo of the nice {pt1} {class}, {caption}
-a photo of the small {pt1} {class}, {caption}
-a photo of the weird {pt1} {class}, {caption}
-a photo of the large {pt1} {class}, {caption}
-a photo of a cool {pt1} {class}, {caption}
+a photo of a {pt1} {class}, {caption}
+a rendering of a {pt1} {class}, {caption}
+a cropped photo of the {pt1} {class}, {caption}
+the photo of a {pt1} {class}, {caption}
+a photo of a clean {pt1} {class}, {caption}
+a photo of a dirty {pt1} {class}, {caption}
+a dark photo of the {pt1} {class}, {caption}
+a photo of my {pt1} {class}, {caption}
+a photo of the cool {pt1} {class}, {caption}
+a close-up photo of a {pt1} {class}, {caption}
+a bright photo of the {pt1} {class}, {caption}
+a cropped photo of a {pt1} {class}, {caption}
+a photo of the {pt1} {class}, {caption}
+a good photo of the {pt1} {class}, {caption}
+a photo of one {pt1} {class}, {caption}
+a close-up photo of the {pt1} {class}, {caption}
+a rendition of the {pt1} {class}, {caption}
+a photo of the clean {pt1} {class}, {caption}
+a rendition of a {pt1} {class}, {caption}
+a photo of a nice {pt1} {class}, {caption}
+a good photo of a {pt1} {class}, {caption}
+a photo of the nice {pt1} {class}, {caption}
+a photo of the small {pt1} {class}, {caption}
+a photo of the weird {pt1} {class}, {caption}
+a photo of the large {pt1} {class}, {caption}
+a photo of a cool {pt1} {class}, {caption}
 a photo of a small {pt1} {class}, {caption}
```

### Comparing `hcpdiff-0.2.2/prompt_tuning_template/style.txt` & `hcpdiff-0.3.0/prompt_tuning_template/style_caption.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-a painting in the style of {pt1} {class}
-a rendering in the style of {pt1} {class}
-a cropped painting in the style of {pt1} {class}
-the painting in the style of {pt1} {class}
-a clean painting in the style of {pt1} {class}
-a dirty painting in the style of {pt1} {class}
-a dark painting in the style of {pt1} {class}
-a picture in the style of {pt1} {class}
-a cool painting in the style of {pt1} {class}
-a close-up painting in the style of {pt1} {class}
-a bright painting in the style of {pt1} {class}
-a cropped painting in the style of {pt1} {class}
-a good painting in the style of {pt1} {class}
-a close-up painting in the style of {pt1} {class}
-a rendition in the style of {pt1} {class}
-a nice painting in the style of {pt1} {class}
-a small painting in the style of {pt1} {class}
-a weird painting in the style of {pt1} {class}
-a large painting in the style of {pt1} {class}
+a painting in the style of {pt1} {class}, {caption}
+a rendering in the style of {pt1} {class}, {caption}
+a cropped painting in the style of {pt1} {class}, {caption}
+the painting in the style of {pt1} {class}, {caption}
+a clean painting in the style of {pt1} {class}, {caption}
+a dirty painting in the style of {pt1} {class}, {caption}
+a dark painting in the style of {pt1} {class}, {caption}
+a picture in the style of {pt1} {class}, {caption}
+a cool painting in the style of {pt1} {class}, {caption}
+a close-up painting in the style of {pt1} {class}, {caption}
+a bright painting in the style of {pt1} {class}, {caption}
+a cropped painting in the style of {pt1} {class}, {caption}
+a good painting in the style of {pt1} {class}, {caption}
+a close-up painting in the style of {pt1} {class}, {caption}
+a rendition in the style of {pt1} {class}, {caption}
+a nice painting in the style of {pt1} {class}, {caption}
+a small painting in the style of {pt1} {class}, {caption}
+a weird painting in the style of {pt1} {class}, {caption}
+a large painting in the style of {pt1} {class}, {caption}
```

### Comparing `hcpdiff-0.2.2/prompt_tuning_template/style_caption.txt` & `hcpdiff-0.3.0/prompt_tuning_template/style.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-a painting in the style of {pt1} {class}, {caption}
-a rendering in the style of {pt1} {class}, {caption}
-a cropped painting in the style of {pt1} {class}, {caption}
-the painting in the style of {pt1} {class}, {caption}
-a clean painting in the style of {pt1} {class}, {caption}
-a dirty painting in the style of {pt1} {class}, {caption}
-a dark painting in the style of {pt1} {class}, {caption}
-a picture in the style of {pt1} {class}, {caption}
-a cool painting in the style of {pt1} {class}, {caption}
-a close-up painting in the style of {pt1} {class}, {caption}
-a bright painting in the style of {pt1} {class}, {caption}
-a cropped painting in the style of {pt1} {class}, {caption}
-a good painting in the style of {pt1} {class}, {caption}
-a close-up painting in the style of {pt1} {class}, {caption}
-a rendition in the style of {pt1} {class}, {caption}
-a nice painting in the style of {pt1} {class}, {caption}
-a small painting in the style of {pt1} {class}, {caption}
-a weird painting in the style of {pt1} {class}, {caption}
-a large painting in the style of {pt1} {class}, {caption}
+a painting in the style of {pt1} {class}
+a rendering in the style of {pt1} {class}
+a cropped painting in the style of {pt1} {class}
+the painting in the style of {pt1} {class}
+a clean painting in the style of {pt1} {class}
+a dirty painting in the style of {pt1} {class}
+a dark painting in the style of {pt1} {class}
+a picture in the style of {pt1} {class}
+a cool painting in the style of {pt1} {class}
+a close-up painting in the style of {pt1} {class}
+a bright painting in the style of {pt1} {class}
+a cropped painting in the style of {pt1} {class}
+a good painting in the style of {pt1} {class}
+a close-up painting in the style of {pt1} {class}
+a rendition in the style of {pt1} {class}
+a nice painting in the style of {pt1} {class}
+a small painting in the style of {pt1} {class}
+a weird painting in the style of {pt1} {class}
+a large painting in the style of {pt1} {class}
```

