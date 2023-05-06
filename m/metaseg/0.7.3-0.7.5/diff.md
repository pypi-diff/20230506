# Comparing `tmp/metaseg-0.7.3.tar.gz` & `tmp/metaseg-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metaseg-0.7.3.tar", last modified: Tue Apr 25 08:40:39 2023, max compression
+gzip compressed data, was "metaseg-0.7.5.tar", last modified: Sat May  6 11:09:44 2023, max compression
```

## Comparing `metaseg-0.7.3.tar` & `metaseg-0.7.5.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-25 08:40:39.278399 metaseg-0.7.3/
--rw-r--r--   0 kadir     (1000) kadir     (1001)    11357 2023-04-20 11:50:36.000000 metaseg-0.7.3/LICENSE
--rw-r--r--   0 kadir     (1000) kadir     (1001)       24 2023-04-20 11:50:36.000000 metaseg-0.7.3/MANIFEST.in
--rw-r--r--   0 kadir     (1000) kadir     (1001)     4419 2023-04-25 08:40:39.278399 metaseg-0.7.3/PKG-INFO
--rw-r--r--   0 kadir     (1000) kadir     (1001)     4145 2023-04-23 14:51:06.000000 metaseg-0.7.3/README.md
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-25 08:40:39.271732 metaseg-0.7.3/metaseg/
--rw-r--r--   0 kadir     (1000) kadir     (1001)      707 2023-04-25 08:40:22.000000 metaseg-0.7.3/metaseg/__init__.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     2847 2023-04-25 08:37:15.000000 metaseg-0.7.3/metaseg/falai_demo.py
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-25 08:40:39.275065 metaseg-0.7.3/metaseg/generator/
--rw-r--r--   0 kadir     (1000) kadir     (1001)        0 2023-04-20 11:50:36.000000 metaseg-0.7.3/metaseg/generator/__init__.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)    15127 2023-04-20 11:50:36.000000 metaseg-0.7.3/metaseg/generator/automatic_mask_generator.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     2936 2023-04-20 11:50:36.000000 metaseg-0.7.3/metaseg/generator/build_sam.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)    11570 2023-04-20 11:50:36.000000 metaseg-0.7.3/metaseg/generator/predictor.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     8162 2023-04-25 08:39:32.000000 metaseg-0.7.3/metaseg/mask_predictor.py
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-25 08:40:39.278399 metaseg-0.7.3/metaseg/modeling/
--rw-r--r--   0 kadir     (1000) kadir     (1001)      465 2023-04-20 11:50:36.000000 metaseg-0.7.3/metaseg/modeling/__init__.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     1479 2023-04-20 11:50:36.000000 metaseg-0.7.3/metaseg/modeling/common.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)    14341 2023-04-20 11:50:36.000000 metaseg-0.7.3/metaseg/modeling/image_encoder.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     6540 2023-04-20 11:50:36.000000 metaseg-0.7.3/metaseg/modeling/mask_decoder.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     8596 2023-04-20 11:50:36.000000 metaseg-0.7.3/metaseg/modeling/prompt_encoder.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     7273 2023-04-20 11:50:36.000000 metaseg-0.7.3/metaseg/modeling/sam.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     8332 2023-04-20 11:50:36.000000 metaseg-0.7.3/metaseg/modeling/transformer.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     3515 2023-04-20 11:50:36.000000 metaseg-0.7.3/metaseg/sahi_predict.py
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-25 08:40:39.278399 metaseg-0.7.3/metaseg/utils/
--rw-r--r--   0 kadir     (1000) kadir     (1001)      276 2023-04-20 11:50:36.000000 metaseg-0.7.3/metaseg/utils/__init__.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)    12621 2023-04-20 11:50:36.000000 metaseg-0.7.3/metaseg/utils/amg.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     2807 2023-04-23 14:10:49.000000 metaseg-0.7.3/metaseg/utils/data_utils.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     1231 2023-04-20 11:50:36.000000 metaseg-0.7.3/metaseg/utils/file_utils.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     5743 2023-04-20 11:50:36.000000 metaseg-0.7.3/metaseg/utils/onnx.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     3874 2023-04-20 11:50:36.000000 metaseg-0.7.3/metaseg/utils/transforms.py
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-25 08:40:39.278399 metaseg-0.7.3/metaseg/webapp/
--rw-r--r--   0 kadir     (1000) kadir     (1001)        0 2023-04-20 11:50:36.000000 metaseg-0.7.3/metaseg/webapp/__init__.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     8416 2023-04-20 11:50:36.000000 metaseg-0.7.3/metaseg/webapp/app.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     2470 2023-04-20 11:50:36.000000 metaseg-0.7.3/metaseg/webapp/demo.py
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-25 08:40:39.271732 metaseg-0.7.3/metaseg.egg-info/
--rw-r--r--   0 kadir     (1000) kadir     (1001)     4419 2023-04-25 08:40:39.000000 metaseg-0.7.3/metaseg.egg-info/PKG-INFO
--rw-r--r--   0 kadir     (1000) kadir     (1001)      903 2023-04-25 08:40:39.000000 metaseg-0.7.3/metaseg.egg-info/SOURCES.txt
--rw-r--r--   0 kadir     (1000) kadir     (1001)        1 2023-04-25 08:40:39.000000 metaseg-0.7.3/metaseg.egg-info/dependency_links.txt
--rw-r--r--   0 kadir     (1000) kadir     (1001)      183 2023-04-25 08:40:39.000000 metaseg-0.7.3/metaseg.egg-info/requires.txt
--rw-r--r--   0 kadir     (1000) kadir     (1001)        8 2023-04-25 08:40:39.000000 metaseg-0.7.3/metaseg.egg-info/top_level.txt
--rw-r--r--   0 kadir     (1000) kadir     (1001)       80 2023-04-20 11:50:36.000000 metaseg-0.7.3/pyproject.toml
--rw-r--r--   0 kadir     (1000) kadir     (1001)      158 2023-04-23 14:51:06.000000 metaseg-0.7.3/requirements.txt
--rw-r--r--   0 kadir     (1000) kadir     (1001)      430 2023-04-25 08:40:39.281732 metaseg-0.7.3/setup.cfg
--rw-r--r--   0 kadir     (1000) kadir     (1001)     1529 2023-04-21 13:07:40.000000 metaseg-0.7.3/setup.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-05-06 11:09:44.526430 metaseg-0.7.5/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)    11357 2023-05-06 11:05:04.000000 metaseg-0.7.5/LICENSE
+-rw-r--r--   0 kadir     (1000) kadir     (1001)       24 2023-05-06 11:05:04.000000 metaseg-0.7.5/MANIFEST.in
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     4491 2023-05-06 11:09:44.526430 metaseg-0.7.5/PKG-INFO
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     4217 2023-05-06 11:06:51.000000 metaseg-0.7.5/README.md
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-05-06 11:09:44.523097 metaseg-0.7.5/metaseg/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      556 2023-05-06 11:09:28.000000 metaseg-0.7.5/metaseg/__init__.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     2848 2023-05-06 11:09:38.000000 metaseg-0.7.5/metaseg/falai_demo.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-05-06 11:09:44.523097 metaseg-0.7.5/metaseg/generator/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)        0 2023-05-06 11:05:04.000000 metaseg-0.7.5/metaseg/generator/__init__.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)    15127 2023-05-06 11:05:04.000000 metaseg-0.7.5/metaseg/generator/automatic_mask_generator.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     2936 2023-05-06 11:05:04.000000 metaseg-0.7.5/metaseg/generator/build_sam.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)    11570 2023-05-06 11:05:04.000000 metaseg-0.7.5/metaseg/generator/predictor.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     8161 2023-05-06 11:09:38.000000 metaseg-0.7.5/metaseg/mask_predictor.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-05-06 11:09:44.526430 metaseg-0.7.5/metaseg/modeling/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      465 2023-05-06 11:05:04.000000 metaseg-0.7.5/metaseg/modeling/__init__.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     1479 2023-05-06 11:05:04.000000 metaseg-0.7.5/metaseg/modeling/common.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)    14341 2023-05-06 11:05:04.000000 metaseg-0.7.5/metaseg/modeling/image_encoder.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     6540 2023-05-06 11:05:04.000000 metaseg-0.7.5/metaseg/modeling/mask_decoder.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     8596 2023-05-06 11:05:04.000000 metaseg-0.7.5/metaseg/modeling/prompt_encoder.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     7273 2023-05-06 11:05:04.000000 metaseg-0.7.5/metaseg/modeling/sam.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     8332 2023-05-06 11:05:04.000000 metaseg-0.7.5/metaseg/modeling/transformer.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     3515 2023-05-06 11:05:04.000000 metaseg-0.7.5/metaseg/sahi_predict.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-05-06 11:09:44.526430 metaseg-0.7.5/metaseg/utils/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      276 2023-05-06 11:05:04.000000 metaseg-0.7.5/metaseg/utils/__init__.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)    12621 2023-05-06 11:05:04.000000 metaseg-0.7.5/metaseg/utils/amg.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     2807 2023-05-06 11:05:04.000000 metaseg-0.7.5/metaseg/utils/data_utils.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     1231 2023-05-06 11:05:04.000000 metaseg-0.7.5/metaseg/utils/file_utils.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     5743 2023-05-06 11:05:04.000000 metaseg-0.7.5/metaseg/utils/onnx.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     3874 2023-05-06 11:05:04.000000 metaseg-0.7.5/metaseg/utils/transforms.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-05-06 11:09:44.526430 metaseg-0.7.5/metaseg/webapp/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)        0 2023-05-06 11:05:04.000000 metaseg-0.7.5/metaseg/webapp/__init__.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     8416 2023-05-06 11:05:04.000000 metaseg-0.7.5/metaseg/webapp/app.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     2470 2023-05-06 11:05:04.000000 metaseg-0.7.5/metaseg/webapp/demo.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-05-06 11:09:44.523097 metaseg-0.7.5/metaseg.egg-info/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     4491 2023-05-06 11:09:44.000000 metaseg-0.7.5/metaseg.egg-info/PKG-INFO
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      903 2023-05-06 11:09:44.000000 metaseg-0.7.5/metaseg.egg-info/SOURCES.txt
+-rw-r--r--   0 kadir     (1000) kadir     (1001)        1 2023-05-06 11:09:44.000000 metaseg-0.7.5/metaseg.egg-info/dependency_links.txt
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      183 2023-05-06 11:09:44.000000 metaseg-0.7.5/metaseg.egg-info/requires.txt
+-rw-r--r--   0 kadir     (1000) kadir     (1001)        8 2023-05-06 11:09:44.000000 metaseg-0.7.5/metaseg.egg-info/top_level.txt
+-rw-r--r--   0 kadir     (1000) kadir     (1001)       80 2023-05-06 11:05:04.000000 metaseg-0.7.5/pyproject.toml
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      158 2023-05-06 11:09:17.000000 metaseg-0.7.5/requirements.txt
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      430 2023-05-06 11:09:44.529764 metaseg-0.7.5/setup.cfg
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     1529 2023-05-06 11:05:04.000000 metaseg-0.7.5/setup.py
```

### Comparing `metaseg-0.7.3/LICENSE` & `metaseg-0.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `metaseg-0.7.3/PKG-INFO` & `metaseg-0.7.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: metaseg
-Version: 0.7.3
-Home-page: https://github.com/kadirnar/segment-anything-pip
-Author: kadirnar
-License: Apache-2.0
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: all
-Provides-Extra: dev
-License-File: LICENSE
-
 <div align="center">
 <h2>
      MetaSeg: Packaged version of the Segment Anything repository
 </h2>
 <div>
     <img width="1000" alt="teaser" src="https://github.com/kadirnar/segment-anything-pip/releases/download/v0.2.2/metaseg_demo.gif">
 </div>
@@ -86,15 +74,15 @@
     output_path="output.mp4",
 )
 ```
 
 ### [SAHI](https://github.com/obss/sahi) + Segment Anything
 
 ```python
-from metaseg import sahi_sliced_predict, SahiAutoSegmentation
+from metaseg.sahi_predict import SahiAutoSegmentation, sahi_sliced_predict
 
 image_path = "test.jpg"
 boxes = sahi_sliced_predict(
     image_path=image_path,
     detection_model_type="yolov5", #yolov8, detectron2, mmdetection, torchvision
     detection_model_path="yolov5l6.pt",
     conf_th=0.25,
@@ -116,14 +104,15 @@
 )
 ```
 <img width="700" alt="teaser" src="https://github.com/kadirnar/segment-anything-pip/releases/download/v0.5.0/sahi_autoseg.png">
 
 ### [FalAI(Cloud GPU)](https://docs.fal.ai/fal-serverless/quickstart) + Segment Anything
 ```bash
 pip install fal_serverless
+fal-serverless auth login
 ```
 
 ```python
 # For Auto Mask
 from metaseg import falai_automask_image
 
 image = falai_automask_image(
@@ -133,15 +122,15 @@
     points_per_batch=32,
     min_area=0,
 )   
 image.show() # Show image
 image.save("output.jpg") # Save image
 
 # For Manual Mask
-from metaseg import falai_manualmask_image
+from metaseg.falai_demo import falai_automask_image, falai_manuelmask_image
 
 image = falai_manualmask_image(
     image_path="data.jpg",
     model_type="vit_b",
     input_point=[[100, 100], [200, 200]],
     input_label=[0, 1],
     input_box=[100, 100, 200, 200], # or [[100, 100, 200, 200], [100, 100, 200, 200]]
```

