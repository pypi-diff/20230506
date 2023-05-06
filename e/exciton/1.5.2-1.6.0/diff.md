# Comparing `tmp/exciton-1.5.2-py3-none-any.whl.zip` & `tmp/exciton-1.6.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 54651 bytes, number of entries: 57
+Zip file size: 57281 bytes, number of entries: 60
 -rw-rw-r--  2.0 unx        0 b- defN 23-Mar-11 03:14 exciton/__init__.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Mar-11 03:14 exciton/ml/__init__.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Mar-26 00:50 exciton/ml/classification/__init__.py
 -rw-rw-r--  2.0 unx     1461 b- defN 23-Mar-26 01:24 exciton/ml/classification/utils.py
 -rw-rw-r--  2.0 unx       98 b- defN 23-Mar-26 03:49 exciton/ml/classification/bert/__init__.py
 -rw-rw-r--  2.0 unx     5860 b- defN 23-Mar-29 15:08 exciton/ml/classification/bert/model.py
 -rw-rw-r--  2.0 unx     1966 b- defN 23-Mar-29 14:55 exciton/ml/classification/bert/trainer.py
@@ -28,32 +28,35 @@
 -rw-rw-r--  2.0 unx       85 b- defN 23-Mar-23 01:29 exciton/ml/tagging/xlmroberta/__init__.py
 -rw-rw-r--  2.0 unx     5536 b- defN 23-Mar-24 13:01 exciton/ml/tagging/xlmroberta/model.py
 -rw-rw-r--  2.0 unx     2407 b- defN 23-Mar-23 01:31 exciton/ml/tagging/xlmroberta/trainer.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Mar-11 03:13 exciton/nlp/__init__.py
 -rw-rw-r--  2.0 unx       56 b- defN 23-Mar-27 15:43 exciton/nlp/event_detection/__init__.py
 -rw-rw-r--  2.0 unx     3880 b- defN 23-Mar-27 20:00 exciton/nlp/event_detection/bert.py
 -rw-rw-r--  2.0 unx     2794 b- defN 23-Mar-27 20:00 exciton/nlp/event_detection/utils.py
+-rw-rw-r--  2.0 unx       87 b- defN 23-May-06 01:54 exciton/nlp/lang_detection/__init__.py
+-rw-rw-r--  2.0 unx     2417 b- defN 23-May-06 02:02 exciton/nlp/lang_detection/exciton_detection.py
 -rw-rw-r--  2.0 unx      103 b- defN 23-Mar-29 04:15 exciton/nlp/named_entity_recognition/__init__.py
 -rw-rw-r--  2.0 unx     3980 b- defN 23-Apr-26 01:32 exciton/nlp/named_entity_recognition/bert.py
 -rw-rw-r--  2.0 unx     1479 b- defN 23-Mar-24 15:07 exciton/nlp/named_entity_recognition/spacy.py
 -rw-rw-r--  2.0 unx     2942 b- defN 23-Mar-29 02:24 exciton/nlp/named_entity_recognition/utils.py
 -rw-rw-r--  2.0 unx     7039 b- defN 23-Apr-22 11:32 exciton/nlp/named_entity_recognition/xlm_hrl.py
 -rw-rw-r--  2.0 unx     3852 b- defN 23-Mar-24 16:02 exciton/nlp/named_entity_recognition/xlmroberta.py
 -rw-rw-r--  2.0 unx      110 b- defN 23-Mar-23 03:01 exciton/nlp/named_entity_recogonition/__init__.py
 -rw-rw-r--  2.0 unx     3779 b- defN 23-Mar-22 23:36 exciton/nlp/named_entity_recogonition/bert.py
 -rw-rw-r--  2.0 unx     3782 b- defN 23-Mar-22 19:09 exciton/nlp/named_entity_recogonition/service.py
 -rw-rw-r--  2.0 unx     3192 b- defN 23-Mar-23 02:02 exciton/nlp/named_entity_recogonition/utils.py
 -rw-rw-r--  2.0 unx     3876 b- defN 23-Mar-23 02:49 exciton/nlp/named_entity_recogonition/xlmroberta.py
