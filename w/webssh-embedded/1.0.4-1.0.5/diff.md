# Comparing `tmp/webssh_embedded-1.0.4.tar.gz` & `tmp/webssh_embedded-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webssh_embedded-1.0.4.tar", last modified: Sun Apr 16 16:13:12 2023, max compression
+gzip compressed data, was "webssh_embedded-1.0.5.tar", last modified: Sat May  6 06:51:24 2023, max compression
```

## Comparing `webssh_embedded-1.0.4.tar` & `webssh_embedded-1.0.5.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-16 16:13:12.780186 webssh_embedded-1.0.4/
--rw-r--r--   0 kali      (1000) kali      (1000)     2255 2023-04-13 11:38:35.000000 webssh_embedded-1.0.4/LICENSE
--rw-r--r--   0 kali      (1000) kali      (1000)       87 2023-04-12 10:34:57.000000 webssh_embedded-1.0.4/MANIFEST.in
--rw-r--r--   0 kali      (1000) kali      (1000)      778 2023-04-16 16:13:12.780186 webssh_embedded-1.0.4/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)      218 2023-04-16 16:12:51.000000 webssh_embedded-1.0.4/README.rst
--rw-r--r--   0 kali      (1000) kali      (1000)      172 2023-04-16 16:13:12.780186 webssh_embedded-1.0.4/setup.cfg
--rw-r--r--   0 kali      (1000) kali      (1000)     1067 2023-04-11 18:02:24.000000 webssh_embedded-1.0.4/setup.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-16 16:13:12.768186 webssh_embedded-1.0.4/webssh_embedded/
--rw-r--r--   0 kali      (1000) kali      (1000)      328 2023-04-11 15:20:01.000000 webssh_embedded-1.0.4/webssh_embedded/__init__.py
--rw-r--r--   0 kali      (1000) kali      (1000)       80 2023-04-16 16:04:00.000000 webssh_embedded-1.0.4/webssh_embedded/_version.py
--rw-r--r--   0 kali      (1000) kali      (1000)    23739 2023-04-11 15:20:01.000000 webssh_embedded-1.0.4/webssh_embedded/handler.py
--rw-r--r--   0 kali      (1000) kali      (1000)     2049 2023-04-11 15:20:01.000000 webssh_embedded-1.0.4/webssh_embedded/main.py
--rw-r--r--   0 kali      (1000) kali      (1000)     2677 2023-04-11 15:20:01.000000 webssh_embedded-1.0.4/webssh_embedded/policy.py
--rw-r--r--   0 kali      (1000) kali      (1000)     6630 2023-04-11 17:53:31.000000 webssh_embedded-1.0.4/webssh_embedded/settings.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-16 16:13:12.764186 webssh_embedded-1.0.4/webssh_embedded/static/
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-16 16:13:12.776186 webssh_embedded-1.0.4/webssh_embedded/static/css/
--rw-r--r--   0 kali      (1000) kali      (1000)   155758 2023-04-11 15:20:01.000000 webssh_embedded-1.0.4/webssh_embedded/static/css/bootstrap.min.css
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-16 16:13:12.776186 webssh_embedded-1.0.4/webssh_embedded/static/css/fonts/
--rw-r--r--   0 kali      (1000) kali      (1000)        0 2023-04-11 15:20:01.000000 webssh_embedded-1.0.4/webssh_embedded/static/css/fonts/.gitignore
--rw-r--r--   0 kali      (1000) kali      (1000)      145 2023-04-11 15:20:01.000000 webssh_embedded-1.0.4/webssh_embedded/static/css/fullscreen.min.css
--rw-r--r--   0 kali      (1000) kali      (1000)     1344 2023-04-11 15:20:01.000000 webssh_embedded-1.0.4/webssh_embedded/static/css/xterm.min.css
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-16 16:13:12.776186 webssh_embedded-1.0.4/webssh_embedded/static/img/
--rw-r--r--   0 kali      (1000) kali      (1000)     5953 2023-04-11 15:20:01.000000 webssh_embedded-1.0.4/webssh_embedded/static/img/favicon.png
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-16 16:13:12.780186 webssh_embedded-1.0.4/webssh_embedded/static/js/
--rw-r--r--   0 kali      (1000) kali      (1000)    56292 2023-04-11 15:20:01.000000 webssh_embedded-1.0.4/webssh_embedded/static/js/bootstrap.min.js
--rw-r--r--   0 kali      (1000) kali      (1000)     4635 2023-04-16 16:03:44.000000 webssh_embedded-1.0.4/webssh_embedded/static/js/iframetest.html
--rw-r--r--   0 kali      (1000) kali      (1000)    86927 2023-04-11 15:20:01.000000 webssh_embedded-1.0.4/webssh_embedded/static/js/jquery.min.js
--rw-r--r--   0 kali      (1000) kali      (1000)    23784 2023-04-11 15:20:01.000000 webssh_embedded-1.0.4/webssh_embedded/static/js/main.js
--rw-r--r--   0 kali      (1000) kali      (1000)    21004 2023-04-11 15:20:01.000000 webssh_embedded-1.0.4/webssh_embedded/static/js/popper.min.js
--rw-r--r--   0 kali      (1000) kali      (1000)     2377 2023-04-11 15:20:01.000000 webssh_embedded-1.0.4/webssh_embedded/static/js/xterm-addon-fit.min.js
--rw-r--r--   0 kali      (1000) kali      (1000)   251949 2023-04-11 15:20:01.000000 webssh_embedded-1.0.4/webssh_embedded/static/js/xterm.min.js
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-16 16:13:12.780186 webssh_embedded-1.0.4/webssh_embedded/templates/
--rw-r--r--   0 kali      (1000) kali      (1000)     4604 2023-04-11 15:20:01.000000 webssh_embedded-1.0.4/webssh_embedded/templates/index.html
--rw-r--r--   0 kali      (1000) kali      (1000)     2919 2023-04-11 15:20:01.000000 webssh_embedded-1.0.4/webssh_embedded/utils.py
--rw-r--r--   0 kali      (1000) kali      (1000)    10816 2023-04-13 17:52:22.000000 webssh_embedded-1.0.4/webssh_embedded/worker.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-16 16:13:12.772186 webssh_embedded-1.0.4/webssh_embedded.egg-info/
--rw-r--r--   0 kali      (1000) kali      (1000)      778 2023-04-16 16:13:12.000000 webssh_embedded-1.0.4/webssh_embedded.egg-info/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)     1036 2023-04-16 16:13:12.000000 webssh_embedded-1.0.4/webssh_embedded.egg-info/SOURCES.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        1 2023-04-16 16:13:12.000000 webssh_embedded-1.0.4/webssh_embedded.egg-info/dependency_links.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       64 2023-04-16 16:13:12.000000 webssh_embedded-1.0.4/webssh_embedded.egg-info/entry_points.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       54 2023-04-16 16:13:12.000000 webssh_embedded-1.0.4/webssh_embedded.egg-info/requires.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       16 2023-04-16 16:13:12.000000 webssh_embedded-1.0.4/webssh_embedded.egg-info/top_level.txt
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-05-06 06:51:24.512149 webssh_embedded-1.0.5/
+-rw-r--r--   0 kali      (1000) kali      (1000)     2255 2023-04-13 11:38:35.000000 webssh_embedded-1.0.5/LICENSE
+-rw-r--r--   0 kali      (1000) kali      (1000)       87 2023-04-12 10:34:57.000000 webssh_embedded-1.0.5/MANIFEST.in
+-rw-r--r--   0 kali      (1000) kali      (1000)     1245 2023-05-06 06:51:24.512149 webssh_embedded-1.0.5/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)      685 2023-05-06 06:48:52.000000 webssh_embedded-1.0.5/README.rst
+-rw-r--r--   0 kali      (1000) kali      (1000)      172 2023-05-06 06:51:24.516151 webssh_embedded-1.0.5/setup.cfg
+-rw-r--r--   0 kali      (1000) kali      (1000)     1067 2023-04-11 18:02:24.000000 webssh_embedded-1.0.5/setup.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-05-06 06:51:24.500143 webssh_embedded-1.0.5/webssh_embedded/
+-rw-r--r--   0 kali      (1000) kali      (1000)      328 2023-04-27 10:02:53.000000 webssh_embedded-1.0.5/webssh_embedded/__init__.py
+-rw-r--r--   0 kali      (1000) kali      (1000)       80 2023-05-06 06:13:01.000000 webssh_embedded-1.0.5/webssh_embedded/_version.py
+-rw-r--r--   0 kali      (1000) kali      (1000)    24246 2023-04-30 07:58:01.000000 webssh_embedded-1.0.5/webssh_embedded/handler.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     2049 2023-04-27 10:02:53.000000 webssh_embedded-1.0.5/webssh_embedded/main.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     2677 2023-04-27 10:02:53.000000 webssh_embedded-1.0.5/webssh_embedded/policy.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     6630 2023-04-27 10:02:53.000000 webssh_embedded-1.0.5/webssh_embedded/settings.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-05-06 06:51:24.488137 webssh_embedded-1.0.5/webssh_embedded/static/
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-05-06 06:51:24.504145 webssh_embedded-1.0.5/webssh_embedded/static/css/
+-rw-r--r--   0 kali      (1000) kali      (1000)   155758 2023-04-27 10:02:53.000000 webssh_embedded-1.0.5/webssh_embedded/static/css/bootstrap.min.css
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-05-06 06:51:24.504145 webssh_embedded-1.0.5/webssh_embedded/static/css/fonts/
+-rw-r--r--   0 kali      (1000) kali      (1000)        0 2023-04-27 10:02:53.000000 webssh_embedded-1.0.5/webssh_embedded/static/css/fonts/.gitignore
+-rw-r--r--   0 kali      (1000) kali      (1000)      145 2023-04-27 10:02:53.000000 webssh_embedded-1.0.5/webssh_embedded/static/css/fullscreen.min.css
+-rw-r--r--   0 kali      (1000) kali      (1000)     1344 2023-04-27 10:02:53.000000 webssh_embedded-1.0.5/webssh_embedded/static/css/xterm.min.css
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-05-06 06:51:24.504145 webssh_embedded-1.0.5/webssh_embedded/static/img/
+-rw-r--r--   0 kali      (1000) kali      (1000)     5953 2023-04-27 10:02:53.000000 webssh_embedded-1.0.5/webssh_embedded/static/img/favicon.png
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-05-06 06:51:24.512149 webssh_embedded-1.0.5/webssh_embedded/static/js/
+-rw-r--r--   0 kali      (1000) kali      (1000)    56292 2023-04-27 10:02:53.000000 webssh_embedded-1.0.5/webssh_embedded/static/js/bootstrap.min.js
+-rw-r--r--   0 kali      (1000) kali      (1000)     4803 2023-04-27 12:17:25.000000 webssh_embedded-1.0.5/webssh_embedded/static/js/iframetest.html
+-rw-r--r--   0 kali      (1000) kali      (1000)    86927 2023-04-27 10:02:53.000000 webssh_embedded-1.0.5/webssh_embedded/static/js/jquery.min.js
+-rw-r--r--   0 kali      (1000) kali      (1000)    23287 2023-04-27 11:34:32.000000 webssh_embedded-1.0.5/webssh_embedded/static/js/main.js
+-rw-r--r--   0 kali      (1000) kali      (1000)    21004 2023-04-27 10:02:53.000000 webssh_embedded-1.0.5/webssh_embedded/static/js/popper.min.js
+-rw-r--r--   0 kali      (1000) kali      (1000)     2377 2023-04-27 10:02:53.000000 webssh_embedded-1.0.5/webssh_embedded/static/js/xterm-addon-fit.min.js
+-rw-r--r--   0 kali      (1000) kali      (1000)   251949 2023-04-27 10:02:53.000000 webssh_embedded-1.0.5/webssh_embedded/static/js/xterm.min.js
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-05-06 06:51:24.512149 webssh_embedded-1.0.5/webssh_embedded/templates/
+-rw-r--r--   0 kali      (1000) kali      (1000)     4604 2023-04-27 10:02:53.000000 webssh_embedded-1.0.5/webssh_embedded/templates/index.html
+-rw-r--r--   0 kali      (1000) kali      (1000)     2919 2023-04-27 10:02:53.000000 webssh_embedded-1.0.5/webssh_embedded/utils.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     9037 2023-04-27 14:42:49.000000 webssh_embedded-1.0.5/webssh_embedded/worker.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-05-06 06:51:24.504145 webssh_embedded-1.0.5/webssh_embedded.egg-info/
+-rw-r--r--   0 kali      (1000) kali      (1000)     1245 2023-05-06 06:51:24.000000 webssh_embedded-1.0.5/webssh_embedded.egg-info/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)     1036 2023-05-06 06:51:24.000000 webssh_embedded-1.0.5/webssh_embedded.egg-info/SOURCES.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)        1 2023-05-06 06:51:24.000000 webssh_embedded-1.0.5/webssh_embedded.egg-info/dependency_links.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       64 2023-05-06 06:51:24.000000 webssh_embedded-1.0.5/webssh_embedded.egg-info/entry_points.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       54 2023-05-06 06:51:24.000000 webssh_embedded-1.0.5/webssh_embedded.egg-info/requires.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       16 2023-05-06 06:51:24.000000 webssh_embedded-1.0.5/webssh_embedded.egg-info/top_level.txt
```

### Comparing `webssh_embedded-1.0.4/LICENSE` & `webssh_embedded-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `webssh_embedded-1.0.4/setup.py` & `webssh_embedded-1.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `webssh_embedded-1.0.4/webssh_embedded/handler.py` & `webssh_embedded-1.0.5/webssh_embedded/handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -659,36 +659,45 @@
 
         resize = msg.get('resize')
         if resize and len(resize) == 2:
             try:
                 worker.chan.resize_pty(*resize)
             except (TypeError, struct.error, paramiko.SSHException):
                 pass
