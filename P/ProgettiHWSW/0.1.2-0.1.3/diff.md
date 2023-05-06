# Comparing `tmp/ProgettiHWSW-0.1.2.tar.gz` & `tmp/ProgettiHWSW-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ProgettiHWSW-0.1.2.tar", last modified: Mon Jun 14 20:57:09 2021, max compression
+gzip compressed data, was "ProgettiHWSW-0.1.3.tar", last modified: Sat May  6 07:54:07 2023, max compression
```

## Comparing `ProgettiHWSW-0.1.2.tar` & `ProgettiHWSW-0.1.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 arda      (1000) arda      (1000)        0 2021-06-14 20:57:09.502829 ProgettiHWSW-0.1.2/
--rw-rw-r--   0 arda      (1000) arda      (1000)     1013 2021-06-14 20:57:09.498829 ProgettiHWSW-0.1.2/PKG-INFO
-drwxrwxr-x   0 arda      (1000) arda      (1000)        0 2021-06-14 20:57:09.498829 ProgettiHWSW-0.1.2/ProgettiHWSW/
--rw-r--r--   0 arda      (1000) arda      (1000)     4423 2021-06-14 20:44:09.000000 ProgettiHWSW-0.1.2/ProgettiHWSW/ProgettiHWSWAPI.py
--rw-r--r--   0 arda      (1000) arda      (1000)       60 2021-06-14 20:44:09.000000 ProgettiHWSW-0.1.2/ProgettiHWSW/__init__.py
--rw-r--r--   0 arda      (1000) arda      (1000)     1037 2021-06-14 20:44:09.000000 ProgettiHWSW-0.1.2/ProgettiHWSW/analog.py
--rw-r--r--   0 arda      (1000) arda      (1000)      803 2021-06-14 20:44:09.000000 ProgettiHWSW-0.1.2/ProgettiHWSW/api.py
--rw-r--r--   0 arda      (1000) arda      (1000)      173 2021-06-14 20:44:09.000000 ProgettiHWSW-0.1.2/ProgettiHWSW/const.py
--rw-r--r--   0 arda      (1000) arda      (1000)     1068 2021-06-14 20:44:09.000000 ProgettiHWSW-0.1.2/ProgettiHWSW/input.py
--rw-r--r--   0 arda      (1000) arda      (1000)     1679 2021-06-14 20:44:09.000000 ProgettiHWSW-0.1.2/ProgettiHWSW/relay.py
--rw-r--r--   0 arda      (1000) arda      (1000)     1039 2021-06-14 20:44:09.000000 ProgettiHWSW-0.1.2/ProgettiHWSW/temperature.py
-drwxrwxr-x   0 arda      (1000) arda      (1000)        0 2021-06-14 20:57:09.498829 ProgettiHWSW-0.1.2/ProgettiHWSW.egg-info/
--rw-rw-r--   0 arda      (1000) arda      (1000)     1013 2021-06-14 20:57:09.000000 ProgettiHWSW-0.1.2/ProgettiHWSW.egg-info/PKG-INFO
--rw-rw-r--   0 arda      (1000) arda      (1000)      426 2021-06-14 20:57:09.000000 ProgettiHWSW-0.1.2/ProgettiHWSW.egg-info/SOURCES.txt
--rw-rw-r--   0 arda      (1000) arda      (1000)        1 2021-06-14 20:57:09.000000 ProgettiHWSW-0.1.2/ProgettiHWSW.egg-info/dependency_links.txt
--rw-rw-r--   0 arda      (1000) arda      (1000)        1 2021-06-14 20:57:09.000000 ProgettiHWSW-0.1.2/ProgettiHWSW.egg-info/not-zip-safe
--rw-rw-r--   0 arda      (1000) arda      (1000)       13 2021-06-14 20:57:09.000000 ProgettiHWSW-0.1.2/ProgettiHWSW.egg-info/requires.txt
--rw-rw-r--   0 arda      (1000) arda      (1000)       13 2021-06-14 20:57:09.000000 ProgettiHWSW-0.1.2/ProgettiHWSW.egg-info/top_level.txt
--rwxrwxrwx   0 arda      (1000) arda      (1000)      192 2020-11-19 20:06:55.000000 ProgettiHWSW-0.1.2/README.md
--rw-rw-r--   0 arda      (1000) arda      (1000)       38 2021-06-14 20:57:09.502829 ProgettiHWSW-0.1.2/setup.cfg
--rwxrwxrwx   0 arda      (1000) arda      (1000)     1221 2021-06-14 20:56:01.000000 ProgettiHWSW-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-06 07:54:07.778021 ProgettiHWSW-0.1.3/
+-rw-rw-rw-   0        0        0      975 2023-05-06 07:54:07.776016 ProgettiHWSW-0.1.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-06 07:54:07.734806 ProgettiHWSW-0.1.3/ProgettiHWSW/
+-rw-rw-rw-   0        0        0     4425 2023-05-06 07:51:46.000000 ProgettiHWSW-0.1.3/ProgettiHWSW/ProgettiHWSWAPI.py
+-rw-rw-rw-   0        0        0       60 2021-06-14 20:44:09.000000 ProgettiHWSW-0.1.3/ProgettiHWSW/__init__.py
+-rw-rw-rw-   0        0        0     1035 2023-05-06 07:51:32.000000 ProgettiHWSW-0.1.3/ProgettiHWSW/analog.py
+-rw-rw-rw-   0        0        0      803 2021-06-14 20:44:09.000000 ProgettiHWSW-0.1.3/ProgettiHWSW/api.py
+-rw-rw-rw-   0        0        0      173 2021-06-14 20:44:09.000000 ProgettiHWSW-0.1.3/ProgettiHWSW/const.py
+-rw-rw-rw-   0        0        0     1066 2023-05-06 07:51:48.000000 ProgettiHWSW-0.1.3/ProgettiHWSW/input.py
+-rw-rw-rw-   0        0        0     1690 2023-05-06 07:51:40.000000 ProgettiHWSW-0.1.3/ProgettiHWSW/relay.py
+-rw-rw-rw-   0        0        0     1039 2021-06-14 20:44:09.000000 ProgettiHWSW-0.1.3/ProgettiHWSW/temperature.py
+drwxrwxrwx   0        0        0        0 2023-05-06 07:54:07.773516 ProgettiHWSW-0.1.3/ProgettiHWSW.egg-info/
+-rw-rw-rw-   0        0        0      975 2023-05-06 07:54:07.000000 ProgettiHWSW-0.1.3/ProgettiHWSW.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      426 2023-05-06 07:54:07.000000 ProgettiHWSW-0.1.3/ProgettiHWSW.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 07:54:07.000000 ProgettiHWSW-0.1.3/ProgettiHWSW.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-06 07:54:07.000000 ProgettiHWSW-0.1.3/ProgettiHWSW.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       13 2023-05-06 07:54:07.000000 ProgettiHWSW-0.1.3/ProgettiHWSW.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-06 07:54:07.000000 ProgettiHWSW-0.1.3/ProgettiHWSW.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      192 2020-11-19 20:06:55.000000 ProgettiHWSW-0.1.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-06 07:54:07.778021 ProgettiHWSW-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1221 2023-05-06 07:53:30.000000 ProgettiHWSW-0.1.3/setup.py
```

### Comparing `ProgettiHWSW-0.1.2/ProgettiHWSW/ProgettiHWSWAPI.py` & `ProgettiHWSW-0.1.3/ProgettiHWSW/ProgettiHWSWAPI.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,26 +21,27 @@
         """Initialize the API and return the corresponding object class."""
         self.api = API(f"http://{ip}")
         self.ip = ip
         self.board_data = None
 
     def create_unique_id(self, number, io_type: str):
         """Generate an id based on IP address and a number."""