--rw-rw-r--  2.0 unx       55 b- defN 23-Mar-16 02:32 exciton/nlp/sentence_tokenizer/__init__.py
+-rw-rw-r--  2.0 unx       59 b- defN 23-May-05 01:21 exciton/nlp/sentence_tokenizer/__init__.py
+-rw-rw-r--  2.0 unx     3977 b- defN 23-May-02 03:18 exciton/nlp/sentence_tokenizer/exciton_sbd.py
 -rw-rw-r--  2.0 unx     3977 b- defN 23-May-02 03:18 exciton/nlp/sentence_tokenizer/service.py
 -rw-rw-r--  2.0 unx       84 b- defN 23-May-01 15:45 exciton/nlp/text_matching/__init__.py
 -rw-rw-r--  2.0 unx     2562 b- defN 23-May-01 17:44 exciton/nlp/text_matching/exciton_matching.py
 -rw-rw-r--  2.0 unx       50 b- defN 23-Mar-12 04:02 exciton/nlp/translation/__init__.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Mar-11 23:23 exciton/nlp/translation/m2m100/__init__.py
 -rw-rw-r--  2.0 unx     4289 b- defN 23-Apr-22 11:14 exciton/nlp/translation/m2m100/service.py
 -rw-rw-r--  2.0 unx     2172 b- defN 23-Mar-12 03:47 exciton/nlp/translation/m2m100/utils.py
--rw-r--r--  2.0 unx    11417 b- defN 23-May-02 03:19 exciton-1.5.2.dist-info/LICENSE
--rw-rw-r--  2.0 unx     1598 b- defN 23-May-02 03:19 exciton-1.5.2.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-02 03:19 exciton-1.5.2.dist-info/WHEEL
--rw-rw-r--  2.0 unx        8 b- defN 23-May-02 03:19 exciton-1.5.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     5285 b- defN 23-May-02 03:19 exciton-1.5.2.dist-info/RECORD
-57 files, 145166 bytes uncompressed, 46029 bytes compressed:  68.3%
+-rw-r--r--  2.0 unx    11417 b- defN 23-May-06 02:05 exciton-1.6.0.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     1598 b- defN 23-May-06 02:05 exciton-1.6.0.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-06 02:05 exciton-1.6.0.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        8 b- defN 23-May-06 02:05 exciton-1.6.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     5584 b- defN 23-May-06 02:05 exciton-1.6.0.dist-info/RECORD
+60 files, 151950 bytes uncompressed, 48171 bytes compressed:  68.3%
```

## zipnote {}

```diff
@@ -93,14 +93,20 @@
 
 Filename: exciton/nlp/event_detection/bert.py
 Comment: 
 
 Filename: exciton/nlp/event_detection/utils.py
 Comment: 
 
+Filename: exciton/nlp/lang_detection/__init__.py
+Comment: 
+
+Filename: exciton/nlp/lang_detection/exciton_detection.py
+Comment: 
+
 Filename: exciton/nlp/named_entity_recognition/__init__.py
 Comment: 
 
 Filename: exciton/nlp/named_entity_recognition/bert.py
 Comment: 
 
 Filename: exciton/nlp/named_entity_recognition/spacy.py
@@ -129,14 +135,17 @@
 
 Filename: exciton/nlp/named_entity_recogonition/xlmroberta.py
 Comment: 
 
 Filename: exciton/nlp/sentence_tokenizer/__init__.py
 Comment: 
 
+Filename: exciton/nlp/sentence_tokenizer/exciton_sbd.py
+Comment: 
+
 Filename: exciton/nlp/sentence_tokenizer/service.py
 Comment: 
 
 Filename: exciton/nlp/text_matching/__init__.py
 Comment: 
 
 Filename: exciton/nlp/text_matching/exciton_matching.py
@@ -150,23 +159,23 @@
 
 Filename: exciton/nlp/translation/m2m100/service.py
 Comment: 
 
 Filename: exciton/nlp/translation/m2m100/utils.py
 Comment: 
 
