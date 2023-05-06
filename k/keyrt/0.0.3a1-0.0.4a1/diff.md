# Comparing `tmp/keyrt-0.0.3a1.tar.gz` & `tmp/keyrt-0.0.4a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keyrt-0.0.3a1.tar", last modified: Thu Mar 16 11:42:40 2023, max compression
+gzip compressed data, was "keyrt-0.0.4a1.tar", last modified: Sat May  6 13:12:05 2023, max compression
```

## Comparing `keyrt-0.0.3a1.tar` & `keyrt-0.0.4a1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 white     (1000) wjite     (1001)        0 2023-03-16 11:42:40.407277 keyrt-0.0.3a1/
--rw-r--r--   0 white     (1000) wjite     (1001)      953 2023-03-16 11:42:40.407277 keyrt-0.0.3a1/PKG-INFO
--rw-r--r--   0 white     (1000) wjite     (1001)      715 2022-07-12 18:26:09.000000 keyrt-0.0.3a1/README.md
-drwxr-xr-x   0 white     (1000) wjite     (1001)        0 2023-03-16 11:42:40.400610 keyrt-0.0.3a1/keyrt/
--rw-r--r--   0 white     (1000) wjite     (1001)       51 2022-07-07 07:11:24.000000 keyrt-0.0.3a1/keyrt/__init__.py
--rw-r--r--   0 white     (1000) wjite     (1001)     5879 2023-03-16 11:42:32.000000 keyrt-0.0.3a1/keyrt/aioclient.py
-drwxr-xr-x   0 white     (1000) wjite     (1001)        0 2023-03-16 11:42:40.400610 keyrt-0.0.3a1/keyrt/models/
--rw-r--r--   0 white     (1000) wjite     (1001)      231 2023-02-10 22:48:17.000000 keyrt-0.0.3a1/keyrt/models/__init__.py
--rw-r--r--   0 white     (1000) wjite     (1001)     1411 2023-02-10 22:49:09.000000 keyrt-0.0.3a1/keyrt/models/cameras.py
--rw-r--r--   0 white     (1000) wjite     (1001)     2083 2023-02-10 22:49:09.000000 keyrt-0.0.3a1/keyrt/models/codes.py
--rw-r--r--   0 white     (1000) wjite     (1001)     1534 2023-03-15 12:24:54.000000 keyrt-0.0.3a1/keyrt/models/devices.py
--rw-r--r--   0 white     (1000) wjite     (1001)      387 2023-02-10 22:48:17.000000 keyrt-0.0.3a1/keyrt/models/tokens.py
--rw-r--r--   0 white     (1000) wjite     (1001)     3548 2023-02-10 22:48:17.000000 keyrt-0.0.3a1/keyrt/models/user.py
-drwxr-xr-x   0 white     (1000) wjite     (1001)        0 2023-03-16 11:42:40.400610 keyrt-0.0.3a1/keyrt.egg-info/
--rw-r--r--   0 white     (1000) wjite     (1001)      953 2023-03-16 11:42:40.000000 keyrt-0.0.3a1/keyrt.egg-info/PKG-INFO
--rw-r--r--   0 white     (1000) wjite     (1001)      399 2023-03-16 11:42:40.000000 keyrt-0.0.3a1/keyrt.egg-info/SOURCES.txt
--rw-r--r--   0 white     (1000) wjite     (1001)        1 2023-03-16 11:42:40.000000 keyrt-0.0.3a1/keyrt.egg-info/dependency_links.txt
--rw-r--r--   0 white     (1000) wjite     (1001)       30 2023-03-16 11:42:40.000000 keyrt-0.0.3a1/keyrt.egg-info/requires.txt
--rw-r--r--   0 white     (1000) wjite     (1001)        6 2023-03-16 11:42:40.000000 keyrt-0.0.3a1/keyrt.egg-info/top_level.txt
--rw-r--r--   0 white     (1000) wjite     (1001)       38 2023-03-16 11:42:40.407277 keyrt-0.0.3a1/setup.cfg
--rw-r--r--   0 white     (1000) wjite     (1001)      668 2023-03-16 11:42:32.000000 keyrt-0.0.3a1/setup.py
-drwxr-xr-x   0 white     (1000) wjite     (1001)        0 2023-03-16 11:42:40.400610 keyrt-0.0.3a1/tests/
--rw-r--r--   0 white     (1000) wjite     (1001)     2149 2023-02-10 22:48:17.000000 keyrt-0.0.3a1/tests/test_codes.py
--rw-r--r--   0 white     (1000) wjite     (1001)      899 2022-07-12 18:28:47.000000 keyrt-0.0.3a1/tests/test_devices.py
--rw-r--r--   0 white     (1000) wjite     (1001)      469 2022-07-12 18:19:18.000000 keyrt-0.0.3a1/tests/test_user.py
+drwxr-xr-x   0 white     (1000) wjite     (1001)        0 2023-05-06 13:12:05.305427 keyrt-0.0.4a1/
+-rw-r--r--   0 white     (1000) wjite     (1001)     1244 2023-05-06 13:12:05.305427 keyrt-0.0.4a1/PKG-INFO
+-rw-r--r--   0 white     (1000) wjite     (1001)     1006 2023-03-17 07:01:38.000000 keyrt-0.0.4a1/README.md
+drwxr-xr-x   0 white     (1000) wjite     (1001)        0 2023-05-06 13:12:05.302094 keyrt-0.0.4a1/keyrt/
+-rw-r--r--   0 white     (1000) wjite     (1001)       51 2022-07-07 07:11:24.000000 keyrt-0.0.4a1/keyrt/__init__.py
+-rw-r--r--   0 white     (1000) wjite     (1001)     6019 2023-04-24 11:07:19.000000 keyrt-0.0.4a1/keyrt/aioclient.py
+drwxr-xr-x   0 white     (1000) wjite     (1001)        0 2023-05-06 13:12:05.302094 keyrt-0.0.4a1/keyrt/models/
+-rw-r--r--   0 white     (1000) wjite     (1001)      231 2023-03-17 06:52:24.000000 keyrt-0.0.4a1/keyrt/models/__init__.py
+-rw-r--r--   0 white     (1000) wjite     (1001)     1418 2023-03-17 07:07:25.000000 keyrt-0.0.4a1/keyrt/models/cameras.py
+-rw-r--r--   0 white     (1000) wjite     (1001)     2093 2023-05-06 13:06:40.000000 keyrt-0.0.4a1/keyrt/models/codes.py
+-rw-r--r--   0 white     (1000) wjite     (1001)     1605 2023-03-17 07:07:25.000000 keyrt-0.0.4a1/keyrt/models/devices.py
+-rw-r--r--   0 white     (1000) wjite     (1001)      387 2023-02-10 22:48:17.000000 keyrt-0.0.4a1/keyrt/models/tokens.py
+-rw-r--r--   0 white     (1000) wjite     (1001)     3548 2023-03-17 06:52:24.000000 keyrt-0.0.4a1/keyrt/models/user.py
+drwxr-xr-x   0 white     (1000) wjite     (1001)        0 2023-05-06 13:12:05.302094 keyrt-0.0.4a1/keyrt.egg-info/
+-rw-r--r--   0 white     (1000) wjite     (1001)     1244 2023-05-06 13:12:05.000000 keyrt-0.0.4a1/keyrt.egg-info/PKG-INFO
+-rw-r--r--   0 white     (1000) wjite     (1001)      399 2023-05-06 13:12:05.000000 keyrt-0.0.4a1/keyrt.egg-info/SOURCES.txt
+-rw-r--r--   0 white     (1000) wjite     (1001)        1 2023-05-06 13:12:05.000000 keyrt-0.0.4a1/keyrt.egg-info/dependency_links.txt
+-rw-r--r--   0 white     (1000) wjite     (1001)       31 2023-05-06 13:12:05.000000 keyrt-0.0.4a1/keyrt.egg-info/requires.txt
+-rw-r--r--   0 white     (1000) wjite     (1001)        6 2023-05-06 13:12:05.000000 keyrt-0.0.4a1/keyrt.egg-info/top_level.txt
+-rw-r--r--   0 white     (1000) wjite     (1001)       38 2023-05-06 13:12:05.305427 keyrt-0.0.4a1/setup.cfg
+-rw-r--r--   0 white     (1000) wjite     (1001)      668 2023-05-06 03:01:00.000000 keyrt-0.0.4a1/setup.py
+drwxr-xr-x   0 white     (1000) wjite     (1001)        0 2023-05-06 13:12:05.302094 keyrt-0.0.4a1/tests/
+-rw-r--r--   0 white     (1000) wjite     (1001)     2149 2023-03-17 06:52:26.000000 keyrt-0.0.4a1/tests/test_codes.py
+-rw-r--r--   0 white     (1000) wjite     (1001)      899 2022-07-12 18:28:47.000000 keyrt-0.0.4a1/tests/test_devices.py
+-rw-r--r--   0 white     (1000) wjite     (1001)      469 2022-07-12 18:19:18.000000 keyrt-0.0.4a1/tests/test_user.py
```

### Comparing `keyrt-0.0.3a1/PKG-INFO` & `keyrt-0.0.4a1/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: keyrt
-Version: 0.0.3a1
-Summary: KeyRT
-Home-page: https://github.com/WhiteApfel/keyrt
-Author: WhiteApfel
-Author-email: white@pfel.ru
-License: Mozilla Public License 2.0
-Description-Content-Type: text/markdown
-
 # KeyRT
 
 Не знаю, зачем тебе может понадобиться автоматизация открытия дверей и выдачи кодов,
 но это твоё право, я даю тебе удобный инструмент для его реализации. Да здравствует питон.
 
 ## Установка
 
