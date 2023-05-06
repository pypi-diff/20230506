# Comparing `tmp/pytorch_optimizer-2.8.0.tar.gz` & `tmp/pytorch_optimizer-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytorch_optimizer-2.8.0.tar", max compression
+gzip compressed data, was "pytorch_optimizer-2.9.0.tar", max compression
```

## Comparing `pytorch_optimizer-2.8.0.tar` & `pytorch_optimizer-2.9.0.tar`

### file list

```diff
@@ -1,65 +1,72 @@
--rw-r--r--   0        0        0    11357 2023-04-29 08:52:01.235538 pytorch_optimizer-2.8.0/LICENSE
--rw-r--r--   0        0        0    38338 2023-04-29 08:52:01.235538 pytorch_optimizer-2.8.0/README.rst
--rw-r--r--   0        0        0     3807 2023-04-29 08:52:01.243538 pytorch_optimizer-2.8.0/pyproject.toml
--rw-r--r--   0        0        0     6858 2023-04-29 08:52:01.243538 pytorch_optimizer-2.8.0/pytorch_optimizer/__init__.py
--rw-r--r--   0        0        0        0 2023-04-29 08:52:01.243538 pytorch_optimizer-2.8.0/pytorch_optimizer/base/__init__.py
--rw-r--r--   0        0        0     1583 2023-04-29 08:52:01.243538 pytorch_optimizer-2.8.0/pytorch_optimizer/base/exception.py
--rw-r--r--   0        0        0     5782 2023-04-29 08:52:01.243538 pytorch_optimizer-2.8.0/pytorch_optimizer/base/optimizer.py
--rw-r--r--   0        0        0     2761 2023-04-29 08:52:01.243538 pytorch_optimizer-2.8.0/pytorch_optimizer/base/scheduler.py
--rw-r--r--   0        0        0      491 2023-04-29 08:52:01.243538 pytorch_optimizer-2.8.0/pytorch_optimizer/base/types.py
--rw-r--r--   0        0        0        0 2023-04-29 08:52:01.243538 pytorch_optimizer-2.8.0/pytorch_optimizer/experimental/__init__.py
--rw-r--r--   0        0        0     1595 2023-04-29 08:52:01.243538 pytorch_optimizer-2.8.0/pytorch_optimizer/experimental/deberta_v3_lr_scheduler.py
--rw-r--r--   0        0        0      131 2023-04-29 08:52:01.243538 pytorch_optimizer-2.8.0/pytorch_optimizer/lr_scheduler/__init__.py
--rw-r--r--   0        0        0      971 2023-04-29 08:52:01.243538 pytorch_optimizer-2.8.0/pytorch_optimizer/lr_scheduler/chebyshev.py
--rw-r--r--   0        0        0     4034 2023-04-29 08:52:01.243538 pytorch_optimizer-2.8.0/pytorch_optimizer/lr_scheduler/cosine_anealing.py
--rw-r--r--   0        0        0     1255 2023-04-29 08:52:01.243538 pytorch_optimizer-2.8.0/pytorch_optimizer/lr_scheduler/linear_warmup.py
--rw-r--r--   0        0        0     1400 2023-04-29 08:52:01.243538 pytorch_optimizer-2.8.0/pytorch_optimizer/lr_scheduler/proportion.py
--rw-r--r--   0        0        0        0 2023-04-29 08:52:01.243538 pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/__init__.py
--rw-r--r--   0        0        0     4401 2023-04-29 08:52:01.243538 pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/a2grad.py
--rw-r--r--   0        0        0     7547 2023-04-29 08:52:01.243538 pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/adabelief.py
--rw-r--r--   0        0        0     5515 2023-04-29 08:52:01.243538 pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/adabound.py
--rw-r--r--   0        0        0     8416 2023-04-29 08:52:01.243538 pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/adafactor.py
--rw-r--r--   0        0        0     6037 2023-04-29 08:52:01.243538 pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/adai.py
--rw-r--r--   0        0        0     4543 2023-04-29 08:52:01.243538 pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/adamod.py
--rw-r--r--   0        0        0     6166 2023-04-29 08:52:01.243538 pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/adamp.py
--rw-r--r--   0        0        0     6089 2023-04-29 08:52:01.243538 pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/adams.py
--rw-r--r--   0        0        0     6544 2023-04-29 08:52:01.243538 pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/adan.py
--rw-r--r--   0        0        0     5438 2023-04-29 08:52:01.243538 pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/adanorm.py
--rw-r--r--   0        0        0     6142 2023-04-29 08:52:01.243538 pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/adapnm.py
--rw-r--r--   0        0        0      781 2023-04-29 08:52:01.243538 pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/agc.py
--rw-r--r--   0        0        0     3113 2023-04-29 08:52:01.243538 pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/aggmo.py
--rw-r--r--   0        0        0     3873 2023-04-29 08:52:01.243538 pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/alig.py
--rw-r--r--   0        0        0     5498 2023-04-29 08:52:01.243538 pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/apollo.py
--rw-r--r--   0        0        0    24966 2023-04-29 08:52:01.243538 pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/dadapt.py
--rw-r--r--   0        0        0     7250 2023-04-29 08:52:01.243538 pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/diffgrad.py
--rw-r--r--   0        0        0    10702 2023-04-29 08:52:01.243538 pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/fp16.py
--rw-r--r--   0        0        0     2861 2023-04-29 08:52:01.243538 pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/fromage.py
--rw-r--r--   0        0        0      474 2023-04-29 08:52:01.243538 pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/gc.py
--rw-r--r--   0        0        0     7601 2023-04-29 08:52:01.243538 pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/gsam.py
--rw-r--r--   0        0        0     8607 2023-04-29 08:52:01.243538 pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/lamb.py
--rw-r--r--   0        0        0     3923 2023-04-29 08:52:01.243538 pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/lars.py
--rw-r--r--   0        0        0     4228 2023-04-29 08:52:01.243538 pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/lion.py
--rw-r--r--   0        0        0     4178 2023-04-29 08:52:01.243538 pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/lookahead.py
--rw-r--r--   0        0        0     6550 2023-04-29 08:52:01.243538 pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/madgrad.py
--rw-r--r--   0        0        0     3264 2023-04-29 08:52:01.243538 pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/msvag.py
--rw-r--r--   0        0        0     3639 2023-04-29 08:52:01.243538 pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/nero.py
--rw-r--r--   0        0        0     4188 2023-04-29 08:52:01.243538 pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/novograd.py
--rw-r--r--   0        0        0     4314 2023-04-29 08:52:01.243538 pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/pcgrad.py
--rw-r--r--   0        0        0     4146 2023-04-29 08:52:01.243538 pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/pid.py
--rw-r--r--   0        0        0     3615 2023-04-29 08:52:01.243538 pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/pnm.py
--rw-r--r--   0        0        0     4810 2023-04-29 08:52:01.243538 pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/qhadam.py
--rw-r--r--   0        0        0     3286 2023-04-29 08:52:01.243538 pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/qhm.py
--rw-r--r--   0        0        0     5748 2023-04-29 08:52:01.243538 pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/radam.py
--rw-r--r--   0        0        0     6969 2023-04-29 08:52:01.243538 pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/ranger.py
--rw-r--r--   0        0        0    12435 2023-04-29 08:52:01.243538 pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/ranger21.py
--rw-r--r--   0        0        0    15565 2023-04-29 08:52:01.243538 pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/rotograd.py
--rw-r--r--   0        0        0     4722 2023-04-29 08:52:01.243538 pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/sam.py
--rw-r--r--   0        0        0    10706 2023-04-29 08:52:01.243538 pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/sgd.py
--rw-r--r--   0        0        0     3921 2023-04-29 08:52:01.243538 pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/sgdp.py
--rw-r--r--   0        0        0    15801 2023-04-29 08:52:01.243538 pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/shampoo.py
--rw-r--r--   0        0        0    20180 2023-04-29 08:52:01.243538 pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/shampoo_utils.py
--rw-r--r--   0        0        0     5123 2023-04-29 08:52:01.243538 pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/sm3.py
--rw-r--r--   0        0        0     7169 2023-04-29 08:52:01.243538 pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/swats.py
--rw-r--r--   0        0        0     8880 2023-04-29 08:52:01.243538 pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/utils.py
--rw-r--r--   0        0        0     5115 2023-04-29 08:52:01.243538 pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/yogi.py
--rw-r--r--   0        0        0    40454 1970-01-01 00:00:00.000000 pytorch_optimizer-2.8.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-06 08:07:56.335615 pytorch_optimizer-2.9.0/LICENSE
+-rw-r--r--   0        0        0    60156 2023-05-06 08:07:56.335615 pytorch_optimizer-2.9.0/README.rst
+-rw-r--r--   0        0        0     4383 2023-05-06 08:07:56.343615 pytorch_optimizer-2.9.0/pyproject.toml
+-rw-r--r--   0        0        0     7354 2023-05-06 08:07:56.343615 pytorch_optimizer-2.9.0/pytorch_optimizer/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-06 08:07:56.343615 pytorch_optimizer-2.9.0/pytorch_optimizer/base/__init__.py
+-rw-r--r--   0        0        0     1583 2023-05-06 08:07:56.343615 pytorch_optimizer-2.9.0/pytorch_optimizer/base/exception.py
+-rw-r--r--   0        0        0     6913 2023-05-06 08:07:56.343615 pytorch_optimizer-2.9.0/pytorch_optimizer/base/optimizer.py
+-rw-r--r--   0        0        0     2761 2023-05-06 08:07:56.343615 pytorch_optimizer-2.9.0/pytorch_optimizer/base/scheduler.py
+-rw-r--r--   0        0        0      491 2023-05-06 08:07:56.343615 pytorch_optimizer-2.9.0/pytorch_optimizer/base/types.py
+-rw-r--r--   0        0        0      131 2023-05-06 08:07:56.343615 pytorch_optimizer-2.9.0/pytorch_optimizer/lr_scheduler/__init__.py
+-rw-r--r--   0        0        0      971 2023-05-06 08:07:56.343615 pytorch_optimizer-2.9.0/pytorch_optimizer/lr_scheduler/chebyshev.py
+-rw-r--r--   0        0        0     4034 2023-05-06 08:07:56.343615 pytorch_optimizer-2.9.0/pytorch_optimizer/lr_scheduler/cosine_anealing.py
+-rw-r--r--   0        0        0        0 2023-05-06 08:07:56.343615 pytorch_optimizer-2.9.0/pytorch_optimizer/lr_scheduler/experimental/__init__.py
+-rw-r--r--   0        0        0     1595 2023-05-06 08:07:56.343615 pytorch_optimizer-2.9.0/pytorch_optimizer/lr_scheduler/experimental/deberta_v3_lr_scheduler.py
+-rw-r--r--   0        0        0     1255 2023-05-06 08:07:56.343615 pytorch_optimizer-2.9.0/pytorch_optimizer/lr_scheduler/linear_warmup.py
+-rw-r--r--   0        0        0     1400 2023-05-06 08:07:56.343615 pytorch_optimizer-2.9.0/pytorch_optimizer/lr_scheduler/proportion.py
+-rw-r--r--   0        0        0        0 2023-05-06 08:07:56.343615 pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/__init__.py
+-rw-r--r--   0        0        0     4437 2023-05-06 08:07:56.343615 pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/a2grad.py
+-rw-r--r--   0        0        0     6701 2023-05-06 08:07:56.343615 pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/adabelief.py
+-rw-r--r--   0        0        0     5470 2023-05-06 08:07:56.343615 pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/adabound.py
+-rw-r--r--   0        0        0     3573 2023-05-06 08:07:56.343615 pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/adadelta.py
+-rw-r--r--   0        0        0     8782 2023-05-06 08:07:56.343615 pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/adafactor.py
+-rw-r--r--   0        0        0     6122 2023-05-06 08:07:56.343615 pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/adai.py
+-rw-r--r--   0        0        0     4976 2023-05-06 08:07:56.343615 pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/adamax.py
+-rw-r--r--   0        0        0     4664 2023-05-06 08:07:56.343615 pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/adamod.py
+-rw-r--r--   0        0        0     6501 2023-05-06 08:07:56.343615 pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/adamp.py
+-rw-r--r--   0        0        0     6417 2023-05-06 08:07:56.343615 pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/adams.py
+-rw-r--r--   0        0        0     6274 2023-05-06 08:07:56.343615 pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/adan.py
+-rw-r--r--   0        0        0     5253 2023-05-06 08:07:56.343615 pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/adanorm.py
+-rw-r--r--   0        0        0     6014 2023-05-06 08:07:56.343615 pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/adapnm.py
+-rw-r--r--   0        0        0     4169 2023-05-06 08:07:56.343615 pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/adashift.py
+-rw-r--r--   0        0        0     4138 2023-05-06 08:07:56.343615 pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/adasmooth.py
+-rw-r--r--   0        0        0      781 2023-05-06 08:07:56.343615 pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/agc.py
+-rw-r--r--   0        0        0     3172 2023-05-06 08:07:56.343615 pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/aggmo.py
+-rw-r--r--   0        0        0     3618 2023-05-06 08:07:56.343615 pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/alig.py
+-rw-r--r--   0        0        0     5290 2023-05-06 08:07:56.343615 pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/apollo.py
+-rw-r--r--   0        0        0     4803 2023-05-06 08:07:56.343615 pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/avagrad.py
+-rw-r--r--   0        0        0    25140 2023-05-06 08:07:56.343615 pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/dadapt.py
+-rw-r--r--   0        0        0     6749 2023-05-06 08:07:56.343615 pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/diffgrad.py
+-rw-r--r--   0        0        0    10702 2023-05-06 08:07:56.343615 pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/fp16.py
+-rw-r--r--   0        0        0     2764 2023-05-06 08:07:56.343615 pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/fromage.py
+-rw-r--r--   0        0        0      474 2023-05-06 08:07:56.343615 pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/gc.py
+-rw-r--r--   0        0        0     2517 2023-05-06 08:07:56.343615 pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/gravity.py
+-rw-r--r--   0        0        0     7544 2023-05-06 08:07:56.343615 pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/gsam.py
+-rw-r--r--   0        0        0     8316 2023-05-06 08:07:56.343615 pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/lamb.py
+-rw-r--r--   0        0        0     3546 2023-05-06 08:07:56.343615 pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/lars.py
+-rw-r--r--   0        0        0     4106 2023-05-06 08:07:56.343615 pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/lion.py
+-rw-r--r--   0        0        0     4113 2023-05-06 08:07:56.343615 pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/lookahead.py
+-rw-r--r--   0        0        0     6466 2023-05-06 08:07:56.343615 pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/madgrad.py
+-rw-r--r--   0        0        0     3172 2023-05-06 08:07:56.347616 pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/msvag.py
+-rw-r--r--   0        0        0     3595 2023-05-06 08:07:56.347616 pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/nero.py
+-rw-r--r--   0        0        0     4520 2023-05-06 08:07:56.347616 pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/novograd.py
+-rw-r--r--   0        0        0     4214 2023-05-06 08:07:56.347616 pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/pcgrad.py
+-rw-r--r--   0        0        0     4233 2023-05-06 08:07:56.347616 pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/pid.py
+-rw-r--r--   0        0        0     3741 2023-05-06 08:07:56.347616 pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/pnm.py
+-rw-r--r--   0        0        0     4827 2023-05-06 08:07:56.347616 pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/qhadam.py
+-rw-r--r--   0        0        0     3249 2023-05-06 08:07:56.347616 pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/qhm.py
+-rw-r--r--   0        0        0     5622 2023-05-06 08:07:56.347616 pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/radam.py
+-rw-r--r--   0        0        0     6744 2023-05-06 08:07:56.347616 pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/ranger.py
+-rw-r--r--   0        0        0    12772 2023-05-06 08:07:56.347616 pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/ranger21.py
+-rw-r--r--   0        0        0    15565 2023-05-06 08:07:56.347616 pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/rotograd.py
+-rw-r--r--   0        0        0     4638 2023-05-06 08:07:56.347616 pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/sam.py
+-rw-r--r--   0        0        0    10375 2023-05-06 08:07:56.347616 pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/sgd.py
+-rw-r--r--   0        0        0     4276 2023-05-06 08:07:56.347616 pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/sgdp.py
+-rw-r--r--   0        0        0    16132 2023-05-06 08:07:56.347616 pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/shampoo.py
+-rw-r--r--   0        0        0    20625 2023-05-06 08:07:56.347616 pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/shampoo_utils.py
+-rw-r--r--   0        0        0     5081 2023-05-06 08:07:56.347616 pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/sm3.py
+-rw-r--r--   0        0        0     2852 2023-05-06 08:07:56.347616 pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/srmm.py
+-rw-r--r--   0        0        0     7165 2023-05-06 08:07:56.347616 pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/swats.py
+-rw-r--r--   0        0        0     8832 2023-05-06 08:07:56.347616 pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/utils.py
+-rw-r--r--   0        0        0     5306 2023-05-06 08:07:56.347616 pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/yogi.py
+-rw-r--r--   0        0        0    62650 1970-01-01 00:00:00.000000 pytorch_optimizer-2.9.0/PKG-INFO
```

### Comparing `pytorch_optimizer-2.8.0/LICENSE` & `pytorch_optimizer-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.8.0/pyproject.toml` & `pytorch_optimizer-2.9.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "pytorch_optimizer"
-version = "2.8.0"
+version = "2.9.0"
 description = "optimizer & lr scheduler implementations in PyTorch with clean-code, strict types. Also, including useful optimization ideas."
 license = "Apache-2.0"
 authors = ["kozistr <kozistr@gmail.com>"]
 maintainers = ["kozistr <kozistr@gmail.com>"]
 readme = "README.rst"
 homepage = "https://github.com/kozistr/pytorch_optimizer"
 repository = "https://github.com/kozistr/pytorch_optimizer"
 documentation = "https://pytorch-optimizers.readthedocs.io/en/latest"
-keywords = ["pytorch", "deep-learning", "optimizer", "lr scheduler"]
+keywords = ["pytorch", "deep-learning", "optimizer", "lr scheduler", "A2Grad", "ASGD", "AccSGD", "AdaBelief", "AdaBound", "AdaDelta", "AdaFactor", "AdaMax", "AdaMod", "AdaNorm", "AdaPNM", "AdaSmooth", "Adai", "AdamP", "AdamS", "Adan", "AggMo", "AliG", "Apollo", "AvaGrad", "DAdaptAdaGrad", "DAdaptAdam", "DAdaptAdan", "DAdaptSGD", "DiffGrad", "Fromage", "Gravity", "LARS", "Lamb", "Lion", "MADGRAD", "MSVAG", "Nero", "NovoGrad", "PID", "PNM", "QHAdam", "QHM", "RAdam", "Ranger", "Ranger21", "SGDP", "SGDW", "SM3", "SRMM", "SWATS", "ScalableShampoo", "Shampoo", "Yogi", "SAM", "GSAM", "PCGrad", "RotoGrad"]
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Education",
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "Programming Language :: Python :: 3",
@@ -44,15 +44,15 @@
 
 [tool.poetry.dev-dependencies]
 isort = [
     { version = "==5.11.5", python = ">=3.7,<3.8"},
     { version = "^5.12.0", python = ">=3.8"}
 ]
 black = "^23.3.0"
-ruff = "^0.0.262"
+ruff = "^0.0.264"
 pytest = "^7.3.1"
 pytest-cov = "^4.0.0"
 
 [[tool.poetry.source]]
 name = "torch"
 url = "https://download.pytorch.org/whl/cpu"
 secondary = true
@@ -83,14 +83,15 @@
 target-version = "py39"
 
 [tool.ruff.per-file-ignores]
 "./hubconf.py" = ["D", "INP001"]
 "./tests/__init__.py" = ["D"]
 "./tests/constants.py" = ["D"]
 "./tests/utils.py" = ["D"]
+"./tests/test_base.py" = ["D", "S101"]
 "./tests/test_utils.py" = ["D", "S101"]
 "./tests/test_gradients.py" = ["D", "S101"]
 "./tests/test_optimizers.py" = ["D", "S101"]
 "./tests/test_optimizer_parameters.py" = ["D", "S101"]
 "./tests/test_general_optimizer_parameters.py" = ["D", "S101"]
 "./tests/test_load_optimizers.py" = ["D", "S101"]
 "./tests/test_load_lr_schedulers.py" = ["D", "S101"]
```

### Comparing `pytorch_optimizer-2.8.0/pytorch_optimizer/__init__.py` & `pytorch_optimizer-2.9.0/pytorch_optimizer/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,45 +1,51 @@
 # ruff: noqa
 from typing import Dict, List
 
 from torch import nn
 
 from pytorch_optimizer.base.types import OPTIMIZER, PARAMETERS, SCHEDULER
-from pytorch_optimizer.experimental.deberta_v3_lr_scheduler import deberta_v3_large_lr_scheduler
 from pytorch_optimizer.lr_scheduler import (
     ConstantLR,
     CosineAnnealingLR,
     CosineAnnealingWarmRestarts,
     CyclicLR,
     OneCycleLR,
 )
 from pytorch_optimizer.lr_scheduler.chebyshev import get_chebyshev_schedule
 from pytorch_optimizer.lr_scheduler.cosine_anealing import CosineAnnealingWarmupRestarts
+from pytorch_optimizer.lr_scheduler.experimental.deberta_v3_lr_scheduler import deberta_v3_large_lr_scheduler
 from pytorch_optimizer.lr_scheduler.linear_warmup import CosineScheduler, LinearScheduler, PolyScheduler
 from pytorch_optimizer.lr_scheduler.proportion import ProportionScheduler
 from pytorch_optimizer.optimizer.a2grad import A2Grad
 from pytorch_optimizer.optimizer.adabelief import AdaBelief
 from pytorch_optimizer.optimizer.adabound import AdaBound
+from pytorch_optimizer.optimizer.adadelta import AdaDelta
 from pytorch_optimizer.optimizer.adafactor import AdaFactor
 from pytorch_optimizer.optimizer.adai import Adai
+from pytorch_optimizer.optimizer.adamax import AdaMax
 from pytorch_optimizer.optimizer.adamod import AdaMod
 from pytorch_optimizer.optimizer.adamp import AdamP
 from pytorch_optimizer.optimizer.adams import AdamS
 from pytorch_optimizer.optimizer.adan import Adan
 from pytorch_optimizer.optimizer.adanorm import AdaNorm
 from pytorch_optimizer.optimizer.adapnm import AdaPNM
+from pytorch_optimizer.optimizer.adashift import AdaShift
+from pytorch_optimizer.optimizer.adasmooth import AdaSmooth
 from pytorch_optimizer.optimizer.agc import agc
 from pytorch_optimizer.optimizer.aggmo import AggMo
 from pytorch_optimizer.optimizer.alig import AliG
 from pytorch_optimizer.optimizer.apollo import Apollo
+from pytorch_optimizer.optimizer.avagrad import AvaGrad
 from pytorch_optimizer.optimizer.dadapt import DAdaptAdaGrad, DAdaptAdam, DAdaptAdan, DAdaptSGD
 from pytorch_optimizer.optimizer.diffgrad import DiffGrad
 from pytorch_optimizer.optimizer.fp16 import DynamicLossScaler, SafeFP16Optimizer
 from pytorch_optimizer.optimizer.fromage import Fromage
 from pytorch_optimizer.optimizer.gc import centralize_gradient
+from pytorch_optimizer.optimizer.gravity import Gravity
 from pytorch_optimizer.optimizer.gsam import GSAM
 from pytorch_optimizer.optimizer.lamb import Lamb
 from pytorch_optimizer.optimizer.lars import LARS
 from pytorch_optimizer.optimizer.lion import Lion
 from pytorch_optimizer.optimizer.lookahead import Lookahead
 from pytorch_optimizer.optimizer.madgrad import MADGRAD
 from pytorch_optimizer.optimizer.msvag import MSVAG
@@ -70,14 +76,15 @@
     SQRTNGraft,
     compute_power_schur_newton,
     compute_power_svd,
     merge_small_dims,
     power_iteration,
 )
 from pytorch_optimizer.optimizer.sm3 import SM3