-Filename: exciton-1.5.2.dist-info/LICENSE
+Filename: exciton-1.6.0.dist-info/LICENSE
 Comment: 
 
-Filename: exciton-1.5.2.dist-info/METADATA
+Filename: exciton-1.6.0.dist-info/METADATA
 Comment: 
 
-Filename: exciton-1.5.2.dist-info/WHEEL
+Filename: exciton-1.6.0.dist-info/WHEEL
 Comment: 
 
-Filename: exciton-1.5.2.dist-info/top_level.txt
+Filename: exciton-1.6.0.dist-info/top_level.txt
 Comment: 
 
-Filename: exciton-1.5.2.dist-info/RECORD
+Filename: exciton-1.6.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## exciton/nlp/sentence_tokenizer/__init__.py

```diff
@@ -1,2 +1,2 @@
 # flake8: noqa
-from .service import Sentence_Tokenizer
+from .exciton_sbd import Sentence_Tokenizer
```

## Comparing `exciton-1.5.2.dist-info/LICENSE` & `exciton-1.6.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `exciton-1.5.2.dist-info/METADATA` & `exciton-1.6.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exciton
-Version: 1.5.2
+Version: 1.6.0
 Summary: Domain-specific Natural Language Processing with exciton
 Home-page: https://exciton.com
 Author: The ExcitonX Team
 Author-email: excitonx@gmail.com
 License: UNKNOWN
 Keywords: exciton NLP Deep Learning
 Platform: UNKNOWN
```

## Comparing `exciton-1.5.2.dist-info/RECORD` & `exciton-1.6.0.dist-info/RECORD`

 * *Files 7% similar despite different names*

```diff
@@ -27,31 +27,34 @@
 exciton/ml/tagging/xlmroberta/__init__.py,sha256=gW7BwstJPJ-io9ALYvgRxuV4mCjNzISYkC57EhfWnSQ,85
 exciton/ml/tagging/xlmroberta/model.py,sha256=ftiQz67oXA__KPcJXKJrU0qkr0DwPRyfXhYy0cq1zWQ,5536
 exciton/ml/tagging/xlmroberta/trainer.py,sha256=e-oFF7RZU77_M2BSjrN960d7wjvTX-TtLX6wUJR4fEI,2407
 exciton/nlp/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 exciton/nlp/event_detection/__init__.py,sha256=FtWq9rkjsaiONszetzyC4FfMmrdPnaLyaZUFV5jjFuY,56
 exciton/nlp/event_detection/bert.py,sha256=YlYlOwVgP0i-oaAyyuMaSRhLrbAusJY_oZFprTtS1dc,3880
 exciton/nlp/event_detection/utils.py,sha256=tB3xz3d1NPl_kqckKPsdioVVQov9nYaR9mIeoNlZHY4,2794
+exciton/nlp/lang_detection/__init__.py,sha256=27sbeph7FR7Zka5kdrOnuGaG3bqNntj4ZZlMgVq5bAg,87
+exciton/nlp/lang_detection/exciton_detection.py,sha256=h87wXeuo9ftnWvDpeRzfSbHpND8z7N5LROhvUdS-h2s,2417
 exciton/nlp/named_entity_recognition/__init__.py,sha256=5TDJAZbbyW3LCtFSn0dFfRg9qIYYnC4G_ipR61o48jw,103
 exciton/nlp/named_entity_recognition/bert.py,sha256=quGAtehmxcjvaHUS9fke4VoPUysBXTOUffvaMgIQ58c,3980
 exciton/nlp/named_entity_recognition/spacy.py,sha256=ty2au1Mxk-12pN-X4PSroPCe4EfasNXSopGq5IH0P9g,1479
 exciton/nlp/named_entity_recognition/utils.py,sha256=9FSHdPhuBBn1tzZL_c22PVDOA002pmSzGDWXuCIn4C8,2942
 exciton/nlp/named_entity_recognition/xlm_hrl.py,sha256=7KZwR6vDDGlWvL1IziTQfJNoxvrI7o4RKb7cjnDNOe8,7039
 exciton/nlp/named_entity_recognition/xlmroberta.py,sha256=6KOEGAvv8j1leK9MFIB8cW22nnU3lVM79zlae_qJizc,3852
 exciton/nlp/named_entity_recogonition/__init__.py,sha256=gC16LpmP1h04d4QdzP7z5hSyul7EUkS3WE0lJC-1dK4,110
 exciton/nlp/named_entity_recogonition/bert.py,sha256=UZbWOJTqBADH5dGRV56uMn6mdW7hUouvfTZ7NqIiqKg,3779
 exciton/nlp/named_entity_recogonition/service.py,sha256=hb9VxtZ_eiF578oC621Wu5jU5TgaZ-fzOzKf6EjU3NY,3782
 exciton/nlp/named_entity_recogonition/utils.py,sha256=0GaerSJudvinee0rxL6zRtrSOhvGSUzbNoNci7KTzl4,3192
 exciton/nlp/named_entity_recogonition/xlmroberta.py,sha256=av4mSyZ5DNaN0KmmpEw4WkzGsrgupR8X0FiU1cdA4dw,3876
