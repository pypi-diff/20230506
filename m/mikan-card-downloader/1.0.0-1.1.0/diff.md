# Comparing `tmp/mikan_card_downloader-1.0.0.tar.gz` & `tmp/mikan_card_downloader-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mikan_card_downloader-1.0.0.tar", max compression
+gzip compressed data, was "mikan_card_downloader-1.1.0.tar", max compression
```

## Comparing `mikan_card_downloader-1.0.0.tar` & `mikan_card_downloader-1.1.0.tar`

### file list

```diff
@@ -1,12 +1,11 @@
--rw-r--r--   0        0        0    35149 2021-11-29 13:57:47.295968 mikan_card_downloader-1.0.0/LICENSE
--rw-r--r--   0        0        0     1041 2023-04-26 22:38:39.384353 mikan_card_downloader-1.0.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-20 20:32:09.133338 mikan_card_downloader-1.0.0/src/mikan/__init__.py
--rw-r--r--   0        0        0     1317 2023-04-26 16:41:23.873925 mikan_card_downloader-1.0.0/src/mikan/classes.py
--rw-r--r--   0        0        0     1306 2023-04-21 03:31:38.850291 mikan_card_downloader-1.0.0/src/mikan/config.py
--rw-r--r--   0        0        0     3209 2023-04-26 16:41:23.873925 mikan_card_downloader-1.0.0/src/mikan/downloader.py
--rw-r--r--   0        0        0     5958 2023-04-26 22:37:48.260144 mikan_card_downloader-1.0.0/src/mikan/html_parser.py
--rw-r--r--   0        0        0     1382 2023-04-23 20:48:44.204752 mikan_card_downloader-1.0.0/src/mikan/json_utils.py
--rwxr-xr-x   0        0        0     2217 2023-04-26 22:37:48.260144 mikan_card_downloader-1.0.0/src/mikan/main.py
--rw-r--r--   0        0        0        0 2023-04-20 20:32:09.133338 mikan_card_downloader-1.0.0/src/mikan/py.typed
--rw-r--r--   0        0        0      911 1970-01-01 00:00:00.000000 mikan_card_downloader-1.0.0/setup.py
--rw-r--r--   0        0        0      594 1970-01-01 00:00:00.000000 mikan_card_downloader-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2021-11-29 13:57:47.295968 mikan_card_downloader-1.1.0/LICENSE
+-rw-r--r--   0        0        0     1041 2023-05-06 20:00:28.315898 mikan_card_downloader-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-20 20:32:09.133338 mikan_card_downloader-1.1.0/src/mikan/__init__.py
+-rw-r--r--   0        0        0     1536 2023-05-05 22:20:27.438705 mikan_card_downloader-1.1.0/src/mikan/classes.py
+-rw-r--r--   0        0        0     1491 2023-05-05 22:20:27.438705 mikan_card_downloader-1.1.0/src/mikan/config.py
+-rw-r--r--   0        0        0     3294 2023-05-05 22:20:27.438705 mikan_card_downloader-1.1.0/src/mikan/downloader.py
+-rw-r--r--   0        0        0     5958 2023-05-05 21:55:44.145052 mikan_card_downloader-1.1.0/src/mikan/html_parser.py
+-rw-r--r--   0        0        0     1382 2023-04-23 20:48:44.204752 mikan_card_downloader-1.1.0/src/mikan/json_utils.py
+-rwxr-xr-x   0        0        0     2383 2023-05-05 22:20:27.438705 mikan_card_downloader-1.1.0/src/mikan/main.py
+-rw-r--r--   0        0        0        0 2023-04-20 20:32:09.133338 mikan_card_downloader-1.1.0/src/mikan/py.typed
+-rw-r--r--   0        0        0      594 1970-01-01 00:00:00.000000 mikan_card_downloader-1.1.0/PKG-INFO
```

### Comparing `mikan_card_downloader-1.0.0/LICENSE` & `mikan_card_downloader-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mikan_card_downloader-1.0.0/pyproject.toml` & `mikan_card_downloader-1.1.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mikan-card-downloader"
-version = "1.0.0"
+version = "1.1.0"
 description = "Downloads cards and stills from SIFAS and SIF."
 authors = ["DemonicSavage"]
 license = "GPLv3"
 packages = [
     {include = "mikan", from = "src"}
 ]
```

### Comparing `mikan_card_downloader-1.0.0/src/mikan/classes.py` & `mikan_card_downloader-1.1.0/src/mikan/classes.py`

 * *Files 17% similar despite different names*

```diff
@@ -33,8 +33,15 @@
 @dataclass
 class SIFCard:
     results_dir: ClassVar = "SIF_Cards"
     list_url_template: ClassVar = "https://schoolido.lu/api/cardids/"
     url_template: ClassVar = "https://schoolido.lu/api/cards/"
 
 
