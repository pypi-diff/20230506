# Comparing `tmp/gradio_client-0.1.4.tar.gz` & `tmp/gradio_client-0.2.0.tar.gz`

## Comparing `gradio_client-0.1.4.tar` & `gradio_client-0.2.0.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0     5654 2020-02-02 00:00:00.000000 gradio_client-0.1.4/README.md
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 gradio_client-0.1.4/requirements.txt
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 gradio_client-0.1.4/gradio_client/__init__.py
--rw-r--r--   0        0        0    46264 2020-02-02 00:00:00.000000 gradio_client-0.1.4/gradio_client/client.py
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 gradio_client-0.1.4/gradio_client/data_classes.py
--rw-r--r--   0        0        0    10499 2020-02-02 00:00:00.000000 gradio_client-0.1.4/gradio_client/documentation.py
--rw-r--r--   0        0        0   722623 2020-02-02 00:00:00.000000 gradio_client-0.1.4/gradio_client/media_data.py
--rw-r--r--   0        0        0    20110 2020-02-02 00:00:00.000000 gradio_client-0.1.4/gradio_client/serializing.py
--rw-r--r--   0        0        0    14633 2020-02-02 00:00:00.000000 gradio_client-0.1.4/gradio_client/utils.py
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 gradio_client-0.1.4/gradio_client/version.txt
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 gradio_client-0.1.4/.gitignore
--rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 gradio_client-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     6410 2020-02-02 00:00:00.000000 gradio_client-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     5654 2020-02-02 00:00:00.000000 gradio_client-0.2.0/README.md
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 gradio_client-0.2.0/requirements.txt
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 gradio_client-0.2.0/gradio_client/__init__.py
+-rw-r--r--   0        0        0    46849 2020-02-02 00:00:00.000000 gradio_client-0.2.0/gradio_client/client.py
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 gradio_client-0.2.0/gradio_client/data_classes.py
+-rw-r--r--   0        0        0    10494 2020-02-02 00:00:00.000000 gradio_client-0.2.0/gradio_client/documentation.py
+-rw-r--r--   0        0        0   722623 2020-02-02 00:00:00.000000 gradio_client-0.2.0/gradio_client/media_data.py
+-rw-r--r--   0        0        0    18574 2020-02-02 00:00:00.000000 gradio_client-0.2.0/gradio_client/serializing.py
+-rw-r--r--   0        0        0     4356 2020-02-02 00:00:00.000000 gradio_client-0.2.0/gradio_client/types.json
+-rw-r--r--   0        0        0    16272 2020-02-02 00:00:00.000000 gradio_client-0.2.0/gradio_client/utils.py
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 gradio_client-0.2.0/gradio_client/version.txt
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 gradio_client-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 gradio_client-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     6410 2020-02-02 00:00:00.000000 gradio_client-0.2.0/PKG-INFO
```

### Comparing `gradio_client-0.1.4/README.md` & `gradio_client-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `gradio_client-0.1.4/gradio_client/client.py` & `gradio_client-0.2.0/gradio_client/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import urllib.parse
 import uuid
 import warnings
 from concurrent.futures import Future, TimeoutError
 from datetime import datetime
 from pathlib import Path
 from threading import Lock
-from typing import Any, Callable, Dict, List, Tuple
+from typing import Any, Callable
 
 import huggingface_hub
 import requests
 import websockets
 from huggingface_hub import SpaceStage
 from huggingface_hub.utils import (
     RepositoryNotFoundError,
@@ -26,15 +26,20 @@
 )
 from packaging import version
 from typing_extensions import Literal
 
 from gradio_client import serializing, utils
 from gradio_client.documentation import document, set_documentation_group
 from gradio_client.serializing import Serializable
-from gradio_client.utils import Communicator, JobStatus, Status, StatusUpdate
+from gradio_client.utils import (
+    Communicator,
+    JobStatus,
+    Status,
+    StatusUpdate,
+)
 
 set_documentation_group("py-client")
 
 
 @document("predict", "submit", "view_api", "duplicate")
 class Client:
     """
@@ -128,15 +133,15 @@
     def duplicate(
         cls,
         from_id: str,
         to_id: str | None = None,
         hf_token: str | None = None,
         private: bool = True,
         hardware: str | None = None,
-        secrets: Dict[str, str] | None = None,
+        secrets: dict[str, str] | None = None,
         sleep_timeout: int = 5,
         max_workers: int = 40,
         verbose: bool = True,
     ):
         """
         Duplicates a Hugging Face Space under your account and returns a Client object
         for the new Space. No duplication is created if the Space already exists in your
@@ -165,18 +170,18 @@
             HF_TOKEN = os.environ.get("HF_TOKEN")
             client = Client.duplicate("abidlabs/whisper", hf_token=HF_TOKEN)
             client.predict("audio_sample.wav")
             >> "This is a test of the whisper speech recognition model."
         """
         try:
             original_info = huggingface_hub.get_space_runtime(from_id, token=hf_token)
-        except RepositoryNotFoundError:
+        except RepositoryNotFoundError as rnfe:
             raise ValueError(
                 f"Could not find Space: {from_id}. If it is a private Space, please provide an `hf_token`."
-            )
+            ) from rnfe
         if to_id:
             if "/" in to_id:
                 to_id = to_id.split("/")[1]
             space_id = huggingface_hub.get_full_repo_name(to_id, token=hf_token)
         else:
             space_id = huggingface_hub.get_full_repo_name(
                 from_id.split("/")[1], token=hf_token
@@ -212,15 +217,15 @@
             if verbose:
                 print(f"Created new Space: {utils.SPACE_URL.format(space_id)}")
         current_info = huggingface_hub.get_space_runtime(space_id, token=hf_token)
         current_hardware = (
             current_info.hardware or huggingface_hub.SpaceHardware.CPU_BASIC
         )
         hardware = hardware or original_info.hardware
-        if not current_hardware == hardware:
+        if current_hardware != hardware:
             huggingface_hub.request_space_hardware(space_id, hardware)  # type: ignore
             print(
                 f"-------\nNOTE: this Space uses upgraded hardware: {hardware}... see billing info at https://huggingface.co/settings/billing\n-------"
             )
         if verbose:
             print("")
         client = cls(
@@ -258,15 +263,15 @@
         return self.submit(*args, api_name=api_name, fn_index=fn_index).result()
 
     def submit(
         self,
         *args,
         api_name: str | None = None,
         fn_index: int | None = None,
-        result_callbacks: Callable | List[Callable] | None = None,
+        result_callbacks: Callable | list[Callable] | None = None,
     ) -> Job:
         """
         Creates and returns a Job object which calls the Gradio API in a background thread. The job can be used to retrieve the status and result of the remote API call.
 
         Parameters:
             args: The arguments to pass to the remote API. The order of the arguments must match the order of the inputs in the Gradio app.
             api_name: The name of the API endpoint to call starting with a leading slash, e.g. "/predict". Does not need to be provided if the Gradio app has only one named API endpoint.
@@ -319,15 +324,15 @@
         return job
 
     def view_api(
         self,
         all_endpoints: bool | None = None,
         print_info: bool = True,
         return_format: Literal["dict", "str"] | None = None,
-    ) -> Dict | str | None:
+    ) -> dict | str | None:
         """
         Prints the usage info for the API. If the Gradio app has multiple API endpoints, the usage info for each endpoint will be printed separately. If return_format="dict" the info is returned in dictionary format, as shown in the example below.
 
         Parameters:
             all_endpoints: If True, prints information for both named and unnamed endpoints in the Gradio app. If False, will only print info about named endpoints. If None (default), will only print info about unnamed endpoints if there are no named endpoints.
             print_info: If True, prints the usage info to the console. If False, does not print the usage info.
             return_format: If None, nothing is returned. If "str", returns the same string that would be printed to the console. If "dict", returns the usage info as a dictionary that can be programmatically parsed, and *all endpoints are returned in the dictionary* regardless of the value of `all_endpoints`. The format of the dictionary is in the docstring of this method.
@@ -395,25 +400,25 @@
         """
         if self.serialize:
             api_info_url = urllib.parse.urljoin(self.src, utils.API_INFO_URL)
         else:
             api_info_url = urllib.parse.urljoin(self.src, utils.RAW_API_INFO_URL)
         r = requests.get(api_info_url, headers=self.headers)
 
-        # Versions of Gradio older than 3.26 returned format of the API info
+        # Versions of Gradio older than 3.28.3 returned format of the API info
         # from the /info endpoint
         if (
-            version.parse(self.config.get("version", "2.0")) >= version.Version("3.26")
+            version.parse(self.config.get("version", "2.0")) > version.Version("3.28.3")
             and r.ok
         ):
             info = r.json()
         else:
             fetch = requests.post(
                 utils.SPACE_FETCHER_URL,
-                json={"serialize": self.serialize, "config": json.dumps(self.config)},
+                json={"config": json.dumps(self.config), "serialize": self.serialize},
             )
             if fetch.ok:
                 info = fetch.json()["api"]
             else:
                 raise ValueError(f"Could not fetch api info for {self.src}")
         num_named_endpoints = len(info["named_endpoints"])
         num_unnamed_endpoints = len(info["unnamed_endpoints"])
@@ -445,22 +450,22 @@
 
     def reset_session(self) -> None:
         self.session_hash = str(uuid.uuid4())
 
     def _render_endpoints_info(
         self,
         name_or_index: str | int,
-        endpoints_info: Dict[str, List[Dict[str, str]]],
+        endpoints_info: dict[str, list[dict[str, Any]]],
     ) -> str:
-        parameter_names = list(p["label"] for p in endpoints_info["parameters"])
+        parameter_names = [p["label"] for p in endpoints_info["parameters"]]
         parameter_names = [utils.sanitize_parameter_names(p) for p in parameter_names]
         rendered_parameters = ", ".join(parameter_names)
         if rendered_parameters:
             rendered_parameters = rendered_parameters + ", "
-        return_values = list(p["label"] for p in endpoints_info["returns"])
+        return_values = [p["label"] for p in endpoints_info["returns"]]
         return_values = [utils.sanitize_parameter_names(r) for r in return_values]
         rendered_return_values = ", ".join(return_values)
         if len(return_values) > 1:
             rendered_return_values = f"({rendered_return_values})"
 
         if isinstance(name_or_index, str):
             final_param = f'api_name="{name_or_index}"'
@@ -469,21 +474,33 @@
         else:
             raise ValueError("name_or_index must be a string or integer")
 
         human_info = f"\n - predict({rendered_parameters}{final_param}) -> {rendered_return_values}\n"
         human_info += "    Parameters:\n"
         if endpoints_info["parameters"]:
             for info in endpoints_info["parameters"]:
-                human_info += f"     - [{info['component']}] {utils.sanitize_parameter_names(info['label'])}: {info['type_python']} ({info['type_description']})\n"
+                desc = (
+                    f" ({info['python_type']['description']})"
+                    if info["python_type"].get("description")
+                    else ""
+                )
+                type_ = info["python_type"]["type"]
+                human_info += f"     - [{info['component']}] {utils.sanitize_parameter_names(info['label'])}: {type_}{desc} \n"
         else:
             human_info += "     - None\n"
         human_info += "    Returns:\n"
         if endpoints_info["returns"]:
             for info in endpoints_info["returns"]:
-                human_info += f"     - [{info['component']}] {utils.sanitize_parameter_names(info['label'])}: {info['type_python']} ({info['type_description']})\n"
+                desc = (
+                    f" ({info['python_type']['description']})"
+                    if info["python_type"].get("description")
+                    else ""
+                )
+                type_ = info["python_type"]["type"]
+                human_info += f"     - [{info['component']}] {utils.sanitize_parameter_names(info['label'])}: {type_}{desc} \n"
         else:
             human_info += "     - None\n"
 
         return human_info
 
     def __repr__(self):
         return self.view_api(print_info=False, return_format="str")
@@ -538,39 +555,41 @@
     def __del__(self):
         if hasattr(self, "executor"):
             self.executor.shutdown(wait=True)
 
     def _space_name_to_src(self, space) -> str | None:
         return huggingface_hub.space_info(space, token=self.hf_token).host  # type: ignore
 
-    def _get_config(self) -> Dict:
+    def _get_config(self) -> dict:
         r = requests.get(
             urllib.parse.urljoin(self.src, utils.CONFIG_URL), headers=self.headers
         )
         if r.ok:
             return r.json()
         else:  # to support older versions of Gradio
             r = requests.get(self.src, headers=self.headers)
             # some basic regex to extract the config
             result = re.search(r"window.gradio_config = (.*?);[\s]*</script>", r.text)
             try:
                 config = json.loads(result.group(1))  # type: ignore
-            except AttributeError:
-                raise ValueError(f"Could not get Gradio config from: {self.src}")
+            except AttributeError as ae:
+                raise ValueError(
+                    f"Could not get Gradio config from: {self.src}"
+                ) from ae
             if "allow_flagging" in config:
                 raise ValueError(
                     "Gradio 2.x is not supported by this client. Please upgrade your Gradio app to Gradio 3.x or higher."
                 )
             return config
 
 
 class Endpoint:
     """Helper class for storing all the information about a single API endpoint."""
 
-    def __init__(self, client: Client, fn_index: int, dependency: Dict):
+    def __init__(self, client: Client, fn_index: int, dependency: dict):
         self.client: Client = client
         self.fn_index = fn_index
         self.dependency = dependency
         api_name = dependency.get("api_name")
         self.api_name: str | None = None if api_name is None else "/" + api_name
         self.use_ws = self._use_websocket(self.dependency)
         self.input_component_types = []
@@ -609,15 +628,15 @@
                     if not helper.job.outputs:
                         helper.job.outputs.append(predictions)
             return predictions
 
         return _inner
 
     def make_predict(self, helper: Communicator | None = None):
-        def _predict(*data) -> Tuple:
+        def _predict(*data) -> tuple:
             data = json.dumps(
                 {
                     "data": data,
                     "fn_index": self.fn_index,
                     "session_hash": self.client.session_hash,
                 }
             )
@@ -635,55 +654,57 @@
             else:
                 response = requests.post(
                     self.client.api_url, headers=self.client.headers, data=data
                 )
                 result = json.loads(response.content.decode("utf-8"))
             try:
                 output = result["data"]
-            except KeyError:
+            except KeyError as ke:
                 is_public_space = (
                     self.client.space_id
                     and not huggingface_hub.space_info(self.client.space_id).private
                 )
                 if "error" in result and "429" in result["error"] and is_public_space:
                     raise utils.TooManyRequestsError(
-                        f"Too many requests to the API, please try again later. To avoid being rate-limited, please duplicate the Space using Client.duplicate({self.client.space_id}) and pass in your Hugging Face token."
-                    )
+                        f"Too many requests to the API, please try again later. To avoid being rate-limited, "
+                        f"please duplicate the Space using Client.duplicate({self.client.space_id}) "
+                        f"and pass in your Hugging Face token."
+                    ) from None
                 elif "error" in result:
-                    raise ValueError(result["error"])
+                    raise ValueError(result["error"]) from None
                 raise KeyError(
                     f"Could not find 'data' key in response. Response received: {result}"
-                )
+                ) from ke
             return tuple(output)
 
         return _predict
 
     def _predict_resolve(self, *data) -> Any:
         """Needed for gradio.load(), which has a slightly different signature for serializing/deserializing"""
         outputs = self.make_predict()(*data)
         if len(self.dependency["outputs"]) == 1:
             return outputs[0]
         return outputs
 
     def _upload(
-        self, file_paths: List[str | List[str]]
-    ) -> List[str | List[str]] | List[Dict[str, Any] | List[Dict[str, Any]]]:
+        self, file_paths: list[str | list[str]]
+    ) -> list[str | list[str]] | list[dict[str, Any] | list[dict[str, Any]]]:
         if not file_paths:
             return []
         # Put all the filepaths in one file
         # but then keep track of which index in the
         # original list they came from so we can recreate
         # the original structure
         files = []
         indices = []
         for i, fs in enumerate(file_paths):
             if not isinstance(fs, list):
                 fs = [fs]
             for f in fs:
-                files.append(("files", (Path(f).name, open(f, "rb"))))
+                files.append(("files", (Path(f).name, open(f, "rb"))))  # noqa: SIM115
                 indices.append(i)
         r = requests.post(
             self.client.upload_url, headers=self.client.headers, files=files
         )
         if r.status_code != 200:
             uploaded = file_paths
         else:
@@ -710,25 +731,25 @@
                         "data": None,
                     }
                 uploaded.append(res)
         return uploaded
 
     def _add_uploaded_files_to_data(
         self,
-        files: List[str | List[str]] | List[Dict[str, Any] | List[Dict[str, Any]]],
-        data: List[Any],
+        files: list[str | list[str]] | list[dict[str, Any] | list[dict[str, Any]]],
+        data: list[Any],
     ) -> None:
         """Helper function to modify the input data with the uploaded files."""
         file_counter = 0
         for i, t in enumerate(self.input_component_types):
             if t in ["file", "uploadbutton"]:
                 data[i] = files[file_counter]
                 file_counter += 1
 
-    def serialize(self, *data) -> Tuple:
+    def serialize(self, *data) -> tuple:
         data = list(data)
         for i, input_component_type in enumerate(self.input_component_types):
             if input_component_type == utils.STATE_COMPONENT:
                 data.insert(i, None)
         assert len(data) == len(
             self.serializers
         ), f"Expected {len(self.serializers)} arguments, got {len(data)}"
@@ -740,43 +761,43 @@
         ]
         uploaded_files = self._upload(files)
         self._add_uploaded_files_to_data(uploaded_files, data)
 
         o = tuple([s.serialize(d) for s, d in zip(self.serializers, data)])
         return o
 
-    def deserialize(self, *data) -> Tuple | Any:
+    def deserialize(self, *data) -> tuple | Any:
         assert len(data) == len(
             self.deserializers
         ), f"Expected {len(self.deserializers)} outputs, got {len(data)}"
         outputs = tuple(
             [
                 s.deserialize(d, hf_token=self.client.hf_token, root_url=self.root_url)
                 for s, d, oct in zip(
                     self.deserializers, data, self.output_component_types
                 )
-                if not oct == utils.STATE_COMPONENT
+                if oct != utils.STATE_COMPONENT
             ]
         )
         if (
             len(
                 [
                     oct
                     for oct in self.output_component_types
-                    if not oct == utils.STATE_COMPONENT
+                    if oct != utils.STATE_COMPONENT
                 ]
             )
             == 1
         ):
             output = outputs[0]
         else:
             output = outputs
         return output
 
-    def _setup_serializers(self) -> Tuple[List[Serializable], List[Serializable]]:
+    def _setup_serializers(self) -> tuple[list[Serializable], list[Serializable]]:
         inputs = self.dependency["inputs"]
         serializers = []
 
         for i in inputs:
             for component in self.client.config["components"]:
                 if component["id"] == i:
                     component_name = component["type"]
@@ -812,15 +833,15 @@
                             component_name in serializing.COMPONENT_MAPPING
                         ), f"Unknown component: {component_name}, you may need to update your gradio_client version."
                         deserializer = serializing.COMPONENT_MAPPING[component_name]
                     deserializers.append(deserializer())  # type: ignore
 
         return serializers, deserializers
 
-    def _use_websocket(self, dependency: Dict) -> bool:
+    def _use_websocket(self, dependency: dict) -> bool:
         queue_enabled = self.client.config.get("enable_queue", False)
         queue_uses_websocket = version.parse(
             self.client.config.get("version", "2.0")
         ) >= version.Version("3.2")
         dependency_uses_queue = dependency.get("queue", False) is not False
         return queue_enabled and queue_uses_websocket and dependency_uses_queue
 
@@ -865,15 +886,15 @@
         self._counter = 0
         self.verbose = verbose
         self.space_id = space_id
 
     def __iter__(self) -> Job:
         return self
 
-    def __next__(self) -> Tuple | Any:
+    def __next__(self) -> tuple | Any:
         if not self.communicator:
             raise StopIteration()
 
         with self.communicator.lock:
             if self.communicator.job.latest_status.code == Status.FINISHED:
                 raise StopIteration()
 
@@ -917,15 +938,15 @@
                 with self.communicator.lock:
                     if self.communicator.job.outputs:
                         return self.communicator.job.outputs[0]
                 time.sleep(0.01)
         else:
             return super().result(timeout=timeout)
 
-    def outputs(self) -> List[Tuple | Any]:
+    def outputs(self) -> list[tuple | Any]:
         """
         Returns a list containing the latest outputs from the Job.
 
         If the endpoint has multiple output components, the list will contain
         a tuple of results. Otherwise, it will contain the results without storing them
         in tuples.
```

