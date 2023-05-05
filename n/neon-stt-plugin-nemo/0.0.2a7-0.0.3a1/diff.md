# Comparing `tmp/neon_stt_plugin_nemo-0.0.2a7-py3-none-any.whl.zip` & `tmp/neon_stt_plugin_nemo-0.0.3a1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 4950 bytes, number of entries: 8
--rw-r--r--  2.0 unx     3482 b- defN 23-Mar-14 18:37 neon_stt_plugin_nemo/__init__.py
--rw-r--r--  2.0 unx     1634 b- defN 23-Mar-14 18:37 neon_stt_plugin_nemo-0.0.2a7.dist-info/LICENSE.md
--rw-r--r--  2.0 unx      916 b- defN 23-Mar-14 18:37 neon_stt_plugin_nemo-0.0.2a7.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Mar-14 18:37 neon_stt_plugin_nemo-0.0.2a7.dist-info/WHEEL
--rw-r--r--  2.0 unx       73 b- defN 23-Mar-14 18:37 neon_stt_plugin_nemo-0.0.2a7.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       21 b- defN 23-Mar-14 18:37 neon_stt_plugin_nemo-0.0.2a7.dist-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 23-Mar-14 18:37 neon_stt_plugin_nemo-0.0.2a7.dist-info/zip-safe
--rw-rw-r--  2.0 unx      763 b- defN 23-Mar-14 18:37 neon_stt_plugin_nemo-0.0.2a7.dist-info/RECORD
-8 files, 6982 bytes uncompressed, 3578 bytes compressed:  48.8%
+Zip file size: 5012 bytes, number of entries: 8
+-rw-r--r--  2.0 unx     3586 b- defN 23-May-05 22:21 neon_stt_plugin_nemo/__init__.py
+-rw-r--r--  2.0 unx     1634 b- defN 23-May-05 22:21 neon_stt_plugin_nemo-0.0.3a1.dist-info/LICENSE.md
+-rw-r--r--  2.0 unx      966 b- defN 23-May-05 22:21 neon_stt_plugin_nemo-0.0.3a1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-05 22:21 neon_stt_plugin_nemo-0.0.3a1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       73 b- defN 23-May-05 22:21 neon_stt_plugin_nemo-0.0.3a1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       21 b- defN 23-May-05 22:21 neon_stt_plugin_nemo-0.0.3a1.dist-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-May-05 22:21 neon_stt_plugin_nemo-0.0.3a1.dist-info/zip-safe
+-rw-rw-r--  2.0 unx      763 b- defN 23-May-05 22:21 neon_stt_plugin_nemo-0.0.3a1.dist-info/RECORD
+8 files, 7136 bytes uncompressed, 3640 bytes compressed:  49.0%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
 Filename: neon_stt_plugin_nemo/__init__.py
 Comment: 
 
-Filename: neon_stt_plugin_nemo-0.0.2a7.dist-info/LICENSE.md
+Filename: neon_stt_plugin_nemo-0.0.3a1.dist-info/LICENSE.md
 Comment: 
 
-Filename: neon_stt_plugin_nemo-0.0.2a7.dist-info/METADATA
+Filename: neon_stt_plugin_nemo-0.0.3a1.dist-info/METADATA
 Comment: 
 
-Filename: neon_stt_plugin_nemo-0.0.2a7.dist-info/WHEEL
+Filename: neon_stt_plugin_nemo-0.0.3a1.dist-info/WHEEL
 Comment: 
 
-Filename: neon_stt_plugin_nemo-0.0.2a7.dist-info/entry_points.txt
+Filename: neon_stt_plugin_nemo-0.0.3a1.dist-info/entry_points.txt
 Comment: 
 
-Filename: neon_stt_plugin_nemo-0.0.2a7.dist-info/top_level.txt
+Filename: neon_stt_plugin_nemo-0.0.3a1.dist-info/top_level.txt
 Comment: 
 
-Filename: neon_stt_plugin_nemo-0.0.2a7.dist-info/zip-safe
+Filename: neon_stt_plugin_nemo-0.0.3a1.dist-info/zip-safe
 Comment: 
 
-Filename: neon_stt_plugin_nemo-0.0.2a7.dist-info/RECORD
+Filename: neon_stt_plugin_nemo-0.0.3a1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## neon_stt_plugin_nemo/__init__.py

