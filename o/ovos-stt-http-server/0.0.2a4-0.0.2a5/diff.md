# Comparing `tmp/ovos-stt-http-server-0.0.2a4.tar.gz` & `tmp/ovos-stt-http-server-0.0.2a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovos-stt-http-server-0.0.2a4.tar", last modified: Fri May  5 22:02:37 2023, max compression
+gzip compressed data, was "ovos-stt-http-server-0.0.2a5.tar", last modified: Fri May  5 23:20:06 2023, max compression
```

## Comparing `ovos-stt-http-server-0.0.2a4.tar` & `ovos-stt-http-server-0.0.2a5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:02:37.584654 ovos-stt-http-server-0.0.2a4/
--rw-r--r--   0 runner    (1001) docker     (123)    11347 2023-05-05 22:02:36.000000 ovos-stt-http-server-0.0.2a4/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-05-05 22:02:37.584654 ovos-stt-http-server-0.0.2a4/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:02:37.576654 ovos-stt-http-server-0.0.2a4/ovos_stt_http_server/
--rw-r--r--   0 runner    (1001) docker     (123)     4931 2023-05-05 22:02:36.000000 ovos-stt-http-server-0.0.2a4/ovos_stt_http_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-05-05 22:02:36.000000 ovos-stt-http-server-0.0.2a4/ovos_stt_http_server/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:02:37.584654 ovos-stt-http-server-0.0.2a4/ovos_stt_http_server/audio/
--rw-r--r--   0 runner    (1001) docker     (123)    58605 2023-05-05 22:02:36.000000 ovos-stt-http-server-0.0.2a4/ovos_stt_http_server/audio/ca.mp3
--rw-r--r--   0 runner    (1001) docker     (123)    54765 2023-05-05 22:02:36.000000 ovos-stt-http-server-0.0.2a4/ovos_stt_http_server/audio/de.mp3
--rw-r--r--   0 runner    (1001) docker     (123)    50925 2023-05-05 22:02:36.000000 ovos-stt-http-server-0.0.2a4/ovos_stt_http_server/audio/en.mp3
--rw-r--r--   0 runner    (1001) docker     (123)    55341 2023-05-05 22:02:36.000000 ovos-stt-http-server-0.0.2a4/ovos_stt_http_server/audio/es.mp3
--rw-r--r--   0 runner    (1001) docker     (123)    57453 2023-05-05 22:02:36.000000 ovos-stt-http-server-0.0.2a4/ovos_stt_http_server/audio/fr.mp3
--rw-r--r--   0 runner    (1001) docker     (123)    62637 2023-05-05 22:02:36.000000 ovos-stt-http-server-0.0.2a4/ovos_stt_http_server/audio/it.mp3
--rw-r--r--   0 runner    (1001) docker     (123)    68781 2023-05-05 22:02:36.000000 ovos-stt-http-server-0.0.2a4/ovos_stt_http_server/audio/nl.mp3
--rw-r--r--   0 runner    (1001) docker     (123)    48813 2023-05-05 22:02:36.000000 ovos-stt-http-server-0.0.2a4/ovos_stt_http_server/audio/pt.mp3
--rw-r--r--   0 runner    (1001) docker     (123)    67821 2023-05-05 22:02:36.000000 ovos-stt-http-server-0.0.2a4/ovos_stt_http_server/audio/uk.mp3
--rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-05-05 22:02:36.000000 ovos-stt-http-server-0.0.2a4/ovos_stt_http_server/gradio_app.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-05 22:02:36.000000 ovos-stt-http-server-0.0.2a4/ovos_stt_http_server/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:02:37.580654 ovos-stt-http-server-0.0.2a4/ovos_stt_http_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-05-05 22:02:37.000000 ovos-stt-http-server-0.0.2a4/ovos_stt_http_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-05-05 22:02:37.000000 ovos-stt-http-server-0.0.2a4/ovos_stt_http_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 22:02:37.000000 ovos-stt-http-server-0.0.2a4/ovos_stt_http_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-05 22:02:37.000000 ovos-stt-http-server-0.0.2a4/ovos_stt_http_server.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-05 22:02:37.000000 ovos-stt-http-server-0.0.2a4/ovos_stt_http_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-05 22:02:37.000000 ovos-stt-http-server-0.0.2a4/ovos_stt_http_server.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 22:02:37.000000 ovos-stt-http-server-0.0.2a4/ovos_stt_http_server.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 22:02:37.584654 ovos-stt-http-server-0.0.2a4/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3049 2023-05-05 22:02:36.000000 ovos-stt-http-server-0.0.2a4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 23:20:06.118240 ovos-stt-http-server-0.0.2a5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11347 2023-05-05 23:20:05.000000 ovos-stt-http-server-0.0.2a5/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-05-05 23:20:06.118240 ovos-stt-http-server-0.0.2a5/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 23:20:06.114240 ovos-stt-http-server-0.0.2a5/ovos_stt_http_server/
+-rw-r--r--   0 runner    (1001) docker     (123)     4931 2023-05-05 23:20:05.000000 ovos-stt-http-server-0.0.2a5/ovos_stt_http_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-05-05 23:20:05.000000 ovos-stt-http-server-0.0.2a5/ovos_stt_http_server/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 23:20:06.118240 ovos-stt-http-server-0.0.2a5/ovos_stt_http_server/audio/
+-rw-r--r--   0 runner    (1001) docker     (123)    58605 2023-05-05 23:20:05.000000 ovos-stt-http-server-0.0.2a5/ovos_stt_http_server/audio/ca.mp3
+-rw-r--r--   0 runner    (1001) docker     (123)    54765 2023-05-05 23:20:05.000000 ovos-stt-http-server-0.0.2a5/ovos_stt_http_server/audio/de.mp3
+-rw-r--r--   0 runner    (1001) docker     (123)    50925 2023-05-05 23:20:05.000000 ovos-stt-http-server-0.0.2a5/ovos_stt_http_server/audio/en.mp3
+-rw-r--r--   0 runner    (1001) docker     (123)    55341 2023-05-05 23:20:05.000000 ovos-stt-http-server-0.0.2a5/ovos_stt_http_server/audio/es.mp3
+-rw-r--r--   0 runner    (1001) docker     (123)    57453 2023-05-05 23:20:05.000000 ovos-stt-http-server-0.0.2a5/ovos_stt_http_server/audio/fr.mp3
+-rw-r--r--   0 runner    (1001) docker     (123)    62637 2023-05-05 23:20:05.000000 ovos-stt-http-server-0.0.2a5/ovos_stt_http_server/audio/it.mp3
+-rw-r--r--   0 runner    (1001) docker     (123)    68781 2023-05-05 23:20:05.000000 ovos-stt-http-server-0.0.2a5/ovos_stt_http_server/audio/nl.mp3
+-rw-r--r--   0 runner    (1001) docker     (123)    48813 2023-05-05 23:20:05.000000 ovos-stt-http-server-0.0.2a5/ovos_stt_http_server/audio/pt.mp3
+-rw-r--r--   0 runner    (1001) docker     (123)    67821 2023-05-05 23:20:05.000000 ovos-stt-http-server-0.0.2a5/ovos_stt_http_server/audio/uk.mp3
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-05-05 23:20:05.000000 ovos-stt-http-server-0.0.2a5/ovos_stt_http_server/gradio_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-05 23:20:05.000000 ovos-stt-http-server-0.0.2a5/ovos_stt_http_server/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 23:20:06.114240 ovos-stt-http-server-0.0.2a5/ovos_stt_http_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-05-05 23:20:06.000000 ovos-stt-http-server-0.0.2a5/ovos_stt_http_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-05-05 23:20:06.000000 ovos-stt-http-server-0.0.2a5/ovos_stt_http_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 23:20:06.000000 ovos-stt-http-server-0.0.2a5/ovos_stt_http_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-05 23:20:06.000000 ovos-stt-http-server-0.0.2a5/ovos_stt_http_server.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-05 23:20:06.000000 ovos-stt-http-server-0.0.2a5/ovos_stt_http_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-05 23:20:06.000000 ovos-stt-http-server-0.0.2a5/ovos_stt_http_server.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 23:20:06.000000 ovos-stt-http-server-0.0.2a5/ovos_stt_http_server.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 23:20:06.118240 ovos-stt-http-server-0.0.2a5/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3049 2023-05-05 23:20:05.000000 ovos-stt-http-server-0.0.2a5/setup.py
```

### Comparing `ovos-stt-http-server-0.0.2a4/LICENSE.md` & `ovos-stt-http-server-0.0.2a5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ovos-stt-http-server-0.0.2a4/PKG-INFO` & `ovos-stt-http-server-0.0.2a5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovos-stt-http-server
-Version: 0.0.2a4
+Version: 0.0.2a5
 Summary: simple aiohttp server to host OpenVoiceOS stt plugins as a service
 Home-page: https://github.com/OpenVoiceOS/ovos-stt-http-server
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Keywords: plugin STT OVOS OpenVoiceOS
 Platform: UNKNOWN
