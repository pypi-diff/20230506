# Comparing `tmp/RobloxPyApi3-2.0.732a0.tar.gz` & `tmp/RobloxPyApi3-2.0.754.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RobloxPyApi3-2.0.732a0.tar", last modified: Sat May  6 16:02:22 2023, max compression
+gzip compressed data, was "RobloxPyApi3-2.0.754.tar", last modified: Sat May  6 16:10:22 2023, max compression
```

## Comparing `RobloxPyApi3-2.0.732a0.tar` & `RobloxPyApi3-2.0.754.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 16:02:24.000000 RobloxPyApi3-2.0.732a0/
--rw-rw-rw-   0        0        0       61 2023-04-27 12:20:20.000000 RobloxPyApi3-2.0.732a0/MANIFEST.in
--rw-rw-rw-   0        0        0     2229 2023-05-06 16:02:24.000000 RobloxPyApi3-2.0.732a0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-06 16:02:24.000000 RobloxPyApi3-2.0.732a0/RobloxPyApi3/
--rw-rw-rw-   0        0        0    19220 2023-04-27 12:29:54.000000 RobloxPyApi3-2.0.732a0/RobloxPyApi3/AccountInformation.py
--rw-rw-rw-   0        0        0    15348 2023-05-05 19:16:44.000000 RobloxPyApi3-2.0.732a0/RobloxPyApi3/Auth.py
--rw-rw-rw-   0        0        0    21919 2023-04-27 12:29:56.000000 RobloxPyApi3-2.0.732a0/RobloxPyApi3/Avatar.py
--rw-rw-rw-   0        0        0    16458 2023-05-06 16:02:08.000000 RobloxPyApi3-2.0.732a0/RobloxPyApi3/Captcha.py
--rw-rw-rw-   0        0        0    36825 2023-04-27 12:29:56.000000 RobloxPyApi3-2.0.732a0/RobloxPyApi3/Catalog.py
--rw-rw-rw-   0        0        0     2739 2023-04-08 19:22:28.000000 RobloxPyApi3-2.0.732a0/RobloxPyApi3/Check.png
--rw-rw-rw-   0        0        0    18452 2023-04-27 12:29:56.000000 RobloxPyApi3-2.0.732a0/RobloxPyApi3/Client.py
--rw-rw-rw-   0        0        0     1557 2023-04-12 19:25:10.000000 RobloxPyApi3-2.0.732a0/RobloxPyApi3/Enums.py
--rw-rw-rw-   0        0        0     2213 2023-04-09 08:16:10.000000 RobloxPyApi3-2.0.732a0/RobloxPyApi3/Errors.py
--rw-rw-rw-   0        0        0    14748 2023-04-27 12:29:54.000000 RobloxPyApi3-2.0.732a0/RobloxPyApi3/FriendsAPI.py
--rw-rw-rw-   0        0        0     5938 2023-04-27 12:30:26.000000 RobloxPyApi3-2.0.732a0/RobloxPyApi3/JoinGame.py
--rw-rw-rw-   0        0        0      461 2023-04-27 12:29:54.000000 RobloxPyApi3-2.0.732a0/RobloxPyApi3/LeaveGame.py
--rw-rw-rw-   0        0        0     9570 2023-05-05 19:39:40.000000 RobloxPyApi3-2.0.732a0/RobloxPyApi3/MultiAccount.py
-drwxrwxrwx   0        0        0        0 2023-05-06 16:02:24.000000 RobloxPyApi3-2.0.732a0/RobloxPyApi3/Place/
--rw-rw-rw-   0        0        0     1977 2023-03-30 08:25:08.000000 RobloxPyApi3-2.0.732a0/RobloxPyApi3/Place/CallMethods.py
--rw-rw-rw-   0        0        0     3312 2023-04-27 12:29:54.000000 RobloxPyApi3-2.0.732a0/RobloxPyApi3/Place/Instructions.py
--rw-rw-rw-   0        0        0    26394 2023-04-27 12:29:56.000000 RobloxPyApi3-2.0.732a0/RobloxPyApi3/Place/Place.py
--rw-rw-rw-   0        0        0      122 2023-04-27 12:29:56.000000 RobloxPyApi3-2.0.732a0/RobloxPyApi3/Place/__init__.py
--rw-rw-rw-   0        0        0     9691 2023-04-27 12:29:54.000000 RobloxPyApi3-2.0.732a0/RobloxPyApi3/Place/rbxLua2py.py
--rw-rw-rw-   0        0        0     5550 2023-03-03 16:26:02.000000 RobloxPyApi3-2.0.732a0/RobloxPyApi3/Place.py
--rw-rw-rw-   0        0        0        0 2023-03-03 14:18:04.000000 RobloxPyApi3-2.0.732a0/RobloxPyApi3/PlacePropTypes.py
--rw-rw-rw-   0        0        0      505 2023-04-27 12:29:54.000000 RobloxPyApi3-2.0.732a0/RobloxPyApi3/SessionUtilities.py
--rw-rw-rw-   0        0        0       50 2023-04-15 15:18:22.000000 RobloxPyApi3-2.0.732a0/RobloxPyApi3/Test.py
--rw-rw-rw-   0        0        0     2762 2023-04-27 12:24:10.000000 RobloxPyApi3-2.0.732a0/RobloxPyApi3/Utilities.py
--rw-rw-rw-   0        0        0     1594 2023-04-27 13:26:04.000000 RobloxPyApi3-2.0.732a0/RobloxPyApi3/Version.py
--rw-rw-rw-   0        0        0     1049 2023-05-05 11:47:44.000000 RobloxPyApi3-2.0.732a0/RobloxPyApi3/__Changes__.py
--rw-rw-rw-   0        0        0    50881 2023-04-27 12:22:44.000000 RobloxPyApi3-2.0.732a0/RobloxPyApi3/__init__.py
--rw-rw-rw-   0        0        0     4637 2023-04-27 12:29:56.000000 RobloxPyApi3-2.0.732a0/RobloxPyApi3/friends.py
-drwxrwxrwx   0        0        0        0 2023-05-06 16:02:24.000000 RobloxPyApi3-2.0.732a0/RobloxPyApi3.egg-info/
--rw-rw-rw-   0        0        0     2229 2023-05-06 16:02:22.000000 RobloxPyApi3-2.0.732a0/RobloxPyApi3.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      918 2023-05-06 16:02:24.000000 RobloxPyApi3-2.0.732a0/RobloxPyApi3.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 16:02:22.000000 RobloxPyApi3-2.0.732a0/RobloxPyApi3.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2023-05-06 16:02:22.000000 RobloxPyApi3-2.0.732a0/RobloxPyApi3.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-06 16:02:22.000000 RobloxPyApi3-2.0.732a0/RobloxPyApi3.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-06 16:02:24.000000 RobloxPyApi3-2.0.732a0/setup.cfg
--rw-rw-rw-   0        0        0     2721 2023-05-06 16:02:08.000000 RobloxPyApi3-2.0.732a0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-06 16:10:22.000000 RobloxPyApi3-2.0.754/
+-rw-rw-rw-   0        0        0       61 2023-04-27 12:20:20.000000 RobloxPyApi3-2.0.754/MANIFEST.in
+-rw-rw-rw-   0        0        0     2235 2023-05-06 16:10:24.000000 RobloxPyApi3-2.0.754/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-06 16:10:22.000000 RobloxPyApi3-2.0.754/RobloxPyApi3/
+-rw-rw-rw-   0        0        0    19220 2023-04-27 12:29:54.000000 RobloxPyApi3-2.0.754/RobloxPyApi3/AccountInformation.py
+-rw-rw-rw-   0        0        0    15348 2023-05-05 19:16:44.000000 RobloxPyApi3-2.0.754/RobloxPyApi3/Auth.py
+-rw-rw-rw-   0        0        0    21919 2023-04-27 12:29:56.000000 RobloxPyApi3-2.0.754/RobloxPyApi3/Avatar.py
+-rw-rw-rw-   0        0        0    16423 2023-05-06 16:08:36.000000 RobloxPyApi3-2.0.754/RobloxPyApi3/Captcha.py
+-rw-rw-rw-   0        0        0    36825 2023-04-27 12:29:56.000000 RobloxPyApi3-2.0.754/RobloxPyApi3/Catalog.py
+-rw-rw-rw-   0        0        0     2739 2023-04-08 19:22:28.000000 RobloxPyApi3-2.0.754/RobloxPyApi3/Check.png
+-rw-rw-rw-   0        0        0    18452 2023-04-27 12:29:56.000000 RobloxPyApi3-2.0.754/RobloxPyApi3/Client.py
+-rw-rw-rw-   0        0        0     1557 2023-04-12 19:25:10.000000 RobloxPyApi3-2.0.754/RobloxPyApi3/Enums.py
+-rw-rw-rw-   0        0        0     2213 2023-04-09 08:16:10.000000 RobloxPyApi3-2.0.754/RobloxPyApi3/Errors.py
+-rw-rw-rw-   0        0        0    14748 2023-04-27 12:29:54.000000 RobloxPyApi3-2.0.754/RobloxPyApi3/FriendsAPI.py
+-rw-rw-rw-   0        0        0     5938 2023-04-27 12:30:26.000000 RobloxPyApi3-2.0.754/RobloxPyApi3/JoinGame.py
+-rw-rw-rw-   0        0        0      461 2023-04-27 12:29:54.000000 RobloxPyApi3-2.0.754/RobloxPyApi3/LeaveGame.py
+-rw-rw-rw-   0        0        0     9570 2023-05-05 19:39:40.000000 RobloxPyApi3-2.0.754/RobloxPyApi3/MultiAccount.py
+drwxrwxrwx   0        0        0        0 2023-05-06 16:10:22.000000 RobloxPyApi3-2.0.754/RobloxPyApi3/Place/
+-rw-rw-rw-   0        0        0     1977 2023-03-30 08:25:08.000000 RobloxPyApi3-2.0.754/RobloxPyApi3/Place/CallMethods.py
+-rw-rw-rw-   0        0        0     3312 2023-04-27 12:29:54.000000 RobloxPyApi3-2.0.754/RobloxPyApi3/Place/Instructions.py
+-rw-rw-rw-   0        0        0    26394 2023-04-27 12:29:56.000000 RobloxPyApi3-2.0.754/RobloxPyApi3/Place/Place.py
+-rw-rw-rw-   0        0        0      122 2023-04-27 12:29:56.000000 RobloxPyApi3-2.0.754/RobloxPyApi3/Place/__init__.py
+-rw-rw-rw-   0        0        0     9691 2023-04-27 12:29:54.000000 RobloxPyApi3-2.0.754/RobloxPyApi3/Place/rbxLua2py.py
+-rw-rw-rw-   0        0        0     5550 2023-03-03 16:26:02.000000 RobloxPyApi3-2.0.754/RobloxPyApi3/Place.py
+-rw-rw-rw-   0        0        0        0 2023-03-03 14:18:04.000000 RobloxPyApi3-2.0.754/RobloxPyApi3/PlacePropTypes.py
+-rw-rw-rw-   0        0        0      505 2023-04-27 12:29:54.000000 RobloxPyApi3-2.0.754/RobloxPyApi3/SessionUtilities.py
+-rw-rw-rw-   0        0        0       50 2023-04-15 15:18:22.000000 RobloxPyApi3-2.0.754/RobloxPyApi3/Test.py
+-rw-rw-rw-   0        0        0     2762 2023-04-27 12:24:10.000000 RobloxPyApi3-2.0.754/RobloxPyApi3/Utilities.py
+-rw-rw-rw-   0        0        0     1594 2023-04-27 13:26:04.000000 RobloxPyApi3-2.0.754/RobloxPyApi3/Version.py
+-rw-rw-rw-   0        0        0     1049 2023-05-05 11:47:44.000000 RobloxPyApi3-2.0.754/RobloxPyApi3/__Changes__.py
+-rw-rw-rw-   0        0        0    50881 2023-04-27 12:22:44.000000 RobloxPyApi3-2.0.754/RobloxPyApi3/__init__.py
+-rw-rw-rw-   0        0        0     4637 2023-04-27 12:29:56.000000 RobloxPyApi3-2.0.754/RobloxPyApi3/friends.py
+drwxrwxrwx   0        0        0        0 2023-05-06 16:10:22.000000 RobloxPyApi3-2.0.754/RobloxPyApi3.egg-info/
+-rw-rw-rw-   0        0        0     2235 2023-05-06 16:10:22.000000 RobloxPyApi3-2.0.754/RobloxPyApi3.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      918 2023-05-06 16:10:22.000000 RobloxPyApi3-2.0.754/RobloxPyApi3.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 16:10:22.000000 RobloxPyApi3-2.0.754/RobloxPyApi3.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2023-05-06 16:10:22.000000 RobloxPyApi3-2.0.754/RobloxPyApi3.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-06 16:10:22.000000 RobloxPyApi3-2.0.754/RobloxPyApi3.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-06 16:10:24.000000 RobloxPyApi3-2.0.754/setup.cfg
+-rw-rw-rw-   0        0        0     2728 2023-05-06 16:10:06.000000 RobloxPyApi3-2.0.754/setup.py
```

### Comparing `RobloxPyApi3-2.0.732a0/PKG-INFO` & `RobloxPyApi3-2.0.754/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: RobloxPyApi3
-Version: 2.0.732a0
-Summary: RobloxPyApi3 is a Python API controller for Roblox, offering API wrapping, multi-account management, and more. Create and manage Roblox accounts and Places with ease.
+Version: 2.0.754
+Summary: RobloxPyApi3 is a Python API controller for Roblox, offering API wrapping, multi-account management, and more. Create and manage Roblox accounts and Places with ease. Thanks.
 Author: pyProjects3 (github.com/pyProjects3)
 License: MIT
 Keywords: Roblox,Api,wrapper,Bot,Client,Automated,Account Management,rbx,Python3,Place automation,post requests,get requests,JSON,Authorization,Roblox Development
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `RobloxPyApi3-2.0.732a0/RobloxPyApi3/AccountInformation.py` & `RobloxPyApi3-2.0.754/RobloxPyApi3/AccountInformation.py`

 * *Files identical despite different names*