@@ -23,12 +13,24 @@
 
 ### Открытие двери
 
 ```python
 from keyrt import KeyRT
 
 async def main():
-    keyrt_client = KeyRT(access_token='YOUR_ACCESS_TOKEN'
-                         )
+    keyrt_client = KeyRT(access_token='YOUR_ACCESS_TOKEN')
+    
+    # Список устройств: домофон, шлагбаум, ворота
     devices = await keyrt_client.get_devices()
-    assert await keyrt_client.open_device(devices.devices[0].id)
-```
+    
+    for i, device in enumerate(devices):
+        example = devices[i]
+        assert example is device
+        
+        example = devices[device.]
+    
+    assert await keyrt_client.open_device(devices[0].id)
+    
+    # Камеры 
+    cameras = await keyrt_client.get_cameras()
+    
+```
```

### Comparing `keyrt-0.0.3a1/keyrt/aioclient.py` & `keyrt-0.0.4a1/keyrt/aioclient.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import time
-from base64 import b64encode, b64decode
+from base64 import b64decode, b64encode
 from io import BytesIO
 from typing import Literal
 
 from httpx import AsyncClient
 
-from keyrt.models.cameras import Cameras, CamerasResponse, Camera
+from keyrt.models.cameras import Camera, Cameras, CamerasResponse
 from keyrt.models.codes import Codes, CodesResponse
