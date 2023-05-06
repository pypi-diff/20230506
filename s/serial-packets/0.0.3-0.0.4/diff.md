# Comparing `tmp/serial_packets-0.0.3.tar.gz` & `tmp/serial_packets-0.0.4.tar.gz`

## Comparing `serial_packets-0.0.3.tar` & `serial_packets-0.0.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 serial_packets-0.0.3/src/serial_packets/__init__.py
--rw-r--r--   0        0        0     5800 2020-02-02 00:00:00.000000 serial_packets-0.0.3/src/serial_packets/_packet_decoder.py
--rw-r--r--   0        0        0     3207 2020-02-02 00:00:00.000000 serial_packets-0.0.3/src/serial_packets/_packet_encoder.py
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 serial_packets-0.0.3/src/serial_packets/_packets.py
--rw-r--r--   0        0        0    11734 2020-02-02 00:00:00.000000 serial_packets-0.0.3/src/serial_packets/client.py
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 serial_packets-0.0.3/src/serial_packets/packets.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 serial_packets-0.0.3/src/serial_packets/py.typed
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 serial_packets-0.0.3/.gitignore
--rw-r--r--   0        0        0     7169 2020-02-02 00:00:00.000000 serial_packets-0.0.3/LICENSE
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 serial_packets-0.0.3/README.md
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 serial_packets-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 serial_packets-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 serial_packets-0.0.4/src/serial_packets/__init__.py
+-rw-r--r--   0        0        0     7036 2020-02-02 00:00:00.000000 serial_packets-0.0.4/src/serial_packets/_packet_decoder.py
+-rw-r--r--   0        0        0     4061 2020-02-02 00:00:00.000000 serial_packets-0.0.4/src/serial_packets/_packet_encoder.py
+-rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 serial_packets-0.0.4/src/serial_packets/_packets.py
+-rw-r--r--   0        0        0    17205 2020-02-02 00:00:00.000000 serial_packets-0.0.4/src/serial_packets/client.py
+-rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 serial_packets-0.0.4/src/serial_packets/packets.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 serial_packets-0.0.4/src/serial_packets/py.typed
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 serial_packets-0.0.4/.gitignore
+-rw-r--r--   0        0        0     7169 2020-02-02 00:00:00.000000 serial_packets-0.0.4/LICENSE
+-rw-r--r--   0        0        0    13657 2020-02-02 00:00:00.000000 serial_packets-0.0.4/README.md
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 serial_packets-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0    14014 2020-02-02 00:00:00.000000 serial_packets-0.0.4/PKG-INFO
```

### Comparing `serial_packets-0.0.3/src/serial_packets/_packet_encoder.py` & `serial_packets-0.0.4/src/serial_packets/_packet_encoder.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,47 +1,57 @@
 from __future__ import annotations
 
 import logging
 import time
 
 from PyCRC.CRCCCITT import CRCCCITT
-from ._packets import PacketType, PACKET_FLAG, PACKET_ESC, DATA_MAX_LEN, PACKET_MAX_LEN,  PRE_FLAG_TIMEOUT
+from ._packets import PacketType, PACKET_FLAG, PACKET_ESC, MAX_DATA_LEN, MAX_PACKET_LEN,  PRE_FLAG_TIMEOUT
 
 logger = logging.getLogger(__name__)
 
 
 class PacketEncoder:
 
     def __init__(self):
-        self.__packets_counter = 0
         self.__last_packet_time = 0
         self.__crc_calc = CRCCCITT("FFFF")
 
     def __construct_command_packet(self, cmd_id: int, endpoint: int, data: bytearray):
-        """Construct command packet, before byte stuffing"""
+        """Constructs a command packet, before byte stuffing"""
         packet = bytearray()
         packet.append(PacketType.COMMAND.value)
         packet.extend(cmd_id.to_bytes(4, 'big'))
         packet.append(endpoint)
         packet.extend(data)
         crc = self.__crc_calc.calculate(bytes(packet))
         packet.extend(crc.to_bytes(2, 'big'))
-        assert (len(packet) <= PACKET_MAX_LEN)
+        assert (len(packet) <= MAX_PACKET_LEN)
         return packet
 
     def __construct_response_packet(self, cmd_id: int, status: int, data: bytearray):