### Comparing `RobloxPyApi3-2.0.732a0/RobloxPyApi3/Auth.py` & `RobloxPyApi3-2.0.754/RobloxPyApi3/Auth.py`

 * *Files identical despite different names*

### Comparing `RobloxPyApi3-2.0.732a0/RobloxPyApi3/Avatar.py` & `RobloxPyApi3-2.0.754/RobloxPyApi3/Avatar.py`

 * *Files identical despite different names*

### Comparing `RobloxPyApi3-2.0.732a0/RobloxPyApi3/Captcha.py` & `RobloxPyApi3-2.0.754/RobloxPyApi3/Captcha.py`

 * *Files 1% similar despite different names*

```diff
@@ -298,16 +298,14 @@
             solver_url = f'https://roblox-api.arkoselabs.com/fc/gc/?token={self.TokenID}&{self.location}&lang=en&pk={self.Type}&cdn_url=https%3A%2F%2Froblox-api.arkoselabs.com%2Fcdn%2Ffc'
             #print(
                 #f'- Received Captcha Details!\n\n\nCaptchaId : {self.ID}\nCaptchaBlob : {self.blob}\nLocation : {self.location}\ntoken : {self.TokenID}\n\n\n(Starting selenium browser to solve the captcha)..\n\n\n')
             print("[INFO] Starting Web browser to solve the captcha.")
             time.sleep(1)
             WEB.open(solver_url)
             time.sleep(1)
-
-            image = 'Check.png'
             d = os.path.dirname(os.path.realpath(__file__))
             p = os.path.join(d,'Check.png')
             while True:
                 try:
                     # locate the image on the screen
                     location = pyautogui.locateOnScreen(p)
```