### Comparing `gradio_client-0.1.4/gradio_client/documentation.py` & `gradio_client-0.2.0/gradio_client/documentation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Contains methods that generate documentation for Gradio functions and classes."""
 
 from __future__ import annotations
 
 import inspect
-from typing import Callable, Dict, List, Tuple
+from typing import Callable
 
 classes_to_document = {}
 classes_inherit_documentation = {}
 documentation_group = None
 
 
 def set_documentation_group(m):
@@ -17,15 +17,15 @@
         classes_to_document[m] = []
 
 
 def extract_instance_attr_doc(cls, attr):
     code = inspect.getsource(cls.__init__)
     lines = [line.strip() for line in code.split("\n")]
     i = None
-    for i, line in enumerate(lines):
+    for i, line in enumerate(lines):  # noqa: B007
         if line.startswith("self." + attr + ":") or line.startswith(
             "self." + attr + " ="
         ):
             break
     assert i is not None, f"Could not find {attr} in {cls.__name__}"
     start_line = lines.index('"""', i)
     end_line = lines.index('"""', start_line + 1)
@@ -57,15 +57,15 @@
             classes_inherit_documentation[cls] = None
         classes_to_document[documentation_group].append((cls, fns))
         return cls
 
     return inner_doc
 
 
-def document_fn(fn: Callable, cls) -> Tuple[str, List[Dict], Dict, str | None]:
+def document_fn(fn: Callable, cls) -> tuple[str, list[dict], dict, str | None]:
     """
     Generates documentation for any function.
     Parameters:
         fn: Function to document
     Returns:
         description: General description of fn
         parameters: A list of dicts for each parameter, storing data for the parameter name, annotation and doc
```

### Comparing `gradio_client-0.1.4/gradio_client/media_data.py` & `gradio_client-0.2.0/gradio_client/media_data.py`

 * *Files identical despite different names*

### Comparing `gradio_client-0.1.4/gradio_client/serializing.py` & `gradio_client-0.2.0/gradio_client/serializing.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,42 +1,50 @@
 from __future__ import annotations
 
 import json
 import os
 import uuid
-from abc import ABC
 from pathlib import Path
-from typing import Any, Dict, List, Tuple
+from typing import Any
 
 from gradio_client import media_data, utils
 from gradio_client.data_classes import FileData
 
+serializer_types = json.load(open(Path(__file__).parent / "types.json"))
 
-class Serializable(ABC):
-    def api_info(self) -> Dict[str, List[str]]:
+
+class Serializable:
+    def serialized_info(self):
+        """
+        The typing information for this component as a dictionary whose values are a list of 2 strings: [Python type, language-agnostic description].
+        Keys of the dictionary are: raw_input, raw_output, serialized_input, serialized_output
+        """
+        return self.api_info()
+
+    def api_info(self) -> dict[str, list[str]]:
         """
         The typing information for this component as a dictionary whose values are a list of 2 strings: [Python type, language-agnostic description].
         Keys of the dictionary are: raw_input, raw_output, serialized_input, serialized_output
         """
         raise NotImplementedError()
 
-    def example_inputs(self) -> Dict[str, Any]:
+    def example_inputs(self) -> dict[str, Any]:
         """
         The example inputs for this component as a dictionary whose values are example inputs compatible with this component.
         Keys of the dictionary are: raw, serialized
         """
         raise NotImplementedError()
 
     # For backwards compatibility
-    def input_api_info(self) -> Tuple[str, str]:
+    def input_api_info(self) -> tuple[str, str]:
         api_info = self.api_info()
         return (api_info["serialized_input"][0], api_info["serialized_input"][1])
 
     # For backwards compatibility
-    def output_api_info(self) -> Tuple[str, str]:
+    def output_api_info(self) -> tuple[str, str]:
         api_info = self.api_info()
         return (api_info["serialized_output"][0], api_info["serialized_output"][1])
 
     def serialize(self, x: Any, load_dir: str | Path = ""):
         """
         Convert data from human-readable format to serialized format for a browser.
         """
@@ -54,113 +62,101 @@
         """
         return x
 
 
 class SimpleSerializable(Serializable):
     """General class that does not perform any serialization or deserialization."""
 