@@ -36,20 +36,27 @@
 ## Usage
 
 ```bash
 ovos-stt-server --help
 usage: ovos-stt-server [-h] [--engine ENGINE] [--port PORT] [--host HOST]
 
 options:
-  -h, --help       show this help message and exit
-  --engine ENGINE  stt plugin to be used
-  --port PORT      port number
-  --host HOST      host
+  -h, --help                  show this help message and exit
+  --engine ENGINE             stt plugin to be used
+  --port PORT                 port number
+  --host HOST                 host
+  --lang LANG                 default language
+  --gradio                    flag to enable Gradio web UI
+  --cache                     flag to pre-cache examples in Gradio web UI
+  --title TITLE               title for Gradio UI
+  --description DESCRIPTION   Description for Gradio UI
+  --info INFO                 Text to display in Gradio UI
+  --badge BADGE               URL of badge to show in Gradio UI
 ```
-
+> Note: `ffmpeg` is required for Gradio
 ## Companion plugin
 
 Use with OpenVoiceOS [companion plugin](https://github.com/OpenVoiceOS/ovos-stt-server-plugin)
 
 
 ## Docker
```

### Comparing `ovos-stt-http-server-0.0.2a4/ovos_stt_http_server/__init__.py` & `ovos-stt-http-server-0.0.2a5/ovos_stt_http_server/__init__.py`

 * *Files identical despite different names*

### Comparing `ovos-stt-http-server-0.0.2a4/ovos_stt_http_server/__main__.py` & `ovos-stt-http-server-0.0.2a5/ovos_stt_http_server/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,27 +23,29 @@
     parser.add_argument("--engine", help="stt plugin to be used", required=True)
     parser.add_argument("--port", help="port number", default=8080)
     parser.add_argument("--host", help="host", default="0.0.0.0")
     parser.add_argument("--lang", help="default language supported by plugin",
                         default="en-us")
     parser.add_argument("--gradio", help="Enable Gradio Web UI",
                         action="store_true")
+    parser.add_argument("--cache", help="Cache models for Gradio demo",
+                        action="store_true")
     parser.add_argument("--title", help="Title for webUI",
                         default="STT")
     parser.add_argument("--description", help="Text description to print in UI",
                         default="Get Speech-To-Text")
     parser.add_argument("--info", help="Text to display at end of UI",
                         default=None)
     parser.add_argument("--badge", help="URL of visitor badge", default=None)
     args = parser.parse_args()
 
     server, engine = start_stt_server(args.engine)
     LOG.info("Server Started")
     if args.gradio:
         bind_gradio_service(server, engine, args.title, args.description,
-                            args.info, args.badge, args.lang)
+                            args.info, args.badge, args.lang, args.cache)
         LOG.info("Gradio Started")
     uvicorn.run(server, host=args.host, port=args.port)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `ovos-stt-http-server-0.0.2a4/ovos_stt_http_server/audio/ca.mp3` & `ovos-stt-http-server-0.0.2a5/ovos_stt_http_server/audio/ca.mp3`

 * *Files identical despite different names*