### Comparing `RobloxPyApi3-2.0.732a0/RobloxPyApi3/Catalog.py` & `RobloxPyApi3-2.0.754/RobloxPyApi3/Catalog.py`

 * *Files identical despite different names*

### Comparing `RobloxPyApi3-2.0.732a0/RobloxPyApi3/Check.png` & `RobloxPyApi3-2.0.754/RobloxPyApi3/Check.png`

 * *Files identical despite different names*

### Comparing `RobloxPyApi3-2.0.732a0/RobloxPyApi3/Client.py` & `RobloxPyApi3-2.0.754/RobloxPyApi3/Client.py`

 * *Files identical despite different names*

### Comparing `RobloxPyApi3-2.0.732a0/RobloxPyApi3/Enums.py` & `RobloxPyApi3-2.0.754/RobloxPyApi3/Enums.py`

 * *Files identical despite different names*

### Comparing `RobloxPyApi3-2.0.732a0/RobloxPyApi3/Errors.py` & `RobloxPyApi3-2.0.754/RobloxPyApi3/Errors.py`

 * *Files identical despite different names*

### Comparing `RobloxPyApi3-2.0.732a0/RobloxPyApi3/FriendsAPI.py` & `RobloxPyApi3-2.0.754/RobloxPyApi3/FriendsAPI.py`

 * *Files identical despite different names*

