# Comparing `tmp/multibot-1.9.0.tar.gz` & `tmp/multibot-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multibot-1.9.0.tar", last modified: Tue Jan 10 23:34:00 2023, max compression
+gzip compressed data, was "multibot-1.9.1.tar", last modified: Sat May  6 18:45:29 2023, max compression
```

## Comparing `multibot-1.9.0.tar` & `multibot-1.9.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 23:34:00.841485 multibot-1.9.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-01-10 23:33:46.000000 multibot-1.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18570 2023-01-10 23:34:00.841485 multibot-1.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17861 2023-01-10 23:33:46.000000 multibot-1.9.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 23:34:00.833485 multibot-1.9.0/multibot/
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-01-10 23:33:46.000000 multibot-1.9.0/multibot/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 23:34:00.837485 multibot-1.9.0/multibot/bots/
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-01-10 23:33:46.000000 multibot-1.9.0/multibot/bots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29151 2023-01-10 23:33:46.000000 multibot-1.9.0/multibot/bots/discord_bot.py
--rw-r--r--   0 runner    (1001) docker     (123)    39512 2023-01-10 23:33:46.000000 multibot-1.9.0/multibot/bots/multi_bot.py
--rw-r--r--   0 runner    (1001) docker     (123)    26341 2023-01-10 23:33:46.000000 multibot-1.9.0/multibot/bots/telegram_bot.py
--rw-r--r--   0 runner    (1001) docker     (123)    12446 2023-01-10 23:33:46.000000 multibot-1.9.0/multibot/bots/twitch_bot.py
--rw-r--r--   0 runner    (1001) docker     (123)     7858 2023-01-10 23:33:46.000000 multibot-1.9.0/multibot/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-01-10 23:33:46.000000 multibot-1.9.0/multibot/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 23:34:00.837485 multibot-1.9.0/multibot/models/
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-01-10 23:33:46.000000 multibot-1.9.0/multibot/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-01-10 23:33:46.000000 multibot-1.9.0/multibot/models/buttons.py
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-01-10 23:33:46.000000 multibot-1.9.0/multibot/models/chat.py
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-01-10 23:33:46.000000 multibot-1.9.0/multibot/models/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-01-10 23:33:46.000000 multibot-1.9.0/multibot/models/event_component.py
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-01-10 23:33:46.000000 multibot-1.9.0/multibot/models/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-01-10 23:33:46.000000 multibot-1.9.0/multibot/models/penalties.py
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-01-10 23:33:46.000000 multibot-1.9.0/multibot/models/registered_callback.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-01-10 23:33:46.000000 multibot-1.9.0/multibot/models/role.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-01-10 23:33:46.000000 multibot-1.9.0/multibot/models/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 23:34:00.837485 multibot-1.9.0/multibot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18570 2023-01-10 23:34:00.000000 multibot-1.9.0/multibot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-01-10 23:34:00.000000 multibot-1.9.0/multibot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-10 23:34:00.000000 multibot-1.9.0/multibot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-01-10 23:34:00.000000 multibot-1.9.0/multibot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-01-10 23:34:00.000000 multibot-1.9.0/multibot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-01-10 23:33:46.000000 multibot-1.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-01-10 23:34:00.841485 multibot-1.9.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 18:45:29.423969 multibot-1.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-06 18:45:10.000000 multibot-1.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18536 2023-05-06 18:45:29.423969 multibot-1.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17861 2023-05-06 18:45:10.000000 multibot-1.9.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 18:45:29.415969 multibot-1.9.1/multibot/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-06 18:45:10.000000 multibot-1.9.1/multibot/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 18:45:29.419968 multibot-1.9.1/multibot/bots/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-06 18:45:10.000000 multibot-1.9.1/multibot/bots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28838 2023-05-06 18:45:10.000000 multibot-1.9.1/multibot/bots/discord_bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41050 2023-05-06 18:45:10.000000 multibot-1.9.1/multibot/bots/multi_bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26591 2023-05-06 18:45:10.000000 multibot-1.9.1/multibot/bots/telegram_bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12498 2023-05-06 18:45:10.000000 multibot-1.9.1/multibot/bots/twitch_bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7957 2023-05-06 18:45:10.000000 multibot-1.9.1/multibot/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-06 18:45:10.000000 multibot-1.9.1/multibot/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 18:45:29.423969 multibot-1.9.1/multibot/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-06 18:45:10.000000 multibot-1.9.1/multibot/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-05-06 18:45:10.000000 multibot-1.9.1/multibot/models/buttons.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-06 18:45:10.000000 multibot-1.9.1/multibot/models/chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-06 18:45:10.000000 multibot-1.9.1/multibot/models/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-06 18:45:10.000000 multibot-1.9.1/multibot/models/event_component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-05-06 18:45:10.000000 multibot-1.9.1/multibot/models/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-05-06 18:45:10.000000 multibot-1.9.1/multibot/models/penalties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-05-06 18:45:10.000000 multibot-1.9.1/multibot/models/registered_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-06 18:45:10.000000 multibot-1.9.1/multibot/models/role.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-06 18:45:10.000000 multibot-1.9.1/multibot/models/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 18:45:29.419968 multibot-1.9.1/multibot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18536 2023-05-06 18:45:29.000000 multibot-1.9.1/multibot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-06 18:45:29.000000 multibot-1.9.1/multibot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 18:45:29.000000 multibot-1.9.1/multibot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-06 18:45:29.000000 multibot-1.9.1/multibot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-06 18:45:29.000000 multibot-1.9.1/multibot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-06 18:45:10.000000 multibot-1.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-05-06 18:45:29.423969 multibot-1.9.1/setup.cfg
```

### Comparing `multibot-1.9.0/LICENSE` & `multibot-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `multibot-1.9.0/PKG-INFO` & `multibot-1.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 Metadata-Version: 2.1
 Name: multibot
-Version: 1.9.0
+Version: 1.9.1
 Summary: Platform agnostic high-level bot infrastructure. Develop one bot and you will have three: one for Discord, another one for Telegram and another one for Twitch. All bots use the same objects and logic.  For now there are adapters for three platforms but more may be added in the future.
 Home-page: https://github.com/AlberLC/multibot
 Author: AlberLC
-Author-email: alberlc@outlook.com
 Project-URL: Bug Tracker, https://github.com/AlberLC/multibot/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 License-File: LICENSE
```

### Comparing `multibot-1.9.0/README.rst` & `multibot-1.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `multibot-1.9.0/multibot/bots/discord_bot.py` & `multibot-1.9.1/multibot/bots/discord_bot.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 from __future__ import annotations  # todo0 remove when it's by default
 
 __all__ = ['DiscordBot']
 
-import asyncio
+import contextlib
 import datetime
 import io
 import logging
 import pathlib
 import random
 import traceback
 from collections.abc import Iterable, Sequence
 from typing import Any
 
 import discord
 import discord.ext
 import flanautils
-import pymongo
-from flanautils import Media, MediaType, NotFoundError, OrderedSet, return_if_first_empty
+from flanautils import Media, MediaType, NotFoundError, OrderedSet, ResponseError, return_if_first_empty
 
 from multibot import constants
 from multibot.bots.multi_bot import MultiBot, parse_arguments
 from multibot.exceptions import LimitError, SendError, UserDisconnectedError
-from multibot.models import Button, ButtonsInfo, Chat, Message, Mute, Platform, Role, User
+from multibot.models import Button, Chat, Message, Mute, Platform, Role, User
 
 
 # --------------------------------------------------------------------------------------------------- #
 # ------------------------------------------- DISCORD_BOT ------------------------------------------- #
 # --------------------------------------------------------------------------------------------------- #
 class DiscordBot(MultiBot[discord.ext.commands.Bot]):
     def __init__(self, token: str):