### Comparing `ovos-stt-http-server-0.0.2a4/ovos_stt_http_server/audio/de.mp3` & `ovos-stt-http-server-0.0.2a5/ovos_stt_http_server/audio/de.mp3`

 * *Files identical despite different names*

### Comparing `ovos-stt-http-server-0.0.2a4/ovos_stt_http_server/audio/en.mp3` & `ovos-stt-http-server-0.0.2a5/ovos_stt_http_server/audio/en.mp3`

 * *Files identical despite different names*

### Comparing `ovos-stt-http-server-0.0.2a4/ovos_stt_http_server/audio/es.mp3` & `ovos-stt-http-server-0.0.2a5/ovos_stt_http_server/audio/es.mp3`

 * *Files identical despite different names*

### Comparing `ovos-stt-http-server-0.0.2a4/ovos_stt_http_server/audio/fr.mp3` & `ovos-stt-http-server-0.0.2a5/ovos_stt_http_server/audio/fr.mp3`

 * *Files identical despite different names*

### Comparing `ovos-stt-http-server-0.0.2a4/ovos_stt_http_server/audio/it.mp3` & `ovos-stt-http-server-0.0.2a5/ovos_stt_http_server/audio/it.mp3`

 * *Files identical despite different names*

### Comparing `ovos-stt-http-server-0.0.2a4/ovos_stt_http_server/audio/nl.mp3` & `ovos-stt-http-server-0.0.2a5/ovos_stt_http_server/audio/nl.mp3`

 * *Files identical despite different names*