+from pytorch_optimizer.optimizer.srmm import SRMM
 from pytorch_optimizer.optimizer.swats import SWATS
 from pytorch_optimizer.optimizer.utils import (
     clip_grad_norm,
     disable_running_stats,
     enable_running_stats,
     get_global_gradient_norm,
     get_optimizer_parameters,
@@ -127,14 +134,21 @@
     SM3,
     AdaNorm,
     A2Grad,
     AccSGD,
     SGDW,
     Yogi,
     ASGD,
+    AdaMax,
+    Gravity,
+    AdaSmooth,
+    SRMM,
+    AvaGrad,
+    AdaShift,
+    AdaDelta,
 ]
 OPTIMIZERS: Dict[str, OPTIMIZER] = {str(optimizer.__name__).lower(): optimizer for optimizer in OPTIMIZER_LIST}
 
 LR_SCHEDULER_LIST: List[SCHEDULER] = [
     CosineAnnealingWarmupRestarts,
     ConstantLR,
     CosineAnnealingLR,
```

### Comparing `pytorch_optimizer-2.8.0/pytorch_optimizer/base/exception.py` & `pytorch_optimizer-2.9.0/pytorch_optimizer/base/exception.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.8.0/pytorch_optimizer/base/scheduler.py` & `pytorch_optimizer-2.9.0/pytorch_optimizer/base/scheduler.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.8.0/pytorch_optimizer/experimental/deberta_v3_lr_scheduler.py` & `pytorch_optimizer-2.9.0/pytorch_optimizer/lr_scheduler/experimental/deberta_v3_lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.8.0/pytorch_optimizer/lr_scheduler/chebyshev.py` & `pytorch_optimizer-2.9.0/pytorch_optimizer/lr_scheduler/chebyshev.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.8.0/pytorch_optimizer/lr_scheduler/cosine_anealing.py` & `pytorch_optimizer-2.9.0/pytorch_optimizer/lr_scheduler/cosine_anealing.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.8.0/pytorch_optimizer/lr_scheduler/linear_warmup.py` & `pytorch_optimizer-2.9.0/pytorch_optimizer/lr_scheduler/linear_warmup.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.8.0/pytorch_optimizer/lr_scheduler/proportion.py` & `pytorch_optimizer-2.9.0/pytorch_optimizer/lr_scheduler/proportion.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/a2grad.py` & `pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/a2grad.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,60 +11,57 @@
 
 class A2Grad(Optimizer, BaseOptimizer):
     r"""Optimal Adaptive and Accelerated Stochastic Gradient Descent.
 
     :param params: PARAMETERS. iterable of parameters to optimize or dicts defining parameter groups.
     :param lr: Optional[float]. learning rate. no needed.
     :param beta: float. beta.
-    :param lips. float. Lipschitz constant.
+    :param lips: float. Lipschitz constant.
     :param rho: float. represents the degree of weighting decrease, a constant smoothing factor between 0 and 1.
     :param variant: str. type of A2Grad optimizer. 'uni', 'inc', 'exp'.
     """
 
     def __init__(
         self,
         params: PARAMETERS,
-        lr: Optional[None] = None,
+        lr: Optional[float] = None,
         beta: float = 10.0,
         lips: float = 10.0,
         rho: float = 0.5,
         variant: str = 'uni',
     ):
-        self.lr = lr
-        self.beta = beta
-        self.lips = lips
-        self.rho = rho
-        self.variant = variant
+        self.validate_learning_rate(lr)
+        self.validate_non_negative(lips, 'lips')
+        self.validate_non_negative(rho, 'rho')
+        self.validate_a2grad_variant(variant)
 
-        self.validate_parameters()
+        self.variant = variant
 
         defaults: DEFAULTS = {'beta': beta, 'lips': lips}
         if variant == 'exp':
             defaults.update({'rho': rho})
 
         super().__init__(params, defaults)
 
-    def validate_parameters(self):
-        self.validate_lipschitz_constant(self.lips)
-        self.validate_rho(self.rho)
-        self.validate_a2grad_variant(self.variant)
-
     def __str__(self) -> str:
         return 'A2Grad'
 
     @torch.no_grad()
     def reset(self):
         for group in self.param_groups:
+            group['step'] = 0
             for p in group['params']:
                 state = self.state[p]
 
                 state['alpha_k'] = 1.0
                 state['v_k'] = torch.zeros((1,), dtype=p.dtype, device=p.device)
                 state['avg_grad'] = torch.zeros_like(p)
                 state['x_k'] = p.clone()
+                if self.variant == 'exp':
+                    state['v_kk'] = torch.zeros((1,), dtype=p.dtype, device=p.device)
 
     @torch.no_grad()
     def step(self, closure: CLOSURE = None) -> LOSS:
         loss: LOSS = None
         if closure is not None:
             with torch.enable_grad():
                 loss = closure()
@@ -83,15 +80,14 @@
                     continue
 
                 grad = p.grad
                 if grad.is_sparse:
                     raise NoSparseGradientError(str(self))
 
                 state = self.state[p]
-
                 if len(state) == 0:
                     state['alpha_k'] = 1.0
                     state['v_k'] = torch.zeros((1,), dtype=grad.dtype, device=grad.device)
                     state['avg_grad'] = grad.clone()
                     state['x_k'] = p.clone()
                     if self.variant == 'exp':
                         state['v_kk'] = torch.zeros((1,), dtype=grad.dtype, device=grad.device)
```

### Comparing `pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/adabelief.py` & `pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/lamb.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,196 +1,217 @@
-import math
+from typing import Union
 
 import torch
-from torch.optim.optimizer import Optimizer
+from torch.optim import Optimizer
 
 from pytorch_optimizer.base.exception import NoSparseGradientError
 from pytorch_optimizer.base.optimizer import BaseOptimizer
 from pytorch_optimizer.base.types import BETAS, CLOSURE, DEFAULTS, LOSS, PARAMETERS
+from pytorch_optimizer.optimizer.utils import get_global_gradient_norm
 
 
-class AdaBelief(Optimizer, BaseOptimizer):
-    r"""Adapting Step-sizes by the Belief in Observed Gradients.
+class Lamb(Optimizer, BaseOptimizer):
+    r"""Large Batch Optimization for Deep Learning.
+
+        This Lamb implementation is based on the paper v3, which does not use de-biasing.
 
     :param params: PARAMETERS. iterable of parameters to optimize or dicts defining parameter groups.
     :param lr: float. learning rate.
     :param betas: BETAS. coefficients used for computing running averages of gradient and the squared hessian trace.
     :param weight_decay: float. weight decay (L2 penalty).
-    :param n_sma_threshold: number of SMA threshold (recommended is 5).
     :param weight_decouple: bool. the optimizer uses decoupled weight decay as in AdamW.
     :param fixed_decay: bool. fix weight decay.
     :param rectify: bool. perform the rectified update similar to RAdam.
-    :param degenerated_to_sgd: bool. perform SGD update when variance of gradient is high.
-    :param amsgrad: bool. whether to use the AMSBound variant.
+    :param degenerated_to_sgd: bool. degenerated to SGD.
+    :param n_sma_threshold: int. (recommended is 5).
+    :param grad_averaging: bool. whether apply (1 - beta2) to gradient when calculating running averages of gradient.
+    :param max_grad_norm: float. max gradient norm to clip.
     :param r: float. EMA factor. between 0.9 ~ 0.99 is preferred.
     :param adanorm: bool. whether to use the AdaNorm variant.
     :param adam_debias: bool. Only correct the denominator to avoid inflating step sizes early in training.
+    :param adam: bool. always use trust ratio = 1, which turns this into Adam. Useful for comparison purposes.
+    :param pre_norm: bool. perform pre-normalization of all gradients.
     :param eps: float. term added to the denominator to improve numerical stability.
     """
 
+    clamp: float = 10.0
+
     def __init__(
         self,
         params: PARAMETERS,
         lr: float = 1e-3,
         betas: BETAS = (0.9, 0.999),
         weight_decay: float = 0.0,
-        n_sma_threshold: int = 5,
         weight_decouple: bool = True,
         fixed_decay: bool = False,
-        rectify: bool = True,
-        degenerated_to_sgd: bool = True,
-        amsgrad: bool = False,
+        rectify: bool = False,
+        degenerated_to_sgd: bool = False,
+        n_sma_threshold: int = 5,
+        grad_averaging: bool = True,
+        max_grad_norm: float = 1.0,
+        adam: bool = False,
+        pre_norm: bool = False,
         r: float = 0.95,
         adanorm: bool = False,
         adam_debias: bool = False,
-        eps: float = 1e-16,
+        eps: float = 1e-6,
     ):
-        self.lr = lr
-        self.betas = betas
-        self.weight_decay = weight_decay
-        self.n_sma_threshold = n_sma_threshold
-        self.degenerated_to_sgd = degenerated_to_sgd
-        self.eps = eps
+        self.validate_learning_rate(lr)
+        self.validate_betas(betas)
+        self.validate_non_negative(weight_decay, 'weight_decay')
+        self.validate_non_negative(max_grad_norm, 'max_grad_norm')
+        self.validate_non_negative(eps, 'eps')
 
-        self.validate_parameters()
+        self.degenerated_to_sgd = degenerated_to_sgd
+        self.n_sma_threshold = n_sma_threshold
+        self.pre_norm = pre_norm
 
         defaults: DEFAULTS = {
             'lr': lr,
             'betas': betas,
             'weight_decay': weight_decay,
             'weight_decouple': weight_decouple,
             'fixed_decay': fixed_decay,
             'rectify': rectify,
-            'amsgrad': amsgrad,
+            'grad_averaging': grad_averaging,
+            'max_grad_norm': max_grad_norm,
+            'adam': adam,
             'adanorm': adanorm,
             'adam_debias': adam_debias,
             'eps': eps,
         }
         if adanorm:
             defaults.update({'r': r})
 
         super().__init__(params, defaults)
 
-    def validate_parameters(self):
-        self.validate_learning_rate(self.lr)
-        self.validate_betas(self.betas)
-        self.validate_weight_decay(self.weight_decay)
-        self.validate_epsilon(self.eps)
-
     def __str__(self) -> str:
-        return 'AdaBelief'
+        return 'Lamb'
 
     @torch.no_grad()
     def reset(self):
         for group in self.param_groups:
-            group['step'] = 0
             for p in group['params']:
                 state = self.state[p]
 
+                state['step'] = 0
                 state['exp_avg'] = torch.zeros_like(p)
-                state['exp_avg_var'] = torch.zeros_like(p)
+                state['exp_avg_sq'] = torch.zeros_like(p)
                 if group['adanorm']:
                     state['exp_grad_norm'] = torch.zeros((1,), dtype=p.dtype, device=p.device)
-                if group['amsgrad']:
-                    state['max_exp_avg_var'] = torch.zeros_like(p)
+
+    @torch.no_grad()
+    def get_global_gradient_norm(self) -> Union[torch.Tensor, float]:
+        if self.defaults['max_grad_norm'] == 0.0:
+            return 1.0
+
+        global_grad_norm = get_global_gradient_norm(self.param_groups, self.param_groups[0]['params'][0].device)
+        global_grad_norm.sqrt_().add_(self.defaults['eps'])
+
+        return torch.clamp(self.defaults['max_grad_norm'] / global_grad_norm, max=1.0)
 
     @torch.no_grad()
     def step(self, closure: CLOSURE = None) -> LOSS:
         loss: LOSS = None
         if closure is not None:
             with torch.enable_grad():
                 loss = closure()
 
+        grad_norm = 1.0
+        if self.pre_norm:
+            grad_norm = self.get_global_gradient_norm()
+
         for group in self.param_groups:
             if 'step' in group:
                 group['step'] += 1
             else:
                 group['step'] = 1
 
             beta1, beta2 = group['betas']
-            weight_decay = group['weight_decay']
 
-            bias_correction1 = 1.0 - beta1 ** group['step']
-            bias_correction2_sq = math.sqrt(1.0 - beta2 ** group['step'])
+            beta3: float = 1.0 - beta1 if group['grad_averaging'] else 1.0
+            bias_correction1: float = 1.0 - beta1 ** group['step']
 
-            if group['rectify']:
-                n_sma_max: float = 2.0 / (1.0 - beta2) - 1.0
-                beta2_t: float = beta2 ** group['step']
-                n_sma: float = n_sma_max - 2 * group['step'] * beta2_t / (1.0 - beta2_t)
+            step_size, n_sma = self.get_rectify_step_size(
+                is_rectify=group['rectify'],
+                step=group['step'],
+                lr=group['lr'],
+                beta2=beta2,
+                n_sma_threshold=self.n_sma_threshold,
+                degenerated_to_sgd=self.degenerated_to_sgd,
+            )
+
+            step_size = self.apply_adam_debias(
+                adam_debias=group['adam_debias'],
+                step_size=step_size,
+                bias_correction1=bias_correction1,
+            )
 
             for p in group['params']:
                 if p.grad is None:
                     continue
 
                 grad = p.grad
                 if grad.is_sparse:
                     raise NoSparseGradientError(str(self))
 
+                if self.pre_norm:
+                    grad.div_(grad_norm)
+
                 state = self.state[p]
+
                 if len(state) == 0:
                     state['exp_avg'] = torch.zeros_like(p)
-                    state['exp_avg_var'] = torch.zeros_like(p)
+                    state['exp_avg_sq'] = torch.zeros_like(p)
                     if group['adanorm']:
                         state['exp_grad_norm'] = torch.zeros((1,), dtype=grad.dtype, device=grad.device)
-                    if group['amsgrad']:
-                        state['max_exp_avg_var'] = torch.zeros_like(p)
-
-                if group['weight_decouple']:
-                    p.mul_(1.0 - group['weight_decay'] * (1.0 if group['fixed_decay'] else group['lr']))
-                elif weight_decay > 0.0:
-                    grad.add_(p, alpha=weight_decay)
-
-                exp_avg, exp_avg_var = state['exp_avg'], state['exp_avg_var']
-
-                s_grad = grad
-                if group['adanorm']:
-                    grad_norm = torch.linalg.norm(grad)
-
-                    exp_grad_norm = state['exp_grad_norm']
-                    exp_grad_norm.mul_(group['r']).add_(grad_norm, alpha=1.0 - group['r'])
 
-                    if exp_grad_norm > grad_norm:
-                        s_grad *= exp_grad_norm / grad_norm
-
-                exp_avg.mul_(beta1).add_(s_grad, alpha=1.0 - beta1)
-                grad_residual = s_grad - exp_avg
-                exp_avg_var.mul_(beta2).addcmul_(grad_residual, grad_residual, value=1.0 - beta2).add_(self.eps)
-
-                if group['amsgrad']:
-                    max_exp_avg_var = state['max_exp_avg_var']
-                    torch.max(max_exp_avg_var, exp_avg_var, out=max_exp_avg_var)
-                    de_nom = max_exp_avg_var.add(self.eps).sqrt()
+                s_grad = self.get_adanorm_gradient(
+                    grad=grad,
+                    adanorm=group['adanorm'],
+                    exp_grad_norm=state.get('exp_grad_norm', None),
+                    r=group.get('r', None),
+                )
+
+                exp_avg, exp_avg_sq = state['exp_avg'], state['exp_avg_sq']
+                exp_avg.mul_(beta1).add_(s_grad, alpha=beta3)
+                exp_avg_sq.mul_(beta2).addcmul_(grad, grad, value=1.0 - beta2)
+
+                self.apply_weight_decay(
+                    p=p,
+                    grad=None,
+                    lr=group['lr'],
+                    weight_decay=group['weight_decay'],
+                    weight_decouple=group['weight_decouple'],
+                    fixed_decay=group['fixed_decay'],
+                )
+
+                if group['rectify']:
+                    update = p.clone()
+                    if n_sma >= self.n_sma_threshold:
+                        de_nom = exp_avg_sq.sqrt().add_(group['eps'])
+                        update.addcdiv_(exp_avg, de_nom, value=-step_size)
+                    else:
+                        update.add_(exp_avg, alpha=-step_size)
                 else:
-                    de_nom = exp_avg_var.add(self.eps).sqrt()
-
-                de_nom.div_(bias_correction2_sq).add_(self.eps)
-
-                if not group['rectify']:
-                    step_size: float = group['lr'] if group['adam_debias'] else group['lr'] / bias_correction1
-                    p.addcdiv_(exp_avg, de_nom, value=-step_size)
-                    continue
+                    update = exp_avg / exp_avg_sq.sqrt().add_(group['eps'])
 
-                if n_sma >= self.n_sma_threshold:
-                    step_size = math.sqrt(
-                        (1 - beta2_t)
-                        * (n_sma - 4)
-                        / (n_sma_max - 4)
-                        * (n_sma - 2)
-                        / n_sma
-                        * n_sma_max
-                        / (n_sma_max - 2)
-                    )
-                elif self.degenerated_to_sgd:
-                    step_size = 1.0
+                weight_norm = torch.linalg.norm(p).clamp_(min=0, max=self.clamp)
+                p_norm = torch.linalg.norm(update)
+                trust_ratio: float = 1.0 if weight_norm == 0 or p_norm == 0 else weight_norm / (p_norm + group['eps'])
+
+                state['weight_norm'] = weight_norm
+                state['adam_norm'] = p_norm
+                state['trust_ratio'] = trust_ratio
+
+                if group['adam']:
+                    trust_ratio = 1.0
+
+                if group['rectify']:
+                    if n_sma >= self.n_sma_threshold:
+                        p.addcdiv_(exp_avg, de_nom, value=-step_size * trust_ratio)
+                    else:
+                        p.add_(exp_avg, alpha=-step_size * trust_ratio)
                 else:
-                    step_size = -1
-
-                if not group['adam_debias']:
-                    step_size /= bias_correction1
-
-                if n_sma >= self.n_sma_threshold:
-                    de_nom = exp_avg_var.sqrt().add_(self.eps)
-                    p.addcdiv_(exp_avg, de_nom, value=-step_size * group['lr'])
-                elif step_size > 0:
-                    p.add_(exp_avg, alpha=-step_size * group['lr'])
+                    p.add_(update, alpha=-step_size * trust_ratio)
 
         return loss
```

### Comparing `pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/adabound.py` & `pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/adabound.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,75 +16,67 @@
     :param lr: float. learning rate.
     :param final_lr: float. final learning rate.
     :param betas: BETAS. coefficients used for computing running averages of gradient and the squared hessian trace.
     :param gamma: float. convergence speed of the bound functions.
     :param weight_decay: float. weight decay (L2 penalty).
     :param weight_decouple: bool. the optimizer uses decoupled weight decay as in AdamW.
     :param fixed_decay: bool. fix weight decay.
-    :param amsbound: bool. whether to use the AMSBound variant.
-    :param adam_debias_term: bool. Only correct the denominator to avoid inflating step sizes early in training.
+    :param ams_bound: bool. whether to use the AMSBound variant.
+    :param adam_debias: bool. Only correct the denominator to avoid inflating step sizes early in training.
     :param eps: float. term added to the denominator to improve numerical stability.
     """
 
     def __init__(
         self,
         params: PARAMETERS,
         lr: float = 1e-3,
         final_lr: float = 1e-1,
         betas: BETAS = (0.9, 0.999),
         gamma: float = 1e-3,
         weight_decay: float = 0.0,
         weight_decouple: bool = True,
         fixed_decay: bool = False,
-        amsbound: bool = False,
+        ams_bound: bool = False,
         adam_debias: bool = False,
         eps: float = 1e-8,
     ):
-        self.lr = lr
-        self.betas = betas
-        self.weight_decay = weight_decay
-        self.eps = eps
-
-        self.validate_parameters()
+        self.validate_learning_rate(lr)
+        self.validate_betas(betas)
+        self.validate_non_negative(weight_decay, 'weight_decay')
+        self.validate_non_negative(eps, 'eps')
 
         defaults: DEFAULTS = {
             'lr': lr,
             'betas': betas,
             'final_lr': final_lr,
             'gamma': gamma,
             'weight_decay': weight_decay,
             'weight_decouple': weight_decouple,
             'fixed_decay': fixed_decay,
-            'amsbound': amsbound,
+            'ams_bound': ams_bound,
             'adam_debias': adam_debias,
             'eps': eps,
         }
         super().__init__(params, defaults)
 
         self.base_lrs: List[float] = [group['lr'] for group in self.param_groups]
 
-    def validate_parameters(self):
-        self.validate_learning_rate(self.lr)
-        self.validate_betas(self.betas)
-        self.validate_weight_decay(self.weight_decay)
-        self.validate_epsilon(self.eps)
-
     def __str__(self) -> str:
         return 'AdaBound'
 
     @torch.no_grad()
     def reset(self):
         for group in self.param_groups:
+            group['step'] = 0
             for p in group['params']:
                 state = self.state[p]
 
-                state['step'] = 0
                 state['exp_avg'] = torch.zeros_like(p)
                 state['exp_avg_sq'] = torch.zeros_like(p)
-                if group['amsbound']:
+                if group['ams_bound']:
                     state['max_exp_avg_sq'] = torch.zeros_like(p)
 
     @torch.no_grad()
     def step(self, closure: CLOSURE = None) -> LOSS:
         loss: LOSS = None
         if closure is not None:
             with torch.enable_grad():
@@ -94,57 +86,62 @@
             if 'step' in group:
                 group['step'] += 1
             else:
                 group['step'] = 1
 
             beta1, beta2 = group['betas']
 
-            bias_correction1 = 1.0 - beta1 ** group['step']
-            bias_correction2_sq = math.sqrt(1.0 - beta2 ** group['step'])
+            bias_correction1: float = 1.0 - beta1 ** group['step']
+            bias_correction2_sq: float = math.sqrt(1.0 - beta2 ** group['step'])
 
-            final_lr = group['final_lr'] * group['lr'] / base_lr
-            lower_bound = final_lr * (1 - 1 / (group['gamma'] * group['step'] + 1))
-            upper_bound = final_lr * (1 + 1 / (group['gamma'] * group['step']))
+            final_lr: float = group['final_lr'] * group['lr'] / base_lr
+            lower_bound: float = final_lr * (1 - 1 / (group['gamma'] * group['step'] + 1))
+            upper_bound: float = final_lr * (1 + 1 / (group['gamma'] * group['step']))
 
             for p in group['params']:
                 if p.grad is None:
                     continue
 
                 grad = p.grad
                 if grad.is_sparse:
                     raise NoSparseGradientError(str(self))
 
                 state = self.state[p]
 
                 if len(state) == 0:
                     state['exp_avg'] = torch.zeros_like(p)
                     state['exp_avg_sq'] = torch.zeros_like(p)
-                    if group['amsbound']:
+                    if group['ams_bound']:
                         state['max_exp_avg_sq'] = torch.zeros_like(p)
 
-                if group['weight_decouple']:
-                    p.mul_(1.0 - group['weight_decay'] * (1.0 if group['fixed_decay'] else group['lr']))
-                elif group['weight_decay'] > 0.0:
-                    grad.add_(p, alpha=group['weight_decay'])
+                self.apply_weight_decay(
+                    p=p,
+                    grad=grad,
+                    lr=group['lr'],
+                    weight_decay=group['weight_decay'],
+                    weight_decouple=group['weight_decouple'],
+                    fixed_decay=group['fixed_decay'],
+                )
 
                 exp_avg, exp_avg_sq = state['exp_avg'], state['exp_avg_sq']
-
                 exp_avg.mul_(beta1).add_(grad, alpha=1.0 - beta1)
                 exp_avg_sq.mul_(beta2).addcmul_(grad, grad, value=1.0 - beta2)
 
-                if group['amsbound']:
-                    max_exp_avg_sq = state['max_exp_avg_sq']
-                    torch.max(max_exp_avg_sq, exp_avg_sq, out=max_exp_avg_sq)
-                    de_nom = max_exp_avg_sq.add(group['eps']).sqrt()
-                else:
-                    de_nom = exp_avg_sq.add(group['eps']).sqrt()
-
-                step_size = group['lr'] * bias_correction2_sq
-                if not group['adam_debias']:
-                    step_size /= bias_correction1
+                de_nom = self.apply_ams_bound(
+                    ams_bound=group['ams_bound'],
+                    exp_avg_sq=exp_avg_sq,
+                    max_exp_avg_sq=state.get('max_exp_avg_sq', None),
+                    eps=group['eps'],
+                )
+
+                step_size = self.apply_adam_debias(
+                    adam_debias=group['adam_debias'],
+                    step_size=group['lr'] * bias_correction2_sq,
+                    bias_correction1=bias_correction1,
+                )
 
-                step_size = torch.full_like(de_nom, step_size)
-                step_size.div_(de_nom).clamp_(lower_bound, upper_bound).mul_(exp_avg)
+                step_size = torch.full_like(de_nom, fill_value=step_size)
+                step_size.div_(de_nom).clamp_(min=lower_bound, max=upper_bound).mul_(exp_avg)
 
                 p.add_(-step_size)
 
         return loss
```

### Comparing `pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/adafactor.py` & `pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/adafactor.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,16 +13,18 @@
     r"""Adaptive Learning Rates with Sublinear Memory Cost.
 
     :param params: PARAMETERS. iterable of parameters to optimize or dicts defining parameter groups.
     :param lr: float. learning rate.
     :param betas: BETAS. coefficients used for computing running averages of gradient and the squared hessian trace.
     :param decay_rate: float. coefficient used to compute running averages of square gradient.
     :param weight_decay: float. weight decay (L2 penalty).
+    :param weight_decouple: bool. the optimizer uses decoupled weight decay as in AdamW.
+    :param fixed_decay: bool. fix weight decay.
     :param clip_threshold: float. threshold of root-mean-square of final gradient update.
-    :param amsgrad: bool. whether to use the AMSBound variant.
+    :param ams_bound: bool. whether to use the AMSBound variant.
     :param scale_parameter: bool. if true, learning rate is scaled by root-mean-square of parameter.
     :param relative_step: bool. if true, time-dependent learning rate is computed instead of external learning rate.
     :param warmup_init: bool. time-dependent learning rate computation depends on whether warm-up initialization
         is being used.
     :param eps1: float. term added to the denominator to improve numerical stability.
     :param eps2: float. term added to the denominator to improve numerical stability.
     """
@@ -30,53 +32,50 @@
     def __init__(
         self,
         params: PARAMETERS,
         lr: Optional[float] = 1e-3,
         betas: BETAS = (0.9, 0.999),
         decay_rate: float = -0.8,
         weight_decay: float = 0.0,
+        weight_decouple: bool = True,
+        fixed_decay: bool = False,
         clip_threshold: float = 1.0,
-        amsgrad: bool = False,
+        ams_bound: bool = False,
         scale_parameter: bool = True,
         relative_step: bool = True,
         warmup_init: bool = False,
         eps1: float = 1e-30,
         eps2: float = 1e-3,
     ):
-        self.lr = lr
-        self.betas = betas
+        self.validate_learning_rate(lr)
+        self.validate_betas(betas)
+        self.validate_non_negative(weight_decay, 'weight_decay')
+        self.validate_non_negative(eps1, 'eps1')
+        self.validate_non_negative(eps2, 'eps2')
+
         self.decay_rate = decay_rate
-        self.weight_decay = weight_decay
         self.clip_threshold = clip_threshold
-        self.amsgrad = amsgrad
-        self.relative_step = relative_step
         self.eps1 = eps1
         self.eps2 = eps2
 
-        self.validate_parameters()
-
         defaults: DEFAULTS = {
             'lr': lr,
+            'betas': betas,
             'weight_decay': weight_decay,
-            'amsgrad': amsgrad,
+            'weight_decouple': weight_decouple,
+            'fixed_decay': fixed_decay,
+            'ams_bound': ams_bound,
             'scale_parameter': scale_parameter,
             'relative_step': relative_step,
             'warmup_init': warmup_init,
             'eps1': eps1,
             'eps2': eps2,
         }
         super().__init__(params, defaults)
 
-    def validate_parameters(self):
-        self.validate_learning_rate(self.lr)
-        self.validate_betas(self.betas)
-        self.validate_weight_decay(self.weight_decay)
-        self.validate_epsilon(self.eps1)
-        self.validate_epsilon(self.eps2)
-
     def __str__(self) -> str:
         return 'AdaFactor'
 
     @torch.no_grad()
     def reset(self):
         for group in self.param_groups:
             group['step'] = 0
@@ -94,15 +93,15 @@
                     state['exp_avg_sq_row'] = torch.zeros(grad_shape[:-1], dtype=grad.dtype, device=grad.device)
                     state['exp_avg_sq_col'] = torch.zeros(
                         grad_shape[:-2] + grad_shape[-1:], dtype=grad.dtype, device=grad.device
                     )
                 else:
                     state['exp_avg_sq'] = torch.zeros_like(grad)
 
-                if group['amsgrad']:
+                if group['ams_bound']:
                     state['exp_avg_sq_hat'] = torch.zeros_like(grad)
 
                 state['RMS'] = 0.0
 
     def get_lr(
         self, lr: float, step: int, rms: float, relative_step: bool, warmup_init: bool, scale_parameter: bool
     ) -> float:
@@ -146,14 +145,16 @@
 
         for group in self.param_groups:
             if 'step' in group:
                 group['step'] += 1
             else:
                 group['step'] = 1
 
+            beta1, _ = group['betas']
+
             beta2_t: float = 1.0 - math.pow(group['step'], self.decay_rate)
 
             for p in group['params']:
                 if p.grad is None:
                     continue
 
                 grad = p.grad
@@ -172,25 +173,25 @@
                         state['exp_avg_sq_row'] = torch.zeros(grad_shape[:-1], dtype=grad.dtype, device=grad.device)
                         state['exp_avg_sq_col'] = torch.zeros(
                             grad_shape[:-2] + grad_shape[-1:], dtype=grad.dtype, device=grad.device
                         )
                     else:
                         state['exp_avg_sq'] = torch.zeros_like(grad)
 
-                    if group['amsgrad']:
+                    if group['ams_bound']:
                         state['exp_avg_sq_hat'] = torch.zeros_like(grad)
 
                     state['RMS'] = 0.0
 
                 state['RMS'] = self.get_rms(p)
 
-                lr = self.get_lr(
-                    group['lr'],
-                    group['step'],
-                    state['RMS'],
+                lr: float = self.get_lr(
+                    lr=group['lr'],
+                    step=group['step'],
+                    rms=state['RMS'],
                     relative_step=group['relative_step'],
                     warmup_init=group['warmup_init'],
                     scale_parameter=group['scale_parameter'],
                 )
 
                 update = torch.mul(grad, grad).add_(self.eps1)
 
@@ -202,25 +203,31 @@
 
                     self.approximate_sq_grad(exp_avg_sq_row, exp_avg_sq_col, update)
                 else:
                     exp_avg_sq = state['exp_avg_sq']
                     exp_avg_sq.mul_(beta2_t).add_(update, alpha=1.0 - beta2_t)
                     torch.rsqrt(exp_avg_sq, out=update)
 
-                if group['amsgrad']:
+                if group['ams_bound']:
                     exp_avg_sq_hat = state['exp_avg_sq_hat']
                     torch.max(exp_avg_sq_hat, 1 / update, out=exp_avg_sq_hat)
                     torch.rsqrt(exp_avg_sq_hat / beta2_t, out=update)
 
                 update.mul_(grad)
 
                 update.div_((self.get_rms(update) / self.clip_threshold).clamp_(min=1.0)).mul_(lr)
 
                 exp_avg = state['exp_avg']
-                exp_avg.mul_(self.betas[0]).add_(update, alpha=1.0 - self.betas[0])
+                exp_avg.mul_(beta1).add_(update, alpha=1.0 - beta1)
 
-                if group['weight_decay'] > 0.0:
-                    p.add_(p, alpha=-lr * group['weight_decay'])
+                self.apply_weight_decay(
+                    p=p,
+                    grad=None,
+                    lr=lr,
+                    weight_decay=group['weight_decay'],
+                    weight_decouple=group['weight_decouple'],
+                    fixed_decay=group['fixed_decay'],
+                )
 
                 p.add_(-exp_avg)
 
         return loss
```

### Comparing `pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/adai.py` & `pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/adai.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,60 +13,53 @@
     r"""Disentangling the Effects of Adaptive Learning Rate and Momentum.
 
     :param params: PARAMETERS. iterable of parameters to optimize or dicts defining parameter groups.
     :param lr: float. learning rate.
     :param betas: BETAS. coefficients used for computing running averages of gradient and the squared hessian trace.
     :param weight_decay: float. weight decay (L2 penalty).
     :param weight_decouple: bool. the optimizer uses decoupled weight decay as in AdamW.
+    :param fixed_decay: bool. fix weight decay.
     :param stable_weight_decay: bool. perform stable weight decay.
     :param dampening: float. dampening for momentum. where dampening < 1, it will show some adaptive-moment behavior.
     :param use_gc: bool. use gradient centralization.
     :param eps: float. term added to the denominator to improve numerical stability.
     """
 
     def __init__(
         self,
         params: PARAMETERS,
         lr: float = 1e-3,
         betas: BETAS = (0.1, 0.99),
         weight_decay: float = 0.0,
         weight_decouple: bool = False,
+        fixed_decay: bool = False,
         stable_weight_decay: bool = False,
         dampening: float = 1.0,
         use_gc: bool = False,
         eps: float = 1e-3,
     ):
-        self.lr = lr
-        self.betas = betas
-        self.weight_decay = weight_decay
-        self.weight_decouple = weight_decouple
-        self.stable_weight_decay = stable_weight_decay
-        self.dampening = dampening
-        self.use_gc = use_gc
-        self.eps = eps
+        self.validate_learning_rate(lr)
+        self.validate_betas(betas)
+        self.validate_non_negative(weight_decay, 'weight_decay')
+        self.validate_non_negative(eps, 'eps')
 
-        self.validate_parameters()
+        self.use_gc = use_gc
 
         defaults: DEFAULTS = {
             'lr': lr,
             'betas': betas,
             'weight_decay': weight_decay,
             'weight_decouple': weight_decouple,
+            'fixed_decay': fixed_decay,
             'stable_weight_decay': stable_weight_decay,
             'dampening': dampening,
             'eps': eps,
         }
         super().__init__(params, defaults)
 
-    def validate_parameters(self):
-        self.validate_learning_rate(self.lr)
-        self.validate_betas(self.betas)
-        self.validate_weight_decay(self.weight_decay)
-        self.validate_epsilon(self.eps)
-
     def __str__(self) -> str:
         return 'Adai'
 
     @torch.no_grad()
     def reset(self):
         for group in self.param_groups:
             for p in group['params']:
@@ -108,62 +101,70 @@
                     state['beta1_prod'] = torch.ones_like(p)
 
                 state['step'] += 1
 
                 if self.use_gc:
                     grad = centralize_gradient(grad, gc_conv_only=False)
 
-                bias_correction2 = 1.0 - beta2 ** state['step']
+                bias_correction2: float = 1.0 - beta2 ** state['step']
 
                 if not group['stable_weight_decay'] and group['weight_decay'] > 0.0:
-                    if group['weight_decouple']:
-                        p.mul_(1.0 - group['lr'] * group['weight_decay'])
-                    else:
-                        grad.add_(p, alpha=group['weight_decay'])
+                    self.apply_weight_decay(
+                        p=p,
+                        grad=grad,
+                        lr=group['lr'],
+                        weight_decay=group['weight_decay'],
+                        weight_decouple=group['weight_decouple'],
+                        fixed_decay=group['fixed_decay'],
+                    )
 
                 exp_avg_sq = state['exp_avg_sq']
                 exp_avg_sq.mul_(beta2).addcmul_(grad, grad, value=1.0 - beta2)
 
                 exp_avg_sq_hat_sum += exp_avg_sq.sum() / bias_correction2
 
         if param_size == 0:
             raise ZeroParameterSizeError()
 
         exp_avg_sq_hat_mean = exp_avg_sq_hat_sum / param_size
 
         for group in self.param_groups:
             beta0, beta2 = group['betas']
-            beta0_dp = math.pow(beta0, 1.0 - group['dampening'])
+            beta0_dp: float = math.pow(beta0, 1.0 - group['dampening'])
             for p in group['params']:
                 if p.grad is None:
                     continue
 
                 grad = p.grad
+
                 state = self.state[p]
 
                 if group['stable_weight_decay'] and group['weight_decay'] > 0.0:
-                    if group['weight_decouple']:
-                        p.mul_(1.0 - group['lr'] * group['weight_decay'])
-                    else:
-                        grad.add_(p, alpha=group['weight_decay'])
+                    self.apply_weight_decay(
+                        p=p,
+                        grad=grad,
+                        lr=group['lr'],
+                        weight_decay=group['weight_decay'],
+                        weight_decouple=group['weight_decouple'],
+                        fixed_decay=group['fixed_decay'],
+                    )
 
-                bias_correction2 = 1.0 - beta2 ** state['step']
+                bias_correction2: float = 1.0 - beta2 ** state['step']
 
                 exp_avg, exp_avg_sq = state['exp_avg'], state['exp_avg_sq']
 
                 exp_avg_sq_hat = exp_avg_sq / bias_correction2
                 beta1 = (
-                    1.0 - (exp_avg_sq_hat / exp_avg_sq_hat_mean).pow(1.0 / (3.0 - 2.0 * group['dampening'])).mul(beta0)
-                ).clamp(0.0, 1.0 - group['eps'])
-                beta3 = (1.0 - beta1).pow(group['dampening'])
+                    1.0
+                    - (exp_avg_sq_hat / exp_avg_sq_hat_mean).pow_(1.0 / (3.0 - 2.0 * group['dampening'])).mul_(beta0)
+                ).clamp_(0.0, 1.0 - group['eps'])
+                beta3 = (1.0 - beta1).pow_(group['dampening'])
 
                 beta1_prod = state['beta1_prod']
                 beta1_prod.mul_(beta1)
 
-                bias_correction1 = 1.0 - beta1_prod
-
                 exp_avg.mul_(beta1).addcmul_(beta3, grad)
-                exp_avg_hat = exp_avg.div(bias_correction1).mul(beta0_dp)
+                exp_avg_hat = exp_avg.div(1.0 - beta1_prod).mul_(beta0_dp)
 
                 p.add_(exp_avg_hat, alpha=-group['lr'])
 
         return loss
```

### Comparing `pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/adamod.py` & `pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/adasmooth.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,131 +1,124 @@
-import math
-
 import torch
 from torch.optim.optimizer import Optimizer
 
 from pytorch_optimizer.base.exception import NoSparseGradientError
 from pytorch_optimizer.base.optimizer import BaseOptimizer
 from pytorch_optimizer.base.types import BETAS, CLOSURE, DEFAULTS, LOSS, PARAMETERS
 
 
-class AdaMod(Optimizer, BaseOptimizer):
-    r"""An Adaptive and Momental Bound Method for Stochastic Learning.
+class AdaSmooth(Optimizer, BaseOptimizer):
+    r"""An Adaptive Learning Rate Method based on Effective Ratio.
 
     :param params: PARAMETERS. iterable of parameters to optimize or dicts defining parameter groups.
     :param lr: float. learning rate.
     :param betas: BETAS. coefficients used for computing running averages of gradient and the squared hessian trace.
-        beta3 is for smoothing coefficient for adaptive learning rates.
     :param weight_decay: float. weight decay (L2 penalty).
     :param weight_decouple: bool. the optimizer uses decoupled weight decay as in AdamW.
-    :param adam_debias: bool. Only correct the denominator to avoid inflating step sizes early in training.
+    :param fixed_decay: bool. fix weight decay.
     :param eps: float. term added to the denominator to improve numerical stability.
     """
 
     def __init__(
         self,
         params: PARAMETERS,
         lr: float = 1e-3,
-        betas: BETAS = (0.9, 0.99, 0.9999),
+        betas: BETAS = (0.5, 0.99),
         weight_decay: float = 0.0,
-        weight_decouple: bool = True,
-        adam_debias: bool = False,
-        eps: float = 1e-8,
+        weight_decouple: bool = False,
+        fixed_decay: bool = False,
+        eps: float = 1e-6,
     ):
-        self.lr = lr
-        self.betas = betas
-        self.weight_decay = weight_decay
-        self.eps = eps
-
-        self.validate_parameters()
+        self.validate_learning_rate(lr)
+        self.validate_betas(betas)
+        self.validate_non_negative(weight_decay, 'weight_decay')
+        self.validate_non_negative(eps, 'eps')
 
         defaults: DEFAULTS = {
             'lr': lr,
             'betas': betas,
             'weight_decay': weight_decay,
             'weight_decouple': weight_decouple,
-            'adam_debias': adam_debias,
+            'fixed_decay': fixed_decay,
             'eps': eps,
         }
-        super().__init__(params, defaults)
 
-    def validate_parameters(self):
-        self.validate_learning_rate(self.lr)
-        self.validate_betas(self.betas)
-        self.validate_weight_decay(self.weight_decay)
-        self.validate_epsilon(self.eps)
+        super().__init__(params, defaults)
 
     def __str__(self) -> str:
-        return 'AdaMod'
+        return 'AdaSmooth'
 
     @torch.no_grad()
     def reset(self):
         for group in self.param_groups:
             group['step'] = 0
             for p in group['params']:
                 state = self.state[p]
 
-                state['exp_avg'] = torch.zeros_like(p)
+                state['prev_param'] = torch.zeros_like(p)
+                state['s'] = torch.zeros_like(p)
+                state['n'] = torch.zeros_like(p)
                 state['exp_avg_sq'] = torch.zeros_like(p)
-                state['exp_avg_lr'] = torch.zeros_like(p)
 
     @torch.no_grad()
     def step(self, closure: CLOSURE = None) -> LOSS:
         loss: LOSS = None
         if closure is not None:
             with torch.enable_grad():
                 loss = closure()
 
         for group in self.param_groups:
             if 'step' in group:
                 group['step'] += 1
             else:
                 group['step'] = 1
 
-            beta1, beta2, beta3 = group['betas']
-
-            bias_correction1 = 1.0 - beta1 ** group['step']
-            bias_correction2_sq = math.sqrt(1.0 - beta2 ** group['step'])
+            beta1, beta2 = group['betas']
 
             for p in group['params']:
                 if p.grad is None:
                     continue
 
                 grad = p.grad
                 if grad.is_sparse:
                     raise NoSparseGradientError(str(self))
 
                 state = self.state[p]
 
                 if len(state) == 0:
-                    state['exp_avg'] = torch.zeros_like(p)
+                    state['prev_param'] = torch.zeros_like(p)
+                    state['s'] = torch.zeros_like(p)
+                    state['n'] = torch.zeros_like(p)
                     state['exp_avg_sq'] = torch.zeros_like(p)
-                    state['exp_avg_lr'] = torch.zeros_like(p)
 
-                exp_avg, exp_avg_sq = state['exp_avg'], state['exp_avg_sq']
-                exp_avg.mul_(beta1).add_(grad, alpha=1.0 - beta1)
-                exp_avg_sq.mul_(beta2).addcmul_(grad, grad, value=1.0 - beta2)
-
-                de_nom = exp_avg_sq.sqrt().add_(group['eps'])
-
-                step_size = torch.full_like(
-                    de_nom,
-                    fill_value=group['lr']
-                    * bias_correction2_sq
-                    / (bias_correction1 if not group['adam_debias'] else 1.0),
+                self.apply_weight_decay(
+                    p=p,
+                    grad=p.grad,
+                    lr=group['lr'],
+                    weight_decay=group['weight_decay'],
+                    weight_decouple=group['weight_decouple'],
+                    fixed_decay=group['fixed_decay'],
                 )
-                step_size.div_(de_nom)
 
-                if group['weight_decouple']:
-                    p.mul_(1.0 - group['weight_decay'] * group['lr'])
-                elif group['weight_decay'] > 0.0:
-                    grad.add_(p, alpha=group['weight_decay'])
+                prev_param = state['prev_param']
+                p_diff = p - prev_param
 
-                exp_avg_lr = state['exp_avg_lr']
-                exp_avg_lr.mul_(beta3).add_(step_size, alpha=1.0 - beta3)
+                s, n = state['s'], state['n']
+                s.add_(p_diff)
+                n.add_(p_diff.abs())
 
-                torch.min(step_size, exp_avg_lr, out=step_size)
-                step_size.mul_(exp_avg)
+                c = s.sum().abs_().div_(n.sum())  # e_t
+                c.mul_(beta2 - beta1).add_(1.0 - beta2)
+
+                c_p2 = c.pow(2)
+
+                exp_avg_sq = state['exp_avg_sq']
+                exp_avg_sq.mul_(1.0 - c_p2).addcmul_(grad, grad, value=c_p2)
+
+                step_size = torch.full_like(exp_avg_sq, fill_value=group['lr'])
+                step_size.div_((exp_avg_sq + group['eps']).sqrt()).mul_(grad)
 
                 p.add_(-step_size)
 
+                state['prev_param'].copy_(p)
+
         return loss
```

### Comparing `pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/adamp.py` & `pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/adamp.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 class AdamP(Optimizer, BaseOptimizer):
     r"""Slowing Down the Slowdown for Momentum Optimizers on Scale-invariant Weights.
 
     :param params: PARAMETERS. iterable of parameters to optimize or dicts defining parameter groups.
     :param lr: float. learning rate.
     :param betas: BETAS. coefficients used for computing running averages of gradient and the squared hessian trace.
     :param weight_decay: float. weight decay (L2 penalty).
+    :param weight_decouple: bool. the optimizer uses decoupled weight decay as in AdamW.
+    :param fixed_decay: bool. fix weight decay.
     :param delta: float. threshold that determines whether a set of parameters is scale invariant or not.
     :param wd_ratio: float. relative weight decay applied on scale-invariant parameters compared to that applied
         on scale-variant parameters.
     :param use_gc: bool. use gradient centralization.
     :param nesterov: bool. enables Nesterov momentum.
     :param r: float. EMA factor. between 0.9 ~ 0.99 is preferred.
     :param adanorm: bool. whether to use the AdaNorm variant.
@@ -30,55 +32,51 @@
 
     def __init__(
         self,
         params: PARAMETERS,
         lr: float = 1e-3,
         betas: BETAS = (0.9, 0.999),
         weight_decay: float = 0.0,
+        weight_decouple: bool = True,
+        fixed_decay: bool = False,
         delta: float = 0.1,
         wd_ratio: float = 0.1,
         use_gc: bool = False,
         nesterov: bool = False,
         r: float = 0.95,
         adanorm: bool = False,
         adam_debias: bool = False,
         eps: float = 1e-8,
     ):
-        self.lr = lr
-        self.betas = betas
-        self.weight_decay = weight_decay
-        self.eps = eps
-        self.wd_ratio = wd_ratio
-        self.use_gc = use_gc
+        self.validate_learning_rate(lr)
+        self.validate_betas(betas)
+        self.validate_non_negative(weight_decay, 'weight_decay')
+        self.validate_range(wd_ratio, 'wd_ratio', 0.0, 1.0)
+        self.validate_non_negative(eps, 'eps')
 
-        self.validate_parameters()
+        self.use_gc = use_gc
 
         defaults: DEFAULTS = {
             'lr': lr,
             'betas': betas,
             'weight_decay': weight_decay,
+            'weight_decouple': weight_decouple,
+            'fixed_decay': fixed_decay,
             'delta': delta,
             'wd_ratio': wd_ratio,
             'nesterov': nesterov,
             'adanorm': adanorm,
             'adam_debias': adam_debias,
             'eps': eps,
         }
         if adanorm:
             defaults.update({'r': r})
 
         super().__init__(params, defaults)
 
-    def validate_parameters(self):
-        self.validate_learning_rate(self.lr)
-        self.validate_betas(self.betas)
-        self.validate_weight_decay(self.weight_decay)
-        self.validate_weight_decay_ratio(self.wd_ratio)
-        self.validate_epsilon(self.eps)
-
     def __str__(self) -> str:
         return 'AdamP'
 
     @torch.no_grad()
     def reset(self):
         for group in self.param_groups:
             group['step'] = 0
@@ -100,16 +98,17 @@
         for group in self.param_groups:
             if 'step' in group:
                 group['step'] += 1
             else:
                 group['step'] = 1
 
             beta1, beta2 = group['betas']
-            bias_correction1 = 1.0 - beta1 ** group['step']
-            bias_correction2_sq = math.sqrt(1.0 - beta2 ** group['step'])
+
+            bias_correction1: float = 1.0 - beta1 ** group['step']
+            bias_correction2_sq: float = math.sqrt(1.0 - beta2 ** group['step'])
 
             for p in group['params']:
                 if p.grad is None:
                     continue
 
                 grad = p.grad
                 if grad.is_sparse:
@@ -118,29 +117,25 @@
                 state = self.state[p]
                 if len(state) == 0:
                     state['exp_avg'] = torch.zeros_like(p)
                     state['exp_avg_sq'] = torch.zeros_like(p)
                     if group['adanorm']:
                         state['exp_grad_norm'] = torch.zeros((1,), dtype=grad.dtype, device=grad.device)
 
-                exp_avg, exp_avg_sq = state['exp_avg'], state['exp_avg_sq']
-
                 if self.use_gc:
                     grad = centralize_gradient(grad, gc_conv_only=False)
 
-                s_grad = grad
-                if group['adanorm']:
-                    grad_norm = torch.linalg.norm(grad)
-
-                    exp_grad_norm = state['exp_grad_norm']
-                    exp_grad_norm.mul_(group['r']).add_(grad_norm, alpha=1.0 - group['r'])
-
-                    if exp_grad_norm > grad_norm:
-                        s_grad *= exp_grad_norm / grad_norm
+                s_grad = self.get_adanorm_gradient(
+                    grad=grad,
+                    adanorm=group['adanorm'],
+                    exp_grad_norm=state.get('exp_grad_norm', None),
+                    r=group.get('r', None),
+                )
 
+                exp_avg, exp_avg_sq = state['exp_avg'], state['exp_avg_sq']
                 exp_avg.mul_(beta1).add_(s_grad, alpha=1.0 - beta1)
                 exp_avg_sq.mul_(beta2).addcmul_(grad, grad, value=1.0 - beta2)
 
                 inv_de_nom = exp_avg_sq.rsqrt().add_(group['eps']).mul_(bias_correction2_sq)
 
                 perturb = exp_avg.clone()
                 if group['nesterov']:
@@ -155,14 +150,26 @@
                         grad,
                         perturb,
                         group['delta'],
                         group['wd_ratio'],
                         group['eps'],
                     )
 
