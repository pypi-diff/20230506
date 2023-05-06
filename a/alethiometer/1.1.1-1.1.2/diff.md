# Comparing `tmp/alethiometer-1.1.1.tar.gz` & `tmp/alethiometer-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alethiometer-1.1.1.tar", last modified: Fri May  5 16:17:07 2023, max compression
+gzip compressed data, was "alethiometer-1.1.2.tar", last modified: Sat May  6 09:28:46 2023, max compression
```

## Comparing `alethiometer-1.1.1.tar` & `alethiometer-1.1.2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxr-x   0 u2280887  (1000) u2280887  (1000)        0 2023-05-05 16:17:07.432465 alethiometer-1.1.1/
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)    11357 2023-04-07 16:49:02.000000 alethiometer-1.1.1/LICENSE
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     8965 2023-05-05 16:17:07.432465 alethiometer-1.1.1/PKG-INFO
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     8255 2023-05-05 16:15:51.000000 alethiometer-1.1.1/README.md
-drwxrwxr-x   0 u2280887  (1000) u2280887  (1000)        0 2023-05-05 16:17:07.428465 alethiometer-1.1.1/alethiometer/
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)      313 2023-04-11 12:10:43.000000 alethiometer-1.1.1/alethiometer/__init__.py
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)      245 2023-05-05 16:15:55.000000 alethiometer-1.1.1/alethiometer/__version__.py
-drwxrwxr-x   0 u2280887  (1000) u2280887  (1000)        0 2023-05-05 16:17:07.428465 alethiometer-1.1.1/alethiometer/datasets/
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)      254 2023-04-07 17:54:55.000000 alethiometer-1.1.1/alethiometer/datasets/__init__.py
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     4853 2023-04-17 13:10:20.000000 alethiometer-1.1.1/alethiometer/datasets/dataset.py
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     2174 2023-04-07 17:54:22.000000 alethiometer-1.1.1/alethiometer/datasets/h5py_dataset.py
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     5109 2023-04-07 17:55:28.000000 alethiometer-1.1.1/alethiometer/datasets/imagenet16.py
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     1077 2023-04-07 15:01:32.000000 alethiometer-1.1.1/alethiometer/utils.py
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     5512 2023-05-01 09:09:45.000000 alethiometer-1.1.1/alethiometer/zc_proxy.py
-drwxrwxr-x   0 u2280887  (1000) u2280887  (1000)        0 2023-05-05 16:17:07.432465 alethiometer-1.1.1/alethiometer/zero_cost_metrics/
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     1734 2023-04-30 15:50:05.000000 alethiometer-1.1.1/alethiometer/zero_cost_metrics/__init__.py
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     1475 2023-04-07 17:10:09.000000 alethiometer-1.1.1/alethiometer/zero_cost_metrics/grad_norm.py
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     3624 2023-04-07 17:13:08.000000 alethiometer-1.1.1/alethiometer/zero_cost_metrics/grasp.py
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     2926 2023-04-11 16:57:48.000000 alethiometer-1.1.1/alethiometer/zero_cost_metrics/naswot.py
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     2079 2023-04-28 20:46:05.000000 alethiometer-1.1.1/alethiometer/zero_cost_metrics/naswot_relu.py
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     2023 2023-04-07 17:09:49.000000 alethiometer-1.1.1/alethiometer/zero_cost_metrics/snip.py
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     1928 2023-04-07 17:06:05.000000 alethiometer-1.1.1/alethiometer/zero_cost_metrics/synflow.py
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     5830 2023-05-05 16:11:36.000000 alethiometer-1.1.1/alethiometer/zero_cost_metrics/t_cet.py
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)    16377 2023-05-04 11:20:27.000000 alethiometer-1.1.1/alethiometer/zero_cost_metrics/tenas.py
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     3420 2023-04-28 21:42:23.000000 alethiometer-1.1.1/alethiometer/zero_cost_metrics/zen.py
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     4522 2023-05-01 21:46:32.000000 alethiometer-1.1.1/alethiometer/zero_cost_metrics/zico.py
-drwxrwxr-x   0 u2280887  (1000) u2280887  (1000)        0 2023-05-05 16:17:07.428465 alethiometer-1.1.1/alethiometer.egg-info/
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     8965 2023-05-05 16:17:07.000000 alethiometer-1.1.1/alethiometer.egg-info/PKG-INFO
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)      976 2023-05-05 16:17:07.000000 alethiometer-1.1.1/alethiometer.egg-info/SOURCES.txt
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)        1 2023-05-05 16:17:07.000000 alethiometer-1.1.1/alethiometer.egg-info/dependency_links.txt
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)       37 2023-05-05 16:17:07.000000 alethiometer-1.1.1/alethiometer.egg-info/requires.txt
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)       13 2023-05-05 16:17:07.000000 alethiometer-1.1.1/alethiometer.egg-info/top_level.txt
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)       38 2023-05-05 16:17:07.432465 alethiometer-1.1.1/setup.cfg
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     6031 2023-04-07 18:04:03.000000 alethiometer-1.1.1/setup.py
-drwxrwxr-x   0 u2280887  (1000) u2280887  (1000)        0 2023-05-05 16:17:07.432465 alethiometer-1.1.1/tests/
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     1219 2023-04-25 09:05:55.000000 alethiometer-1.1.1/tests/test_nwot_api.py
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     1946 2023-04-30 16:15:53.000000 alethiometer-1.1.1/tests/test_tcet.py
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     3355 2023-04-29 09:46:22.000000 alethiometer-1.1.1/tests/test_zc.py
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     1319 2023-05-01 11:23:22.000000 alethiometer-1.1.1/tests/test_zico.py
+drwxrwxr-x   0 u2280887  (1000) u2280887  (1000)        0 2023-05-06 09:28:46.304340 alethiometer-1.1.2/
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)    11357 2023-04-07 16:49:02.000000 alethiometer-1.1.2/LICENSE
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     9164 2023-05-06 09:28:46.304340 alethiometer-1.1.2/PKG-INFO
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     8454 2023-05-06 09:28:20.000000 alethiometer-1.1.2/README.md
+drwxrwxr-x   0 u2280887  (1000) u2280887  (1000)        0 2023-05-06 09:28:46.300340 alethiometer-1.1.2/alethiometer/
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)      313 2023-04-11 12:10:43.000000 alethiometer-1.1.2/alethiometer/__init__.py
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)      245 2023-05-06 09:23:55.000000 alethiometer-1.1.2/alethiometer/__version__.py
+drwxrwxr-x   0 u2280887  (1000) u2280887  (1000)        0 2023-05-06 09:28:46.300340 alethiometer-1.1.2/alethiometer/datasets/
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)      254 2023-04-07 17:54:55.000000 alethiometer-1.1.2/alethiometer/datasets/__init__.py
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     4853 2023-04-17 13:10:20.000000 alethiometer-1.1.2/alethiometer/datasets/dataset.py
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     2174 2023-04-07 17:54:22.000000 alethiometer-1.1.2/alethiometer/datasets/h5py_dataset.py
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     5109 2023-04-07 17:55:28.000000 alethiometer-1.1.2/alethiometer/datasets/imagenet16.py
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     1077 2023-04-07 15:01:32.000000 alethiometer-1.1.2/alethiometer/utils.py
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     5512 2023-05-01 09:09:45.000000 alethiometer-1.1.2/alethiometer/zc_proxy.py
+drwxrwxr-x   0 u2280887  (1000) u2280887  (1000)        0 2023-05-06 09:28:46.304340 alethiometer-1.1.2/alethiometer/zero_cost_metrics/
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     1734 2023-04-30 15:50:05.000000 alethiometer-1.1.2/alethiometer/zero_cost_metrics/__init__.py
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     1475 2023-04-07 17:10:09.000000 alethiometer-1.1.2/alethiometer/zero_cost_metrics/grad_norm.py
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     3624 2023-04-07 17:13:08.000000 alethiometer-1.1.2/alethiometer/zero_cost_metrics/grasp.py
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     2926 2023-04-11 16:57:48.000000 alethiometer-1.1.2/alethiometer/zero_cost_metrics/naswot.py
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     2079 2023-04-28 20:46:05.000000 alethiometer-1.1.2/alethiometer/zero_cost_metrics/naswot_relu.py
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     2023 2023-04-07 17:09:49.000000 alethiometer-1.1.2/alethiometer/zero_cost_metrics/snip.py
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     1928 2023-04-07 17:06:05.000000 alethiometer-1.1.2/alethiometer/zero_cost_metrics/synflow.py
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     5830 2023-05-05 16:11:36.000000 alethiometer-1.1.2/alethiometer/zero_cost_metrics/t_cet.py
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)    16709 2023-05-06 09:22:38.000000 alethiometer-1.1.2/alethiometer/zero_cost_metrics/tenas.py
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     3420 2023-04-28 21:42:23.000000 alethiometer-1.1.2/alethiometer/zero_cost_metrics/zen.py
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     4522 2023-05-01 21:46:32.000000 alethiometer-1.1.2/alethiometer/zero_cost_metrics/zico.py
+drwxrwxr-x   0 u2280887  (1000) u2280887  (1000)        0 2023-05-06 09:28:46.300340 alethiometer-1.1.2/alethiometer.egg-info/
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     9164 2023-05-06 09:28:46.000000 alethiometer-1.1.2/alethiometer.egg-info/PKG-INFO
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)      976 2023-05-06 09:28:46.000000 alethiometer-1.1.2/alethiometer.egg-info/SOURCES.txt
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)        1 2023-05-06 09:28:46.000000 alethiometer-1.1.2/alethiometer.egg-info/dependency_links.txt
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)       37 2023-05-06 09:28:46.000000 alethiometer-1.1.2/alethiometer.egg-info/requires.txt
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)       13 2023-05-06 09:28:46.000000 alethiometer-1.1.2/alethiometer.egg-info/top_level.txt
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)       38 2023-05-06 09:28:46.304340 alethiometer-1.1.2/setup.cfg
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     6031 2023-04-07 18:04:03.000000 alethiometer-1.1.2/setup.py
+drwxrwxr-x   0 u2280887  (1000) u2280887  (1000)        0 2023-05-06 09:28:46.304340 alethiometer-1.1.2/tests/
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     1219 2023-04-25 09:05:55.000000 alethiometer-1.1.2/tests/test_nwot_api.py
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     1946 2023-04-30 16:15:53.000000 alethiometer-1.1.2/tests/test_tcet.py
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     3355 2023-04-29 09:46:22.000000 alethiometer-1.1.2/tests/test_zc.py
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     1319 2023-05-01 11:23:22.000000 alethiometer-1.1.2/tests/test_zico.py
```

### Comparing `alethiometer-1.1.1/LICENSE` & `alethiometer-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `alethiometer-1.1.1/PKG-INFO` & `alethiometer-1.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alethiometer
-Version: 1.1.1
+Version: 1.1.2
 Summary: ZC proxies calculation repo, altered from foresight package.
 Home-page: https://github.com/iViolinSolo/zero-cost-proxies
 Author: ViolinSolo
 Author-email: i.violinsolo@gmail.com
 License: Apache Software License
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
@@ -16,15 +16,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 <!--
  * @Author: ViolinSolo
  * @Date: 2023-03-26 10:11:01
- * @LastEditTime: 2023-05-05 17:15:45
+ * @LastEditTime: 2023-05-06 10:28:20
  * @LastEditors: ViolinSolo
  * @Description: Readme
  * @FilePath: /zero-cost-proxies/README.md
 -->
 # zero-cost-proxies
 Independent ZC proxies only for testing on it. 
 
@@ -64,14 +64,16 @@
 = lrn,                                                  = 
 =-------------------------------------------------------=
 = zico, not work in torch-cpu, I will check it later.   =
 =     zico must use at least two batches of data,       =
 =     in order to calculate cross-batch (non-zero) std  =
 =-------------------------------------------------------=
 = tcet,                                                 =
+= snr-synflow,                                          =
+= snr-snip,                                             =
 =========================================================
 ```
 
 ## 0. How to install.
 1. First create conda env with python version >= 3.6, this repo has been completely tested on python 3.9.  
     ```bash
     conda install pytorch==1.13.1 torchvision==0.14.1 torchaudio==0.13.1 pytorch-cuda=11.6 -c pytorch -c nvidia
@@ -105,14 +107,16 @@
 ## 1. Tests
 ImageNet16-120 cannot be automatically downloaded. Using script under `scripts/download_data.sh` to download:
 ```bash
 source scripts/download_data.sh nb201 ImageNet16-120
 # do not use `bash`, use `source` instead
 ```
 ## 2. Versions
+- V1.1.2  
+Fix bug in `tenas`, add net instance deep copy to avoid weight changes.
 - V1.1.1  
 Fix warnings in `tenas`, now using new torch api to calc eigenvalue.  
 Fix bug in `tcet`, add net instance deep copy to avoid weight changes, add manually designed `tcet` copy process, remove bn in synflow, add bn in snip.
 - V1.1.0  
 Add `tcet` metric, which calculates TCET score.
 Add `snr` metrics, which calculates SNR family scores.
 - V1.0.10
```

