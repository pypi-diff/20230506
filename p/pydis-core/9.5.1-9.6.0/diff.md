# Comparing `tmp/pydis_core-9.5.1.tar.gz` & `tmp/pydis_core-9.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydis_core-9.5.1.tar", max compression
+gzip compressed data, was "pydis_core-9.6.0.tar", max compression
```

## Comparing `pydis_core-9.5.1.tar` & `pydis_core-9.6.0.tar`

### file list

```diff
@@ -1,23 +1,22 @@
--rw-r--r--   0        0        0     1071 2022-03-31 15:49:16.729733 pydis_core-9.5.1/LICENSE
--rw-r--r--   0        0        0      331 2023-02-09 21:50:49.567310 pydis_core-9.5.1/pydis_core/__init__.py
--rw-r--r--   0        0        0    11308 2023-03-02 22:58:06.664515 pydis_core-9.5.1/pydis_core/_bot.py
--rw-r--r--   0        0        0     1917 2023-02-09 21:50:49.567310 pydis_core-9.5.1/pydis_core/async_stats.py
--rw-r--r--   0        0        0      104 2022-11-05 14:18:24.787185 pydis_core-9.5.1/pydis_core/exts/__init__.py
--rw-r--r--   0        0        0     6349 2023-02-09 21:50:49.609519 pydis_core-9.5.1/pydis_core/site_api.py
--rw-r--r--   0        0        0     1314 2023-02-09 21:50:49.609519 pydis_core-9.5.1/pydis_core/utils/__init__.py
--rw-r--r--   0        0        0     1680 2022-11-05 14:18:24.788185 pydis_core-9.5.1/pydis_core/utils/_extensions.py
--rw-r--r--   0        0        0     2740 2022-11-05 14:18:24.789186 pydis_core-9.5.1/pydis_core/utils/_monkey_patches.py
--rw-r--r--   0        0        0     1810 2022-11-05 14:18:24.789186 pydis_core-9.5.1/pydis_core/utils/caching.py
--rw-r--r--   0        0        0     1705 2023-02-09 21:50:49.610663 pydis_core-9.5.1/pydis_core/utils/channel.py
--rw-r--r--   0        0        0     1521 2022-11-05 14:18:24.790186 pydis_core-9.5.1/pydis_core/utils/commands.py
--rw-r--r--   0        0        0     7725 2023-02-09 21:50:49.667635 pydis_core-9.5.1/pydis_core/utils/cooldown.py
--rw-r--r--   0        0        0     4267 2022-11-11 15:00:18.292347 pydis_core-9.5.1/pydis_core/utils/function.py
--rw-r--r--   0        0        0     4468 2023-02-09 21:50:49.674633 pydis_core-9.5.1/pydis_core/utils/interactions.py
--rw-r--r--   0        0        0     1432 2022-11-06 00:01:44.084076 pydis_core-9.5.1/pydis_core/utils/logging.py
--rw-r--r--   0        0        0     1995 2023-02-09 21:50:49.689686 pydis_core-9.5.1/pydis_core/utils/members.py
--rw-r--r--   0        0        0     2397 2022-11-05 14:18:24.793186 pydis_core-9.5.1/pydis_core/utils/regex.py
--rw-r--r--   0        0        0    10227 2023-02-09 21:50:49.689686 pydis_core-9.5.1/pydis_core/utils/scheduling.py
--rw-r--r--   0        0        0     2196 2023-03-02 22:58:06.665516 pydis_core-9.5.1/pyproject.toml
--rw-r--r--   0        0        0      120 2022-05-31 19:45:29.494670 pydis_core-9.5.1/README.md
--rw-r--r--   0        0        0     1036 1970-01-01 00:00:00.000000 pydis_core-9.5.1/setup.py
--rw-r--r--   0        0        0     1246 1970-01-01 00:00:00.000000 pydis_core-9.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2022-03-31 15:49:16.729733 pydis_core-9.6.0/LICENSE
+-rw-r--r--   0        0        0      331 2023-02-09 21:50:49.567310 pydis_core-9.6.0/pydis_core/__init__.py
+-rw-r--r--   0        0        0    11450 2023-05-06 12:14:38.832461 pydis_core-9.6.0/pydis_core/_bot.py
+-rw-r--r--   0        0        0     1917 2023-02-09 21:50:49.567310 pydis_core-9.6.0/pydis_core/async_stats.py
+-rw-r--r--   0        0        0      104 2022-11-05 14:18:24.787185 pydis_core-9.6.0/pydis_core/exts/__init__.py
+-rw-r--r--   0        0        0     6349 2023-02-09 21:50:49.609519 pydis_core-9.6.0/pydis_core/site_api.py
+-rw-r--r--   0        0        0     1314 2023-02-09 21:50:49.609519 pydis_core-9.6.0/pydis_core/utils/__init__.py
+-rw-r--r--   0        0        0     1680 2022-11-05 14:18:24.788185 pydis_core-9.6.0/pydis_core/utils/_extensions.py
+-rw-r--r--   0        0        0     2740 2022-11-05 14:18:24.789186 pydis_core-9.6.0/pydis_core/utils/_monkey_patches.py
+-rw-r--r--   0        0        0     1810 2022-11-05 14:18:24.789186 pydis_core-9.6.0/pydis_core/utils/caching.py
+-rw-r--r--   0        0        0     1705 2023-02-09 21:50:49.610663 pydis_core-9.6.0/pydis_core/utils/channel.py
+-rw-r--r--   0        0        0     1521 2022-11-05 14:18:24.790186 pydis_core-9.6.0/pydis_core/utils/commands.py
+-rw-r--r--   0        0        0     7725 2023-02-09 21:50:49.667635 pydis_core-9.6.0/pydis_core/utils/cooldown.py
+-rw-r--r--   0        0        0     4267 2022-11-11 15:00:18.292347 pydis_core-9.6.0/pydis_core/utils/function.py
+-rw-r--r--   0        0        0     4468 2023-02-09 21:50:49.674633 pydis_core-9.6.0/pydis_core/utils/interactions.py
+-rw-r--r--   0        0        0     1432 2022-11-06 00:01:44.084076 pydis_core-9.6.0/pydis_core/utils/logging.py
+-rw-r--r--   0        0        0     1995 2023-02-09 21:50:49.689686 pydis_core-9.6.0/pydis_core/utils/members.py
+-rw-r--r--   0        0        0     2397 2022-11-05 14:18:24.793186 pydis_core-9.6.0/pydis_core/utils/regex.py
+-rw-r--r--   0        0        0    10227 2023-02-09 21:50:49.689686 pydis_core-9.6.0/pydis_core/utils/scheduling.py
+-rw-r--r--   0        0        0     2196 2023-05-06 12:14:38.832461 pydis_core-9.6.0/pyproject.toml
+-rw-r--r--   0        0        0      120 2022-05-31 19:45:29.494670 pydis_core-9.6.0/README.md
+-rw-r--r--   0        0        0     1246 1970-01-01 00:00:00.000000 pydis_core-9.6.0/PKG-INFO
```

### Comparing `pydis_core-9.5.1/LICENSE` & `pydis_core-9.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydis_core-9.5.1/pydis_core/_bot.py` & `pydis_core-9.6.0/pydis_core/_bot.py`

 * *Files 3% similar despite different names*

```diff
@@ -115,15 +115,18 @@
                 statsd_url,
                 retry_after * 2,
                 attempt + 1
             )
 
     async def _load_extensions(self, module: types.ModuleType) -> None:
         """Load all the extensions within the given module and save them to ``self.all_extensions``."""