-                if group['weight_decay'] > 0.0:
-                    p.mul_(1.0 - group['lr'] * group['weight_decay'] * wd_ratio)
+                self.apply_weight_decay(
+                    p=p,
+                    grad=None,
+                    lr=group['lr'],
+                    weight_decay=group['weight_decay'],
+                    weight_decouple=group['weight_decouple'],
+                    fixed_decay=group['fixed_decay'],
+                    ratio=wd_ratio,
+                )
+
+                step_size: float = self.apply_adam_debias(
+                    adam_debias=group['adam_debias'],
+                    step_size=group['lr'],
+                    bias_correction1=bias_correction1,
+                )
 
-                step_size: float = group['lr'] if group['adam_debias'] else group['lr'] / bias_correction1
                 p.add_(perturb, alpha=-step_size)
 
         return loss
```

### Comparing `pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/adams.py` & `pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/adanorm.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,170 +1,144 @@
 import math
 
 import torch
 from torch.optim.optimizer import Optimizer
 
-from pytorch_optimizer.base.exception import NoSparseGradientError, ZeroParameterSizeError
+from pytorch_optimizer.base.exception import NoSparseGradientError
 from pytorch_optimizer.base.optimizer import BaseOptimizer
 from pytorch_optimizer.base.types import BETAS, CLOSURE, DEFAULTS, LOSS, PARAMETERS
 
 
-class AdamS(Optimizer, BaseOptimizer):
-    r"""Adam with stable weight decay.
+class AdaNorm(Optimizer, BaseOptimizer):
+    r"""Symbolic Discovery of Optimization Algorithms.
 
     :param params: PARAMETERS. iterable of parameters to optimize or dicts defining parameter groups.
     :param lr: float. learning rate.
     :param betas: BETAS. coefficients used for computing running averages of gradient and the squared hessian trace.
-    :param weight_decay: float. weight decay (L2 penalty).
-    :param amsgrad: bool. whether to use the AMSGrad variant of this algorithm from the paper.
     :param r: float. EMA factor. between 0.9 ~ 0.99 is preferred.
-    :param adanorm: bool. whether to use the AdaNorm variant.
+    :param weight_decay: float. weight decay (L2 penalty).
+    :param weight_decouple: bool. the optimizer uses decoupled weight decay as in AdamW.
+    :param fixed_decay: bool. fix weight decay.
+    :param ams_bound: bool. whether to use the AMSBound variant.
     :param adam_debias: bool. Only correct the denominator to avoid inflating step sizes early in training.
     :param eps: float. term added to the denominator to improve numerical stability.
     """
 
     def __init__(
         self,
         params: PARAMETERS,
         lr: float = 1e-3,
-        betas: BETAS = (0.9, 0.999),
-        weight_decay: float = 1e-4,
-        amsgrad: bool = False,
+        betas: BETAS = (0.9, 0.99),
         r: float = 0.95,
-        adanorm: bool = False,
+        weight_decay: float = 0.0,
+        weight_decouple: bool = True,
+        fixed_decay: bool = False,
+        ams_bound: bool = False,
         adam_debias: bool = False,
         eps: float = 1e-8,
     ):
-        self.lr = lr
-        self.betas = betas
-        self.weight_decay = weight_decay
-        self.eps = eps
-
-        self.validate_parameters()
+        self.validate_learning_rate(lr)
+        self.validate_betas(betas)
+        self.validate_non_negative(weight_decay, 'weight_decay')
+        self.validate_non_negative(eps, 'eps')
 
         defaults: DEFAULTS = {
             'lr': lr,
             'betas': betas,
+            'r': r,
             'weight_decay': weight_decay,
-            'amsgrad': amsgrad,
-            'adanorm': adanorm,
+            'weight_decouple': weight_decouple,
+            'fixed_decay': fixed_decay,
+            'ams_bound': ams_bound,
             'adam_debias': adam_debias,
             'eps': eps,
         }
-        if adanorm:
-            defaults.update({'r': r})
-
         super().__init__(params, defaults)
 
-    def validate_parameters(self):
-        self.validate_learning_rate(self.lr)
-        self.validate_betas(self.betas)
-        self.validate_weight_decay(self.weight_decay)
-        self.validate_epsilon(self.eps)
-
     def __str__(self) -> str:
-        return 'AdamS'
+        return 'AdaNorm'
 
     @torch.no_grad()
     def reset(self):
         for group in self.param_groups:
+            group['step'] = 0
             for p in group['params']:
                 state = self.state[p]
 
-                state['step'] = 0
                 state['exp_avg'] = torch.zeros_like(p)
-                state['exp_avg_sq'] = torch.zeros_like(p)
-                if group['amsgrad']:
-                    state['max_exp_avg_sq'] = torch.zeros_like(p)
-                if group['adanorm']:
-                    state['exp_grad_norm'] = torch.zeros((1,), dtype=p.dtype, device=p.device)
+                state['exp_avg_var'] = torch.zeros_like(p)
+                state['exp_grad_norm'] = torch.zeros((1,), dtype=p.dtype, device=p.device)
+                if group['ams_bound']:
+                    state['max_exp_avg_var'] = torch.zeros_like(p)
 
     @torch.no_grad()
     def step(self, closure: CLOSURE = None) -> LOSS:
         loss: LOSS = None
         if closure is not None:
             with torch.enable_grad():
                 loss = closure()
 
-        param_size: int = 0
-        exp_avg_sq_hat_sum: float = 0.0
-
         for group in self.param_groups:
+            if 'step' in group:
+                group['step'] += 1
+            else:
+                group['step'] = 1
+
             beta1, beta2 = group['betas']
+
+            bias_correction1: float = 1.0 - beta1 ** group['step']
+            bias_correction2_sq: float = math.sqrt(1.0 - beta2 ** group['step'])
+
             for p in group['params']:
                 if p.grad is None:
                     continue
 
                 grad = p.grad
                 if grad.is_sparse:
                     raise NoSparseGradientError(str(self))
 
-                param_size += p.numel()
-
                 state = self.state[p]
 
                 if len(state) == 0:
-                    state['step'] = 0
                     state['exp_avg'] = torch.zeros_like(p)
-                    state['exp_avg_sq'] = torch.zeros_like(p)
-                    if group['amsgrad']:
-                        state['max_exp_avg_sq'] = torch.zeros_like(p)
-                    if group['adanorm']:
-                        state['exp_grad_norm'] = torch.zeros((1,), dtype=p.dtype, device=p.device)
-
-                state['step'] += 1
-                exp_avg, exp_avg_sq = state['exp_avg'], state['exp_avg_sq']
-
-                bias_correction2 = 1.0 - beta2 ** state['step']
-
-                s_grad = grad
-                if group['adanorm']:
-                    grad_norm = torch.linalg.norm(grad)
-
-                    exp_grad_norm = state['exp_grad_norm']
-                    exp_grad_norm.mul_(group['r']).add_(grad_norm, alpha=1.0 - group['r'])
+                    state['exp_avg_var'] = torch.zeros_like(p)
+                    state['exp_grad_norm'] = torch.zeros((1,), dtype=p.dtype, device=p.device)
+                    if group['ams_bound']:
+                        state['max_exp_avg_var'] = torch.zeros_like(p)
 
-                    if exp_grad_norm > grad_norm:
-                        s_grad *= exp_grad_norm / grad_norm
+                self.apply_weight_decay(
+                    p=p,
+                    grad=grad,
+                    lr=group['lr'],
+                    weight_decay=group['weight_decay'],
+                    weight_decouple=group['weight_decouple'],
+                    fixed_decay=group['fixed_decay'],
+                )
+
+                s_grad = self.get_adanorm_gradient(
+                    grad=grad,
+                    adanorm=True,
+                    exp_grad_norm=state['exp_grad_norm'],
+                    r=group['r'],
+                )
 
+                exp_avg, exp_avg_var = state['exp_avg'], state['exp_avg_var']
                 exp_avg.mul_(beta1).add_(s_grad, alpha=1.0 - beta1)
-                exp_avg_sq.mul_(beta2).addcmul_(grad, grad, value=1.0 - beta2)
-
-                if group['amsgrad']:
-                    max_exp_avg_sq = state['max_exp_avg_sq']
-                    torch.max(max_exp_avg_sq, exp_avg_sq, out=max_exp_avg_sq)
-                    exp_avg_sq_hat = max_exp_avg_sq
-                else:
-                    exp_avg_sq_hat = exp_avg_sq
-
-                exp_avg_sq_hat_sum += exp_avg_sq_hat.sum() / bias_correction2
-
-        if param_size == 0:
-            raise ZeroParameterSizeError()
-
-        exp_avg_sq_hat_mean = math.sqrt(exp_avg_sq_hat_sum / param_size) + self.eps
-
-        for group in self.param_groups:
-            beta1, beta2 = group['betas']
-            for p in group['params']:
-                if p.grad is None:
-                    continue
-
-                state = self.state[p]
-
-                if group['weight_decay'] > 0.0:
-                    p.mul_(1.0 - group['lr'] * group['weight_decay'] / exp_avg_sq_hat_mean)
-
-                exp_avg, exp_avg_sq = state['exp_avg'], state['exp_avg_sq']
-
-                bias_correction1 = 1.0 - beta1 ** state['step']
-                bias_correction2 = 1.0 - beta2 ** state['step']
-
-                exp_avg_sq_hat = state['max_exp_avg_sq'] if group['amsgrad'] else exp_avg_sq
-                exp_avg_sq_hat.div_(bias_correction2)
+                exp_avg_var.mul_(beta2).addcmul_(grad, grad, value=1.0 - beta2)
 
-                de_nom = exp_avg_sq_hat.sqrt().add(group['eps'])
+                de_nom = self.apply_ams_bound(
+                    ams_bound=group['ams_bound'],
+                    exp_avg_sq=exp_avg_var,
+                    max_exp_avg_sq=state.get('max_exp_avg_var', None),
+                    eps=group['eps'],
+                )
+                de_nom.div_(bias_correction2_sq)
+
+                step_size: float = self.apply_adam_debias(
+                    adam_debias=group['adam_debias'],
+                    step_size=group['lr'],
+                    bias_correction1=bias_correction1,
+                )
 
-                step_size = group['lr'] if group['adam_debias'] else group['lr'] / bias_correction1
                 p.addcdiv_(exp_avg, de_nom, value=-step_size)
 
         return loss
```

### Comparing `pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/adan.py` & `pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/adan.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,22 +35,22 @@
         weight_decouple: bool = False,
         max_grad_norm: float = 0.0,
         use_gc: bool = False,
         r: float = 0.95,
         adanorm: bool = False,
         eps: float = 1e-8,
     ):
-        self.lr = lr
-        self.betas = betas
-        self.weight_decay = weight_decay
+        self.validate_learning_rate(lr)
+        self.validate_betas(betas)
+        self.validate_non_negative(weight_decay, 'weight_decay')
+        self.validate_non_negative(max_grad_norm, 'max_grad_norm')
+        self.validate_non_negative(eps, 'eps')
+
         self.max_grad_norm = max_grad_norm
         self.use_gc = use_gc
-        self.eps = eps
-
-        self.validate_parameters()
 
         defaults: DEFAULTS = {
             'lr': lr,
             'betas': betas,
             'weight_decay': weight_decay,
             'weight_decouple': weight_decouple,
             'max_grad_norm': max_grad_norm,
@@ -58,21 +58,14 @@
             'eps': eps,
         }
         if adanorm:
             defaults.update({'r': r})
 
         super().__init__(params, defaults)
 
-    def validate_parameters(self):
-        self.validate_learning_rate(self.lr)
-        self.validate_betas(self.betas)
-        self.validate_weight_decay(self.weight_decay)
-        self.validate_epsilon(self.eps)
-        self.validate_norm(self.max_grad_norm)
-
     def __str__(self) -> str:
         return 'Adan'
 
     @torch.no_grad()
     def reset(self):
         for group in self.param_groups:
             group['step'] = 0
@@ -88,15 +81,15 @@
 
     @torch.no_grad()
     def get_global_gradient_norm(self) -> Union[torch.Tensor, float]:
         if self.defaults['max_grad_norm'] == 0.0:
             return 1.0
 
         global_grad_norm = get_global_gradient_norm(self.param_groups, self.param_groups[0]['params'][0].device)
-        global_grad_norm.sqrt_().add_(self.eps)
+        global_grad_norm.sqrt_().add_(self.defaults['eps'])
 
         return torch.clamp(self.defaults['max_grad_norm'] / global_grad_norm, max=1.0)
 
     @torch.no_grad()
     def step(self, closure: CLOSURE = None) -> LOSS:
         loss: LOSS = None
         if closure is not None:
@@ -108,17 +101,18 @@
         for group in self.param_groups:
             if 'step' in group:
                 group['step'] += 1
             else:
                 group['step'] = 1
 
             beta1, beta2, beta3 = group['betas']
-            bias_correction1 = 1.0 - beta1 ** group['step']
-            bias_correction2 = 1.0 - beta2 ** group['step']
-            bias_correction3_sq = math.sqrt(1.0 - beta3 ** group['step'])
+
+            bias_correction1: float = 1.0 - beta1 ** group['step']
+            bias_correction2: float = 1.0 - beta2 ** group['step']
+            bias_correction3_sq: float = math.sqrt(1.0 - beta3 ** group['step'])
 
             for p in group['params']:
                 if p.grad is None:
                     continue
 
                 grad = p.grad
                 if grad.is_sparse:
@@ -137,34 +131,30 @@
 
                 if self.use_gc:
                     grad = centralize_gradient(grad, gc_conv_only=False)
 
                 grad_diff = state['previous_grad']
                 grad_diff.add_(grad)
 
-                s_grad = grad
-                if group['adanorm']:
-                    grad_norm = torch.linalg.norm(grad)
-
-                    exp_grad_norm = state['exp_grad_norm']
-                    exp_grad_norm.mul_(group['r']).add_(grad_norm, alpha=1.0 - group['r'])
-
-                    if exp_grad_norm > grad_norm:
-                        s_grad *= exp_grad_norm / grad_norm
+                s_grad = self.get_adanorm_gradient(
+                    grad=grad,
+                    adanorm=group['adanorm'],
+                    exp_grad_norm=state.get('exp_grad_norm', None),
+                    r=group.get('r', None),
+                )
 
                 exp_avg, exp_avg_sq, exp_avg_diff = state['exp_avg'], state['exp_avg_sq'], state['exp_avg_diff']
 
                 exp_avg.mul_(beta1).add_(s_grad, alpha=1.0 - beta1)
                 exp_avg_diff.mul_(beta2).add_(grad_diff, alpha=1.0 - beta2)
 
                 grad_diff.mul_(beta2).add_(grad)
                 exp_avg_sq.mul_(beta3).addcmul_(grad_diff, grad_diff, value=1.0 - beta3)
 
-                de_nom = exp_avg_sq.sqrt()
-                de_nom.div_(bias_correction3_sq).add_(group['eps'])
+                de_nom = exp_avg_sq.sqrt().div_(bias_correction3_sq).add_(group['eps'])
 
                 if group['weight_decouple']:
                     p.mul_(1.0 - group['lr'] * group['weight_decay'])
 
                 p.addcdiv_(exp_avg, de_nom, value=-group['lr'] / bias_correction1)
                 p.addcdiv_(exp_avg_diff, de_nom, value=-group['lr'] * beta2 / bias_correction2)
```

### Comparing `pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/adanorm.py` & `pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/yogi.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,83 +4,79 @@
 from torch.optim.optimizer import Optimizer
 
 from pytorch_optimizer.base.exception import NoSparseGradientError
 from pytorch_optimizer.base.optimizer import BaseOptimizer
 from pytorch_optimizer.base.types import BETAS, CLOSURE, DEFAULTS, LOSS, PARAMETERS
 
 
-class AdaNorm(Optimizer, BaseOptimizer):
-    r"""Symbolic Discovery of Optimization Algorithms.
+class Yogi(Optimizer, BaseOptimizer):
+    r"""Decoupled Weight Decay Regularization.
 
     :param params: PARAMETERS. iterable of parameters to optimize or dicts defining parameter groups.
     :param lr: float. learning rate.
     :param betas: BETAS. coefficients used for computing running averages of gradient and the squared hessian trace.
-    :param r: float. EMA factor. between 0.9 ~ 0.99 is preferred.
+    :param initial_accumulator: float. initial values for first and second moments.
     :param weight_decay: float. weight decay (L2 penalty).
     :param weight_decouple: bool. the optimizer uses decoupled weight decay as in AdamW.
     :param fixed_decay: bool. fix weight decay.
-    :param amsgrad: bool. whether to use the AMSGrad variant of this algorithm from the paper.
+    :param r: float. EMA factor. between 0.9 ~ 0.99 is preferred.
+    :param adanorm: bool. whether to use the AdaNorm variant.
     :param adam_debias: bool. Only correct the denominator to avoid inflating step sizes early in training.
     :param eps: float. term added to the denominator to improve numerical stability.
     """
 
     def __init__(
         self,
         params: PARAMETERS,
-        lr: float = 1e-3,
-        betas: BETAS = (0.9, 0.99),
-        r: float = 0.95,
+        lr: float = 1e-2,
+        betas: BETAS = (0.9, 0.999),
+        initial_accumulator: float = 1e-6,
         weight_decay: float = 0.0,
         weight_decouple: bool = True,
         fixed_decay: bool = False,
-        amsgrad: bool = False,
+        r: float = 0.95,
+        adanorm: bool = False,
         adam_debias: bool = False,
-        eps: float = 1e-8,
+        eps: float = 1e-3,
     ):
-        self.lr = lr
-        self.betas = betas
-        self.weight_decay = weight_decay
-        self.eps = eps
-
-        self.validate_parameters()
+        self.validate_learning_rate(lr)
+        self.validate_betas(betas)
+        self.validate_non_negative(weight_decay, 'weight_decay')
+        self.validate_non_negative(eps, 'eps')
 
         defaults: DEFAULTS = {
             'lr': lr,
             'betas': betas,
-            'r': r,
             'weight_decay': weight_decay,
             'weight_decouple': weight_decouple,
             'fixed_decay': fixed_decay,
-            'amsgrad': amsgrad,
+            'initial_accumulator': initial_accumulator,
+            'adanorm': adanorm,
             'adam_debias': adam_debias,
             'eps': eps,
         }
-        super().__init__(params, defaults)
+        if adanorm:
+            defaults.update({'r': r})
 
-    def validate_parameters(self):
-        self.validate_learning_rate(self.lr)
-        self.validate_betas(self.betas)
-        self.validate_weight_decay(self.weight_decay)
-        self.validate_epsilon(self.eps)
+        super().__init__(params, defaults)
 
     def __str__(self) -> str:
-        return 'AdaNorm'
+        return 'Yogi'
 
     @torch.no_grad()
     def reset(self):
         for group in self.param_groups:
+            group['step'] = 0
             for p in group['params']:
                 state = self.state[p]
 
-                state['step'] = 0
-                state['exp_avg'] = torch.zeros_like(p)
-                state['exp_avg_var'] = torch.zeros_like(p)
-                state['exp_grad_norm'] = torch.zeros((1,), dtype=p.dtype, device=p.device)
-                if group['amsgrad']:
-                    state['max_exp_avg_var'] = torch.zeros_like(p)
+                state['exp_avg'] = torch.full_like(p, fill_value=group['initial_accumulator'])
+                state['exp_avg_sq'] = torch.full_like(p, fill_value=group['initial_accumulator'])
+                if group['adanorm']:
+                    state['exp_grad_norm'] = torch.zeros((1,), dtype=p.dtype, device=p.device)
 
     @torch.no_grad()
     def step(self, closure: CLOSURE = None) -> LOSS:
         loss: LOSS = None
         if closure is not None:
             with torch.enable_grad():
                 loss = closure()
@@ -89,58 +85,57 @@
             if 'step' in group:
                 group['step'] += 1
             else:
                 group['step'] = 1
 
             beta1, beta2 = group['betas']
 
-            bias_correction1 = 1 - beta1 ** group['step']
-            bias_correction2_sq = math.sqrt(1 - beta2 ** group['step'])
+            bias_correction1: float = 1.0 - beta1 ** group['step']
+            bias_correction2_sq: float = math.sqrt(1.0 - beta2 ** group['step'])
 
             for p in group['params']:
                 if p.grad is None:
                     continue
 
                 grad = p.grad
                 if grad.is_sparse:
                     raise NoSparseGradientError(str(self))
 
                 state = self.state[p]
 
                 if len(state) == 0:
-                    state['exp_avg'] = torch.zeros_like(p)
-                    state['exp_avg_var'] = torch.zeros_like(p)
-                    state['exp_grad_norm'] = torch.zeros((1,), dtype=p.dtype, device=p.device)
-                    if group['amsgrad']:
-                        state['max_exp_avg_var'] = torch.zeros_like(p)
-
-                if group['weight_decouple']:
-                    p.mul_(1.0 - group['weight_decay'] * (1.0 if group['fixed_decay'] else group['lr']))
-                elif group['weight_decay'] > 0.0:
-                    grad.add_(p, alpha=group['weight_decay'])
-
-                grad_norm = torch.linalg.norm(grad)
-
-                exp_grad_norm = state['exp_grad_norm']
-                exp_grad_norm.mul_(group['r']).add_(grad_norm, alpha=1.0 - group['r'])
+                    state['exp_avg'] = torch.full_like(p, fill_value=group['initial_accumulator'])
+                    state['exp_avg_sq'] = torch.full_like(p, fill_value=group['initial_accumulator'])
+                    if group['adanorm']:
+                        state['exp_grad_norm'] = torch.zeros((1,), dtype=grad.dtype, device=grad.device)
+
+                self.apply_weight_decay(
+                    p=p,
+                    grad=p.grad,
+                    lr=group['lr'],
+                    weight_decay=group['weight_decay'],
+                    weight_decouple=group['weight_decouple'],
+                    fixed_decay=group['fixed_decay'],
+                )
+
+                s_grad = self.get_adanorm_gradient(
+                    grad=grad,
+                    adanorm=group['adanorm'],
+                    exp_grad_norm=state.get('exp_grad_norm', None),
+                    r=group.get('r', None),
+                )
 
-                s_grad = grad
-                if exp_grad_norm > grad_norm:
-                    s_grad *= exp_grad_norm / grad_norm
+                grad_p2 = grad.mul(grad)
 
-                exp_avg, exp_avg_var = state['exp_avg'], state['exp_avg_var']
+                exp_avg, exp_avg_sq = state['exp_avg'], state['exp_avg_sq']
                 exp_avg.mul_(beta1).add_(s_grad, alpha=1.0 - beta1)
-                exp_avg_var.mul_(beta2).addcmul_(grad, grad, value=1.0 - beta2)
+                exp_avg_sq.addcmul_((exp_avg_sq - grad_p2).sign_(), grad_p2, value=-(1.0 - beta2))
 
-                if group['amsgrad']:
-                    max_exp_avg_var = state['max_exp_avg_var']
-                    torch.max(max_exp_avg_var, exp_avg_var, out=max_exp_avg_var)
-                    de_nom = max_exp_avg_var.sqrt().add_(group['eps'])
-                else:
-                    de_nom = exp_avg_var.sqrt().add_(group['eps'])
+                de_nom = exp_avg_sq.sqrt().div_(bias_correction2_sq).add_(group['eps'])
 
-                de_nom.div_(bias_correction2_sq).add_(group['eps'])
+                step_size: float = self.apply_adam_debias(
+                    adam_debias=group['adam_debias'], step_size=group['lr'], bias_correction1=bias_correction1
+                )
 
-                step_size = group['lr'] if group['adam_debias'] else group['lr'] / bias_correction1
                 p.addcdiv_(exp_avg, de_nom, value=-step_size)
 
         return loss
```

### Comparing `pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/adapnm.py` & `pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/adapnm.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,77 +12,71 @@
     r"""Adam + Positive-Negative Momentum Optimizers.
 
     :param params: PARAMETERS. iterable of parameters to optimize or dicts defining parameter groups.
     :param lr: float. learning rate.
     :param betas: BETAS. coefficients used for computing running averages of gradient and the squared hessian trace.
     :param weight_decay: float. weight decay (L2 penalty).
     :param weight_decouple: bool. use weight_decouple.
-    :param amsgrad: bool. whether to use the AMSGrad variant of this algorithm from the paper.
+    :param fixed_decay: bool. fix weight decay.
+    :param ams_bound: bool. whether to use the ams_bound variant.
     :param r: float. EMA factor. between 0.9 ~ 0.99 is preferred.
     :param adanorm: bool. whether to use the AdaNorm variant.
     :param adam_debias: bool. Only correct the denominator to avoid inflating step sizes early in training.
     :param eps: float. term added to the denominator to improve numerical stability.
     """
 
     def __init__(
         self,
         params: PARAMETERS,
         lr: float = 1e-3,
         betas: BETAS = (0.9, 0.999, 1.0),
         weight_decay: float = 0.0,
         weight_decouple: bool = True,
-        amsgrad: bool = True,
+        fixed_decay: bool = False,
+        ams_bound: bool = True,
         r: float = 0.95,
         adanorm: bool = False,
         adam_debias: bool = False,
         eps: float = 1e-8,
     ):
-        self.lr = lr
-        self.betas = betas
-        self.weight_decay = weight_decay
-        self.weight_decouple = weight_decouple
-        self.eps = eps
-
-        self.validate_parameters()
+        self.validate_learning_rate(lr)
+        self.validate_betas(betas)
+        self.validate_non_negative(weight_decay, 'weight_decay')
+        self.validate_non_negative(eps, 'eps')
 
         defaults: DEFAULTS = {
             'lr': lr,
             'betas': betas,
             'weight_decay': weight_decay,
             'weight_decouple': weight_decouple,
-            'amsgrad': amsgrad,
+            'fixed_decay': fixed_decay,
+            'ams_bound': ams_bound,
             'adanorm': adanorm,
             'adam_debias': adam_debias,
             'eps': eps,
         }
         if adanorm:
             defaults.update({'r': r})
 
         super().__init__(params, defaults)
 
-    def validate_parameters(self):
-        self.validate_learning_rate(self.lr)
-        self.validate_betas(self.betas)
-        self.validate_weight_decay(self.weight_decay)
-        self.validate_epsilon(self.eps)
-
     def __str__(self) -> str:
         return 'AdaPNM'
 
     @torch.no_grad()
     def reset(self):
         for group in self.param_groups:
+            group['step'] = 0
             for p in group['params']:
                 state = self.state[p]
 
-                state['step'] = 0
                 state['exp_avg'] = torch.zeros_like(p)
                 state['exp_avg_sq'] = torch.zeros_like(p)
                 state['neg_exp_avg'] = torch.zeros_like(p)
-                if group['amsgrad']:
+                if group['ams_bound']:
                     state['max_exp_avg_sq'] = torch.zeros_like(p)
                 if group['adanorm']:
                     state['exp_grad_norm'] = torch.zeros((1,), dtype=p.dtype, device=p.device)
 
     @torch.no_grad()
     def step(self, closure: CLOSURE = None) -> LOSS:
         loss: LOSS = None
@@ -93,68 +87,71 @@
         for group in self.param_groups:
             if 'step' in group:
                 group['step'] += 1
             else:
                 group['step'] = 1
 
             beta1, beta2, beta3 = group['betas']
-            noise_norm = math.sqrt((1 + beta3) ** 2 + beta3 ** 2)  # fmt: skip
 
-            bias_correction1 = 1 - beta1 ** group['step']
-            bias_correction2_sq = math.sqrt(1 - beta2 ** group['step'])
+            noise_norm: float = math.sqrt((1 + beta3) ** 2 + beta3 ** 2)  # fmt: skip
+            bias_correction1: float = 1.0 - beta1 ** group['step']
+            bias_correction2_sq: float = math.sqrt(1.0 - beta2 ** group['step'])
 
             for p in group['params']:
                 if p.grad is None:
                     continue
 
                 grad = p.grad
                 if grad.is_sparse:
                     raise NoSparseGradientError(str(self))
 
-                if group['weight_decouple']:
-                    p.mul_(1.0 - group['lr'] * group['weight_decay'])
-                else:
-                    grad.add_(p, alpha=group['weight_decay'])
-
                 state = self.state[p]
                 if len(state) == 0:
                     state['exp_avg'] = torch.zeros_like(p)
                     state['exp_avg_sq'] = torch.zeros_like(p)
                     state['neg_exp_avg'] = torch.zeros_like(p)
-                    if group['amsgrad']:
+                    if group['ams_bound']:
                         state['max_exp_avg_sq'] = torch.zeros_like(p)
                     if group['adanorm']:
                         state['exp_grad_norm'] = torch.zeros((1,), dtype=grad.dtype, device=grad.device)
 
+                self.apply_weight_decay(
+                    p=p,
+                    grad=grad,
+                    lr=group['lr'],
+                    weight_decay=group['weight_decay'],
+                    weight_decouple=group['weight_decouple'],
+                    fixed_decay=group['fixed_decay'],
+                )
+
                 if group['step'] % 2 == 1:
                     exp_avg, neg_exp_avg = state['exp_avg'], state['neg_exp_avg']
                 else:
                     exp_avg, neg_exp_avg = state['neg_exp_avg'], state['exp_avg']
 
-                s_grad = grad
-                if group['adanorm']:
-                    grad_norm = torch.linalg.norm(grad)
-
-                    exp_grad_norm = state['exp_grad_norm']
-                    exp_grad_norm.mul_(group['r']).add_(grad_norm, alpha=1.0 - group['r'])
-
-                    if exp_grad_norm > grad_norm:
-                        s_grad *= exp_grad_norm / grad_norm
+                s_grad = self.get_adanorm_gradient(
+                    grad=grad,
+                    adanorm=group['adanorm'],
+                    exp_grad_norm=state.get('exp_grad_norm', None),
+                    r=group.get('r', None),
+                )
 
                 exp_avg_sq = state['exp_avg_sq']
                 exp_avg.mul_(beta1 ** 2).add_(s_grad, alpha=1.0 - beta1 ** 2)  # fmt: skip
                 exp_avg_sq.mul_(beta2).addcmul_(grad, grad, value=1.0 - beta2)
 
-                if group['amsgrad']:
-                    max_exp_avg_sq = state['max_exp_avg_sq']
-                    torch.max(max_exp_avg_sq, exp_avg_sq, out=max_exp_avg_sq)
-                    exp_avg_sq_hat = max_exp_avg_sq.add_(group['eps'])
-                else:
-                    exp_avg_sq_hat = exp_avg_sq.add_(group['eps'])
-
-                de_nom = (exp_avg_sq_hat.sqrt() / bias_correction2_sq).add_(group['eps'])
+                de_nom = self.apply_ams_bound(
+                    ams_bound=group['ams_bound'],
+                    exp_avg_sq=exp_avg_sq,
+                    max_exp_avg_sq=state.get('max_exp_avg_sq', None),
+                    eps=group['eps'],
+                )
+                de_nom.div_(bias_correction2_sq)
+
+                step_size: float = self.apply_adam_debias(
+                    adam_debias=group['adam_debias'], step_size=group['lr'], bias_correction1=bias_correction1
+                )
 
-                step_size: float = group['lr'] if group['adam_debias'] else group['lr'] / bias_correction1
-                pn_momentum = exp_avg.mul(1.0 + beta3).add(neg_exp_avg, alpha=-beta3).mul(1.0 / noise_norm)
+                pn_momentum = exp_avg.mul(1.0 + beta3).add_(neg_exp_avg, alpha=-beta3).mul_(1.0 / noise_norm)
                 p.addcdiv_(pn_momentum, de_nom, value=-step_size)
 
         return loss
```

### Comparing `pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/aggmo.py` & `pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/aggmo.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,43 +10,39 @@
     r"""Aggregated Momentum: Stability Through Passive Damping.
 
     :param params: PARAMETERS. iterable of parameters to optimize or dicts defining parameter groups.
     :param lr: float. learning rate.
     :param betas: BETAS. coefficients used for computing running averages of gradient and the squared hessian trace.
     :param weight_decay: float. weight decay (L2 penalty).
     :param weight_decouple: bool. the optimizer uses decoupled weight decay as in AdamW.
+    :param fixed_decay: bool. fix weight decay.
     """
 
     def __init__(
         self,
         params: PARAMETERS,
         lr: float = 1e-3,
         betas: BETAS = (0.0, 0.9, 0.99),
         weight_decay: float = 0.0,
         weight_decouple: bool = False,
+        fixed_decay: bool = False,
     ):
-        self.lr = lr
-        self.betas = betas
-        self.weight_decay = weight_decay
-
-        self.validate_parameters()
+        self.validate_learning_rate(lr)
+        self.validate_betas(betas)
+        self.validate_non_negative(weight_decay, 'weight_decay')
 
         defaults: DEFAULTS = {
             'lr': lr,
             'betas': betas,
             'weight_decay': weight_decay,
             'weight_decouple': weight_decouple,
+            'fixed_decay': fixed_decay,
         }
         super().__init__(params, defaults)
 
-    def validate_parameters(self):
-        self.validate_learning_rate(self.lr)
-        self.validate_betas(self.betas)
-        self.validate_weight_decay(self.weight_decay)
-
     def __str__(self) -> str:
         return 'AggMo'
 
     @torch.no_grad()
     def reset(self):
         for group in self.param_groups:
             group['step'] = 0
@@ -79,18 +75,22 @@
                     raise NoSparseGradientError(str(self))
 
                 state = self.state[p]
 
                 if len(state) == 0:
                     state['momentum_buffer'] = {beta: torch.zeros_like(p) for beta in betas}
 
-                if group['weight_decouple']:
-                    p.mul_(1.0 - group['weight_decay'] * group['lr'])
-                elif group['weight_decay'] > 0.0:
-                    grad.add_(p, alpha=group['weight_decay'])
+                self.apply_weight_decay(
+                    p=p,
+                    grad=grad,
+                    lr=group['lr'],
+                    weight_decay=group['weight_decay'],
+                    weight_decouple=group['weight_decouple'],
+                    fixed_decay=group['fixed_decay'],
+                )
 
                 for beta in betas:
                     buf = state['momentum_buffer'][beta]
                     buf.mul_(beta).add_(grad)
 
                     p.add_(buf, alpha=-group['lr'] / len(betas))
```

### Comparing `pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/alig.py` & `pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/alig.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,46 +10,38 @@
 
 
 class AliG(Optimizer, BaseOptimizer):
     r"""Adaptive Learning Rates for Interpolation with Gradients.
 
     :param params: PARAMETERS. iterable of parameters to optimize or dicts defining parameter groups.
     :param max_lr: Optional[float]. max learning rate.
-    :param projection_fn : Callable. projection function to enforce constraints.
+    :param projection_fn: Callable. projection function to enforce constraints.
     :param momentum: float. momentum.
     :param adjusted_momentum: bool. if True, use pytorch-like momentum, instead of standard Nesterov momentum.
-    :param eps: float. term added to the denominator to improve numerical stability.
     """
 
     def __init__(
         self,
         params: PARAMETERS,
         max_lr: Optional[float] = None,
         projection_fn: Optional[Callable] = None,
         momentum: float = 0.0,
         adjusted_momentum: bool = False,
-        eps: float = 1e-5,
     ):
-        self.max_lr = max_lr
-        self.projection_fn = projection_fn
-        self.momentum = momentum
-        self.eps = eps
+        self.validate_learning_rate(max_lr)
+        self.validate_range(momentum, 'momentum', 0.0, 1.0)
 
-        self.validate_parameters()
+        self.projection_fn = projection_fn
 
         defaults: DEFAULTS = {'max_lr': max_lr, 'adjusted_momentum': adjusted_momentum, 'momentum': momentum}
         super().__init__(params, defaults)
 
         if self.projection_fn is not None:
             self.projection_fn()
 
-    def validate_parameters(self):
-        self.validate_momentum(self.momentum)
-        self.validate_epsilon(self.eps)
-
     def __str__(self) -> str:
         return 'AliG'
 
     @torch.no_grad()
     def reset(self):
         for group in self.param_groups:
             for p in group['params']:
@@ -58,15 +50,15 @@
                 if group['momentum'] > 0.0:
                     state['momentum_buffer'] = torch.zeros_like(p)
 
     @torch.no_grad()
     def compute_step_size(self, loss: float) -> float:
         r"""Compute step_size."""
         global_grad_norm = get_global_gradient_norm(self.param_groups, torch.device('cpu'))
-        global_grad_norm.add_(self.eps)
+        global_grad_norm.add_(1e-6)
 
         return loss / global_grad_norm.item()
 
     @torch.no_grad()
     def step(self, closure: CLOSURE = None) -> LOSS:
         if closure is None:
             raise NoClosureError('AliG', '(e.g. `optimizer.step(lambda: float(loss))`).')
```

### Comparing `pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/apollo.py` & `pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/apollo.py`

 * *Files 10% similar despite different names*

```diff
@@ -31,45 +31,36 @@
         beta: float = 0.9,
         rebound: str = 'constant',
         weight_decay: float = 0.0,
         weight_decay_type: str = 'l2',
         warmup_steps: int = 500,
         eps: float = 1e-4,
     ):