### Comparing `alethiometer-1.1.1/README.md` & `alethiometer-1.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 <!--
  * @Author: ViolinSolo
  * @Date: 2023-03-26 10:11:01
- * @LastEditTime: 2023-05-05 17:15:45
+ * @LastEditTime: 2023-05-06 10:28:20
  * @LastEditors: ViolinSolo
  * @Description: Readme
  * @FilePath: /zero-cost-proxies/README.md
 -->
 # zero-cost-proxies
 Independent ZC proxies only for testing on it. 
 
@@ -45,14 +45,16 @@
 = lrn,                                                  = 
 =-------------------------------------------------------=
 = zico, not work in torch-cpu, I will check it later.   =
 =     zico must use at least two batches of data,       =
 =     in order to calculate cross-batch (non-zero) std  =
 =-------------------------------------------------------=
 = tcet,                                                 =
+= snr-synflow,                                          =
+= snr-snip,                                             =
 =========================================================
 ```
 
 ## 0. How to install.
 1. First create conda env with python version >= 3.6, this repo has been completely tested on python 3.9.  
     ```bash
     conda install pytorch==1.13.1 torchvision==0.14.1 torchaudio==0.13.1 pytorch-cuda=11.6 -c pytorch -c nvidia
@@ -86,14 +88,16 @@
 ## 1. Tests
 ImageNet16-120 cannot be automatically downloaded. Using script under `scripts/download_data.sh` to download:
 ```bash
 source scripts/download_data.sh nb201 ImageNet16-120
 # do not use `bash`, use `source` instead
 ```
 ## 2. Versions