+        log.info("Waiting for guild %d to be avialable before loading extensions.", self.guild_id)
+
         await self.wait_until_guild_available()
+        log.info("Loading extensions...")
         self.all_extensions = walk_extensions(module)
 
         for extension in self.all_extensions:
             scheduling.create_task(self.load_extension(extension))
 
     async def _sync_app_commands(self) -> None:
         """Sync global & guild specific application commands after extensions are loaded."""
```

### Comparing `pydis_core-9.5.1/pydis_core/async_stats.py` & `pydis_core-9.6.0/pydis_core/async_stats.py`

 * *Files identical despite different names*

### Comparing `pydis_core-9.5.1/pydis_core/site_api.py` & `pydis_core-9.6.0/pydis_core/site_api.py`

 * *Files identical despite different names*

### Comparing `pydis_core-9.5.1/pydis_core/utils/__init__.py` & `pydis_core-9.6.0/pydis_core/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pydis_core-9.5.1/pydis_core/utils/_extensions.py` & `pydis_core-9.6.0/pydis_core/utils/_extensions.py`

 * *Files identical despite different names*

### Comparing `pydis_core-9.5.1/pydis_core/utils/_monkey_patches.py` & `pydis_core-9.6.0/pydis_core/utils/_monkey_patches.py`

 * *Files identical despite different names*

### Comparing `pydis_core-9.5.1/pydis_core/utils/caching.py` & `pydis_core-9.6.0/pydis_core/utils/caching.py`

 * *Files identical despite different names*

### Comparing `pydis_core-9.5.1/pydis_core/utils/channel.py` & `pydis_core-9.6.0/pydis_core/utils/channel.py`

 * *Files identical despite different names*

### Comparing `pydis_core-9.5.1/pydis_core/utils/commands.py` & `pydis_core-9.6.0/pydis_core/utils/commands.py`

 * *Files identical despite different names*

### Comparing `pydis_core-9.5.1/pydis_core/utils/cooldown.py` & `pydis_core-9.6.0/pydis_core/utils/cooldown.py`

 * *Files identical despite different names*

### Comparing `pydis_core-9.5.1/pydis_core/utils/function.py` & `pydis_core-9.6.0/pydis_core/utils/function.py`

 * *Files identical despite different names*

### Comparing `pydis_core-9.5.1/pydis_core/utils/interactions.py` & `pydis_core-9.6.0/pydis_core/utils/interactions.py`

 * *Files identical despite different names*

### Comparing `pydis_core-9.5.1/pydis_core/utils/logging.py` & `pydis_core-9.6.0/pydis_core/utils/logging.py`

 * *Files identical despite different names*

### Comparing `pydis_core-9.5.1/pydis_core/utils/members.py` & `pydis_core-9.6.0/pydis_core/utils/members.py`

 * *Files identical despite different names*

### Comparing `pydis_core-9.5.1/pydis_core/utils/regex.py` & `pydis_core-9.6.0/pydis_core/utils/regex.py`

 * *Files identical despite different names*

### Comparing `pydis_core-9.5.1/pydis_core/utils/scheduling.py` & `pydis_core-9.6.0/pydis_core/utils/scheduling.py`

 * *Files identical despite different names*

### Comparing `pydis_core-9.5.1/pyproject.toml` & `pydis_core-9.6.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydis_core"
-version = "9.5.1"
+version = "9.6.0"
 description = "PyDis core provides core functionality and utility to the bots of the Python Discord community."
 authors = ["Python Discord <info@pythondiscord.com>"]
 license = "MIT"
 classifiers=[
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
@@ -21,15 +21,15 @@
 documentation = "https://bot-core.pythondiscord.com/"
 repository = "https://github.com/python-discord/bot-core"
 keywords = ["bot", "discord", "discord.py"]
 
 [tool.poetry.dependencies]
 python = "3.10.* || 3.11.*"
 
-"discord.py" = "2.2.2"
+"discord.py" = "2.2.3"
 async-rediscache = { version = "1.0.0rc2", extras = ["fakeredis"], optional = true }
 statsd  = "4.0.1"
 aiodns = "3.0.0"
 
 [tool.poetry.extras]
 async-rediscache = ["async-rediscache"]
```

### Comparing `pydis_core-9.5.1/PKG-INFO` & `pydis_core-9.6.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydis-core
-Version: 9.5.1
+Version: 9.6.0
 Summary: PyDis core provides core functionality and utility to the bots of the Python Discord community.
 Home-page: https://pythondiscord.com/
 License: MIT
 Keywords: bot,discord,discord.py
 Author: Python Discord
 Author-email: info@pythondiscord.com
 Requires-Python: >=3.10.0,<3.12.0
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Provides-Extra: async-rediscache
 Requires-Dist: aiodns (==3.0.0)
 Requires-Dist: async-rediscache[fakeredis] (==1.0.0rc2) ; extra == "async-rediscache"
-Requires-Dist: discord.py (==2.2.2)
+Requires-Dist: discord.py (==2.2.3)
 Requires-Dist: statsd (==4.0.1)
 Project-URL: Documentation, https://bot-core.pythondiscord.com/
 Project-URL: Repository, https://github.com/python-discord/bot-core
 Description-Content-Type: text/markdown
 
 # bot-core ![Version]
```