-    def api_info(self) -> Dict[str, str | List[str]]:
+    def api_info(self) -> dict[str, bool | dict]:
         return {
-            "raw_input": ["Any", ""],
-            "raw_output": ["Any", ""],
-            "serialized_input": ["Any", ""],
-            "serialized_output": ["Any", ""],
+            "info": serializer_types["SimpleSerializable"],
+            "serialized_info": False,
         }
 
-    def example_inputs(self) -> Dict[str, Any]:
+    def example_inputs(self) -> dict[str, Any]:
         return {
             "raw": None,
             "serialized": None,
         }
 
 
 class StringSerializable(Serializable):
     """Expects a string as input/output but performs no serialization."""
 
-    def api_info(self) -> Dict[str, List[str]]:
+    def api_info(self) -> dict[str, bool | dict]:
         return {
-            "raw_input": ["str", "string value"],
-            "raw_output": ["str", "string value"],
-            "serialized_input": ["str", "string value"],
-            "serialized_output": ["str", "string value"],
+            "info": serializer_types["StringSerializable"],
+            "serialized_info": False,
         }
 
-    def example_inputs(self) -> Dict[str, Any]:
+    def example_inputs(self) -> dict[str, Any]:
         return {
             "raw": "Howdy!",
             "serialized": "Howdy!",
         }
 
 
 class ListStringSerializable(Serializable):
     """Expects a list of strings as input/output but performs no serialization."""
 