#### html2text {}

```diff
@@ -1,11 +1,7 @@
-Metadata-Version: 2.1 Name: metaseg Version: 0.7.3 Home-page: https://
-github.com/kadirnar/segment-anything-pip Author: kadirnar License: Apache-2.0
-Requires-Python: >=3.8 Description-Content-Type: text/markdown Provides-Extra:
-all Provides-Extra: dev License-File: LICENSE
    ***** MetaSeg: Packaged version of the Segment Anything repository *****
                                    [teaser]
                 [downloads] [pypi_version] [HuggingFace_Spaces]
 This repo is a packaged version of the [segment-anything](https://github.com/
 facebookresearch/segment-anything) model. ### Installation ```bash pip install
 metaseg ``` ### Usage ```python from metaseg import SegAutoMaskPredictor,
 SegManualMaskPredictor # If gpu memory is not enough, reduce the
@@ -20,29 +16,30 @@
 model_type="vit_l", # vit_l, vit_h, vit_b input_point=[[100, 100], [200, 200]],
 input_label=[0, 1], input_box=[100, 100, 200, 200], # or [[100, 100, 200, 200],
 [100, 100, 200, 200]] multimask_output=False, random_color=False, show=True,
 save=False, ) # For video results = SegManualMaskPredictor().video_predict
 ( source="test.mp4", model_type="vit_l", # vit_l, vit_h, vit_b input_point=[0,
 0, 100, 100] input_label=[0, 1], input_box=None, multimask_output=False,
 random_color=False, output_path="output.mp4", ) ``` ### [SAHI](https://
-github.com/obss/sahi) + Segment Anything ```python from metaseg import
-sahi_sliced_predict, SahiAutoSegmentation image_path = "test.jpg" boxes =
-sahi_sliced_predict( image_path=image_path, detection_model_type="yolov5",
+github.com/obss/sahi) + Segment Anything ```python from metaseg.sahi_predict
+import SahiAutoSegmentation, sahi_sliced_predict image_path = "test.jpg" boxes
+= sahi_sliced_predict( image_path=image_path, detection_model_type="yolov5",
 #yolov8, detectron2, mmdetection, torchvision
 detection_model_path="yolov5l6.pt", conf_th=0.25, image_size=1280,
 slice_height=256, slice_width=256, overlap_height_ratio=0.2,
 overlap_width_ratio=0.2, ) SahiAutoSegmentation().predict( source=image_path,
 model_type="vit_b", input_box=boxes, multimask_output=False,
 random_color=False, show=True, save=False, ) ``` [teaser] ### [FalAI(Cloud
 GPU)](https://docs.fal.ai/fal-serverless/quickstart) + Segment Anything ```bash
-pip install fal_serverless ``` ```python # For Auto Mask from metaseg import
-falai_automask_image image = falai_automask_image( image_path="data.jpg",
-model_type="vit_b", points_per_side=16, points_per_batch=32, min_area=0, )
-image.show() # Show image image.save("output.jpg") # Save image # For Manual
-Mask from metaseg import falai_manualmask_image image = falai_manualmask_image
+pip install fal_serverless fal-serverless auth login ``` ```python # For Auto
+Mask from metaseg import falai_automask_image image = falai_automask_image
+( image_path="data.jpg", model_type="vit_b", points_per_side=16,
+points_per_batch=32, min_area=0, ) image.show() # Show image image.save
+("output.jpg") # Save image # For Manual Mask from metaseg.falai_demo import
+falai_automask_image, falai_manuelmask_image image = falai_manualmask_image
 ( image_path="data.jpg", model_type="vit_b", input_point=[[100, 100], [200,
 200]], input_label=[0, 1], input_box=[100, 100, 200, 200], # or [[100, 100,
 200, 200], [100, 100, 200, 200]] multimask_output=False, random_color=False, )
 image.show() # Show image image.save("output.jpg") # Save image ``` # Extra
 Features - [x] Support for Yolov5/8, Detectron2, Mmdetection, Torchvision
 models - [x] Support for video and web application(Huggingface Spaces) - [x]
 Support for manual single multi box and point selection - [x] Support for pip