-        unencoded_ascii = (f"{self.ip}_{io_type}_{number}_{random.random()}").encode('ascii')
+        unencoded_ascii = (
+            f"{self.ip}_{io_type}_{number}_{random.random()}").encode('ascii')
         base64_bytes = base64.b64encode(unencoded_ascii)
-        
+
         return base64_bytes.decode('ascii')
 
     async def check_board(self):
         """Check if this board is existing and valid."""
         request = await self.api.request(STATUS_XML_PATH)
         if request is False:
             return False
 
-        root = etree.XML(bytes(request, encoding = 'utf-8'))
+        root = etree.XML(bytes(request, encoding='utf-8'))
 
         relay_tags = root.xpath("//*[starts-with(local-name(), 'led')]")
         input_tags = root.xpath("//*[starts-with(local-name(), 'btn')]")
         analog_tags = root.xpath("//*[starts-with(local-name(), 'pot')]")
         temp_tags = root.xpath("//*[starts-with(local-name(), 'temp')]")
         rfid_tags = root.xpath("//*[starts-with(local-name(), 'rfid')]")
 
@@ -60,23 +61,23 @@
 
     async def get_states_by_tag_prefix(self, tag: str, is_analog: bool = False):
         """Return all states with the XML tag prefix."""
         request = await self.api.request(STATUS_XML_PATH)
         if request is False:
             return False
 
-        root = etree.XML(bytes(request, encoding = 'utf-8'))
+        root = etree.XML(bytes(request, encoding='utf-8'))
         tags = root.xpath(f"//*[starts-with(local-name(), '{tag}')]")
 
         if len(tags) <= 0:
             return False
 
         states = {}
         for i in tags:
-            number = str(i.tag[len(tag):])
+            number = str(i.tag[len(tag):], 16)
             if is_analog:
                 states[number] = i.text
             else:
                 states[number] = (
                     True if i.text in ("up", "1", "on") else False
                 )
 
