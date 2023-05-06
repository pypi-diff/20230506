# Comparing `tmp/pyroporn-0.2.1.tar.gz` & `tmp/pyroporn-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyroporn-0.2.1.tar", last modified: Sat May  6 07:41:49 2023, max compression
+gzip compressed data, was "pyroporn-0.2.2.tar", last modified: Sat May  6 07:51:42 2023, max compression
```

## Comparing `pyroporn-0.2.1.tar` & `pyroporn-0.2.2.tar`

### file list

```diff
@@ -1,56 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 07:41:49.269063 pyroporn-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-06 07:41:49.269063 pyroporn-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-06 07:41:34.000000 pyroporn-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 07:41:49.257063 pyroporn-0.2.1/pyroporn/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-06 07:41:34.000000 pyroporn-0.2.1/pyroporn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20991 2023-05-06 07:41:34.000000 pyroporn-0.2.1/pyroporn/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6623 2023-05-06 07:41:34.000000 pyroporn-0.2.1/pyroporn/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 07:41:49.261062 pyroporn-0.2.1/pyroporn/database/
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-06 07:41:34.000000 pyroporn-0.2.1/pyroporn/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-05-06 07:41:34.000000 pyroporn-0.2.1/pyroporn/database/bdbDatabase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-05-06 07:41:34.000000 pyroporn-0.2.1/pyroporn/database/bubDatabase.py
--rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-05-06 07:41:34.000000 pyroporn-0.2.1/pyroporn/database/othDatabase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-05-06 07:41:34.000000 pyroporn-0.2.1/pyroporn/database/papDatabase.py
--rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-05-06 07:41:34.000000 pyroporn-0.2.1/pyroporn/database/pmoDatabase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-06 07:41:34.000000 pyroporn-0.2.1/pyroporn/database/pobDatabase.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 07:41:49.265063 pyroporn-0.2.1/pyroporn/decorators/
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-06 07:41:34.000000 pyroporn-0.2.1/pyroporn/decorators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-06 07:41:34.000000 pyroporn-0.2.1/pyroporn/decorators/addhandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-05-06 07:41:34.000000 pyroporn-0.2.1/pyroporn/decorators/botcmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6317 2023-05-06 07:41:34.000000 pyroporn-0.2.1/pyroporn/decorators/forcesub.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-06 07:41:34.000000 pyroporn-0.2.1/pyroporn/decorators/genbuttons.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-06 07:41:34.000000 pyroporn-0.2.1/pyroporn/decorators/getjson.py
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-06 07:41:34.000000 pyroporn-0.2.1/pyroporn/decorators/getlink.py
--rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-05-06 07:41:34.000000 pyroporn-0.2.1/pyroporn/decorators/oncmd.py
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-06 07:41:34.000000 pyroporn-0.2.1/pyroporn/decorators/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 07:41:49.265063 pyroporn-0.2.1/pyroporn/methods/
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-06 07:41:34.000000 pyroporn-0.2.1/pyroporn/methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-05-06 07:41:34.000000 pyroporn-0.2.1/pyroporn/methods/content.py
--rw-r--r--   0 runner    (1001) docker     (123)     8161 2023-05-06 07:41:34.000000 pyroporn-0.2.1/pyroporn/methods/getfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     7325 2023-05-06 07:41:34.000000 pyroporn-0.2.1/pyroporn/methods/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     9364 2023-05-06 07:41:34.000000 pyroporn-0.2.1/pyroporn/methods/thumbnail.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 07:41:49.269063 pyroporn-0.2.1/pyroporn/types/
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-06 07:41:34.000000 pyroporn-0.2.1/pyroporn/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10063 2023-05-06 07:41:34.000000 pyroporn-0.2.1/pyroporn/types/inline.py
--rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-05-06 07:41:34.000000 pyroporn-0.2.1/pyroporn/types/inlineBdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-05-06 07:41:34.000000 pyroporn-0.2.1/pyroporn/types/inlineBub.py
--rw-r--r--   0 runner    (1001) docker     (123)     5881 2023-05-06 07:41:34.000000 pyroporn-0.2.1/pyroporn/types/inlinePob.py
--rw-r--r--   0 runner    (1001) docker     (123)     3668 2023-05-06 07:41:34.000000 pyroporn-0.2.1/pyroporn/types/inlineVip.py
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-06 07:41:34.000000 pyroporn-0.2.1/pyroporn/types/style.py
--rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-05-06 07:41:34.000000 pyroporn-0.2.1/pyroporn/types/text.py
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-05-06 07:41:34.000000 pyroporn-0.2.1/pyroporn/userbot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 07:41:49.269063 pyroporn-0.2.1/pyroporn/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-06 07:41:34.000000 pyroporn-0.2.1/pyroporn/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-05-06 07:41:34.000000 pyroporn-0.2.1/pyroporn/utilities/formater.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-06 07:41:34.000000 pyroporn-0.2.1/pyroporn/utilities/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-05-06 07:41:34.000000 pyroporn-0.2.1/pyroporn/utilities/mongo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-05-06 07:41:34.000000 pyroporn-0.2.1/pyroporn/utilities/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-06 07:41:34.000000 pyroporn-0.2.1/pyroporn/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 07:41:49.261062 pyroporn-0.2.1/pyroporn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-06 07:41:49.000000 pyroporn-0.2.1/pyroporn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-05-06 07:41:49.000000 pyroporn-0.2.1/pyroporn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 07:41:49.000000 pyroporn-0.2.1/pyroporn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-06 07:41:49.000000 pyroporn-0.2.1/pyroporn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-06 07:41:49.000000 pyroporn-0.2.1/pyroporn.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 07:41:49.269063 pyroporn-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-05-06 07:41:34.000000 pyroporn-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 07:51:42.396471 pyroporn-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-06 07:51:42.396471 pyroporn-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-06 07:51:31.000000 pyroporn-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 07:51:42.392471 pyroporn-0.2.2/pyroporn/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-06 07:51:31.000000 pyroporn-0.2.2/pyroporn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20913 2023-05-06 07:51:31.000000 pyroporn-0.2.2/pyroporn/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6623 2023-05-06 07:51:31.000000 pyroporn-0.2.2/pyroporn/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 07:51:42.392471 pyroporn-0.2.2/pyroporn/database/
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-06 07:51:31.000000 pyroporn-0.2.2/pyroporn/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-05-06 07:51:31.000000 pyroporn-0.2.2/pyroporn/database/bdbDatabase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-05-06 07:51:31.000000 pyroporn-0.2.2/pyroporn/database/bubDatabase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-05-06 07:51:31.000000 pyroporn-0.2.2/pyroporn/database/othDatabase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-05-06 07:51:31.000000 pyroporn-0.2.2/pyroporn/database/papDatabase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-05-06 07:51:31.000000 pyroporn-0.2.2/pyroporn/database/pmoDatabase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-06 07:51:31.000000 pyroporn-0.2.2/pyroporn/database/pobDatabase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 07:51:42.392471 pyroporn-0.2.2/pyroporn/decorators/
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-06 07:51:31.000000 pyroporn-0.2.2/pyroporn/decorators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-06 07:51:31.000000 pyroporn-0.2.2/pyroporn/decorators/addhandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-05-06 07:51:31.000000 pyroporn-0.2.2/pyroporn/decorators/botcmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6317 2023-05-06 07:51:31.000000 pyroporn-0.2.2/pyroporn/decorators/forcesub.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-06 07:51:31.000000 pyroporn-0.2.2/pyroporn/decorators/genbuttons.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-06 07:51:31.000000 pyroporn-0.2.2/pyroporn/decorators/getjson.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-06 07:51:31.000000 pyroporn-0.2.2/pyroporn/decorators/getlink.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-05-06 07:51:31.000000 pyroporn-0.2.2/pyroporn/decorators/oncmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-06 07:51:31.000000 pyroporn-0.2.2/pyroporn/decorators/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 07:51:42.392471 pyroporn-0.2.2/pyroporn/methods/
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-06 07:51:31.000000 pyroporn-0.2.2/pyroporn/methods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-05-06 07:51:31.000000 pyroporn-0.2.2/pyroporn/methods/content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8161 2023-05-06 07:51:31.000000 pyroporn-0.2.2/pyroporn/methods/getfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7325 2023-05-06 07:51:31.000000 pyroporn-0.2.2/pyroporn/methods/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9364 2023-05-06 07:51:31.000000 pyroporn-0.2.2/pyroporn/methods/thumbnail.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 07:51:42.396471 pyroporn-0.2.2/pyroporn/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-06 07:51:31.000000 pyroporn-0.2.2/pyroporn/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10063 2023-05-06 07:51:31.000000 pyroporn-0.2.2/pyroporn/types/inline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-05-06 07:51:31.000000 pyroporn-0.2.2/pyroporn/types/inlineBdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-05-06 07:51:31.000000 pyroporn-0.2.2/pyroporn/types/inlineBub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5881 2023-05-06 07:51:31.000000 pyroporn-0.2.2/pyroporn/types/inlinePob.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3668 2023-05-06 07:51:31.000000 pyroporn-0.2.2/pyroporn/types/inlineVip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-06 07:51:31.000000 pyroporn-0.2.2/pyroporn/types/style.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-05-06 07:51:31.000000 pyroporn-0.2.2/pyroporn/types/text.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 07:51:42.396471 pyroporn-0.2.2/pyroporn/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-06 07:51:31.000000 pyroporn-0.2.2/pyroporn/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-05-06 07:51:31.000000 pyroporn-0.2.2/pyroporn/utilities/formater.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-06 07:51:31.000000 pyroporn-0.2.2/pyroporn/utilities/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-05-06 07:51:31.000000 pyroporn-0.2.2/pyroporn/utilities/mongo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-05-06 07:51:31.000000 pyroporn-0.2.2/pyroporn/utilities/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-06 07:51:31.000000 pyroporn-0.2.2/pyroporn/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 07:51:42.392471 pyroporn-0.2.2/pyroporn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-06 07:51:42.000000 pyroporn-0.2.2/pyroporn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-05-06 07:51:42.000000 pyroporn-0.2.2/pyroporn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 07:51:42.000000 pyroporn-0.2.2/pyroporn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-06 07:51:42.000000 pyroporn-0.2.2/pyroporn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-06 07:51:42.000000 pyroporn-0.2.2/pyroporn.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 07:51:42.396471 pyroporn-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-05-06 07:51:31.000000 pyroporn-0.2.2/setup.py
```

### Comparing `pyroporn-0.2.1/PKG-INFO` & `pyroporn-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyroporn
-Version: 0.2.1
+Version: 0.2.2
 Summary: Best Porn Code for the Pyrogram Library.
 Home-page: https://github.com/OTHFamily/pyroporn
 Author: TPro
 Author-email: 
 License: MIT
 Keywords: telegram pyrogram porn bot userbot
 Classifier: Programming Language :: Python