```

### Comparing `metaseg-0.7.3/README.md` & `metaseg-0.7.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+Metadata-Version: 2.1
+Name: metaseg
+Version: 0.7.5
+Home-page: https://github.com/kadirnar/segment-anything-pip
+Author: kadirnar
+License: Apache-2.0
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: all
+Provides-Extra: dev
+License-File: LICENSE
+
 <div align="center">
 <h2>
      MetaSeg: Packaged version of the Segment Anything repository
 </h2>
 <div>
     <img width="1000" alt="teaser" src="https://github.com/kadirnar/segment-anything-pip/releases/download/v0.2.2/metaseg_demo.gif">
 </div>
@@ -74,15 +86,15 @@
     output_path="output.mp4",
 )
 ```
 
 ### [SAHI](https://github.com/obss/sahi) + Segment Anything
 
 ```python
-from metaseg import sahi_sliced_predict, SahiAutoSegmentation
+from metaseg.sahi_predict import SahiAutoSegmentation, sahi_sliced_predict
 
 image_path = "test.jpg"
 boxes = sahi_sliced_predict(
     image_path=image_path,
     detection_model_type="yolov5", #yolov8, detectron2, mmdetection, torchvision
     detection_model_path="yolov5l6.pt",
     conf_th=0.25,
@@ -104,14 +116,15 @@
 )
 ```
 <img width="700" alt="teaser" src="https://github.com/kadirnar/segment-anything-pip/releases/download/v0.5.0/sahi_autoseg.png">
 
 ### [FalAI(Cloud GPU)](https://docs.fal.ai/fal-serverless/quickstart) + Segment Anything
 ```bash
 pip install fal_serverless