@@ -221,25 +220,28 @@
 
     @staticmethod
     @return_if_first_empty
     async def _prepare_media_to_send(media: Media) -> discord.File | None:
         if not media:
             return
 
-        file_stem = f"{media.title or 'bot_media'}"
+        file_stem = media.title or 'bot_media'
         file_name = f"{file_stem}{f'.{media.extension}' if media.extension else ''}"
 
         if media.url:
             if pathlib.Path(media.url).is_file():
                 if (path_suffix := pathlib.Path(media.url).suffix) and len(path_suffix) <= constants.MAX_FILE_EXTENSION_LENGHT:
                     return discord.File(media.url)
                 else:
                     return discord.File(media.url, filename=file_name)
             elif not media.bytes_:
-                media.bytes_ = await flanautils.get_request(media.url)
+                try:
+                    media.bytes_ = await flanautils.get_request(media.url)
+                except ResponseError:
+                    pass
 
         if bytes_ := media.bytes_:
             if media.type_ is MediaType.GIF:
                 bytes_ = await flanautils.to_gif(bytes_)
             if media.title:
                 try:
                     bytes_ = await flanautils.edit_metadata(bytes_, {'title': file_stem}, overwrite=False)
@@ -303,35 +305,36 @@
             user.save(('roles',))
 
     @return_if_first_empty(exclude_self_types='DiscordBot', globals_=globals())
     async def clear(self, n_messages: int, chat: int | str | Chat | Message):
         if n_messages > 100:
             raise LimitError('El máximo es 100.')
 
-        chat = await self.get_chat(chat)
-        if chat.is_private:
+        if (chat := await self.get_chat(chat)).is_private:
             return
 
+        n_messages = int(n_messages)
+
         while n_messages > 0:
             if n_messages > 100:
                 n_messages_chunk = 100
                 n_messages -= 100
             else:
                 n_messages_chunk = n_messages
                 n_messages = 0
 
             try:
-                await chat.original_object.purge(limit=n_messages_chunk)
+                message_ids = [message.id for message in await chat.original_object.purge(limit=n_messages_chunk)]
             except discord.errors.HTTPException:
                 raise LimitError(f'Solo puedo eliminar mensajes con menos de 14 días {random.choice(constants.SAD_EMOJIS)}')
 
-            database_messages_to_delete_generator = self.Message.find({'platform': self.platform.value, 'chat': chat.object_id}, sort_keys=(('date', pymongo.DESCENDING),), limit=n_messages_chunk, lazy=True)
-            for database_message_to_delete in database_messages_to_delete_generator:
-                database_message_to_delete.is_deleted = True
-                database_message_to_delete.save()
+            deleted_messages_generator = self.Message.find({'platform': self.platform.value, 'id': {'$in': message_ids}, 'chat': chat.object_id}, lazy=True)
+            for deleted_message in deleted_messages_generator:
+                deleted_message.is_deleted = True
+                deleted_message.save()
 
     @return_if_first_empty(exclude_self_types='DiscordBot', globals_=globals())
     async def delete_message(
         self,
         message_to_delete: int | str | Message,
         chat: int | str | Chat | Message = None,
         raise_not_found=False
@@ -350,15 +353,15 @@
         except discord.errors.NotFound:
             if raise_not_found:
                 raise NotFoundError(traceback.format_exc().splitlines()[-1])
         except discord.errors.Forbidden:
             return
 
         message_to_delete.is_deleted = True
-        message_to_delete.save()
+        message_to_delete.save(('is_deleted',))
 
     # noinspection PyTypeChecker
     def distribute_buttons(self, texts: Sequence[str], vertically=False) -> list[list[str]]:
         texts = [f'{text[:constants.DISCORD_BUTTON_MAX_CHARACTERS - 3]}...' if len(text) > constants.DISCORD_BUTTON_MAX_CHARACTERS else text for text in texts]
 
         if len(texts) <= constants.DISCORD_BUTTONS_MAX and vertically:
             return flanautils.chunks(texts, 1)
@@ -414,26 +417,32 @@
 
     @return_if_first_empty(exclude_self_types='DiscordBot', globals_=globals())
     async def get_chat(self, chat: int | str | User | Chat | Message) -> Chat | None:
         match chat:
             case int(chat_id):
                 pass
             case str(chat_name):
-                chat_id = self.Chat.find_one({'platform': self.platform.value, 'name': chat_name}).id
+                if chat := self.Chat.find_one({'platform': self.platform.value, 'name': chat_name}):
+                    chat_id = chat.id
+                else:
+                    return
             case self.User() as user:
                 return await self._create_chat_from_discord_chat(await user.original_object.create_dm())
             case self.Chat():
                 return chat
             case self.Message() as message:
                 return message.chat
             case _:
                 raise TypeError('bad arguments')
 
-        # noinspection PyTypeChecker
-        return await self._create_chat_from_discord_chat(self.client.get_channel(chat_id) or await self.client.fetch_channel(chat_id))
+        try:
+            # noinspection PyTypeChecker
+            return await self._create_chat_from_discord_chat(self.client.get_channel(chat_id) or await self.client.fetch_channel(chat_id))
+        except discord.errors.NotFound:
+            pass
 
     @return_if_first_empty(exclude_self_types='DiscordBot', globals_=globals())
     async def get_current_roles(self, user: int | str | User | constants.DISCORD_USER, group_: int | str | Chat | Message = None) -> list[Role]:
         if isinstance(user, User) and not group_:
             original_user = user.original_object
         elif isinstance(user, int | str | User):
             original_user = (await self.get_user(user, group_)).original_object
@@ -454,45 +463,52 @@
         if group_ is None:
             return user
         else:
             return await self.get_user(user, group_)
 
     @return_if_first_empty(exclude_self_types='DiscordBot', globals_=globals())
     async def get_message(self, message: int | str | Message, chat: int | str | User | Chat | Message) -> Message | None:
+        if not (chat := await self.get_chat(chat)):
+            return
+
         match message:
             case int(message_id):
                 pass
             case str(message_id):
                 message_id = int(message_id)
             case self.Message():
                 return message
             case _:
                 raise TypeError('bad arguments')
 
-        chat = await self.get_chat(chat)
-        return await self._get_message(await chat.original_object.fetch_message(message_id))
+        try:
+            return await self._get_message(await chat.original_object.fetch_message(message_id))
+        except discord.errors.NotFound:
+            return
 
     @return_if_first_empty(exclude_self_types='DiscordBot', globals_=globals())
     async def get_group_roles(self, group_: int | str | Chat | Message) -> list[Role]:
         if not (discord_group := await self._get_discord_group(group_)):
             return []
 
         # noinspection PyTypeChecker
         return [Role(self.platform, discord_role.id, discord_group.id, discord_role.name, discord_role.permissions.administrator, discord_role) for discord_role in discord_group.roles]
 
     @return_if_first_empty(exclude_self_types='DiscordBot', globals_=globals())
     async def get_user(self, user: int | str | User, group_: int | str | Chat | Message = None) -> User | None:
         if not (user_id := self.get_user_id(user)):
             return
 
-        if group_ is None:
-            original_user = self.client.get_user(user_id) or await self.client.fetch_user(user_id)
-        else:
-            discord_group = await self._get_discord_group(group_)
-            original_user = discord_group.get_member(user_id)
+        try:
+            if group_ is None:
+                original_user = self.client.get_user(user_id) or await self.client.fetch_user(user_id)
+            elif not (discord_group := await self._get_discord_group(group_)) or not (original_user := discord_group.get_member(user_id)):
+                return
+        except discord.errors.NotFound:
+            return
 
         return await self._create_user_from_discord_user(original_user)
 
     @return_if_first_empty(exclude_self_types='DiscordBot', globals_=globals())
     async def get_users(self, group_: int | str | Chat | Message) -> list[User]:
         discord_group = await self._get_discord_group(group_)
         return [await self._create_user_from_discord_user(member) for member in discord_group.members]
@@ -579,15 +595,15 @@
         data: dict = None,
         silent: bool = False,
         send_as_file: bool = None,
         edit=False
     ) -> Message | None:
         async def file_too_large():
             if random.randint(0, 10):