-
+        #the special commands are ones that we can just execute and not wait for its status.
+        special_commands=['script']
         data = msg.get('data')
         if data and isinstance(data, UnicodeType):
             #use regular expressions to search for command inserted into the terminal
-            match_object=re.search("echo 'COMMAND_OUTPUT!@#",data)
+            match_object=re.search("!@#abc123",data)
             if(match_object):
-                match_object1=re.search(";time",data)
-                match_object2=re.search(";echo",data)
-                if(match_object1 and match_object2):
+                data=data[match_object.start()+9:]
+                match_object2=re.search(";echo 'Command_",data)
+                if(match_object2):
                     #tell the worker that a command has arrived
-                    worker.input_command.append(data[match_object1.start()+7:match_object2.start()-1])
+                    worker.input_command.append(data[:match_object2.start()])
+                    for i in special_commands:
+                        x=re.search(i,data[:match_object2.start()])
+                        if(x):
+                            if(x.start()==0):
+                                data=data[:match_object2.start()]+"\n"
+                                worker.input_command.pop(0)
+                                break
+                    else:
                     #tell the worker that time at which command has arrived
-                    worker.timestamp.append(datetime.now())
+                        worker.entry_timestamp.append(datetime.now())
                     #create a unique identifier for every command
-                    uid='CID'
-                    for i in range(10):
-                        uid=uid+str(random.randint(0,9))
-                    for i in range(3):
-                        uid=uid+random.choice(string.ascii_letters).upper()
-                    worker.command_ids.append(uid)
-                    worker.push_command_id()
-                    logging.info("Command recieved")
+                        uid='CID'
+                        for i in range(10):
+                            uid=uid+str(random.randint(0,9))
+                        for i in range(3):
+                            uid=uid+random.choice(string.ascii_letters).upper()
+                        worker.command_ids.append(uid)
+                        worker.push_command_id()
+                        logging.info("Command recieved")
                     
             worker.data_to_dst.append(data)
             worker.on_write()
 
     def on_close(self):
         logging.info('Disconnected from {}:{}'.format(*self.src_addr))
         if not self.close_reason:
```

### Comparing `webssh_embedded-1.0.4/webssh_embedded/main.py` & `webssh_embedded-1.0.5/webssh_embedded/main.py`

 * *Files identical despite different names*

### Comparing `webssh_embedded-1.0.4/webssh_embedded/policy.py` & `webssh_embedded-1.0.5/webssh_embedded/policy.py`

 * *Files identical despite different names*

### Comparing `webssh_embedded-1.0.4/webssh_embedded/settings.py` & `webssh_embedded-1.0.5/webssh_embedded/settings.py`

 * *Files identical despite different names*

### Comparing `webssh_embedded-1.0.4/webssh_embedded/static/css/bootstrap.min.css` & `webssh_embedded-1.0.5/webssh_embedded/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `webssh_embedded-1.0.4/webssh_embedded/static/css/xterm.min.css` & `webssh_embedded-1.0.5/webssh_embedded/static/css/xterm.min.css`

 * *Files identical despite different names*

### Comparing `webssh_embedded-1.0.4/webssh_embedded/static/img/favicon.png` & `webssh_embedded-1.0.5/webssh_embedded/static/img/favicon.png`

 * *Files identical despite different names*

### Comparing `webssh_embedded-1.0.4/webssh_embedded/static/js/bootstrap.min.js` & `webssh_embedded-1.0.5/webssh_embedded/static/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `webssh_embedded-1.0.4/webssh_embedded/static/js/iframetest.html` & `webssh_embedded-1.0.5/webssh_embedded/static/js/iframetest.html`

 * *Files 9% similar despite different names*