+        self.validate_learning_rate(lr)
+        self.validate_range(beta, 'beta', 0.0, 1.0, range_type='[]')
+        self.validate_rebound(rebound)
+        self.validate_non_negative(weight_decay, 'weight_decay')
+        self.validate_weight_decay_type(weight_decay_type)
+        self.validate_non_negative(eps, 'eps')
+
         self.lr = lr
-        self.beta = beta
-        self.rebound = rebound
-        self.weight_decay = weight_decay
-        self.weight_decay_type = weight_decay_type
         self.warmup_steps = warmup_steps
-        self.eps = eps
-
-        self.validate_parameters()
-
         self.init_lr: float = init_lr if init_lr is not None else lr / 1000.0
 
         defaults: DEFAULTS = {
             'lr': lr,
             'init_lr': self.init_lr,
             'beta': beta,
             'rebound': rebound,
             'weight_decay': weight_decay,
             'weight_decay_type': weight_decay_type,
             'eps': eps,
         }
         super().__init__(params, defaults)
 
-    def validate_parameters(self):
-        self.validate_learning_rate(self.lr)
-        self.validate_beta(self.beta)
-        self.validate_rebound(self.rebound)
-        self.validate_weight_decay(self.weight_decay)
-        self.validate_weight_decay_type(self.weight_decay_type)
-        self.validate_epsilon(self.eps)
-
     def __str__(self) -> str:
         return 'Apollo'
 
     @torch.no_grad()
     def reset(self):
         for group in self.param_groups:
             group['step'] = 0
@@ -128,15 +119,15 @@
                     rebound = delta_grad.norm(p=np.inf)
                 else:
                     rebound = 1e-2
                     eps /= rebound
 
                 exp_avg_grad.add_(delta_grad, alpha=alpha)
 
-                de_nom = d_p.norm(p=4).add(eps)
+                de_nom = d_p.norm(p=4).add_(eps)
                 d_p.div_(de_nom)
 
                 v_sq = d_p.mul(d_p)
                 delta = delta_grad.div_(de_nom).mul_(d_p).sum().mul(-alpha) - b.mul(v_sq).sum()
 
                 b.addcmul_(v_sq, delta)
```

### Comparing `pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/dadapt.py` & `pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/dadapt.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,71 +1,68 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the license found in the
 # LICENSE file in the root directory of this source tree.
 
+import math
+
 import torch
 from torch.optim.optimizer import Optimizer
 
 from pytorch_optimizer.base.exception import NoSparseGradientError
 from pytorch_optimizer.base.optimizer import BaseOptimizer
 from pytorch_optimizer.base.types import BETAS, CLOSURE, DEFAULTS, LOSS, PARAMETERS
-from pytorch_optimizer.optimizer.utils import to_real
+from pytorch_optimizer.optimizer.utils import get_global_gradient_norm, to_real
 
 
 class DAdaptAdaGrad(Optimizer, BaseOptimizer):
     r"""AdaGrad with D-Adaptation. Leave LR set to 1 unless you encounter instability.
 
     :param params: PARAMETERS. iterable of parameters to optimize or dicts defining parameter groups.
     :param lr: float. learning rate.
     :param momentum: float. momentum.
     :param d0: float. initial D estimate for D-adaptation (default 1e-6). Rarely needs changing.
     :param growth_rate: float. prevent the D estimate from growing faster than this multiplicative rate.
-        Default is inf, for unrestricted.
     :param weight_decay: float. weight decay (L2 penalty).
+    :param weight_decouple: bool. the optimizer uses decoupled weight decay as in AdamW.
+    :param fixed_decay: bool. fix weight decay.
     :param eps: float. term added to the denominator to improve numerical stability.
     """
 
     def __init__(
         self,
         params: PARAMETERS,
         lr: float = 1.0,
         momentum: float = 0.0,
         d0: float = 1e-6,
         growth_rate: float = float('inf'),
         weight_decay: float = 0.0,
+        weight_decouple: bool = False,
+        fixed_decay: bool = False,
         eps: float = 0.0,
     ):
-        self.lr = lr
-        self.momentum = momentum
-        self.d0 = d0
-        self.growth_rate = growth_rate
-        self.weight_decay = weight_decay
-        self.eps = eps
-
-        self.validate_parameters()
+        self.validate_learning_rate(lr)
+        self.validate_range(momentum, 'momentum', 0.0, 1.0, range_type='[)')
+        self.validate_non_negative(weight_decay, 'weight_decay')
+        self.validate_non_negative(eps, 'eps')
 
         defaults: DEFAULTS = {
             'lr': lr,
             'momentum': momentum,
             'd': d0,
             'growth_rate': growth_rate,
             'weight_decay': weight_decay,
+            'weight_decouple': weight_decouple,
+            'fixed_decay': fixed_decay,
             'k': 0,
             'eps': eps,
         }
         super().__init__(params, defaults)
 
-    def validate_parameters(self):
-        self.validate_learning_rate(self.lr)
-        self.validate_momentum(self.momentum)
-        self.validate_weight_decay(self.weight_decay)
-        self.validate_epsilon(self.eps)
-
     def __str__(self) -> str:
         return 'DAdaptAdaGrad'
 
     @torch.no_grad()
     def reset(self):
         for group in self.param_groups:
             for p in group['params']:
@@ -84,36 +81,35 @@
     def step(self, closure: CLOSURE = None) -> LOSS:
         loss: LOSS = None
         if closure is not None:
             with torch.enable_grad():
                 loss = closure()
 
         group = self.param_groups[0]
+        device = group['params'][0].device
 
-        lr, momentum, growth_rate = group['lr'], group['momentum'], group['growth_rate']
-
-        d = group['d']
-        d_lr = float(d * lr)
+        d, lr = group['d'], group['lr']
+        d_lr: float = d * lr
 
-        g_sq = torch.tensor([0.0], device=group['params'][0].device)
-        sk_sq_weighted_change = torch.tensor([0.0], device=group['params'][0].device)
-        sk_l1_change = torch.tensor([0.0], device=group['params'][0].device)
+        g_sq = torch.tensor([0.0], device=device)
+        sk_sq_weighted_change = torch.tensor([0.0], device=device)
+        sk_l1_change = torch.tensor([0.0], device=device)
         if 'gsq_weighted' not in group:
-            group['gsq_weighted'] = torch.tensor([0.0], device=group['params'][0].device)
+            group['gsq_weighted'] = torch.tensor([0.0], device=device)
         if 'sk_sq_weighted' not in group:
-            group['sk_sq_weighted'] = torch.tensor([0.0], device=group['params'][0].device)
+            group['sk_sq_weighted'] = torch.tensor([0.0], device=device)
         if 'sk_l1' not in group:
-            group['sk_l1'] = torch.tensor([0.0], device=group['params'][0].device)
+            group['sk_l1'] = torch.tensor([0.0], device=device)
 
         gsq_weighted = group['gsq_weighted']
         sk_sq_weighted = group['sk_sq_weighted']
         sk_l1 = group['sk_l1']
 
         for group in self.param_groups:
-            weight_decay, eps = group['weight_decay'], group['eps']
+            eps = group['eps']
             for p in group['params']:
                 if p.grad is None:
                     continue
 
                 grad = p.grad
 
                 state = self.state[p]
@@ -163,16 +159,22 @@
                         grad.indices(), weighted_sk_p1_delta_masked, grad.shape
                     )
                     weighted_sk.add_(weighted_sk_p1_delta)
 
                     sk_l1_masked = sk_masked._values().abs().sum()
                     sk_l1_change.add_(sk_l1_masked - old_sk_l1_masked)
                 else:
-                    if weight_decay > 0.0:
-                        grad.add_(p, alpha=weight_decay)
+                    self.apply_weight_decay(
+                        p=p,
+                        grad=grad,
+                        lr=group['lr'],
+                        weight_decay=group['weight_decay'],
+                        weight_decouple=group['weight_decouple'],
+                        fixed_decay=group['fixed_decay'],
+                    )
 
                     old_sk_sq_weighted_param = sk.pow(2).div(torch.sqrt(alpha_k) + eps).sum()
                     old_sk_l1_param = sk.abs().sum()
 
                     alpha_k.add_(grad.pow(2))
                     grad_sq = grad.pow(2).div(torch.sqrt(alpha_k) + eps).sum()
                     g_sq.add_(grad_sq)
@@ -190,32 +192,31 @@
         sk_l1.add_(sk_l1_change)
 
         if sk_l1 == 0:
             return loss
 
         if lr > 0.0:
             d_hat = (sk_sq_weighted - gsq_weighted) / sk_l1
-            d = self.d0 = max(d, min(d_hat, d * growth_rate))
+            d = group['d'] = max(d, min(d_hat.item(), d * group['growth_rate']))
 
         for group in self.param_groups:
             group['gsq_weighted'] = gsq_weighted
             group['sk_sq_weighted'] = sk_sq_weighted
             group['sk_l1'] = sk_l1
             group['d'] = d
 
             for p in group['params']:
                 if p.grad is None:
                     continue
 
                 grad = p.grad
+
                 state = self.state[p]
 
-                alpha_k = state['alpha_k']
-                sk = state['sk']
-                x0 = state['x0']
+                alpha_k, sk, x0 = state['alpha_k'], state['sk'], state['x0']
 
                 if grad.is_sparse:
                     grad = grad.coalesce()
 
                     sk_masked = sk.sparse_mask(grad).coalesce()._values()
                     alpha_k_masked = alpha_k.sparse_mask(grad).coalesce()._values()
                     x0_masked = x0.sparse_mask(grad).coalesce()._values()
@@ -223,331 +224,320 @@
 
                     loc_masked = x0_masked - sk_masked.div(torch.sqrt(alpha_k_masked + group['eps']))
 
                     loc_delta_masked = loc_masked - p_masked
                     loc_delta = torch.sparse_coo_tensor(grad.indices(), loc_delta_masked, grad.shape)
                     p.add_(loc_delta)
                 else:
-                    z = x0 - sk.div(torch.sqrt(alpha_k) + group['eps'])
+                    z = x0 - sk.div(alpha_k.sqrt().add_(group['eps']))
 
-                    if momentum > 0.0:
-                        p.mul_(momentum).add_(z, alpha=1.0 - momentum)
+                    if group['momentum'] > 0.0:
+                        p.mul_(group['momentum']).add_(z, alpha=1.0 - group['momentum'])
                     else:
                         p.copy_(z)
 
             group['k'] += 1
 
         return loss
 
 
 class DAdaptAdam(Optimizer, BaseOptimizer):
-    r"""Adam with D-Adaptation. Leave LR set to 1 unless you encounter instability.
+    r"""Adam with D-Adaptation. Leave LR set to 1 unless you encounter instability. This implementation is based on V3.
 
     :param params: PARAMETERS. iterable of parameters to optimize or dicts defining parameter groups.
     :param lr: float. learning rate.
     :param betas: BETAS. betas.
     :param d0: float. initial D estimate for D-adaptation (default 1e-6). Rarely needs changing.
     :param growth_rate: float. prevent the D estimate from growing faster than this multiplicative rate.
-        Default is inf, for unrestricted.
     :param weight_decay: float. weight decay (L2 penalty).
     :param weight_decouple: bool. use AdamW style weight decay.
+    :param fixed_decay: bool. fix weight decay.
+    :param bias_correction: bool. Turn on Adam's bias correction.
     :param eps: float. term added to the denominator to improve numerical stability.
     """
 
     def __init__(
         self,
         params: PARAMETERS,
         lr: float = 1.0,
         betas: BETAS = (0.9, 0.999),
         d0: float = 1e-6,
         growth_rate: float = float('inf'),
         weight_decay: float = 0.0,
         weight_decouple: bool = False,
-        eps: float = 1e-8,
+        fixed_decay: bool = False,
+        bias_correction: bool = False,
+        eps: float = 0.0,
     ):
-        self.lr = lr
-        self.betas = betas
-        self.d0 = d0
-        self.growth_rate = growth_rate
-        self.weight_decay = weight_decay
-        self.weight_decouple = weight_decouple
-        self.eps = eps
-
-        self.validate_parameters()
+        self.validate_learning_rate(lr)
+        self.validate_betas(betas)
+        self.validate_non_negative(weight_decay, 'weight_decay')
+        self.validate_non_negative(eps, 'eps')
 
         defaults: DEFAULTS = {
             'lr': lr,
             'betas': betas,
             'd': d0,
             'growth_rate': growth_rate,
             'weight_decay': weight_decay,
             'weight_decouple': weight_decouple,
-            'k': 0,
+            'fixed_decay': fixed_decay,
+            'bias_correction': bias_correction,
+            'step': 0,
             'eps': eps,
         }
         super().__init__(params, defaults)
 
-    def validate_parameters(self):
-        self.validate_learning_rate(self.lr)
-        self.validate_betas(self.betas)
-        self.validate_weight_decay(self.weight_decay)
-        self.validate_epsilon(self.eps)
-
     def __str__(self) -> str:
         return 'DAdaptAdam'
 
     @torch.no_grad()
     def reset(self):
         for group in self.param_groups:
+            group['step'] = 0
             for p in group['params']:
                 if p.grad is None:
                     continue
 
                 state = self.state[p]
 
-                state['step'] = 0
                 state['s'] = torch.zeros_like(p)
                 state['exp_avg'] = torch.zeros_like(p)
                 state['exp_avg_sq'] = torch.zeros_like(p)
 
     @torch.no_grad()
     def step(self, closure: CLOSURE = None) -> LOSS:
         loss: LOSS = None
         if closure is not None:
             with torch.enable_grad():
                 loss = closure()
 
         group = self.param_groups[0]
+        device = group['params'][0].device
 
         beta1, beta2 = group['betas']
-        growth_rate = group['growth_rate']
 
-        d, lr = group['d'], group['lr']
-        d_lr = float(d * lr)
+        beta2_sq: float = math.sqrt(beta2)
 
-        g_sq = torch.tensor([0.0], device=group['params'][0].device)
-        sk_sq_weighted = torch.tensor([0.0], device=group['params'][0].device)
-        sk_l1 = torch.tensor([0.0], device=group['params'][0].device)
-        if 'gsq_weighted' not in group:
-            group['gsq_weighted'] = torch.tensor([0.0], device=group['params'][0].device)
-        gsq_weighted = group['gsq_weighted']
+        d: float = group['d']
+        lr: float = group['lr']
+
+        bias_correction1: float = 1.0 - beta1 ** (group['step'] + 1)
+        bias_correction2_sq: float = math.sqrt(1.0 - beta2 ** (group['step'] + 1))
+        bias_correction: float = bias_correction1 / bias_correction2_sq
+
+        # it's not Adam Debias
+        d_lr: float = self.apply_adam_debias(
+            not group['bias_correction'], step_size=d * lr, bias_correction1=bias_correction
+        )
+
+        sk_l1 = torch.tensor([0.0], device=device)
+        numerator_acc = torch.tensor([0.0], device=device)
+
+        if 'numerator_weighted' not in group:
+            group['numerator_weighted'] = torch.tensor([0.0], device=device)
+        numerator_weighted = group['numerator_weighted']
 
         for group in self.param_groups:
             for p in group['params']:
                 if p.grad is None:
                     continue
 
                 grad = p.grad
                 if grad.is_sparse:
                     raise NoSparseGradientError(str(self))
 
                 state = self.state[p]
                 if 'step' not in state:
-                    state['step'] = 0
                     state['s'] = torch.zeros_like(p)
                     state['exp_avg'] = torch.zeros_like(p)
                     state['exp_avg_sq'] = torch.zeros_like(p)
 
-                exp_avg, exp_avg_sq = state['exp_avg'], state['exp_avg_sq']
-
-                grad_power = to_real(grad * grad.conj())
-
-                exp_avg.mul_(beta1).add_(grad, alpha=d_lr * (1.0 - beta1))
-                exp_avg_sq.mul_(beta2).add_(grad_power, alpha=1.0 - beta2)
+                exp_avg, exp_avg_sq, s = state['exp_avg'], state['exp_avg_sq'], state['s']
 
                 de_nom = exp_avg_sq.sqrt().add_(group['eps'])
+                numerator_acc.add_(torch.dot(grad.flatten(), s.div(de_nom).flatten()), alpha=d_lr)
 
-                g_sq.add_(grad_power.div_(de_nom).sum())
+                exp_avg.mul_(beta1).add_(grad, alpha=d_lr * (1.0 - beta1))
+                exp_avg_sq.mul_(beta2).addcmul_(grad, grad, value=1.0 - beta2)
 
-                s = state['s']
-                s.mul_(beta2).add_(grad, alpha=d_lr * (1.0 - beta2))
+                s.mul_(beta2_sq).add_(grad, alpha=d_lr * (1.0 - beta2_sq))
 
-                sk_sq_weighted.add_(to_real(s * s.conj()).div_(de_nom).sum())
                 sk_l1.add_(s.abs().sum())
 
         if sk_l1 == 0:
             return loss
 
-        gsq_weighted.mul_(beta2).add_(g_sq, alpha=(d_lr ** 2) * (1.0 - beta2))  # fmt: skip
+        numerator_weighted.mul_(beta2_sq).add_(numerator_acc, alpha=1.0 - beta2_sq)  # fmt: skip
 
         if lr > 0.0:
-            d_hat = (sk_sq_weighted / (1.0 - beta2) - gsq_weighted) / sk_l1
-            d = max(d, min(d_hat, d * growth_rate))
+            d_hat = numerator_weighted / (1.0 - beta2_sq) * sk_l1
+            d = max(d, min(d_hat.item(), d * group['growth_rate']))
 
         for group in self.param_groups:
-            group['gsq_weighted'] = gsq_weighted
+            group['numerator_weighted'] = numerator_weighted
             group['d'] = d
+
             for p in group['params']:
                 if p.grad is None:
                     continue
 
                 state = self.state[p]
 
-                state['step'] += 1
                 exp_avg, exp_avg_sq = state['exp_avg'], state['exp_avg_sq']
 
                 de_nom = exp_avg_sq.sqrt().add_(group['eps'])
-                de_nom = de_nom.type(p.type())
-
-                if group['weight_decay'] > 0.0 and group['weight_decouple']:
-                    p.add_(p, alpha=-group['weight_decay'] * d_lr)
 
-                p.addcdiv_(exp_avg, de_nom, value=-1)
+                self.apply_weight_decay(
+                    p=p,
+                    grad=None,
+                    lr=d_lr,
+                    weight_decay=group['weight_decay'],
+                    weight_decouple=group['weight_decouple'],
+                    fixed_decay=group['fixed_decay'],
+                )
 
-            group['k'] += 1
+                p.addcdiv_(exp_avg, de_nom, value=-1.0)
 
         return loss
 
 
 class DAdaptSGD(Optimizer, BaseOptimizer):
-    r"""SGD with D-Adaptation. Leave LR set to 1 unless you encounter instability.
+    r"""SGD with D-Adaptation. Leave LR set to 1 unless you encounter instability. This implementation is based on V3.
 
     :param params: PARAMETERS. iterable of parameters to optimize or dicts defining parameter groups.
     :param lr: float. learning rate.
     :param momentum: float. momentum.
     :param d0: float. initial D estimate for D-adaptation (default 1e-6). Rarely needs changing.
     :param growth_rate: float. prevent the D estimate from growing faster than this multiplicative rate.
-        Default is inf, for unrestricted.
     :param weight_decay: float. weight decay (L2 penalty).
+    :param weight_decouple: bool. the optimizer uses decoupled weight decay as in AdamW.
+    :param fixed_decay: bool. fix weight decay.
     """
 
     def __init__(
         self,
         params: PARAMETERS,
         lr: float = 1.0,
-        momentum: float = 0.0,
+        momentum: float = 0.9,
         d0: float = 1e-6,
         growth_rate: float = float('inf'),
         weight_decay: float = 0.0,
+        weight_decouple: bool = False,
+        fixed_decay: bool = False,
     ):
-        self.lr = lr
-        self.momentum = momentum
-        self.d0 = d0
-        self.growth_rate = growth_rate
-        self.weight_decay = weight_decay
-        self.validate_parameters()
+        self.validate_learning_rate(lr)
+        self.validate_range(momentum, 'momentum', 0.0, 1.0, range_type='[)')
+        self.validate_non_negative(weight_decay, 'weight_decay')
 
         defaults: DEFAULTS = {
             'lr': lr,
             'momentum': momentum,
             'd': d0,
             'growth_rate': growth_rate,
             'weight_decay': weight_decay,
-            'k': 0,
+            'weight_decouple': weight_decouple,
+            'fixed_decay': fixed_decay,
+            'step': 0,
         }
         super().__init__(params, defaults)
 
-    def validate_parameters(self):
-        self.validate_learning_rate(self.lr)
-        self.validate_momentum(self.momentum)
-        self.validate_weight_decay(self.weight_decay)
-
     def __str__(self) -> str:
         return 'DAdaptSGD'
 
     @torch.no_grad()
     def reset(self):
         for group in self.param_groups:
+            group['step'] = 0
             for p in group['params']:
                 if p.grad is None:
                     continue
 
                 state = self.state[p]
 
-                state['step'] = 0
+                state['z'] = p.clone()
                 state['s'] = torch.zeros_like(p)
-                state['exp_avg'] = torch.zeros_like(p)
-                state['exp_avg_sq'] = torch.zeros_like(p)
+                state['x0'] = p.clone()
 
     @torch.no_grad()
     def step(self, closure: CLOSURE = None) -> LOSS:
         loss: LOSS = None
         if closure is not None:
             with torch.enable_grad():
                 loss = closure()
 
         group = self.param_groups[0]
+        device = group['params'][0].device
 
-        growth_rate = group['growth_rate']
+        sk_sq = torch.tensor([0.0], device=device)
+        if 'numerator_weighted' not in group:
+            group['numerator_weighted'] = torch.tensor([0.0], device=device)
+        numerator_weighted = group['numerator_weighted']
 
-        g_sq = torch.tensor([0.0], device=group['params'][0].device)
-        sk_sq = torch.tensor([0.0], device=group['params'][0].device)
-        if 'gsq_weighted' not in group:
-            group['gsq_weighted'] = torch.tensor([0.0], device=group['params'][0].device)
-        gsq_weighted = group['gsq_weighted']
+        if group['step'] == 0:
+            group['g0_norm'] = get_global_gradient_norm(self.param_groups, device).sqrt_().item()
+        g0_norm = group['g0_norm']
+
+        if g0_norm == 0:
+            return loss
+
+        d, lr = group['d'], group['lr']
+        d_lr: float = d * lr / g0_norm
 
         for group in self.param_groups:
-            weight_decay = group['weight_decay']
             for p in group['params']:
                 if p.grad is None:
                     continue
 
                 grad = p.grad
                 if grad.is_sparse:
                     raise NoSparseGradientError(str(self))
 
-                if weight_decay > 0.0:
-                    grad.add_(p, alpha=weight_decay)
-
                 state = self.state[p]
-                if 'z' not in state:
-                    state['z'] = torch.clone(p)
+                if len(state) == 0:
+                    state['z'] = p.clone()
                     state['s'] = torch.zeros_like(p)
-                    state['x0'] = torch.clone(p)
+                    state['x0'] = p.clone()
 
-                g_sq.add_(grad.pow(2).sum())
-
-        if g_sq == 0:
-            return loss
-
-        group = self.param_groups[0]
-
-        if group['k'] == 0:
-            group['g0_norm'] = g_sq.sqrt().item()
-        g0_norm = group['g0_norm']
-
-        d, lr = group['d'], group['lr']
-        d_lr = float(d * lr) / g0_norm
-
-        for group in self.param_groups:
-            for p in group['params']:
-                if p.grad is None:
-                    continue
-
-                state = self.state[p]
+                self.apply_weight_decay(
+                    p=p,
+                    grad=None,
+                    lr=d_lr,
+                    weight_decay=group['weight_decay'],
+                    weight_decouple=group['weight_decouple'],
+                    fixed_decay=group['fixed_decay'],
+                )
 
                 s = state['s']
-                s.add_(p.grad, alpha=d_lr)
+                numerator_weighted.add_(torch.dot(grad.flatten(), s.flatten()), alpha=d_lr)
 
+                s.add_(grad, alpha=d_lr)
                 sk_sq.add_(s.pow(2).sum())
 
-        gsq_weighted.add_(g_sq, alpha=d_lr ** 2)  # fmt: skip
-
         if lr > 0.0:
-            d_hat = (sk_sq - gsq_weighted) / sk_sq.sqrt()
-            d = max(d, min(d_hat, d * growth_rate))
+            d_hat = 2.0 * numerator_weighted / sk_sq.sqrt()
+            d = max(d, min(d_hat.item(), d * group['growth_rate']))
 
         for group in self.param_groups:
-            group['gsq_weighted'] = gsq_weighted
+            group['step'] += 1
+
+            group['numerator_weighted'] = numerator_weighted
             group['d'] = d
-            group['g0_norm'] = g0_norm
 
             for p in group['params']:
                 if p.grad is None:
                     continue
 
                 state = self.state[p]
 
                 z = state['z']
                 z.copy_(state['x0'] - state['s'])
 
                 p.mul_(group['momentum']).add_(z, alpha=1.0 - group['momentum'])
 
-            group['k'] += 1
-
         return loss
 
 
 class DAdaptAdan(Optimizer, BaseOptimizer):
     r"""Adan with D-Adaptation. Leave LR set to 1 unless you encounter instability.
 
     :param params: PARAMETERS. iterable of parameters to optimize or dicts defining parameter groups.
@@ -568,41 +558,31 @@
         betas: BETAS = (0.98, 0.92, 0.99),
         weight_decay: float = 0.0,
         weight_decouple: bool = False,
         d0: float = 1e-6,
         growth_rate: float = float('inf'),
         eps: float = 1e-8,
     ):
-        self.lr = lr
-        self.betas = betas
-        self.weight_decay = weight_decay
-        self.d0 = d0
-        self.growth_rate = growth_rate
-        self.eps = eps
-
-        self.validate_parameters()
+        self.validate_learning_rate(lr)
+        self.validate_betas(betas)
+        self.validate_non_negative(weight_decay, 'weight_decay')
+        self.validate_non_negative(eps, 'eps')
 
         defaults: DEFAULTS = {
             'lr': lr,
             'betas': betas,
             'weight_decay': weight_decay,
             'weight_decouple': weight_decouple,
             'd': d0,
             'growth_rate': growth_rate,
             'k': 0,
             'eps': eps,
         }
         super().__init__(params, defaults)
 
-    def validate_parameters(self):
-        self.validate_learning_rate(self.lr)
-        self.validate_betas(self.betas)
-        self.validate_weight_decay(self.weight_decay)
-        self.validate_epsilon(self.eps)
-
     def __str__(self) -> str:
         return 'DAdaptAdan'
 
     @torch.no_grad()
     def reset(self):
         for group in self.param_groups:
             for p in group['params']:
```

### Comparing `pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/diffgrad.py` & `pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/adabelief.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,94 +4,91 @@
 from torch.optim.optimizer import Optimizer
 
 from pytorch_optimizer.base.exception import NoSparseGradientError
 from pytorch_optimizer.base.optimizer import BaseOptimizer
 from pytorch_optimizer.base.types import BETAS, CLOSURE, DEFAULTS, LOSS, PARAMETERS
 
 
-class DiffGrad(Optimizer, BaseOptimizer):
-    r"""An Optimization Method for Convolutional Neural Networks.
+class AdaBelief(Optimizer, BaseOptimizer):
+    r"""Adapting Step-sizes by the Belief in Observed Gradients.
 
     :param params: PARAMETERS. iterable of parameters to optimize or dicts defining parameter groups.
     :param lr: float. learning rate.
     :param betas: BETAS. coefficients used for computing running averages of gradient and the squared hessian trace.
     :param weight_decay: float. weight decay (L2 penalty).
+    :param weight_decouple: bool. the optimizer uses decoupled weight decay as in AdamW.
+    :param fixed_decay: bool. fix weight decay.
     :param rectify: bool. perform the rectified update similar to RAdam.
-    :param n_sma_threshold: int. (recommended is 5).
-    :param degenerated_to_sgd: bool. degenerated to SGD.
-    :param amsgrad: bool. whether to use the AMSBound variant.
+    :param n_sma_threshold: number of SMA threshold (recommended is 5).
+    :param degenerated_to_sgd: bool. perform SGD update when variance of gradient is high.
+    :param ams_bound: bool. whether to use the AMSBound variant.
     :param r: float. EMA factor. between 0.9 ~ 0.99 is preferred.
     :param adanorm: bool. whether to use the AdaNorm variant.
     :param adam_debias: bool. Only correct the denominator to avoid inflating step sizes early in training.
     :param eps: float. term added to the denominator to improve numerical stability.
     """
 
     def __init__(
         self,
         params: PARAMETERS,
         lr: float = 1e-3,
         betas: BETAS = (0.9, 0.999),
         weight_decay: float = 0.0,
-        rectify: bool = False,
+        weight_decouple: bool = True,
+        fixed_decay: bool = False,
+        rectify: bool = True,
         n_sma_threshold: int = 5,
         degenerated_to_sgd: bool = True,
-        amsgrad: bool = False,
+        ams_bound: bool = False,
         r: float = 0.95,
         adanorm: bool = False,
         adam_debias: bool = False,
-        eps: float = 1e-8,
+        eps: float = 1e-16,
     ):
-        self.lr = lr
-        self.betas = betas
-        self.weight_decay = weight_decay
-        self.rectify = rectify
+        self.validate_learning_rate(lr)
+        self.validate_betas(betas)
+        self.validate_non_negative(weight_decay, 'weight_decay')
+        self.validate_non_negative(eps, 'eps')
+
         self.n_sma_threshold = n_sma_threshold
         self.degenerated_to_sgd = degenerated_to_sgd
-        self.eps = eps
-
-        self.validate_parameters()
 
         defaults: DEFAULTS = {
             'lr': lr,
             'betas': betas,
             'weight_decay': weight_decay,
+            'weight_decouple': weight_decouple,
+            'fixed_decay': fixed_decay,
             'rectify': rectify,
-            'amsgrad': amsgrad,
+            'ams_bound': ams_bound,
             'adanorm': adanorm,
             'adam_debias': adam_debias,
             'eps': eps,
         }
         if adanorm:
             defaults.update({'r': r})
 
         super().__init__(params, defaults)
 
-    def validate_parameters(self):
-        self.validate_learning_rate(self.lr)
-        self.validate_betas(self.betas)
-        self.validate_weight_decay(self.weight_decay)
-        self.validate_epsilon(self.eps)
-
     def __str__(self) -> str:
-        return 'diffRGrad' if self.rectify else 'diffGrad'
+        return 'AdaBelief'
 
     @torch.no_grad()
     def reset(self):
         for group in self.param_groups:
             group['step'] = 0
             for p in group['params']:
                 state = self.state[p]
 
                 state['exp_avg'] = torch.zeros_like(p)
-                state['exp_avg_sq'] = torch.zeros_like(p)
-                state['previous_grad'] = torch.zeros_like(p)
-                if group['amsgrad']:
-                    state['max_exp_avg_sq'] = torch.zeros_like(p)
+                state['exp_avg_var'] = torch.zeros_like(p)
                 if group['adanorm']:
                     state['exp_grad_norm'] = torch.zeros((1,), dtype=p.dtype, device=p.device)
+                if group['ams_bound']:
+                    state['max_exp_avg_var'] = torch.zeros_like(p)
 
     @torch.no_grad()
     def step(self, closure: CLOSURE = None) -> LOSS:
         loss: LOSS = None
         if closure is not None:
             with torch.enable_grad():
                 loss = closure()
@@ -100,94 +97,82 @@
             if 'step' in group:
                 group['step'] += 1
             else:
                 group['step'] = 1
 
             beta1, beta2 = group['betas']
 
-            bias_correction1 = 1.0 - beta1 ** group['step']
+            bias_correction1: float = 1.0 - beta1 ** group['step']
+            bias_correction2_sq: float = math.sqrt(1.0 - beta2 ** group['step'])
 
-            if group['rectify']:
-                n_sma_max: float = 2.0 / (1.0 - beta2) - 1.0
-                beta2_t: float = beta2 ** group['step']
-                n_sma: float = n_sma_max - 2 * group['step'] * beta2_t / (1.0 - beta2_t)
+            step_size, n_sma = self.get_rectify_step_size(
+                is_rectify=group['rectify'],
+                step=group['step'],
+                lr=group['lr'],
+                beta2=beta2,
+                n_sma_threshold=self.n_sma_threshold,
+                degenerated_to_sgd=self.degenerated_to_sgd,
+            )
+
+            step_size = self.apply_adam_debias(
+                adam_debias=group['adam_debias'],
+                step_size=step_size,
+                bias_correction1=bias_correction1,
+            )
 
             for p in group['params']:
                 if p.grad is None:
                     continue
 
                 grad = p.grad
                 if grad.is_sparse:
                     raise NoSparseGradientError(str(self))
 
                 state = self.state[p]
                 if len(state) == 0:
                     state['exp_avg'] = torch.zeros_like(p)
-                    state['exp_avg_sq'] = torch.zeros_like(p)
-                    state['previous_grad'] = torch.zeros_like(p)
-                    if group['amsgrad']:
-                        state['max_exp_avg_sq'] = torch.zeros_like(p)
+                    state['exp_avg_var'] = torch.zeros_like(p)
                     if group['adanorm']:
                         state['exp_grad_norm'] = torch.zeros((1,), dtype=grad.dtype, device=grad.device)
+                    if group['ams_bound']:
+                        state['max_exp_avg_var'] = torch.zeros_like(p)
 
-                exp_avg, exp_avg_sq = state['exp_avg'], state['exp_avg_sq']
-
-                s_grad = grad
-                if group['adanorm']:
-                    grad_norm = torch.linalg.norm(grad)
-
-                    exp_grad_norm = state['exp_grad_norm']
-                    exp_grad_norm.mul_(group['r']).add_(grad_norm, alpha=1.0 - group['r'])
-
-                    if exp_grad_norm > grad_norm:
-                        s_grad *= exp_grad_norm / grad_norm
+                self.apply_weight_decay(
+                    p=p,
+                    grad=grad,
+                    lr=group['lr'],
+                    weight_decay=group['weight_decay'],
+                    weight_decouple=group['weight_decouple'],
+                    fixed_decay=group['fixed_decay'],
+                )
+
+                s_grad = self.get_adanorm_gradient(
+                    grad=grad,
+                    adanorm=group['adanorm'],
+                    exp_grad_norm=state.get('exp_grad_norm', None),
+                    r=group.get('r', None),
+                )
 
+                exp_avg, exp_avg_var = state['exp_avg'], state['exp_avg_var']
                 exp_avg.mul_(beta1).add_(s_grad, alpha=1.0 - beta1)
-                exp_avg_sq.mul_(beta2).addcmul_(grad, grad, value=1.0 - beta2)
 
-                if group['amsgrad']:
-                    max_exp_avg_sq = state['max_exp_avg_sq']
-                    torch.max(max_exp_avg_sq, exp_avg_sq, out=max_exp_avg_sq)
-                    de_nom = max_exp_avg_sq.add(group['eps']).sqrt()
-                else:
-                    de_nom = exp_avg_sq.add(group['eps']).sqrt()
-
-                de_nom.add_(group['eps'])
-
-                # compute diffGrad coefficient (dfc)
-                dfc = state['previous_grad'].clone()
-                dfc.sub_(grad).abs_().sigmoid_().mul_(exp_avg)
-                state['previous_grad'].copy_(grad)
+                grad_residual = grad - exp_avg
+                exp_avg_var.mul_(beta2).addcmul_(grad_residual, grad_residual, value=1.0 - beta2).add_(group['eps'])
+
+                de_nom = self.apply_ams_bound(
+                    ams_bound=group['ams_bound'],
+                    exp_avg_sq=exp_avg_var,
+                    max_exp_avg_sq=state.get('max_exp_avg_var', None),
+                    eps=group['eps'],
+                )
 
                 if not group['rectify']:
-                    step_size: float = group['lr'] if group['adam_debias'] else group['lr'] / bias_correction1
+                    de_nom.div_(bias_correction2_sq)
                     p.addcdiv_(exp_avg, de_nom, value=-step_size)
                     continue
 
                 if n_sma >= self.n_sma_threshold:
-                    step_size = math.sqrt(
-                        (1 - beta2_t)
-                        * (n_sma - 4)
-                        / (n_sma_max - 4)
-                        * (n_sma - 2)
-                        / n_sma
-                        * n_sma_max
-                        / (n_sma_max - 2)
-                    )
-                elif self.degenerated_to_sgd:
-                    step_size = 1.0
-                else:
-                    step_size = -1
-
-                if not group['adam_debias']:
-                    step_size /= bias_correction1
-
-                if group['weight_decay'] > 0.0:
-                    p.add_(p, alpha=-group['weight_decay'] * group['lr'])
-
-                if n_sma >= self.n_sma_threshold:
-                    de_nom = exp_avg_sq.sqrt().add_(group['eps'])
-                    p.addcdiv_(dfc, de_nom, value=-step_size * group['lr'])
+                    p.addcdiv_(exp_avg, de_nom, value=-step_size)
                 elif step_size > 0:
-                    p.add_(exp_avg, alpha=-step_size * group['lr'])
+                    p.add_(exp_avg, alpha=-step_size)
 
         return loss
```

### Comparing `pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/fp16.py` & `pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/fp16.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/fromage.py` & `pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/fromage.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,25 +20,21 @@
     :param params: PARAMETERS. iterable of parameters to optimize or dicts defining parameter groups.
     :param lr: float. learning rate.
     :param p_bound: Optional[float]. Restricts the optimisation to a bounded set. A value of 2.0 restricts parameter
         norms to lie within 2x their initial norms. This regularises the model class.
     """
 
     def __init__(self, params: PARAMETERS, lr: float = 1e-2, p_bound: Optional[float] = None):
-        self.lr = lr
-        self.p_bound = p_bound
+        self.validate_learning_rate(lr)
 
-        self.validate_parameters()
+        self.p_bound = p_bound
 
         defaults: DEFAULTS = {'lr': lr}
         super().__init__(params, defaults)
 
-    def validate_parameters(self):
-        self.validate_learning_rate(self.lr)
-
     def __str__(self) -> str:
         return 'Fromage'
 
     @torch.no_grad()
     def reset(self):
         for group in self.param_groups:
             for p in group['params']:
```

### Comparing `pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/gsam.py` & `pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/gsam.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,14 +50,16 @@
         model: nn.Module,
         rho_scheduler,
         alpha: float = 0.4,
         adaptive: bool = False,
         perturb_eps: float = 1e-12,
         **kwargs,
     ):
+        self.validate_range(alpha, 'alpha', 0.0, 1.0)
+
         self.model = model
         self.rho_scheduler = rho_scheduler
         self.alpha = alpha
         self.adaptive = adaptive
         self.perturb_eps = perturb_eps
 
         self.rho_t: float = 0.0
@@ -69,25 +71,20 @@
         else:  # PyTorch <= 1.11.0 does not have AVG, need to manually average across processes
             self.grad_reduce = ReduceOp.SUM
             self.manual_average: bool = True
 
         self.base_optimizer = base_optimizer
         self.param_groups = self.base_optimizer.param_groups
 
-        self.validate_parameters()
-
         defaults: DEFAULTS = {'adaptive': adaptive}
         defaults.update(kwargs)
         super().__init__(params, defaults)
 
         self.update_rho_t()
 
-    def validate_parameters(self):
-        self.validate_alpha(self.alpha)
-
     def __str__(self) -> str:
         return 'GSAM'
 
     @torch.no_grad()
     def reset(self):
         pass
```

### Comparing `pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/lamb.py` & `pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/swats.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,229 +1,193 @@
 import math
-from typing import Union
 
 import torch
-from torch.optim import Optimizer
+from torch.optim.optimizer import Optimizer
 
 from pytorch_optimizer.base.exception import NoSparseGradientError
 from pytorch_optimizer.base.optimizer import BaseOptimizer
 from pytorch_optimizer.base.types import BETAS, CLOSURE, DEFAULTS, LOSS, PARAMETERS
-from pytorch_optimizer.optimizer.utils import get_global_gradient_norm
 
 
-class Lamb(Optimizer, BaseOptimizer):
-    r"""Large Batch Optimization for Deep Learning.
+class SWATS(Optimizer, BaseOptimizer):
+    r"""Improving Generalization Performance by Switching from Adam to SGD.
 
-        This Lamb implementation is based on the paper v3, which does not use de-biasing.
+        Currently, there's convergence issue. So, careful at using it.
 
     :param params: PARAMETERS. iterable of parameters to optimize or dicts defining parameter groups.
     :param lr: float. learning rate.
     :param betas: BETAS. coefficients used for computing running averages of gradient and the squared hessian trace.
     :param weight_decay: float. weight decay (L2 penalty).
-    :param rectify: bool. perform the rectified update similar to RAdam.
-    :param degenerated_to_sgd: bool. degenerated to SGD.
-    :param n_sma_threshold: int. (recommended is 5).
-    :param grad_averaging: bool. whether apply (1 - beta2) to gradient when calculating running averages of gradient.
-    :param max_grad_norm: float. max gradient norm to clip.
+    :param weight_decouple: bool. the optimizer uses decoupled weight decay as in AdamW.
+    :param fixed_decay: bool. fix weight decay.
+    :param ams_bound: bool. whether to use the ams_bound variant of this algorithm from the paper.
+    :param nesterov: bool. enables Nesterov momentum.
     :param r: float. EMA factor. between 0.9 ~ 0.99 is preferred.
     :param adanorm: bool. whether to use the AdaNorm variant.
     :param adam_debias: bool. Only correct the denominator to avoid inflating step sizes early in training.
-    :param adam: bool. always use trust ratio = 1, which turns this into Adam. Useful for comparison purposes.
-    :param pre_norm: bool. perform pre-normalization of all gradients.
     :param eps: float. term added to the denominator to improve numerical stability.
     """
 
-    clamp: float = 10.0
-
     def __init__(
         self,
         params: PARAMETERS,
         lr: float = 1e-3,
         betas: BETAS = (0.9, 0.999),
         weight_decay: float = 0.0,
-        rectify: bool = False,
-        degenerated_to_sgd: bool = False,
-        n_sma_threshold: int = 5,
-        grad_averaging: bool = True,
-        max_grad_norm: float = 1.0,
-        adam: bool = False,
-        pre_norm: bool = False,
+        weight_decouple: bool = False,
+        fixed_decay: bool = False,
+        ams_bound: bool = False,
+        nesterov: bool = False,
         r: float = 0.95,
         adanorm: bool = False,
         adam_debias: bool = False,
-        eps: float = 1e-6,
+        eps: float = 1e-9,
     ):
-        self.lr = lr
-        self.betas = betas
-        self.weight_decay = weight_decay
-        self.degenerated_to_sgd = degenerated_to_sgd
-        self.n_sma_threshold = n_sma_threshold
-        self.max_grad_norm = max_grad_norm
-        self.pre_norm = pre_norm
-        self.eps = eps
-
-        self.validate_parameters()
+        self.validate_learning_rate(lr)
+        self.validate_betas(betas)
+        self.validate_non_negative(weight_decay, 'weight_decay')
+        self.validate_non_negative(eps, 'eps')
 
         defaults: DEFAULTS = {
             'lr': lr,
             'betas': betas,
             'weight_decay': weight_decay,
-            'rectify': rectify,
-            'grad_averaging': grad_averaging,
-            'max_grad_norm': max_grad_norm,
-            'adam': adam,
+            'weight_decouple': weight_decouple,
+            'fixed_decay': fixed_decay,
+            'ams_bound': ams_bound,
+            'nesterov': nesterov,
             'adanorm': adanorm,
             'adam_debias': adam_debias,
+            'phase': 'adam',
             'eps': eps,
         }
         if adanorm:
             defaults.update({'r': r})
 
         super().__init__(params, defaults)
 
-    def validate_parameters(self):
-        self.validate_learning_rate(self.lr)
-        self.validate_betas(self.betas)
-        self.validate_weight_decay(self.weight_decay)
-        self.validate_epsilon(self.eps)
-        self.validate_norm(self.max_grad_norm)
-
     def __str__(self) -> str:
-        return 'Lamb'
+        return 'SWATS'
 
     @torch.no_grad()
     def reset(self):
         for group in self.param_groups:
+            group['step'] = 0
             for p in group['params']:
                 state = self.state[p]
 
-                state['step'] = 0
                 state['exp_avg'] = torch.zeros_like(p)
                 state['exp_avg_sq'] = torch.zeros_like(p)
+                state['exp_avg2'] = torch.zeros((1,), dtype=p.dtype, device=p.device)
+                if group['ams_bound']:
+                    state['max_exp_avg_sq'] = torch.zeros_like(p)
                 if group['adanorm']:
                     state['exp_grad_norm'] = torch.zeros((1,), dtype=p.dtype, device=p.device)
 
     @torch.no_grad()
-    def get_global_gradient_norm(self) -> Union[torch.Tensor, float]:
-        if self.defaults['max_grad_norm'] == 0.0:
-            return 1.0
-
-        global_grad_norm = get_global_gradient_norm(self.param_groups, self.param_groups[0]['params'][0].device)
-        global_grad_norm.sqrt_().add_(self.eps)
-
-        return torch.clamp(self.defaults['max_grad_norm'] / global_grad_norm, max=1.0)
-
-    @torch.no_grad()
     def step(self, closure: CLOSURE = None) -> LOSS:
         loss: LOSS = None
         if closure is not None:
             with torch.enable_grad():
                 loss = closure()
 
-        grad_norm = 1.0
-        if self.pre_norm:
-            grad_norm = self.get_global_gradient_norm()
-
         for group in self.param_groups:
             if 'step' in group:
                 group['step'] += 1
             else:
                 group['step'] = 1
 
             beta1, beta2 = group['betas']
-            beta3 = 1.0 - beta1 if group['grad_averaging'] else 1.0
 
-            bias_correction1 = 1.0 - beta1 ** group['step']
-
-            if group['rectify']:
-                n_sma_max: float = 2.0 / (1.0 - beta2) - 1.0
-                beta2_t: float = beta2 ** group['step']
-                n_sma: float = n_sma_max - 2 * group['step'] * beta2_t / (1.0 - beta2_t)
+            bias_correction1: float = 1.0 - beta1 ** group['step']
+            bias_correction2: float = 1.0 - beta2 ** group['step']
 
             for p in group['params']:
                 if p.grad is None:
                     continue
 
                 grad = p.grad
                 if grad.is_sparse:
                     raise NoSparseGradientError(str(self))
 
-                if self.pre_norm:
-                    grad.div_(grad_norm)
-
                 state = self.state[p]
 
                 if len(state) == 0:
                     state['exp_avg'] = torch.zeros_like(p)
                     state['exp_avg_sq'] = torch.zeros_like(p)
+                    state['exp_avg2'] = torch.zeros((1,), dtype=grad.dtype, device=grad.device)
+                    if group['ams_bound']:
+                        state['max_exp_avg_sq'] = torch.zeros_like(p)
                     if group['adanorm']:
                         state['exp_grad_norm'] = torch.zeros((1,), dtype=grad.dtype, device=grad.device)
 
-                s_grad = grad
-                if group['adanorm']:
-                    grad_norm = torch.linalg.norm(grad)
+                self.apply_weight_decay(
+                    p=p,
+                    grad=p.grad,
+                    lr=group['lr'],
+                    weight_decay=group['weight_decay'],
+                    weight_decouple=group['weight_decouple'],
+                    fixed_decay=group['fixed_decay'],
+                )
+
+                if group['phase'] == 'sgd':
+                    if 'momentum_buffer' not in state:
+                        state['momentum_buffer'] = torch.zeros_like(grad)
+
+                    buf = state['momentum_buffer']
+                    buf.mul_(beta1).add_(grad)
+
+                    grad = buf.clone()
+
+                    grad.mul_(1.0 - beta1)
+                    if group['nesterov']:
+                        grad.add_(buf, alpha=beta1)
 
-                    exp_grad_norm = state['exp_grad_norm']
-                    exp_grad_norm.mul_(group['r']).add_(grad_norm, alpha=1.0 - group['r'])
+                    p.add_(grad, alpha=-group['lr'])
 
-                    if exp_grad_norm > grad_norm:
-                        s_grad *= exp_grad_norm / grad_norm
+                    continue
 
-                exp_avg, exp_avg_sq = state['exp_avg'], state['exp_avg_sq']
+                s_grad = self.get_adanorm_gradient(
+                    grad=grad,
+                    adanorm=group['adanorm'],
+                    exp_grad_norm=state.get('exp_grad_norm', None),
+                    r=group.get('r', None),
+                )
 
-                exp_avg.mul_(beta1).add_(s_grad, alpha=beta3)
+                exp_avg, exp_avg_sq = state['exp_avg'], state['exp_avg_sq']
+                exp_avg.mul_(beta1).add_(s_grad, alpha=1.0 - beta1)
                 exp_avg_sq.mul_(beta2).addcmul_(grad, grad, value=1.0 - beta2)
 
-                if group['weight_decay'] > 0.0:
-                    p.add_(p, alpha=-group['weight_decay'] * group['lr'])
-
-                if group['rectify']:
-                    if n_sma >= self.n_sma_threshold:
-                        step_size = math.sqrt(
-                            (1 - beta2_t)
-                            * (n_sma - 4)
-                            / (n_sma_max - 4)
-                            * (n_sma - 2)
-                            / n_sma
-                            * n_sma_max
-                            / (n_sma_max - 2)
-                        )
-                    elif self.degenerated_to_sgd:
-                        step_size = 1.0
-                    else:
-                        step_size = -1
-
-                    if not group['adam_debias']:
-                        step_size /= bias_correction1
-                else:
-                    step_size = group['lr']
-
-                if group['rectify']:
-                    update = p.clone()
-                    if n_sma >= self.n_sma_threshold:
-                        de_nom = exp_avg_sq.sqrt().add_(group['eps'])
-                        update.addcdiv_(exp_avg, de_nom, value=-step_size)
-                    else:
-                        update.add_(exp_avg, alpha=-step_size)
-                else:
-                    update = exp_avg / exp_avg_sq.sqrt().add(group['eps'])
-
-                weight_norm = torch.linalg.norm(p).clamp(0, self.clamp)
-                p_norm = torch.linalg.norm(update)
-                trust_ratio: float = 1.0 if weight_norm == 0 or p_norm == 0 else weight_norm / (p_norm + self.eps)
-
-                state['weight_norm'] = weight_norm
-                state['adam_norm'] = p_norm
-                state['trust_ratio'] = trust_ratio
-
-                if group['adam']:
-                    trust_ratio = 1.0
-
-                if group['rectify']:
-                    if n_sma >= self.n_sma_threshold:
-                        p.addcdiv_(exp_avg, de_nom, value=-step_size * trust_ratio)
-                    else:
-                        p.add_(exp_avg, alpha=-step_size * trust_ratio)
-                else:
-                    p.add_(update, alpha=-step_size * trust_ratio)
+                de_nom = self.apply_ams_bound(
+                    ams_bound=group['ams_bound'],
+                    exp_avg_sq=exp_avg_sq,
+                    max_exp_avg_sq=state.get('max_exp_avg_sq', None),
+                    eps=group['eps'],
+                )
+
+                step_size: float = self.apply_adam_debias(
+                    adam_debias=group['adam_debias'],
+                    step_size=group['lr'] * math.sqrt(bias_correction2),
+                    bias_correction1=bias_correction1,
+                )
+
+                perturb = exp_avg.clone()
+                perturb.div_(de_nom).mul(-step_size)
+
+                p.add_(perturb)
+
+                perturb_view = perturb.view(-1)
+                pg = perturb_view.dot(grad.view(-1))
+
+                if pg != 0:
+                    scaling = perturb_view.dot(perturb_view).div_(-pg)
+
+                    exp_avg2 = state['exp_avg2']
+                    exp_avg2.mul_(beta2).add_(scaling, alpha=1.0 - beta2)
+
+                    corrected_exp_avg = exp_avg2 / bias_correction2
+
+                    if group['step'] > 1 and corrected_exp_avg.allclose(scaling, rtol=group['eps']):
+                        group['phase'] = 'sgd'
+                        group['lr'] = corrected_exp_avg.item()
 
         return loss
```

### Comparing `pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/lars.py` & `pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/sgdp.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,117 +1,122 @@
 import torch
-from torch.optim import Optimizer
+from torch.optim.optimizer import Optimizer
 
 from pytorch_optimizer.base.exception import NoSparseGradientError
 from pytorch_optimizer.base.optimizer import BaseOptimizer
 from pytorch_optimizer.base.types import CLOSURE, DEFAULTS, LOSS, PARAMETERS
+from pytorch_optimizer.optimizer.utils import projection
 
 
-class LARS(Optimizer, BaseOptimizer):
-    r"""Layer-wise Adaptive Rate Scaling (no rate scaling or weight decay for parameters <= 1D).
+class SGDP(Optimizer, BaseOptimizer):
+    r"""SGD + Slowing Down the Slowdown for Momentum Optimizers on Scale-invariant Weights.
 
     :param params: PARAMETERS. iterable of parameters to optimize or dicts defining parameter groups.
     :param lr: float. learning rate.
-    :param weight_decay: float. weight decay (L2 penalty).
-    :param momentum: float. momentum.
+    :param momentum: float. momentum factor.
     :param dampening: float. dampening for momentum.
-    :param trust_coefficient: float. trust_coefficient.
+    :param weight_decay: float. weight decay (L2 penalty).
+    :param weight_decouple: bool. the optimizer uses decoupled weight decay as in AdamW.
+    :param fixed_decay: bool. fix weight decay.
+    :param delta: float. threshold that determines whether a set of parameters is scale invariant or not.
+    :param wd_ratio: float. relative weight decay applied on scale-invariant parameters compared to that applied
+        on scale-variant parameters.
     :param nesterov: bool. enables nesterov momentum.
-    :param eps: float. epsilon.
+    :param eps: float. term added to the denominator to improve numerical stability.
     """
 
     def __init__(
         self,
         params: PARAMETERS,
         lr: float = 1e-3,
-        weight_decay: float = 0.0,
-        momentum: float = 0.9,
+        momentum: float = 0.0,
         dampening: float = 0.0,
-        trust_coefficient: float = 1e-3,
+        weight_decay: float = 0.0,
+        weight_decouple: bool = True,
+        fixed_decay: bool = False,
+        delta: float = 0.1,
+        wd_ratio: float = 0.1,
         nesterov: bool = False,
-        eps: float = 1e-6,
+        eps: float = 1e-8,
     ):
-        self.lr = lr
-        self.weight_decay = weight_decay
-        self.momentum = momentum
-        self.dampening = dampening
-        self.trust_coefficient = trust_coefficient
-        self.nesterov = nesterov
-        self.eps = eps
-
-        self.validate_parameters()
+        self.validate_learning_rate(lr)
+        self.validate_non_negative(weight_decay, 'weight_decay')
+        self.validate_range(wd_ratio, 'wd_ratio', 0.0, 1.0)
+        self.validate_non_negative(eps, 'eps')
 
         defaults: DEFAULTS = {
             'lr': lr,
             'weight_decay': weight_decay,
+            'weight_decouple': weight_decouple,
+            'fixed_decay': fixed_decay,
             'momentum': momentum,
             'dampening': dampening,
-            'trust_coefficient': trust_coefficient,
+            'delta': delta,
+            'wd_ratio': wd_ratio,
             'nesterov': nesterov,
+            'eps': eps,
         }
         super().__init__(params, defaults)
 
-    def validate_parameters(self):
-        self.validate_learning_rate(self.lr)
-        self.validate_weight_decay(self.weight_decay)
-        self.validate_momentum(self.momentum)
-        self.validate_trust_coefficient(self.trust_coefficient)
-        self.validate_epsilon(self.eps)
-
     def __str__(self) -> str:
-        return 'Lars'
+        return 'SGDP'
 
     @torch.no_grad()
     def reset(self):
         for group in self.param_groups:
             for p in group['params']:
                 state = self.state[p]
 
-                state['mu'] = torch.zeros_like(p)
+                state['momentum'] = torch.zeros_like(p)
 
     @torch.no_grad()
     def step(self, closure: CLOSURE = None) -> LOSS:
         loss: LOSS = None
         if closure is not None:
             with torch.enable_grad():
                 loss = closure()
 
         for group in self.param_groups:
+            momentum = group['momentum']
             for p in group['params']:
                 if p.grad is None:
                     continue
 
                 grad = p.grad
                 if grad.is_sparse:
                     raise NoSparseGradientError(str(self))
 
-                if p.ndim > 1:  # if not normalization gamma/beta or bias
-                    param_norm = torch.linalg.norm(p)
-                    update_norm = torch.linalg.norm(grad)
-
-                    one = torch.ones_like(param_norm)
-
-                    trust_ratio = torch.where(
-                        param_norm > 0.0,
-                        torch.where(update_norm > 0.0, (group['trust_coefficient'] * param_norm / update_norm), one),
-                        one,
-                    )
+                state = self.state[p]
+                if len(state) == 0:
+                    state['momentum'] = torch.zeros_like(p)
 
-                    grad.add_(p, alpha=group['weight_decay'])
-                    grad.mul_(trust_ratio)
+                buf = state['momentum']
+                buf.mul_(momentum).add_(grad, alpha=1.0 - group['dampening'])
+
+                d_p = buf.clone()
+                if group['nesterov']:
+                    d_p = d_p.mul_(momentum).add_(grad)
+
+                wd_ratio: float = 1.0
+                if len(p.shape) > 1:
+                    d_p, wd_ratio = projection(
+                        p,
+                        grad,
+                        d_p,
+                        group['delta'],
+                        group['wd_ratio'],
+                        group['eps'],
+                    )
 
-                if group['momentum'] > 0.0:
-                    state = self.state[p]
-                    if 'momentum_buffer' not in state:
-                        state['momentum_buffer'] = grad.clone().detach()
-
-                    mb = state['momentum_buffer']
-                    mb.mul_(group['momentum']).add_(grad, alpha=1.0 - group['dampening'])
-
-                    if group['nesterov']:
-                        grad.add_(mb, alpha=group['momentum'])
-                    else:
-                        grad.copy_(mb)
+                self.apply_weight_decay(
+                    p=p,
+                    grad=None,
+                    lr=group['lr'],
+                    weight_decay=group['weight_decay'],
+                    weight_decouple=group['weight_decouple'],
+                    fixed_decay=group['fixed_decay'],
+                    ratio=wd_ratio / (1.0 - momentum),
+                )
 
-                p.add_(grad, alpha=-group['lr'])
+                p.add_(d_p, alpha=-group['lr'])
 
         return loss
```

### Comparing `pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/lion.py` & `pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/lion.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,54 +11,51 @@
     r"""Symbolic Discovery of Optimization Algorithms.
 
     :param params: PARAMETERS. iterable of parameters to optimize or dicts defining parameter groups.
     :param lr: float. learning rate.
     :param betas: BETAS. coefficients used for computing running averages of gradient and the squared hessian trace.
     :param weight_decay: float. weight decay (L2 penalty).
     :param weight_decouple: bool. the optimizer uses decoupled weight decay as in AdamW.
+    :param fixed_decay: bool. fix weight decay.
     :param use_gc: bool. use gradient centralization.
     :param r: float. EMA factor. between 0.9 ~ 0.99 is preferred.
     :param adanorm: bool. whether to use the AdaNorm variant.
     """
 
     def __init__(
         self,
         params: PARAMETERS,
         lr: float = 1e-4,
         betas: BETAS = (0.9, 0.99),
         weight_decay: float = 0.0,
         weight_decouple: bool = True,
+        fixed_decay: bool = False,
         use_gc: bool = False,
         r: float = 0.95,
         adanorm: bool = False,
     ):
-        self.lr = lr
-        self.betas = betas
-        self.weight_decay = weight_decay
-        self.use_gc = use_gc
+        self.validate_learning_rate(lr)
+        self.validate_betas(betas)
+        self.validate_non_negative(weight_decay, 'weight_decay')
 
-        self.validate_parameters()
+        self.use_gc = use_gc
 
         defaults: DEFAULTS = {
             'lr': lr,
             'betas': betas,
             'weight_decay': weight_decay,
             'weight_decouple': weight_decouple,
+            'fixed_decay': fixed_decay,
             'adanorm': adanorm,
         }
         if adanorm:
             defaults.update({'r': r})
 
         super().__init__(params, defaults)
 
-    def validate_parameters(self):
-        self.validate_learning_rate(self.lr)
-        self.validate_betas(self.betas)
-        self.validate_weight_decay(self.weight_decay)
-
     def __str__(self) -> str:
         return 'Lion'
 
     @torch.no_grad()
     def reset(self):
         for group in self.param_groups:
             for p in group['params']:
@@ -73,15 +70,14 @@
         loss: LOSS = None
         if closure is not None:
             with torch.enable_grad():
                 loss = closure()
 
         for group in self.param_groups:
             beta1, beta2 = group['betas']
-            weight_decay = group['weight_decay']
             for p in group['params']:
                 if p.grad is None:
                     continue
 
                 grad = p.grad
                 if grad.is_sparse:
                     raise NoSparseGradientError(str(self))
@@ -92,29 +88,29 @@
                     state['exp_avg'] = torch.zeros_like(p)
                     if group['adanorm']:
                         state['exp_grad_norm'] = torch.zeros((1,), dtype=grad.dtype, device=grad.device)
 
                 if self.use_gc:
                     grad = centralize_gradient(grad, gc_conv_only=False)
 
-                if weight_decay > 0.0:
-                    if group['weight_decouple']:
-                        p.mul_(1.0 - group['lr'] * weight_decay)
-                    else:
-                        grad.add_(p, alpha=weight_decay)
-
-                s_grad = grad
-                if group['adanorm']:
-                    grad_norm = torch.linalg.norm(grad)
-
-                    exp_grad_norm = state['exp_grad_norm']
-                    exp_grad_norm.mul_(group['r']).add_(grad_norm, alpha=1.0 - group['r'])
-
-                    if exp_grad_norm > grad_norm:
-                        s_grad *= exp_grad_norm / grad_norm
+                self.apply_weight_decay(
+                    p=p,
+                    grad=p.grad,
+                    lr=group['lr'],
+                    weight_decay=group['weight_decay'],
+                    weight_decouple=group['weight_decouple'],
+                    fixed_decay=group['fixed_decay'],
+                )
+
+                s_grad = self.get_adanorm_gradient(
+                    grad=grad,
+                    adanorm=group['adanorm'],
+                    exp_grad_norm=state.get('exp_grad_norm', None),
+                    r=group.get('r', None),
+                )
 
                 exp_avg = state['exp_avg']
                 update = exp_avg.clone()
 
                 update.mul_(beta1).add_(grad, alpha=1.0 - beta1).sign_()
                 exp_avg.mul_(beta2).add_(s_grad, alpha=1.0 - beta2)
```

### Comparing `pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/lookahead.py` & `pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/lookahead.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,40 +19,37 @@
     def __init__(
         self,
         optimizer: OPTIMIZER,
         k: int = 5,
         alpha: float = 0.5,
         pullback_momentum: str = 'none',
     ):
-        self.optimizer = optimizer
-        self.k = k
+        self.validate_positive(k, 'k')
+        self.validate_range(alpha, 'alpha', 0.0, 1.0)
+        self.validate_pullback_momentum(pullback_momentum)
+
         self.alpha = alpha
+        self.k = k
         self.pullback_momentum = pullback_momentum
 
-        self.validate_parameters()
-
+        self.optimizer = optimizer
         self.param_groups = self.optimizer.param_groups
         self.state: STATE = defaultdict(dict)
 
         for group in self.param_groups:
             if 'counter' not in group:
                 group['counter'] = 0
 
             for p in group['params']:
                 state = self.state[p]
                 state['slow_params'] = torch.empty_like(p)
                 state['slow_params'].copy_(p)
                 if self.pullback_momentum == 'pullback':
                     state['slow_momentum'] = torch.zeros_like(p)
 
-    def validate_parameters(self):
-        self.validate_lookahead_k(self.k)
-        self.validate_alpha(self.alpha)
-        self.validate_pullback_momentum(self.pullback_momentum)
-
     def __getstate__(self):
         return {
             'state': self.state,
             'optimizer': self.optimizer,
             'alpha': self.alpha,
             'k': self.k,
             'pullback_momentum': self.pullback_momentum,
```

### Comparing `pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/madgrad.py` & `pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/madgrad.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,43 +18,40 @@
 
     :param params: PARAMETERS. iterable of parameters to optimize or dicts defining parameter groups.
     :param lr: float. learning rate.
     :param eps: float. term added to the denominator to improve numerical stability.
     :param weight_decay: float. weight decay (L2 penalty).
         MADGRAD optimizer requires less weight decay than other methods, often as little as zero.
         On sparse problems both weight_decay and momentum should be set to 0.
-    :param decouple_decay: float. Apply AdamW style decoupled weight decay.
+    :param weight_decouple: float. Apply AdamW style decoupled weight decay.
     """
 
     def __init__(
         self,
         params: PARAMETERS,
         lr: float = 1e-3,
         momentum: float = 0.9,
         weight_decay: float = 0.0,
-        decouple_decay: bool = False,
+        weight_decouple: bool = False,
         eps: float = 1e-6,
     ):
-        self.lr = lr
-        self.momentum = momentum
-        self.weight_decay = weight_decay
-        self.decouple_decay = decouple_decay
-        self.eps = eps
-
-        self.validate_parameters()
-
-        defaults: DEFAULTS = {'lr': lr, 'weight_decay': weight_decay, 'momentum': momentum, 'eps': eps}
+        self.validate_learning_rate(lr)
+        self.validate_non_negative(weight_decay, 'weight_decay')
+        self.validate_range(momentum, 'momentum', 0.0, 1.0)
+        self.validate_non_negative(eps, 'eps')
+
+        defaults: DEFAULTS = {
+            'lr': lr,
+            'weight_decay': weight_decay,
+            'weight_decouple': weight_decouple,
+            'momentum': momentum,
+            'eps': eps,
+        }
         super().__init__(params, defaults)
 
-    def validate_parameters(self):
-        self.validate_learning_rate(self.lr)
-        self.validate_weight_decay(self.weight_decay)
-        self.validate_momentum(self.momentum)
-        self.validate_epsilon(self.eps)
-
     def __str__(self) -> str:
         return 'MADGRAD'
 
     @torch.no_grad()
     def reset(self):
         self.state['k'] = torch.tensor([0], dtype=torch.long, requires_grad=False)
 
@@ -97,15 +94,15 @@
                     if momentum > 0.0:
                         state['x0'] = torch.clone(p).detach()
 
                 if momentum > 0.0 and grad.is_sparse:
                     raise NoSparseGradientError(str(self), note='momentum > 0.0')
 
                 grad_sum_sq, s = state['grad_sum_sq'], state['s']
-                if weight_decay > 0.0 and not self.decouple_decay:
+                if weight_decay > 0.0 and not group['weight_decouple']:
                     if grad.is_sparse:
                         raise NoSparseGradientError(str(self), note='weight_decay')
 
                     # original implementation. not AdamW style
                     grad.add_(p, alpha=weight_decay)
 
                 if grad.is_sparse:
@@ -148,22 +145,22 @@
                     rms = grad_sum_sq.pow(1 / 3).add_(eps)
 
                     if eps == 0.0:
                         rms[rms == 0] = float('inf')
 
                     s.add_(grad, alpha=_lambda)
 
-                    if weight_decay > 0.0 and self.decouple_decay:
+                    if weight_decay > 0.0 and group['weight_decouple']:
                         p_old = p.clone()
 
                     if momentum == 0.0:
                         p.copy_(x0.addcdiv(s, rms, value=-1))
                     else:
                         z = x0.addcdiv(s, rms, value=-1)
                         p.mul_(momentum).add_(z, alpha=1.0 - momentum)
 
-                    if weight_decay > 0.0 and self.decouple_decay:
+                    if weight_decay > 0.0 and group['weight_decouple']:
                         p.add_(p_old, alpha=-lr * weight_decay)
 
         self.state['k'] += 1
 
         return loss
```

### Comparing `pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/msvag.py` & `pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/msvag.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,26 +11,20 @@
 
     :param params: PARAMETERS. iterable of parameters to optimize or dicts defining parameter groups.
     :param lr: float. learning rate.
     :param beta: float. Moving average (momentum) constant (scalar tensor or float value).
     """
 
     def __init__(self, params: PARAMETERS, lr: float = 1e-2, beta: float = 0.9):
-        self.lr = lr
-        self.beta = beta
-
-        self.validate_parameters()
+        self.validate_learning_rate(lr)
+        self.validate_range(beta, 'beta', 0.0, 1.0, range_type='[]')
 
         defaults: DEFAULTS = {'lr': lr, 'beta': beta}
         super().__init__(params, defaults)
 
-    def validate_parameters(self):
-        self.validate_learning_rate(self.lr)
-        self.validate_beta(self.beta)
-
     def __str__(self) -> str:
         return 'MSVAG'
 
     @torch.no_grad()
     def reset(self):
         for group in self.param_groups:
             for p in group['params']:
```

### Comparing `pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/nero.py` & `pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/nero.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,38 +16,31 @@
     :param constraints: bool.
     :param eps: float. term added to the denominator to improve numerical stability.
     """
 
     def __init__(
         self, params: PARAMETERS, lr: float = 0.01, beta: float = 0.999, constraints: bool = True, eps: float = 1e-8
     ):
-        self.lr = lr
-        self.beta = beta
-        self.eps = eps
+        self.validate_learning_rate(lr)
+        self.validate_range(beta, 'beta', 0.0, 1.0, range_type='[]')
+        self.validate_non_negative(eps, 'eps')
 
-        self.validate_parameters()
-
-        defaults: DEFAULTS = {'lr': lr, 'constraints': constraints}
+        defaults: DEFAULTS = {'lr': lr, 'beta': beta, 'constraints': constraints, 'eps': eps}
         super().__init__(params, defaults)
 
-    def validate_parameters(self):
-        self.validate_learning_rate(self.lr)
-        self.validate_beta(self.beta)
-        self.validate_epsilon(self.eps)
-
     def __str__(self) -> str:
         return 'Nero'
 
     @torch.no_grad()
     def reset(self):
         for group in self.param_groups:
             for p in group['params']:
                 if group['constraints'] and p.dim() > 1:
                     p.sub_(neuron_mean(p))
-                    p.div_(neuron_norm(p) + self.eps)
+                    p.div_(neuron_norm(p) + group['eps'])
 
                 state = self.state[p]
 
                 state['step'] = 0
                 state['exp_avg_sq'] = torch.zeros_like(neuron_norm(p))
                 state['scale'] = neuron_norm(p).mean()
 
@@ -70,34 +63,34 @@
                 if grad.is_sparse:
                     raise NoSparseGradientError(str(self))
 
                 state = self.state[p]
                 if len(state) == 0:
                     if group['constraints'] and p.dim() > 1:
                         p.sub_(neuron_mean(p))
-                        p.div_(neuron_norm(p) + self.eps)
+                        p.div_(neuron_norm(p) + group['eps'])
 
                     state['step'] = 0
                     state['exp_avg_sq'] = torch.zeros_like(neuron_norm(p))
                     state['scale'] = neuron_norm(p).mean()
                     if state['scale'] == 0.0:
                         state['scale'] = 0.01
 
                 state['step'] += 1
 
                 grad_norm = neuron_norm(grad)
 
                 exp_avg_sq = state['exp_avg_sq']
-                exp_avg_sq.mul_(self.beta).addcmul_(grad_norm, grad_norm, value=1.0 - self.beta)
+                exp_avg_sq.mul_(group['beta']).addcmul_(grad_norm, grad_norm, value=1.0 - group['beta'])
 
-                bias_correction: float = 1.0 - self.beta ** state['step']
+                bias_correction: float = 1.0 - group['beta'] ** state['step']
 
-                grad_normed = grad / ((exp_avg_sq / bias_correction).sqrt() + self.eps)
+                grad_normed = grad / ((exp_avg_sq / bias_correction).sqrt_().add_(group['eps']))
                 torch.nan_to_num(grad_normed, nan=0.0, out=grad_normed)
 
-                p.sub_(group['lr'] * state['scale'] * grad_normed)
+                p.sub_(grad_normed, alpha=group['lr'] * state['scale'])
 
                 if group['constraints'] and p.dim() > 1:
                     p.sub_(neuron_mean(p))
-                    p.div_(neuron_norm(p) + self.eps)
+                    p.div_(neuron_norm(p) + group['eps'])
 
         return loss
```

### Comparing `pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/novograd.py` & `pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/novograd.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,66 +11,64 @@
 class NovoGrad(Optimizer, BaseOptimizer):
     r"""Stochastic Gradient Methods with Layer-wise Adaptive Moments for Training of Deep Networks.
 
     :param params: PARAMETERS. iterable of parameters to optimize or dicts defining parameter groups.
     :param lr: float. learning rate.
     :param betas: BETAS. coefficients used for computing running averages of gradient and the squared hessian trace.
     :param weight_decay: float. weight decay (L2 penalty).
+    :param weight_decouple: bool. the optimizer uses decoupled weight decay as in AdamW.
+    :param fixed_decay: bool. fix weight decay.
     :param grad_averaging: bool. multiply ck (1 - momentum).
     :param adam_debias: bool. Only correct the denominator to avoid inflating step sizes early in training.
     :param eps: float. term added to the denominator to improve numerical stability.
     """
 
     def __init__(
         self,
         params: PARAMETERS,
         lr: float = 1e-3,
         betas: BETAS = (0.95, 0.98),
         weight_decay: float = 0.0,
+        weight_decouple: bool = False,
+        fixed_decay: bool = False,
         grad_averaging: bool = False,
         adam_debias: bool = False,
         eps: float = 1e-8,
     ):
-        self.lr = lr
-        self.betas = betas
-        self.weight_decay = weight_decay
-        self.eps = eps
-
-        self.validate_parameters()
+        self.validate_learning_rate(lr)
+        self.validate_betas(betas)
+        self.validate_non_negative(weight_decay, 'weight_decay')
+        self.validate_non_negative(eps, 'eps')
 
         defaults: DEFAULTS = {
             'lr': lr,
             'betas': betas,
             'weight_decay': weight_decay,
+            'weight_decouple': weight_decouple,
+            'fixed_decay': fixed_decay,
             'grad_averaging': grad_averaging,
             'adam_debias': adam_debias,
             'eps': eps,
         }
         super().__init__(params, defaults)
 