-                error_message = 'El archivo pesa más de 8 MB.'
+                error_message = f'El archivo pesa más de {constants.DISCORD_MEDIA_MAX_BYTES // 1000000} MB.'
             else:
                 error_message = 'El archivo pesa mas que tu madre'
             await self._manage_exceptions(SendError(error_message), chat)
 
         text = self._parse_html_to_discord_markdown(text)
         if (
                 media
@@ -602,14 +618,16 @@
             file = None
         else:
             try:
                 file = await self._prepare_media_to_send(media)
             except LimitError:
                 await file_too_large()
                 return
+            if not text and not file:
+                return
 
         view = None
         if buttons:
             view = discord.ui.View(timeout=None)
             for i, row in enumerate(buttons):
                 for button in row:
                     discord_button = discord.ui.Button(label=button.text, row=i)
@@ -626,57 +644,30 @@
                 kwargs['view'] = view
 
             try:
                 message.original_object = await message.original_object.edit(**kwargs)
             except discord.errors.NotFound:
                 return
 
-            if media is not None:
-                message.medias = [media]
-            try:
-                if buttons is not None:
-                    self._message_cache[message.id, chat.id].buttons_info.buttons = buttons
-                if buttons_key is not None:
-                    self._message_cache[message.id, chat.id].buttons_info.key = buttons_key
-            except (AttributeError, KeyError):
-                message.buttons_info = ButtonsInfo(buttons=buttons, key=buttons_key)
-                self._message_cache[message.id, chat.id] = message
-            if data is not None:
-                message.data = data
-
-            message.update_last_edit()
-            message.save()
-
-            return message
+            return self._update_message_attributes(message, media, buttons, chat, buttons_key, data, update_last_edit=True)
 
         match reply_to:
             case int(message_id):
                 reply_to = await chat.original_object.fetch_message(message_id)
             case str(message_id):
                 reply_to = await chat.original_object.fetch_message(int(message_id))
             case self.Message() as message_to_reply:
                 reply_to = message_to_reply.original_object
 
         try:
-            bot_message = await self._get_message(await chat.original_object.send(text, file=file, view=view, reference=reply_to))
+            bot_message = await self._get_message(await chat.original_object.send(text, file=file, view=view, reference=reply_to, silent=silent))
         except discord.errors.HTTPException as e:
             if 'too large' in str(e).lower():
                 await file_too_large()
                 return
             raise
 
-        if buttons:
-            bot_message.buttons_info = ButtonsInfo(buttons=buttons, key=buttons_key)
-        if media:
-            bot_message.medias.append(media)
-        if data:
-            bot_message.data = data
-        if bot_message.buttons_info or bot_message.data:
-            self._message_cache[bot_message.id, chat.id] = bot_message
-
-        bot_message.save()
-
-        return bot_message
-
-    async def typing_delay(self, message: Message):
-        async with message.chat.original_object.typing():
-            await asyncio.sleep(random.randint(1, 3))
+        return self._update_message_attributes(bot_message, media, buttons, chat, buttons_key, data)
+
+    async def typing(self, chat: int | str | User | Chat | Message) -> contextlib.AbstractAsyncContextManager:
+        chat = await self.get_chat(chat)
+        return chat.original_object.typing()
```

### Comparing `multibot-1.9.0/multibot/bots/multi_bot.py` & `multibot-1.9.1/multibot/bots/multi_bot.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     'owner',
     'parse_arguments',
     'reply',
     'MultiBot'
 ]
 
 import asyncio
+import contextlib
 import datetime
 import functools
 import random
 import traceback
 from abc import ABC
 from collections import defaultdict
 from collections.abc import Callable, Coroutine, Iterable, Iterator, Sequence
@@ -27,15 +28,15 @@
 
 import flanautils
 import pymongo
 from flanautils import AmbiguityError, Media, NotFoundError, OrderedSet, ScoreMatch, return_if_first_empty, shift_args_if_called
 
 from multibot import constants
 from multibot.exceptions import BadRoleError, LimitError, SendError, UserDisconnectedError
-from multibot.models import Ban, Button, Chat, Message, Mute, Penalty, Platform, RegisteredCallback, Role, User
+from multibot.models import Ban, Button, ButtonsInfo, Chat, Message, Mute, Penalty, Platform, RegisteredCallback, Role, User
 
 
 # ---------------------------------------------------- #
 # -------------------- DECORATORS -------------------- #
 # ---------------------------------------------------- #
 @shift_args_if_called
 def find_message(func_: Callable = None, /, return_if_not_found=False) -> Callable:
@@ -301,14 +302,15 @@
     User = User
 
     def __init__(self, token: str, client: T):
         self.platform: Platform | None = None
         self.id: int | None = None
         self.name: str | None = None
         self.owner_id: int | None = None
+        self._owner_chat: Chat | None = None
         self.token: str = token
         self.client: T = client
         self._registered_callbacks: list[RegisteredCallback] = []
         self._registered_button_callbacks: dict[Any, list[Callable]] = defaultdict(list)
         # noinspection PyPep8Naming
         MessageType = self.Message
         self._message_cache: dict[tuple[int, int], MessageType] = {}
@@ -368,15 +370,15 @@
     async def _get_mentions(self, original_message: constants.ORIGINAL_MESSAGE) -> list[User]:
         pass
 
     @return_if_first_empty(exclude_self_types='MultiBot', globals_=globals())
     async def _get_message(
         self,
         event: constants.MESSAGE_EVENT,
-        pull_overwrite_fields: Iterable[str] = ('_id',)
+        pull_overwrite_fields: Iterable[str] = ('_id', 'date')
     ) -> Message:
         original_message = await self._get_original_message(event)
 
         message_id = await self._get_message_id(original_message)
         chat = await self._get_chat(original_message)
         try:
             cached_message = self._message_cache[message_id, chat.id]
@@ -481,15 +483,15 @@
                 always_callbacks.add(registered_callback)
             elif registered_callback.default:
                 default_callbacks.add(registered_callback)
             else:
                 mached_keywords_groups = 0
                 total_score = 0
                 for keywords_group in registered_callback.keywords:
-                    important_words |= {original_text_word for original_text_word in original_words if flanautils.cartesian_product_string_matching(original_text_word, keywords_group, min_score=registered_callback.min_score)}
+                    important_words |= {original_word for original_word in original_words if flanautils.cartesian_product_string_matching(original_word, keywords_group, min_score=registered_callback.min_score)}
                     word_matches = flanautils.cartesian_product_string_matching(important_words, keywords_group, min_score=registered_callback.min_score)
                     score = sum((max(matches.values()) + 1) ** score_reward_exponent for matches in word_matches.values())
                     try:
                         score /= max(1., keywords_lenght_penalty * len(keywords_group))
                     except ZeroDivisionError:
                         continue
                     if score:
@@ -543,15 +545,45 @@
         pass
 
     async def _unmute(self, user: int | str | User, group_: int | str | Chat | Message, message: Message = None):
         pass
 
     async def _unpenalize_later(self, penalty: Penalty, unpenalize_method: Callable, message: Message = None):
         if penalty.time and penalty.time <= constants.TIME_THRESHOLD_TO_MANUAL_UNPUNISH:
-            await flanautils.do_later(penalty.time, self._remove_penalty, penalty, unpenalize_method, message)
+            flanautils.do_later(penalty.time, self._remove_penalty, penalty, unpenalize_method, message)
+
+    def _update_message_attributes(
+        self,
+        message: Message,
+        media: Media = None,
+        buttons: list[str | tuple[str, bool] | Button | list[str | tuple[str, bool] | Button]] | None = None,
+        chat: int | str | User | Chat | Message | None = None,
+        buttons_key: Any = None,
+        data: dict = None,
+        update_last_edit=False
+    ):
+        if media is not None and (not media.bytes_ or len(media.bytes_) <= constants.PYMONGO_MEDIA_MAX_BYTES):
+            message.medias = [media]
+        try:
+            if buttons is not None:
+                self._message_cache[message.id, chat.id].buttons_info.buttons = buttons
+            if buttons_key is not None:
+                self._message_cache[message.id, chat.id].buttons_info.key = buttons_key
+        except (AttributeError, KeyError):
+            message.buttons_info = ButtonsInfo(buttons=buttons, key=buttons_key)
+        if data is not None:
+            message.data = data
+        if message.buttons_info or message.data is not None:
+            self._message_cache[message.id, chat.id] = message
+
+        if update_last_edit:
+            message.update_last_edit()
+        message.save()
+
+        return message
 
     # ---------------------------------------------- #
     #                    HANDLERS                    #
     # ---------------------------------------------- #
     @find_message
     async def _on_button_press_raw(self, message: Message):
         if not message.buttons_info:
@@ -576,18 +608,18 @@
                 except Exception as e:
                     await self._manage_exceptions(e, message, reraise=True)
 
     async def _on_ready(self):
         constants.load_environment()
         flanautils.init_database()
         print(f'{self.name} activado en {self.platform.name} (id: {self.id})')
-        await flanautils.do_every(constants.CHECK_OLD_CACHE_MESSAGES_EVERY_SECONDS, self.check_old_cache_messages)
-        await flanautils.do_every(constants.CHECK_OLD_DATABASE_MESSAGES_EVERY_SECONDS, self.check_old_database_messages)
-        await flanautils.do_every(constants.CHECK_PENALTIES_EVERY_SECONDS, self.check_bans)
-        await flanautils.do_every(constants.CHECK_PENALTIES_EVERY_SECONDS, self.check_mutes)
+        flanautils.do_every(constants.CHECK_OLD_CACHE_MESSAGES_EVERY_SECONDS, self.check_old_cache_messages)
+        flanautils.do_every(constants.CHECK_OLD_DATABASE_MESSAGES_EVERY_SECONDS, self.check_old_database_messages)
+        flanautils.do_every(constants.CHECK_PENALTIES_EVERY_SECONDS, self.check_bans)
+        flanautils.do_every(constants.CHECK_PENALTIES_EVERY_SECONDS, self.check_mutes)
 
     # -------------------------------------------------------- #
     # -------------------- PUBLIC METHODS -------------------- #
     # -------------------------------------------------------- #
     async def accept_button_event(self, event: constants.MESSAGE_EVENT | Message):
         pass
 
@@ -614,18 +646,17 @@
                 break
 
             keys_to_delete.append(k)
 
         for key in keys_to_delete:
             del self._message_cache[key]
 
-    @classmethod
-    def check_old_database_messages(cls):
+    def check_old_database_messages(self):
         before_date = datetime.datetime.now(datetime.timezone.utc) - constants.DATABASE_MESSAGE_EXPIRATION_TIME
-        cls.Message.delete_many_raw({'date': {'$lte': before_date}})
+        self.Message.delete_many_raw({'platform': self.platform.value, 'date': {'$lte': before_date}})
 
     @return_if_first_empty(exclude_self_types='MultiBot', globals_=globals())
     async def clear(self, n_messages: int, chat: int | str | Chat | Message):
         pass
 
     @return_if_first_empty(exclude_self_types='MultiBot', globals_=globals())
     async def delete_message(
@@ -683,35 +714,29 @@
     async def get_chat(self, chat: int | str | User | Chat | Message) -> Chat | None:
         pass
 
     @return_if_first_empty(exclude_self_types='MultiBot', globals_=globals())
     async def get_current_roles(self, user: int | str | User | constants.ORIGINAL_USER, group_: int | str | Chat | Message = None) -> list[Role]:
         return []
 
-    def get_formatted_last_database_messages(self, n_messages: int, name_limit=20, platform_limit=10, chat_limit=10, text_limit=30, timezone=None, simple=False) -> str:
-        counter = 0
-
+    def get_formatted_last_database_messages(self, n_messages: int, name_limit=10, platform_limit=10, chat_limit=10, text_limit=40, timezone=None, simple=False) -> str:
         if simple:
             title = f"       {'Usuario'[:name_limit]:<{name_limit}}  {'Texto'[:text_limit]:<{text_limit}}  {'Fecha':<12}"
 
             def generator_():
-                nonlocal counter
                 for i, message in enumerate(self.get_last_database_messages(n_messages, lazy=True), start=1):
-                    counter += 1
                     name = message.author.name.split('#')[0]
                     text = repr(message.text).replace('`', '').strip("'")
                     date = message.date.astimezone(timezone).strftime('%d  %H:%M')
                     yield f"{i:>4}.  {name[:name_limit]:<{name_limit}}  {text[:text_limit]:<{text_limit}}  {date}"
         else:
             title = f"       {'Usuario'[:name_limit]:<{name_limit}}  {'Plataforma'[:platform_limit]:<{platform_limit}}  {'Chat'[:chat_limit]:<{chat_limit}}  {'Texto'[:text_limit]:<{text_limit}}  {'Fecha':<20}"
 
             def generator_():
-                nonlocal counter
                 for i, message in enumerate(self.get_last_database_messages(n_messages, lazy=True), start=1):
-                    counter += 1
                     name = message.author.name.split('#')[0]
                     platform = Platform(message.platform).name
                     chat = message.chat.name
                     text = repr(message.text).replace('`', '').strip("'")
                     date = message.date.astimezone(timezone).strftime('%d/%m/%Y  %H:%M:%S')
                     yield f"{i:>4}.  {name[:name_limit]:<{name_limit}}  {platform[:platform_limit]:<{platform_limit}}  {chat[:chat_limit]:<{chat_limit}}  {text[:text_limit]:<{text_limit}}  {date}"
 
@@ -825,14 +850,20 @@
     async def mute(self, user: int | str | User, group_: int | str | Chat | Message, time: int | datetime.timedelta = None, message: Message = None):
         # noinspection PyTypeChecker
         mute = Mute(self.platform, self.get_user_id(user), self.get_group_id(group_), time)
         await self._mute(mute.user_id, mute.group_id, message)
         mute.save(pull_exclude_fields=('until',))
         await self._unpenalize_later(mute, self._unmute, message)
 
+    @property
+    async def owner_chat(self) -> Chat:
+        if not self._owner_chat:
+            self._owner_chat = await self.get_chat(self.owner_id) or await self.get_chat(await self.get_user(self.owner_id))
+        return self._owner_chat
+
     @overload
     def register(self, func_: Callable = None, keywords=(), priority: int | float = 1, min_score=constants.PARSER_MIN_SCORE_DEFAULT, always=False, default=False):
         pass
 
     @overload
     def register(self, keywords=(), priority: int | float = 1, min_score=constants.PARSER_MIN_SCORE_DEFAULT, always=False, default=False):
         pass
@@ -881,37 +912,39 @@
         edit=False
     ) -> Message | None:
         pass
 
     @parse_arguments
     async def send_error(self, *args, **kwargs) -> constants.ORIGINAL_MESSAGE:
         bot_message = await self.send(*args, **kwargs)
-        await flanautils.do_later(constants.ERROR_MESSAGE_DURATION, self.delete_message, bot_message)
+        flanautils.do_later(constants.ERROR_MESSAGE_DURATION, self.delete_message, bot_message)
         return bot_message
 
     @inline
     async def send_inline_results(self, message: Message):
         pass
 