```

### Comparing `pyroporn-0.2.1/pyroporn/client.py` & `pyroporn-0.2.2/pyroporn/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,43 +65,42 @@
         except Exception as e:
             self.logs.warning(e)
             self.logs.warning(f"Pastikan bot adalah Admin di OTH Content DB")
             sys.exit()
             
         if string:
             for session in string:
-                self.SESSION.append(str(session))
-                #bot_ = RawClient(
-                #    "NewUserbot",
-                #    api_id=self.API_ID,
-                #    api_hash=self.API_HASH,
-                #    device_model="@OnTheHerd",
-                #    session_string=session,
-                #    plugins={"root": "Tele.userbot"},
-                #)
-                #try:
-                #    await bot_.start()
-                #except AuthKeyDuplicated:
-                #    await self.del_session(session)
-                #except AuthKeyUnregistered:
-                #    await self.del_session(session)
-                #except SessionRevoked:
-                #    await self.del_session(session)
-                #except SessionPasswordNeeded:
-                #    await self.del_session(session)
-                #except UserDeactivated:
-                #    await self.del_session(session)
-                #except UserDeactivatedBan:
-                #    await self.del_session(session)
-                #self.rawbot.append(bot_)
-                #try:
-                #    mebot = await bot_.get_me()
-                #    self.logs.info(f"Userbot Started !\nName: {mebot.first_name}\nUserID: {mebot.id}")
-                #except BaseException:
-                #    pass
+                bot_ = RawClient(
+                    "NewUserbot",
+                    api_id=self.API_ID,
+                    api_hash=self.API_HASH,
+                    device_model="@OnTheHerd",
+                    session_string=session,
+                    #plugins={"root": "Tele.userbot"},
+                )
+                try:
+                    await bot_.start()
+                except AuthKeyDuplicated:
+                    await self.del_session(session)
+                except AuthKeyUnregistered:
+                    await self.del_session(session)
+                except SessionRevoked:
+                    await self.del_session(session)
+                except SessionPasswordNeeded:
+                    await self.del_session(session)
+                except UserDeactivated:
+                    await self.del_session(session)
+                except UserDeactivatedBan:
+                    await self.del_session(session)
+                self.rawbot.append(bot_)
+                try:
+                    mebot = await bot_.get_me()
+                    self.logs.info(f"Userbot Started !\nName: {mebot.first_name}\nUserID: {mebot.id}")
+                except BaseException:
+                    pass
         self.BLCHAT.append(self.id)
         self.logs.info(f"OTH Started !\nName: {self.name}\nUserID: {self.id}")     
     
     async def stop(self, *args):
         await super().stop()
         
         