-Item: TypeAlias = Card | Still | SIFCard
+@dataclass
+class SIF2Card:
+    results_dir: ClassVar = "SIF2_Cards"
+    list_url_template: ClassVar = "https://idol.st/ajax/SIF2/cards/?page="
+    url_template: ClassVar = "https://idol.st/ajax/SIF2/card/"
+
+
+Item: TypeAlias = Card | Still | SIFCard | SIF2Card
```

### Comparing `mikan_card_downloader-1.0.0/src/mikan/config.py` & `mikan_card_downloader-1.1.0/src/mikan/config.py`

 * *Files 11% similar despite different names*

```diff
@@ -34,7 +34,16 @@
 
         cfg["Paths"]["data_dir"] = str(Path(selected_dir).expanduser().resolve())
         with open(cfg_file, "w") as file:
             cfg.write(file)
 
     cfg.read(cfg_file)
     return Path(cfg["Paths"]["data_dir"])
+
+
+def get_cookie(path: Path) -> str:
+    cfg_file = path / "config.cfg"
+    try:
+        cfg.read(cfg_file)
+        return cfg["Other"]["cookie"]
+    except KeyError:
+        return ""
```

### Comparing `mikan_card_downloader-1.0.0/src/mikan/downloader.py` & `mikan_card_downloader-1.1.0/src/mikan/downloader.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,25 +22,29 @@
 
 import mikan.html_parser as parser
 from mikan import json_utils
 from mikan.classes import Item
 
 
 class Downloader:
-    def __init__(self, data_path: Path, config_path: Path, img_type: type[Item]):
+    def __init__(
+        self, data_path: Path, config_path: Path, img_type: type[Item], cookie: str = ""
+    ):
         self.base_path = data_path.expanduser()
         self.path = self.base_path / img_type.results_dir
         self.objs: dict[str, dict[str, list[str]]] = {}
 
         self.config_path = config_path
 
         self.img_type = img_type
         self.objs[self.img_type.results_dir] = {}
 
-        self.session = aiohttp.ClientSession(timeout=aiohttp.ClientTimeout(total=None))
+        self.session = aiohttp.ClientSession(
+            timeout=aiohttp.ClientTimeout(total=None), cookies={"sessionid": cookie}
+        )
 
         json_utils.load_cards(self.objs, self.config_path)
 
         self.parser = parser.Parser(self.objs, self.img_type, self.session)
 
     async def __aenter__(self) -> Downloader:
         return self
```

### Comparing `mikan_card_downloader-1.0.0/src/mikan/html_parser.py` & `mikan_card_downloader-1.1.0/src/mikan/html_parser.py`

 * *Files identical despite different names*

### Comparing `mikan_card_downloader-1.0.0/src/mikan/json_utils.py` & `mikan_card_downloader-1.1.0/src/mikan/json_utils.py`

 * *Files identical despite different names*

### Comparing `mikan_card_downloader-1.0.0/src/mikan/main.py` & `mikan_card_downloader-1.1.0/src/mikan/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,52 +18,56 @@
 import sys
 from pathlib import Path
 from typing import Type
 
 import platformdirs
 
 from mikan import config
-from mikan.classes import Card, Item, SIFCard, Still
+from mikan.classes import Card, Item, SIF2Card, SIFCard, Still
 from mikan.downloader import Downloader
 
 
 class UnrecognizedArgumentException(Exception):
     pass
 
 
 class InvalidPathException(Exception):
     pass
 
 
 async def run(
     path: Path = Path(platformdirs.user_config_dir("mikan", ensure_exists=True))
 ) -> None:
-    img_type: Type[Card | Still | SIFCard] = Card
+    img_type: Type[Card | Still | SIFCard | SIF2Card] = Card
     if len(sys.argv) > 1:
         if sys.argv[1] == "--stills":
             img_type = Still
         elif sys.argv[1] == "--sif":
             img_type = SIFCard
+        elif sys.argv[1] == "--sif2":
+            img_type = SIF2Card
         else:
             raise UnrecognizedArgumentException(
-                "Only recognized arguments are --stills and --sif."
+                "Only recognized arguments are --stills, --sif and --sif2."
             )
 
     data_dir = config.get_data_dir(path)
     if data_dir.exists() and not data_dir.is_dir():  # pragma: no cover
         raise InvalidPathException(
             "The specified directory is not valid (is a regular file)."
         )
-    await card_searcher(data_dir, path, img_type)
+
+    cookie = config.get_cookie(path)
+    await card_searcher(data_dir, path, img_type, cookie)
 
 
 async def card_searcher(
-    data_path: Path, config_path: Path, img_type: type[Item]
+    data_path: Path, config_path: Path, img_type: type[Item], cookie: str
 ) -> None:
-    async with Downloader(data_path, config_path, img_type) as downloader:
+    async with Downloader(data_path, config_path, img_type, cookie) as downloader:
         await downloader.update()
         await downloader.get()
 
 
 def main() -> None:  # pragma: no cover
     if sys.platform.startswith("win"):
         asyncio.set_event_loop_policy(asyncio.WindowsSelectorEventLoopPolicy())
```

### Comparing `mikan_card_downloader-1.0.0/PKG-INFO` & `mikan_card_downloader-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mikan-card-downloader
-Version: 1.0.0
+Version: 1.1.0
 Summary: Downloads cards and stills from SIFAS and SIF.
 License: GPLv3
 Author: DemonicSavage
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