+fal-serverless auth login
 ```
 
 ```python
 # For Auto Mask
 from metaseg import falai_automask_image
 
 image = falai_automask_image(
@@ -121,15 +134,15 @@
     points_per_batch=32,
     min_area=0,
 )   
 image.show() # Show image
 image.save("output.jpg") # Save image
 
 # For Manual Mask
-from metaseg import falai_manualmask_image
+from metaseg.falai_demo import falai_automask_image, falai_manuelmask_image
 
 image = falai_manualmask_image(
     image_path="data.jpg",
     model_type="vit_b",
     input_point=[[100, 100], [200, 200]],
     input_label=[0, 1],
     input_box=[100, 100, 200, 200], # or [[100, 100, 200, 200], [100, 100, 200, 200]]
```

#### html2text {}

```diff
@@ -1,7 +1,11 @@
+Metadata-Version: 2.1 Name: metaseg Version: 0.7.5 Home-page: https://
+github.com/kadirnar/segment-anything-pip Author: kadirnar License: Apache-2.0
+Requires-Python: >=3.8 Description-Content-Type: text/markdown Provides-Extra:
+all Provides-Extra: dev License-File: LICENSE
    ***** MetaSeg: Packaged version of the Segment Anything repository *****
                                    [teaser]
                 [downloads] [pypi_version] [HuggingFace_Spaces]
 This repo is a packaged version of the [segment-anything](https://github.com/
 facebookresearch/segment-anything) model. ### Installation ```bash pip install
 metaseg ``` ### Usage ```python from metaseg import SegAutoMaskPredictor,
 SegManualMaskPredictor # If gpu memory is not enough, reduce the
@@ -16,29 +20,30 @@
 model_type="vit_l", # vit_l, vit_h, vit_b input_point=[[100, 100], [200, 200]],
 input_label=[0, 1], input_box=[100, 100, 200, 200], # or [[100, 100, 200, 200],
 [100, 100, 200, 200]] multimask_output=False, random_color=False, show=True,
 save=False, ) # For video results = SegManualMaskPredictor().video_predict
 ( source="test.mp4", model_type="vit_l", # vit_l, vit_h, vit_b input_point=[0,
 0, 100, 100] input_label=[0, 1], input_box=None, multimask_output=False,
 random_color=False, output_path="output.mp4", ) ``` ### [SAHI](https://
-github.com/obss/sahi) + Segment Anything ```python from metaseg import
-sahi_sliced_predict, SahiAutoSegmentation image_path = "test.jpg" boxes =
-sahi_sliced_predict( image_path=image_path, detection_model_type="yolov5",
+github.com/obss/sahi) + Segment Anything ```python from metaseg.sahi_predict
+import SahiAutoSegmentation, sahi_sliced_predict image_path = "test.jpg" boxes
+= sahi_sliced_predict( image_path=image_path, detection_model_type="yolov5",
 #yolov8, detectron2, mmdetection, torchvision
 detection_model_path="yolov5l6.pt", conf_th=0.25, image_size=1280,
 slice_height=256, slice_width=256, overlap_height_ratio=0.2,
 overlap_width_ratio=0.2, ) SahiAutoSegmentation().predict( source=image_path,
 model_type="vit_b", input_box=boxes, multimask_output=False,
 random_color=False, show=True, save=False, ) ``` [teaser] ### [FalAI(Cloud
 GPU)](https://docs.fal.ai/fal-serverless/quickstart) + Segment Anything ```bash
-pip install fal_serverless ``` ```python # For Auto Mask from metaseg import
-falai_automask_image image = falai_automask_image( image_path="data.jpg",
-model_type="vit_b", points_per_side=16, points_per_batch=32, min_area=0, )
-image.show() # Show image image.save("output.jpg") # Save image # For Manual
-Mask from metaseg import falai_manualmask_image image = falai_manualmask_image
+pip install fal_serverless fal-serverless auth login ``` ```python # For Auto
+Mask from metaseg import falai_automask_image image = falai_automask_image
+( image_path="data.jpg", model_type="vit_b", points_per_side=16,
+points_per_batch=32, min_area=0, ) image.show() # Show image image.save
+("output.jpg") # Save image # For Manual Mask from metaseg.falai_demo import
+falai_automask_image, falai_manuelmask_image image = falai_manualmask_image
 ( image_path="data.jpg", model_type="vit_b", input_point=[[100, 100], [200,
 200]], input_label=[0, 1], input_box=[100, 100, 200, 200], # or [[100, 100,
 200, 200], [100, 100, 200, 200]] multimask_output=False, random_color=False, )
 image.show() # Show image image.save("output.jpg") # Save image ``` # Extra
 Features - [x] Support for Yolov5/8, Detectron2, Mmdetection, Torchvision
 models - [x] Support for video and web application(Huggingface Spaces) - [x]
 Support for manual single multi box and point selection - [x] Support for pip