### Comparing `RobloxPyApi3-2.0.732a0/RobloxPyApi3/JoinGame.py` & `RobloxPyApi3-2.0.754/RobloxPyApi3/JoinGame.py`

 * *Files identical despite different names*

### Comparing `RobloxPyApi3-2.0.732a0/RobloxPyApi3/MultiAccount.py` & `RobloxPyApi3-2.0.754/RobloxPyApi3/MultiAccount.py`

 * *Files identical despite different names*

### Comparing `RobloxPyApi3-2.0.732a0/RobloxPyApi3/Place/CallMethods.py` & `RobloxPyApi3-2.0.754/RobloxPyApi3/Place/CallMethods.py`

 * *Files identical despite different names*

### Comparing `RobloxPyApi3-2.0.732a0/RobloxPyApi3/Place/Instructions.py` & `RobloxPyApi3-2.0.754/RobloxPyApi3/Place/Instructions.py`

 * *Files identical despite different names*

### Comparing `RobloxPyApi3-2.0.732a0/RobloxPyApi3/Place/Place.py` & `RobloxPyApi3-2.0.754/RobloxPyApi3/Place/Place.py`

 * *Files identical despite different names*

### Comparing `RobloxPyApi3-2.0.732a0/RobloxPyApi3/Place/rbxLua2py.py` & `RobloxPyApi3-2.0.754/RobloxPyApi3/Place/rbxLua2py.py`

 * *Files identical despite different names*

