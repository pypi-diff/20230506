# Comparing `tmp/chatgpt_bot-0.1.3.tar.gz` & `tmp/chatgpt_bot-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatgpt_bot-0.1.3.tar", max compression
+gzip compressed data, was "chatgpt_bot-0.1.4.tar", max compression
```

## Comparing `chatgpt_bot-0.1.3.tar` & `chatgpt_bot-0.1.4.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0      621 2023-05-02 00:55:38.104075 chatgpt_bot-0.1.3/README.md
--rwxr-xr-x   0        0        0     4964 2023-05-02 00:53:52.160595 chatgpt_bot-0.1.3/chatgpt_bot/__init__.py
--rw-r--r--   0        0        0      569 2023-05-02 00:56:05.047942 chatgpt_bot-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1403 1970-01-01 00:00:00.000000 chatgpt_bot-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      621 2023-05-02 00:55:38.104075 chatgpt_bot-0.1.4/README.md
+-rwxr-xr-x   0        0        0     5047 2023-05-06 11:55:31.529451 chatgpt_bot-0.1.4/chatgpt_bot/__init__.py
+-rw-r--r--   0        0        0      569 2023-05-06 11:55:49.377339 chatgpt_bot-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1403 1970-01-01 00:00:00.000000 chatgpt_bot-0.1.4/PKG-INFO
```

### Comparing `chatgpt_bot-0.1.3/README.md` & `chatgpt_bot-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `chatgpt_bot-0.1.3/chatgpt_bot/__init__.py` & `chatgpt_bot-0.1.4/chatgpt_bot/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,29 +16,32 @@
         self,
         conversation_id: str,
         api_key: str,
         system_prompt: str = "You are a helpful virtual assistant.",
         database_filename: str = "database.sqlite3",
         model: str = "gpt-3.5-turbo",
         message_limit: Optional[int] = None,
+        time_limit: Optional[int] = None,
     ):
         """
         Initialize the class.
 
         conversation_id - A random conversation ID (whatever you want).
         api_key - Your OpenAI API key.
         system_prompt - The ChatGPT system prompt you want to use.
         database_filename - Where you want to save the database."
         model - The ChatGPT model version to use.
         message_limit - The number of messages to retrieve from history every time.
+        time_limit - Only send GPT previous messages exchanged within `time_limit` hours.
         """
         openai.api_key = api_key
         self._conversation_id = conversation_id
         self._system_prompt = system_prompt
         self._message_limit = message_limit
+        self._time_limit = time_limit
         self._model = model
         self._con = sqlite3.connect(database_filename)
         self._cur = self._con.cursor()
 
         self._cur.execute(
             """
         CREATE TABLE IF NOT EXISTS "Message" (
@@ -84,34 +87,32 @@
             (self._conversation_id, "user" if user else "assistant", message),
         )
 
         self._con.commit()
 
     def _get_messages(self) -> List[Dict[str, Any]]:
         """Retrieve all messages from the database."""
-        if self._message_limit:
-            self._cur.execute(
-                """
-            SELECT id, timestamp, role, message FROM "Message" WHERE
-            conversation_id=?
-            ORDER BY timestamp DESC
-            LIMIT ?;
-            """,
-                (self._conversation_id, self._message_limit),
-            )
-        else:
-            self._cur.execute(
-                """
+        query = [
+            """
             SELECT id, timestamp, role, message FROM "Message" WHERE
             conversation_id=?
-            ORDER BY timestamp DESC
-            """,
-                (self._conversation_id,),
+            """
+        ]
+
+        if self._time_limit:
+            query.append(
+                f"AND timestamp >= datetime('now', '-{self._time_limit} hours')"
             )
 
+        query.append("ORDER BY timestamp DESC")
+
+        if self._message_limit:
+            query.append(f"LIMIT {self._message_limit}")
+
+        self._cur.execute(" ".join(query), (self._conversation_id,))
         messages = [
             {"id": x[0], "timestamp": x[1], "role": x[2], "message": x[3]}
             for x in reversed(self._cur.fetchall())
         ]
         return messages
 
     def get_metadata(self) -> Any:
```

### Comparing `chatgpt_bot-0.1.3/pyproject.toml` & `chatgpt_bot-0.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "chatgpt-bot"
-version = "0.1.3"
+version = "0.1.4"
 description = "A library that takes the pain out of creating ChatGPT bots."
 authors = ["Stavros Korokithakis <hi@stavros.io>"]
 repository = "https://github.com/skorokithakis/ChatGPT-Bot"
 homepage = "https://github.com/skorokithakis/ChatGPT-Bot"
 license = "MIT"
 readme = "README.md"
 packages = [{include = "chatgpt_bot"}]
```

### Comparing `chatgpt_bot-0.1.3/PKG-INFO` & `chatgpt_bot-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatgpt-bot
-Version: 0.1.3
+Version: 0.1.4
 Summary: A library that takes the pain out of creating ChatGPT bots.
 Home-page: https://github.com/skorokithakis/ChatGPT-Bot
 License: MIT
 Author: Stavros Korokithakis
 Author-email: hi@stavros.io
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