-    async def send_interrogation(self, message: Message) -> constants.ORIGINAL_MESSAGE:
-        return await self.send(random.choice(constants.INTERROGATION_PHRASES), message)
-
-    async def send_negative(self, message: Message) -> constants.ORIGINAL_MESSAGE:
-        return await self.send(random.choice(constants.NO_PHRASES), message)
+    async def send_interrogation(self, chat: int | str | User | Chat | Message) -> constants.ORIGINAL_MESSAGE:
+        chat = await self.get_chat(chat)
+        return await self.send(random.choice(constants.INTERROGATION_PHRASES), chat)
+
+    async def send_negative(self, chat: int | str | User | Chat | Message) -> constants.ORIGINAL_MESSAGE:
+        chat = await self.get_chat(chat)
+        return await self.send(random.choice(constants.NO_PHRASES), chat)
 
     def start(self) -> Coroutine | None:
         self._add_handlers()
         try:
             asyncio.get_running_loop()
         except RuntimeError:
             self._start_sync()
         else:
             return self._start_async()
 
-    async def typing_delay(self, message: Message):
+    async def typing(self, chat: int | str | User | Chat | Message) -> contextlib.AbstractAsyncContextManager:
         pass
 
     async def unban(self, user: int | str | User, group_: int | str | Chat | Message, message: Message = None):
         # noinspection PyTypeChecker
         ban = Ban(self.platform, self.get_user_id(user), self.get_group_id(group_))
         await self._remove_penalty(ban, self._unban, message)
```

### Comparing `multibot-1.9.0/multibot/bots/telegram_bot.py` & `multibot-1.9.1/multibot/bots/telegram_bot.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,29 +3,31 @@
 __all__ = ['user_client', 'TelegramBot']
 
 import asyncio
 import contextlib
 import functools
 import io
 import pathlib
+import struct
 from collections.abc import Coroutine
 from typing import Any, Callable, Sequence
 
 import flanautils
 import pymongo
 import telethon
 import telethon.hints
-from flanautils import Media, MediaType, OrderedSet, Source, return_if_first_empty, shift_args_if_called
+import telethon.tl.types
+from flanautils import Media, MediaType, OrderedSet, ResponseError, Source, return_if_first_empty, shift_args_if_called
 from telethon import TelegramClient
 from telethon.sessions import StringSession
 
 from multibot import constants
 from multibot.bots.multi_bot import MultiBot, find_message, inline, parse_arguments
 from multibot.exceptions import LimitError
-from multibot.models import Button, ButtonsInfo, Chat, Message, Platform, User
+from multibot.models import Button, Chat, Message, Platform, User
 
 
 # ---------------------------------------------------- #
 # ----------------- CONTEXT MANAGERS ----------------- #
 # ---------------------------------------------------- #
 @contextlib.asynccontextmanager
 async def use_user_client(self: TelegramBot):
@@ -95,40 +97,14 @@
     async def _ban(self, user: int | str | User, group_: int | str | Chat | Message, message: Message = None):
         user = await self.get_user(user, group_)
         chat = await self.get_chat(group_)
 
         await self.client.edit_permissions(chat.original_object, user.original_object, view_messages=False)
 
     @return_if_first_empty(exclude_self_types='TelegramBot', globals_=globals())
-    async def _create_bot_message_from_telegram_bot_message(
-        self,
-        original_message: constants.TELEGRAM_MESSAGE,
-        media: Media,
-        chat: Chat,
-        buttons: list[list[Button]] = None,
-        buttons_key: Any = None,
-        data: dict = None
-    ) -> Message | None:
-        original_message._sender = await self.client.get_me()
-        original_message._chat = chat.original_object
-        bot_message = await self._get_message(original_message)
-        if buttons:
-            bot_message.buttons_info = ButtonsInfo(buttons=buttons, key=buttons_key)
-        if media and (not media.bytes_ or len(media.bytes_) <= constants.PYMONGO_MEDIA_MAX_BYTES):
-            bot_message.medias.append(media)
-        if data:
-            bot_message.data = data
-        if bot_message.buttons_info or bot_message.data:
-            self._message_cache[bot_message.id, chat.id] = bot_message
-
-        bot_message.save()
-
-        return bot_message
-
-    @return_if_first_empty(exclude_self_types='TelegramBot', globals_=globals())
     async def _create_chat_from_telegram_chat(self, original_chat: constants.TELEGRAM_CHAT) -> Chat | None:
         chat_name = self._get_entity_name(original_chat)
         if isinstance(original_chat, constants.TELEGRAM_USER):
             group_id = None
             group_name = None
         else:
             group_id = original_chat.id
@@ -198,18 +174,22 @@
         if replied_message := await self._get_replied_message(original_message):
             mentions.add(replied_message.author)
 
         text = await self._get_text(original_message)
         chat = await self._get_chat(original_message)
 
         for entity in original_message.entities or ():
+            if not isinstance(entity, telethon.tl.types.MessageEntityMention):
+                continue
+
             try:
                 mentions.add(await self.get_user(text[entity.offset:entity.offset + entity.length], chat.group_id))
             except ValueError:
                 if getattr(entity, 'user_id', None):
+                    # noinspection PyUnresolvedReferences
                     mentions.add(await self.get_user(entity.user_id, chat.group_id))
 
         text = flanautils.remove_symbols(text, replace_with=' ')
         words = text.lower().split()
 
         for participant in await self.client.get_participants(chat.original_object):
             user_name = self._get_entity_name(participant).lower()
@@ -255,18 +235,21 @@
             if not pathlib.Path(media.url).is_file() and media.source is Source.INSTAGRAM and (not (path_suffix := pathlib.Path(media.url).suffix) or len(path_suffix) > constants.MAX_FILE_EXTENSION_LENGHT):
                 return f'{media.url}.{media.extension}'
             else:
                 return media.url
 
         async def bytes_file() -> io.BytesIO | None:
             if not media.bytes_:
-                return
+                try:
+                    media.bytes_ = await flanautils.get_request(media.url)
+                except ResponseError:
+                    return
 
             bytes_ = media.bytes_
-            file_stem = f"{media.title or 'bot_media'}"
+            file_stem = media.title or 'bot_media'
             if media.title or is_inline:
                 try:
                     bytes_ = await flanautils.edit_metadata(bytes_, {'title': file_stem}, overwrite=False)
                 except FileNotFoundError:
                     pass
             file_ = io.BytesIO(bytes_)
             file_.name = f"{file_stem}{f'.{media.extension}' if media.extension else ''}"
@@ -322,32 +305,33 @@
 
     @user_client
     @return_if_first_empty(exclude_self_types='TelegramBot', globals_=globals())
     async def clear(self, n_messages: int, chat: int | str | Chat | Message):
         if n_messages > constants.DELETE_MESSAGE_LIMIT:
             raise LimitError('El máximo es 100.')
 
+        n_messages = int(n_messages)
         chat = await self.get_chat(chat)
 
         async with use_user_client(self):
             user_client_user = await self._create_user_from_telegram_user(await self.user_client.get_me(), chat.group_id)
             if await self.client.is_bot() and user_client_user not in await self.get_users(chat):
                 return
 
             if chat.is_group:
-                original_chat = chat.original_object
+                original_chat = await self.user_client.get_entity(chat.original_object)
             else:
                 original_chat = await self.user_client.get_input_entity(self.name)
 
             message_ids = [message.id async for message in self.user_client.iter_messages(original_chat, n_messages)]
             await self.user_client.delete_messages(original_chat, message_ids)