-    def validate_parameters(self):
-        self.validate_learning_rate(self.lr)
-        self.validate_betas(self.betas)
-        self.validate_weight_decay(self.weight_decay)
-        self.validate_epsilon(self.eps)
-
     def __str__(self) -> str:
         return 'NovoGrad'
 
     @torch.no_grad()
     def reset(self):
         for group in self.param_groups:
             group['step'] = 0
             for p in group['params']:
                 state = self.state[p]
 
                 grad = p.grad
-                g_2 = grad ** 2  # fmt: skip
 
-                state['step'] = 0
+                g_2 = grad.pow(2).sum()  # fmt: skip
+
                 state['moments'] = grad.div(g_2.sqrt() + group['eps']) + group['weight_decay'] * p
                 state['grads_ema'] = g_2
 
     @torch.no_grad()
     def step(self, closure: CLOSURE = None) -> LOSS:
         loss: LOSS = None
         if closure is not None:
@@ -80,49 +78,55 @@
         for group in self.param_groups:
             if 'step' in group:
                 group['step'] += 1
             else:
                 group['step'] = 1
 
             beta1, beta2 = group['betas']
-            weight_decay = group['weight_decay']
 
-            bias_correction1 = 1.0 - beta1 ** group['step']
-            bias_correction2_sq = math.sqrt(1.0 - beta2 ** group['step'])
+            bias_correction1: float = 1.0 - beta1 ** group['step']
+            bias_correction2_sq: float = math.sqrt(1.0 - beta2 ** group['step'])
 
             step_size: float = group['lr'] * bias_correction2_sq
             if not group['adam_debias']:
                 step_size /= bias_correction1
 
             for p in group['params']:
                 if p.grad is None:
                     continue
 
                 grad = p.grad
                 if grad.is_sparse:
                     raise NoSparseGradientError(str(self))
 
                 state = self.state[p]
-                g_2 = grad ** 2  # fmt: skip
 
-                if len(state) == 0:
-                    state['moments'] = grad.div(g_2.sqrt() + group['eps']) + weight_decay * p
-                    state['grads_ema'] = g_2
+                grad_p2 = grad.pow(2).sum()
 
-                moments, grads_ema = state['moments'], state['grads_ema']
+                if len(state) == 0:
+                    state['moments'] = grad.div(grad_p2.sqrt() + group['eps']) + group['weight_decay'] * p
+                    state['grads_ema'] = grad_p2
 
-                grads_ema.mul_(beta2).add_(g_2, alpha=1.0 - beta2)
+                grads_ema = state['grads_ema']
+                grads_ema.mul_(beta2).add_(grad_p2, alpha=1.0 - beta2)
 
                 de_nom = grads_ema.sqrt().add_(group['eps'])
                 grad.div_(de_nom)
 
-                if weight_decay > 0.0:
-                    grad.add_(p, alpha=weight_decay)
+                self.apply_weight_decay(
+                    p=p,
+                    grad=p.grad,
+                    lr=group['lr'],
+                    weight_decay=group['weight_decay'],
+                    weight_decouple=group['weight_decouple'],
+                    fixed_decay=group['fixed_decay'],
+                )
 
                 if group['grad_averaging']:
                     grad.mul_(1.0 - beta1)
 
+                moments = state['moments']
                 moments.mul_(beta1).add_(grad)
 
                 p.add_(moments, alpha=-step_size)
 
         return loss
```

### Comparing `pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/pcgrad.py` & `pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/pcgrad.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,22 +14,19 @@
     r"""Gradient Surgery for Multi-Task Learning.
 
     :param optimizer: OPTIMIZER: optimizer instance.
     :param reduction: str. reduction method.
     """
 
     def __init__(self, optimizer: OPTIMIZER, reduction: str = 'mean'):
+        self.validate_reduction(reduction)
+
         self.optimizer = optimizer
         self.reduction = reduction
 
-        self.validate_parameters()
-
-    def validate_parameters(self):
-        self.validate_reduction(self.reduction)
-
     @torch.no_grad()
     def reset(self):
         self.zero_grad()
 
     def zero_grad(self):
         return self.optimizer.zero_grad(set_to_none=True)
 
@@ -92,15 +89,15 @@
         for i, g_i in enumerate(pc_grad):
             random.shuffle(grads)
             for g_j in grads:
                 g_i_g_j: torch.Tensor = torch.dot(g_i, g_j)
                 if g_i_g_j < 0:
                     pc_grad[i] -= g_i_g_j * g_j / (g_j.norm() ** 2)
 
-        merged_grad: torch.Tensor = torch.zeros_like(grads[0], device=grads[0].device)
+        merged_grad: torch.Tensor = torch.zeros_like(grads[0])
 
         shared_pc_gradients: torch.Tensor = torch.stack([g[shared] for g in pc_grad])
         if self.reduction == 'mean':
             merged_grad[shared] = shared_pc_gradients.mean(dim=0)
         else:
             merged_grad[shared] = shared_pc_gradients.sum(dim=0)
```

### Comparing `pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/pid.py` & `pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/adadelta.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,120 +2,105 @@
 from torch.optim.optimizer import Optimizer
 
 from pytorch_optimizer.base.exception import NoSparseGradientError
 from pytorch_optimizer.base.optimizer import BaseOptimizer
 from pytorch_optimizer.base.types import CLOSURE, DEFAULTS, LOSS, PARAMETERS
 
 
-class PID(Optimizer, BaseOptimizer):
-    r"""A PID Controller Approach for Stochastic Optimization of Deep Networks.
+class AdaDelta(Optimizer, BaseOptimizer):
+    r"""An Adaptive Learning Rate Method.
 
     :param params: PARAMETERS. iterable of parameters to optimize or dicts defining parameter groups.
     :param lr: float. learning rate.
-    :param momentum: float. momentum factor.
-    :param dampening: float. dampening for momentum.
-    :param derivative: float. D part of the PID.
-    :param integral: float. I part of the PID.
+    :param rho: float. coefficient used for computing a running average of squared gradients.
     :param weight_decay: float. weight decay (L2 penalty).
     :param weight_decouple: bool. the optimizer uses decoupled weight decay as in AdamW.
+    :param fixed_decay: bool. fix weight decay.
+    :param eps: float. term added to the denominator to improve numerical stability.
     """
 
     def __init__(
         self,
         params: PARAMETERS,
-        lr: float = 1e-3,
-        momentum: float = 0.0,
-        dampening: float = 0.0,
-        derivative: float = 10.0,
-        integral: float = 5.0,
+        lr: float = 1.0,
+        rho: float = 0.9,
         weight_decay: float = 0.0,
         weight_decouple: bool = False,
+        fixed_decay: bool = False,
+        eps: float = 1e-6,
     ):
-        self.lr = lr
-        self.momentum = momentum
-        self.dampening = dampening
-        self.derivative = derivative
-        self.integral = integral
-        self.weight_decay = weight_decay
-
-        self.validate_parameters()
+        self.validate_learning_rate(lr)
+        self.validate_range(rho, 'rho', 0.0, 1.0)
+        self.validate_non_negative(weight_decay, 'weight_decay')
+        self.validate_non_negative(eps, 'eps')
 
         defaults: DEFAULTS = {
             'lr': lr,
-            'momentum': momentum,
-            'dampening': dampening,
-            'derivative': derivative,
-            'integral': integral,
+            'rho': rho,
             'weight_decay': weight_decay,
             'weight_decouple': weight_decouple,
+            'fixed_decay': fixed_decay,
+            'eps': eps,
         }
         super().__init__(params, defaults)
 
-    def validate_parameters(self):
-        self.validate_learning_rate(self.lr)
-        self.validate_momentum(self.momentum)
-        self.validate_weight_decay(self.weight_decay)
-
     def __str__(self) -> str:
-        return 'PID'
+        return 'AdaDelta'
 
     @torch.no_grad()
     def reset(self):
         for group in self.param_groups:
             group['step'] = 0
             for p in group['params']:
                 state = self.state[p]
 
-                if group['momentum'] > 0.0:
-                    state['grad_buffer'] = torch.zeros_like(p)
-                    state['i_buffer'] = torch.zeros_like(p)
-                    state['d_buffer'] = torch.zeros_like(p)
+                state['square_avg'] = torch.zeros_like(p)
+                state['acc_delta'] = torch.zeros_like(p)
 
     @torch.no_grad()
     def step(self, closure: CLOSURE = None) -> LOSS:
         loss: LOSS = None
         if closure is not None:
             with torch.enable_grad():
                 loss = closure()
 
         for group in self.param_groups:
             if 'step' in group:
                 group['step'] += 1
             else:
                 group['step'] = 1
 
+            rho: float = group['rho']
+
             for p in group['params']:
                 if p.grad is None:
                     continue
 
                 grad = p.grad
                 if grad.is_sparse:
                     raise NoSparseGradientError(str(self))
 
                 state = self.state[p]
 
-                if len(state) == 0 and group['momentum'] > 0.0:
-                    state['grad_buffer'] = torch.zeros_like(p)
-                    state['i_buffer'] = torch.zeros_like(p)
-                    state['d_buffer'] = torch.zeros_like(p)
-
-                if group['weight_decouple']:
-                    p.mul_(1.0 - group['weight_decay'] * group['lr'])
-                elif group['weight_decay'] > 0.0:
-                    grad.add_(p, alpha=group['weight_decay'])
-
-                if group['momentum'] > 0.0:
-                    i_buf = state['i_buffer']
-                    i_buf.mul_(group['momentum']).add_(grad, alpha=1.0 - group['dampening'])
-
-                    g_buf, d_buf = state['grad_buffer'], state['d_buffer']
-                    d_buf.mul_(group['momentum'])
-
-                    if group['step'] > 1:
-                        d_buf.add_(grad - g_buf, alpha=1.0 - group['momentum'])
-                        g_buf.copy_(grad)
+                if len(state) == 0:
+                    state['square_avg'] = torch.zeros_like(p)
+                    state['acc_delta'] = torch.zeros_like(p)
+
+                self.apply_weight_decay(
+                    p=p,
+                    grad=grad,
+                    lr=group['lr'],
+                    weight_decay=group['weight_decay'],
+                    weight_decouple=group['weight_decouple'],
+                    fixed_decay=group['fixed_decay'],
+                )
+
+                square_avg, acc_delta = state['square_avg'], state['acc_delta']
+                square_avg.mul_(rho).addcmul_(grad, grad, value=1.0 - rho)
 
-                    grad.add_(i_buf, alpha=group['integral']).add_(d_buf, alpha=group['derivative'])
+                std = square_avg.add(group['eps']).sqrt_()
+                delta = acc_delta.add(group['eps']).sqrt_().div_(std).mul_(grad)
 
-                p.add_(grad, alpha=-group['lr'])
+                acc_delta.mul_(rho).addcmul_(delta, delta, value=1.0 - rho)
+                p.add_(delta, alpha=-group['lr'])
 
         return loss
```

### Comparing `pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/pnm.py` & `pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/pnm.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,95 +12,98 @@
     r"""Positive-Negative Momentum Optimizers.
 
     :param params: PARAMETERS. iterable of parameters to optimize or dicts defining parameter groups.
     :param lr: float. learning rate.
     :param betas: BETAS. coefficients used for computing running averages of gradient and the squared hessian trace.
     :param weight_decay: float. weight decay (L2 penalty).
     :param weight_decouple: bool. use weight_decouple.
+    :param fixed_decay: bool. fix weight decay.
     :param eps: float. term added to the denominator to improve numerical stability.
     """
 
     def __init__(
         self,
         params: PARAMETERS,
         lr: float = 1e-3,
         betas: BETAS = (0.9, 1.0),
         weight_decay: float = 0.0,
         weight_decouple: bool = True,
+        fixed_decay: bool = False,
         eps: float = 1e-8,
     ):
-        self.lr = lr
-        self.betas = betas
-        self.weight_decay = weight_decay
-        self.eps = eps
-
-        self.validate_parameters()
+        self.validate_learning_rate(lr)
+        self.validate_betas(betas)
+        self.validate_non_negative(weight_decay, 'weight_decay')
+        self.validate_non_negative(eps, 'eps')
 
         defaults: DEFAULTS = {
             'lr': lr,
             'betas': betas,
             'weight_decay': weight_decay,
             'weight_decouple': weight_decouple,
+            'fixed_decay': fixed_decay,
         }
         super().__init__(params, defaults)
 
-    def validate_parameters(self):
-        self.validate_learning_rate(self.lr)
-        self.validate_betas(self.betas)
-        self.validate_weight_decay(self.weight_decay)
-        self.validate_epsilon(self.eps)
-
     def __str__(self) -> str:
         return 'PNM'
 
     @torch.no_grad()
     def reset(self):
         for group in self.param_groups:
+            group['step'] = 0
             for p in group['params']:
                 state = self.state[p]
 
-                state['step'] = 0
                 state['pos_momentum'] = torch.zeros_like(p)
                 state['neg_momentum'] = torch.zeros_like(p)
 
     @torch.no_grad()
     def step(self, closure: CLOSURE = None) -> LOSS:
         loss: LOSS = None
         if closure is not None:
             with torch.enable_grad():
                 loss = closure()
 
         for group in self.param_groups:
+            if 'step' in group:
+                group['step'] += 1
+            else:
+                group['step'] = 1
+
             beta1, beta2 = group['betas']
-            noise_norm = math.sqrt((1 + beta2) ** 2 + beta2 ** 2)  # fmt: skip
+
+            noise_norm: float = math.sqrt((1 + beta2) ** 2 + beta2 ** 2)  # fmt: skip
+
             for p in group['params']:
                 if p.grad is None:
                     continue
 
                 grad = p.grad
                 if grad.is_sparse:
                     raise NoSparseGradientError(str(self))
 
-                if group['weight_decouple']:
-                    p.mul_(1.0 - group['lr'] * group['weight_decay'])
-                else:
-                    grad.add_(p, alpha=group['weight_decay'])
-
                 state = self.state[p]
                 if len(state) == 0:
-                    state['step'] = 0
                     state['pos_momentum'] = torch.zeros_like(p)
                     state['neg_momentum'] = torch.zeros_like(p)
 
-                state['step'] += 1
+                self.apply_weight_decay(
+                    p=p,
+                    grad=p.grad,
+                    lr=group['lr'],
+                    weight_decay=group['weight_decay'],
+                    weight_decouple=group['weight_decouple'],
+                    fixed_decay=group['fixed_decay'],
+                )
 
-                if state['step'] % 2 == 1:
+                if group['step'] % 2 == 1:
                     pos_momentum, neg_momentum = state['pos_momentum'], state['neg_momentum']
                 else:
                     neg_momentum, pos_momentum = state['pos_momentum'], state['neg_momentum']
 
                 pos_momentum.mul_(beta1 ** 2).add_(grad, alpha=1.0 - beta1 ** 2)  # fmt: skip
-                delta_p = pos_momentum.mul(1 + beta2).add(neg_momentum, alpha=-beta2).mul(1.0 / noise_norm)
 
+                delta_p = pos_momentum.mul(1 + beta2).add_(neg_momentum, alpha=-beta2).mul_(1.0 / noise_norm)
                 p.add_(delta_p, alpha=-group['lr'])
 
         return loss
```

### Comparing `pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/qhadam.py` & `pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/qhadam.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,52 +13,46 @@
 
     :param params: PARAMETERS. iterable of parameters to optimize or dicts defining parameter groups.
     :param lr: float. learning rate.
     :param betas: BETAS. coefficients used for computing running averages of gradient and the squared hessian trace.
     :param nus: Tuple[float, float]. immediate discount factors used to estimate the gradient and its square.
     :param weight_decay: float. weight decay (L2 penalty).
     :param weight_decouple: bool. the optimizer uses decoupled weight decay as in AdamW.
+    :param fixed_decay: bool. fix weight decay.
     :param eps: float. term added to the denominator to improve numerical stability.
     """
 
     def __init__(
         self,
         params: PARAMETERS,
         lr: float = 1e-3,
         betas: BETAS = (0.9, 0.999),
         nus: Tuple[float, float] = (1.0, 1.0),
         weight_decay: float = 0.0,
         weight_decouple: bool = False,
+        fixed_decay: bool = False,
         eps: float = 1e-8,
     ):
-        self.lr = lr
-        self.betas = betas
-        self.nus = nus
-        self.weight_decay = weight_decay
-        self.eps = eps
-
-        self.validate_parameters()
+        self.validate_learning_rate(lr)
+        self.validate_betas(betas)
+        self.validate_nus(nus)
+        self.validate_non_negative(weight_decay, 'weight_decay')
+        self.validate_non_negative(eps, 'eps')
 
         defaults: DEFAULTS = {
             'lr': lr,
             'betas': betas,
             'nus': nus,
             'weight_decay': weight_decay,
             'weight_decouple': weight_decouple,
+            'fixed_decay': fixed_decay,
             'eps': eps,
         }
         super().__init__(params, defaults)
 
-    def validate_parameters(self):
-        self.validate_learning_rate(self.lr)
-        self.validate_betas(self.betas)
-        self.validate_weight_decay(self.weight_decay)
-        self.validate_epsilon(self.eps)
-        self.validate_nus(self.nus)
-
     def __str__(self) -> str:
         return 'QHAdam'
 
     @torch.no_grad()
     def reset(self):
         for group in self.param_groups:
             group['step'] = 0
@@ -98,18 +92,22 @@
 
                 if len(state) == 0:
                     state['beta1_weight'] = torch.zeros((1,), dtype=grad.dtype, device=grad.device)
                     state['beta2_weight'] = torch.zeros((1,), dtype=grad.dtype, device=grad.device)
                     state['exp_avg'] = torch.zeros_like(p)
                     state['exp_avg_sq'] = torch.zeros_like(p)
 
-                if group['weight_decouple']:
-                    p.mul_(1.0 - group['weight_decay'] * group['lr'])
-                elif group['weight_decay'] > 0.0:
-                    grad.add_(p, alpha=group['weight_decay'])
+                self.apply_weight_decay(
+                    p=p,
+                    grad=p.grad,
+                    lr=group['lr'],
+                    weight_decay=group['weight_decay'],
+                    weight_decouple=group['weight_decouple'],
+                    fixed_decay=group['fixed_decay'],
+                )
 
                 beta1_weight, beta2_weight = state['beta1_weight'], state['beta2_weight']
                 beta1_weight.mul_(beta1).add_(1.0)
                 beta2_weight.mul_(beta2).add_(1.0)
 
                 beta1_adj = 1.0 - (1.0 / beta1_weight)
                 beta2_adj = 1.0 - (1.0 / beta2_weight)
```

### Comparing `pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/qhm.py` & `pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/pid.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,68 +2,72 @@
 from torch.optim.optimizer import Optimizer
 
 from pytorch_optimizer.base.exception import NoSparseGradientError
 from pytorch_optimizer.base.optimizer import BaseOptimizer
 from pytorch_optimizer.base.types import CLOSURE, DEFAULTS, LOSS, PARAMETERS
 
 
-class QHM(Optimizer, BaseOptimizer):
-    r"""Quasi-hyperbolic momentum (QHM) optimization algorithm.
+class PID(Optimizer, BaseOptimizer):
+    r"""A PID Controller Approach for Stochastic Optimization of Deep Networks.
 
     :param params: PARAMETERS. iterable of parameters to optimize or dicts defining parameter groups.
     :param lr: float. learning rate.
     :param momentum: float. momentum factor.
-    :param nu: float. immediate discount factor used to estimate the gradient and its square.
+    :param dampening: float. dampening for momentum.
+    :param derivative: float. D part of the PID.
+    :param integral: float. I part of the PID.
     :param weight_decay: float. weight decay (L2 penalty).
     :param weight_decouple: bool. the optimizer uses decoupled weight decay as in AdamW.
-    :param eps: float. term added to the denominator to improve numerical stability.
+    :param fixed_decay: bool. fix weight decay.
     """
 
     def __init__(
         self,
         params: PARAMETERS,
         lr: float = 1e-3,
         momentum: float = 0.0,
-        nu: float = 1.0,
+        dampening: float = 0.0,
+        derivative: float = 10.0,
+        integral: float = 5.0,
         weight_decay: float = 0.0,
         weight_decouple: bool = False,
+        fixed_decay: bool = False,
     ):
-        self.lr = lr
-        self.momentum = momentum
-        self.nu = nu
-        self.weight_decay = weight_decay
-
-        self.validate_parameters()
+        self.validate_learning_rate(lr)
+        self.validate_range(momentum, 'momentum', 0.0, 1.0)
+        self.validate_non_negative(derivative, 'derivative')
+        self.validate_non_negative(integral, 'integral')
+        self.validate_non_negative(weight_decay, 'weight_decay')
 
         defaults: DEFAULTS = {
             'lr': lr,
             'momentum': momentum,
-            'nu': nu,
+            'dampening': dampening,
+            'derivative': derivative,
+            'integral': integral,
             'weight_decay': weight_decay,
             'weight_decouple': weight_decouple,
+            'fixed_decay': fixed_decay,
         }
         super().__init__(params, defaults)
 
-    def validate_parameters(self):
-        self.validate_learning_rate(self.lr)
-        self.validate_momentum(self.momentum)
-        self.validate_weight_decay(self.weight_decay)
-        self.validate_nus(self.nu)
-
     def __str__(self) -> str:
-        return 'QHM'
+        return 'PID'
 
     @torch.no_grad()
     def reset(self):
         for group in self.param_groups:
             group['step'] = 0
             for p in group['params']:
                 state = self.state[p]
 
-                state['momentum_buffer'] = torch.zeros_like(p)
+                if group['momentum'] > 0.0:
+                    state['grad_buffer'] = torch.zeros_like(p)
+                    state['i_buffer'] = torch.zeros_like(p)
+                    state['d_buffer'] = torch.zeros_like(p)
 
     @torch.no_grad()
     def step(self, closure: CLOSURE = None) -> LOSS:
         loss: LOSS = None
         if closure is not None:
             with torch.enable_grad():
                 loss = closure()
@@ -80,22 +84,37 @@
 
                 grad = p.grad
                 if grad.is_sparse:
                     raise NoSparseGradientError(str(self))
 
                 state = self.state[p]
 
-                if len(state) == 0:
-                    state['momentum_buffer'] = torch.zeros_like(p)
-
-                if group['weight_decouple']:
-                    p.mul_(1.0 - group['weight_decay'] * group['lr'])
-                elif group['weight_decay'] > 0.0:
-                    grad.add_(p, alpha=group['weight_decay'])
+                if len(state) == 0 and group['momentum'] > 0.0:
+                    state['grad_buffer'] = torch.zeros_like(p)
+                    state['i_buffer'] = torch.zeros_like(p)
+                    state['d_buffer'] = torch.zeros_like(p)
+
+                self.apply_weight_decay(
+                    p=p,
+                    grad=p.grad,
+                    lr=group['lr'],
+                    weight_decay=group['weight_decay'],
+                    weight_decouple=group['weight_decouple'],
+                    fixed_decay=group['fixed_decay'],
+                )
+
+                if group['momentum'] > 0.0:
+                    i_buf = state['i_buffer']
+                    i_buf.mul_(group['momentum']).add_(grad, alpha=1.0 - group['dampening'])
+
+                    g_buf, d_buf = state['grad_buffer'], state['d_buffer']
+                    d_buf.mul_(group['momentum'])
+
+                    if group['step'] > 1:
+                        d_buf.add_(grad - g_buf, alpha=1.0 - group['momentum'])
+                        g_buf.copy_(grad)
 
-                buf = state['momentum_buffer']
-                buf.mul_(group['momentum']).add_(grad, alpha=1.0 - group['momentum'])
+                    grad.add_(i_buf, alpha=group['integral']).add_(d_buf, alpha=group['derivative'])
 
-                p.add_(buf, alpha=-group['lr'] * group['nu'])
-                p.add_(grad, alpha=-group['lr'] * (1.0 - group['nu']))
+                p.add_(grad, alpha=-group['lr'])
 
         return loss
```

### Comparing `pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/radam.py` & `pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/ranger.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,85 +1,97 @@
-import math
-
 import torch
 from torch.optim.optimizer import Optimizer
 
 from pytorch_optimizer.base.exception import NoSparseGradientError
 from pytorch_optimizer.base.optimizer import BaseOptimizer
 from pytorch_optimizer.base.types import BETAS, CLOSURE, DEFAULTS, LOSS, PARAMETERS
+from pytorch_optimizer.optimizer.gc import centralize_gradient
 
 
-class RAdam(Optimizer, BaseOptimizer):
-    r"""Rectified Adam.
+class Ranger(Optimizer, BaseOptimizer):
+    r"""a synergistic optimizer combining RAdam and LookAhead, and now GC in one optimizer.
 
     :param params: PARAMETERS. iterable of parameters to optimize or dicts defining parameter groups.
     :param lr: float. learning rate.
     :param betas: BETAS. coefficients used for computing running averages of gradient and the squared hessian trace.
     :param weight_decay: float. weight decay (L2 penalty).
+    :param weight_decouple: bool. the optimizer uses decoupled weight decay as in AdamW.
+    :param fixed_decay: bool. fix weight decay.
     :param n_sma_threshold: int. (recommended is 5).
-    :param degenerated_to_sgd: float. degenerated to SGD.
+    :param degenerated_to_sgd: bool. perform SGD update when variance of gradient is high.
+    :param use_gc: bool. use Gradient Centralization (both convolution & fc layers).
+    :param gc_conv_only: bool. use Gradient Centralization (only convolution layer).
     :param r: float. EMA factor. between 0.9 ~ 0.99 is preferred.
     :param adanorm: bool. whether to use the AdaNorm variant.
     :param adam_debias: bool. Only correct the denominator to avoid inflating step sizes early in training.
     :param eps: float. term added to the denominator to improve numerical stability.
     """
 
     def __init__(
         self,
         params: PARAMETERS,
         lr: float = 1e-3,
-        betas: BETAS = (0.9, 0.999),
-        weight_decay: float = 0.0,
+        alpha: float = 0.5,
+        k: int = 6,
         n_sma_threshold: int = 5,
         degenerated_to_sgd: bool = False,
+        betas: BETAS = (0.95, 0.999),
+        eps: float = 1e-5,
+        weight_decay: float = 0.0,
+        weight_decouple: bool = True,
+        fixed_decay: bool = False,
+        use_gc: bool = True,
+        gc_conv_only: bool = False,
         r: float = 0.95,
         adanorm: bool = False,
         adam_debias: bool = False,
-        eps: float = 1e-8,
     ):
-        self.lr = lr
-        self.betas = betas
-        self.weight_decay = weight_decay
+        self.validate_learning_rate(lr)
+        self.validate_betas(betas)
+        self.validate_non_negative(weight_decay, 'weight_decay')
+        self.validate_positive(k, 'k')
+        self.validate_non_negative(eps, 'eps')
+
         self.n_sma_threshold = n_sma_threshold
         self.degenerated_to_sgd = degenerated_to_sgd
-        self.eps = eps
-
-        self.validate_parameters()
+        self.use_gc = use_gc
+        self.gc_gradient_threshold: int = 3 if gc_conv_only else 1
 
         defaults: DEFAULTS = {
             'lr': lr,
             'betas': betas,
+            'alpha': alpha,
+            'k': k,
+            'step_counter': 0,
             'weight_decay': weight_decay,
+            'weight_decouple': weight_decouple,
+            'fixed_decay': fixed_decay,
             'adanorm': adanorm,
             'adam_debias': adam_debias,
             'eps': eps,
         }
         if adanorm:
             defaults.update({'r': r})
 
         super().__init__(params, defaults)
 
-    def validate_parameters(self):
-        self.validate_learning_rate(self.lr)
-        self.validate_betas(self.betas)
-        self.validate_weight_decay(self.weight_decay)
-        self.validate_epsilon(self.eps)
-
     def __str__(self) -> str:
-        return 'RAdam'
+        return 'Ranger'
 
     @torch.no_grad()
     def reset(self):
         for group in self.param_groups:
+            group['step'] = 0
             for p in group['params']:
                 state = self.state[p]
 
-                state['step'] = 0
                 state['exp_avg'] = torch.zeros_like(p)
                 state['exp_avg_sq'] = torch.zeros_like(p)
+                state['slow_buffer'] = torch.empty_like(p)
+                state['slow_buffer'].copy_(p)
                 if group['adanorm']:
                     state['exp_grad_norm'] = torch.zeros((1,), dtype=p.dtype, device=p.device)
 
     @torch.no_grad()
     def step(self, closure: CLOSURE = None) -> LOSS:
         loss: LOSS = None
         if closure is not None:
@@ -89,74 +101,76 @@
         for group in self.param_groups:
             if 'step' in group:
                 group['step'] += 1
             else:
                 group['step'] = 1
 
             beta1, beta2 = group['betas']
+            bias_correction1: float = 1.0 - beta1 ** group['step']
 
-            bias_correction1 = 1.0 - beta1 ** group['step']
-
-            n_sma_max: float = 2.0 / (1.0 - beta2) - 1.0
-            beta2_t: float = beta2 ** group['step']
-            n_sma: float = n_sma_max - 2 * group['step'] * beta2_t / (1.0 - beta2_t)
+            step_size, n_sma = self.get_rectify_step_size(
+                is_rectify=True,
+                step=group['step'],
+                lr=group['lr'],
+                beta2=beta2,
+                n_sma_threshold=self.n_sma_threshold,
+                degenerated_to_sgd=self.degenerated_to_sgd,
+            )
+
+            step_size = self.apply_adam_debias(
+                adam_debias=group['adam_debias'],
+                step_size=step_size,
+                bias_correction1=bias_correction1,
+            )
 
             for p in group['params']:
                 if p.grad is None:
                     continue
 
                 grad = p.grad
                 if grad.is_sparse:
                     raise NoSparseGradientError(str(self))
 
                 state = self.state[p]
-
                 if len(state) == 0:
-                    state['step'] = 0
                     state['exp_avg'] = torch.zeros_like(p)
                     state['exp_avg_sq'] = torch.zeros_like(p)
+                    state['slow_buffer'] = torch.empty_like(p)
+                    state['slow_buffer'].copy_(p)
                     if group['adanorm']:
                         state['exp_grad_norm'] = torch.zeros((1,), dtype=grad.dtype, device=grad.device)
 
-                s_grad = grad
-                if group['adanorm']:
-                    grad_norm = torch.linalg.norm(grad)
-
-                    exp_grad_norm = state['exp_grad_norm']
-                    exp_grad_norm.mul_(group['r']).add_(grad_norm, alpha=1.0 - group['r'])
+                if self.use_gc and grad.dim() > self.gc_gradient_threshold:
+                    grad = centralize_gradient(grad, gc_conv_only=False)
 
-                    if exp_grad_norm > grad_norm:
-                        s_grad *= exp_grad_norm / grad_norm
+                self.apply_weight_decay(
+                    p=p,
+                    grad=None,
+                    lr=group['lr'],
+                    weight_decay=group['weight_decay'],
+                    weight_decouple=group['weight_decouple'],
+                    fixed_decay=group['fixed_decay'],
+                )
+
+                s_grad = self.get_adanorm_gradient(
+                    grad=grad,
+                    adanorm=group['adanorm'],
+                    exp_grad_norm=state.get('exp_grad_norm', None),
+                    r=group.get('r', None),
+                )
 
                 exp_avg, exp_avg_sq = state['exp_avg'], state['exp_avg_sq']
-
                 exp_avg.mul_(beta1).add_(s_grad, alpha=1.0 - beta1)
                 exp_avg_sq.mul_(beta2).addcmul_(grad, grad, value=1.0 - beta2)
 
                 if n_sma >= self.n_sma_threshold:
-                    step_size = math.sqrt(
-                        (1 - beta2_t)
-                        * (n_sma - 4)
-                        / (n_sma_max - 4)
-                        * (n_sma - 2)
-                        / n_sma
-                        * n_sma_max
-                        / (n_sma_max - 2)
-                    )
-                elif self.degenerated_to_sgd:
-                    step_size = 1.0
+                    de_nom = exp_avg_sq.sqrt().add_(group['eps'])
+                    p.addcdiv_(exp_avg, de_nom, value=-step_size)
                 else:
-                    step_size = -1
+                    p.add_(exp_avg, alpha=-step_size)
 
-                if not group['adam_debias']:
-                    step_size /= bias_correction1
-
-                if group['weight_decay'] > 0.0 and (n_sma >= self.n_sma_threshold or step_size > 0):
-                    p.add_(p, alpha=-group['weight_decay'] * group['lr'])
-
-                if n_sma >= self.n_sma_threshold:
-                    de_nom = exp_avg_sq.sqrt().add_(group['eps'])
-                    p.addcdiv_(exp_avg, de_nom, value=-step_size * group['lr'])
-                elif step_size > 0:
-                    p.add_(exp_avg, alpha=-step_size * group['lr'])
+                if group['step'] % group['k'] == 0:
+                    slow_p = state['slow_buffer']
+                    slow_p.add_(p - slow_p, alpha=group['alpha'])
+                    p.copy_(slow_p)
 
         return loss
```

### Comparing `pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/ranger.py` & `pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/radam.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,104 +1,82 @@
-import math
-
 import torch
 from torch.optim.optimizer import Optimizer
 
 from pytorch_optimizer.base.exception import NoSparseGradientError
 from pytorch_optimizer.base.optimizer import BaseOptimizer
 from pytorch_optimizer.base.types import BETAS, CLOSURE, DEFAULTS, LOSS, PARAMETERS
-from pytorch_optimizer.optimizer.gc import centralize_gradient
 
 
-class Ranger(Optimizer, BaseOptimizer):
-    r"""a synergistic optimizer combining RAdam and LookAhead, and now GC in one optimizer.
+class RAdam(Optimizer, BaseOptimizer):
+    r"""Rectified Adam.
 
     :param params: PARAMETERS. iterable of parameters to optimize or dicts defining parameter groups.
     :param lr: float. learning rate.
     :param betas: BETAS. coefficients used for computing running averages of gradient and the squared hessian trace.
     :param weight_decay: float. weight decay (L2 penalty).
+    :param weight_decouple: bool. the optimizer uses decoupled weight decay as in AdamW.
+    :param fixed_decay: bool. fix weight decay.
     :param n_sma_threshold: int. (recommended is 5).