### Comparing `ovos-stt-http-server-0.0.2a4/ovos_stt_http_server/audio/pt.mp3` & `ovos-stt-http-server-0.0.2a5/ovos_stt_http_server/audio/pt.mp3`

 * *Files identical despite different names*

### Comparing `ovos-stt-http-server-0.0.2a4/ovos_stt_http_server/audio/uk.mp3` & `ovos-stt-http-server-0.0.2a5/ovos_stt_http_server/audio/uk.mp3`

 * *Files identical despite different names*

### Comparing `ovos-stt-http-server-0.0.2a4/ovos_stt_http_server/gradio_app.py` & `ovos-stt-http-server-0.0.2a5/ovos_stt_http_server/gradio_app.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 
 import gradio as gr
 
-from os.path import join, dirname, basename, splitext
+from os.path import join, dirname, basename, splitext, isfile
 from ovos_utils.log import LOG
 from ovos_stt_http_server import ModelContainer, bytes2audiodata
 
 STT = None
 
 
 def transcribe(audio_file, language: str):
     with open(audio_file, 'rb') as f:
         audio = f.read()
     return STT.process_audio(bytes2audiodata(audio), language)
 
 
 def bind_gradio_service(app, stt_engine: ModelContainer,
                         title, description, info, badge,
-                        default_lang="en"):
+                        default_lang="en", cache=True):
     global STT
     STT = stt_engine
     languages = list(stt_engine.plugin().available_languages or [default_lang])
     languages.sort()
     LOG.debug(languages)
 
     if default_lang not in languages:
@@ -28,29 +28,30 @@
         default_lang = default_lang.split('-')[0]
     if default_lang not in languages:
         LOG.warning(f"{default_lang} not in languages, choosing first lang")
         default_lang = languages[0]
 
     examples = [join(dirname(__file__), 'audio', f'{lang.split("-")[0]}.mp3')
                 for lang in languages]
+    examples = [example for example in examples if isfile(example)]
     iface = gr.Interface(
         fn=transcribe,
         inputs=[
             gr.Audio(source="microphone", type="filepath"),
             gr.Radio(
                 label="Language",
                 choices=languages,
                 value=default_lang
             )
         ],
         outputs=[
             "textbox"
         ],
         examples=[[e, basename(splitext(e)[0])] for e in examples],
-        cache_examples=True,  # Takes some time at init, but speeds up runtime
+        cache_examples=cache,  # Takes some time at init, but speeds up runtime
         live=True,
         title=title,
         description=description,
         article=info,
         analytics_enabled=False)
 
     LOG.info(f"Mounting app to /gradio")
```

### Comparing `ovos-stt-http-server-0.0.2a4/ovos_stt_http_server.egg-info/PKG-INFO` & `ovos-stt-http-server-0.0.2a5/ovos_stt_http_server.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovos-stt-http-server
-Version: 0.0.2a4
+Version: 0.0.2a5
 Summary: simple aiohttp server to host OpenVoiceOS stt plugins as a service
 Home-page: https://github.com/OpenVoiceOS/ovos-stt-http-server
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Keywords: plugin STT OVOS OpenVoiceOS
 Platform: UNKNOWN
@@ -36,20 +36,27 @@
 ## Usage
 
 ```bash
 ovos-stt-server --help
 usage: ovos-stt-server [-h] [--engine ENGINE] [--port PORT] [--host HOST]
 
 options:
-  -h, --help       show this help message and exit
-  --engine ENGINE  stt plugin to be used
-  --port PORT      port number
-  --host HOST      host
+  -h, --help                  show this help message and exit
+  --engine ENGINE             stt plugin to be used
+  --port PORT                 port number
+  --host HOST                 host
+  --lang LANG                 default language
+  --gradio                    flag to enable Gradio web UI
+  --cache                     flag to pre-cache examples in Gradio web UI
+  --title TITLE               title for Gradio UI
+  --description DESCRIPTION   Description for Gradio UI
+  --info INFO                 Text to display in Gradio UI
+  --badge BADGE               URL of badge to show in Gradio UI
 ```
-
+> Note: `ffmpeg` is required for Gradio
 ## Companion plugin
 
 Use with OpenVoiceOS [companion plugin](https://github.com/OpenVoiceOS/ovos-stt-server-plugin)
 
 
 ## Docker
```

### Comparing `ovos-stt-http-server-0.0.2a4/ovos_stt_http_server.egg-info/SOURCES.txt` & `ovos-stt-http-server-0.0.2a5/ovos_stt_http_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ovos-stt-http-server-0.0.2a4/setup.py` & `ovos-stt-http-server-0.0.2a5/setup.py`

 * *Files identical despite different names*