```diff
@@ -24,15 +24,15 @@
 # OR PROFITS;  OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 import numpy as np
 
-from streaming_stt_nemo import Model
+from streaming_stt_nemo import Model, languages
 from ovos_plugin_manager.templates.stt import STT
 from ovos_utils.log import LOG
 from speech_recognition import AudioData
 
 
 class NemoSTT(STT):
     default_lang = "en"
@@ -56,14 +56,17 @@
             if self.cache_engines:
                 self._engines[language] = model
         else:
             model = self._engines[language]
 
         return model
 
+    @property
+    def available_languages(self) -> set:
+        return set(languages.keys())
 
     def execute(self, audio: AudioData, language = None):
         '''
         Executes speach recognition
 
         Parameters:
                     audio : input audio file path
```

## Comparing `neon_stt_plugin_nemo-0.0.2a7.dist-info/LICENSE.md` & `neon_stt_plugin_nemo-0.0.3a1.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `neon_stt_plugin_nemo-0.0.2a7.dist-info/METADATA` & `neon_stt_plugin_nemo-0.0.3a1.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-stt-plugin-nemo
-Version: 0.0.2a7
+Version: 0.0.3a1
 Summary: Nemo STT plugin for Neon
 Home-page: https://github.com/NeonGeckoCom/neon-stt-plugin-nemo
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3.0
 Keywords: mycroft plugin stt
 Classifier: Intended Audience :: Developers
@@ -13,14 +13,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: numpy
 Requires-Dist: ovos-plugin-manager (~=0.0.21)
 Requires-Dist: ovos-utils (~=0.0.30)
 Requires-Dist: streaming-stt-nemo (~=0.1)
 Requires-Dist: SpeechRecognition (~=3.8)
+Requires-Dist: mycroft-messagebus-client (~=0.10)
 
 # NeonAI Nemo STT Plugin 
 [Mycroft](https://mycroft-ai.gitbook.io/docs/mycroft-technologies/mycroft-core/plugins) compatible
 Neon Nemo STT Plugin Speech-to-Text.
 
 # Configuration:
 ```yaml
```

## Comparing `neon_stt_plugin_nemo-0.0.2a7.dist-info/RECORD` & `neon_stt_plugin_nemo-0.0.3a1.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-neon_stt_plugin_nemo/__init__.py,sha256=R7RA0qZmll_miF6swEUrE4DeOWdJMwrZpLhOqqdcOTo,3482
-neon_stt_plugin_nemo-0.0.2a7.dist-info/LICENSE.md,sha256=gxKa3HnxC7fSIlGFpLAiSAhQS22pIyVEyXmPQR2KlXM,1634
-neon_stt_plugin_nemo-0.0.2a7.dist-info/METADATA,sha256=PdiIiCXpwoVUUC406FAkPjBJBoTld8uD-Q1zyjf2rQA,916
-neon_stt_plugin_nemo-0.0.2a7.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-neon_stt_plugin_nemo-0.0.2a7.dist-info/entry_points.txt,sha256=GrVSOmJbddTpT2Z2JC9Xt5vsgpTZRFpyfwQ1E-HZWKQ,73
-neon_stt_plugin_nemo-0.0.2a7.dist-info/top_level.txt,sha256=paHfnP5olm0mLnGfvMW0UuUMQK_0rBDMIWZGpoUEh78,21
-neon_stt_plugin_nemo-0.0.2a7.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-neon_stt_plugin_nemo-0.0.2a7.dist-info/RECORD,,
+neon_stt_plugin_nemo/__init__.py,sha256=aOFVNOZfCrycYQRkwZH18LHGzqvlRuDXTQLBFh0nPnQ,3586
+neon_stt_plugin_nemo-0.0.3a1.dist-info/LICENSE.md,sha256=gxKa3HnxC7fSIlGFpLAiSAhQS22pIyVEyXmPQR2KlXM,1634
+neon_stt_plugin_nemo-0.0.3a1.dist-info/METADATA,sha256=rcaRzPy9FSu-1u-7UyvEShJh16fThqG8wJhAVR5O_OU,966
+neon_stt_plugin_nemo-0.0.3a1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+neon_stt_plugin_nemo-0.0.3a1.dist-info/entry_points.txt,sha256=GrVSOmJbddTpT2Z2JC9Xt5vsgpTZRFpyfwQ1E-HZWKQ,73
+neon_stt_plugin_nemo-0.0.3a1.dist-info/top_level.txt,sha256=paHfnP5olm0mLnGfvMW0UuUMQK_0rBDMIWZGpoUEh78,21
+neon_stt_plugin_nemo-0.0.3a1.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+neon_stt_plugin_nemo-0.0.3a1.dist-info/RECORD,,
```