-    def api_info(self) -> Dict[str, List[str]]:
+    def api_info(self) -> dict[str, bool | dict]:
         return {
-            "raw_input": ["List[str]", "list of string values"],
-            "raw_output": ["List[str]", "list of string values"],
-            "serialized_input": ["List[str]", "list of string values"],
-            "serialized_output": ["List[str]", "list of string values"],
+            "info": serializer_types["ListStringSerializable"],
+            "serialized_info": False,
         }
 
-    def example_inputs(self) -> Dict[str, Any]:
+    def example_inputs(self) -> dict[str, Any]:
         return {
             "raw": ["Howdy!", "Merhaba"],
             "serialized": ["Howdy!", "Merhaba"],
         }
 
 
 class BooleanSerializable(Serializable):
     """Expects a boolean as input/output but performs no serialization."""
 
-    def api_info(self) -> Dict[str, List[str]]:
+    def api_info(self) -> dict[str, bool | dict]:
         return {
-            "raw_input": ["bool", "boolean value"],
-            "raw_output": ["bool", "boolean value"],
-            "serialized_input": ["bool", "boolean value"],
-            "serialized_output": ["bool", "boolean value"],
+            "info": serializer_types["BooleanSerializable"],
+            "serialized_info": False,
         }
 
-    def example_inputs(self) -> Dict[str, Any]:
+    def example_inputs(self) -> dict[str, Any]:
         return {
             "raw": True,
             "serialized": True,
         }
 
 
 class NumberSerializable(Serializable):
     """Expects a number (int/float) as input/output but performs no serialization."""
 