-        """Construct response packet, before byte stuffing"""
+        """Constructs a response packet, before byte stuffing"""
         packet = bytearray()
         packet.append(PacketType.RESPONSE.value)
         packet.extend(cmd_id.to_bytes(4, 'big'))
         packet.append(status)
         packet.extend(data)
         crc = self.__crc_calc.calculate(bytes(packet))
         packet.extend(crc.to_bytes(2, 'big'))
-        assert (len(packet) <= PACKET_MAX_LEN)
+        assert (len(packet) <= MAX_PACKET_LEN)
+        return packet
+      
+    def __construct_message_packet(self, endpoint: int, data: bytearray):
+        """Constructs a message packet, before byte stuffing"""
+        packet = bytearray()
+        packet.append(PacketType.MESSAGE.value)
+        packet.append(endpoint)
+        packet.extend(data)
+        crc = self.__crc_calc.calculate(bytes(packet))
+        packet.extend(crc.to_bytes(2, 'big'))
+        assert (len(packet) <= MAX_PACKET_LEN)
         return packet
 
     def __stuff_packet_bytes(self, packet: bytearray, insert_pre_flag: bool):
         """Byte stuff the packet using HDLC format. Also adds packet flag(s)"""
         result = bytearray()
         if insert_pre_flag:
             result.append(PACKET_FLAG)
@@ -59,21 +69,30 @@
         self.__last_packet_time = time.time()
         elapsed = self.__last_packet_time - last_packet_time
         # We insert a pre packet flag only if the packets are sparse.
         insert_pre_flag = elapsed > PRE_FLAG_TIMEOUT
         return insert_pre_flag
 
     def encode_command_packet(self, cmd_id: int, endpoint: int, data: bytearray):
-        """Returns a command packet in wire format"""
-        assert (len(data) <= DATA_MAX_LEN)
+        """Returns the command packet in wire format"""
+        assert (len(data) <= MAX_DATA_LEN)
         insert_pre_flag = self.__track_packet_interval()
         packet = self.__construct_command_packet(cmd_id, endpoint, data)
         stuffed_packet = self.__stuff_packet_bytes(packet, insert_pre_flag)
         return stuffed_packet
 
     def encode_response_packet(self, cmd_id: int, status: int, data: bytearray):
-        """Returns a packet in wire format."""
-        assert (len(data) <= DATA_MAX_LEN)
+        """Returns the packet in wire format."""
+        assert (len(data) <= MAX_DATA_LEN)
         insert_pre_flag = self.__track_packet_interval()
         packet = self.__construct_response_packet(cmd_id, status, data)
         stuffed_packet = self.__stuff_packet_bytes(packet, insert_pre_flag)
         return stuffed_packet
+      
+    def encode_message_packet(self,  endpoint: int, data: bytearray):
+        """Returns the message packet in wire format"""
+        assert (len(data) <= MAX_DATA_LEN)
+        insert_pre_flag = self.__track_packet_interval()
+        packet = self.__construct_message_packet(endpoint, data)
+        stuffed_packet = self.__stuff_packet_bytes(packet, insert_pre_flag)
+        return stuffed_packet  
+
```

### Comparing `serial_packets-0.0.3/src/serial_packets/_packets.py` & `serial_packets-0.0.4/src/serial_packets/_packets.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,37 @@
 from __future__ import annotations
 
 from enum import Enum
-from .packets import DATA_MAX_LEN
+from .packets import MAX_DATA_LEN
 
 # Flag and escape bytes per HDLC specification.
 PACKET_FLAG = 0x7E
 PACKET_ESC = 0X7D
 
 # Prefix a packet with a flag byte only if interval from previous
 # encoded packet is longer that this time in secs.
 PRE_FLAG_TIMEOUT = 1.0
 
 # Packet sizes in bytes, with zero data length, and before
 # byte stuffing, and flagging.
-PACKET_MIN_OVERHEAD = 4
-PACKET_MAX_OVERHEAD = 8
+MIN_PACKET_OVERHEAD = 4
+MAX_PACKET_OVERHEAD = 8
 