+- V1.1.2  
+Fix bug in `tenas`, add net instance deep copy to avoid weight changes.
 - V1.1.1  
 Fix warnings in `tenas`, now using new torch api to calc eigenvalue.  
 Fix bug in `tcet`, add net instance deep copy to avoid weight changes, add manually designed `tcet` copy process, remove bn in synflow, add bn in snip.
 - V1.1.0  
 Add `tcet` metric, which calculates TCET score.
 Add `snr` metrics, which calculates SNR family scores.
 - V1.0.10
```

### Comparing `alethiometer-1.1.1/alethiometer/datasets/dataset.py` & `alethiometer-1.1.2/alethiometer/datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `alethiometer-1.1.1/alethiometer/datasets/h5py_dataset.py` & `alethiometer-1.1.2/alethiometer/datasets/h5py_dataset.py`

 * *Files identical despite different names*

### Comparing `alethiometer-1.1.1/alethiometer/datasets/imagenet16.py` & `alethiometer-1.1.2/alethiometer/datasets/imagenet16.py`

 * *Files identical despite different names*

### Comparing `alethiometer-1.1.1/alethiometer/utils.py` & `alethiometer-1.1.2/alethiometer/utils.py`

 * *Files identical despite different names*

### Comparing `alethiometer-1.1.1/alethiometer/zc_proxy.py` & `alethiometer-1.1.2/alethiometer/zc_proxy.py`

 * *Files identical despite different names*