-from keyrt.models.devices import DevicesResponse, Devices
+from keyrt.models.devices import Devices, DevicesResponse
 from keyrt.models.tokens import OauthTokensResponse
 from keyrt.models.user import User, UserResponse
 
 
 class KeyRT:
     def __init__(self, access_token: str = None):
         self._access_token: str = access_token
@@ -29,15 +29,15 @@
         method: Literal["GET", "POST", "PUT", "DELETE"],
         url: str,
         params: dict | None = None,
         data: dict | None = None,
         json: dict | None = None,
         headers: dict | None = None,
         access_token: str | None = None,
-        cookies: dict | None = None
+        cookies: dict | None = None,
     ):
         if access_token is not None:
             headers = (headers or {}) | {"Authorization": f"Bearer {access_token}"}
         return await self.session.request(
             method=method,
             url=url,
             headers=headers,
@@ -68,42 +68,44 @@
     async def get_cameras(self, access_token: str = None) -> Cameras:
         response = await self.request(
             method="GET",
             url="https://vc.key.rt.ru/api/v1/cameras",
             params={
                 "offset": 0,
                 "limit": 1000,
+                "category_types": ",".join(["intercom", "barrier", "outdoor_camera"])
             },
             access_token=access_token,
         )
 
         return CamerasResponse(**response.json()).data
 
-    async def get_camera_shot(self, camera: Camera, timestamp: int, access_token: str = None) -> BytesIO:
+    async def get_camera_shot(
+        self, camera: Camera, timestamp: str, access_token: str = None
+    ) -> BytesIO:
         shot_url = camera.screenshot_url_template
         shot_url = (
             shot_url.replace("{size}", "original")
             .replace("{timestamp}", timestamp or str(int(time.time())))
             .replace("{cdn_token}", camera.screenshot_token)
         )
 
         response = await self.request(
             method="GET",
             url=shot_url,
-            cookies={
-                "utoken": camera.user_token
-            },
+            cookies={"utoken": camera.user_token},
             access_token=access_token,
         )
 
         if response.is_success:
             buffer = BytesIO()
             buffer.write(response.content)
             buffer.seek(0)
             return buffer
+        raise ValueError(f"{response.status_code} {response.text=}")
 
     async def open_device(self, device_id: str, access_token: str = None) -> bool:
         response = await self.request(
             method="POST",
             url=f"/v2/app/devices/{device_id}/open",
             access_token=access_token,
         )
```

### Comparing `keyrt-0.0.3a1/keyrt/models/cameras.py` & `keyrt-0.0.4a1/keyrt/models/cameras.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from datetime import datetime
-from typing import Any, List, Optional, Iterator
+from typing import Any, Iterator, List
 
 from pydantic import BaseModel, Field
 
 
 class Category(BaseModel):
     id: int
     title: str
@@ -44,15 +44,15 @@
     vendor: str
 
 
 class Cameras(BaseModel):
     cameras: List[Camera] = Field(..., alias="items")
     total: int
 
-    def __getitem__(self, item):
+    def __getitem__(self, item) -> Camera:
         # by camera id
         for camera in self.cameras:
             if camera.id == str(item):
                 return camera
 
         # by title
         for camera in self.cameras:
@@ -60,15 +60,15 @@
                 return camera
 
         return self.cameras[item]
 
     def __iter__(self) -> Iterator[Camera]:
         return iter(self.cameras)
 
-    def __len__(self):
+    def __len__(self) -> int:
         return len(self.cameras)
 
 
 class CamerasResponse(BaseModel):
     data: Cameras
     error: Any
     request_id: str
```

### Comparing `keyrt-0.0.3a1/keyrt/models/codes.py` & `keyrt-0.0.4a1/keyrt/models/codes.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 class FlatItem(BaseModel):
     id: int
     number: str
 
 
 class UserInfo(BaseModel):
     id: int
-    email: str
+    email: Optional[str]
     login: str
     phone_number: str
     status: str
 
 
 class Company(BaseModel):
     id: int
```

### Comparing `keyrt-0.0.3a1/keyrt/models/devices.py` & `keyrt-0.0.4a1/keyrt/models/devices.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from datetime import datetime
-from typing import Any, List, Optional
+from typing import Iterator
 
 from pydantic import BaseModel
 
 
 class Capability(BaseModel):
     name: str
     setup: bool
@@ -17,32 +17,32 @@
     inter_code_type: str
 
 
 class Device(BaseModel):
     id: str
     device_type: str
     serial_number: str
-    device_group: List[str]
+    device_group: list[str]
     entrance: int
     utc_offset_minutes: int
     camera_id: str
     description: str
     is_favorite: bool
     is_active: bool
     name_by_company: str
     name_by_user: str | None
     accept_concierge_call: bool
-    capabilities: List[Capability]
-    inter_codes: List[InterCode]
+    capabilities: list[Capability]
+    inter_codes: list[InterCode]
 
 
 class Devices(BaseModel):
-    devices: List[Device]
+    devices: list[Device]
 
-    def __getitem__(self, item):
+    def __getitem__(self, item) -> Device:
         # by device id
         for device in self.devices:
             if device.id == str(item):
                 return device
 
         # by serial_number
         for device in self.devices:
@@ -50,23 +50,23 @@
                 return device
 
         # by camera_id
         for device in self.devices:
             if device.camera_id == str(item):
                 return device
 
-        # by name_by_user
+        # by name_by_user or name_by_company
         for device in self.devices:
-            if device.name_by_user == str(item):
+            if str(item) in (device.name_by_company, device.name_by_user):
                 return device
 
         return self.devices[item]
 
-    def __iter__(self):
+    def __iter__(self) -> Iterator[Device]:
         return iter(self.devices)
 
-    def __len__(self):
+    def __len__(self) -> int:
         return len(self.devices)
 
 
 class DevicesResponse(BaseModel):
     data: Devices
```

### Comparing `keyrt-0.0.3a1/keyrt/models/user.py` & `keyrt-0.0.4a1/keyrt/models/user.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Any, List, Optional
 
-from pydantic import BaseModel, validator, root_validator
+from pydantic import BaseModel, root_validator, validator
 
 
 class Company(BaseModel):
     id: int
     vc_id: int
     title: str
     utc_offset: int
```

### Comparing `keyrt-0.0.3a1/setup.py` & `keyrt-0.0.4a1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 def requirements():
     with open("requirements.txt", "r") as req:
         return [r for r in req.read().split("\n") if r]
 
 
 setup(
     name="keyrt",
-    version="0.0.3a1",
+    version="0.0.4a1",
     packages=["keyrt", "keyrt.models"],
     url="https://github.com/WhiteApfel/keyrt",
     license="Mozilla Public License 2.0",
     author="WhiteApfel",
     author_email="white@pfel.ru",
     description="KeyRT",
     install_requires=requirements(),
```

### Comparing `keyrt-0.0.3a1/tests/test_codes.py` & `keyrt-0.0.4a1/tests/test_codes.py`

 * *Files identical despite different names*

### Comparing `keyrt-0.0.3a1/tests/test_devices.py` & `keyrt-0.0.4a1/tests/test_devices.py`

 * *Files identical despite different names*