-            database_messages_to_delete_generator = self.Message.find({'platform': self.platform.value, 'chat': chat.object_id}, sort_keys=(('date', pymongo.DESCENDING),), limit=n_messages, lazy=True)
-            for database_message_to_delete in database_messages_to_delete_generator:
-                database_message_to_delete.is_deleted = True
-                database_message_to_delete.save()
+            deleted_messages_generator = self.Message.find({'platform': self.platform.value, 'chat': chat.object_id}, sort_keys=(('date', pymongo.DESCENDING),), limit=n_messages, lazy=True)
+            for deleted_message in deleted_messages_generator:
+                deleted_message.is_deleted = True
+                deleted_message.save()
 
     @return_if_first_empty(exclude_self_types='TelegramBot', globals_=globals())
     async def delete_message(
         self,
         message_to_delete: int | str | Message,
         chat: int | str | Chat | Message = None,
         raise_not_found=False
@@ -358,15 +342,15 @@
             chat = await self.get_chat(chat)
             chat.pull_from_database()
             if not isinstance(message_to_delete, Message):
                 message_to_delete = self.Message.find_one({'platform': self.platform.value, 'id': int(message_to_delete), 'chat': chat.object_id})
             await self.client.delete_messages(chat.original_object, message_to_delete.id)
 
         message_to_delete.is_deleted = True
-        message_to_delete.save()
+        message_to_delete.save(('is_deleted',))
 
     # noinspection PyTypeChecker
     def distribute_buttons(self, texts: Sequence[str], vertically=False) -> list[list[str]]:
         if vertically:
             return flanautils.chunks(texts, 1)
         else:
             return flanautils.chunks(texts, constants.TELEGRAM_BUTTONS_MAX_PER_LINE)
@@ -381,43 +365,58 @@
             case self.Chat():
                 return chat
             case self.Message() as message:
                 return message.chat
             case _ as chat_id_or_name:
                 pass
 
-        return await self._create_chat_from_telegram_chat(await self.client.get_entity(chat_id_or_name))
+        try:
+            return await self._create_chat_from_telegram_chat(await self.client.get_entity(chat_id_or_name))
+        except (ValueError, telethon.errors.rpcerrorlist.UsernameInvalidError):
+            pass
 
     async def get_me(self, group_: int | str | Chat = None):
         return await self._create_user_from_telegram_user(await self.client.get_me(), group_)
 
     @return_if_first_empty(exclude_self_types='TelegramBot', globals_=globals())
     async def get_message(self, message: int | str | Message, chat: int | str | User | Chat | Message) -> Message | None:
+        if not (chat := await self.get_chat(chat)):
+            return
+
         match message:
             case int(message_id):
                 pass
             case str(message_id):
                 pass
             case self.Message():
                 return message
             case _:
                 raise TypeError('bad arguments')
 
-        chat = await self.get_chat(chat)
-        return await self._get_message(await self.client.get_messages(chat.original_object, ids=message_id))
+        try:
+            with flanautils.suppress_low_level_stderr():
+                return await self._get_message(await self.client.get_messages(chat.original_object, ids=message_id))
+        except (TypeError, struct.error):
+            pass
 
     @return_if_first_empty(exclude_self_types='TelegramBot', globals_=globals())
     async def get_user(self, user: int | str | User, group_: int | str | Chat | Message = None) -> User | None:
         match user:
             case self.User() if user.original_object:
                 original_user = user.original_object
-            case self.User():
-                original_user = await self.client.get_entity(user.id)
             case _:
-                original_user = await self.client.get_entity(user)
+                match user:
+                    case self.User():
+                        user_id_or_name = user.id
+                    case user_id_or_name:
+                        pass
+                try:
+                    original_user = await self.client.get_entity(user_id_or_name)
+                except (ValueError, telethon.errors.rpcerrorlist.UsernameInvalidError):
+                    return
 
         return await self._create_user_from_telegram_user(original_user, group_)
 
     @return_if_first_empty(exclude_self_types='TelegramBot', globals_=globals())
     async def get_users(self, group_: int | str | Chat | Message) -> list[User]:
         chat = await self.get_chat(group_)
         return [await self._create_user_from_telegram_user(participant, chat.id) for participant in await self.client.get_participants(chat.original_object)]
@@ -461,15 +460,16 @@
                 telegram_buttons_row = []
                 for button in row:
                     telegram_buttons_row.append(telethon.Button.inline(button.text))
                 telegram_buttons.append(telegram_buttons_row)
 
         kwargs = {
             'file': file,
-            'parse_mode': 'html'
+            'parse_mode': 'html',
+            'supports_streaming': True
         }
 
         if message:
             if send_as_file is None:
                 word_matches = flanautils.cartesian_product_string_matching(message.text, constants.KEYWORDS['send_as_file'], min_score=constants.TELEGRAM_SEND_AS_FILE_MIN_SCORE)
                 send_as_file_score = sum(max(matches.values()) for text_word, matches in word_matches.items())
                 kwargs['force_document'] = bool(send_as_file_score)
@@ -492,58 +492,63 @@
                         telethon.errors.rpcerrorlist.PeerIdInvalidError,
                         telethon.errors.rpcerrorlist.MessageIdInvalidError,
                         telethon.errors.rpcerrorlist.MessageNotModifiedError,
                         telethon.errors.rpcerrorlist.UserIsBlockedError
                 ):
                     return
 
-                if media is not None:
-                    message.medias = [media]
-                try:
-                    if buttons is not None:
-                        self._message_cache[message.id, chat.id].buttons_info.buttons = buttons
-                    if buttons_key is not None:
-                        self._message_cache[message.id, chat.id].buttons_info.key = buttons_key
-                except (AttributeError, KeyError):
-                    message.buttons_info = ButtonsInfo(buttons=buttons, key=buttons_key)
-                    self._message_cache[message.id, chat.id] = message
-                if data is not None:
-                    message.data = data
-                message.update_last_edit()
-                message.save()
-                return message
+                return self._update_message_attributes(message, media, buttons, chat, buttons_key, data, update_last_edit=True)
 
         match reply_to:
             case str():
                 reply_to = int(reply_to)
             case self.Message() as message_to_reply:
                 reply_to = message_to_reply.original_object
 
         with flanautils.suppress_stderr():
-            parse_retries = 1
-            while True:
+            attempts = 2
+            for attempt in range(attempts - 1, -1, -1):
                 try:
                     original_message = await self.client.send_message(chat.original_object, text, buttons=telegram_buttons, reply_to=reply_to, silent=silent, **kwargs)
-                except telethon.errors.rpcerrorlist.WebpageCurlFailedError:
-                    if media.bytes_:
-                        kwargs['file'] = await self._prepare_media_to_send(media, prefer_bytes=True)
+                except telethon.errors.VideoContentTypeInvalidError:
+                    if attempt:
+                        try:
+                            del kwargs['supports_streaming']
+                        except KeyError:
+                            pass
+                    else:
+                        raise
+                except telethon.errors.WebpageCurlFailedError:
+                    if bytes_ := await self._prepare_media_to_send(media, prefer_bytes=True):
+                        kwargs['file'] = bytes_
                     else:
                         raise
                 except ValueError as e:
-                    if 'parse' in str(e).lower() and parse_retries:
-                        del kwargs['parse_mode']
-                        parse_retries -= 1
+                    if 'parse' in str(e).lower() and attempt:
+                        try:
+                            del kwargs['parse_mode']
+                        except KeyError:
+                            pass
                     else:
                         raise
-                except (telethon.errors.rpcerrorlist.MediaEmptyError, telethon.errors.rpcerrorlist.PeerIdInvalidError, telethon.errors.rpcerrorlist.UserIsBlockedError):
+                except telethon.errors.rpcerrorlist.MediaEmptyError:
+                    if (bytes_ := await self._prepare_media_to_send(media, prefer_bytes=True)) and isinstance(bytes_, bytes):
+                        kwargs['file'] = bytes_
+                    else:
+                        return
+                except (telethon.errors.rpcerrorlist.PeerIdInvalidError, telethon.errors.rpcerrorlist.UserIsBlockedError):
                     return
                 else:
                     break
 