### Comparing `alethiometer-1.1.1/alethiometer/zero_cost_metrics/__init__.py` & `alethiometer-1.1.2/alethiometer/zero_cost_metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `alethiometer-1.1.1/alethiometer/zero_cost_metrics/grad_norm.py` & `alethiometer-1.1.2/alethiometer/zero_cost_metrics/grad_norm.py`

 * *Files identical despite different names*

### Comparing `alethiometer-1.1.1/alethiometer/zero_cost_metrics/grasp.py` & `alethiometer-1.1.2/alethiometer/zero_cost_metrics/grasp.py`

 * *Files identical despite different names*

### Comparing `alethiometer-1.1.1/alethiometer/zero_cost_metrics/naswot.py` & `alethiometer-1.1.2/alethiometer/zero_cost_metrics/naswot.py`

 * *Files identical despite different names*

### Comparing `alethiometer-1.1.1/alethiometer/zero_cost_metrics/naswot_relu.py` & `alethiometer-1.1.2/alethiometer/zero_cost_metrics/naswot_relu.py`

 * *Files identical despite different names*

### Comparing `alethiometer-1.1.1/alethiometer/zero_cost_metrics/snip.py` & `alethiometer-1.1.2/alethiometer/zero_cost_metrics/snip.py`

 * *Files identical despite different names*