-    def api_info(self) -> Dict[str, List[str]]:
+    def api_info(self) -> dict[str, bool | dict]:
         return {
-            "raw_input": ["int | float", "numeric value"],
-            "raw_output": ["int | float", "numeric value"],
-            "serialized_input": ["int | float", "numeric value"],
-            "serialized_output": ["int | float", "numeric value"],
+            "info": serializer_types["NumberSerializable"],
+            "serialized_info": False,
         }
 
-    def example_inputs(self) -> Dict[str, Any]:
+    def example_inputs(self) -> dict[str, Any]:
         return {
             "raw": 5,
             "serialized": 5,
         }
 
 
 class ImgSerializable(Serializable):
     """Expects a base64 string as input/output which is serialized to a filepath."""
 
-    def api_info(self) -> Dict[str, List[str]]:
-        return {
-            "raw_input": ["str", "base64 representation of image"],
-            "raw_output": ["str", "base64 representation of image"],
-            "serialized_input": ["str", "filepath or URL to image"],
-            "serialized_output": ["str", "filepath or URL to image"],
-        }
+    def serialized_info(self):
+        return {"type": "string", "description": "filepath or URL to image"}
+
+    def api_info(self) -> dict[str, bool | dict]:
+        return {"info": serializer_types["ImgSerializable"], "serialized_info": True}
 
