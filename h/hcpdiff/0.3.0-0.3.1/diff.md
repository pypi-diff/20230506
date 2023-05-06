# Comparing `tmp/hcpdiff-0.3.0.tar.gz` & `tmp/hcpdiff-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hcpdiff-0.3.0.tar", last modified: Sat May  6 03:28:25 2023, max compression
+gzip compressed data, was "hcpdiff-0.3.1.tar", last modified: Sat May  6 03:50:19 2023, max compression
```

## Comparing `hcpdiff-0.3.0.tar` & `hcpdiff-0.3.1.tar`

### file list

```diff
@@ -1,100 +1,100 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:28:25.861787 hcpdiff-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5407 2023-05-06 03:28:25.861787 hcpdiff-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4690 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:28:25.845787 hcpdiff-0.3.0/cfgs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:28:25.849787 hcpdiff-0.3.0/cfgs/infer/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/cfgs/infer/change_vae.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/cfgs/infer/euler_a.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/cfgs/infer/img2img.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/cfgs/infer/img2img_controlnet.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/cfgs/infer/text2img.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:28:25.849787 hcpdiff-0.3.0/cfgs/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/cfgs/plugins/plugin_controlnet.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     9778 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/cfgs/te_struct.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:28:25.849787 hcpdiff-0.3.0/cfgs/train/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:28:25.849787 hcpdiff-0.3.0/cfgs/train/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/cfgs/train/examples/CustomDiffusion.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/cfgs/train/examples/DreamArtist++.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/cfgs/train/examples/DreamArtist.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/cfgs/train/examples/DreamBooth.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/cfgs/train/examples/TextualInversion.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/cfgs/train/examples/controlnet.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/cfgs/train/examples/fine-tuning.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/cfgs/train/examples/locon.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/cfgs/train/examples/lora_conventional.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/cfgs/train/examples/min_snr.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/cfgs/train/train_base.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/cfgs/train/tuning_base.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    45190 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/cfgs/unet_struct.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:28:25.849787 hcpdiff-0.3.0/hcpdiff/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/hcpdiff/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:28:25.853787 hcpdiff-0.3.0/hcpdiff/ckpt_manager/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/hcpdiff/ckpt_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/hcpdiff/ckpt_manager/ckpt_pkl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/hcpdiff/ckpt_manager/ckpt_safetensor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:28:25.853787 hcpdiff-0.3.0/hcpdiff/data/
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/hcpdiff/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8554 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/hcpdiff/data/bucket.py
--rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/hcpdiff/data/cond_pair_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     6104 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/hcpdiff/data/pair_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/hcpdiff/data/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:28:25.853787 hcpdiff-0.3.0/hcpdiff/loggers/
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/hcpdiff/loggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/hcpdiff/loggers/base_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/hcpdiff/loggers/cli_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/hcpdiff/loggers/tensorboard_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/hcpdiff/loggers/wandb_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:28:25.857787 hcpdiff-0.3.0/hcpdiff/loss/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/hcpdiff/loss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/hcpdiff/loss/min_snr_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/hcpdiff/loss/mse_loss.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:28:25.857787 hcpdiff-0.3.0/hcpdiff/models/
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/hcpdiff/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/hcpdiff/models/cfg_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     7744 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/hcpdiff/models/controlnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/hcpdiff/models/layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6677 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/hcpdiff/models/lora_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7832 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/hcpdiff/models/lora_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     8754 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/hcpdiff/models/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/hcpdiff/models/text_emb_ex.py
--rw-r--r--   0 runner    (1001) docker     (123)     5674 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/hcpdiff/models/textencoder_ex.py
--rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/hcpdiff/models/tokenizer_ex.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:28:25.857787 hcpdiff-0.3.0/hcpdiff/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/hcpdiff/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/hcpdiff/tools/convert_caption_txt2json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/hcpdiff/tools/create_embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/hcpdiff/tools/gen_from_ptlist.py
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/hcpdiff/tools/init_proj.py
--rw-r--r--   0 runner    (1001) docker     (123)     8326 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/hcpdiff/tools/sd2diffusers.py
--rw-r--r--   0 runner    (1001) docker     (123)    26244 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/hcpdiff/train_ac.py
--rw-r--r--   0 runner    (1001) docker     (123)     4785 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/hcpdiff/train_ac_single.py
--rw-r--r--   0 runner    (1001) docker     (123)     9319 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/hcpdiff/train_colo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:28:25.861787 hcpdiff-0.3.0/hcpdiff/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/hcpdiff/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/hcpdiff/utils/caption_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    12819 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/hcpdiff/utils/cfg_net_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/hcpdiff/utils/colo_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/hcpdiff/utils/ema.py
--rw-r--r--   0 runner    (1001) docker     (123)     8433 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/hcpdiff/utils/img_size_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)     7052 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/hcpdiff/utils/net_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/hcpdiff/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7221 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/hcpdiff/visualizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:28:25.853787 hcpdiff-0.3.0/hcpdiff.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5407 2023-05-06 03:28:25.000000 hcpdiff-0.3.0/hcpdiff.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-05-06 03:28:25.000000 hcpdiff-0.3.0/hcpdiff.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 03:28:25.000000 hcpdiff-0.3.0/hcpdiff.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-06 03:28:25.000000 hcpdiff-0.3.0/hcpdiff.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-06 03:28:25.000000 hcpdiff-0.3.0/hcpdiff.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-06 03:28:25.000000 hcpdiff-0.3.0/hcpdiff.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:28:25.861787 hcpdiff-0.3.0/prompt_tuning_template/
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/prompt_tuning_template/caption.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/prompt_tuning_template/name.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/prompt_tuning_template/name_2pt_caption.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/prompt_tuning_template/name_caption.txt
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/prompt_tuning_template/object.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/prompt_tuning_template/object_caption.txt
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/prompt_tuning_template/style.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/prompt_tuning_template/style_caption.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 03:28:25.861787 hcpdiff-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-05-06 03:28:14.000000 hcpdiff-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:50:19.112728 hcpdiff-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-06 03:50:05.000000 hcpdiff-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5407 2023-05-06 03:50:19.108728 hcpdiff-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4690 2023-05-06 03:50:05.000000 hcpdiff-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:50:19.096728 hcpdiff-0.3.1/cfgs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:50:19.096728 hcpdiff-0.3.1/cfgs/infer/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-06 03:50:05.000000 hcpdiff-0.3.1/cfgs/infer/change_vae.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-06 03:50:05.000000 hcpdiff-0.3.1/cfgs/infer/euler_a.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-05-06 03:50:05.000000 hcpdiff-0.3.1/cfgs/infer/img2img.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-06 03:50:05.000000 hcpdiff-0.3.1/cfgs/infer/img2img_controlnet.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-05-06 03:50:05.000000 hcpdiff-0.3.1/cfgs/infer/text2img.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:50:19.096728 hcpdiff-0.3.1/cfgs/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-06 03:50:05.000000 hcpdiff-0.3.1/cfgs/plugins/plugin_controlnet.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     9778 2023-05-06 03:50:05.000000 hcpdiff-0.3.1/cfgs/te_struct.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:50:19.096728 hcpdiff-0.3.1/cfgs/train/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:50:19.100728 hcpdiff-0.3.1/cfgs/train/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-05-06 03:50:05.000000 hcpdiff-0.3.1/cfgs/train/examples/CustomDiffusion.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-05-06 03:50:05.000000 hcpdiff-0.3.1/cfgs/train/examples/DreamArtist++.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-05-06 03:50:05.000000 hcpdiff-0.3.1/cfgs/train/examples/DreamArtist.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-05-06 03:50:05.000000 hcpdiff-0.3.1/cfgs/train/examples/DreamBooth.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-05-06 03:50:05.000000 hcpdiff-0.3.1/cfgs/train/examples/TextualInversion.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-05-06 03:50:05.000000 hcpdiff-0.3.1/cfgs/train/examples/controlnet.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-05-06 03:50:05.000000 hcpdiff-0.3.1/cfgs/train/examples/fine-tuning.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-05-06 03:50:05.000000 hcpdiff-0.3.1/cfgs/train/examples/locon.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-05-06 03:50:05.000000 hcpdiff-0.3.1/cfgs/train/examples/lora_conventional.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-05-06 03:50:05.000000 hcpdiff-0.3.1/cfgs/train/examples/min_snr.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-05-06 03:50:05.000000 hcpdiff-0.3.1/cfgs/train/train_base.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-06 03:50:05.000000 hcpdiff-0.3.1/cfgs/train/tuning_base.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    45190 2023-05-06 03:50:05.000000 hcpdiff-0.3.1/cfgs/unet_struct.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:50:19.100728 hcpdiff-0.3.1/hcpdiff/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 03:50:05.000000 hcpdiff-0.3.1/hcpdiff/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:50:19.100728 hcpdiff-0.3.1/hcpdiff/ckpt_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-06 03:50:05.000000 hcpdiff-0.3.1/hcpdiff/ckpt_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-05-06 03:50:05.000000 hcpdiff-0.3.1/hcpdiff/ckpt_manager/ckpt_pkl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-05-06 03:50:05.000000 hcpdiff-0.3.1/hcpdiff/ckpt_manager/ckpt_safetensor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:50:19.100728 hcpdiff-0.3.1/hcpdiff/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-06 03:50:05.000000 hcpdiff-0.3.1/hcpdiff/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8554 2023-05-06 03:50:05.000000 hcpdiff-0.3.1/hcpdiff/data/bucket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-05-06 03:50:05.000000 hcpdiff-0.3.1/hcpdiff/data/cond_pair_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6104 2023-05-06 03:50:05.000000 hcpdiff-0.3.1/hcpdiff/data/pair_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-05-06 03:50:05.000000 hcpdiff-0.3.1/hcpdiff/data/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:50:19.104728 hcpdiff-0.3.1/hcpdiff/loggers/
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-06 03:50:05.000000 hcpdiff-0.3.1/hcpdiff/loggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-06 03:50:05.000000 hcpdiff-0.3.1/hcpdiff/loggers/base_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-05-06 03:50:05.000000 hcpdiff-0.3.1/hcpdiff/loggers/cli_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-05-06 03:50:05.000000 hcpdiff-0.3.1/hcpdiff/loggers/tensorboard_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-05-06 03:50:05.000000 hcpdiff-0.3.1/hcpdiff/loggers/wandb_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:50:19.104728 hcpdiff-0.3.1/hcpdiff/loss/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-06 03:50:05.000000 hcpdiff-0.3.1/hcpdiff/loss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-05-06 03:50:05.000000 hcpdiff-0.3.1/hcpdiff/loss/min_snr_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-06 03:50:05.000000 hcpdiff-0.3.1/hcpdiff/loss/mse_loss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:50:19.104728 hcpdiff-0.3.1/hcpdiff/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-06 03:50:05.000000 hcpdiff-0.3.1/hcpdiff/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-05-06 03:50:05.000000 hcpdiff-0.3.1/hcpdiff/models/cfg_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7744 2023-05-06 03:50:05.000000 hcpdiff-0.3.1/hcpdiff/models/controlnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-05-06 03:50:05.000000 hcpdiff-0.3.1/hcpdiff/models/layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6677 2023-05-06 03:50:05.000000 hcpdiff-0.3.1/hcpdiff/models/lora_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7832 2023-05-06 03:50:05.000000 hcpdiff-0.3.1/hcpdiff/models/lora_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8754 2023-05-06 03:50:05.000000 hcpdiff-0.3.1/hcpdiff/models/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-05-06 03:50:05.000000 hcpdiff-0.3.1/hcpdiff/models/text_emb_ex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5674 2023-05-06 03:50:05.000000 hcpdiff-0.3.1/hcpdiff/models/textencoder_ex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-05-06 03:50:05.000000 hcpdiff-0.3.1/hcpdiff/models/tokenizer_ex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:50:19.108728 hcpdiff-0.3.1/hcpdiff/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 03:50:05.000000 hcpdiff-0.3.1/hcpdiff/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-06 03:50:05.000000 hcpdiff-0.3.1/hcpdiff/tools/convert_caption_txt2json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-05-06 03:50:05.000000 hcpdiff-0.3.1/hcpdiff/tools/create_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-05-06 03:50:05.000000 hcpdiff-0.3.1/hcpdiff/tools/gen_from_ptlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-05-06 03:50:05.000000 hcpdiff-0.3.1/hcpdiff/tools/init_proj.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15067 2023-05-06 03:50:05.000000 hcpdiff-0.3.1/hcpdiff/tools/sd2diffusers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26244 2023-05-06 03:50:05.000000 hcpdiff-0.3.1/hcpdiff/train_ac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4785 2023-05-06 03:50:05.000000 hcpdiff-0.3.1/hcpdiff/train_ac_single.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9319 2023-05-06 03:50:05.000000 hcpdiff-0.3.1/hcpdiff/train_colo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:50:19.108728 hcpdiff-0.3.1/hcpdiff/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 03:50:05.000000 hcpdiff-0.3.1/hcpdiff/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-05-06 03:50:05.000000 hcpdiff-0.3.1/hcpdiff/utils/caption_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12819 2023-05-06 03:50:05.000000 hcpdiff-0.3.1/hcpdiff/utils/cfg_net_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-05-06 03:50:05.000000 hcpdiff-0.3.1/hcpdiff/utils/colo_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-05-06 03:50:05.000000 hcpdiff-0.3.1/hcpdiff/utils/ema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8433 2023-05-06 03:50:05.000000 hcpdiff-0.3.1/hcpdiff/utils/img_size_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7052 2023-05-06 03:50:05.000000 hcpdiff-0.3.1/hcpdiff/utils/net_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-05-06 03:50:05.000000 hcpdiff-0.3.1/hcpdiff/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7221 2023-05-06 03:50:05.000000 hcpdiff-0.3.1/hcpdiff/visualizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:50:19.100728 hcpdiff-0.3.1/hcpdiff.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5407 2023-05-06 03:50:19.000000 hcpdiff-0.3.1/hcpdiff.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-05-06 03:50:19.000000 hcpdiff-0.3.1/hcpdiff.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 03:50:19.000000 hcpdiff-0.3.1/hcpdiff.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-06 03:50:19.000000 hcpdiff-0.3.1/hcpdiff.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-06 03:50:19.000000 hcpdiff-0.3.1/hcpdiff.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-06 03:50:19.000000 hcpdiff-0.3.1/hcpdiff.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:50:19.108728 hcpdiff-0.3.1/prompt_tuning_template/
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-06 03:50:05.000000 hcpdiff-0.3.1/prompt_tuning_template/caption.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-06 03:50:05.000000 hcpdiff-0.3.1/prompt_tuning_template/name.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-06 03:50:05.000000 hcpdiff-0.3.1/prompt_tuning_template/name_2pt_caption.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-06 03:50:05.000000 hcpdiff-0.3.1/prompt_tuning_template/name_caption.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-05-06 03:50:05.000000 hcpdiff-0.3.1/prompt_tuning_template/object.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-06 03:50:05.000000 hcpdiff-0.3.1/prompt_tuning_template/object_caption.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-05-06 03:50:05.000000 hcpdiff-0.3.1/prompt_tuning_template/style.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-06 03:50:05.000000 hcpdiff-0.3.1/prompt_tuning_template/style_caption.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 03:50:19.112728 hcpdiff-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-05-06 03:50:05.000000 hcpdiff-0.3.1/setup.py
```

### Comparing `hcpdiff-0.3.0/LICENSE` & `hcpdiff-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.0/PKG-INFO` & `hcpdiff-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcpdiff
-Version: 0.3.0
+Version: 0.3.1
 Summary: A universal Stable-Diffusion toolbox
 Home-page: https://github.com/7eu7d7/HCP-Diffusion
 Author: Ziyi Dong
 Author-email: dzy7eu7d7@gmail.com
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hcpdiff-0.3.0/README.md` & `hcpdiff-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.0/cfgs/infer/euler_a.yaml` & `hcpdiff-0.3.1/cfgs/infer/euler_a.yaml`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.0/cfgs/infer/img2img.yaml` & `hcpdiff-0.3.1/cfgs/infer/img2img.yaml`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.0/cfgs/infer/img2img_controlnet.yaml` & `hcpdiff-0.3.1/cfgs/infer/img2img_controlnet.yaml`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.0/cfgs/infer/text2img.yaml` & `hcpdiff-0.3.1/cfgs/infer/text2img.yaml`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.0/cfgs/te_struct.txt` & `hcpdiff-0.3.1/cfgs/te_struct.txt`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.0/cfgs/train/examples/CustomDiffusion.yaml` & `hcpdiff-0.3.1/cfgs/train/examples/CustomDiffusion.yaml`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.0/cfgs/train/examples/DreamArtist++.yaml` & `hcpdiff-0.3.1/cfgs/train/examples/DreamArtist++.yaml`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.0/cfgs/train/examples/DreamArtist.yaml` & `hcpdiff-0.3.1/cfgs/train/examples/DreamArtist.yaml`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.0/cfgs/train/examples/DreamBooth.yaml` & `hcpdiff-0.3.1/cfgs/train/examples/DreamBooth.yaml`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.0/cfgs/train/examples/TextualInversion.yaml` & `hcpdiff-0.3.1/cfgs/train/examples/TextualInversion.yaml`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.0/cfgs/train/examples/controlnet.yaml` & `hcpdiff-0.3.1/cfgs/train/examples/controlnet.yaml`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.0/cfgs/train/examples/fine-tuning.yaml` & `hcpdiff-0.3.1/cfgs/train/examples/fine-tuning.yaml`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.0/cfgs/train/examples/locon.yaml` & `hcpdiff-0.3.1/cfgs/train/examples/locon.yaml`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.0/cfgs/train/examples/lora_conventional.yaml` & `hcpdiff-0.3.1/cfgs/train/examples/lora_conventional.yaml`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.0/cfgs/train/examples/min_snr.yaml` & `hcpdiff-0.3.1/cfgs/train/examples/min_snr.yaml`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.0/cfgs/train/train_base.yaml` & `hcpdiff-0.3.1/cfgs/train/train_base.yaml`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.0/cfgs/train/tuning_base.yaml` & `hcpdiff-0.3.1/cfgs/train/tuning_base.yaml`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.0/cfgs/unet_struct.txt` & `hcpdiff-0.3.1/cfgs/unet_struct.txt`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.0/hcpdiff/ckpt_manager/ckpt_pkl.py` & `hcpdiff-0.3.1/hcpdiff/ckpt_manager/ckpt_pkl.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.0/hcpdiff/ckpt_manager/ckpt_safetensor.py` & `hcpdiff-0.3.1/hcpdiff/ckpt_manager/ckpt_safetensor.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.0/hcpdiff/data/__init__.py` & `hcpdiff-0.3.1/hcpdiff/data/__init__.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.0/hcpdiff/data/bucket.py` & `hcpdiff-0.3.1/hcpdiff/data/bucket.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.0/hcpdiff/data/cond_pair_dataset.py` & `hcpdiff-0.3.1/hcpdiff/data/cond_pair_dataset.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.0/hcpdiff/data/pair_dataset.py` & `hcpdiff-0.3.1/hcpdiff/data/pair_dataset.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.0/hcpdiff/data/utils.py` & `hcpdiff-0.3.1/hcpdiff/data/utils.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.0/hcpdiff/loggers/base_logger.py` & `hcpdiff-0.3.1/hcpdiff/loggers/base_logger.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.0/hcpdiff/loggers/cli_logger.py` & `hcpdiff-0.3.1/hcpdiff/loggers/cli_logger.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.0/hcpdiff/loggers/tensorboard_logger.py` & `hcpdiff-0.3.1/hcpdiff/loggers/tensorboard_logger.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.0/hcpdiff/loggers/wandb_logger.py` & `hcpdiff-0.3.1/hcpdiff/loggers/wandb_logger.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.0/hcpdiff/loss/min_snr_loss.py` & `hcpdiff-0.3.1/hcpdiff/loss/min_snr_loss.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.0/hcpdiff/models/cfg_context.py` & `hcpdiff-0.3.1/hcpdiff/models/cfg_context.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.0/hcpdiff/models/controlnet.py` & `hcpdiff-0.3.1/hcpdiff/models/controlnet.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.0/hcpdiff/models/layers.py` & `hcpdiff-0.3.1/hcpdiff/models/layers.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.0/hcpdiff/models/lora_base.py` & `hcpdiff-0.3.1/hcpdiff/models/lora_base.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.0/hcpdiff/models/lora_layers.py` & `hcpdiff-0.3.1/hcpdiff/models/lora_layers.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.0/hcpdiff/models/plugin.py` & `hcpdiff-0.3.1/hcpdiff/models/plugin.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.0/hcpdiff/models/text_emb_ex.py` & `hcpdiff-0.3.1/hcpdiff/models/text_emb_ex.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.0/hcpdiff/models/textencoder_ex.py` & `hcpdiff-0.3.1/hcpdiff/models/textencoder_ex.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.0/hcpdiff/models/tokenizer_ex.py` & `hcpdiff-0.3.1/hcpdiff/models/tokenizer_ex.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.0/hcpdiff/tools/convert_caption_txt2json.py` & `hcpdiff-0.3.1/hcpdiff/tools/convert_caption_txt2json.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.0/hcpdiff/tools/create_embedding.py` & `hcpdiff-0.3.1/hcpdiff/tools/create_embedding.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.0/hcpdiff/tools/gen_from_ptlist.py` & `hcpdiff-0.3.1/hcpdiff/tools/gen_from_ptlist.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.0/hcpdiff/tools/init_proj.py` & `hcpdiff-0.3.1/hcpdiff/tools/init_proj.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.0/hcpdiff/train_ac.py` & `hcpdiff-0.3.1/hcpdiff/train_ac.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.0/hcpdiff/train_ac_single.py` & `hcpdiff-0.3.1/hcpdiff/train_ac_single.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.0/hcpdiff/train_colo.py` & `hcpdiff-0.3.1/hcpdiff/train_colo.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.0/hcpdiff/utils/caption_tools.py` & `hcpdiff-0.3.1/hcpdiff/utils/caption_tools.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.0/hcpdiff/utils/cfg_net_tools.py` & `hcpdiff-0.3.1/hcpdiff/utils/cfg_net_tools.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.0/hcpdiff/utils/colo_utils.py` & `hcpdiff-0.3.1/hcpdiff/utils/colo_utils.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.0/hcpdiff/utils/ema.py` & `hcpdiff-0.3.1/hcpdiff/utils/ema.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.0/hcpdiff/utils/img_size_tool.py` & `hcpdiff-0.3.1/hcpdiff/utils/img_size_tool.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.0/hcpdiff/utils/net_utils.py` & `hcpdiff-0.3.1/hcpdiff/utils/net_utils.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.0/hcpdiff/utils/utils.py` & `hcpdiff-0.3.1/hcpdiff/utils/utils.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.0/hcpdiff/visualizer.py` & `hcpdiff-0.3.1/hcpdiff/visualizer.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.0/hcpdiff.egg-info/PKG-INFO` & `hcpdiff-0.3.1/hcpdiff.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcpdiff
-Version: 0.3.0
+Version: 0.3.1
 Summary: A universal Stable-Diffusion toolbox
 Home-page: https://github.com/7eu7d7/HCP-Diffusion
 Author: Ziyi Dong
 Author-email: dzy7eu7d7@gmail.com
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hcpdiff-0.3.0/hcpdiff.egg-info/SOURCES.txt` & `hcpdiff-0.3.1/hcpdiff.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.0/prompt_tuning_template/object.txt` & `hcpdiff-0.3.1/prompt_tuning_template/object.txt`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.0/prompt_tuning_template/object_caption.txt` & `hcpdiff-0.3.1/prompt_tuning_template/object_caption.txt`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.0/prompt_tuning_template/style.txt` & `hcpdiff-0.3.1/prompt_tuning_template/style.txt`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.0/prompt_tuning_template/style_caption.txt` & `hcpdiff-0.3.1/prompt_tuning_template/style_caption.txt`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.0/setup.py` & `hcpdiff-0.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
             file_dict[prefix+root].append(os.path.join(root, name))
     return [(k, v) for k, v in file_dict.items()]
 
 
 setuptools.setup(
     name="hcpdiff",
     py_modules=["hcpdiff"],
-    version="0.3.0",
+    version="0.3.1",
     author="Ziyi Dong",
     author_email="dzy7eu7d7@gmail.com",
     description="A universal Stable-Diffusion toolbox",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/7eu7d7/HCP-Diffusion",
     packages=setuptools.find_packages(),
```