### Comparing `RobloxPyApi3-2.0.732a0/RobloxPyApi3/Place.py` & `RobloxPyApi3-2.0.754/RobloxPyApi3/Place.py`

 * *Files identical despite different names*

### Comparing `RobloxPyApi3-2.0.732a0/RobloxPyApi3/Utilities.py` & `RobloxPyApi3-2.0.754/RobloxPyApi3/Utilities.py`

 * *Files identical despite different names*

### Comparing `RobloxPyApi3-2.0.732a0/RobloxPyApi3/Version.py` & `RobloxPyApi3-2.0.754/RobloxPyApi3/Version.py`

 * *Files identical despite different names*

### Comparing `RobloxPyApi3-2.0.732a0/RobloxPyApi3/__Changes__.py` & `RobloxPyApi3-2.0.754/RobloxPyApi3/__Changes__.py`

 * *Files identical despite different names*

### Comparing `RobloxPyApi3-2.0.732a0/RobloxPyApi3/__init__.py` & `RobloxPyApi3-2.0.754/RobloxPyApi3/__init__.py`

 * *Files identical despite different names*

### Comparing `RobloxPyApi3-2.0.732a0/RobloxPyApi3/friends.py` & `RobloxPyApi3-2.0.754/RobloxPyApi3/friends.py`

 * *Files identical despite different names*

### Comparing `RobloxPyApi3-2.0.732a0/RobloxPyApi3.egg-info/PKG-INFO` & `RobloxPyApi3-2.0.754/RobloxPyApi3.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: RobloxPyApi3
-Version: 2.0.732a0
-Summary: RobloxPyApi3 is a Python API controller for Roblox, offering API wrapping, multi-account management, and more. Create and manage Roblox accounts and Places with ease.
+Version: 2.0.754
+Summary: RobloxPyApi3 is a Python API controller for Roblox, offering API wrapping, multi-account management, and more. Create and manage Roblox accounts and Places with ease. Thanks.
 Author: pyProjects3 (github.com/pyProjects3)
 License: MIT
 Keywords: Roblox,Api,wrapper,Bot,Client,Automated,Account Management,rbx,Python3,Place automation,post requests,get requests,JSON,Authorization,Roblox Development
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `RobloxPyApi3-2.0.732a0/RobloxPyApi3.egg-info/SOURCES.txt` & `RobloxPyApi3-2.0.754/RobloxPyApi3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `RobloxPyApi3-2.0.732a0/setup.py` & `RobloxPyApi3-2.0.754/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 from RobloxPyApi3.Version import __Copyright__
-Version = "2.0.732a"
+Version = "2.0.754"
 
-Description = "RobloxPyApi3 is a Python API controller for Roblox, offering API wrapping, multi-account management, and more. Create and manage Roblox accounts and Places with ease."
+Description = "RobloxPyApi3 is a Python API controller for Roblox, offering API wrapping, multi-account management, and more. Create and manage Roblox accounts and Places with ease. Thanks."
 
 Long_Description = f"""
 Welcome to the RobloxPyAPI3 package, created by pyProjects3. This package is designed to make Roblox game development possible in python, API Wrapper (Access Roblox API), Multi Account management and being able to join games and leave games.
 
 One of the key features of this package is its support for Place creation. With our Place creation tools, you can now create your Roblox Places in python, whether you're working on a personal project or developing a game with a team. Our tools make it easy to upload new assets, manage permissions, and more.
 
 In addition to Place creation, the RobloxPyAPI3 package includes an API Wrapper that provides easy access to the Roblox API. Our wrapper simplifies the process of sending and receiving data from the Roblox API, making it easier to build automated bots and other tools that interact with the Roblox platform.
```

