# Comparing `tmp/silero_api_server-0.0.3.tar.gz` & `tmp/silero_api_server-0.0.6.tar.gz`

## Comparing `silero_api_server-0.0.3.tar` & `silero_api_server-0.0.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 silero_api_server-0.0.3/.env
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 silero_api_server-0.0.3/requirements.txt
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 silero_api_server-0.0.3/run.ps1
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 silero_api_server-0.0.3/run.sh
--rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 silero_api_server-0.0.3/.github/workflows/publish-to-test-pypi.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 silero_api_server-0.0.3/silero_api_server/__init__.py
--rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 silero_api_server-0.0.3/silero_api_server/server.py
--rw-r--r--   0        0        0     2298 2020-02-02 00:00:00.000000 silero_api_server-0.0.3/silero_api_server/tts.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 silero_api_server-0.0.3/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 silero_api_server-0.0.3/LICENSE
--rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 silero_api_server-0.0.3/README.md
--rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 silero_api_server-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     2046 2020-02-02 00:00:00.000000 silero_api_server-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 silero_api_server-0.0.6/.env
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 silero_api_server-0.0.6/requirements.txt
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 silero_api_server-0.0.6/run.ps1
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 silero_api_server-0.0.6/run.sh
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 silero_api_server-0.0.6/.github/workflows/publish-to-test-pypi.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 silero_api_server-0.0.6/silero_api_server/__init__.py
+-rw-r--r--   0        0        0     2122 2020-02-02 00:00:00.000000 silero_api_server-0.0.6/silero_api_server/server.py
+-rw-r--r--   0        0        0     2405 2020-02-02 00:00:00.000000 silero_api_server-0.0.6/silero_api_server/tts.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 silero_api_server-0.0.6/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 silero_api_server-0.0.6/LICENSE
+-rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 silero_api_server-0.0.6/README.md
+-rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 silero_api_server-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     2046 2020-02-02 00:00:00.000000 silero_api_server-0.0.6/PKG-INFO
```

### Comparing `silero_api_server-0.0.3/.github/workflows/publish-to-test-pypi.yml` & `silero_api_server-0.0.6/.github/workflows/publish-to-test-pypi.yml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 name: Publish Python 🐍 distributions 📦 to PyPI and TestPyPI
 on:
   push:
+    branches:
+      - master
+    tags:
+      - '*'
 jobs:
   build-n-publish:
     name: Build and publish Python 🐍 distributions 📦 to PyPI and TestPyPI
     runs-on: ubuntu-latest
     steps:
     - uses: actions/checkout@v3
     - name: Set up Python
```

### Comparing `silero_api_server-0.0.3/silero_api_server/tts.py` & `silero_api_server-0.0.6/silero_api_server/tts.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 from hashlib import md5
 from loguru import logger
 
 class SileroTtsService:
     """
     Generate TTS wav files using Silero
     """
-    def __init__(self) -> None:
+    def __init__(self, sample_path) -> None:
         self.sample_text = "The fallowed fallen swindle auspacious goats in portable power stations."
-
+        self.sample_path = sample_path
         # Silero works fine on CPU
         self.device = torch.device('cpu')
         torch.set_num_threads(4)
         torchaudio.set_audio_backend("soundfile")
 
         # Make sure we  have the model
         self.local_file = 'model.pt'
@@ -42,25 +42,25 @@
         audio = self.model.save_wav(text=text,speaker=speaker,sample_rate=self.sample_rate)
         return audio
 
     def get_speakers(self):
         return self.model.speakers
 
     def generate_samples(self):
-
         logger.warning("Removing current samples")
-        for file in os.listdir('samples'):
-            os.remove(f"samples/{file}")
+        for file in os.listdir(self.sample_path):
+            os.remove(f"{self.sample_path}/{file}")
 
         logger.info("Creating new samples. This should take a minute...")
         for speaker in self.model.speakers:
             name = f"{speaker}.wav"
             if os.path.exists(name):
                 continue
             audio = self.model.save_wav(text=self.sample_text,speaker=speaker,sample_rate=self.sample_rate)
-            os.rename(audio, f"samples/{name}")
+            os.rename(audio, f"{self.sample_path}/{name}")
         logger.info("New samples created")  
 
     def update_sample_text(self,text: str):
+        if not text: return
         self.sample_text = text
         logger.info(f"Sample text updated to {self.sample_text}")
```

### Comparing `silero_api_server-0.0.3/LICENSE` & `silero_api_server-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `silero_api_server-0.0.3/README.md` & `silero_api_server-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `silero_api_server-0.0.3/pyproject.toml` & `silero_api_server-0.0.6/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "silero-api-server"
-version = "0.0.3"
+version = "0.0.6"
 authors = [
   { name="Ouoertheo", email="ouoertheo@tomeofjamin.net" },
 ]
 description = "A simple FastAPI server to host Silero TTS"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `silero_api_server-0.0.3/PKG-INFO` & `silero_api_server-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: silero-api-server
-Version: 0.0.3
+Version: 0.0.6
 Summary: A simple FastAPI server to host Silero TTS
 Project-URL: Homepage, https://github.com/ouoertheo/silero-api-server
 Project-URL: Bug Tracker, https://github.com/ouoertheo/silero-api-server/issues
 Author-email: Ouoertheo <ouoertheo@tomeofjamin.net>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

