# Comparing `tmp/silero_api_server-0.0.6.tar.gz` & `tmp/silero_api_server-0.0.7.tar.gz`

## Comparing `silero_api_server-0.0.6.tar` & `silero_api_server-0.0.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 silero_api_server-0.0.6/.env
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 silero_api_server-0.0.6/requirements.txt
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 silero_api_server-0.0.6/run.ps1
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 silero_api_server-0.0.6/run.sh
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 silero_api_server-0.0.6/.github/workflows/publish-to-test-pypi.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 silero_api_server-0.0.6/silero_api_server/__init__.py
--rw-r--r--   0        0        0     2122 2020-02-02 00:00:00.000000 silero_api_server-0.0.6/silero_api_server/server.py
--rw-r--r--   0        0        0     2405 2020-02-02 00:00:00.000000 silero_api_server-0.0.6/silero_api_server/tts.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 silero_api_server-0.0.6/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 silero_api_server-0.0.6/LICENSE
--rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 silero_api_server-0.0.6/README.md
--rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 silero_api_server-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     2046 2020-02-02 00:00:00.000000 silero_api_server-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 silero_api_server-0.0.7/.env
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 silero_api_server-0.0.7/requirements.txt
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 silero_api_server-0.0.7/run.ps1
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 silero_api_server-0.0.7/run.sh
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 silero_api_server-0.0.7/.github/workflows/publish-to-test-pypi.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 silero_api_server-0.0.7/silero_api_server/__init__.py
+-rw-r--r--   0        0        0     2161 2020-02-02 00:00:00.000000 silero_api_server-0.0.7/silero_api_server/server.py
+-rw-r--r--   0        0        0     2405 2020-02-02 00:00:00.000000 silero_api_server-0.0.7/silero_api_server/tts.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 silero_api_server-0.0.7/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 silero_api_server-0.0.7/LICENSE
+-rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 silero_api_server-0.0.7/README.md
+-rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 silero_api_server-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     2046 2020-02-02 00:00:00.000000 silero_api_server-0.0.7/PKG-INFO
```

### Comparing `silero_api_server-0.0.6/.github/workflows/publish-to-test-pypi.yml` & `silero_api_server-0.0.7/.github/workflows/publish-to-test-pypi.yml`

 * *Files identical despite different names*

### Comparing `silero_api_server-0.0.6/silero_api_server/server.py` & `silero_api_server-0.0.7/silero_api_server/server.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from loguru import logger
 from typing import Optional
 
 dotenv.load_dotenv()
 HOSTNAME = os.getenv('TTS_SERVER_HOSTNAME')
 PORT = os.getenv('TTS_SERVER_PORT')
 LOCAL_URL = f"http://{HOSTNAME}:{PORT}"
-SAMPLE_PATH = 'samples'
+SAMPLE_PATH = os.path.join(os.path.dirname(__file__),'sample')
 
 tts_service = SileroTtsService(os.path.abspath(SAMPLE_PATH))
 app = FastAPI()
 
 # Make sure the samples directory exists
 if not os.path.exists(SAMPLE_PATH):
     os.mkdir(SAMPLE_PATH)
```

### Comparing `silero_api_server-0.0.6/silero_api_server/tts.py` & `silero_api_server-0.0.7/silero_api_server/tts.py`

 * *Files identical despite different names*

### Comparing `silero_api_server-0.0.6/LICENSE` & `silero_api_server-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `silero_api_server-0.0.6/README.md` & `silero_api_server-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `silero_api_server-0.0.6/pyproject.toml` & `silero_api_server-0.0.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "silero-api-server"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Ouoertheo", email="ouoertheo@tomeofjamin.net" },
 ]
 description = "A simple FastAPI server to host Silero TTS"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `silero_api_server-0.0.6/PKG-INFO` & `silero_api_server-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: silero-api-server
-Version: 0.0.6
+Version: 0.0.7
 Summary: A simple FastAPI server to host Silero TTS
 Project-URL: Homepage, https://github.com/ouoertheo/silero-api-server
 Project-URL: Bug Tracker, https://github.com/ouoertheo/silero-api-server/issues
 Author-email: Ouoertheo <ouoertheo@tomeofjamin.net>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