@@ -84,15 +85,15 @@
 
     async def get_rfid(self):
         """Return the RFID number of lastly read tag."""
         request = await self.api.request(STATUS_XML_PATH)
         if request is False:
             return False
 
-        root = etree.XML(bytes(request, encoding = 'utf-8'))
+        root = etree.XML(bytes(request, encoding='utf-8'))
         tags = root.xpath(f"//*[starts-with(local-name(), 'rfid')]")
 
         if len(tags) <= 0:
             return False
 
         rfid_number = tags[0].text
 
@@ -125,8 +126,7 @@
     def get_pot(self, pot_number: int) -> AnalogInput:
         """Return the AnalogInput class."""
         return AnalogInput(self.api, pot_number)
 
     def get_temp(self, temp_number: int) -> Temperature:
         """Return the Temperature class."""
         return Temperature(self.api, temp_number)
-
```

### Comparing `ProgettiHWSW-0.1.2/ProgettiHWSW/analog.py` & `ProgettiHWSW-0.1.3/ProgettiHWSW/analog.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
     async def update(self):
         """Update the input status."""
         request = await self.api.request(STATUS_XML_PATH)
         if request is False:
             return False
 
-        root = etree.XML(bytes(request, encoding = 'utf-8'))
+        root = etree.XML(bytes(request, encoding='utf-8'))
 
         path = root.xpath(f"//pot{str(self.pot_number)}")
         if not len(path) > 0:
             return False
 
         self._state = path[0].text
         return True
```

### Comparing `ProgettiHWSW-0.1.2/ProgettiHWSW/api.py` & `ProgettiHWSW-0.1.3/ProgettiHWSW/api.py`

 * *Files identical despite different names*

### Comparing `ProgettiHWSW-0.1.2/ProgettiHWSW/input.py` & `ProgettiHWSW-0.1.3/ProgettiHWSW/input.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
     async def update(self):
         """Update the input status."""
         request = await self.api.request(STATUS_XML_PATH)
         if request is False:
             return False
 
-        root = etree.XML(bytes(request, encoding = 'utf-8'))
+        root = etree.XML(bytes(request, encoding='utf-8'))
 
         path = root.xpath(f"//btn{str(self.input_number)}")
         if not len(path) > 0:
             return False
 
         self.state = True if path[0].text in ("up", "1", "on") else False
         return True
```

### Comparing `ProgettiHWSW-0.1.2/ProgettiHWSW/relay.py` & `ProgettiHWSW-0.1.3/ProgettiHWSW/relay.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,27 +36,28 @@
         """Toggle the relay."""
         command = TOGGLE_BASE + self.relay_number
         await self.api.execute(command)
 
     async def control(self, state: bool):
         """Control the relay state."""
         command = (
-            (TURN_ON_BASE if self.relay_mode == "bistable" else TEMP_MONOSTABLE_BASE)
+            (TURN_ON_BASE if self.relay_mode ==
+             "bistable" else TEMP_MONOSTABLE_BASE)
             if state is True
             else TURN_OFF_BASE
         ) + self.relay_number
         await self.api.execute(command)
 
     async def update(self):
         """Update the relay status."""
         request = await self.api.request(STATUS_XML_PATH)
         if request is False:
             return False
 
-        root = etree.XML(bytes(request, encoding = 'utf-8'))
+        root = etree.XML(bytes(request, encoding='utf-8'))
 
         path = root.xpath(f"//led{str(self.relay_number)}")
         if not len(path) > 0:
             return False
 
         self.state = True if path[0].text in ("up", "1", "on") else False
         return True
```

### Comparing `ProgettiHWSW-0.1.2/ProgettiHWSW/temperature.py` & `ProgettiHWSW-0.1.3/ProgettiHWSW/temperature.py`

 * *Files identical despite different names*

### Comparing `ProgettiHWSW-0.1.2/setup.py` & `ProgettiHWSW-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,20 +9,20 @@
         return readable.read()
 
 
 README = read_file("README.md")
 
 setuptools.setup(
     name="ProgettiHWSW",
-    version="0.1.2",
+    version="0.1.3",
     long_description="\n\n".join([README]),
     long_description_content_type="text/markdown",
     description="Controls ProgettiHWSW relay boards.",
     url="http://github.com/ardaseremet/progettihwsw",
-    download_url="http://github.com/ardaseremet/progettihwsw/tarball/0.1.2",
+    download_url="http://github.com/ardaseremet/progettihwsw/tarball/0.1.3",
     author="Arda Seremet",
     author_email="ardaseremet@outlook.com",
     license="MIT",
     packages=setuptools.find_packages(),
     install_requires=["aiohttp", "lxml"],
     zip_safe=False,
     classifiers=[
```