### Comparing `alethiometer-1.1.1/alethiometer/zero_cost_metrics/synflow.py` & `alethiometer-1.1.2/alethiometer/zero_cost_metrics/synflow.py`

 * *Files identical despite different names*

### Comparing `alethiometer-1.1.1/alethiometer/zero_cost_metrics/t_cet.py` & `alethiometer-1.1.2/alethiometer/zero_cost_metrics/t_cet.py`

 * *Files identical despite different names*

### Comparing `alethiometer-1.1.1/alethiometer/zero_cost_metrics/tenas.py` & `alethiometer-1.1.2/alethiometer/zero_cost_metrics/tenas.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 '''
 Author: ViolinSolo
 Date: 2023-04-28 17:26:50
-LastEditTime: 2023-05-04 12:20:27
+LastEditTime: 2023-05-06 10:22:37
 LastEditors: ViolinSolo
 Description: TENAS score computation
-FilePath: /zero-cost-test/home/u2280887/GitHub/zero-cost-proxies/alethiometer/zero_cost_metrics/tenas.py
+FilePath: /zero-cost-proxies/alethiometer/zero_cost_metrics/tenas.py
 '''
 '''
 Copyright (C) 2010-2021 Alibaba Group Holding Limited.
 This file is modified from:
 https://github.com/VITA-Group/TENAS
 ------------------------------------------------------------
 modified by ViolinSolo from 
 https://github.com/idstcv/ZenNAS/blob/main/ZeroShotProxy/compute_te_nas_score.py
 '''
 
 # import os, sys
 # sys.path.append(os.path.dirname(os.path.dirname(os.path.abspath(__file__))))
 
 import argparse
+import gc
 import time
 import torch
 from torch import nn
 import numpy as np
 # import global_utils, argparse, ModelLoader, time
 from . import metric
 
@@ -325,19 +326,29 @@
     return -1 * ntk_score
 
 
 # =============================================================================
 #  TENAS score computation: tenas part
 # =============================================================================
 
-@metric('tenas', bn=True, num_batch=1)
+@metric('tenas', bn=True, num_batch=1, bn_shadow=True)
 def compute_TENAS_score(net: nn.Module, inputs, targets, split_data=1, loss_fn=None,  # these are necessary arguments limited by *zero_cost_metrics.__init__.calc_metric*, if you want to add more arguments, modify @metric decorator's parameters to provide dynamic default values.
-                     num_batch=None): # additional arguments
-    ntk = compute_NTK_score(net, inputs, targets, split_data, loss_fn, num_batch)
-    RN = compute_RN_score(net, inputs, targets, split_data, loss_fn, num_batch)
+                     num_batch=None, bn_shadow=True): # additional arguments
+    net1 = net.get_prunable_copy(bn=bn_shadow)  # manually keep bn in lnwot, and remove bn in synflow
+    ntk = compute_NTK_score(net1, inputs, targets, split_data, loss_fn, num_batch)
+    del net1
+    torch.cuda.empty_cache()
+    gc.collect()
+
+    net2 = net.get_prunable_copy(bn=bn_shadow)  # manually keep bn in lnwot, and remove bn in synflow
+    RN = compute_RN_score(net2, inputs, targets, split_data, loss_fn, num_batch)
+    del net2
+    torch.cuda.empty_cache()
+    gc.collect()
+
     the_score = ntk + RN
     return the_score
 
 
 # def parse_cmd_options(argv):
 #     parser = argparse.ArgumentParser()
 #     parser.add_argument('--batch_size', type=int, default=16, help='number of instances in one mini-batch.')
```

### Comparing `alethiometer-1.1.1/alethiometer/zero_cost_metrics/zen.py` & `alethiometer-1.1.2/alethiometer/zero_cost_metrics/zen.py`

 * *Files identical despite different names*

### Comparing `alethiometer-1.1.1/alethiometer/zero_cost_metrics/zico.py` & `alethiometer-1.1.2/alethiometer/zero_cost_metrics/zico.py`

 * *Files identical despite different names*

### Comparing `alethiometer-1.1.1/alethiometer.egg-info/PKG-INFO` & `alethiometer-1.1.2/alethiometer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alethiometer
-Version: 1.1.1
+Version: 1.1.2
 Summary: ZC proxies calculation repo, altered from foresight package.
 Home-page: https://github.com/iViolinSolo/zero-cost-proxies
 Author: ViolinSolo
 Author-email: i.violinsolo@gmail.com
 License: Apache Software License
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
@@ -16,15 +16,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 <!--
  * @Author: ViolinSolo
  * @Date: 2023-03-26 10:11:01
- * @LastEditTime: 2023-05-05 17:15:45
+ * @LastEditTime: 2023-05-06 10:28:20
  * @LastEditors: ViolinSolo
  * @Description: Readme
  * @FilePath: /zero-cost-proxies/README.md
 -->
 # zero-cost-proxies
 Independent ZC proxies only for testing on it. 
 
@@ -64,14 +64,16 @@
 = lrn,                                                  = 
 =-------------------------------------------------------=
 = zico, not work in torch-cpu, I will check it later.   =
 =     zico must use at least two batches of data,       =
 =     in order to calculate cross-batch (non-zero) std  =
 =-------------------------------------------------------=
 = tcet,                                                 =
+= snr-synflow,                                          =
+= snr-snip,                                             =
 =========================================================
 ```
 
 ## 0. How to install.
 1. First create conda env with python version >= 3.6, this repo has been completely tested on python 3.9.  
     ```bash
     conda install pytorch==1.13.1 torchvision==0.14.1 torchaudio==0.13.1 pytorch-cuda=11.6 -c pytorch -c nvidia
@@ -105,14 +107,16 @@
 ## 1. Tests
 ImageNet16-120 cannot be automatically downloaded. Using script under `scripts/download_data.sh` to download:
 ```bash
 source scripts/download_data.sh nb201 ImageNet16-120
 # do not use `bash`, use `source` instead
 ```
 ## 2. Versions
+- V1.1.2  
+Fix bug in `tenas`, add net instance deep copy to avoid weight changes.
 - V1.1.1  
 Fix warnings in `tenas`, now using new torch api to calc eigenvalue.  
 Fix bug in `tcet`, add net instance deep copy to avoid weight changes, add manually designed `tcet` copy process, remove bn in synflow, add bn in snip.
 - V1.1.0  
 Add `tcet` metric, which calculates TCET score.
 Add `snr` metrics, which calculates SNR family scores.
 - V1.0.10
```

### Comparing `alethiometer-1.1.1/alethiometer.egg-info/SOURCES.txt` & `alethiometer-1.1.2/alethiometer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alethiometer-1.1.1/setup.py` & `alethiometer-1.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `alethiometer-1.1.1/tests/test_nwot_api.py` & `alethiometer-1.1.2/tests/test_nwot_api.py`

 * *Files identical despite different names*

### Comparing `alethiometer-1.1.1/tests/test_tcet.py` & `alethiometer-1.1.2/tests/test_tcet.py`

 * *Files identical despite different names*

### Comparing `alethiometer-1.1.1/tests/test_zc.py` & `alethiometer-1.1.2/tests/test_zc.py`

 * *Files identical despite different names*

### Comparing `alethiometer-1.1.1/tests/test_zico.py` & `alethiometer-1.1.2/tests/test_zico.py`

 * *Files identical despite different names*