```diff
@@ -1,55 +1,52 @@
 <html>
 <head>
 <style>
-#terminal{
-/*width: 500px;
-height:500px;
+#clear{
 position:absolute;
-left:500px;
-top:500px;*/
+top:60px;
+right:0px;
+}
+#terminal{
 position:absolute;
 bottom:0px;
 height:300px;
 width:100%;
 resize:both;
 overflow:auto;
 }
 </style>
-<!--Interactive JS library
-<script src="https://cdn.jsdelivr.net/gh/interactiveJS/interactiveJS@v2.0.1/src/interactive.min.js"></script>
-<link href="https://cdn.jsdelivr.net/gh/interactiveJS/interactiveJS@v2.0.1/src/css/interactive.min.css" rel="stylesheet"/>-->
 </head>
 <body>
 
 <!--The div 'app' is a div that contains mechanisms to:
 1. Type input command and send it to the iframe
 2. Display the command status, time and command id for the entered command
 -->
 <div id="app">
   <input id="message" type="text" />
-  <button id="sendMessage">Send Message</button><br>
+  <button id="sendMessage">Execute Command</button><br>
   <button id="CES">Command Execution Status</button><br>
   <input id="Time" type="text" readonly/>
   <input id="command_id" type="text" readonly/>
 </div>
+<div id="clear">
+Yellow button is to be used only when button input is disabled due to some error.<br>
+<button onclick="clear_storage()" style="background-color:yellow">CLEAR PENDING COMMAND</button>
+</div>
 
 <div id="terminal">
 <!--To obtain the form page and enter ssh credentials
 http://localhost:8888-->
 <!--To bypass form if credentials are already known.Make sure password is entered in Base64 form. To obtain base64 form use the following command:
 echo -n 'password' | base64
 http://localhost:8888?hostname=<hostname>&&username=<username>&&password=<base_64_encoded>-->
 <iframe id="myFrame" src="http://localhost:8888" style="width:100%; height:100%;"></iframe>
 </div>
 </body>
-<!--add resizable, closeable, maximizable and minimizable features through InteractiveJS Javascript library-->
-<script>
-      //interactive('terminal');
-</script>
 <script>
 //script to send command to the iframe.
   var button = document.querySelector("#sendMessage");
   function sendMessage() {
   if(sessionStorage.command_state==='1'){
   alert("You have a command running in the terminal. Please wait for its completion. You can open a new tab for entering commands if needed");}
   else{
@@ -113,8 +110,17 @@
 document.getElementById("CES").style.background='green';
 else
 document.getElementById("CES").style.background='red';
     socket.close()
 });
 }
 </script>
+<script>
+//to clear session storage in case of error. This makes it convenient for the user to enable button input instead of manually clearing session storage
+function clear_storage(){
+sessionStorage.command_state=0;
+//since the terminal is in an error state, reload the iframe to obtain a fresh terminal.
+const iframe = document.querySelector("iframe");
+iframe.contentWindow.location.reload();
+}
+</script>
 </html>
```

