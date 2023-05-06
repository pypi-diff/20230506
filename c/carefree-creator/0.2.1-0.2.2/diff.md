# Comparing `tmp/carefree-creator-0.2.1.tar.gz` & `tmp/carefree-creator-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "carefree-creator-0.2.1.tar", last modified: Wed Apr  5 06:43:39 2023, max compression
+gzip compressed data, was "carefree-creator-0.2.2.tar", last modified: Sat May  6 05:30:48 2023, max compression
```

## Comparing `carefree-creator-0.2.1.tar` & `carefree-creator-0.2.2.tar`

### file list

```diff
@@ -1,42 +1,47 @@
-drwxrwxrwx   0        0        0        0 2023-04-05 06:43:39.168072 carefree-creator-0.2.1/
--rw-rw-rw-   0        0        0     1090 2022-10-31 07:20:41.000000 carefree-creator-0.2.1/LICENSE
--rw-rw-rw-   0        0        0      195 2023-04-05 06:43:03.000000 carefree-creator-0.2.1/MANIFEST.in
--rw-rw-rw-   0        0        0    40232 2023-04-05 06:43:39.168072 carefree-creator-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0    39930 2023-04-05 06:43:03.000000 carefree-creator-0.2.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-05 06:43:39.153476 carefree-creator-0.2.1/carefree_creator.egg-info/
--rw-rw-rw-   0        0        0    40232 2023-04-05 06:43:39.000000 carefree-creator-0.2.1/carefree_creator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      844 2023-04-05 06:43:39.000000 carefree-creator-0.2.1/carefree_creator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-05 06:43:39.000000 carefree-creator-0.2.1/carefree_creator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-04-05 06:43:39.000000 carefree-creator-0.2.1/carefree_creator.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      138 2023-04-05 06:43:39.000000 carefree-creator-0.2.1/carefree_creator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-05 06:43:39.000000 carefree-creator-0.2.1/carefree_creator.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-05 06:43:39.162584 carefree-creator-0.2.1/cfcreator/
--rw-rw-rw-   0        0        0       96 2023-04-05 06:43:03.000000 carefree-creator-0.2.1/cfcreator/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-05 06:43:39.163575 carefree-creator-0.2.1/cfcreator/apis/
--rw-rw-rw-   0        0        0      821 2023-04-05 06:43:03.000000 carefree-creator-0.2.1/cfcreator/apis/config.yml
--rw-rw-rw-   0        0        0     9036 2023-04-05 06:43:03.000000 carefree-creator-0.2.1/cfcreator/apis/interface.py
-drwxrwxrwx   0        0        0        0 2023-04-05 06:43:39.164573 carefree-creator-0.2.1/cfcreator/apis/kafka/
--rw-rw-rw-   0        0        0      821 2023-04-05 06:43:03.000000 carefree-creator-0.2.1/cfcreator/apis/kafka/config.yml
--rw-rw-rw-   0        0        0    12668 2023-04-05 06:43:03.000000 carefree-creator-0.2.1/cfcreator/apis/kafka/consumer.py
--rw-rw-rw-   0        0        0    12109 2023-04-05 06:43:03.000000 carefree-creator-0.2.1/cfcreator/apis/kafka/producer.py
--rw-rw-rw-   0        0        0     2984 2023-04-05 06:43:03.000000 carefree-creator-0.2.1/cfcreator/cli.py
--rw-rw-rw-   0        0        0    18794 2023-04-05 06:43:03.000000 carefree-creator-0.2.1/cfcreator/common.py
--rw-rw-rw-   0        0        0    14003 2023-04-05 06:43:03.000000 carefree-creator-0.2.1/cfcreator/control.py
--rw-rw-rw-   0        0        0     3259 2023-04-05 06:43:03.000000 carefree-creator-0.2.1/cfcreator/control_multi.py
--rw-rw-rw-   0        0        0     8444 2023-04-05 06:43:03.000000 carefree-creator-0.2.1/cfcreator/cos.py
--rw-rw-rw-   0        0        0     4566 2023-04-05 06:43:03.000000 carefree-creator-0.2.1/cfcreator/cv.py
--rw-rw-rw-   0        0        0     2087 2023-04-05 06:43:03.000000 carefree-creator-0.2.1/cfcreator/endpoints.py
--rw-rw-rw-   0        0        0    18991 2023-04-05 06:43:03.000000 carefree-creator-0.2.1/cfcreator/img2img.py
--rw-rw-rw-   0        0        0     1636 2023-04-05 06:43:03.000000 carefree-creator-0.2.1/cfcreator/img2txt.py
--rw-rw-rw-   0        0        0     3298 2023-04-05 06:43:03.000000 carefree-creator-0.2.1/cfcreator/parameters.py
--rw-rw-rw-   0        0        0     3167 2023-04-05 06:43:03.000000 carefree-creator-0.2.1/cfcreator/pipeline.py
-drwxrwxrwx   0        0        0        0 2023-04-05 06:43:39.166566 carefree-creator-0.2.1/cfcreator/sdks/
--rw-rw-rw-   0        0        0       45 2023-04-05 06:43:03.000000 carefree-creator-0.2.1/cfcreator/sdks/__init__.py
--rw-rw-rw-   0        0        0      659 2023-04-05 06:43:03.000000 carefree-creator-0.2.1/cfcreator/sdks/direct.py
--rw-rw-rw-   0        0        0     2130 2023-04-05 06:43:03.000000 carefree-creator-0.2.1/cfcreator/sdks/kafka.py
--rw-rw-rw-   0        0        0     1103 2023-04-05 06:43:03.000000 carefree-creator-0.2.1/cfcreator/sdks/utils.py
--rw-rw-rw-   0        0        0     5764 2023-04-05 06:43:03.000000 carefree-creator-0.2.1/cfcreator/txt2img.py
--rw-rw-rw-   0        0        0     2371 2023-04-05 06:43:03.000000 carefree-creator-0.2.1/cfcreator/txt2txt.py
--rw-rw-rw-   0        0        0     4631 2023-04-05 06:43:03.000000 carefree-creator-0.2.1/cfcreator/utils.py
--rw-rw-rw-   0        0        0       42 2023-04-05 06:43:39.168072 carefree-creator-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0     1014 2023-04-05 06:43:03.000000 carefree-creator-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-06 05:30:48.650275 carefree-creator-0.2.2/
+-rw-rw-rw-   0        0        0     1090 2022-10-31 07:20:41.000000 carefree-creator-0.2.2/LICENSE
+-rw-rw-rw-   0        0        0      195 2023-04-13 07:31:10.000000 carefree-creator-0.2.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     4419 2023-05-06 05:30:48.650275 carefree-creator-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4117 2023-05-06 03:00:57.000000 carefree-creator-0.2.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-06 05:30:48.638038 carefree-creator-0.2.2/carefree_creator.egg-info/
+-rw-rw-rw-   0        0        0     4419 2023-05-06 05:30:48.000000 carefree-creator-0.2.2/carefree_creator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      962 2023-05-06 05:30:48.000000 carefree-creator-0.2.2/carefree_creator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 05:30:48.000000 carefree-creator-0.2.2/carefree_creator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-05-06 05:30:48.000000 carefree-creator-0.2.2/carefree_creator.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      138 2023-05-06 05:30:48.000000 carefree-creator-0.2.2/carefree_creator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-06 05:30:48.000000 carefree-creator-0.2.2/carefree_creator.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-06 05:30:48.643297 carefree-creator-0.2.2/cfcreator/
+-rw-rw-rw-   0        0        0       96 2023-04-18 08:30:52.000000 carefree-creator-0.2.2/cfcreator/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 05:30:48.644874 carefree-creator-0.2.2/cfcreator/apis/
+-rw-rw-rw-   0        0        0      821 2023-04-13 07:31:10.000000 carefree-creator-0.2.2/cfcreator/apis/config.yml
+-rw-rw-rw-   0        0        0     9036 2023-04-23 02:27:17.000000 carefree-creator-0.2.2/cfcreator/apis/interface.py
+drwxrwxrwx   0        0        0        0 2023-05-06 05:30:48.646275 carefree-creator-0.2.2/cfcreator/apis/kafka/
+-rw-rw-rw-   0        0        0      821 2023-04-18 08:30:52.000000 carefree-creator-0.2.2/cfcreator/apis/kafka/config.yml
+-rw-rw-rw-   0        0        0    13665 2023-05-06 03:04:49.000000 carefree-creator-0.2.2/cfcreator/apis/kafka/consumer.py
+-rw-rw-rw-   0        0        0    12109 2023-05-06 03:04:49.000000 carefree-creator-0.2.2/cfcreator/apis/kafka/producer.py
+-rw-rw-rw-   0        0        0     2984 2023-04-23 02:27:17.000000 carefree-creator-0.2.2/cfcreator/cli.py
+-rw-rw-rw-   0        0        0    22444 2023-05-06 03:04:49.000000 carefree-creator-0.2.2/cfcreator/common.py
+-rw-rw-rw-   0        0        0    14925 2023-05-06 03:00:57.000000 carefree-creator-0.2.2/cfcreator/control.py
+-rw-rw-rw-   0        0        0     2226 2023-05-06 03:00:57.000000 carefree-creator-0.2.2/cfcreator/control_multi.py
+-rw-rw-rw-   0        0        0     8444 2023-05-06 03:04:49.000000 carefree-creator-0.2.2/cfcreator/cos.py
+-rw-rw-rw-   0        0        0     4566 2023-04-18 08:30:52.000000 carefree-creator-0.2.2/cfcreator/cv.py
+-rw-rw-rw-   0        0        0     2458 2023-05-06 03:04:49.000000 carefree-creator-0.2.2/cfcreator/endpoints.py
+-rw-rw-rw-   0        0        0    20283 2023-05-06 03:00:57.000000 carefree-creator-0.2.2/cfcreator/img2img.py
+-rw-rw-rw-   0        0        0     1657 2023-05-06 03:04:49.000000 carefree-creator-0.2.2/cfcreator/img2txt.py
+drwxrwxrwx   0        0        0        0 2023-05-06 05:30:48.648275 carefree-creator-0.2.2/cfcreator/legacy/
+-rw-rw-rw-   0        0        0        0 2023-05-06 03:00:57.000000 carefree-creator-0.2.2/cfcreator/legacy/__init__.py
+-rw-rw-rw-   0        0        0     2102 2023-05-06 03:00:57.000000 carefree-creator-0.2.2/cfcreator/legacy/common.py
+-rw-rw-rw-   0        0        0    13724 2023-05-06 03:00:57.000000 carefree-creator-0.2.2/cfcreator/legacy/control.py
+-rw-rw-rw-   0        0        0     3216 2023-05-06 03:00:57.000000 carefree-creator-0.2.2/cfcreator/legacy/control_multi.py
+-rw-rw-rw-   0        0        0     3298 2023-05-06 03:04:49.000000 carefree-creator-0.2.2/cfcreator/parameters.py
+-rw-rw-rw-   0        0        0     3431 2023-05-06 03:04:49.000000 carefree-creator-0.2.2/cfcreator/pipeline.py
+drwxrwxrwx   0        0        0        0 2023-05-06 05:30:48.649275 carefree-creator-0.2.2/cfcreator/sdks/
+-rw-rw-rw-   0        0        0       45 2023-04-18 08:30:52.000000 carefree-creator-0.2.2/cfcreator/sdks/__init__.py
+-rw-rw-rw-   0        0        0      659 2023-04-23 02:27:17.000000 carefree-creator-0.2.2/cfcreator/sdks/direct.py
+-rw-rw-rw-   0        0        0     2130 2023-04-23 02:27:17.000000 carefree-creator-0.2.2/cfcreator/sdks/kafka.py
+-rw-rw-rw-   0        0        0     1103 2023-04-23 02:27:17.000000 carefree-creator-0.2.2/cfcreator/sdks/utils.py
+-rw-rw-rw-   0        0        0     6800 2023-05-06 03:00:57.000000 carefree-creator-0.2.2/cfcreator/txt2img.py
+-rw-rw-rw-   0        0        0     2371 2023-04-23 02:27:17.000000 carefree-creator-0.2.2/cfcreator/txt2txt.py
+-rw-rw-rw-   0        0        0     4631 2023-04-23 02:27:17.000000 carefree-creator-0.2.2/cfcreator/utils.py
+-rw-rw-rw-   0        0        0       42 2023-05-06 05:30:48.650275 carefree-creator-0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0     1014 2023-05-06 05:22:15.000000 carefree-creator-0.2.2/setup.py
```

### Comparing `carefree-creator-0.2.1/LICENSE` & `carefree-creator-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `carefree-creator-0.2.1/carefree_creator.egg-info/SOURCES.txt` & `carefree-creator-0.2.2/carefree_creator.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -24,11 +24,15 @@
 cfcreator/txt2txt.py
 cfcreator/utils.py
 cfcreator/apis/config.yml
 cfcreator/apis/interface.py
 cfcreator/apis/kafka/config.yml
 cfcreator/apis/kafka/consumer.py
 cfcreator/apis/kafka/producer.py
+cfcreator/legacy/__init__.py
+cfcreator/legacy/common.py
+cfcreator/legacy/control.py
+cfcreator/legacy/control_multi.py
 cfcreator/sdks/__init__.py
 cfcreator/sdks/direct.py
 cfcreator/sdks/kafka.py
 cfcreator/sdks/utils.py
```