-        return await self._create_bot_message_from_telegram_bot_message(original_message, media, chat, buttons, buttons_key, data)
+        original_message._sender = await self.client.get_me()
+        original_message._chat = chat.original_object
+        bot_message = await self._get_message(original_message)
+
+        return self._update_message_attributes(bot_message, media, buttons, chat, buttons_key, data)
 
     @inline
     async def send_inline_results(self, message: Message):
         async def create_result(media: Media, prefer_bytes=False) -> telethon.types.InputBotInlineResultPhoto | telethon.types.InputBotInlineResultDocument:
             file = await self._prepare_media_to_send(media, prefer_bytes, is_inline=True)
             match media.type_:
                 case MediaType.IMAGE:
@@ -592,7 +597,11 @@
 
         try:
             asyncio.get_running_loop()
         except RuntimeError:
             return asyncio.run(string_session_())
         else:
             return string_session_()
+
+    async def typing(self, chat: int | str | User | Chat | Message) -> contextlib.AbstractAsyncContextManager:
+        chat = await self.get_chat(chat)
+        return self.client.action(chat.original_object, 'typing')
```

### Comparing `multibot-1.9.0/multibot/bots/twitch_bot.py` & `multibot-1.9.1/multibot/bots/twitch_bot.py`

 * *Files 1% similar despite different names*

```diff
@@ -139,14 +139,15 @@
         await super()._on_ready()
 
     # -------------------------------------------------------- #
     # -------------------- PUBLIC METHODS -------------------- #
     # -------------------------------------------------------- #
     @return_if_first_empty(exclude_self_types='TwitchBot', globals_=globals())
     async def clear(self, n_messages: int, chat: int | str | Chat | Message):