#### html2text {}

```diff
@@ -1,5 +1,7 @@
-
-[                    ] Send Message
+[                    ] Execute Command
 Command Execution Status
 [                    ] [                    ]
+Yellow button is to be used only when button input is disabled due to some
+error.
+CLEAR PENDING COMMAND
```

### Comparing `webssh_embedded-1.0.4/webssh_embedded/static/js/jquery.min.js` & `webssh_embedded-1.0.5/webssh_embedded/static/js/jquery.min.js`

 * *Files identical despite different names*

### Comparing `webssh_embedded-1.0.4/webssh_embedded/static/js/main.js` & `webssh_embedded-1.0.5/webssh_embedded/static/js/main.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -422,38 +422,23 @@
                 $('#b3').click();
             }
         }
 
         //function to extract command status and execution time sent by the server and send it to the iframe
         function get_time_status(text) {
             var command_output = null;
-            /*
-              var t=text.toString();
-              if(t.search("COMMAND_EXECUTION!@#")!=-1){
-              this.flag=1;
-              }
-              var pos1=t.search('real');
-              if(pos1!=-1 && this.flag==1){
-              var beg=pos1+5;
-              var sub=t.substring(beg);
-              var end=sub.search('s');
-              execution_time+=t.substring(beg,beg+end+1);}
-              var pos=t.search('Command_Execution_Status:');
-              if(pos!=-1 && this.flag===1){
-                command_execution_status+=t.substring(pos+25,pos+26);
-                this.flag=0;}*/
             var t = text.toString();
             var pos1 = t.search(";!@#");
             var pos2 = t.search("#@!;");
             if (pos1 != -1 && pos2 != -1) {
                 command_output = JSON.parse(t.substring(pos1 + 4, pos2));
             }
             if (command_output != null) {
                 this.flag = 1;
-                console.log(command_output.Execution_Time + "ffff" + command_output.Command_Execution_Status);
+                console.log("Command_Execution_Time:" + command_output.Execution_Time + " Command Execution Status:" + command_output.Command_Execution_Status);
                 $('#command_output_data').val(JSON.stringify(command_output));
                 $('#b2').click();
             }
         }
 
         function term_write(text) {
             if (term) {
@@ -474,16 +459,16 @@
             }
         }
 
         //to recieve command from the iframe and send it to the server
         function execute_command() {
             var x = document.getElementById('command_data').value
             console.log("command:" + x);
-            var command = "echo 'COMMAND_OUTPUT!@#\n';time (";
-            command += x + ");echo '\nCommand_Execution_Status:'$?\n"
+            var command = "";
+            command += "!@#abc123" + x + ";echo 'Command_Execution_Status:'$?\n"
             try {
                 sock.send(JSON.stringify({
                     'data': command
                 }));
             } catch (err) {
                 console.log("Socket Error; Make sure you reload the webpage and authenticate before passing commands");
             }
```

### Comparing `webssh_embedded-1.0.4/webssh_embedded/static/js/popper.min.js` & `webssh_embedded-1.0.5/webssh_embedded/static/js/popper.min.js`

 * *Files identical despite different names*

### Comparing `webssh_embedded-1.0.4/webssh_embedded/static/js/xterm-addon-fit.min.js` & `webssh_embedded-1.0.5/webssh_embedded/static/js/xterm-addon-fit.min.js`

 * *Files identical despite different names*

### Comparing `webssh_embedded-1.0.4/webssh_embedded/static/js/xterm.min.js` & `webssh_embedded-1.0.5/webssh_embedded/static/js/xterm.min.js`

 * *Files identical despite different names*

### Comparing `webssh_embedded-1.0.4/webssh_embedded/templates/index.html` & `webssh_embedded-1.0.5/webssh_embedded/templates/index.html`

 * *Files identical despite different names*

### Comparing `webssh_embedded-1.0.4/webssh_embedded/utils.py` & `webssh_embedded-1.0.5/webssh_embedded/utils.py`

 * *Files identical despite different names*

### Comparing `webssh_embedded-1.0.4/webssh_embedded/worker.py` & `webssh_embedded-1.0.5/webssh_embedded/worker.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import tornado.websocket
 from uuid import uuid4
 from tornado.ioloop import IOLoop
 from tornado.iostream import _ERRNO_CONNRESET
 from tornado.util import errno_from_exception
 #additional libraries
 import mysql.connector as my
+from datetime import datetime
 import re
 BUF_SIZE = 32 * 1024
 clients = {}  # {ip: {id: worker}}
 
 def clear_worker(worker, clients):
     ip = worker.src_addr[0]
     workers = clients.get(ip)
@@ -42,22 +43,17 @@
         self.fd = chan.fileno()
         self.id = self.gen_id()
         self.data_to_dst = []
         self.handler = None
         self.mode = IOLoop.READ
         self.closed = False
         #the variables defined below are for various purposes. To add one, simpy write self.<variable_name>
-        self.coflag=0
-        self.timeflag1=0
-        self.timeflag2=0
-        self.temp=0
-        self.temp_time_storage=""
         self.input_command=[]
         self.command_ids=[]
-        self.timestamp=[]
+        self.entry_timestamp=[]
         self.session_close_flag=1
         self.cnx=None
         self.mysqlcon_status=0
         
         try:
             self.cnx=my.connect(user="root",host="localhost",password="")
             self.mysqlcon_status=1
@@ -70,67 +66,24 @@
         if events & IOLoop.WRITE:
             self.on_write()
         if events & IOLoop.ERROR:
             self.close(reason='error event occurred')        
             
     #to extract the command execution status and time taken to execute the comand
     def get_time_status(self,text):
-        execution_time=''
         command_execution_status=''
+        execution_time=''
         t=text.decode()
-        if(self.temp==1):
-            self.temp=self.temp+1
-        #co,ro,so,cst are match objects
-        #r,c are indices for 'real' and 'Command_Execution_Status:' respectively
-        co=re.search("COMMAND_OUTPUT!@#",t)
-        if(co):
-            self.coflag=1
-        if(self.coflag==1):
-            ro=re.search('real',t)
-            r=-1
-            if(ro):
-                logging.info("Command time recieved")
-                self.temp=1
-                self.timeflag1=1
-                r=ro.start()
-            try:
-                if(self.timeflag1==1):
-                    tstart,tend=-1,-1
-                    if(self.temp==1):
-                        tstart=re.search('\d+\.\d+',t[r:]).start()
-                        tend=re.search('s',t[r:]).start()
-                        execution_time=execution_time+t[r:][tstart:tend+1]
-                    else:
-                        tstart=re.search('\d+\.\d+',t).start()
-                        tend=re.search('s',t).start()
-                        execution_time=execution_time+t[tstart:tend+1]
-                    self.timeflag1=0
-                    self.timeflag2=1
-                    self.temp_time_storage=execution_time
-            except:
-                    pass
-            c=-1
-            if(self.timeflag2==1):
-                try:
-                    if(self.temp==1):
-                        c=re.search('Command_Execution_Status:',t[r:]).start()
-                        cstring=t[r:][c:].split(':')[1].rstrip('\r')
-                        cst=re.search('[0-9]{1,3}',cstring)
-                        command_execution_status=command_execution_status+cstring[cst.start():cst.end()]
-                    else:
-                        c=re.search('Command_Execution_Status:',t).start()
-                        cstring=t[c:].split(':')[1].rstrip('\r')
-                        cst=re.search('[0-9]{1,3}',cstring)
-                        command_execution_status=command_execution_status+cstring[cst.start():cst.end()]
-                    self.temp=0
-                    self.coflag=0
-                    self.timeflag2=0
-                    execution_time=self.temp_time_storage
-                except:
-                    pass
+        cst=re.search('Command_Execution_Status:[0-9]{1,3}',t)
+        if(cst and len(self.entry_timestamp)!=0):
+            exit_time=datetime.now()
+            execution_time=execution_time+str(round((exit_time-self.entry_timestamp[0]).total_seconds(),2))+"s"
+            colon_pos=re.search(":",t[cst.start():cst.end()]).start()
+            command_execution_status=command_execution_status+t[cst.start()+colon_pos+1:cst.end()]
+            logging.info("Command status and time recieved")
         return command_execution_status,execution_time
     
     #To pass command id to the client
     def push_command_id(self):
        if(len(self.input_command)!=0):
         try:
             res=bytes("!@#Command_ID:"+self.command_ids[0], 'utf-8')
@@ -140,15 +93,15 @@
             
     def insert_command(self,command_execution_status,execution_time):
            cr=self.cnx.cursor(buffered=True)
            cr.execute("use command_database")
            add_command = ("INSERT INTO command_table"
                 "(Command_ID,Command,Command_Execution_Status,Execution_Time,Timestamp)"
                  "VALUES (%s, %s, %s, %s,%s)")
-           command=(self.command_ids[0],self.input_command[0],command_execution_status,execution_time,self.timestamp[0])
+           command=(self.command_ids[0],self.input_command[0],command_execution_status,execution_time,self.entry_timestamp[0])
            try:
                 cr.execute(add_command,command)
                 logging.info("record was successfully inserted")
            except Exception as e:
                 logging.info(e)
            try:
                self.cnx.commit()
@@ -197,26 +150,26 @@
                         self.session_close_flag=1
                         self.insert_command(command_execution_status,execution_time)
                         self.mysqlcon_status=0
                         self.cnx.close()
                         self.clean_up("client disconnected")
                     logging.info("Command:"+self.input_command[0]+",Command_ID:"+self.command_ids[0]+",Command Status:"+
                                  command_execution_status+",Execution time:"+execution_time+
-                                 ",Timestamp:"+str(self.timestamp[0]))
+                                 ",Timestamp:"+str(self.entry_timestamp[0]))
                     #Insert command information into database
                     if(self.mysqlcon_status==1 and len(self.input_command)!=0):
                         self.insert_command(command_execution_status,execution_time)
                     test_string=';!@#{"Command_Execution_Status":"'+command_execution_status+'","Execution_Time":"'+execution_time+'"}#@!;'
                     res = bytes(test_string, 'utf-8')
                     #To send status and time back to client
                     self.handler.write_message(res, binary=True)
                     #To clear inserted command to enable entry of next
                     self.input_command.pop(0)
                     self.command_ids.pop(0)
-                    self.timestamp.pop(0)
+                    self.entry_timestamp.pop(0)
                 self.handler.write_message(data, binary=True)
             except tornado.websocket.WebSocketClosedError:
                 self.close(reason='websocket closed')
 
     def on_write(self):
         logging.debug('worker {} on write'.format(self.id))
         if not self.data_to_dst:
```

### Comparing `webssh_embedded-1.0.4/webssh_embedded.egg-info/SOURCES.txt` & `webssh_embedded-1.0.5/webssh_embedded.egg-info/SOURCES.txt`

 * *Files identical despite different names*