-    def example_inputs(self) -> Dict[str, Any]:
+    def example_inputs(self) -> dict[str, Any]:
         return {
             "raw": media_data.BASE64_IMAGE,
             "serialized": "https://raw.githubusercontent.com/gradio-app/gradio/main/test/test_files/bus.png",
         }
 
     def serialize(
         self,
@@ -201,29 +197,43 @@
         file = utils.decode_base64_to_file(x, dir=save_dir)
         return file.name
 
 
 class FileSerializable(Serializable):
     """Expects a dict with base64 representation of object as input/output which is serialized to a filepath."""
 
-    def api_info(self) -> Dict[str, List[str]]:
+    def serialized_info(self):
+        return self._single_file_serialized_info()
+
+    def _single_file_api_info(self):
+        return {
+            "info": serializer_types["SingleFileSerializable"],
+            "serialized_info": True,
+        }
+
+    def _single_file_serialized_info(self):
+        return {"type": "string", "description": "filepath or URL to file"}
+
+    def _multiple_file_serialized_info(self):
         return {
-            "raw_input": [
-                "str | Dict",
-                "base64 string representation of file; or a dictionary-like object, the keys should be either: is_file (False), data (base64 representation of file) or is_file (True), name (str filename)",
-            ],
-            "raw_output": [
-                "Dict",
-                "dictionary-like object with keys: name (str filename), data (base64 representation of file), is_file (bool, set to False)",
-            ],
-            "serialized_input": ["str", "filepath or URL to file"],
-            "serialized_output": ["str", "filepath or URL to file"],
+            "type": "array",
+            "description": "List of filepath(s) or URL(s) to files",
+            "items": {"type": "string", "description": "filepath or URL to file"},
         }
 
-    def example_inputs(self) -> Dict[str, Any]:
+    def _multiple_file_api_info(self):
+        return {
+            "info": serializer_types["MultipleFileSerializable"],
+            "serialized_info": True,
+        }
+
+    def api_info(self) -> dict[str, dict | bool]:
+        return self._single_file_api_info()
+
+    def example_inputs(self) -> dict[str, Any]:
         return {
             "raw": {"is_file": False, "data": media_data.BASE64_FILE},
             "serialized": "https://github.com/gradio-app/gradio/raw/main/test/test_files/sample_file.pdf",
         }
 
     def _serialize_single(
         self, x: str | FileData | None, load_dir: str | Path = ""
@@ -277,17 +287,17 @@
             raise ValueError(
                 f"A FileSerializable component can only deserialize a string or a dict, not a {type(x)}: {x}"
             )
         return file_name
 
     def serialize(
         self,
-        x: str | FileData | None | List[str | FileData | None],
+        x: str | FileData | None | list[str | FileData | None],
         load_dir: str | Path = "",
-    ) -> FileData | None | List[FileData | None]:
+    ) -> FileData | None | list[FileData | None]:
         """
         Convert from human-friendly version of a file (string filepath) to a
         seralized representation (base64)
         Parameters:
             x: String path to file to serialize
             load_dir: Path to directory containing x
         """
@@ -296,19 +306,19 @@
         if isinstance(x, list):
             return [self._serialize_single(f, load_dir=load_dir) for f in x]
         else:
             return self._serialize_single(x, load_dir=load_dir)
 
     def deserialize(
         self,
-        x: str | FileData | None | List[str | FileData | None],
+        x: str | FileData | None | list[str | FileData | None],
         save_dir: Path | str | None = None,
         root_url: str | None = None,
         hf_token: str | None = None,
-    ) -> str | None | List[str | None]:
+    ) -> str | None | list[str | None]:
         """
         Convert from serialized representation of a file (base64) to a human-friendly
         version (string filepath). Optionally, save the file to the directory specified by `save_dir`
         Parameters:
             x: Base64 representation of file to deserialize into a string filepath
             save_dir: Path to directory to save the deserialized file to
             root_url: If this component is loaded from an external Space, this is the URL of the Space.
@@ -328,46 +338,38 @@
         else:
             return self._deserialize_single(
                 x, save_dir=save_dir, root_url=root_url, hf_token=hf_token
             )
 
 
 class VideoSerializable(FileSerializable):
-    def api_info(self) -> Dict[str, List[str]]:
-        return {
-            "raw_input": [
-                "str | Dict",
-                "base64 string representation of file; or a dictionary-like object, the keys should be either: is_file (False), data (base64 representation of file) or is_file (True), name (str filename)",
-            ],
-            "raw_output": [
-                "Tuple[Dict, Dict]",
-                "a tuple of 2 dictionary-like object with keys: name (str filename), data (base64 representation of file), is_file (bool, set to False). First dictionary is for the video, second dictionary is for the subtitles.",
-            ],
-            "serialized_input": ["str", "filepath or URL to file"],
-            "serialized_output": ["str", "filepath or URL to file"],
-        }
+    def serialized_info(self):
+        return {"type": "string", "description": "filepath or URL to video file"}
+
+    def api_info(self) -> dict[str, dict | bool]:
+        return {"info": serializer_types["FileSerializable"], "serialized_info": True}
 
-    def example_inputs(self) -> Dict[str, Any]:
+    def example_inputs(self) -> dict[str, Any]:
         return {
             "raw": {"is_file": False, "data": media_data.BASE64_VIDEO},
             "serialized": "https://github.com/gradio-app/gradio/raw/main/test/test_files/video_sample.mp4",
         }
 
     def serialize(
         self, x: str | None, load_dir: str | Path = ""
-    ) -> Tuple[FileData | None, None]:
+    ) -> tuple[FileData | None, None]:
         return (super().serialize(x, load_dir), None)  # type: ignore
 
     def deserialize(
         self,
-        x: Tuple[FileData | None, FileData | None] | None,
+        x: tuple[FileData | None, FileData | None] | None,
         save_dir: Path | str | None = None,
         root_url: str | None = None,
         hf_token: str | None = None,
-    ) -> str | Tuple[str | None, str | None] | None:
+    ) -> str | tuple[str | None, str | None] | None:
         """
         Convert from serialized representation of a file (base64) to a human-friendly
         version (string filepath). Optionally, save the file to the directory specified by `save_dir`
         """
         if isinstance(x, (tuple, list)):
             assert len(x) == 2, f"Expected tuple of length 2. Received: {x}"
             x_as_list = [x[0], x[1]]
@@ -375,47 +377,45 @@
             raise ValueError(f"Expected tuple of length 2. Received: {x}")
         deserialized_file = super().deserialize(x_as_list, save_dir, root_url, hf_token)  # type: ignore
         if isinstance(deserialized_file, list):
             return deserialized_file[0]  # ignore subtitles
 
 
 class JSONSerializable(Serializable):
-    def api_info(self) -> Dict[str, List[str]]:
-        return {
-            "raw_input": ["str | Dict | List", "JSON-serializable object or a string"],
-            "raw_output": ["Dict | List", "dictionary- or list-like object"],
-            "serialized_input": ["str", "filepath to JSON file"],
-            "serialized_output": ["str", "filepath to JSON file"],
-        }
+    def serialized_info(self):
+        return {"type": "string", "description": "filepath to JSON file"}
+
+    def api_info(self) -> dict[str, dict | bool]:
+        return {"info": serializer_types["JSONSerializable"], "serialized_info": True}
 
-    def example_inputs(self) -> Dict[str, Any]:
+    def example_inputs(self) -> dict[str, Any]:
         return {
             "raw": {"a": 1, "b": 2},
             "serialized": None,
         }
 
     def serialize(
         self,
         x: str | None,
         load_dir: str | Path = "",
-    ) -> Dict | List | None:
+    ) -> dict | list | None:
         """
         Convert from a a human-friendly version (string path to json file) to a
         serialized representation (json string)
         Parameters:
             x: String path to json file to read to get json string
             load_dir: Path to directory containing x
         """
         if x is None or x == "":
             return None
         return utils.file_to_json(Path(load_dir) / x)
 
     def deserialize(
         self,
-        x: str | Dict | List,
+        x: str | dict | list,
         save_dir: str | Path | None = None,
         root_url: str | None = None,
         hf_token: str | None = None,
     ) -> str | None:
         """
         Convert from serialized representation (json string) to a human-friendly
         version (string path to json file).  Optionally, save the file to the directory specified by `save_dir`
