# Comparing `tmp/serial_packets-0.0.4.tar.gz` & `tmp/serial_packets-0.1.0.tar.gz`

## Comparing `serial_packets-0.0.4.tar` & `serial_packets-0.1.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 serial_packets-0.0.4/src/serial_packets/__init__.py
--rw-r--r--   0        0        0     7036 2020-02-02 00:00:00.000000 serial_packets-0.0.4/src/serial_packets/_packet_decoder.py
--rw-r--r--   0        0        0     4061 2020-02-02 00:00:00.000000 serial_packets-0.0.4/src/serial_packets/_packet_encoder.py
--rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 serial_packets-0.0.4/src/serial_packets/_packets.py
--rw-r--r--   0        0        0    17205 2020-02-02 00:00:00.000000 serial_packets-0.0.4/src/serial_packets/client.py
--rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 serial_packets-0.0.4/src/serial_packets/packets.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 serial_packets-0.0.4/src/serial_packets/py.typed
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 serial_packets-0.0.4/.gitignore
--rw-r--r--   0        0        0     7169 2020-02-02 00:00:00.000000 serial_packets-0.0.4/LICENSE
--rw-r--r--   0        0        0    13657 2020-02-02 00:00:00.000000 serial_packets-0.0.4/README.md
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 serial_packets-0.0.4/pyproject.toml
--rw-r--r--   0        0        0    14014 2020-02-02 00:00:00.000000 serial_packets-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 serial_packets-0.1.0/src/serial_packets/__init__.py
+-rw-r--r--   0        0        0     7036 2020-02-02 00:00:00.000000 serial_packets-0.1.0/src/serial_packets/_packet_decoder.py
+-rw-r--r--   0        0        0     4061 2020-02-02 00:00:00.000000 serial_packets-0.1.0/src/serial_packets/_packet_encoder.py
+-rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 serial_packets-0.1.0/src/serial_packets/_packets.py
+-rw-r--r--   0        0        0    17547 2020-02-02 00:00:00.000000 serial_packets-0.1.0/src/serial_packets/client.py
+-rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 serial_packets-0.1.0/src/serial_packets/packets.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 serial_packets-0.1.0/src/serial_packets/py.typed
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 serial_packets-0.1.0/.gitignore
+-rw-r--r--   0        0        0     7169 2020-02-02 00:00:00.000000 serial_packets-0.1.0/LICENSE
+-rw-r--r--   0        0        0    13657 2020-02-02 00:00:00.000000 serial_packets-0.1.0/README.md
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 serial_packets-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0    14014 2020-02-02 00:00:00.000000 serial_packets-0.1.0/PKG-INFO
```

### Comparing `serial_packets-0.0.4/src/serial_packets/_packet_decoder.py` & `serial_packets-0.1.0/src/serial_packets/_packet_decoder.py`

 * *Files identical despite different names*

### Comparing `serial_packets-0.0.4/src/serial_packets/_packet_encoder.py` & `serial_packets-0.1.0/src/serial_packets/_packet_encoder.py`

 * *Files identical despite different names*

### Comparing `serial_packets-0.0.4/src/serial_packets/_packets.py` & `serial_packets-0.1.0/src/serial_packets/_packets.py`

 * *Files identical despite different names*

### Comparing `serial_packets-0.0.4/src/serial_packets/client.py` & `serial_packets-0.1.0/src/serial_packets/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,36 +79,41 @@
 
 
 class SerialPacketsClient:
 
     def __init__(self,
                  port: str,
                  command_async_callback: Optional(Callable[[int, bytearray],
-                                                           Tuple(int, bytearray)]),
-                 message_async_callback: Optional(Callable[[int, bytearray], None]),
-                 event_async_callback: Optional(Callable[[PacketsEvent], None]),
+                                                           Tuple(int, bytearray)]) = None,
+                 message_async_callback: Optional(Callable[[int, bytearray], None]) = None,
+                 event_async_callback: Optional(Callable[[PacketsEvent], None]) = None,
                  baudrate: int = 115200,
                  workers: int = DEFAULT_WORKERS_COUNT):
         """
         Constructs a serial messaging client. 
         
         The constructor doesn't actually open the port. To do that, call connect().
 
         Args:
         * port: A string with dependent serial port to use. E.g. 'COM1'.
             
-        * command_async_callback: An async callback function to be called on incoming
+        * command_async_callback: An optional async callback function to be called on incoming
           command requests. Ignored if None. This is an async function that accepts 
           an endpoint (int [0-255]) and command data (bytearray, [0 to DATA_MAX_LEN]) and return
           status (int [0-255]) and response data (bytearray, [0 to DATA_MAX_LEN]).
           
-        * message_async_callback: An async callback function to be called on incoming
+        * message_async_callback: An optional async callback function to be called on incoming
           messages. Ignored if None. This is an async function that accepts 
           an endpoint (int [0-255]) and command data (bytearray, [0 to DATA_MAX_LEN]) 
           and does not return a value.
+          
+        * event_async_callback: An optional async callback function to be called on
+          on certain client events such as port connection and disconnection. 
+          Ignored if None. This is an async function that accepts 
+          a PacketEvent argument and returns no value.
                 
         * baudrate: And optional int port baud rate to set. Default is 115200.
         
         * workers: An optional int that specifies how many worker tasks the client should
         use for servicing user callbacks. Having a value higher than 1 allows 
         more parallelism, but may be unnecessary. Range is MIN_WORKERS_COUNT to 
         MAX_WORKERS_COUNT, and default is DEFAULT_WORKERS_COUNT. 
@@ -160,15 +165,15 @@
         logger.debug("Connecting to port [%s]", self.__port)
         try:
             self.__transport, self.__protocol = await serial_asyncio.create_serial_connection(
                 asyncio.get_event_loop(), _SerialProtocol, self.__port, baudrate=self.__baudrate)
         except Exception as e:
             logger.error("%s", e)
             if logging.DEBUG >= logger.getEffectiveLevel():
-              traceback.print_exception(e)
+                traceback.print_exception(e)
             return False
         self.__protocol.set(self, self.__port, self.__packet_decoder)
         return True
 
     def __on_decoded_packet(self, decoded_packet: DecodedCommandPacket | DecodedResponsePacket |
                             DecodedMessagePacket):
         """Called from the packet decoder on each receive packet"""
```

### Comparing `serial_packets-0.0.4/src/serial_packets/packets.py` & `serial_packets-0.1.0/src/serial_packets/packets.py`

 * *Files identical despite different names*

### Comparing `serial_packets-0.0.4/LICENSE` & `serial_packets-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `serial_packets-0.0.4/README.md` & `serial_packets-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `serial_packets-0.0.4/pyproject.toml` & `serial_packets-0.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "serial_packets"
-version = "0.0.4"
+version = "0.1.0"
 authors = [
   { name="Zapta", email="zapta@zapta.com" },
 ]
 description = "A Python impelementation of the Serial Packets protocol"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `serial_packets-0.0.4/PKG-INFO` & `serial_packets-0.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: serial_packets
-Version: 0.0.4
+Version: 0.1.0
 Summary: A Python impelementation of the Serial Packets protocol
 Project-URL: Homepage, https://github.com/zapta/serial_packets_py
 Project-URL: Bug Tracker, https://github.com/zapta/serial_packets_py/issues
 Author-email: Zapta <zapta@zapta.com>
 License-File: LICENSE
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Classifier: Operating System :: OS Independent
```