-    :param degenerated_to_sgd: bool. perform SGD update when variance of gradient is high.
-    :param use_gc: bool. use Gradient Centralization (both convolution & fc layers).
-    :param gc_conv_only: bool. use Gradient Centralization (only convolution layer).
+    :param degenerated_to_sgd: float. degenerated to SGD.
     :param r: float. EMA factor. between 0.9 ~ 0.99 is preferred.
     :param adanorm: bool. whether to use the AdaNorm variant.
     :param adam_debias: bool. Only correct the denominator to avoid inflating step sizes early in training.
     :param eps: float. term added to the denominator to improve numerical stability.
     """
 
     def __init__(
         self,
         params: PARAMETERS,
         lr: float = 1e-3,
-        alpha: float = 0.5,
-        k: int = 6,
+        betas: BETAS = (0.9, 0.999),
+        weight_decay: float = 0.0,
+        weight_decouple: bool = True,
+        fixed_decay: bool = False,
         n_sma_threshold: int = 5,
         degenerated_to_sgd: bool = False,
-        betas: BETAS = (0.95, 0.999),
-        eps: float = 1e-5,
-        weight_decay: float = 0.0,
-        use_gc: bool = True,
-        gc_conv_only: bool = False,
         r: float = 0.95,
         adanorm: bool = False,
         adam_debias: bool = False,
+        eps: float = 1e-8,
     ):
-        self.lr = lr
-        self.alpha = alpha
-        self.k = k
+        self.validate_learning_rate(lr)
+        self.validate_betas(betas)
+        self.validate_non_negative(weight_decay, 'weight_decay')
+        self.validate_non_negative(eps, 'eps')
+
         self.n_sma_threshold = n_sma_threshold
         self.degenerated_to_sgd = degenerated_to_sgd
-        self.betas = betas
-        self.weight_decay = weight_decay
-        self.use_gc = use_gc
-        self.eps = eps
-
-        self.gc_gradient_threshold: int = 3 if gc_conv_only else 1
-
-        self.validate_parameters()
 
         defaults: DEFAULTS = {
             'lr': lr,
             'betas': betas,
-            'alpha': alpha,
-            'k': k,
-            'step_counter': 0,
-            'n_sma_threshold': n_sma_threshold,
             'weight_decay': weight_decay,
+            'weight_decouple': weight_decouple,
+            'fixed_decay': fixed_decay,
             'adanorm': adanorm,
             'adam_debias': adam_debias,
             'eps': eps,
         }
         if adanorm:
             defaults.update({'r': r})
 
         super().__init__(params, defaults)
 
-    def validate_parameters(self):
-        self.validate_learning_rate(self.lr)
-        self.validate_betas(self.betas)
-        self.validate_weight_decay(self.weight_decay)
-        self.validate_lookahead_k(self.k)
-        self.validate_epsilon(self.eps)
-
     def __str__(self) -> str:
-        return 'Ranger'
+        return 'RAdam'
 
     @torch.no_grad()
     def reset(self):
         for group in self.param_groups:
             group['step'] = 0
             for p in group['params']:
                 state = self.state[p]
 
                 state['exp_avg'] = torch.zeros_like(p)
                 state['exp_avg_sq'] = torch.zeros_like(p)
-                state['slow_buffer'] = torch.empty_like(p)
-                state['slow_buffer'].copy_(p)
                 if group['adanorm']:
                     state['exp_grad_norm'] = torch.zeros((1,), dtype=p.dtype, device=p.device)
 
     @torch.no_grad()
     def step(self, closure: CLOSURE = None) -> LOSS:
         loss: LOSS = None
         if closure is not None:
@@ -109,81 +87,68 @@
             if 'step' in group:
                 group['step'] += 1
             else:
                 group['step'] = 1
 
             beta1, beta2 = group['betas']
 
-            bias_correction1 = 1.0 - beta1 ** group['step']
+            bias_correction1: float = 1.0 - beta1 ** group['step']
 
-            n_sma_max: float = 2.0 / (1.0 - beta2) - 1.0
-            beta2_t: float = beta2 ** group['step']
-            n_sma: float = n_sma_max - 2 * group['step'] * beta2_t / (1.0 - beta2_t)
+            step_size, n_sma = self.get_rectify_step_size(
+                is_rectify=True,
+                step=group['step'],
+                lr=group['lr'],
+                beta2=beta2,
+                n_sma_threshold=self.n_sma_threshold,
+                degenerated_to_sgd=self.degenerated_to_sgd,
+            )
+
+            step_size = self.apply_adam_debias(
+                adam_debias=group['adam_debias'],
+                step_size=step_size,
+                bias_correction1=bias_correction1,
+            )
 
             for p in group['params']:
                 if p.grad is None:
                     continue
 
                 grad = p.grad
                 if grad.is_sparse:
                     raise NoSparseGradientError(str(self))
 
                 state = self.state[p]
+
                 if len(state) == 0:
                     state['exp_avg'] = torch.zeros_like(p)
                     state['exp_avg_sq'] = torch.zeros_like(p)
-                    state['slow_buffer'] = torch.empty_like(p)
-                    state['slow_buffer'].copy_(p)
                     if group['adanorm']:
                         state['exp_grad_norm'] = torch.zeros((1,), dtype=grad.dtype, device=grad.device)
 
-                exp_avg, exp_avg_sq = state['exp_avg'], state['exp_avg_sq']
-
-                if self.use_gc and grad.dim() > self.gc_gradient_threshold:
-                    grad = centralize_gradient(grad, gc_conv_only=False)
-
-                s_grad = grad
-                if group['adanorm']:
-                    grad_norm = torch.linalg.norm(grad)
-
-                    exp_grad_norm = state['exp_grad_norm']
-                    exp_grad_norm.mul_(group['r']).add_(grad_norm, alpha=1.0 - group['r'])
+                if step_size > 0 or n_sma >= self.n_sma_threshold:
+                    self.apply_weight_decay(
+                        p=p,
+                        grad=None,
+                        lr=group['lr'],
+                        weight_decay=group['weight_decay'],
+                        weight_decouple=group['weight_decouple'],
+                        fixed_decay=group['fixed_decay'],
+                    )
 
-                    if exp_grad_norm > grad_norm:
-                        s_grad *= exp_grad_norm / grad_norm
+                s_grad = self.get_adanorm_gradient(
+                    grad=grad,
+                    adanorm=group['adanorm'],
+                    exp_grad_norm=state.get('exp_grad_norm', None),
+                    r=group.get('r', None),
+                )
 
+                exp_avg, exp_avg_sq = state['exp_avg'], state['exp_avg_sq']
                 exp_avg.mul_(beta1).add_(s_grad, alpha=1.0 - beta1)
                 exp_avg_sq.mul_(beta2).addcmul_(grad, grad, value=1.0 - beta2)
 
                 if n_sma >= self.n_sma_threshold:
-                    step_size = math.sqrt(
-                        (1 - beta2_t)
-                        * (n_sma - 4)
-                        / (n_sma_max - 4)
-                        * (n_sma - 2)
-                        / n_sma
-                        * n_sma_max
-                        / (n_sma_max - 2)
-                    )
-                elif self.degenerated_to_sgd:
-                    step_size = 1.0
-                else:
-                    step_size = -1
-
-                if not group['adam_debias']:
-                    step_size /= bias_correction1
-
-                if group['weight_decay'] > 0.0:
-                    p.add_(p, alpha=-group['weight_decay'] * group['lr'])
-
-                if n_sma >= self.n_sma_threshold:
                     de_nom = exp_avg_sq.sqrt().add_(group['eps'])
-                    p.addcdiv_(exp_avg, de_nom, value=-step_size * group['lr'])
-                else:
-                    p.add_(exp_avg, alpha=-step_size * group['lr'])
-
-                if group['step'] % group['k'] == 0:
-                    slow_p = state['slow_buffer']
-                    slow_p.add_(p - slow_p, alpha=self.alpha)
-                    p.copy_(slow_p)
+                    p.addcdiv_(exp_avg, de_nom, value=-step_size)
+                elif step_size > 0:
+                    p.add_(exp_avg, alpha=-step_size)
 
         return loss
```

### Comparing `pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/ranger21.py` & `pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/ranger21.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,14 +40,16 @@
     :param agc_clipping_value: float.
     :param agc_eps: float. eps for AGC
     :param centralize_gradients: bool. use GC both convolution & fc layers.
     :param normalize_gradients: bool. use gradient normalization.
     :param lookahead_merge_time: int. merge time.
     :param lookahead_blending_alpha: float. blending alpha.
     :param weight_decay: float. weight decay (L2 penalty).
+    :param weight_decouple: bool. the optimizer uses decoupled weight decay as in AdamW.
+    :param fixed_decay: bool. fix weight decay.
     :param norm_loss_factor: float. norm loss factor.
     :param adam_debias: bool. Only correct the denominator to avoid inflating step sizes early in training.
     :param eps: float. term added to the denominator to improve numerical stability.
     """
 
     def __init__(  # pylint: disable=R0913
         self,
@@ -64,47 +66,53 @@
         agc_clipping_value: float = 1e-2,
         agc_eps: float = 1e-3,
         centralize_gradients: bool = True,
         normalize_gradients: bool = True,
         lookahead_merge_time: int = 5,
         lookahead_blending_alpha: float = 0.5,
         weight_decay: float = 1e-4,
+        weight_decouple: bool = True,
+        fixed_decay: bool = False,
         norm_loss_factor: float = 1e-4,
         adam_debias: bool = False,
         eps: float = 1e-8,
     ):
-        self.lr = lr
+        self.validate_learning_rate(lr)
+        self.validate_learning_rate(warm_down_min_lr)
+        self.validate_betas(betas)
+        self.validate_range(beta0, 'beta0', 0.0, 1.0, range_type='[]')
+        self.validate_non_negative(weight_decay, 'weight_decay')
+        self.validate_non_negative(agc_clipping_value, 'agc_clipping_value')
+        self.validate_non_negative(eps, 'eps')
+        self.validate_non_negative(agc_eps, 'agc_eps')
+
         self.min_lr = warm_down_min_lr
-        self.beta0 = beta0
-        self.betas = betas
         self.use_softplus = use_softplus
         self.beta_softplus = beta_softplus
         self.agc_clipping_value = agc_clipping_value
         self.agc_eps = agc_eps
         self.centralize_gradients = centralize_gradients
         self.normalize_gradients = normalize_gradients
         self.lookahead_merge_time = lookahead_merge_time
         self.lookahead_blending_alpha = lookahead_blending_alpha
-        self.weight_decay = weight_decay
         self.norm_loss_factor = norm_loss_factor
-        self.eps = eps
-
-        self.validate_parameters()
 
         # lookahead
         self.lookahead_step: int = 0
 
         # learning rate
         self.starting_lr = lr
         self.current_lr = lr
 
         defaults: DEFAULTS = {
             'lr': lr,
             'betas': betas,
             'weight_decay': weight_decay,
+            'weight_decouple': weight_decouple,
+            'fixed_decay': fixed_decay,
             'adam_debias': adam_debias,
             'eps': eps,
         }
         super().__init__(params, defaults)
 
         # warmup iterations
         self.num_warm_up_iterations: int = (
@@ -116,46 +124,36 @@
             self.build_warm_down_iterations(num_iterations)
             if num_warm_down_iterations is None
             else num_warm_down_iterations
         )
         self.start_warm_down: int = num_iterations - self.num_warm_down_iterations
         self.warm_down_lr_delta: float = self.starting_lr - self.min_lr
 
-    def validate_parameters(self):
-        self.validate_learning_rate(self.lr)
-        self.validate_learning_rate(self.min_lr)
-        self.validate_betas(self.betas)
-        self.validate_beta0(self.beta0)
-        self.validate_weight_decay(self.weight_decay)
-        self.validate_epsilon(self.eps)
-
     def __str__(self) -> str:
         return 'Ranger21'
 
     @torch.no_grad()
     def reset(self):
         for group in self.param_groups:
+            group['step'] = 0
             for p in group['params']:
                 state = self.state[p]
 
-                state['step'] = 0
                 state['grad_ma'] = torch.zeros_like(p)
                 state['variance_ma'] = torch.zeros_like(p)
                 state['lookahead_params'] = torch.empty_like(p)
                 state['lookahead_params'].copy_(p)
                 state['neg_grad_ma'] = torch.zeros_like(p)
                 state['max_variance_ma'] = torch.zeros_like(p)
 
     @staticmethod
     def build_warm_up_iterations(total_iterations: int, beta2: float, warm_up_pct: float = 0.22) -> int:
         warm_up_iterations: int = math.ceil(2.0 / (1.0 - beta2))  # default un-tuned linear warmup
         beta_pct: float = warm_up_iterations / total_iterations
-        if beta_pct > 0.45:
-            return int(warm_up_pct * total_iterations)
-        return warm_up_iterations
+        return int(warm_up_pct * total_iterations) if beta_pct > 0.45 else warm_up_iterations
 
     @staticmethod
     def build_warm_down_iterations(total_iterations: int, warm_down_pct: float = 0.72) -> int:
         start_warm_down: int = int(warm_down_pct * total_iterations)
         return total_iterations - start_warm_down
 
     def warm_up_dampening(self, lr: float, step: int) -> float:
@@ -201,91 +199,96 @@
         for group in self.param_groups:
             if 'step' in group:
                 group['step'] += 1
             else:
                 group['step'] = 1
 
             beta1, beta2 = group['betas']
+
+            bias_correction2: float = 1.0 - beta2 ** group['step']
+
             for p in group['params']:
                 if p.grad is None:
                     continue
 
                 grad = p.grad
                 if grad.is_sparse:
                     raise NoSparseGradientError(str(self))
 
                 param_size += p.numel()
 
-                # Apply Adaptive Gradient Clipping (AGC)
-                p = agc(p, agc_eps=self.agc_eps, agc_clip_val=self.agc_clipping_value)  # noqa: PLW2901
-
                 state = self.state[p]
                 if len(state) == 0:
                     state['grad_ma'] = torch.zeros_like(p)
                     state['variance_ma'] = torch.zeros_like(p)
                     state['lookahead_params'] = torch.empty_like(p)
                     state['lookahead_params'].copy_(p)
                     state['neg_grad_ma'] = torch.zeros_like(p)
                     state['max_variance_ma'] = torch.zeros_like(p)
 
-                # Apply GC & GradNorm
-                # TODO : Gradient Clipping (Norm)
+                # Apply Adaptive Gradient Clipping (AGC)
+                grad.copy_(agc(p, grad, self.agc_eps, self.agc_clipping_value))
+
+                # Apply gradient centralization & normalization
                 grad = centralize_gradient(grad, gc_conv_only=False)
                 grad = normalize_gradient(grad)
 
-                bias_correction2 = 1.0 - beta2 ** group['step']
-
                 # second moment estimation
                 # using positive-negative momentum and bias correction
                 variance_ma = state['variance_ma']
                 variance_ma.mul_(beta2).addcmul_(grad, grad, value=1.0 - beta2)
                 variance_ma_sum += (variance_ma / bias_correction2).sum()
 
         if param_size == 0:
             raise ZeroParameterSizeError()
 
         variance_normalized = math.sqrt(variance_ma_sum / param_size)
-        if math.isnan(variance_normalized):
-            raise RuntimeError('hit nan for variance_normalized')
 
         # Phase 2 - Apply weight decay and step
         for group in self.param_groups:
-            lr = group['lr']
+            lr: float = group['lr']
             beta1, beta2 = group['betas']
 
-            bias_correction1 = 1.0 - beta1 ** group['step']  # fmt: skip
-            bias_correction2_sq = math.sqrt(1.0 - beta2 ** group['step'])  # fmt: skip
+            bias_correction1: float = 1.0 - beta1 ** group['step']  # fmt: skip
+            bias_correction2_sq: float = math.sqrt(1.0 - beta2 ** group['step'])  # fmt: skip
 
             noise_norm: float = math.sqrt((1.0 + beta2) ** 2 + beta2 ** 2)  # fmt: skip
 
             # warm up & down
             lr = self.warm_up_dampening(lr, group['step'])
             lr = self.warm_down(lr, group['step'])
 
             for p in group['params']:
                 if p.grad is None:
                     continue
 
                 # stable weight decay
-                if group['weight_decay']:
-                    p.mul_(1.0 - group['weight_decay'] * lr / variance_normalized)
+                self.apply_weight_decay(
+                    p=p,
+                    grad=None,
+                    lr=group['lr'],
+                    weight_decay=group['weight_decay'],
+                    weight_decouple=group['weight_decouple'],
+                    fixed_decay=group['fixed_decay'],
+                    ratio=1.0 / variance_normalized,
+                )
 
                 # norm loss
-                correction = 2.0 * self.norm_loss_factor * (1.0 - torch.div(1, unit_norm(p) + self.eps))
+                correction = 2.0 * self.norm_loss_factor * (1.0 - 1.0 / unit_norm(p).add_(group['eps']))
                 p.mul_(1.0 - lr * correction)
 
                 state = self.state[p]
                 if group['step'] % 2 == 1:
                     grad_ma, neg_grad_ma = state['grad_ma'], state['neg_grad_ma']
                 else:
                     grad_ma, neg_grad_ma = state['neg_grad_ma'], state['grad_ma']
 
                 variance_ma = state['variance_ma']
-
                 torch.max(state['max_variance_ma'], variance_ma, out=variance_ma)
+
                 de_nom = (variance_ma.sqrt() / bias_correction2_sq).add_(group['eps'])
 
                 grad = p.grad
                 grad = centralize_gradient(grad, gc_conv_only=False)
                 grad = normalize_gradient(grad)
 
                 grad_ma.mul_(beta1 ** 2).add_(grad, alpha=1.0 - beta1 ** 2)  # fmt: skip
@@ -307,14 +310,14 @@
         if self.lookahead_step >= self.lookahead_merge_time:
             self.lookahead_step: int = 0
             for group in self.param_groups:
                 for p in group['params']:
                     if p.grad is None:
                         continue
 
-                    param_state = self.state[p]
+                    state = self.state[p]
 
                     p.mul_(self.lookahead_blending_alpha).add_(
-                        param_state['lookahead_params'],
+                        state['lookahead_params'],
                         alpha=1.0 - self.lookahead_blending_alpha,
                     )
-                    param_state['lookahead_params'].copy_(p)
+                    state['lookahead_params'].copy_(p)
```

### Comparing `pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/rotograd.py` & `pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/rotograd.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/sam.py` & `pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/sam.py`

 * *Files 16% similar despite different names*

```diff
@@ -59,28 +59,23 @@
         self,
         params: PARAMETERS,
         base_optimizer: OPTIMIZER,
         rho: float = 0.05,
         adaptive: bool = False,
         **kwargs,
     ):
-        self.rho = rho
-
-        self.validate_parameters()
+        self.validate_non_negative(rho, 'rho')
 
         defaults: DEFAULTS = {'rho': rho, 'adaptive': adaptive}
         defaults.update(kwargs)
         super().__init__(params, defaults)
 
         self.base_optimizer = base_optimizer(self.param_groups, **kwargs)
         self.param_groups = self.base_optimizer.param_groups
 
-    def validate_parameters(self):
-        self.validate_rho(self.rho)
-
     def __str__(self) -> str:
         return 'SAM'
 
     @torch.no_grad()
     def reset(self):
         pass
```

### Comparing `pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/sgd.py` & `pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/sgd.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,38 +25,29 @@
         params: PARAMETERS,
         lr: float = 1e-3,
         kappa: float = 1000.0,
         xi: float = 10.0,
         constant: float = 0.7,
         weight_decay: float = 0.0,
     ):
-        self.lr = lr
-        self.kappa = kappa
-        self.xi = xi
-        self.constant = constant
-        self.weight_decay = weight_decay
-
-        self.validate_parameters()
+        self.validate_learning_rate(lr)
+        self.validate_non_negative(kappa, 'kappa')
+        self.validate_non_negative(xi, 'xi')
+        self.validate_non_negative(weight_decay, 'weight_decay')
+        self.validate_boundary(constant, boundary=1.0, bound_type='upper')
 
         defaults: DEFAULTS = {
             'lr': lr,
             'kappa': kappa,
             'xi': xi,
             'constant': constant,
             'weight_decay': weight_decay,
         }
         super().__init__(params, defaults)
 
-    def validate_parameters(self):
-        self.validate_learning_rate(self.lr)
-        self.validate_kappa(self.kappa)
-        self.validate_xi(self.xi)
-        self.validate_weight_decay(self.weight_decay)
-        self.validate_constant(self.constant, boundary=1.0)
-
     def __str__(self) -> str:
         return 'AccSGD'
 
     @torch.no_grad()
     def reset(self):
         for group in self.param_groups:
             for p in group['params']:
@@ -124,36 +115,29 @@
         lr: float = 1e-4,
         momentum: float = 0.0,
         weight_decay: float = 0.0,
         weight_decouple: bool = True,
         dampening: float = 0.0,
         nesterov: bool = False,
     ):
-        self.lr = lr
-        self.momentum = momentum
-        self.weight_decay = weight_decay
-
-        self.validate_parameters()
+        self.validate_learning_rate(lr)
+        self.validate_range(momentum, 'momentum', 0.0, 1.0)
+        self.validate_non_negative(weight_decay, 'weight_decay')
 
         defaults: DEFAULTS = {
             'lr': lr,
             'momentum': momentum,
             'weight_decay': weight_decay,
             'weight_decouple': weight_decouple,
             'dampening': dampening,
             'nesterov': nesterov,
         }
 
         super().__init__(params, defaults)
 
-    def validate_parameters(self):
-        self.validate_learning_rate(self.lr)
-        self.validate_momentum(self.momentum)
-        self.validate_weight_decay(self.weight_decay)
-
     def __str__(self) -> str:
         return 'SGDW'
 
     @torch.no_grad()
     def reset(self):
         for group in self.param_groups:
             for p in group['params']:
@@ -208,56 +192,50 @@
     r"""Adaptive SGD with estimation of the local smoothness (curvature).
 
     :param params: PARAMETERS. iterable of parameters to optimize or dicts defining parameter groups.
     :param lr: float. learning rate.
     :param amplifier: float. amplifier.
     :param weight_decay: float. weight decay (L2 penalty).
     :param weight_decouple: bool. the optimizer uses decoupled weight decay as in AdamW.
+    :param fixed_decay: bool. fix weight decay.
     :param theta: float. theta.
     :param dampening: float. dampening for momentum.
     :param eps: float. term added to the denominator to improve numerical stability.
     """
 
     def __init__(
         self,
         params: PARAMETERS,
         lr: float = 1e-2,
         amplifier: float = 0.02,
         weight_decay: float = 0.0,
         weight_decouple: bool = True,
+        fixed_decay: bool = False,
         theta: float = 1.0,
         dampening: float = 1.0,
         eps: float = 1e-5,
     ):
-        self.lr = lr
-        self.amplifier = amplifier
-        self.theta = theta
-        self.weight_decay = weight_decay
-        self.eps = eps
-
-        self.validate_parameters()
+        self.validate_learning_rate(lr)
+        self.validate_non_negative(amplifier, 'amplifier')
+        self.validate_non_negative(weight_decay, 'weight_decay')
+        self.validate_non_negative(eps, 'eps')
 
         defaults: DEFAULTS = {
             'lr': lr,
             'amplifier': amplifier,
             'weight_decay': weight_decay,
             'weight_decouple': weight_decouple,
+            'fixed_decay': fixed_decay,
             'theta': theta,
             'dampening': dampening,
             'eps': eps,
         }
 
         super().__init__(params, defaults)
 
-    def validate_parameters(self):
-        self.validate_learning_rate(self.lr)
-        self.validate_amplifier(self.amplifier)
-        self.validate_weight_decay(self.weight_decay)
-        self.validate_epsilon(self.eps)
-
     def __str__(self) -> str:
         return 'ASGD'
 
     @torch.no_grad()
     def reset(self):
         for group in self.param_groups:
             for _ in group['params']:
@@ -317,16 +295,19 @@
                 if p.grad is None:
                     continue
 
                 grad = p.grad
                 if grad.is_sparse:
                     raise NoSparseGradientError(str(self))
 
-                if group['weight_decay'] > 0.0:
-                    if group['weight_decouple']:
-                        p.mul_(1.0 - group['lr'] * group['weight_decay'])
-                    else:
-                        grad.add_(p, alpha=group['weight_decay'])
+                self.apply_weight_decay(
+                    p=p,
+                    grad=grad,
+                    lr=group['lr'],
+                    weight_decay=group['weight_decay'],
+                    weight_decouple=group['weight_decouple'],
+                    fixed_decay=group['fixed_decay'],
+                )
 
                 p.add_(grad, alpha=-new_lr)
 
         return loss
```

### Comparing `pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/sgdp.py` & `pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/lars.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,117 +1,103 @@
 import torch
-from torch.optim.optimizer import Optimizer
+from torch.optim import Optimizer
 
 from pytorch_optimizer.base.exception import NoSparseGradientError
 from pytorch_optimizer.base.optimizer import BaseOptimizer
 from pytorch_optimizer.base.types import CLOSURE, DEFAULTS, LOSS, PARAMETERS
-from pytorch_optimizer.optimizer.utils import projection
 
 
-class SGDP(Optimizer, BaseOptimizer):
-    r"""SGD + Slowing Down the Slowdown for Momentum Optimizers on Scale-invariant Weights.
+class LARS(Optimizer, BaseOptimizer):
+    r"""Layer-wise Adaptive Rate Scaling (no rate scaling or weight decay for parameters <= 1D).
 
     :param params: PARAMETERS. iterable of parameters to optimize or dicts defining parameter groups.
     :param lr: float. learning rate.
-    :param momentum: float. momentum factor.
-    :param dampening: float. dampening for momentum.
-    :param eps: float. term added to the denominator to improve numerical stability.
     :param weight_decay: float. weight decay (L2 penalty).
-    :param delta: float. threshold that determines whether a set of parameters is scale invariant or not.
-    :param wd_ratio: float. relative weight decay applied on scale-invariant parameters compared to that applied
-        on scale-variant parameters.
+    :param momentum: float. momentum.
+    :param dampening: float. dampening for momentum.
+    :param trust_coefficient: float. trust_coefficient.
     :param nesterov: bool. enables nesterov momentum.
     """
 
     def __init__(
         self,
         params: PARAMETERS,
         lr: float = 1e-3,
-        momentum: float = 0.0,
-        dampening: float = 0.0,
         weight_decay: float = 0.0,
-        eps: float = 1e-8,
-        delta: float = 0.1,
-        wd_ratio: float = 0.1,
+        momentum: float = 0.9,
+        dampening: float = 0.0,
+        trust_coefficient: float = 1e-3,
         nesterov: bool = False,
     ):
-        self.lr = lr
-        self.weight_decay = weight_decay
-        self.wd_ratio = wd_ratio
-        self.eps = eps
-
-        self.validate_parameters()
+        self.validate_learning_rate(lr)
+        self.validate_non_negative(weight_decay, 'weight_decay')
+        self.validate_range(momentum, 'momentum', 0.0, 1.0)
+        self.validate_non_negative(trust_coefficient, 'trust_coefficient')
 
         defaults: DEFAULTS = {
             'lr': lr,
             'weight_decay': weight_decay,
             'momentum': momentum,
             'dampening': dampening,
-            'delta': delta,
-            'wd_ratio': wd_ratio,
+            'trust_coefficient': trust_coefficient,
             'nesterov': nesterov,
-            'eps': eps,
         }
         super().__init__(params, defaults)
 
-    def validate_parameters(self):
-        self.validate_learning_rate(self.lr)
-        self.validate_weight_decay(self.weight_decay)
-        self.validate_weight_decay_ratio(self.wd_ratio)
-        self.validate_epsilon(self.eps)
-
     def __str__(self) -> str:
-        return 'SGDP'
+        return 'Lars'
 
     @torch.no_grad()
     def reset(self):
         for group in self.param_groups:
             for p in group['params']:
                 state = self.state[p]
 
-                state['momentum'] = torch.zeros_like(p)
+                state['mu'] = torch.zeros_like(p)
 
     @torch.no_grad()
     def step(self, closure: CLOSURE = None) -> LOSS:
         loss: LOSS = None
         if closure is not None:
             with torch.enable_grad():
                 loss = closure()
 
         for group in self.param_groups:
-            momentum = group['momentum']
             for p in group['params']:
                 if p.grad is None:
                     continue
 
                 grad = p.grad
                 if grad.is_sparse:
                     raise NoSparseGradientError(str(self))
 
-                state = self.state[p]
-                if len(state) == 0:
-                    state['momentum'] = torch.zeros_like(p)
-
-                buf = state['momentum']
-                buf.mul_(momentum).add_(grad, alpha=1.0 - group['dampening'])
-
-                d_p = buf.clone()
-                if group['nesterov']:
-                    d_p = d_p.mul_(momentum).add_(grad)
-
-                wd_ratio: float = 1.0
-                if len(p.shape) > 1:
-                    d_p, wd_ratio = projection(
-                        p,
-                        grad,
-                        d_p,
-                        group['delta'],
-                        group['wd_ratio'],
-                        group['eps'],
+                if p.ndim > 1:  # if not normalization gamma/beta or bias
+                    param_norm = torch.linalg.norm(p)
+                    update_norm = torch.linalg.norm(grad)
+
+                    one = torch.ones_like(param_norm)
+
+                    trust_ratio = torch.where(
+                        param_norm > 0.0,
+                        torch.where(update_norm > 0.0, (group['trust_coefficient'] * param_norm / update_norm), one),
+                        one,
                     )
 
-                if group['weight_decay'] > 0.0:
-                    p.mul_(1.0 - group['lr'] * group['weight_decay'] * wd_ratio / (1.0 - momentum))
+                    grad.add_(p, alpha=group['weight_decay'])
+                    grad.mul_(trust_ratio)
+
+                if group['momentum'] > 0.0:
+                    state = self.state[p]
+                    if 'momentum_buffer' not in state:
+                        state['momentum_buffer'] = grad.clone().detach()
+
+                    mb = state['momentum_buffer']
+                    mb.mul_(group['momentum']).add_(grad, alpha=1.0 - group['dampening'])
+
+                    if group['nesterov']:
+                        grad.add_(mb, alpha=group['momentum'])
+                    else:
+                        grad.copy_(mb)
 
-                p.add_(d_p, alpha=-group['lr'])
+                p.add_(grad, alpha=-group['lr'])
 
         return loss
```

### Comparing `pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/shampoo.py` & `pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/shampoo.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,46 +16,50 @@
 class Shampoo(Optimizer, BaseOptimizer):
     r"""Preconditioned Stochastic Tensor Optimization.
 
     :param params: PARAMETERS. iterable of parameters to optimize or dicts defining parameter groups.
     :param lr: float. learning rate.
     :param momentum: float. momentum.
     :param weight_decay: float. weight decay (L2 penalty).
+    :param weight_decouple: bool. the optimizer uses decoupled weight decay as in AdamW.
+    :param fixed_decay: bool. fix weight decay.
     :param preconditioning_compute_steps: int. performance tuning params for controlling memory and compute
         requirements. How often to compute pre-conditioner.
     :param matrix_eps: float. term added to the denominator to improve numerical stability.
     """
 
     def __init__(
         self,
         params: PARAMETERS,
         lr: float = 1e-3,
         momentum: float = 0.0,
         weight_decay: float = 0.0,
+        weight_decouple: bool = False,
+        fixed_decay: bool = False,
         preconditioning_compute_steps: int = 1,
         matrix_eps: float = 1e-6,
     ):
-        self.lr = lr
-        self.momentum = momentum
-        self.weight_decay = weight_decay
+        self.validate_learning_rate(lr)
+        self.validate_range(momentum, 'momentum', 0.0, 1.0)
+        self.validate_non_negative(weight_decay, 'weight_decay')
+        self.validate_step(preconditioning_compute_steps, 'preconditioning_compute_steps')
+        self.validate_non_negative(matrix_eps, 'matrix_eps')
+
         self.preconditioning_compute_steps = preconditioning_compute_steps
         self.matrix_eps = matrix_eps
 
-        self.validate_parameters()
-
-        defaults: DEFAULTS = {'lr': lr, 'momentum': momentum, 'weight_decay': weight_decay}
+        defaults: DEFAULTS = {
+            'lr': lr,
+            'momentum': momentum,
+            'weight_decay': weight_decay,
+            'weight_decouple': weight_decouple,
+            'fixed_decay': fixed_decay,
+        }
         super().__init__(params, defaults)
 
-    def validate_parameters(self):
-        self.validate_learning_rate(self.lr)
-        self.validate_momentum(self.momentum)
-        self.validate_weight_decay(self.weight_decay)
-        self.validate_update_frequency(self.preconditioning_compute_steps)
-        self.validate_epsilon(self.matrix_eps)
-
     def __str__(self) -> str:
         return 'Shampoo'
 
     @torch.no_grad()
     def reset(self):
         for group in self.param_groups:
             group['step'] = 0
@@ -69,15 +73,16 @@
 
         for group in self.param_groups:
             if 'step' in group:
                 group['step'] += 1
             else:
                 group['step'] = 1
 
-            momentum, weight_decay = group['momentum'], group['weight_decay']
+            momentum = group['momentum']
+
             for p in group['params']:
                 if p.grad is None:
                     continue
 
                 grad = p.grad
                 if grad.is_sparse:
                     raise NoSparseGradientError(str(self))
@@ -90,31 +95,37 @@
                     for dim_id, dim in enumerate(grad.size()):
                         state[f'pre_cond_{dim_id}'] = self.matrix_eps * torch.eye(dim, out=grad.new(dim, dim))
                         state[f'inv_pre_cond_{dim_id}'] = grad.new(dim, dim).zero_()
 
                 if momentum > 0.0:
                     grad.mul_(1.0 - momentum).add_(state['momentum_buffer'], alpha=momentum)
 
-                if weight_decay > 0.0:
-                    grad.add_(p, alpha=weight_decay)
+                self.apply_weight_decay(
+                    p=p,
+                    grad=p.grad,
+                    lr=group['lr'],
+                    weight_decay=group['weight_decay'],
+                    weight_decouple=group['weight_decouple'],
+                    fixed_decay=group['fixed_decay'],
+                )
 
                 order: int = grad.ndimension()
                 original_size: int = grad.size()
                 for dim_id, dim in enumerate(grad.size()):
                     pre_cond, inv_pre_cond = state[f'pre_cond_{dim_id}'], state[f'inv_pre_cond_{dim_id}']
 
                     grad = grad.transpose_(0, dim_id).contiguous()
                     transposed_size = grad.size()
 
                     grad = grad.view(dim, -1)
                     grad_t = grad.t()
 
                     pre_cond.add_(grad @ grad_t)
                     if group['step'] % self.preconditioning_compute_steps == 0:
-                        inv_pre_cond.copy_(compute_power_svd(pre_cond, -1.0 / order))
+                        inv_pre_cond.copy_(compute_power_svd(pre_cond, order))
 
                     if dim_id == order - 1:
                         grad = grad_t @ inv_pre_cond
                         grad = grad.view(original_size)
                     else:
                         grad = inv_pre_cond @ grad
                         grad = grad.view(transposed_size)
@@ -156,15 +167,15 @@
         requirements. How often to compute pre-conditioner. Ideally, 1 is the best. However, the current implementation
         doesn't work on the distributed environment (there are no statistics & pre-conditioners sync among replicas),
         compute on the GPU (not CPU) and the precision is fp32 (not fp64).
         Also, followed by the paper, `preconditioning_compute_steps` does not have a significant effect on the
         performance. So, If you have a problem with the speed, try to set this step bigger (e.g. 1000).
     :param statistics_compute_steps: int. How often to compute statistics. usually set to 1 (or 10).
     :param block_size: int. Block size for large layers (if > 0).
-        Block size = 1 ==> Adagrad (Don't do this, extremely inefficient!)
+        Block size = 1 ==> AdaGrad (Don't do this, extremely inefficient!)
         Block size should be as large as feasible under memory/time constraints.
     :param skip_preconditioning_rank_lt: int. Skips preconditioning for parameters with rank less than this value.
     :param no_preconditioning_for_layers_with_dim_gt: int. avoid preconditioning large layers to reduce overall memory.
     :param shape_interpretation: bool. Automatic shape interpretation (for eg: [4, 3, 1024, 512] would
         result in 12 x [1024, 512] L and R statistics. Disabled by default which results in Shampoo constructing
         statistics [4, 4], [3, 3], [1024, 1024], [512, 512].
     :param graft_type: int. type of grafting (SGD or AdaGrad or RMSProp or SQRT_N or None).
@@ -187,65 +198,59 @@
         weight_decay: float = 0.0,
         decoupled_weight_decay: bool = False,
         decoupled_learning_rate: bool = True,
         inverse_exponent_override: int = 0,
         start_preconditioning_step: int = 25,
         preconditioning_compute_steps: int = 1000,
         statistics_compute_steps: int = 1,
-        block_size: int = 256,
+        block_size: int = 512,
         skip_preconditioning_rank_lt: int = 1,
         no_preconditioning_for_layers_with_dim_gt: int = 8192,
         shape_interpretation: bool = True,
         graft_type: int = LayerWiseGrafting.SGD,
         pre_conditioner_type: int = PreConditionerType.ALL,
         nesterov: bool = True,
         diagonal_eps: float = 1e-10,
         matrix_eps: float = 1e-6,
         use_svd: bool = False,
     ):
-        self.lr = lr
-        self.betas = betas
-        self.weight_decay = weight_decay
+        self.validate_learning_rate(lr)
+        self.validate_betas(betas)
+        self.validate_non_negative(weight_decay, 'weight_decay')
+        self.validate_step(start_preconditioning_step, 'start_preconditioning_step')
+        self.validate_step(preconditioning_compute_steps, 'preconditioning_compute_steps')
+        self.validate_step(statistics_compute_steps, 'statistics_compute_steps')
+        self.validate_non_negative(diagonal_eps, 'diagonal_eps')
+        self.validate_non_negative(matrix_eps, 'matrix_eps')
+
         self.inverse_exponent_override = inverse_exponent_override
         self.start_preconditioning_step = start_preconditioning_step
         self.preconditioning_compute_steps = preconditioning_compute_steps
         self.statistics_compute_steps = statistics_compute_steps
         self.block_size = block_size
         self.skip_preconditioning_rank_lt = skip_preconditioning_rank_lt
         self.no_preconditioning_for_layers_with_dim_gt = no_preconditioning_for_layers_with_dim_gt
         self.shape_interpretation = shape_interpretation
         self.graft_type = graft_type
         self.pre_conditioner_type = pre_conditioner_type
         self.diagonal_eps = diagonal_eps
         self.matrix_eps = matrix_eps
         self.use_svd = use_svd
 
-        self.validate_parameters()
-
         defaults: DEFAULTS = {
             'lr': lr,
             'betas': betas,
             'weight_decay': weight_decay,
             'decoupled_weight_decay': decoupled_weight_decay,
             'decoupled_learning_rate': decoupled_learning_rate,
             'moving_average_for_momentum': moving_average_for_momentum,
             'nesterov': nesterov,
         }
         super().__init__(params, defaults)
 
-    def validate_parameters(self):
-        self.validate_learning_rate(self.lr)
-        self.validate_betas(self.betas)
-        self.validate_weight_decay(self.weight_decay)
-        self.validate_update_frequency(self.start_preconditioning_step)
-        self.validate_update_frequency(self.statistics_compute_steps)
-        self.validate_update_frequency(self.preconditioning_compute_steps)
-        self.validate_epsilon(self.diagonal_eps)
-        self.validate_epsilon(self.matrix_eps)
-
     def __str__(self) -> str:
         return 'ScalableShampoo'
 
     @torch.no_grad()
     def reset(self):
         for group in self.param_groups:
             group['step'] = 0
```

### Comparing `pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/shampoo_utils.py` & `pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/shampoo_utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -59,28 +59,28 @@
     r"""Graft using SQRTN."""
 
     def __init__(self, var: torch.Tensor):
         super().__init__(var)
 
     def precondition_gradient(self, grad: torch.Tensor) -> torch.Tensor:
         r"""Get preconditioned gradient."""
-        return grad.sign_()
+        return grad.sign()
 
 
 class AdaGradGraft(SGDGraft):
-    r"""Graft using Adagrad. Essentially an implementation of Adagrad with momentum.
+    r"""Graft using AdaGrad. Essentially an implementation of AdaGrad with momentum.
 
     :param var: torch.Tensor. variable.
     :param diagonal_eps: float. diagonal epsilon.
     """
 
     def __init__(self, var: torch.Tensor, diagonal_eps: float):
         super().__init__(var)
         self.diagonal_eps = diagonal_eps