@@ -427,71 +427,63 @@
         """
         if x is None:
             return None
         return utils.dict_or_str_to_json_file(x, dir=save_dir).name
 
 
 class GallerySerializable(Serializable):
-    def api_info(self) -> Dict[str, List[str]]:
+    def serialized_info(self):
+        return {
+            "type": "string",
+            "description": "path to directory with images and a file associating images with captions called captions.json",
+        }
+
+    def api_info(self) -> dict[str, dict | bool]:
         return {
-            "raw_input": [
-                "List[List[str | None]]",
-                "List of lists. The inner lists should contain two elements: a base64 file representation and an optional caption, the outer list should contain one such list for each image in the gallery.",
-            ],
-            "raw_output": [
-                "List[List[str | None]]",
-                "List of lists. The inner lists should contain two elements: a base64 file representation and an optional caption, the outer list should contain one such list for each image in the gallery.",
-            ],
-            "serialized_input": [
-                "str",
-                "path to directory with images and a file associating images with captions called captions.json",
-            ],
-            "serialized_output": [
-                "str",
-                "path to directory with images and a file associating images with captions called captions.json",
-            ],
+            "info": serializer_types["GallerySerializable"],
+            "serialized_info": True,
         }
 
-    def example_inputs(self) -> Dict[str, Any]:
+    def example_inputs(self) -> dict[str, Any]:
         return {
             "raw": [media_data.BASE64_IMAGE] * 2,
             "serialized": [
                 "https://raw.githubusercontent.com/gradio-app/gradio/main/test/test_files/bus.png",
             ]
             * 2,
         }
 
     def serialize(
         self, x: str | None, load_dir: str | Path = ""
-    ) -> List[List[str | None]] | None:
+    ) -> list[list[str | None]] | None:
         if x is None or x == "":
             return None
         files = []
         captions_file = Path(x) / "captions.json"
         with captions_file.open("r") as captions_json:
             captions = json.load(captions_json)
         for file_name, caption in captions.items():
             img = FileSerializable().serialize(file_name)
             files.append([img, caption])
         return files
 
     def deserialize(
         self,
-        x: List[List[str | None]] | None,
+        x: list[list[str | None]] | None,
         save_dir: str = "",
         root_url: str | None = None,
         hf_token: str | None = None,
     ) -> None | str:
         if x is None:
             return None
         gallery_path = Path(save_dir) / str(uuid.uuid4())
         gallery_path.mkdir(exist_ok=True, parents=True)
         captions = {}
         for img_data in x:
-            if isinstance(img_data, list) or isinstance(img_data, tuple):
+            if isinstance(img_data, (list, tuple)):
                 img_data, caption = img_data
             else:
                 caption = None
             name = FileSerializable().deserialize(
                 img_data, gallery_path, root_url=root_url, hf_token=hf_token
             )
             captions[name] = caption
@@ -507,15 +499,15 @@
     for subcls in cls.__subclasses__():
         SERIALIZER_MAPPING[subcls.__name__] = subcls
 
 SERIALIZER_MAPPING["Serializable"] = SimpleSerializable
 SERIALIZER_MAPPING["File"] = FileSerializable
 SERIALIZER_MAPPING["UploadButton"] = FileSerializable
 
-COMPONENT_MAPPING: Dict[str, type] = {
+COMPONENT_MAPPING: dict[str, type] = {
     "textbox": StringSerializable,
     "number": NumberSerializable,
     "slider": NumberSerializable,
     "checkbox": BooleanSerializable,
     "checkboxgroup": ListStringSerializable,
     "radio": StringSerializable,
     "dropdown": SimpleSerializable,
```

### Comparing `gradio_client-0.1.4/gradio_client/utils.py` & `gradio_client-0.2.0/gradio_client/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,30 +10,30 @@
 import tempfile
 from concurrent.futures import CancelledError
 from dataclasses import dataclass, field
 from datetime import datetime
 from enum import Enum
 from pathlib import Path
 from threading import Lock
-from typing import Any, Callable, Dict, List, Optional, Tuple
+from typing import Any, Callable, Optional
 
 import fsspec.asyn
 import httpx
 import huggingface_hub
 import requests
 from huggingface_hub import SpaceStage
 from websockets.legacy.protocol import WebSocketCommonProtocol
 
 API_URL = "/api/predict/"
 WS_URL = "/queue/join"
 UPLOAD_URL = "/upload"
 CONFIG_URL = "/config"
 API_INFO_URL = "/info"
 RAW_API_INFO_URL = "/info?serialize=False"
-SPACE_FETCHER_URL = "https://gradio-space-api-fetcher.hf.space/api"
+SPACE_FETCHER_URL = "https://gradio-space-api-fetcher-v2.hf.space/api"
 RESET_URL = "/reset"
 SPACE_URL = "https://hf.space/{}"
 
 STATE_COMPONENT = "state"
 INVALID_RUNTIME = [
     SpaceStage.NO_APP_FILE,
     SpaceStage.CONFIG_ERROR,
@@ -80,15 +80,15 @@
     PROCESSING = "PROCESSING"
     ITERATING = "ITERATING"
     PROGRESS = "PROGRESS"
     FINISHED = "FINISHED"
     CANCELLED = "CANCELLED"
 
     @staticmethod
-    def ordering(status: "Status") -> int:
+    def ordering(status: Status) -> int:
         """Order of messages. Helpful for testing."""
         order = [
             Status.STARTING,
             Status.JOINING_QUEUE,
             Status.QUEUE_FULL,
             Status.IN_QUEUE,
             Status.SENDING_DATA,
@@ -96,19 +96,19 @@
             Status.PROGRESS,
             Status.ITERATING,
             Status.FINISHED,
             Status.CANCELLED,
         ]
         return order.index(status)
 
-    def __lt__(self, other: "Status"):
+    def __lt__(self, other: Status):
         return self.ordering(self) < self.ordering(other)
 
     @staticmethod
-    def msg_to_status(msg: str) -> "Status":
+    def msg_to_status(msg: str) -> Status:
         """Map the raw message from the backend to the status code presented to users."""
         return {
             "send_hash": Status.JOINING_QUEUE,
             "queue_full": Status.QUEUE_FULL,
             "estimation": Status.IN_QUEUE,
             "send_data": Status.SENDING_DATA,
             "process_starts": Status.PROCESSING,
@@ -123,15 +123,15 @@
     index: Optional[int]
     length: Optional[int]
     unit: Optional[str]
     progress: Optional[float]
     desc: Optional[str]
 
     @classmethod
-    def from_ws_msg(cls, data: List[Dict]) -> List["ProgressUnit"]:
+    def from_ws_msg(cls, data: list[dict]) -> list[ProgressUnit]:
         return [
             cls(
                 index=d.get("index"),
                 length=d.get("length"),
                 unit=d.get("unit"),
                 progress=d.get("progress"),
                 desc=d.get("desc"),
@@ -146,15 +146,15 @@
 
     code: Status
     rank: int | None
     queue_size: int | None
     eta: float | None
     success: bool | None
     time: datetime | None
-    progress_data: List[ProgressUnit] | None
+    progress_data: list[ProgressUnit] | None
 
 
 def create_initial_status_update():
     return StatusUpdate(
         code=Status.STARTING,
         rank=None,
         queue_size=None,
@@ -169,24 +169,24 @@
 class JobStatus:
     """The job status.
 
     Keeps strack of the latest status update and intermediate outputs (not yet implements).
     """
 
     latest_status: StatusUpdate = field(default_factory=create_initial_status_update)
-    outputs: List[Any] = field(default_factory=list)
+    outputs: list[Any] = field(default_factory=list)
 
 
 @dataclass
 class Communicator:
     """Helper class to help communicate between the worker thread and main thread."""
 
     lock: Lock
     job: JobStatus
-    deserialize: Callable[..., Tuple]
+    deserialize: Callable[..., tuple]
     reset_url: str
     should_cancel: bool = False
 
 
 ########################
 # Network utils
 ########################
@@ -204,15 +204,15 @@
 
 
 async def get_pred_from_ws(
     websocket: WebSocketCommonProtocol,
     data: str,
     hash_data: str,
     helper: Communicator | None = None,
-) -> Dict[str, Any]:
+) -> dict[str, Any]:
     completed = False
     resp = {}
     while not completed:
         # Receive message in the background so that we can
         # cancel even while running a long pred
         task = asyncio.create_task(websocket.recv())
         while not task.done():
@@ -281,17 +281,18 @@
     suffix = Path(url_path).suffix
     file_obj = tempfile.NamedTemporaryFile(
         delete=False,
         prefix=prefix,
         suffix=suffix,
         dir=dir,
     )
-    with requests.get(url_path, headers=headers, stream=True) as r:
-        with open(file_obj.name, "wb") as f:
-            shutil.copyfileobj(r.raw, f)
+    with requests.get(url_path, headers=headers, stream=True) as r, open(
+        file_obj.name, "wb"
+    ) as f:
+        shutil.copyfileobj(r.raw, f)
     return file_obj
 
 
 def create_tmp_copy_of_file(
     file_path: str, dir: str | None = None
 ) -> tempfile._TemporaryFileWrapper:
     if dir is not None:
@@ -356,20 +357,17 @@
     path = str(path)
     if is_valid_url(path):
         return encode_url_to_base64(path)
     else:
         return encode_file_to_base64(path)
 
 
-def decode_base64_to_binary(encoding: str) -> Tuple[bytes, str | None]:
+def decode_base64_to_binary(encoding: str) -> tuple[bytes, str | None]:
     extension = get_extension(encoding)
-    try:
-        data = encoding.split(",")[1]
-    except IndexError:
-        data = ""
+    data = encoding.rsplit(",", 1)[-1]
     return base64.b64decode(data), extension
 
 
 def strip_invalid_filename_characters(filename: str, max_bytes: int = 200) -> str:
     """Strips invalid characters from a filename and ensures that the file_length is less than `max_bytes` bytes."""
     filename = "".join([char for char in filename if char.isalnum() or char in "._- "])
     filename_len = len(filename.encode())
@@ -420,29 +418,29 @@
             dir=dir,
         )
     file_obj.write(data)
     file_obj.flush()
     return file_obj
 
 
-def dict_or_str_to_json_file(jsn: str | Dict | List, dir: str | Path | None = None):
+def dict_or_str_to_json_file(jsn: str | dict | list, dir: str | Path | None = None):
     if dir is not None:
         os.makedirs(dir, exist_ok=True)
 
     file_obj = tempfile.NamedTemporaryFile(
         delete=False, suffix=".json", dir=dir, mode="w+"
     )
     if isinstance(jsn, str):
         jsn = json.loads(jsn)
     json.dump(jsn, file_obj)
     file_obj.flush()
     return file_obj
 
 
-def file_to_json(file_path: str | Path) -> Dict | List:
+def file_to_json(file_path: str | Path) -> dict | list:
     with open(file_path) as f:
         return json.load(f)
 
 
 ###########################
 # HuggingFace Hub API Utils
 ###########################
@@ -459,19 +457,19 @@
     r = requests.post(
         f"https://huggingface.co/api/spaces/{space_id}/sleeptime",
         json={"seconds": timeout_in_seconds},
         headers=headers,
     )
     try:
         huggingface_hub.utils.hf_raise_for_status(r)
-    except huggingface_hub.utils.HfHubHTTPError:
+    except huggingface_hub.utils.HfHubHTTPError as err:
         raise SpaceDuplicationError(
             f"Could not set sleep timeout on duplicated Space. Please visit {SPACE_URL.format(space_id)} "
             "to set a timeout manually to reduce billing charges."
-        )
+        ) from err
 
 
 ########################
 # Misc utils
 ########################
 
 
@@ -485,7 +483,65 @@
 
     Args:
         func:
         *args:
         **kwargs:
     """
     return fsspec.asyn.sync(fsspec.asyn.get_loop(), func, *args, **kwargs)  # type: ignore