### Comparing `carefree-creator-0.2.1/cfcreator/apis/config.yml` & `carefree-creator-0.2.2/cfcreator/apis/config.yml`

 * *Files identical despite different names*

### Comparing `carefree-creator-0.2.1/cfcreator/apis/interface.py` & `carefree-creator-0.2.2/cfcreator/apis/interface.py`

 * *Files identical despite different names*

### Comparing `carefree-creator-0.2.1/cfcreator/apis/kafka/config.yml` & `carefree-creator-0.2.2/cfcreator/apis/kafka/config.yml`

 * *Files identical despite different names*

### Comparing `carefree-creator-0.2.1/cfcreator/apis/kafka/consumer.py` & `carefree-creator-0.2.2/cfcreator/apis/kafka/consumer.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,14 +23,16 @@
 from cfclient.core import HttpClient
 from cfclient.core import TritonClient
 from cfclient.utils import get_err_msg
 from cfclient.utils import run_algorithm
 
 # This is necessary to register the algorithms
 from cfcreator import *
+from cfcreator.legacy.control import ControlNetModel as LegacyControlNetModel
+from cfcreator.legacy.control_multi import ControlMultiModel as LegacyControlMultiModel
 
 
 # logging
 root = os.path.dirname(__file__)
 logging_root = os.path.join(root, "logs", "consumer")
 os.makedirs(logging_root, exist_ok=True)
 with open(os.path.join(root, "config.yml")) as f:
@@ -109,25 +111,41 @@
 
 
 async def post_callback(
     url: str,
     uid: str,
     success: bool,
     data: Dict[str, Any],
+    retry: int = 10,
+    interval: int = 3,
 ) -> None:
-    if url:
+    if not url:
+        return
+
+    async def fn() -> None:
+        cb_data = dict(uid=uid, success=success, data=data)
+        async with http_client.session.post(url, json=cb_data, timeout=interval) as res:
+            if not res.ok:
+                raise ValueError(f"post callback failed ({res.status})")
+
+    msg = ""
+    for i in range(retry):
         try:
-            data = dict(uid=uid, success=success, data=data)
-            async with http_client.session.post(url, json=data, timeout=1) as res:
-                await res.json()
+            await fn()
+            if i > 0:
+                logging.warning(f"succeeded after {i} retries ({msg})")
+            return
         except Exception as err:
-            print(
-                f"\n\n!!! post to callback_url ({url}) failed "
-                f"({get_err_msg(err)}) !!!\n\n"
-            )
+            msg = get_err_msg(err)
+        time.sleep(interval)
+    if msg:
+        print(
+            f"\n\n!!! post to callback_url ({url}) failed "
+            f"(After {retry} retries) ({msg}) !!!\n\n"
+        )
 
 
 def simplify(params: Dict[str, Any]) -> Dict[str, Any]:
     params = shallow_copy_dict(params)
     custom_embeddings = params.get("custom_embeddings")
     if custom_embeddings is not None and isinstance(custom_embeddings, dict):
         simplified_embeddings = {}
@@ -205,35 +223,42 @@
                 t1 = time.time()
                 if task.startswith("control") or task.startswith("pipeline"):
                     procedure = "run_algorithm -> upload_temp_image"
                     url_results = [upload_temp_image(cos_client, arr) for arr in res]
                     urls = [rs.cdn for rs in url_results]
                     t2 = time.time()
                     procedure = "upload_temp_image -> audit_image"