```

### Comparing `metaseg-0.7.3/metaseg/__init__.py` & `metaseg-0.7.5/metaseg/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 
 # This source code is licensed under the license found in the
 # LICENSE file in the root directory of this source tree.
 
-from metaseg.falai_demo import falai_automask_image, falai_manuelmask_image
 from metaseg.generator.automatic_mask_generator import SamAutomaticMaskGenerator
 from metaseg.generator.build_sam import build_sam, build_sam_vit_b, build_sam_vit_h, build_sam_vit_l, sam_model_registry
 from metaseg.generator.predictor import SamPredictor
 from metaseg.mask_predictor import SegAutoMaskPredictor, SegManualMaskPredictor
-from metaseg.sahi_predict import SahiAutoSegmentation, sahi_sliced_predict
 
-__version__ = "0.7.3"
+__version__ = "0.7.5"
```

### Comparing `metaseg-0.7.3/metaseg/falai_demo.py` & `metaseg-0.7.5/metaseg/falai_demo.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,14 +25,15 @@
         save=True,
     )
     with open(output_path, "rb") as f:
         result = f.read()
 
     return result
 
+
 @isolated(requirements=["metaseg"], keep_alive=1800, machine_type="GPU-T4")
 def manuelmask_image(
     data,
     model_type="vit_b",
     input_point=[[100, 100], [200, 200]],
     input_label=[0, 1],
     input_box=[100, 100, 200, 200],
```

### Comparing `metaseg-0.7.3/metaseg/generator/automatic_mask_generator.py` & `metaseg-0.7.5/metaseg/generator/automatic_mask_generator.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.7.3/metaseg/generator/build_sam.py` & `metaseg-0.7.5/metaseg/generator/build_sam.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.7.3/metaseg/generator/predictor.py` & `metaseg-0.7.5/metaseg/generator/predictor.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.7.3/metaseg/mask_predictor.py` & `metaseg-0.7.5/metaseg/mask_predictor.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,17 +2,16 @@
 
 import cv2
 import numpy as np
 import torch
 from tqdm import tqdm
 
 from metaseg.generator.automatic_mask_generator import SamAutomaticMaskGenerator
-from metaseg.generator.predictor import SamPredictor
 from metaseg.generator.build_sam import sam_model_registry
-
+from metaseg.generator.predictor import SamPredictor
 from metaseg.utils import (
     download_model,
     load_box,
     load_image,
     load_mask,
     load_video,
     multi_boxes,
```

### Comparing `metaseg-0.7.3/metaseg/modeling/common.py` & `metaseg-0.7.5/metaseg/modeling/common.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.7.3/metaseg/modeling/image_encoder.py` & `metaseg-0.7.5/metaseg/modeling/image_encoder.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.7.3/metaseg/modeling/mask_decoder.py` & `metaseg-0.7.5/metaseg/modeling/mask_decoder.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.7.3/metaseg/modeling/prompt_encoder.py` & `metaseg-0.7.5/metaseg/modeling/prompt_encoder.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.7.3/metaseg/modeling/sam.py` & `metaseg-0.7.5/metaseg/modeling/sam.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.7.3/metaseg/modeling/transformer.py` & `metaseg-0.7.5/metaseg/modeling/transformer.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.7.3/metaseg/sahi_predict.py` & `metaseg-0.7.5/metaseg/sahi_predict.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.7.3/metaseg/utils/amg.py` & `metaseg-0.7.5/metaseg/utils/amg.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.7.3/metaseg/utils/data_utils.py` & `metaseg-0.7.5/metaseg/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.7.3/metaseg/utils/file_utils.py` & `metaseg-0.7.5/metaseg/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.7.3/metaseg/utils/onnx.py` & `metaseg-0.7.5/metaseg/utils/onnx.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.7.3/metaseg/utils/transforms.py` & `metaseg-0.7.5/metaseg/utils/transforms.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.7.3/metaseg/webapp/app.py` & `metaseg-0.7.5/metaseg/webapp/app.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.7.3/metaseg/webapp/demo.py` & `metaseg-0.7.5/metaseg/webapp/demo.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.7.3/metaseg.egg-info/PKG-INFO` & `metaseg-0.7.5/metaseg.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metaseg
-Version: 0.7.3
+Version: 0.7.5
 Home-page: https://github.com/kadirnar/segment-anything-pip
 Author: kadirnar
 License: Apache-2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: all
 Provides-Extra: dev
@@ -86,15 +86,15 @@
     output_path="output.mp4",
 )
 ```
 
 ### [SAHI](https://github.com/obss/sahi) + Segment Anything
 
 ```python
-from metaseg import sahi_sliced_predict, SahiAutoSegmentation
+from metaseg.sahi_predict import SahiAutoSegmentation, sahi_sliced_predict
 
 image_path = "test.jpg"
 boxes = sahi_sliced_predict(
     image_path=image_path,
     detection_model_type="yolov5", #yolov8, detectron2, mmdetection, torchvision
     detection_model_path="yolov5l6.pt",
     conf_th=0.25,
@@ -116,14 +116,15 @@
 )
 ```
 <img width="700" alt="teaser" src="https://github.com/kadirnar/segment-anything-pip/releases/download/v0.5.0/sahi_autoseg.png">
 
 ### [FalAI(Cloud GPU)](https://docs.fal.ai/fal-serverless/quickstart) + Segment Anything
 ```bash
 pip install fal_serverless
+fal-serverless auth login
 ```
 
 ```python
 # For Auto Mask
 from metaseg import falai_automask_image
 
 image = falai_automask_image(
@@ -133,15 +134,15 @@
     points_per_batch=32,
     min_area=0,
 )   
 image.show() # Show image
 image.save("output.jpg") # Save image
 
 # For Manual Mask
-from metaseg import falai_manualmask_image
+from metaseg.falai_demo import falai_automask_image, falai_manuelmask_image
 
 image = falai_manualmask_image(
     image_path="data.jpg",
     model_type="vit_b",
     input_point=[[100, 100], [200, 200]],
     input_label=[0, 1],
     input_box=[100, 100, 200, 200], # or [[100, 100, 200, 200], [100, 100, 200, 200]]
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: metaseg Version: 0.7.3 Home-page: https://
+Metadata-Version: 2.1 Name: metaseg Version: 0.7.5 Home-page: https://
 github.com/kadirnar/segment-anything-pip Author: kadirnar License: Apache-2.0
 Requires-Python: >=3.8 Description-Content-Type: text/markdown Provides-Extra:
 all Provides-Extra: dev License-File: LICENSE
    ***** MetaSeg: Packaged version of the Segment Anything repository *****
                                    [teaser]
                 [downloads] [pypi_version] [HuggingFace_Spaces]
 This repo is a packaged version of the [segment-anything](https://github.com/
@@ -20,29 +20,30 @@
 model_type="vit_l", # vit_l, vit_h, vit_b input_point=[[100, 100], [200, 200]],
 input_label=[0, 1], input_box=[100, 100, 200, 200], # or [[100, 100, 200, 200],
 [100, 100, 200, 200]] multimask_output=False, random_color=False, show=True,
 save=False, ) # For video results = SegManualMaskPredictor().video_predict
 ( source="test.mp4", model_type="vit_l", # vit_l, vit_h, vit_b input_point=[0,
 0, 100, 100] input_label=[0, 1], input_box=None, multimask_output=False,
 random_color=False, output_path="output.mp4", ) ``` ### [SAHI](https://
-github.com/obss/sahi) + Segment Anything ```python from metaseg import
-sahi_sliced_predict, SahiAutoSegmentation image_path = "test.jpg" boxes =
-sahi_sliced_predict( image_path=image_path, detection_model_type="yolov5",
+github.com/obss/sahi) + Segment Anything ```python from metaseg.sahi_predict
+import SahiAutoSegmentation, sahi_sliced_predict image_path = "test.jpg" boxes
+= sahi_sliced_predict( image_path=image_path, detection_model_type="yolov5",
 #yolov8, detectron2, mmdetection, torchvision
 detection_model_path="yolov5l6.pt", conf_th=0.25, image_size=1280,
 slice_height=256, slice_width=256, overlap_height_ratio=0.2,
 overlap_width_ratio=0.2, ) SahiAutoSegmentation().predict( source=image_path,
 model_type="vit_b", input_box=boxes, multimask_output=False,
 random_color=False, show=True, save=False, ) ``` [teaser] ### [FalAI(Cloud
 GPU)](https://docs.fal.ai/fal-serverless/quickstart) + Segment Anything ```bash
-pip install fal_serverless ``` ```python # For Auto Mask from metaseg import
-falai_automask_image image = falai_automask_image( image_path="data.jpg",
-model_type="vit_b", points_per_side=16, points_per_batch=32, min_area=0, )
-image.show() # Show image image.save("output.jpg") # Save image # For Manual
-Mask from metaseg import falai_manualmask_image image = falai_manualmask_image
+pip install fal_serverless fal-serverless auth login ``` ```python # For Auto
+Mask from metaseg import falai_automask_image image = falai_automask_image
+( image_path="data.jpg", model_type="vit_b", points_per_side=16,
+points_per_batch=32, min_area=0, ) image.show() # Show image image.save
+("output.jpg") # Save image # For Manual Mask from metaseg.falai_demo import
+falai_automask_image, falai_manuelmask_image image = falai_manualmask_image
 ( image_path="data.jpg", model_type="vit_b", input_point=[[100, 100], [200,
 200]], input_label=[0, 1], input_box=[100, 100, 200, 200], # or [[100, 100,
 200, 200], [100, 100, 200, 200]] multimask_output=False, random_color=False, )
 image.show() # Show image image.save("output.jpg") # Save image ``` # Extra
 Features - [x] Support for Yolov5/8, Detectron2, Mmdetection, Torchvision
 models - [x] Support for video and web application(Huggingface Spaces) - [x]
 Support for manual single multi box and point selection - [x] Support for pip
```

### Comparing `metaseg-0.7.3/metaseg.egg-info/SOURCES.txt` & `metaseg-0.7.5/metaseg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `metaseg-0.7.3/setup.py` & `metaseg-0.7.5/setup.py`

 * *Files identical despite different names*