+        n_messages = int(n_messages)
         chat = await self.get_chat(chat)
 
         messages_to_delete: Iterator[Message] = self.Message.find(
             {
                 'platform': self.platform.value,
                 'chat': chat.object_id,
                 'is_deleted': False
@@ -173,15 +174,15 @@
             chat = await self.get_chat(chat)
             chat.pull_from_database()
             if not isinstance(message_to_delete, Message):
                 message_to_delete = self.Message.find_one({'platform': self.platform.value, 'id': int(message_to_delete), 'chat': chat.object_id})
 
         await self.send(f'/delete {message_to_delete.id}', chat)
         message_to_delete.is_deleted = True
-        message_to_delete.save()
+        message_to_delete.save(('is_deleted',))
 
     @return_if_first_empty(exclude_self_types='TwitchBot', globals_=globals())
     async def get_chat(self, chat: int | str | User | Chat | Message = None) -> Chat | None:
         match chat:
             case int(group_id):
                 group_name = self.get_group_name(group_id)
                 if not group_name:
```

### Comparing `multibot-1.9.0/multibot/constants.py` & `multibot-1.9.1/multibot/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 CHECK_PENALTIES_EVERY_SECONDS = datetime.timedelta(hours=1).total_seconds()
 COMMAND_MESSAGE_DURATION = 5
 DATABASE_MESSAGE_EXPIRATION_TIME = datetime.timedelta(weeks=flanautils.WEEKS_IN_A_MONTH)
 DELETE_MESSAGE_LIMIT = 100
 DISCORD_BUTTON_MAX_CHARACTERS = 80
 DISCORD_BUTTONS_MAX = 5
 DISCORD_COMMAND_PREFIX = flanautils.random_string()
-DISCORD_MEDIA_MAX_BYTES = 8000000
+DISCORD_MEDIA_MAX_BYTES = 25000000
 ERROR_MESSAGE_DURATION = 10
 MAX_FILE_EXTENSION_LENGHT = 5
 PARSER_KEYWORDS_LENGHT_PENALTY = 0.001
 PARSER_MAX_WORD_LENGTH = 25
 PARSER_MIN_SCORE_DEFAULT = 0.93
 PARSER_MIN_SCORE_TO_MATCH = 3
 PARSER_SCORE_REWARD_EXPONENT = 2
@@ -76,44 +76,44 @@
 
 GIF_DOMAINS = ('Gfycat', 'Gifbin', 'Giphy', 'Imgur', 'ReactionGifs', 'Tenor')
 
 INTERROGATION_PHRASES = ('?', 'que?', 'que dise', 'no entiendo', 'no entender', 'mi no entender', 'ein?', '🤔', '🤨',
                          '🧐', '🙄', '🙃')
 
 KEYWORDS = {
-    'activate': ('activa', 'activar', 'activate', 'add', 'añade', 'añadir', 'dale', 'deja', 'dejale', 'devuelve',
-                 'devuelvele', 'enable', 'encender', 'enciende', 'habilita', 'habilitar', 'permite'),
-    'all': ('all', 'toda', 'todas', 'todo', 'todos'),
+    'activate': ('abre', 'activa', 'activar', 'activate', 'add', 'añade', 'añadir', 'dale', 'deja', 'dejale',
+                 'devuelve', 'devuelvele', 'enable', 'encender', 'enciende', 'habilita', 'habilitar', 'open',
+                 'permite', 'return'),
+    'all': ('all', 'complete', 'completo', 'entero', 'full', 'toda', 'todas', 'todo', 'todos'),
     'audio': ('audio', 'music', 'musica', 'sonido', 'sound'),
     'audit': ('audit', 'auditoria', 'desconectado', 'disconnect', 'log', 'move', 'mover', 'movido', 'registro'),
     'ban': ('ban', 'banea', 'banealo'),
     'bye': ('adieu', 'adio', 'adiooooo', 'adios', 'agur', 'buenas', 'bye', 'cama', 'chao', 'farewell', 'goodbye',
             'hasta', 'luego', 'noches', 'pronto', 'taluego', 'taluegorl', 'tenga', 'vemos', 'vista', 'voy'),
     'change': ('alter', 'alternar', 'alternate', 'cambiar', 'change', 'default', 'defecto', 'edit', 'editar',
                'exchange', 'modificar', 'modify', 'permutar', 'predeterminado', 'shift', 'swap', 'switch', 'turn',
                'vary'),
     'config': ('ajustar', 'ajuste', 'ajustes', 'automatico', 'automatic', 'config', 'configs', 'configuracion',
                'configuration', 'default', 'defecto', 'setting', 'settings'),
     'date': ('ayer', 'de', 'domingo', 'fin', 'finde', 'friday', 'hoy', 'jueves', 'lunes', 'martes', 'mañana',
              'miercoles', 'monday', 'pasado', 'sabado', 'saturday', 'semana', 'sunday', 'thursday', 'today', 'tomorrow',
              'tuesday', 'viernes', 'wednesday', 'week', 'weekend', 'yesterday'),
-    'deactivate': ('apaga', 'apagar', 'cancel', 'cancela', 'deactivate', 'deactivate', 'desactivar', 'deshabilita',
-                   'deshabilitar', 'disable', 'forbids', 'prohibe', 'quita', 'remove', 'return'),
+    'deactivate': ('apaga', 'apagar', 'cancel', 'cancela', 'cierra', 'close', 'deactivate', 'deactivate', 'desactivar',
+                   'deshabilita', 'deshabilitar', 'disable', 'forbids', 'prohibe', 'quita', 'remove'),
     'delete': ('borra', 'borrado', 'borres', 'clear', 'delete', 'elimina', 'limpia', 'remove'),
     'hello': ('alo', 'aloh', 'buenas', 'dias', 'hello', 'hey', 'hi', 'hola', 'holaaaaaa', 'ola', 'saludos', 'tardes'),
     'help': ('ayuda', 'help'),
-    'last': ('last', 'ultima', 'ultimo'),
+    'last': ('last', 'ultima', 'ultimas', 'ultimo', 'ultimos'),
     'message': ('comentario', 'comment', 'mensaje', 'mensajes', 'message', 'messages', 'original'),
-    'mute': ('calla', 'calle', 'cierra', 'close', 'mute', 'mutea', 'mutealo', 'noise', 'ruido', 'shut', 'silence',
-             'silencia'),
+    'mute': ('calla', 'calle', 'mute', 'mutea', 'mutealo', 'noise', 'ruido', 'shut', 'silence', 'silencia'),
     'negate': ('no', 'ocurra', 'ocurre'),
     'permission': ('permiso', 'permission'),
     'reset': ('recover', 'recovery', 'recupera', 'reinicia', 'reset', 'resetea', 'restart'),
     'role': ('rol', 'role', 'roles'),
-    'send_as_file': ('arhivo', 'calidad', 'compress', 'compression', 'comprimir', 'file', 'quality'),
+    'send_as_file': ('arhivo', 'calidad', 'compresion', 'compress', 'compression', 'comprimir', 'file', 'quality'),
     'show': ('actual', 'enseña', 'estado', 'how', 'muestra', 'show', 'como'),
     'simple': ('sencillo', 'simple'),
     'sound': ('hablar', 'hable', 'micro', 'microfono', 'microphone', 'sonido', 'sound', 'talk', 'volumen'),
     'stop': ('acabar', 'caducar', 'detener', 'end', 'expirar', 'expire', 'finalizar', 'finish', 'parar', 'stop',
              'suspend', 'suspender', 'terminar', 'terminate'),
     'thanks': ('gracia', 'gracias', 'grasia', 'grasias', 'grax', 'thank', 'thanks', 'ty'),
     'unban': ('desbanea', 'unban'),
```

### Comparing `multibot-1.9.0/multibot/models/buttons.py` & `multibot-1.9.1/multibot/models/buttons.py`

 * *Files 8% similar despite different names*

```diff
@@ -43,8 +43,8 @@
         return [button for row in self.buttons for button in row if button.is_checked]
 
     def find_button(self, text: str) -> Button:
         return self[text]
 
     @property
     def pressed_button(self) -> Button | None:
-        return self[self.pressed_text]
+        return self.find_button(self.pressed_text)
```

### Comparing `multibot-1.9.0/multibot/models/chat.py` & `multibot-1.9.1/multibot/models/chat.py`

 * *Files identical despite different names*

### Comparing `multibot-1.9.0/multibot/models/event_component.py` & `multibot-1.9.1/multibot/models/event_component.py`

 * *Files identical despite different names*

### Comparing `multibot-1.9.0/multibot/models/message.py` & `multibot-1.9.1/multibot/models/message.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,11 +36,11 @@
     is_deleted: bool = False
     chat: Chat = None
     replied_message: Message = None
     original_object: constants.ORIGINAL_MESSAGE = None
     original_event: constants.MESSAGE_EVENT = None
 
     def _mongo_repr(self) -> Any:
-        return {k: v.to_dict() if isinstance(v, Media) else v for k, v in super()._mongo_repr().items() if k not in ('buttons_info', 'data')}
+        return {k: v for k, v in super()._mongo_repr().items() if k not in ('buttons_info', 'data')}
 
     def update_last_edit(self):
         self.last_edit = datetime.datetime.now(datetime.timezone.utc)
```

### Comparing `multibot-1.9.0/multibot/models/penalties.py` & `multibot-1.9.1/multibot/models/penalties.py`

 * *Files identical despite different names*

### Comparing `multibot-1.9.0/multibot/models/registered_callback.py` & `multibot-1.9.1/multibot/models/registered_callback.py`

 * *Files 26% similar despite different names*

```diff
@@ -23,34 +23,35 @@
         priority: int | float = 1,
         min_score: float = constants.PARSER_MIN_SCORE_DEFAULT,
         always=False,
         default=False
     ):
         self.callback = callback
 
-        match keywords:
-            case str(text):
-                text = flanautils.remove_accents(text.strip().lower())
-                self.keywords = (tuple(text.split()),)
-            case [*_, [*_]]:
-                def generator():
-                    for element in keywords:
-                        if isinstance(element, str):
-                            text_ = flanautils.remove_accents(element.strip().lower())
-                            keywords_group = tuple(text_.split())
-                        else:
-                            keywords_group = tuple(flanautils.remove_accents(keyword.strip().lower()) for keyword in element)
-                        yield keywords_group
+        if not keywords:
+            keywords = ()
+        elif isinstance(keywords, str):
+            text = flanautils.remove_accents(keywords.strip().lower())
+            self.keywords = (tuple(text.split()),)
+        elif isinstance(keywords, Iterable) and any(not isinstance(keyword, str) and isinstance(keyword, Iterable) for keyword in keywords):
+            def generator():
+                for element in keywords:
+                    if isinstance(element, str):
+                        text_ = flanautils.remove_accents(element.strip().lower())
+                        keywords_group = tuple(text_.split())
+                    else:
+                        keywords_group = tuple(flanautils.remove_accents(keyword.strip().lower()) for keyword in element)
+                    yield keywords_group
 
-                self.keywords = tuple(generator())
-            case [*_, str()]:
-                keywords = (flanautils.remove_accents(keyword.strip().lower()).split() for keyword in keywords)
-                self.keywords = (tuple(flanautils.flatten_iterator(keywords)),)
-            case _:
-                self.keywords = tuple(keywords)
+            self.keywords = tuple(generator())
+        elif isinstance(keywords, Iterable) and any(isinstance(keyword, str) for keyword in keywords):
+            keywords = (flanautils.remove_accents(keyword.strip().lower()).split() for keyword in keywords)
+            self.keywords = (tuple(flanautils.flatten(keywords, lazy=True)),)
+        else:
+            raise TypeError('bad arguments')
 
         self.priority = priority
         self.min_score = min_score
         self.always = always
         self.default = default
 
     def __call__(self, *args, **kwargs):
```

### Comparing `multibot-1.9.0/multibot/models/user.py` & `multibot-1.9.1/multibot/models/user.py`

 * *Files identical despite different names*

### Comparing `multibot-1.9.0/multibot.egg-info/PKG-INFO` & `multibot-1.9.1/multibot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 Metadata-Version: 2.1
 Name: multibot
-Version: 1.9.0
+Version: 1.9.1
 Summary: Platform agnostic high-level bot infrastructure. Develop one bot and you will have three: one for Discord, another one for Telegram and another one for Twitch. All bots use the same objects and logic.  For now there are adapters for three platforms but more may be added in the future.
 Home-page: https://github.com/AlberLC/multibot
 Author: AlberLC
-Author-email: alberlc@outlook.com
 Project-URL: Bug Tracker, https://github.com/AlberLC/multibot/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 License-File: LICENSE
```

### Comparing `multibot-1.9.0/multibot.egg-info/SOURCES.txt` & `multibot-1.9.1/multibot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `multibot-1.9.0/setup.cfg` & `multibot-1.9.1/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 [metadata]
 name = multibot
-version = v1.9.0
+version = v1.9.1
 author = AlberLC
-author_email = alberlc@outlook.com
 description = Platform agnostic high-level bot infrastructure. Develop one bot and you will have three: one for Discord, another one for Telegram and another one for Twitch. All bots use the same objects and logic.  For now there are adapters for three platforms but more may be added in the future.
 long_description = file: README.rst
 url = https://github.com/AlberLC/multibot
 project_urls = 
 	Bug Tracker = https://github.com/AlberLC/multibot/issues
 classifiers = 
 	Programming Language :: Python :: 3.10
```