-                    if not isinstance(model, ControlNetModel) or not model.use_audit:
+                    if (
+                        not isinstance(model, (ControlNetModel, LegacyControlNetModel))
+                        or not model.use_audit
+                    ):
                         reasons = [""] * len(urls)
                     else:
                         reasons = []
                         for i, rs in enumerate(url_results):
                             try:
                                 audit = audit_image(
                                     cos_client, image_mod_client, rs.path
                                 )
                             except:
                                 audit = AuditResponse(safe=False, reason="unknown")
                             if audit.safe:
                                 reasons.append("")
                             else:
-                                urls[i] = None
+                                urls[i] = ""
                                 reasons.append(audit.reason)
                     t3 = time.time()
                     procedure = "audit_image -> redis"
                     if task.startswith("control"):
-                        types = params.get("types")
-                        num_cond = 1 if types is None else len(types)
+                        if isinstance(model, ControlMultiModel):
+                            num_cond = len(set(b.type for b in model.controls))
+                        elif isinstance(model, LegacyControlMultiModel):
+                            num_cond = len(model.types)
+                        else:
+                            num_cond = 1
                         result = dict(
                             uid=uid,
                             response=dict(
                                 hint_urls=urls[:num_cond],
                                 hint_reasons=reasons[:num_cond],
                                 result_urls=urls[num_cond:],
                                 result_reasons=reasons[num_cond:],
@@ -245,15 +270,16 @@
                         raise ValueError(f"unrecognized task '{task}' occurred")
                 elif algorithm.response_model_class is not None:
                     t2 = t3 = t1
                     procedure = "run_algorithm -> redis"
                     result = dict(uid=uid, response=res.dict())
                 else:
                     procedure = "run_algorithm -> upload_temp_image"
-                    urls = upload_temp_image(cos_client, res.body)
+                    content = res[0] if isinstance(res, list) else res.body
+                    urls = upload_temp_image(cos_client, content)
                     t2 = time.time()
                     procedure = "upload_temp_image -> audit_image"
                     if task != "img2img.sr":
                         try:
                             audit = audit_image(audit_redis_client, urls.path)
                         except:
                             audit = AuditResponse(safe=False, reason="unknown")
```

### Comparing `carefree-creator-0.2.1/cfcreator/apis/kafka/producer.py` & `carefree-creator-0.2.2/cfcreator/apis/kafka/producer.py`

 * *Files identical despite different names*

### Comparing `carefree-creator-0.2.1/cfcreator/cli.py` & `carefree-creator-0.2.2/cfcreator/cli.py`

 * *Files identical despite different names*

### Comparing `carefree-creator-0.2.1/cfcreator/common.py` & `carefree-creator-0.2.2/cfcreator/common.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,20 +17,24 @@
 from pydantic import Field
 from pydantic import BaseModel
 from functools import partial
 from cftool.cv import np_to_bytes
 from cfclient.models import TextModel
 from cfclient.models import ImageModel
 from cfclient.models import AlgorithmBase
+from cflearn.zoo import DLZoo
+from cflearn.parameters import OPT
 from cflearn.api.cv import SDVersions
 from cflearn.api.cv import DiffusionAPI
 from cflearn.api.cv import TranslatorAPI
 from cflearn.api.cv import ImageHarmonizationAPI
 from cflearn.api.cv import ControlledDiffusionAPI
 from cflearn.misc.toolkit import _get_file_size
+from cflearn.misc.toolkit import download_model
+from cflearn.models.cv.diffusion import StableDiffusion
 from cflearn.api.cv.third_party.blip import BLIPAPI
 from cflearn.api.cv.third_party.lama import LaMa
 from cflearn.api.cv.third_party.isnet import ISNetAPI
 from cflearn.api.cv.third_party.prompt import PromptEnhanceAPI
 
 from .cos import download_with_retry
 from .cos import download_image_with_retry
@@ -54,31 +58,112 @@
         MY_FANCY_MODEL = "my_fancy_model"
 
     then you can place your model at ~/.cache/external/my_fancy_model.ckpt,
     after which you can specify `my_fancy_model` as the `version` parameter!
     """
 
 
+class SDInpaintingVersions(str, Enum):
+    v1_5 = "v1.5"
+
+
+class ExternalInpaintingVersions(str, Enum):
+    """
+    Specify external SD-inpainting weights that need to be loaded.
+    * these weights should be placed under ~/.cache/external/inpainting/ folder.
+    * file name should be {version}.ckpt
+
+    Example
+    -------
+    class ExternalVersions(str, Enum):
+        MY_FANCY_MODEL = "my_fancy_model"
+
+    then you can place your model at ~/.cache/external/inpainting/my_fancy_model.ckpt,
+    after which you can specify `my_fancy_model` as the `version` parameter!
+    """
+
+
 def merge_enums(*enums: Enum) -> Enum:
     members: Dict[str, str] = {}
     for e in enums:
         for name, member in e.__members__.items():
             members[name] = member.value
     return Enum("MergedVersions", members, type=str)
 
 
 MergedVersions = merge_enums(SDVersions, ExternalVersions)
+MergedInpaintingVersions = merge_enums(SDInpaintingVersions, ExternalInpaintingVersions)
+BaseSDTag = "_base_sd"
+
+
+def _base_sd_path() -> str:
+    root = os.path.join(OPT.cache_dir, DLZoo.model_dir)
+    return download_model("ldm_sd_v1.5", root=root)
 
 
 def _get(init_fn: Callable, init_to_cpu: bool) -> Any:
     if init_to_cpu:
         return init_fn()
     return init_fn("cuda:0", use_half=True)
 
 
+def _load_external(
+    m: ControlledDiffusionAPI,
+    external_enum: Enum,
+    external_folder: str,
+) -> None:
+    print(f"> handling external weights under '{external_folder}'")
+    os.makedirs(external_folder, exist_ok=True)
+    converted_sizes_path = os.path.join(external_folder, "sizes.json")
+    sizes: Dict[str, int]
+    if not os.path.isfile(converted_sizes_path):
+        sizes = {}
+    else:
+        with open(converted_sizes_path, "r") as f:
+            sizes = json.load(f)
+    for version in external_enum:
+        print(f">> handling {version}")
+        converted_path = os.path.join(external_folder, f"{version}_converted.pt")
+        v_size = sizes.get(version)
+        f_size = (
+            None
+            if not os.path.isfile(converted_path)
+            else _get_file_size(converted_path)
+        )
+        if f_size is None or v_size != f_size:
+            if f_size is not None:
+                print(f">> {version} has been converted but size mismatch")
+            print(f">> converting {version}")
+            model_path = os.path.join(external_folder, f"{version}.ckpt")
+            d = cflearn.scripts.sd.convert(model_path, m, load=False)
+            torch.save(d, converted_path)
+            sizes[version] = _get_file_size(converted_path)
+        m.sd_weights.register(version, converted_path)
+    with open(converted_sizes_path, "w") as f:
+        json.dump(sizes, f)
+
+
+def _load_lora(m: ControlledDiffusionAPI, external_folder: str) -> None:
+    print("> loading lora")
+    num_lora = 0
+    lora_folder = os.path.join(external_folder, "lora")
+    os.makedirs(lora_folder, exist_ok=True)
+    for lora_file in os.listdir(lora_folder):
+        try:
+            lora_name = os.path.splitext(lora_file)[0]
+            lora_path = os.path.join(lora_folder, lora_file)
+            print(f">> loading {lora_name}")
+            m.load_sd_lora(lora_name, path=lora_path)
+            num_lora += 1
+        except:
+            print(f">>>> Failed to load!")
+            continue
+    print(f"> {num_lora} lora loaded")
+
+
 def init_sd(init_to_cpu: bool) -> ControlledDiffusionAPI:
     version = MergedVersions.v1_5
     init_fn = partial(ControlledDiffusionAPI.from_sd_version, version)
     m: ControlledDiffusionAPI = _get(init_fn, init_to_cpu)
     focus = get_focus()
     m.sd_weights.limit = pool_limit()
     m.current_sd_version = version
@@ -91,71 +176,61 @@
         targets.append(MergedVersions.DREAMLIKE)
         targets.append(MergedVersions.ANIME_ANYTHING)
         targets.append(MergedVersions.ANIME_HYBRID)
         targets.append(MergedVersions.ANIME_GUOFENG)
         targets.append(MergedVersions.ANIME_ORANGE)
     print(f"> preparing sd weights ({', '.join(targets)}) (focus={focus})")
     m.prepare_sd(targets)
+    m.sd_weights.register(BaseSDTag, _base_sd_path())
     # when focus is SYNC, `init_sd` is called because we need to expose `control_hint`
     # endpoints. However, `sd` itself will never be used, so we can skip some stuffs
+    user_folder = os.path.expanduser("~")
+    external_folder = os.path.join(user_folder, ".cache", "external")
     if focus == Focus.SYNC:
         print("> prepare ControlNet Annotators")
         for hint in m.control_defaults:
             m.prepare_annotator(hint)
     else:
-        print("> handling external weights")
-        external_dir = os.path.join(os.path.expanduser("~"), ".cache", "external")
-        os.makedirs(external_dir, exist_ok=True)
-        converted_sizes_path = os.path.join(external_dir, "sizes.json")
-        sizes: Dict[str, int]
-        if not os.path.isfile(converted_sizes_path):
-            sizes = {}
-        else:
-            with open(converted_sizes_path, "r") as f:
-                sizes = json.load(f)
-        for version in ExternalVersions:
-            print(f">> handling {version}")
-            converted_path = os.path.join(external_dir, f"{version}_converted.pt")
-            v_size = sizes.get(version)
-            f_size = (
-                None
-                if not os.path.isfile(converted_path)
-                else _get_file_size(converted_path)
-            )
-            if f_size is None or v_size != f_size:
-                if f_size is not None:
-                    print(f">> {version} has been converted but size mismatch")
-                print(f">> converting {version}")
-                model_path = os.path.join(external_dir, f"{version}.ckpt")
-                d = cflearn.scripts.sd.convert(model_path, m, load=False)
-                torch.save(d, converted_path)
-                sizes[version] = _get_file_size(converted_path)
-            m.sd_weights.register(version, converted_path)
-        with open(converted_sizes_path, "w") as f:
-            json.dump(sizes, f)
+        _load_external(m, ExternalVersions, external_folder)
         print("> prepare ControlNet weights")
         m.prepare_control_defaults()
         print("> prepare ControlNet Annotators")
         m.prepare_annotators()
         print("> warmup ControlNet")
         m.switch_control(*m.available_control_hints)
+    # lora stuffs
+    _load_lora(m, external_folder)
     # return
     return m
 
 
 def init_sd_inpainting(init_to_cpu: bool) -> ControlledDiffusionAPI:
     register_sd()
-    sd: ControlledDiffusionAPI = api_pool.get(APIs.SD)
+    sd: ControlledDiffusionAPI = api_pool.get(APIs.SD, no_change=True)
     init_fn = ControlledDiffusionAPI.from_sd_inpainting
-    m: ControlledDiffusionAPI = _get(init_fn, init_to_cpu)
-    m.annotators = sd.annotators
-    m.controlnet_weights = sd.controlnet_weights
-    m.current_sd_version = MergedVersions.v1_5
-    m.switch_control(*m.available_control_hints)
-    return m
+    api: ControlledDiffusionAPI = _get(init_fn, init_to_cpu)
+    # manually maintain sd_weights
+    ## original weights
+    api.sd_weights.register(BaseSDTag, _base_sd_path())
+    ## inpainting weights
+    root = os.path.join(OPT.cache_dir, DLZoo.model_dir)
+    inpainting_path = download_model("ldm.sd_inpainting", root=root)
+    api.sd_weights.register(MergedInpaintingVersions.v1_5, inpainting_path)
+    user_folder = os.path.expanduser("~")
+    external_folder = os.path.join(user_folder, ".cache", "external")
+    external_inpainting_folder = os.path.join(external_folder, "inpainting")
+    _load_external(api, ExternalInpaintingVersions, external_inpainting_folder)
+    # lora stuffs
+    _load_lora(api, external_folder)
+    # inject properties from sd
+    api.annotators = sd.annotators
+    api.controlnet_weights = sd.controlnet_weights
+    api.current_sd_version = MergedInpaintingVersions.v1_5
+    api.switch_control(*api.available_control_hints)
+    return api
 
 
 def register_sd() -> None:
     api_pool.register(APIs.SD, init_sd)
 
 
 def register_sd_inpainting() -> None:
@@ -361,17 +436,28 @@
 """,
     )
     custom_embeddings: Dict[str, List[List[float]]] = Field(
         {},
         description="Custom embeddings, often used in textual inversion.",
     )
     tome_info: TomeInfoModel = Field(TomeInfoModel(), description="tomesd settings.")
+    lora_scales: Optional[Dict[str, float]] = Field(
+        None,
+        description="lora scales, key is the name, value is the weight.",
+    )
 
 
-class CommonSDInpaintingModel(BaseModel):
+class ReturnArraysModel(BaseModel):
+    return_arrays: bool = Field(
+        False,
+        description="Whether return List[np.ndarray] directly, only for internal usages.",
+    )
+
+
+class CommonSDInpaintingModel(ReturnArraysModel):
     keep_original: bool = Field(
         False,
         description="Whether strictly keep the original image identical in the output image.",
     )
     use_raw_inpainting: bool = Field(
         False,
         description="""
@@ -411,58 +497,63 @@
     pass
 
 
 class ControlStrengthModel(BaseModel):
     control_strength: float = Field(1.0, description="The strength of the control.")
 
 
-class ReturnArraysModel(BaseModel):
-    return_arrays: bool = Field(
-        False,
-        description="Whether return List[np.ndarray] directly, only for internal usages.",
-    )
-
-
 class _ControlNetModel(BaseModel):
+    url: Optional[str] = Field(None, description="specify this to perform img2img")
     hint_url: str = Field(
         "",
         description="""
 The `cdn` / `cos` url of the user's hint image.
 > If empty string is provided, we will use `url` as `hint_url`.
 > `cos` url from `qcloud` is preferred.
 """,
     )
-    hint_starts: Dict[str, float] = Field(
-        default_factory=lambda: {},
-        description="start ratio of each hint",
-    )
-    prompt: str = Field(..., description="Prompt.")
+    hint_start: Optional[float] = Field(None, description="start ratio of the control")
+    prompt: str = Field("", description="Prompt.")
     fidelity: float = Field(
         0.05,
         ge=0.0,
         le=1.0,
-        description="The fidelity of the input image, only take effects when `use_img2img` is True.",
+        description="The fidelity of the input image, only take effects when `url` is not `None`.",
     )
-    use_img2img: bool = Field(True, description="Whether use img2img method.")
     num_samples: int = Field(1, ge=1, le=4, description="Number of samples.")
     bypass_annotator: bool = Field(False, description="Bypass the annotator.")
     base_model: MergedVersions = Field(
         MergedVersions.v1_5,
         description="The base model.",
     )
     guess_mode: bool = Field(False, description="Guess mode.")
     use_audit: bool = Field(False, description="Whether audit the outputs.")
+    no_switch: bool = Field(
+        False,
+        description="Whether not to switch the ControlNet weights even when the base model has switched.",
+    )
+
+
+# only useful when inpainting model is used
+class _InpaintingMixin(BaseModel):
+    use_latent_guidance: bool = Field(
+        False,
+        description="Whether use the latent of the givent image to guide the generation.",
+    )
+    reference_fidelity: float = Field(
+        0.0, description="Fidelity of the reference image."
+    )
 
 
 class ControlNetModel(
     ReturnArraysModel,
+    _InpaintingMixin,
     DiffusionModel,
     MaxWHModel,
     _ControlNetModel,
-    ImageModel,
 ):
     pass
 
 
 def handle_diffusion_model(m: DiffusionAPI, data: DiffusionModel) -> Dict[str, Any]:
     seed = None if data.seed == -1 else data.seed
     variation_seed = None
@@ -489,14 +580,24 @@
     else:
         if tome_info["seed"] == -1:
             if seed is None:
                 tome_info.pop("seed")
             else:
                 tome_info["seed"] = seed
         m.set_tome_info(tome_info)
+    # lora
+    model = m.m
+    if isinstance(model, StableDiffusion):
+        manager = model.lora_manager
+        if manager.injected:
+            m.cleanup_sd_lora()
+        if data.lora_scales is not None:
+            m.inject_sd_lora(*list(data.lora_scales))
+            m.set_sd_lora_scales(data.lora_scales)
+    # return
     return dict(
         seed=seed,
         variation_seed=variation_seed,
         variation_strength=variation_strength,
         variations=variations,
         num_steps=data.num_steps,
         unconditional_guidance_scale=data.guidance_scale,
```

### Comparing `carefree-creator-0.2.1/cfcreator/control.py` & `carefree-creator-0.2.2/cfcreator/legacy/control.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,35 +21,32 @@
 from cftool.cv import np_to_bytes
 from cftool.cv import restrict_wh
 from cftool.cv import get_suitable_size
 from cfclient.models.core import ImageModel
 from cflearn.api.cv.diffusion import ControlNetHints
 from cflearn.api.cv.diffusion import ControlledDiffusionAPI
 
-from .utils import api_pool
-from .utils import to_canvas
-from .utils import resize_image
-from .utils import APIs
-from .common import register_sd
-from .common import handle_diffusion_model
-from .common import IAlgorithm
 from .common import ControlNetModel
-from .common import ReturnArraysModel
-from .common import ControlStrengthModel
+from ..utils import api_pool
+from ..utils import to_canvas
+from ..utils import resize_image
+from ..utils import APIs
+from ..common import BaseSDTag
+from ..common import register_sd
+from ..common import handle_diffusion_model
+from ..common import IAlgorithm
+from ..common import ReturnArraysModel
+from ..common import ControlStrengthModel
 
 
 root = os.path.dirname(__file__)
 control_depth_endpoint = "/control/depth"
 control_canny_endpoint = "/control/canny"
 control_pose_endpoint = "/control/pose"
 control_mlsd_endpoint = "/control/mlsd"
-control_depth_hint_endpoint = "/control/depth_hint"
-control_canny_hint_endpoint = "/control/canny_hint"
-control_pose_hint_endpoint = "/control/pose_hint"
-control_mlsd_hint_endpoint = "/control/mlsd_hint"
 
 
 images_type = Tuple[np.ndarray, np.ndarray]
 apply_response = Tuple[List[np.ndarray], Dict[str, float]]
 
 
 class ControlNetModelPlaceholder(ControlStrengthModel, ControlNetModel):
@@ -95,15 +92,16 @@
     t0 = time.time()
     if not isinstance(hint_types, list):
         hint_types = [hint_types]
     if len(hint_types) > api.num_pool:
         msg = f"maximum number of control is {api.num_pool}, but got {len(hint_types)}"
         raise ValueError(msg)
     api.switch_sd(common_data.base_model)
-    api.switch_control(*hint_types)
+    base_md = api.sd_weights.get(BaseSDTag) if common_data.no_switch else None
+    api.switch_control(*hint_types, base_md=base_md)
     t1 = time.time()
     all_hint = {}
     all_o_hint_arrays = []
     all_annotator_change_device_times = []
     for hint_type in sorted(hint_types):
         if detect_resolution is None or isinstance(detect_resolution, int):
             h_res = detect_resolution
@@ -152,30 +150,33 @@
             [
                 h_data.control_strength * (0.825 ** float(12 - i))
                 for i in range(num_scales)
             ]
             if h_data.guess_mode
             else ([h_data.control_strength] * num_scales)
         )
-    api.m.control_scales = all_scales
     cond = [common_data.prompt] * common_data.num_samples
     kw = handle_diffusion_model(api, common_data)
-    kw["hint"] = all_hint
-    kw["hint_start"] = common_data.hint_starts
+    keys = sorted([k.value if isinstance(k, ControlNetHints) else k for k in all_hint])
+    kw["hint"] = [(k, all_hint[k]) for k in keys]
+    kw["hint_start"] = [common_data.hint_starts.get(k) for k in keys]
     kw["max_wh"] = common_data.max_wh
+    api.m.control_scales = [all_scales[k] for k in keys]
     dt = time.time()
     if need_change_device:
         api.to("cuda:0", use_half=True, no_annotator=True)
     change_diffusion_device_time = time.time() - dt
     # inpainting workaround
     if api.m.unet_kw["in_channels"] == 9:
         if normalized_inpainting_mask is None:
             raise ValueError("`normalized_input_mask` should be provided to inpainting")
         image = Image.fromarray(input_image)
         inpainting_mask = Image.fromarray(to_uint8(normalized_inpainting_mask))
+        kw["use_latent_guidance"] = common_data.use_latent_guidance
+        kw["reference_fidelity"] = common_data.reference_fidelity
         outs = api.txt2img_inpainting(cond, image, inpainting_mask, **kw)
     elif not common_data.use_img2img:
         kw["size"] = w, h
         outs = api.txt2img(cond, **kw)
     else:
         init_image = cv2.resize(
             input_image,
@@ -259,14 +260,15 @@
     hint_type: ControlNetHints,
 ) -> None:
     class _Model(hint_model_class, ReturnArraysModel, ImageModel):
         pass
 
     class _(IAlgorithm):
         model_class = _Model
+        model_class.__name__ = hint_model_class.__name__
 
         endpoint = hint_endpoint
 
         def initialize(self) -> None:
             register_sd()
 
         async def run(self, data: _Model, *args: Any) -> Response:
@@ -401,27 +403,15 @@
 
 # register
 
 register_control(ControlDepthModel, control_depth_endpoint, ControlNetHints.DEPTH)
 register_control(ControlCannyModel, control_canny_endpoint, ControlNetHints.CANNY)
 register_control(ControlPoseModel, control_pose_endpoint, ControlNetHints.POSE)
 register_control(ControlMLSDModel, control_mlsd_endpoint, ControlNetHints.MLSD)
-register_hint(_DepthModel, control_depth_hint_endpoint, ControlNetHints.DEPTH)
-register_hint(_CannyModel, control_canny_hint_endpoint, ControlNetHints.CANNY)
-register_hint(_PoseModel, control_pose_hint_endpoint, ControlNetHints.POSE)
-register_hint(_MLSDModel, control_mlsd_hint_endpoint, ControlNetHints.MLSD)
 
 
 __all__ = [
     "control_depth_endpoint",
     "control_canny_endpoint",
     "control_pose_endpoint",
     "control_mlsd_endpoint",
-    "control_depth_hint_endpoint",
-    "control_canny_hint_endpoint",
-    "control_pose_hint_endpoint",
-    "control_mlsd_hint_endpoint",
-    "ControlDepthModel",
-    "ControlCannyModel",
-    "ControlPoseModel",
-    "ControlMLSDModel",
 ]
```

### Comparing `carefree-creator-0.2.1/cfcreator/control_multi.py` & `carefree-creator-0.2.2/cfcreator/legacy/control_multi.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 from typing import List
 from fastapi import Response
 from pydantic import Field
 from cftool.cv import np_to_bytes
 from cftool.misc import shallow_copy_dict
 from cflearn.api.cv.diffusion import ControlNetHints
 
-from .utils import to_canvas
-from .utils import APIs
-from .common import register_sd
-from .common import IAlgorithm
 from .common import ControlNetModel
 from .control import get_images
 from .control import apply_control
 from .control import MLSDModel
 from .control import PoseModel
 from .control import CannyModel
 from .control import DepthModel
 from .control import ControlMLSDModel
 from .control import ControlPoseModel
 from .control import ControlCannyModel
 from .control import ControlDepthModel
+from ..utils import to_canvas
+from ..utils import APIs
+from ..common import register_sd
+from ..common import IAlgorithm
 
 
 control_multi_endpoint = "/control/multi"
 model_mapping = {
     ControlNetHints.MLSD: ControlMLSDModel,
     ControlNetHints.POSE: ControlPoseModel,
     ControlNetHints.CANNY: ControlCannyModel,
@@ -103,10 +103,8 @@
         if data.return_arrays:
             return results
         return Response(content=content, media_type="image/png")
 
 
 __all__ = [
     "control_multi_endpoint",
-    "ControlMultiModel",
-    "ControlMulti",
 ]
```

### Comparing `carefree-creator-0.2.1/cfcreator/cos.py` & `carefree-creator-0.2.2/cfcreator/cos.py`

 * *Files identical despite different names*

### Comparing `carefree-creator-0.2.1/cfcreator/cv.py` & `carefree-creator-0.2.2/cfcreator/cv.py`

 * *Files identical despite different names*

### Comparing `carefree-creator-0.2.1/cfcreator/endpoints.py` & `carefree-creator-0.2.2/cfcreator/endpoints.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 from .txt2txt import *
 from .img2img import *
 from .img2txt import *
 from .control import *
 from .control_multi import *
 from .pipeline import *
 from .parameters import Focus
+from .legacy.control import *
+from .legacy.control_multi import *
 
 
 endpoint_to_focuses = {
     # txt2img
     txt2img_sd_endpoint: [
         Focus.ALL,
         Focus.SD,
@@ -44,14 +46,19 @@
     cv_histogram_match_endpoint: [Focus.ALL, Focus.SYNC],
     # ControlNet
     control_depth_endpoint: [Focus.ALL, Focus.CONTROL],
     control_canny_endpoint: [Focus.ALL, Focus.CONTROL],
     control_pose_endpoint: [Focus.ALL, Focus.CONTROL],
     control_mlsd_endpoint: [Focus.ALL, Focus.CONTROL],
     control_multi_endpoint: [Focus.ALL, Focus.CONTROL],
+    new_control_depth_endpoint: [Focus.ALL, Focus.CONTROL],
+    new_control_canny_endpoint: [Focus.ALL, Focus.CONTROL],
+    new_control_pose_endpoint: [Focus.ALL, Focus.CONTROL],
+    new_control_mlsd_endpoint: [Focus.ALL, Focus.CONTROL],
+    new_control_multi_endpoint: [Focus.ALL, Focus.CONTROL],
     control_depth_hint_endpoint: [Focus.ALL, Focus.SYNC, Focus.CONTROL],
     control_canny_hint_endpoint: [Focus.ALL, Focus.SYNC, Focus.CONTROL],
     control_pose_hint_endpoint: [Focus.ALL, Focus.SYNC, Focus.CONTROL],
     control_mlsd_hint_endpoint: [Focus.ALL, Focus.SYNC, Focus.CONTROL],
     # pipeline
     paste_pipeline_endpoint: [Focus.ALL, Focus.SYNC, Focus.PIPELINE],
 }
```

### Comparing `carefree-creator-0.2.1/cfcreator/img2img.py` & `carefree-creator-0.2.2/cfcreator/img2img.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 from .common import get_bytes_from_diffusion
 from .common import get_bytes_from_translator
 from .common import get_normalized_arr_from_diffusion
 from .common import IAlgorithm
 from .common import ImageModel
 from .common import Img2ImgModel
 from .common import CallbackModel
+from .common import ReturnArraysModel
 from .common import Img2ImgDiffusionModel
 from .parameters import verbose
 from .parameters import get_focus
 from .parameters import Focus
 
 
 img2img_sd_endpoint = "/img2img/sd"
@@ -74,61 +75,66 @@
     )
     wh: Tuple[int, int] = Field(
         (0, 0),
         description="The output size, `0` means as-is",
     )
 
 
-class Img2ImgSDModel(Img2ImgDiffusionModel, _Img2ImgSDModel):
+class Img2ImgSDModel(ReturnArraysModel, Img2ImgDiffusionModel, _Img2ImgSDModel):
     pass
 
 
 @IAlgorithm.auto_register()
 class Img2ImgSD(IAlgorithm):
     model_class = Img2ImgSDModel
 
     endpoint = img2img_sd_endpoint
 
     def initialize(self) -> None:
         register_sd()
 
-    async def run(self, data: Img2ImgSDModel, *args: Any) -> Response:
+    async def run(self, data: Img2ImgSDModel, *args: Any, **kwargs: Any) -> Response:
         self.log_endpoint(data)
         t0 = time.time()
         image = await self.download_image_with_retry(data.url)
         t1 = time.time()
         if not data.keep_alpha:
             image = to_rgb(image)
         w, h = data.wh
         if w > 0 and h > 0:
             image = image.resize((w, h), Image.LANCZOS)
         t2 = time.time()
         m = get_sd_from(data)
         t3 = time.time()
-        kwargs = handle_diffusion_model(m, data)
+        kwargs.update(handle_diffusion_model(m, data))
         img_arr = m.img2img(
             image,
             cond=[data.text],
             max_wh=data.max_wh,
             fidelity=data.fidelity,
             anchor=64,
             **kwargs,
         ).numpy()[0]
-        content = get_bytes_from_diffusion(img_arr)
+        if data.return_arrays:
+            content = None
+        else:
+            content = get_bytes_from_diffusion(img_arr)
         t4 = time.time()
         api_pool.cleanup(APIs.SD)
         self.log_times(
             {
                 "download": t1 - t0,
                 "preprocess": t2 - t1,
                 "get_model": t3 - t2,
                 "inference": t4 - t3,
                 "cleanup": time.time() - t4,
             }
         )
+        if content is None:
+            return [to_uint8(get_normalized_arr_from_diffusion(img_arr))]
         return Response(content=content, media_type="image/png")
 
 
 # super resolution (Real-ESRGAN)
 
 
 class _Img2ImgSRModel(BaseModel):
@@ -136,15 +142,15 @@
         False,
         description="Whether the input image is an anime image or not.",
     )
     target_w: int = Field(0, description="The target width. 0 means as-is.")
     target_h: int = Field(0, description="The target height. 0 means as-is.")
 
 
-class Img2ImgSRModel(CallbackModel, _Img2ImgSRModel, Img2ImgModel):
+class Img2ImgSRModel(ReturnArraysModel, CallbackModel, _Img2ImgSRModel, Img2ImgModel):
     pass
 
 
 def apply_sr(
     m: TranslatorAPI,
     image: Image.Image,
     max_wh: int,
@@ -200,39 +206,44 @@
             m,
             image,
             data.max_wh,
             data.target_w,
             data.target_h,
         )
         t3 = time.time()
-        content = get_bytes_from_translator(img_arr, transpose=False)
+        if data.return_arrays:
+            content = None
+        else:
+            content = get_bytes_from_translator(img_arr, transpose=False)
         t4 = time.time()
         api_pool.cleanup(api_key)
         t5 = time.time()
         latencies.update(
             {
                 "download": t1 - t0,
                 "get_model": t2 - t1,
                 "get_bytes": t4 - t3,
                 "cleanup": t5 - t4,
             }
         )
         self.log_times(latencies)
+        if content is None:
+            return [to_uint8(img_arr)]
         return Response(content=content, media_type="image/png")
 
 
 # inpainting (LDM, LaMa)
 
 
 class InpaintingModels(str, Enum):
     SD = "sd"
     LAMA = "lama"
 
 
-class Img2ImgInpaintingModel(Img2ImgDiffusionModel):
+class Img2ImgInpaintingModel(ReturnArraysModel, Img2ImgDiffusionModel):
     model: InpaintingModels = Field(
         InpaintingModels.SD,
         description="The inpainting model that we want to use.",
     )
     use_refine: bool = Field(False, description="Whether should we perform refining.")
     use_pipeline: bool = Field(
         False,
@@ -264,15 +275,20 @@
     def initialize(self) -> None:
         focus = get_focus()
         self.is_sync = focus == Focus.SYNC
         if not self.is_sync:
             register_inpainting()
         register_lama()
 
-    async def run(self, data: Img2ImgInpaintingModel, *args: Any) -> Response:
+    async def run(
+        self,
+        data: Img2ImgInpaintingModel,
+        *args: Any,
+        **kwargs: Any,
+    ) -> Response:
         self.log_endpoint(data)
         t0 = time.time()
         image = await self.download_image_with_retry(data.url)
         mask_url = data.mask_url
         if not mask_url:
             mask = Image.new("L", image.size, color=0)
         else:
@@ -294,18 +310,21 @@
                 mask,
                 None,
                 anchor=None,
                 to_mask=True,
                 to_torch_fmt=False,
             ).image
             mask_arr[mask_arr > 0.0] = 1.0
-            result = m(image_arr, mask_arr, cfg)
-            content = np_to_bytes(result)
+            img_arr = m(image_arr, mask_arr, cfg)
+            content = None if data.return_arrays else np_to_bytes(img_arr)
         else:
-            kwargs = handle_diffusion_model(m, data)
+            kwargs.update(handle_diffusion_model(m, data))
+            mask_arr = np.array(mask)
+            mask_arr[..., -1] = np.where(mask_arr[..., -1] > 0, 255, 0)
+            mask = Image.fromarray(mask_arr)
             if not data.use_pipeline:
                 refine_fidelity = data.refine_fidelity if data.use_refine else None
                 img_arr = m.inpainting(
                     image,
                     mask,
                     max_wh=data.max_wh,
                     refine_fidelity=refine_fidelity,
@@ -324,25 +343,31 @@
                 img_arr = m.inpainting(
                     image,
                     mask,
                     max_wh=data.max_wh,
                     refine_fidelity=data.refine_fidelity,
                     **kwargs,
                 ).numpy()[0]
-            content = get_bytes_from_diffusion(img_arr)
+            if not data.return_arrays:
+                content = get_bytes_from_diffusion(img_arr)
+            else:
+                content = None
+                img_arr = get_normalized_arr_from_diffusion(img_arr)
         t3 = time.time()
         api_pool.cleanup(api_key)
         self.log_times(
             {
                 "download": t1 - t0,
                 "get_model": t2 - t1,
                 "inference": t3 - t2,
                 "cleanup": time.time() - t3,
             }
         )
+        if content is None:
+            return [to_uint8(img_arr)]
         return Response(content=content, media_type="image/png")
 
 
 # semantic2img (LDM)
 
 
 class Img2ImgSemantic2ImgModel(Img2ImgDiffusionModel):
@@ -370,15 +395,20 @@
     model_class = Img2ImgSemantic2ImgModel
 
     endpoint = img2img_semantic2img_endpoint
 
     def initialize(self) -> None:
         register_semantic()
 
-    async def run(self, data: Img2ImgSemantic2ImgModel, *args: Any) -> Response:
+    async def run(
+        self,
+        data: Img2ImgSemantic2ImgModel,
+        *args: Any,
+        **kwargs: Any,
+    ) -> Response:
         self.log_endpoint(data)
         t0 = time.time()
         raw_semantic = await self.download_image_with_retry(data.url)
         t1 = time.time()
         w, h = raw_semantic.size
         raw_arr = np.array(raw_semantic)
         alpha = None
@@ -428,14 +458,15 @@
             alpha = alpha[None, None].astype(np.float32) / 255.0
         img_arr = m.semantic2img(
             semantic,
             alpha=alpha,
             max_wh=data.max_wh,
             verbose=verbose(),
             seed=data.seed,
+            **kwargs,
         ).numpy()[0]
         content = get_bytes_from_diffusion(img_arr)
         t5 = time.time()
         api_pool.cleanup(APIs.SEMANTIC)
         self.log_times(
             {
                 "download": t1 - t0,
@@ -538,54 +569,62 @@
         self.log_times(latencies)
         return Response(content=np_to_bytes(result), media_type="image/png")
 
 
 # salient object detection (isnet)
 
 
+class Img2ImgSODModel(ReturnArraysModel, ImageModel):
+    pass
+
+
 @IAlgorithm.auto_register()
 class Img2ImgSOD(IAlgorithm):
-    model_class = ImageModel
+    model_class = Img2ImgSODModel
 
     endpoint = img2img_sod_endpoint
 
     def initialize(self) -> None:
         register_isnet()
 
-    async def run(self, data: ImageModel, *args: Any) -> Response:
+    async def run(self, data: Img2ImgSODModel, *args: Any) -> Response:
         self.log_endpoint(data)
         t0 = time.time()
         image = await self.download_image_with_retry(data.url)
         t1 = time.time()
         m = api_pool.get(APIs.ISNET)
         t2 = time.time()
-        alpha = to_uint8(m.segment(image))
-        content = np_to_bytes(alpha)
+        rgb = to_rgb(image)
+        alpha = to_uint8(m.segment(rgb))
+        content = None if data.return_arrays else np_to_bytes(alpha)
         t3 = time.time()
         api_pool.cleanup(APIs.ISNET)
         self.log_times(
             {
                 "download": t1 - t0,
                 "get_model": t2 - t1,
                 "inference": t3 - t2,
                 "cleanup": time.time() - t3,
             }
         )
+        if content is None:
+            return [np.concatenate([np.array(rgb), alpha[..., None]], axis=2)]
         return Response(content=content, media_type="image/png")
 
 
 __all__ = [
     "img2img_sd_endpoint",
     "img2img_sr_endpoint",
     "img2img_inpainting_endpoint",
     "img2img_semantic2img_endpoint",
     "img2img_harmonization_endpoint",
     "img2img_sod_endpoint",
     "Img2ImgSDModel",
     "Img2ImgSRModel",
+    "Img2ImgSODModel",
     "Img2ImgInpaintingModel",
     "Img2ImgSemantic2ImgModel",
     "Img2ImgSD",
     "Img2ImgSR",
     "Img2ImgInpainting",
     "Img2ImgSemantic2Img",
     "Img2ImgHarmonizationModel",
```

### Comparing `carefree-creator-0.2.1/cfcreator/img2txt.py` & `carefree-creator-0.2.2/cfcreator/img2txt.py`

 * *Files 5% similar despite different names*

```diff
@@ -55,9 +55,10 @@
             }
         )
         return TextModel(text=caption)
 
 
 __all__ = [
     "img2txt_caption_endpoint",
+    "Img2TxtModel",
     "Img2TxtCaption",
 ]
```

### Comparing `carefree-creator-0.2.1/cfcreator/parameters.py` & `carefree-creator-0.2.2/cfcreator/parameters.py`

 * *Files identical despite different names*

### Comparing `carefree-creator-0.2.1/cfcreator/pipeline.py` & `carefree-creator-0.2.2/cfcreator/pipeline.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,14 +39,15 @@
     original_bg: Image.Image,
     a: float,
     b: float,
     c: float,
     d: float,
     e: float,
     f: float,
+    force_rgb: bool,
 ) -> Tuple[Dict[str, np.ndarray], Dict[str, Any]]:
     t0 = time.time()
     if original_fg.mode != "RGBA":
         original_fg = original_fg.convert("RGBA")
     original_w, original_h = original_bg.size
     affined_fg_array = affine(
         np.array(original_fg),
@@ -56,31 +57,36 @@
         d,
         e,
         f,
         original_w,
         original_h,
     )
     t1 = time.time()
-    rgb = affined_fg_array[..., :3].astype(np.float32) / 255.0
-    mask = affined_fg_array[..., -1:].astype(np.float32) / 255.0
-    original_bg_array = np.array(to_rgb(original_bg)).astype(np.float32) / 255.0
-    merged = rgb * mask + original_bg_array * (1.0 - mask)
+    affined_fg_array = affined_fg_array.astype(np.float32) / 255.0
+    rgb = affined_fg_array[..., :3]
+    mask = affined_fg_array[..., -1:]
+    if force_rgb:
+        original_bg = to_rgb(original_bg)
+    bg_array = np.array(original_bg).astype(np.float32) / 255.0
+    fg_array = rgb if bg_array.shape[2] == 3 else affined_fg_array
+    merged = fg_array * mask + bg_array * (1.0 - mask)
     results = dict(rgb=rgb, mask=mask, merged=to_uint8(merged))
     latencies = {"affine": t1 - t0, "merge": time.time() - t1}
     return results, latencies
 
 
 class _PastePipelineModel(BaseModel):
     bg_url: str = Field(
         ...,
         description="""
 The `cdn` / `cos` url of the background's image.
 > `cos` url from `qcloud` is preferred.
 """,
     )
+    force_rgb: bool = Field(False, description="Whether to force the output to be RGB.")
 
 
 class PastePipelineModel(
     ReturnArraysModel,
     BaseAffineModel,
     _PastePipelineModel,
     ImageModel,
@@ -108,14 +114,15 @@
             original_bg,
             data.a,
             data.b,
             data.c,
             data.d,
             data.e,
             data.f,
+            data.force_rgb,
         )
         latencies["download"] = t1 - t0
         self.log_times(latencies)
         return get_response(data, [results["merged"]])
 
 
 __all__ = [
```

### Comparing `carefree-creator-0.2.1/cfcreator/sdks/direct.py` & `carefree-creator-0.2.2/cfcreator/sdks/direct.py`

 * *Files identical despite different names*

### Comparing `carefree-creator-0.2.1/cfcreator/sdks/kafka.py` & `carefree-creator-0.2.2/cfcreator/sdks/kafka.py`

 * *Files identical despite different names*

### Comparing `carefree-creator-0.2.1/cfcreator/sdks/utils.py` & `carefree-creator-0.2.2/cfcreator/sdks/utils.py`

 * *Files identical despite different names*

### Comparing `carefree-creator-0.2.1/cfcreator/txt2img.py` & `carefree-creator-0.2.2/cfcreator/txt2img.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,74 +1,85 @@
 import time
 
+import numpy as np
+
+from PIL import Image
 from enum import Enum
 from typing import Any
 from fastapi import Response
 from pydantic import Field
 from pydantic import BaseModel
+from cftool.cv import to_uint8
 from cfclient.models import ImageModel
 
 from .utils import api_pool
 from .utils import APIs
 from .common import register_sd
 from .common import register_sd_inpainting
 from .common import get_sd_from
 from .common import handle_diffusion_model
 from .common import get_bytes_from_diffusion
+from .common import get_normalized_arr_from_diffusion
 from .common import IAlgorithm
 from .common import Txt2ImgModel
+from .common import ReturnArraysModel
 from .common import CommonSDInpaintingModel
 
 
 txt2img_sd_endpoint = "/txt2img/sd"
 txt2img_sd_inpainting_endpoint = "/txt2img/sd.inpainting"
 txt2img_sd_outpainting_endpoint = "/txt2img/sd.outpainting"
 
 
 class _Txt2ImgSDModel(BaseModel):
     w: int = Field(512, description="The desired output width.")
     h: int = Field(512, description="The desired output height.")
 
 
-class Txt2ImgSDModel(Txt2ImgModel, _Txt2ImgSDModel):
+class Txt2ImgSDModel(ReturnArraysModel, Txt2ImgModel, _Txt2ImgSDModel):
     pass
 
 
 @IAlgorithm.auto_register()
 class Txt2ImgSD(IAlgorithm):
     model_class = Txt2ImgSDModel
 
     endpoint = txt2img_sd_endpoint
 
     def initialize(self) -> None:
         register_sd()
 
-    async def run(self, data: Txt2ImgSDModel, *args: Any) -> Response:
+    async def run(self, data: Txt2ImgSDModel, *args: Any, **kwargs: Any) -> Response:
         self.log_endpoint(data)
         t0 = time.time()
         m = get_sd_from(data)
         t1 = time.time()
         size = data.w, data.h
-        kwargs = handle_diffusion_model(m, data)
+        kwargs.update(handle_diffusion_model(m, data))
         img_arr = m.txt2img(
             data.text,
             size=size,
             max_wh=data.max_wh,
             **kwargs,
         ).numpy()[0]
-        content = get_bytes_from_diffusion(img_arr)
+        if data.return_arrays:
+            content = None
+        else:
+            content = get_bytes_from_diffusion(img_arr)
         t2 = time.time()
         api_pool.cleanup(APIs.SD)
         self.log_times(
             {
                 "get_model": t1 - t0,
                 "inference": t2 - t1,
                 "cleanup": time.time() - t2,
             }
         )
+        if content is None:
+            return [to_uint8(get_normalized_arr_from_diffusion(img_arr))]
         return Response(content=content, media_type="image/png")
 
 
 class PaddingModes(str, Enum):
     CV2_NS = "cv2_ns"
     CV2_TELEA = "cv2_telea"
 
@@ -94,91 +105,114 @@
 
     endpoint = txt2img_sd_inpainting_endpoint
 
     def initialize(self) -> None:
         register_sd()
         register_sd_inpainting()
 
-    async def run(self, data: Txt2ImgSDInpaintingModel, *args: Any) -> Response:
+    async def run(
+        self,
+        data: Txt2ImgSDInpaintingModel,
+        *args: Any,
+        **kwargs: Any,
+    ) -> Response:
         self.log_endpoint(data)
         t0 = time.time()
         image = await self.download_image_with_retry(data.url)
         mask = await self.download_image_with_retry(data.mask_url)
         t1 = time.time()
         if data.use_raw_inpainting:
             api_key = APIs.SD
             m = get_sd_from(data)
         else:
             api_key = APIs.SD_INPAINTING
             m = api_pool.get(api_key)
             m.disable_control()
         t2 = time.time()
-        kwargs = handle_diffusion_model(m, data)
+        kwargs.update(handle_diffusion_model(m, data))
         kwargs.update(await self.handle_diffusion_inpainting_model(data))
+        mask_arr = np.array(mask)
+        mask_arr[..., -1] = np.where(mask_arr[..., -1] > 0, 255, 0)
+        mask = Image.fromarray(mask_arr)
         img_arr = m.txt2img_inpainting(
             data.text,
             image,
             mask,
             anchor=64,
             max_wh=data.max_wh,
             keep_original=data.keep_original,
             **kwargs,
         ).numpy()[0]
-        content = get_bytes_from_diffusion(img_arr)
+        if data.return_arrays:
+            content = None
+        else:
+            content = get_bytes_from_diffusion(img_arr)
         t3 = time.time()
         api_pool.cleanup(api_key)
         self.log_times(
             {
                 "download": t1 - t0,
                 "get_model": t2 - t1,
                 "inference": t3 - t2,
                 "cleanup": time.time() - t3,
             }
         )
+        if content is None:
+            return [to_uint8(get_normalized_arr_from_diffusion(img_arr))]
         return Response(content=content, media_type="image/png")
 
 
 @IAlgorithm.auto_register()
 class Txt2ImgSDOutpainting(IAlgorithm):
     model_class = Txt2ImgSDOutpaintingModel
 
     endpoint = txt2img_sd_outpainting_endpoint
 
     def initialize(self) -> None:
         register_sd_inpainting()
 
-    async def run(self, data: Txt2ImgSDOutpaintingModel, *args: Any) -> Response:
+    async def run(
+        self,
+        data: Txt2ImgSDOutpaintingModel,
+        *args: Any,
+        **kwargs: Any,
+    ) -> Response:
         self.log_endpoint(data)
         t0 = time.time()
         image = await self.download_image_with_retry(data.url)
         t1 = time.time()
         m = api_pool.get(APIs.SD_INPAINTING)
         m.disable_control()
         t2 = time.time()
-        kwargs = handle_diffusion_model(m, data)
+        kwargs.update(handle_diffusion_model(m, data))
         kwargs.update(await self.handle_diffusion_inpainting_model(data))
         img_arr = m.outpainting(
             data.text,
             image,
             anchor=64,
             max_wh=data.max_wh,
             keep_original=data.keep_original,
             **kwargs,
         ).numpy()[0]
-        content = get_bytes_from_diffusion(img_arr)
+        if data.return_arrays:
+            content = None
+        else:
+            content = get_bytes_from_diffusion(img_arr)
         t3 = time.time()
         api_pool.cleanup(APIs.SD_INPAINTING)
         self.log_times(
             {
                 "download": t1 - t0,
                 "get_model": t2 - t1,
                 "inference": t3 - t2,
                 "cleanup": time.time() - t3,
             }
         )
+        if content is None:
+            return [to_uint8(get_normalized_arr_from_diffusion(img_arr))]
         return Response(content=content, media_type="image/png")
 
 
 __all__ = [
     "txt2img_sd_endpoint",
     "txt2img_sd_inpainting_endpoint",
     "txt2img_sd_outpainting_endpoint",
```

### Comparing `carefree-creator-0.2.1/cfcreator/txt2txt.py` & `carefree-creator-0.2.2/cfcreator/txt2txt.py`

 * *Files identical despite different names*

### Comparing `carefree-creator-0.2.1/cfcreator/utils.py` & `carefree-creator-0.2.2/cfcreator/utils.py`

 * *Files identical despite different names*

### Comparing `carefree-creator-0.2.1/setup.py` & `carefree-creator-0.2.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from setuptools import setup, find_packages
 
-VERSION = "0.2.1"
+VERSION = "0.2.2"
 PACKAGE_NAME = "carefree-creator"
 
 DESCRIPTION = "An AI-powered creator for everyone."
 with open("README.md", encoding="utf-8") as f:
     LONG_DESCRIPTION = f.read()
 
 setup(
     name=PACKAGE_NAME,
     version=VERSION,
     packages=find_packages(exclude=("tests",)),
     include_package_data=True,
     entry_points={"console_scripts": ["cfcreator = cfcreator.cli:main"]},
     install_requires=[
         "click>=8.1.3",
-        "fastapi==0.88.0",
+        "fastapi>=0.95.1",
         "carefree-client>=0.1.9",
-        "carefree-learn[cv_full]>=0.4.1",
+        "carefree-learn[cv_full]>=0.4.2",
     ],
     extras_require={
         "kafka": [
             "kafka-python",
             "redis[hiredis]",
             "cos-python-sdk-v5",
         ]
```