-PACKET_MIN_LEN = PACKET_MIN_OVERHEAD
-PACKET_MAX_LEN = PACKET_MAX_OVERHEAD + DATA_MAX_LEN
+MIN_PACKET_LEN = MIN_PACKET_OVERHEAD
+MAX_PACKET_LEN = MAX_PACKET_OVERHEAD + MAX_DATA_LEN
+
+# Range of command timeout values.
+MIN_CMD_TIMEOUT = 0.1
+MAX_CMD_TIMEOUT = 10.0
+DEFAULT_CMD_TIMEOUT = 1.0
+
+# How many workers the use can request.
+MIN_WORKERS_COUNT = 1
+MAX_WORKERS_COUNT = 30
+DEFAULT_WORKERS_COUNT = 3
 
 # Do not change the numeric tags since the will change
 # the wire representation.
 class PacketType(Enum):
     COMMAND = 1
     RESPONSE = 2
+    MESSAGE = 3
```

### Comparing `serial_packets-0.0.3/src/serial_packets/client.py` & `serial_packets-0.0.4/src/serial_packets/client.py`

 * *Files 23% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 import time
 import traceback
 
 from enum import Enum
 from typing import Optional, Tuple, Dict, Callable
 from asyncio.transports import BaseTransport
 from ._packet_encoder import PacketEncoder
-from ._packet_decoder import PacketDecoder, DecodedPacket
-from ._packets import PacketType, DATA_MAX_LEN
-from .packets import PacketStatus
+from ._packet_decoder import PacketDecoder, DecodedCommandPacket, DecodedResponsePacket, DecodedMessagePacket
+from ._packets import PacketType, MAX_DATA_LEN, MIN_CMD_TIMEOUT, MAX_CMD_TIMEOUT, DEFAULT_CMD_TIMEOUT, MIN_WORKERS_COUNT, MAX_WORKERS_COUNT, DEFAULT_WORKERS_COUNT
+from .packets import PacketStatus, PacketsEvent, PacketsEventType, PacketsEvent, MAX_USER_ENDPOINT
 
 logger = logging.getLogger(__name__)
 
 # pyserial_asyncio is documented at
 # https://github.com/pyserial/pyserial-asyncio
 
 
@@ -40,173 +40,247 @@
         return time.time() > self.__expiration_time
 
 
 class _SerialProtocol(asyncio.Protocol):
     """Callbacks for the asyncio serial client."""
 
     def __init__(self):
+        self.__client: SerialPacketsClient = None
         self.__port: str = None
         self.__packet_decoder: PacketDecoder = None
+        self.__is_connected = False
 
-    def set(self, port: str, packet_decoder: PacketDecoder):
+    def set(self, client: SerialPacketsClient, port: str, packet_decoder: PacketDecoder):
+        self.__client = client
         self.__port = port
         self.__packet_decoder = packet_decoder
 
+    def is_connected(self):
+        return self.__is_connected
+
     def connection_made(self, transport: BaseTransport):
-        logger.info("Serial [%s] opened.", self.__port)
-        # print(f"port opened", flush=True)
-        # transport.serial.rts = False
+        self.__is_connected = True
+        self.__client._post_event(
+            PacketsEvent(PacketsEventType.CONNECTED, f"Connected to {self.__port}"))
 
     def data_received(self, data: bytes):
-        self.__packet_decoder.receive(data)
+        self.__packet_decoder._receive(data)
 
     def connection_lost(self, exc):
-        logger.info("Serial [%s] closed.", self.__port)
+        self.__is_connected = False
+        self.__client._post_event(
+            PacketsEvent(PacketsEventType.DISCONNECTED, f"Disconnected from {self.__port}"))
 
     def pause_writing(self):
         logger.warn("Serial [%s] paused.", self.__port)
         # print('Writing paused', flush=True)
 
     def resume_writing(self):
         logger.warn("Serial [%s] resumed.", self.__port)
-        # print('Writing resumed', flush=True)
 
 
 class SerialPacketsClient:
 
     def __init__(self,
                  port: str,
                  command_async_callback: Optional(Callable[[int, bytearray],
                                                            Tuple(int, bytearray)]),
+                 message_async_callback: Optional(Callable[[int, bytearray], None]),
+                 event_async_callback: Optional(Callable[[PacketsEvent], None]),
                  baudrate: int = 115200,
-                 workers=3):
+                 workers: int = DEFAULT_WORKERS_COUNT):
         """
         Constructs a serial messaging client. 
         
         The constructor doesn't actually open the port. To do that, call connect().
 
         Args:
         * port: A string with dependent serial port to use. E.g. 'COM1'.
             
         * command_async_callback: An async callback function to be called on incoming
           command requests. Ignored if None. This is an async function that accepts 
           an endpoint (int [0-255]) and command data (bytearray, [0 to DATA_MAX_LEN]) and return
           status (int [0-255]) and response data (bytearray, [0 to DATA_MAX_LEN]).
+          
+        * message_async_callback: An async callback function to be called on incoming
+          messages. Ignored if None. This is an async function that accepts 
+          an endpoint (int [0-255]) and command data (bytearray, [0 to DATA_MAX_LEN]) 
+          and does not return a value.
                 
         * baudrate: And optional int port baud rate to set. Default is 115200.
         
+        * workers: An optional int that specifies how many worker tasks the client should
+        use for servicing user callbacks. Having a value higher than 1 allows 
+        more parallelism, but may be unnecessary. Range is MIN_WORKERS_COUNT to 
+        MAX_WORKERS_COUNT, and default is DEFAULT_WORKERS_COUNT. 
+        
         Returns:
         * A new serial messaging client.
         """
-        assert (workers > 0, workers < 10)
+        assert (workers >= MIN_WORKERS_COUNT and workers <= MAX_WORKERS_COUNT)
         self.__port = port
         self.__baudrate = baudrate
         self.__command_async_callback = command_async_callback
+        self.__message_async_callback = message_async_callback
+        self.__event_async_callback = event_async_callback
         self.__transport = None
         self.__protocol = None
         self.__packet_encoder = PacketEncoder()
-        self.__packet_decoder = PacketDecoder()
+        self.__packet_decoder = PacketDecoder(self.__on_decoded_packet)
         self.__command_id_counter = 0
         self.__tx_cmd_contexts: Dict[int, _TxCommandContext] = {}
+        # Work items types:
+        # * PacketsEvent: call user's event handler.
+        # * DecodedCommandPacket: handle incoming command packet.
+        # * DecodedResponsePacket: handle incoming response packet.
+        # * DecodedMessagePacket: handle incoming message packet.
+        self.__work_queue = asyncio.Queue()
         # Per https://stackoverflow.com/questions/71304329
         self.__background_tasks = []
 
-        # Create a worker task to clean pending command contexts that were timeout.
-        logger.debug("Creating cleanup task")
-        task = asyncio.create_task(self.__cleanup_task_body(), name="cleanup")
-        self.__background_tasks.append(task)
+        self.__create_loop_runner_task(self.__cleanup_task_loop, "cleanup")
 
         # Create a few worker tasks to process incoming packets.
         logger.debug("Creating [%d] workers tasks", workers)
-        for i in range(3):
-            task = asyncio.create_task(self.__rx_task_body(), name=f"rx_task_{i+1:02d}")
-            self.__background_tasks.append(task)
+        for i in range(workers):
+            self.__create_loop_runner_task(self.__worker_task_loop, f"rx_task_{i+1:02d}")
 
     def __str__(self) -> str:
         return f"{self.__port}@{self.__baudrate}"
 
-    async def connect(self):
-        """Connect to serial port."""
-        logger.info("Connecting to port [%s]", self.__port)
-        self.__transport, self.__protocol = await serial_asyncio.create_serial_connection(
-            asyncio.get_event_loop(), _SerialProtocol, self.__port, baudrate=self.__baudrate)
-        self.__protocol.set(self.__port, self.__packet_decoder)
-
-    async def __cleanup_task_body(self):
-        """Body of the worker task that clean timeout tx command contexts"""
-        logger.debug("Cleanup task [%s] started", asyncio.current_task().get_name())
-        while True:
-            await asyncio.sleep(0.1)
-            # We can't delete while iterating the dict so iterating
-            # on an independent list of keys instead.
-            keys = list(self.__tx_cmd_contexts.keys())
-            for cmd_id in keys:
-                tx_context = self.__tx_cmd_contexts.get(cmd_id)
-                if tx_context.is_expired():
-                    # print(f"Cleaning timeout command {cmd_id}", flush=True)
-                    logger.warn("Command [%d] timeout", cmd_id)
-                    tx_context.set_result(0xff, bytearray())
-                    self.__tx_cmd_contexts.pop(cmd_id)
+    def is_connected(self) -> bool:
+        """Test if the client is connected to the port."""
+        return self.__protocol and self.__protocol.is_connected()
+
+    def _post_event(self, event: PacketsEvent) -> None:
+        logger.debug("Posted event: %s", event)
+        self.__work_queue.put_nowait(event)
+
+    async def connect(self) -> bool:
+        """Connect to serial port. Returns True if connected to port."""
+        logger.debug("Connecting to port [%s]", self.__port)
+        try:
+            self.__transport, self.__protocol = await serial_asyncio.create_serial_connection(
+                asyncio.get_event_loop(), _SerialProtocol, self.__port, baudrate=self.__baudrate)
+        except Exception as e:
+            logger.error("%s", e)
+            if logging.DEBUG >= logger.getEffectiveLevel():
+              traceback.print_exception(e)
+            return False
+        self.__protocol.set(self, self.__port, self.__packet_decoder)
+        return True
+
+    def __on_decoded_packet(self, decoded_packet: DecodedCommandPacket | DecodedResponsePacket |
+                            DecodedMessagePacket):
+        """Called from the packet decoder on each receive packet"""
+        logger.debug("Queuing incoming packet of type [%s.]", type(decoded_packet).__name__)
+        self.__work_queue.put_nowait(decoded_packet)
+
+    def __create_loop_runner_task(self, task_loop, name):
+        logger.debug("Creating task '%s'", name)
+        task = asyncio.create_task(self.__loop_runner_task(task_loop), name=name)
+        self.__background_tasks.append(task)
 
-    async def __rx_task_body(self):
-        """Body of the worker tasks to serve incoming packets."""
+    async def __loop_runner_task(self, task_loop):
+        """Run worker task loops"""
         task_name = asyncio.current_task().get_name()
-        # print(f"RX task '{task_name}' started", flush=True)
-        logger.debug("RX worker task [%s] started", asyncio.current_task().get_name())
+        logger.debug("Task started '%s'", task_name)
         while True:
-            packet: DecodedPacket = await self.__packet_decoder.get_next_packet()
-            # Since we call user's callback we want to protect the thread from
-            # exceptions.
             try:
-                if packet.type == PacketType.COMMAND:
-                    await self.__handle_incoming_command_packet(packet)
-                    continue
-                if packet.type == PacketType.RESPONSE:
-                    await self.__handle_incoming_response_packet(packet)
-                    continue
-                logger.error(f"Unknown packet type [%d], dropping", packet.type)
+                await task_loop(task_name)
             except Exception as e:
-                logger.error("Exception in worker [%s]: %s", task_name, e)
+                logger.error("Task [%s] exception:", task_name)
                 traceback.print_exception(e)
 
-    async def __handle_incoming_command_packet(self, packet: DecodedPacket):
-        assert (packet.type == PacketType.COMMAND)
+    async def __cleanup_task_loop(self, task_name):
+        """Worker task loop for cleaning outgoing commands that timeout."""
+        await asyncio.sleep(0.05)
+        # NOTE: Deleting dict elements inside a dict iteration is not allowed.
+        # Using a workaround instead.
+        keys = list(self.__tx_cmd_contexts.keys())
+        for cmd_id in keys:
+            tx_context = self.__tx_cmd_contexts.get(cmd_id)
+            if tx_context.is_expired():
+                logger.error("Command [%d] timeout", cmd_id)
+                tx_context.set_result(0xff, bytearray())
+                self.__tx_cmd_contexts.pop(cmd_id)
+
+    async def __worker_task_loop(self, task_name):
+        """Body of the worker tasks to serve incoming packets."""
+        # task_name = asyncio.current_task().get_name()
+        # print(f"RX task '{task_name}' started", flush=True)
+        # logger.debug("RX worker task [%s] started", task_name)
+        # while True:
+        work_item = await self.__work_queue.get()
+        # Since we call user's callback we want to protect the thread from
+        # exceptions.
+        if isinstance(work_item, DecodedCommandPacket):
+            await self.__handle_incoming_command_packet(work_item)
+        elif isinstance(work_item, DecodedResponsePacket):
+            await self.__handle_incoming_response_packet(work_item)
+        elif isinstance(work_item, DecodedMessagePacket):
+            await self.__handle_incoming_message_packet(work_item)
+        elif isinstance(work_item, PacketsEvent):
+            await self.__handle_packets_event(work_item)
+        else:
+            logger.error(f"Unknown work item type [%s], dropping", type(work_item))
+
+    async def __handle_incoming_command_packet(self, decoded_cmd_packet: DecodedCommandPacket):
+        assert (isinstance(decoded_cmd_packet, DecodedCommandPacket))
         if self.__command_async_callback:
-            status, data = await self.__command_async_callback(packet.endpoint, packet.data)
-            if len(data) > DATA_MAX_LEN:
+            status, data = await self.__command_async_callback(decoded_cmd_packet.endpoint,
+                                                               decoded_cmd_packet.data)
+            if len(data) > MAX_DATA_LEN:
                 logger.error("Command response data too long (%d), failing command", len(data))
                 status, data = (PacketStatus.LENGTH_ERROR.value, bytearray())
         else:
             status, data = (PacketStatus.UNHANDLED.value, bytearray())
-        response_packet = self.__packet_encoder.encode_response_packet(packet.cmd_id, status, data)
+        response_packet = self.__packet_encoder.encode_response_packet(
+            decoded_cmd_packet.cmd_id, status, data)
         self.__transport.write(response_packet)
 
-    async def __handle_incoming_response_packet(self, packet: DecodedPacket):
+    async def __handle_incoming_response_packet(self, decoded_rsp_packet: DecodedResponsePacket):
         # print(f"Handling resp packet ({len(self.__tx_cmd_contexts)} tx contexts)", flush=True)
-        assert (packet.type == PacketType.RESPONSE)
-        tx_context: _TxCommandContext = self.__tx_cmd_contexts.pop(packet.cmd_id, None)
+        assert (isinstance(decoded_rsp_packet, DecodedResponsePacket))
+        tx_context: _TxCommandContext = self.__tx_cmd_contexts.pop(decoded_rsp_packet.cmd_id, None)
         if not tx_context:
             logger.error("Response has no matching command [%d], may timeout. Dropping",
-                         packet.cmd_id)
+                         decoded_rsp_packet.cmd_id)
             # print(f"Response has no matching context {packet.cmd_id}, dropping", flush=True)
             return
-        tx_context.set_result(packet.status, packet.data)
+        tx_context.set_result(decoded_rsp_packet.status, decoded_rsp_packet.data)
+
+    async def __handle_incoming_message_packet(self, decoded_msg_packet: DecodedMessagePacket):
+        assert (isinstance(decoded_msg_packet, DecodedMessagePacket))
+        if self.__message_async_callback:
+            await self.__message_async_callback(decoded_msg_packet.endpoint,
+                                                decoded_msg_packet.data)
+        else:
+            logger.debug("No message callback, dropping incoming message")
+
+    async def __handle_packets_event(self, packets_event):
+        assert (isinstance(packets_event, PacketsEvent))
+        if self.__event_async_callback is None:
+            logger.debug("No event callback, dropping event: %s", packets_event)
+        else:
+            logger.debug("Callback with event %s", packets_event)
+            await self.__event_async_callback(packets_event)
 
     async def send_command_blocking(self,
                                     endpoint: int,
                                     data: bytearray,
-                                    timeout=1.0) -> Tuple([int, bytearray]):
+                                    timeout=DEFAULT_CMD_TIMEOUT) -> Tuple([int, bytearray]):
         """ Sends a command and wait for result or timeout. This is a convenience
         method that calls send_command_future() and then waits on the future
         for command result.
 
         Args:
-        * endpoint: The target endpoint (int [0-255]) on the receiver side.  
+        * endpoint: The target endpoint (int [0-MAX_USER_ENDPOINT]) on the receiver side.  
         * data: The command data (bytearray, [0, DATA_MAX_LEN]).
-        * timeout: Command timeout in secs (float 0.1 to 5.0, default 1.0). 
+        * timeout: Command timeout in secs (float MIN_CMD_TIMEOUT to MAX_CMD_TIMEOUT, default DEFAULT_CMD_TIMEOUT). 
         If a command response is not received within this period, the command
         is aborted with status PacketStatus.TIMEOUT.value and an empty 
         data bytearray.
         
         Returns:
         * status: The command returned status (int, [0-255]) or PacketStatus.TIMEOUT.value
         in case of a timeout.
@@ -216,47 +290,73 @@
         future = self.send_command_future(endpoint, data, timeout=timeout)
         status, data = await future
         return (status, data)
 
     def send_command_future(self,
                             endpoint: int,
                             data: bytearray,
-                            timeout=1.0) -> Tuple([int, bytearray]):
+                            timeout=DEFAULT_CMD_TIMEOUT) -> Tuple([int, bytearray]):
         """ Sends a command and return immediately without blocking. 
         
         Caller should wait on the returned future to receive the command
         response once available. The command response is a Tuple with 
         two values, the status code (int, [0-255]) and  response data
         byte returned from the caller (bytearray [0, MAX_DATA_LEN]). Some status
         code values are defined by PacketStatus enum.
 
         Args:
         * endpoint: The target endpoint (int [0-255]) on the receiver side.  
         * data: The command's data (bytearray [0, DATA_MAX_LEN]).
-        * timeout: Command timeout in secs (float 0.1 to 5.0, default 1.0). 
+        * timeout: Command timeout in secs (float MIN_CMD_TIMEOUT to MAX_CMD_TIMEOUT, default DEFAULT_CMD_TIMEOUT). 
         If a command response is not received within this period, the command
         is aborted with status PacketStatus.TIMEOUT.value and an empty 
         data bytearray.
         
         Returns:
         * A future to wait on for command result. 
         """
-        assert (endpoint >= 0 and endpoint <= 255)
-        assert (len(data) <= DATA_MAX_LEN)
-        assert (timeout >= 0.1 and timeout <= 5.0)
+        assert (endpoint >= 0 and endpoint <= MAX_USER_ENDPOINT)
+        assert (len(data) <= MAX_DATA_LEN)
+        assert (timeout >= MIN_CMD_TIMEOUT and timeout <= MAX_CMD_TIMEOUT)
+        if not self.is_connected():
+            logger.error("Client not connected when trying to send a message")
+            future = asyncio.Future()
+            future.set_result((PacketStatus.NOT_CONNECTED.value, bytearray()))
+            return future
         # Allocate a 32 bit fresh command id. Wrap around are ok since
         # commands are short living.
         self.__command_id_counter = (self.__command_id_counter + 1) & 0xffffffff
         cmd_id = self.__command_id_counter
         assert (not cmd_id in self.__tx_cmd_contexts)
         # Encode packet bytes
         packet = self.__packet_encoder.encode_command_packet(cmd_id, endpoint, data)
-        logger.debug("TX command packet [%d]: %s", cmd_id, packet.hex(sep=' '))
+        logger.debug("TX command packet [%d]: %s", endpoint, packet.hex(sep=' '))
         # Create command tx context
         expiration_time = time.time() + timeout
         future = asyncio.Future()
         tx_cmd_context = _TxCommandContext(cmd_id, expiration_time, future)
         self.__tx_cmd_contexts[cmd_id] = tx_cmd_context
         # Start sending
         self.__transport.write(packet)
         # Future will be signaled on response or timeout.
         return future
+
+    def send_message(self, endpoint: int, data: bytearray) -> None:
+        """ Sends a message. Returns immediately, before sending completed. 
+
+            Args:
+            * endpoint: The target endpoint (int [0-255]) on the receiver side.  
+            * data: The message's data (bytearray [0, DATA_MAX_LEN]).
+            
+            Returns:
+            * None.
+            """
+        assert (endpoint >= 0 and endpoint <= MAX_USER_ENDPOINT)
+        assert (len(data) <= MAX_DATA_LEN)
+        if not self.is_connected():
+            logger.warn("Client not connected, ignoring message send")
+            return
+        # Encode packet bytes
+        packet = self.__packet_encoder.encode_message_packet(endpoint, data)
+        logger.debug("TX message packet [%d]: %s", endpoint, packet.hex(sep=' '))
+        # Start sending
+        self.__transport.write(packet)
```

### Comparing `serial_packets-0.0.3/LICENSE` & `serial_packets-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `serial_packets-0.0.3/pyproject.toml` & `serial_packets-0.0.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "serial_packets"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Zapta", email="zapta@zapta.com" },
 ]
 description = "A Python impelementation of the Serial Packets protocol"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