@@ -541,8 +540,8 @@
                             await self.add_user_bub(str(user_id), user)
                         self.bububot.append(bot_)
                         mebot = await bot_.get_me()
                         self.userbub.append(mebot.id)
                         self.logs.info(f"BUB Userbot Started !\nName: {mebot.first_name}\nUserID: {mebot.id}")
                     
         async def stop(self, *args):
-            await super().stop()
+            await super().stop()
```

### Comparing `pyroporn-0.2.1/pyroporn/config.py` & `pyroporn-0.2.2/pyroporn/config.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.2.1/pyroporn/database/bdbDatabase.py` & `pyroporn-0.2.2/pyroporn/database/bdbDatabase.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.2.1/pyroporn/database/bubDatabase.py` & `pyroporn-0.2.2/pyroporn/database/bubDatabase.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.2.1/pyroporn/database/othDatabase.py` & `pyroporn-0.2.2/pyroporn/database/othDatabase.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.2.1/pyroporn/database/papDatabase.py` & `pyroporn-0.2.2/pyroporn/database/papDatabase.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.2.1/pyroporn/database/pmoDatabase.py` & `pyroporn-0.2.2/pyroporn/database/pmoDatabase.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.2.1/pyroporn/database/pobDatabase.py` & `pyroporn-0.2.2/pyroporn/database/pobDatabase.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.2.1/pyroporn/decorators/botcmd.py` & `pyroporn-0.2.2/pyroporn/decorators/botcmd.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.2.1/pyroporn/decorators/forcesub.py` & `pyroporn-0.2.2/pyroporn/decorators/forcesub.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.2.1/pyroporn/decorators/genbuttons.py` & `pyroporn-0.2.2/pyroporn/decorators/genbuttons.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.2.1/pyroporn/decorators/getlink.py` & `pyroporn-0.2.2/pyroporn/decorators/getlink.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.2.1/pyroporn/decorators/oncmd.py` & `pyroporn-0.2.2/pyroporn/decorators/oncmd.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.2.1/pyroporn/methods/content.py` & `pyroporn-0.2.2/pyroporn/methods/content.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.2.1/pyroporn/methods/getfile.py` & `pyroporn-0.2.2/pyroporn/methods/getfile.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.2.1/pyroporn/methods/message.py` & `pyroporn-0.2.2/pyroporn/methods/message.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.2.1/pyroporn/methods/thumbnail.py` & `pyroporn-0.2.2/pyroporn/methods/thumbnail.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.2.1/pyroporn/types/inline.py` & `pyroporn-0.2.2/pyroporn/types/inline.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.2.1/pyroporn/types/inlineBdb.py` & `pyroporn-0.2.2/pyroporn/types/inlineBdb.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.2.1/pyroporn/types/inlineBub.py` & `pyroporn-0.2.2/pyroporn/types/inlineBub.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.2.1/pyroporn/types/inlinePob.py` & `pyroporn-0.2.2/pyroporn/types/inlinePob.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.2.1/pyroporn/types/inlineVip.py` & `pyroporn-0.2.2/pyroporn/types/inlineVip.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.2.1/pyroporn/types/text.py` & `pyroporn-0.2.2/pyroporn/types/text.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.2.1/pyroporn/utilities/formater.py` & `pyroporn-0.2.2/pyroporn/utilities/formater.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.2.1/pyroporn/utilities/logger.py` & `pyroporn-0.2.2/pyroporn/utilities/logger.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.2.1/pyroporn/utilities/mongo.py` & `pyroporn-0.2.2/pyroporn/utilities/mongo.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.2.1/pyroporn/utilities/utils.py` & `pyroporn-0.2.2/pyroporn/utilities/utils.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.2.1/pyroporn.egg-info/PKG-INFO` & `pyroporn-0.2.2/pyroporn.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyroporn
-Version: 0.2.1
+Version: 0.2.2
 Summary: Best Porn Code for the Pyrogram Library.
 Home-page: https://github.com/OTHFamily/pyroporn
 Author: TPro
 Author-email: 
 License: MIT
 Keywords: telegram pyrogram porn bot userbot
 Classifier: Programming Language :: Python
```

### Comparing `pyroporn-0.2.1/pyroporn.egg-info/SOURCES.txt` & `pyroporn-0.2.2/pyroporn.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 README.md
 setup.py
 pyroporn/__init__.py
 pyroporn/client.py
 pyroporn/config.py
-pyroporn/userbot.py
 pyroporn/version.py
 pyroporn.egg-info/PKG-INFO
 pyroporn.egg-info/SOURCES.txt
 pyroporn.egg-info/dependency_links.txt
 pyroporn.egg-info/requires.txt
 pyroporn.egg-info/top_level.txt
 pyroporn/database/__init__.py
```

### Comparing `pyroporn-0.2.1/setup.py` & `pyroporn-0.2.2/setup.py`

 * *Files identical despite different names*