-exciton/nlp/sentence_tokenizer/__init__.py,sha256=yCvDHfXDtN24vbQWjSyAbESSw5c0Qh26EdheavCc_vk,55
+exciton/nlp/sentence_tokenizer/__init__.py,sha256=1hIgq6ayPk2yVdhBgLHe5vXxU2fcDrenz51iKXhx28s,59
+exciton/nlp/sentence_tokenizer/exciton_sbd.py,sha256=3Ssq2UNmhDCezhBJq4V8csacA_0XenYmgPLZfmBtBYc,3977
 exciton/nlp/sentence_tokenizer/service.py,sha256=3Ssq2UNmhDCezhBJq4V8csacA_0XenYmgPLZfmBtBYc,3977
 exciton/nlp/text_matching/__init__.py,sha256=tgQvyWZupI0QAHlnLAJldpOPBCF01OFq2poLH49tAVg,84
 exciton/nlp/text_matching/exciton_matching.py,sha256=Co3l9H_HH5dx_IlOlUL8j1jrbsMOfvP-F9TmpXj2SBs,2562
 exciton/nlp/translation/__init__.py,sha256=gE0YV-s4pB7VQWdsg04hALOBBpuWaQ3AUqpY9rvgI_8,50
 exciton/nlp/translation/m2m100/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 exciton/nlp/translation/m2m100/service.py,sha256=5YlJWxetgB7sIE-93Wsa-3ngJBqCPsqifpPim1oHag4,4289
 exciton/nlp/translation/m2m100/utils.py,sha256=GE8qg2deaHBMVMIHS32Hb5TCxO453kuncQrdJsnRIoU,2172
-exciton-1.5.2.dist-info/LICENSE,sha256=eaaQRm1hnsFuOwXep1_FkcP0t2c5T_wkOJknzzhxf2U,11417
-exciton-1.5.2.dist-info/METADATA,sha256=zZpmxsv0ph2Sz_RApPEIRf10hZ6EwTapNGujcEVoxAo,1598
-exciton-1.5.2.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-exciton-1.5.2.dist-info/top_level.txt,sha256=4a5H-nIPFHu7soZB2r0pfjYuciFSwQFnkl5PhaaT4pY,8
-exciton-1.5.2.dist-info/RECORD,,
+exciton-1.6.0.dist-info/LICENSE,sha256=eaaQRm1hnsFuOwXep1_FkcP0t2c5T_wkOJknzzhxf2U,11417
+exciton-1.6.0.dist-info/METADATA,sha256=Fsq1s7Mi5rRFib1L_nH_3q3Dw7hmZOO4aVHbcQvdnNs,1598
+exciton-1.6.0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+exciton-1.6.0.dist-info/top_level.txt,sha256=4a5H-nIPFHu7soZB2r0pfjYuciFSwQFnkl5PhaaT4pY,8
+exciton-1.6.0.dist-info/RECORD,,
```