+
+
+class APIInfoParseError(ValueError):
+    pass
+
+
+def get_type(schema: dict):
+    if "type" in schema:
+        return schema["type"]
+    elif schema.get("oneOf"):
+        return "oneOf"
+    elif schema.get("anyOf"):
+        return "anyOf"
+    else:
+        raise APIInfoParseError(f"Cannot parse type for {schema}")
+
+
+def json_schema_to_python_type(schema: Any) -> str:
+    """Convert the json schema into a python type hint"""
+    type_ = get_type(schema)
+    if type_ == {}:
+        if "json" in schema["description"]:
+            return "Dict[Any, Any]"
+        else:
+            return "Any"
+    elif type_ == "null":
+        return "None"
+    elif type_ == "integer":
+        return "int"
+    elif type_ == "string":
+        return "str"
+    elif type_ == "boolean":
+        return "bool"
+    elif type_ == "number":
+        return "int | float"
+    elif type_ == "array":
+        items = schema.get("items")
+        if "prefixItems" in items:
+            elements = ", ".join(
+                [json_schema_to_python_type(i) for i in items["prefixItems"]]
+            )
+            return f"Tuple[{elements}]"
+        else:
+            elements = json_schema_to_python_type(items)
+            return f"List[{elements}]"
+    elif type_ == "object":
+        des = ", ".join(
+            [
+                f"{n}: {json_schema_to_python_type(v)} ({v.get('description')})"
+                for n, v in schema["properties"].items()
+            ]
+        )
+        return f"Dict({des})"
+    elif type_ in ["oneOf", "anyOf"]:
+        desc = " | ".join([json_schema_to_python_type(i) for i in schema[type_]])
+        return desc
+    else:
+        raise APIInfoParseError(f"Cannot parse schema {schema}")
```

### Comparing `gradio_client-0.1.4/.gitignore` & `gradio_client-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `gradio_client-0.1.4/pyproject.toml` & `gradio_client-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gradio_client-0.1.4/PKG-INFO` & `gradio_client-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gradio_client
-Version: 0.1.4
+Version: 0.2.0
 Summary: Python library for easily interacting with trained machine learning models
 Project-URL: Homepage, https://github.com/gradio-app/gradio
 Author-email: Abubakar Abid <team@gradio.app>, Ali Abid <team@gradio.app>, Ali Abdalla <team@gradio.app>, Dawood Khan <team@gradio.app>, Ahsen Khaliq <team@gradio.app>, Pete Allen <team@gradio.app>, Freddy Boulton <team@gradio.app>
 License-Expression: Apache-2.0
 Keywords: API,client,machine learning
 Requires-Python: >=3.7
 Requires-Dist: fsspec
```