-        self.statistics: torch.Tensor = torch.zeros_like(var, device=var.device)
+        self.statistics: torch.Tensor = torch.zeros_like(var)
 
     def add_statistics(self, grad: torch.Tensor, _):
         r"""Add the statistics."""
         self.statistics.add_(grad.pow(2))
 
     def precondition_gradient(self, grad: torch.Tensor) -> torch.Tensor:
         r"""Get preconditioned gradient."""
@@ -93,15 +93,15 @@
     :param var: torch.Tensor. variable.
     :param diagonal_eps: float. diagonal epsilon.
     """
 
     def __init__(self, var: torch.Tensor, diagonal_eps: float):
         super().__init__(var)
         self.diagonal_eps = diagonal_eps
-        self.statistics: torch.Tensor = torch.zeros_like(var, device=var.device)
+        self.statistics: torch.Tensor = torch.zeros_like(var)
 
     def add_statistics(self, grad: torch.Tensor, beta2: float):
         r"""Add the statistics."""
         self.statistics.mul_(beta2).addcmul_(grad, grad, value=1.0 - beta2)
 
     def precondition_gradient(self, grad: torch.Tensor) -> torch.Tensor:
         r"""Get preconditioned gradient."""
@@ -134,60 +134,66 @@
                 split_sizes.append(np.array([d], dtype=np.int32))
                 continue
 
             # d - 1, otherwise split appends a 0-size array.
             num_split: int = (d - 1) // block_size
             indices = (np.arange(num_split, dtype=np.int32) + 1) * block_size
 
-            sizes = np.ones(num_split + 1, dtype=np.int32) * block_size
+            sizes: np.ndarray = np.ones(num_split + 1, dtype=np.int32) * block_size
             sizes[-1] = d - indices[-1]
 
             self.splits.append((i, indices))
             self.split_sizes.append((i, sizes))
             split_sizes.append(sizes)
 
         self.num_splits: int = len(split_sizes)
-        self.pre_conditioner_shapes: List[List[int]] = []
+        self.pre_conditioner_shapes: List[List[int]] = self.build_pre_conditioner_shapes(
+            split_sizes, pre_conditioner_type, rank
+        )
+
+    @staticmethod
+    def build_pre_conditioner_shapes(
+        split_sizes: List[np.ndarray], pre_conditioner_type: int, rank: int
+    ) -> List[List[int]]:
+        r"""Build pre-conditioner shapes."""
+        pre_conditioner_shapes: List[List[int]] = []
         for t in itertools.product(*split_sizes):
             t_shape: List[Optional[List[int]]] = [[d, d] for d in t]
             if pre_conditioner_type == PreConditionerType.INPUT:
                 t_shape = t_shape[:-1] + [None]
             if pre_conditioner_type == PreConditionerType.OUTPUT:
                 t_shape = [None] * (rank - 1) + t_shape[-1:]
-            self.pre_conditioner_shapes.extend(t_shape)
+            pre_conditioner_shapes.extend(t_shape)
+        return pre_conditioner_shapes
 
     def shapes_for_pre_conditioners(self) -> List[List[int]]:
         r"""Get shapes of pre-conditioner."""
         return self.pre_conditioner_shapes
 
+    @torch.no_grad()
     def partition(self, x: torch.Tensor) -> List[torch.Tensor]:
         r"""Partition tensor into blocks."""
         if x.shape != self.shape:
-            raise ValueError(f'self._shape != x.shape ({self.shape} vs {x.shape})')
+            raise ValueError(f'self.shape != x.shape ({self.shape} vs {x.shape})')
 
-        tensors: List[torch.Tensor] = [x]
+        tensors = [x]
         for i, sizes in self.split_sizes:
-            tensors_local: List[torch.Tensor] = []
-            for t in tensors:
-                tensors_local.extend(torch.split(t, list(sizes), dim=i))
-            tensors = tensors_local
+            tensors = [torch.split(t, list(sizes), dim=i) for t in tensors]
+            tensors = [t for tensor in tensors for t in tensor]
         return tensors
 
     def merge_partitions(self, partitions: List[torch.Tensor]) -> torch.Tensor:
         r"""Merge partitions back to original shape."""
         for i, indices in reversed(self.splits):
             n: int = len(indices) + 1
 
             partitions: List[torch.Tensor] = [
-                torch.cat(partitions[idx:idx + n], axis=i) for idx in range(0, len(partitions), n)  # fmt: skip
+                torch.cat(partitions[idx:idx + n], dim=i) for idx in range(0, len(partitions), n)  # fmt: skip
             ]
 
-        # TODO
-        # when length of partitions is 1, raise error
-
         return partitions[0]
 
 
 class PreConditionerType(IntEnum):
     r"""Type of PreConditioner.
 
     In default (ALL), computes pre-conditioner for each dim.
@@ -197,25 +203,25 @@
 
     ALL = 0
     INPUT = 1
     OUTPUT = 2
 
 
 class PreConditioner:
-    r"""Compute statistics/shape from gradients for preconditioning.
+    r"""Compute statistics & shape from gradients for preconditioning.
 
     :param var: torch.Tensor. variable.
     :param beta2: float. beta2.
-    :param inverse_exponent_override: int.
-    :param block_size: int.
-    :param skip_preconditioning_rank_lt: int.
-    :param no_preconditioning_for_layers_with_dim_gt: int.
-    :param shape_interpretation: bool.
+    :param inverse_exponent_override: int. override inv exp.
+    :param block_size: int. size of block.
+    :param skip_preconditioning_rank_lt: int. skip low-rank parameter.
+    :param no_preconditioning_for_layers_with_dim_gt: int. skip large size of dim of parameter.
+    :param shape_interpretation: bool. reshaping parameter.
     :param pre_conditioner_type: int. type of pre-conditioner.
-    :param matrix_eps: float.
+    :param matrix_eps: float. epsilon of matrix.
     :param use_svd: bool. use SVD instead of Schur-Newton method to calculate M^{-1/p}.
     """
 
     def __init__(
         self,
         var: torch.Tensor,
         beta2: float,
@@ -302,28 +308,25 @@
                 axes: List[int] = [ax for ax in range(partitioned_grad.ndim) if ax != i]
                 stat: torch.Tensor = torch.tensordot(partitioned_grad, partitioned_grad, dims=[axes, axes])
                 self.statistics[j * self.rank + i].mul_(self.beta2).add_(stat, alpha=self.w2)
 
     def compute_pre_conditioners(self):
         r"""Compute L^{-1/exp} for each stats matrix L.
 
-        If `self.use_svd` is enabled,
-            where all shapes of statistics & pre-conditioners are same, perform batch SVD
-            else, SVD one by one.
-        else (`self.use_svd` is disabled), use Schur-Newton method
+        If `self.use_svd` is enabled and where all shapes of statistics & pre-conditioners are same, perform batch SVD.
+        else, SVD one by one.
+        If `self.use_svd` is disabled, use Schur-Newton method, which is usually much faster.
         """
         if self.use_svd and self.is_same_shapes:
-            self.pre_conditioners = compute_power_svd(
-                matrix=self.statistics, power=-1.0 / self.exponent_for_pre_conditioner
-            )
+            self.pre_conditioners = compute_power_svd(matrix=self.statistics, power=self.exponent_for_pre_conditioner)
             return
 
         for i, statistic in enumerate(self.statistics):
             self.pre_conditioners[i] = (
-                compute_power_svd(matrix=statistic, power=-1.0 / self.exponent_for_pre_conditioner)
+                compute_power_svd(matrix=statistic, power=self.exponent_for_pre_conditioner)
                 if self.use_svd
                 else compute_power_schur_newton(
                     mat_g=statistic, p=self.exponent_for_pre_conditioner, ridge_epsilon=self.matrix_eps
                 )
             )
 
     @staticmethod
@@ -386,48 +389,39 @@
         return SGDGraft(p)
     if graft_type == LayerWiseGrafting.SQRTN:
         return SQRTNGraft(p)
     return Graft(p)
 
 
 @torch.no_grad()
-def power_iteration(mat_g: torch.Tensor, error_tolerance: float = 1e-6, num_iters: int = 50) -> torch.Tensor:
+def power_iteration(mat_g: torch.Tensor, num_iters: int = 100) -> torch.Tensor:
     r"""Compute the maximum eigenvalue of matrix, for scaling.
 
-        Usually, power_iteration method is faster than torch.einval in case of the symmetric PSD matrix.
+        Mostly, power_iteration method is faster than torch.einval in case of the symmetric PSD matrix.
+        Also, I removed the validation, error of singular value every iteration, so that boosting the speed.
 
     :param mat_g: torch.Tensor. the symmetric PSD matrix.
-    :param error_tolerance: float. Iterative exit condition.
     :param num_iters: int. Number of iterations.
     """
     v = torch.randn(mat_g.shape[0], dtype=mat_g.dtype, device=mat_g.device)
-
-    singular_val = 1e-16
+    mat_v = torch.empty_like(v)
 
     for _ in range(num_iters):
-        v.div_(torch.linalg.norm(v))
+        torch.mv(mat_g, v, out=mat_v)
+        v = mat_v.div(torch.linalg.norm(mat_v))
 
-        mat_v = torch.mv(mat_g, v)
-        s_v = torch.dot(v, mat_v)
-
-        if torch.abs_(s_v - singular_val) <= error_tolerance:
-            break
-
-        v = mat_v
-        singular_val = s_v
-
-    return singular_val
+    return (v.t() @ mat_g @ v).clamp_min_(1e-16)
 
 
 @torch.no_grad()
 def compute_power_schur_newton(
     mat_g: torch.Tensor,
     p: int,
     max_iters: int = 100,
-    error_tolerance: float = 1e-6,
+    error_tolerance: float = 1e-3,
     ridge_epsilon: float = 1e-6,
     max_error_ratio: float = 1.2,
 ) -> torch.Tensor:
     r"""Compute G^{-1/p} using a coupled Newton iteration.
 
         See for example equation 3.2 on page 9 of:
             A Schur-Newton Method for the Matrix p-th Root and its Inverse by Chun-Hua Guo and Nicholas J. Higham
@@ -452,60 +446,64 @@
     :param max_error_ratio: float. Sometimes error increases after an iteration before decreasing and converging.
         1.2 factor is used to bound the maximal allowed increase.
     """
     shape: List[int] = mat_g.shape
     if len(shape) == 1:
         return torch.pow(mat_g + ridge_epsilon, -1.0 / p)
 
-    identity = torch.eye(shape[0], device=mat_g.device, dtype=mat_g.dtype)
+    identity = torch.eye(shape[0], dtype=mat_g.dtype, device=mat_g.device)
     if shape[0] == 1:
         return identity
 
-    mat_g.add_(ridge_epsilon * power_iteration(mat_g) * identity)
+    mat_g += power_iteration(mat_g) * identity * ridge_epsilon
 
     z = (1 + p) / (2 * torch.linalg.norm(mat_g))
 
     mat_root = identity * torch.pow(z, 1.0 / p)
+
     mat_m = mat_g * z
 
     alpha: float = -1.0 / p
     alpha_identity = (1.0 - alpha) * identity
 
-    error = torch.max(torch.abs(mat_m - identity))
-
-    new_mat_root = torch.empty_like(mat_root)
+    prev_error = torch.max(torch.abs(mat_m - identity))
 
     for _ in range(max_iters):
         mat_m_i = alpha_identity + alpha * mat_m
 
-        torch.matmul(mat_root, mat_m_i, out=new_mat_root)
+        new_mat_root = torch.matmul(mat_root, mat_m_i)
         torch.matmul(torch.linalg.matrix_power(mat_m_i, p), mat_m, out=mat_m)
 
-        new_error = torch.max(torch.abs(mat_m - identity))
-        if new_error <= error_tolerance or new_error > error * max_error_ratio:
+        error = torch.max(torch.abs(mat_m - identity))
+
+        # NOTE
+        # this is the main bottleneck that makes Scalable Shampoo slow.
+        # because it is handled on the Python side so values need to be on the CPU
+        # while XLA devices (e.g. TPU) doesn't seem to be affected.
+        if torch.logical_or(error > prev_error * max_error_ratio, error <= error_tolerance):
             break
 
         mat_root = new_mat_root
-        error = new_error
+        prev_error = error
 
     return mat_root
 
 
 @torch.no_grad()
 def compute_power_svd(matrix: torch.Tensor, power: float) -> torch.Tensor:
     r"""Compute G^{-1/p} using a SVD.
 
         Calculate SVD on the GPU. Sometimes, SVD on the CPU is faster than GPU, but based on the several experiments,
         CUDA seems much faster than on CPU.
 
     :param matrix: torch.Tensor. a square positive semi-definite matrix.
-    :param power: float. -1.0 / order.
+    :param power: float. rank.
     """
     u, s, vh = torch.linalg.svd(matrix, full_matrices=False)
-    s.pow_(power)
+    s.pow_(-1.0 / power)
     return u @ (s.diag() if len(matrix.shape) == 2 else s.diag_embed()) @ vh
 
 
 def merge_small_dims(shape_to_merge: List[int], max_dim: int) -> List[int]:
     r"""Merge small dimensions.
 
         If there are some small dimensions, we collapse them
```

### Comparing `pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/sm3.py` & `pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/sm3.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,40 +10,33 @@
     r"""Memory-Efficient Adaptive Optimization.
 
     :param params: PARAMETERS. iterable of parameters to optimize or dicts defining parameter groups.
     :param lr: float. learning rate.
     :param momentum: float. coefficient used to scale prior updates before adding. This drastically increases
         memory usage if `momentum > 0.0`. This is ignored if the parameter's gradient is sparse.
     :param beta: float. coefficient used for exponential moving averages.
+    :param eps: float. term added to the denominator to improve numerical stability.
     """
 
     def __init__(
         self,
         params: PARAMETERS,
         lr: float = 1e-1,
         momentum: float = 0.0,
         beta: float = 0.0,
         eps: float = 1e-30,
     ):
-        self.lr = lr
-        self.momentum = momentum
-        self.beta = beta
-        self.eps = eps
-
-        self.validate_parameters()
+        self.validate_learning_rate(lr)
+        self.validate_range(momentum, 'momentum', 0.0, 1.0)
+        self.validate_range(beta, 'beta', 0.0, 1.0, range_type='[]')
+        self.validate_non_negative(eps, 'eps')
 
         defaults: DEFAULTS = {'lr': lr, 'momentum': momentum, 'beta': beta, 'eps': eps}
         super().__init__(params, defaults)
 
-    def validate_parameters(self):
-        self.validate_learning_rate(self.lr)
-        self.validate_momentum(self.momentum)
-        self.validate_beta(self.beta)
-        self.validate_epsilon(self.eps)
-
     def __str__(self) -> str:
         return 'SM3'
 
     @torch.no_grad()
     def reset(self):
         for group in self.param_groups:
             for p in group['params']:
```

### Comparing `pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/swats.py` & `pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/adams.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,194 +1,175 @@
 import math
 
 import torch
 from torch.optim.optimizer import Optimizer
 
-from pytorch_optimizer.base.exception import NoSparseGradientError
+from pytorch_optimizer.base.exception import NoSparseGradientError, ZeroParameterSizeError
 from pytorch_optimizer.base.optimizer import BaseOptimizer
 from pytorch_optimizer.base.types import BETAS, CLOSURE, DEFAULTS, LOSS, PARAMETERS
 
 
-class SWATS(Optimizer, BaseOptimizer):
-    r"""Improving Generalization Performance by Switching from Adam to SGD.
-
-        Currently, there's convergence issue. So, careful at using it.
+class AdamS(Optimizer, BaseOptimizer):
+    r"""Adam with stable weight decay.
 
     :param params: PARAMETERS. iterable of parameters to optimize or dicts defining parameter groups.
     :param lr: float. learning rate.
     :param betas: BETAS. coefficients used for computing running averages of gradient and the squared hessian trace.
     :param weight_decay: float. weight decay (L2 penalty).
     :param weight_decouple: bool. the optimizer uses decoupled weight decay as in AdamW.
-    :param amsgrad: bool. whether to use the AMSGrad variant of this algorithm from the paper.
-    :param nesterov: bool. enables Nesterov momentum.
+    :param fixed_decay: bool. fix weight decay.
+    :param ams_bound: bool. whether to use the AMSBound variant.
     :param r: float. EMA factor. between 0.9 ~ 0.99 is preferred.
     :param adanorm: bool. whether to use the AdaNorm variant.
     :param adam_debias: bool. Only correct the denominator to avoid inflating step sizes early in training.
     :param eps: float. term added to the denominator to improve numerical stability.
     """
 
     def __init__(
         self,
         params: PARAMETERS,
         lr: float = 1e-3,
         betas: BETAS = (0.9, 0.999),
-        weight_decay: float = 0.0,
-        weight_decouple: bool = False,
-        amsgrad: bool = False,
-        nesterov: bool = False,
+        weight_decay: float = 1e-4,
+        weight_decouple: bool = True,
+        fixed_decay: bool = False,
+        ams_bound: bool = False,
         r: float = 0.95,
         adanorm: bool = False,
         adam_debias: bool = False,
-        eps: float = 1e-9,
+        eps: float = 1e-8,
     ):
-        self.lr = lr
-        self.betas = betas
-        self.weight_decay = weight_decay
-        self.eps = eps
-
-        self.validate_parameters()
+        self.validate_learning_rate(lr)
+        self.validate_betas(betas)
+        self.validate_non_negative(weight_decay, 'weight_decay')
+        self.validate_non_negative(eps, 'eps')
 
         defaults: DEFAULTS = {
             'lr': lr,
             'betas': betas,
             'weight_decay': weight_decay,
             'weight_decouple': weight_decouple,
-            'amsgrad': amsgrad,
-            'nesterov': nesterov,
+            'fixed_decay': fixed_decay,
+            'ams_bound': ams_bound,
             'adanorm': adanorm,
             'adam_debias': adam_debias,
-            'phase': 'adam',
             'eps': eps,
         }
         if adanorm:
             defaults.update({'r': r})
 
         super().__init__(params, defaults)
 
-    def validate_parameters(self):
-        self.validate_learning_rate(self.lr)
-        self.validate_betas(self.betas)
-        self.validate_weight_decay(self.weight_decay)
-        self.validate_epsilon(self.eps)
-
     def __str__(self) -> str:
-        return 'SWATS'
+        return 'AdamS'
 
     @torch.no_grad()
     def reset(self):
         for group in self.param_groups:
             for p in group['params']:
                 state = self.state[p]
 
+                state['step'] = 0
                 state['exp_avg'] = torch.zeros_like(p)
                 state['exp_avg_sq'] = torch.zeros_like(p)
-                state['exp_avg2'] = torch.zeros((1,), dtype=p.dtype, device=p.device)
-                if group['amsgrad']:
+                if group['ams_bound']:
                     state['max_exp_avg_sq'] = torch.zeros_like(p)
                 if group['adanorm']:
                     state['exp_grad_norm'] = torch.zeros((1,), dtype=p.dtype, device=p.device)
 
     @torch.no_grad()
     def step(self, closure: CLOSURE = None) -> LOSS:
         loss: LOSS = None
         if closure is not None:
             with torch.enable_grad():
                 loss = closure()
 
-        for group in self.param_groups:
-            if 'step' in group:
-                group['step'] += 1
-            else:
-                group['step'] = 1
+        param_size: int = 0
+        exp_avg_sq_hat_sum: float = 0.0
 
+        for group in self.param_groups:
             beta1, beta2 = group['betas']
-            bias_correction1 = 1.0 - beta1 ** group['step']
-            bias_correction2 = 1.0 - beta2 ** group['step']
-
             for p in group['params']:
                 if p.grad is None:
                     continue
 
                 grad = p.grad
                 if grad.is_sparse:
                     raise NoSparseGradientError(str(self))
 
+                param_size += p.numel()
+
                 state = self.state[p]
 
                 if len(state) == 0:
+                    state['step'] = 0
                     state['exp_avg'] = torch.zeros_like(p)
                     state['exp_avg_sq'] = torch.zeros_like(p)
-                    state['exp_avg2'] = torch.zeros((1,), dtype=grad.dtype, device=grad.device)
-                    if group['amsgrad']:
+                    if group['ams_bound']:
                         state['max_exp_avg_sq'] = torch.zeros_like(p)
                     if group['adanorm']:
-                        state['exp_grad_norm'] = torch.zeros((1,), dtype=grad.dtype, device=grad.device)
-
-                exp_avg, exp_avg_sq = state['exp_avg'], state['exp_avg_sq']
-
-                if group['weight_decouple']:
-                    p.mul_(1.0 - group['weight_decay'] * group['lr'])
-                elif group['weight_decay'] > 0.0:
-                    grad.add_(p, alpha=group['weight_decay'])
-
-                if group['phase'] == 'sgd':
-                    if 'momentum_buffer' not in state:
-                        state['momentum_buffer'] = torch.zeros_like(grad)
-
-                    buf = state['momentum_buffer']
-                    buf.mul_(beta1).add_(grad)
-
-                    grad = buf.clone()
+                        state['exp_grad_norm'] = torch.zeros((1,), dtype=p.dtype, device=p.device)
 
-                    grad.mul_(1.0 - beta1)
-                    if group['nesterov']:
-                        grad.add_(buf, alpha=beta1)
+                state['step'] += 1
 
-                    p.add_(grad, alpha=-group['lr'])
+                bias_correction2: float = 1.0 - beta2 ** state['step']
 
-                    continue
-
-                s_grad = grad
-                if group['adanorm']:
-                    grad_norm = torch.linalg.norm(grad)
-
-                    exp_grad_norm = state['exp_grad_norm']
-                    exp_grad_norm.mul_(group['r']).add_(grad_norm, alpha=1.0 - group['r'])
-
-                    if exp_grad_norm > grad_norm:
-                        s_grad *= exp_grad_norm / grad_norm
+                s_grad = self.get_adanorm_gradient(
+                    grad=grad,
+                    adanorm=group['adanorm'],
+                    exp_grad_norm=state.get('exp_grad_norm', None),
+                    r=group.get('r', None),
+                )
 
+                exp_avg, exp_avg_sq = state['exp_avg'], state['exp_avg_sq']
                 exp_avg.mul_(beta1).add_(s_grad, alpha=1.0 - beta1)
                 exp_avg_sq.mul_(beta2).addcmul_(grad, grad, value=1.0 - beta2)
 
-                if group['amsgrad']:
+                if group['ams_bound']:
                     max_exp_avg_sq = state['max_exp_avg_sq']
                     torch.max(max_exp_avg_sq, exp_avg_sq, out=max_exp_avg_sq)
-                    de_nom = max_exp_avg_sq.sqrt().add_(group['eps'])
+                    exp_avg_sq_hat = max_exp_avg_sq
                 else:
-                    de_nom = exp_avg_sq.sqrt().add_(group['eps'])
-
-                step_size: float = group['lr'] * math.sqrt(bias_correction2)
-                if not group['adam_debias']:
-                    step_size /= bias_correction1
+                    exp_avg_sq_hat = exp_avg_sq
 
-                perturb = exp_avg.clone()
-                perturb.div_(de_nom).mul(-step_size)
+                exp_avg_sq_hat_sum += exp_avg_sq_hat.sum() / bias_correction2
 
-                p.add_(perturb)
+        if param_size == 0:
+            raise ZeroParameterSizeError()
 
-                perturb_view = perturb.view(-1)
-                pg = perturb_view.dot(grad.view(-1))
+        exp_avg_sq_hat_mean: float = math.sqrt(exp_avg_sq_hat_sum / param_size) + self.defaults['eps']
 
-                if pg != 0:
-                    scaling = perturb_view.dot(perturb_view).div_(-pg)
+        for group in self.param_groups:
+            beta1, beta2 = group['betas']
+            for p in group['params']:
+                if p.grad is None:
+                    continue
 
-                    exp_avg2 = state['exp_avg2']
-                    exp_avg2.mul_(beta2).add_(scaling, alpha=1.0 - beta2)
+                state = self.state[p]
 
-                    corrected_exp_avg = exp_avg2 / bias_correction2
+                self.apply_weight_decay(
+                    p=p,
+                    grad=None,
+                    lr=group['lr'],
+                    weight_decay=group['weight_decay'],
+                    weight_decouple=group['weight_decouple'],
+                    fixed_decay=group['fixed_decay'],
+                    ratio=1.0 / exp_avg_sq_hat_mean,
+                )
+
+                bias_correction1: float = 1.0 - beta1 ** state['step']
+                bias_correction2: float = 1.0 - beta2 ** state['step']
+
+                exp_avg_sq_hat = state['max_exp_avg_sq'] if group['ams_bound'] else state['exp_avg_sq']
+                exp_avg_sq_hat.div_(bias_correction2)
+
+                de_nom = exp_avg_sq_hat.sqrt().add_(group['eps'])
+
+                step_size: float = self.apply_adam_debias(
+                    adam_debias=group['adam_debias'],
+                    step_size=group['lr'],
+                    bias_correction1=bias_correction1,
+                )
 
-                    if group['step'] > 1 and corrected_exp_avg.allclose(scaling, rtol=group['eps']):
-                        group['phase'] = 'sgd'
-                        group['lr'] = corrected_exp_avg.item()
+                p.addcdiv_(state['exp_avg'], de_nom, value=-step_size)
 
         return loss
```

### Comparing `pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/utils.py` & `pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 def is_valid_parameters(parameters: PARAMETERS) -> bool:
     r"""Check where the parameters are valid."""
     return isinstance(parameters, (list, tuple)) and len(parameters) > 0 and isinstance(parameters[0], dict)
 
 
 def has_overflow(grad_norm: torch.Tensor) -> bool:
     r"""Detect inf and NaN in grad_norm."""
-    return grad_norm != grad_norm or grad_norm == float('inf')  # pylint: disable=comparison-with-itself
+    return grad_norm != grad_norm or grad_norm == float('inf')
 
 
 def to_real(x: torch.Tensor) -> torch.Tensor:
     r"""Return real value of tensor."""
     return x.real if torch.is_complex(x) else x
 
 
@@ -33,18 +33,18 @@
     :param x: torch.Tensor. gradient.
     :param use_channels: bool. channel-wise normalization.
     :param epsilon: float. eps.
     :return: torch.Tensor. normalized gradient.
     """
     size: int = x.dim()
     if size > 1 and use_channels:
-        s = x.std(dim=tuple(range(1, size)), keepdim=True) + epsilon
+        s = x.std(dim=tuple(range(1, size)), keepdim=True).add_(epsilon)
         x.div_(s)
     elif torch.numel(x) > 2:
-        s = x.std() + epsilon
+        s = x.std().add_(epsilon)
         x.div_(s)
     return x
 
 
 def flatten_grad(grads: List[torch.Tensor]) -> torch.Tensor:
     r"""Flatten the gradient."""
     return torch.cat([grad.flatten() for grad in grads])
@@ -92,18 +92,18 @@
 def clip_grad_norm(parameters: PARAMETERS, max_norm: float = 0, sync: bool = False) -> Union[torch.Tensor, float]:
     r"""Clip gradient norms.
 
         During combination with FSDP, will also ensure that grad norms are aggregated across all workers,
         since each worker only stores their shard of the gradients.
 
     :param parameters: PARAMETERS. Parameters whose gradients we wish to clip.
-    :param max_norm: float. Maximum norm we wish the gradients to have. If non-positive, then
-        we will not perform clipping.
-    :param sync: bool. Boolean indicating whether we should aggregate across the distributed group.
-        Used only in combination with FSDP.
+    :param max_norm: float. Maximum norm we wish the gradients to have. If non-positive, then we will not perform
+        clipping.
+    :param sync: bool. Boolean indicating whether we should aggregate across the distributed group. Used only in
+        combination with FSDP.
     :returns: The gradient norm across all parameters, before clipping.
     """
     if isinstance(parameters, torch.Tensor):
         parameters = [parameters]
 
     # make sure any generators are expanded
     parameters = list(parameters)
@@ -238,15 +238,15 @@
 @torch.no_grad()
 def l2_projection(parameters: PARAMETERS, max_norm: float = 1e2):
     r"""Get l2 normalized parameter."""
     global_norm = torch.sqrt(sum(p.norm().pow(2) for p in parameters))
     if global_norm > max_norm:
         ratio = max_norm / global_norm
         for param in parameters:
-            param *= ratio  # noqa: PLW2901
+            param.mul_(ratio)
 
 
 @torch.no_grad()
 def get_global_gradient_norm(param_groups: List[Dict], device: torch.device) -> torch.Tensor:
     r"""Get global gradient norm."""
     global_grad_norm = torch.zeros(1, dtype=torch.float32, device=device)
```

### Comparing `pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/yogi.py` & `pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/avagrad.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,84 +4,68 @@
 from torch.optim.optimizer import Optimizer
 
 from pytorch_optimizer.base.exception import NoSparseGradientError
 from pytorch_optimizer.base.optimizer import BaseOptimizer
 from pytorch_optimizer.base.types import BETAS, CLOSURE, DEFAULTS, LOSS, PARAMETERS
 
 
-class Yogi(Optimizer, BaseOptimizer):
-    r"""Decoupled Weight Decay Regularization.
+class AvaGrad(Optimizer, BaseOptimizer):
+    r"""Domain-independent Dominance of Adaptive Methods.
 
     :param params: PARAMETERS. iterable of parameters to optimize or dicts defining parameter groups.
     :param lr: float. learning rate.
     :param betas: BETAS. coefficients used for computing running averages of gradient and the squared hessian trace.
-    :param initial_accumulator: float. initial values for first and second moments.
     :param weight_decay: float. weight decay (L2 penalty).
     :param weight_decouple: bool. the optimizer uses decoupled weight decay as in AdamW.
-    :param r: float. EMA factor. between 0.9 ~ 0.99 is preferred.
-    :param adanorm: bool. whether to use the AdaNorm variant.
+    :param fixed_decay: bool. fix weight decay.
     :param adam_debias: bool. Only correct the denominator to avoid inflating step sizes early in training.
     :param eps: float. term added to the denominator to improve numerical stability.
     """
 
     def __init__(
         self,
         params: PARAMETERS,
-        lr: float = 1e-2,
+        lr: float = 1e-1,
         betas: BETAS = (0.9, 0.999),
-        initial_accumulator: float = 1e-6,
         weight_decay: float = 0.0,
         weight_decouple: bool = True,
-        r: float = 0.95,
-        adanorm: bool = False,
+        fixed_decay: bool = False,
         adam_debias: bool = False,
-        eps: float = 1e-3,
+        eps: float = 1e-1,
     ):
-        self.lr = lr
-        self.betas = betas
-        self.initial_accumulator = initial_accumulator
-        self.weight_decay = weight_decay
-        self.eps = eps
-
-        self.validate_parameters()
+        self.validate_learning_rate(lr)
+        self.validate_betas(betas)
+        self.validate_non_negative(weight_decay, 'weight_decay')
+        self.validate_non_negative(eps, 'eps')
 
         defaults: DEFAULTS = {
             'lr': lr,
             'betas': betas,
             'weight_decay': weight_decay,
             'weight_decouple': weight_decouple,
-            'initial_accumulator': initial_accumulator,
-            'adanorm': adanorm,
+            'fixed_decay': fixed_decay,
             'adam_debias': adam_debias,
+            'gamma': None,
             'eps': eps,
         }
-        if adanorm:
-            defaults.update({'r': r})
 
         super().__init__(params, defaults)
 
-    def validate_parameters(self):
-        self.validate_learning_rate(self.lr)
-        self.validate_betas(self.betas)
-        self.validate_weight_decay(self.weight_decay)
-        self.validate_epsilon(self.eps)
-
     def __str__(self) -> str:
-        return 'Yogi'
+        return 'AvaGrad'
 
     @torch.no_grad()
     def reset(self):
         for group in self.param_groups:
+            group['step'] = 0
             for p in group['params']:
                 state = self.state[p]
 
-                state['exp_avg'] = torch.full_like(p, fill_value=group['initial_accumulator'])
-                state['exp_avg_sq'] = torch.full_like(p, fill_value=group['initial_accumulator'])
-                if group['adanorm']:
-                    state['exp_grad_norm'] = torch.zeros((1,), dtype=p.dtype, device=p.device)
+                state['exp_avg'] = torch.zeros_like(p)
+                state['exp_avg_sq'] = torch.zeros_like(p)
 
     @torch.no_grad()
     def step(self, closure: CLOSURE = None) -> LOSS:
         loss: LOSS = None
         if closure is not None:
             with torch.enable_grad():
                 loss = closure()
@@ -89,50 +73,63 @@
         for group in self.param_groups:
             if 'step' in group:
                 group['step'] += 1
             else:
                 group['step'] = 1
 
             beta1, beta2 = group['betas']
-            bias_correction1 = 1.0 - beta1 ** group['step']
-            bias_correction2_sq = math.sqrt(1.0 - beta2 ** group['step'])
+
+            bias_correction1: float = 1.0 - beta1 ** group['step']
+            bias_correction2_sq: float = math.sqrt(1.0 - beta2 ** group['step'])
+            prev_bias_correction2_sq: float = math.sqrt(1.0 - beta2 ** (group['step'] - 1))
+
+            squared_norm: float = 0.0
+            num_params: float = 0.0
 
             for p in group['params']:
                 if p.grad is None:
                     continue
 
                 grad = p.grad
                 if grad.is_sparse:
                     raise NoSparseGradientError(str(self))
 
                 state = self.state[p]
 
                 if len(state) == 0:
-                    state['exp_avg'] = torch.full_like(p, fill_value=group['initial_accumulator'])
-                    state['exp_avg_sq'] = torch.full_like(p, fill_value=group['initial_accumulator'])
-                    if group['adanorm']:
-                        state['exp_grad_norm'] = torch.zeros((1,), dtype=grad.dtype, device=grad.device)
-
-                grad_p2 = grad.mul(grad)
-
-                exp_avg, exp_avg_sq = state['exp_avg'], state['exp_avg_sq']
-
-                s_grad = grad
-                if group['adanorm']:
-                    grad_norm = torch.linalg.norm(grad)
-
-                    exp_grad_norm = state['exp_grad_norm']
-                    exp_grad_norm.mul_(group['r']).add_(grad_norm, alpha=1.0 - group['r'])
-
-                    if exp_grad_norm > grad_norm:
-                        s_grad *= exp_grad_norm / grad_norm
-
-                exp_avg.mul_(beta1).add_(s_grad, alpha=1.0 - beta1)
-                exp_avg_sq.addcmul_((exp_avg_sq - grad_p2).sign_(), grad_p2, value=-(1.0 - beta2))
+                    state['exp_avg'] = torch.zeros_like(p)
+                    state['exp_avg_sq'] = torch.zeros_like(p)
 
-                de_nom = exp_avg_sq.sqrt()
-                de_nom.div_(bias_correction2_sq).add_(group['eps'])
+                self.apply_weight_decay(
+                    p=p,
+                    grad=p.grad,
+                    lr=group['lr'],
+                    weight_decay=group['weight_decay'],
+                    weight_decouple=group['weight_decouple'],
+                    fixed_decay=group['fixed_decay'],
+                )
+
+                exp_avg = state['exp_avg']
+                exp_avg.mul_(beta1).add_(grad, alpha=1.0 - beta1)
+
+                exp_avg_sq = state['exp_avg_sq']
+                sqrt_exp_avg_sq = exp_avg_sq.sqrt()
+
+                if group['step'] > 1:
+                    de_nom = sqrt_exp_avg_sq.div(prev_bias_correction2_sq).add_(group['eps'])
+
+                    step_size: float = self.apply_adam_debias(
+                        adam_debias=group['adam_debias'],
+                        step_size=group['gamma'] * group['lr'],
+                        bias_correction1=bias_correction1,
+                    )
+                    p.addcdiv_(exp_avg, de_nom, value=-step_size)
+
+                exp_avg_sq.mul_(beta2).addcmul_(grad, grad, value=1.0 - beta2)
+
+                param_wise_lr = sqrt_exp_avg_sq.div_(bias_correction2_sq).add_(group['eps'])
+                squared_norm += param_wise_lr.norm(-2) ** -2
+                num_params += param_wise_lr.numel()
 
-                step_size: float = group['lr'] / bias_correction1 if not group['adam_debias'] else group['lr']
-                p.addcdiv_(exp_avg, de_nom, value=-step_size)
+            group['gamma'] = 0.0 if num_params == 0.0 else 1.0 / math.sqrt(squared_norm / num_params)
 
         return loss
```

