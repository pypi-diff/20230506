# Comparing `tmp/micropython_rp2_stubs-1.19.1.post9.tar.gz` & `tmp/micropython_rp2_stubs-1.20.0.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "micropython_rp2_stubs-1.19.1.post9.tar", max compression
+gzip compressed data, was "micropython_rp2_stubs-1.20.0.post1.tar", max compression
```

## Comparing `micropython_rp2_stubs-1.19.1.post9.tar` & `micropython_rp2_stubs-1.20.0.post1.tar`

### file list

```diff
@@ -1,77 +1,65 @@
--rw-r--r--   0        0        0     1070 2023-01-16 00:27:49.481318 micropython_rp2_stubs-1.19.1.post9/LICENSE.md
--rw-r--r--   0        0        0     2035 2023-01-16 00:27:49.481318 micropython_rp2_stubs-1.19.1.post9/README.md
--rw-r--r--   0        0        0       67 2023-01-16 00:27:03.181532 micropython_rp2_stubs-1.19.1.post9/_boot.pyi
--rw-r--r--   0        0        0       67 2023-01-16 00:27:03.181532 micropython_rp2_stubs-1.19.1.post9/_boot_fat.pyi
--rw-r--r--   0        0        0      269 2023-01-16 00:27:03.185532 micropython_rp2_stubs-1.19.1.post9/_onewire.pyi
--rw-r--r--   0        0        0     1321 2023-01-16 00:27:03.185532 micropython_rp2_stubs-1.19.1.post9/_rp2.pyi
--rw-r--r--   0        0        0      825 2023-01-16 00:27:03.185532 micropython_rp2_stubs-1.19.1.post9/_thread.pyi
--rw-r--r--   0        0        0      353 2023-01-16 00:27:03.185532 micropython_rp2_stubs-1.19.1.post9/_uasyncio.pyi
--rw-r--r--   0        0        0     1037 2023-01-16 00:27:03.185532 micropython_rp2_stubs-1.19.1.post9/aioble/__init__.pyi
--rw-r--r--   0        0        0     1153 2023-01-16 00:27:03.185532 micropython_rp2_stubs-1.19.1.post9/aioble/central.pyi
--rw-r--r--   0        0        0      848 2023-01-16 00:27:03.185532 micropython_rp2_stubs-1.19.1.post9/aioble/client.pyi
--rw-r--r--   0        0        0      430 2023-01-16 00:27:03.185532 micropython_rp2_stubs-1.19.1.post9/aioble/core.pyi
--rw-r--r--   0        0        0      690 2023-01-16 00:27:03.189532 micropython_rp2_stubs-1.19.1.post9/aioble/device.pyi
--rw-r--r--   0        0        0      400 2023-01-16 00:27:03.189532 micropython_rp2_stubs-1.19.1.post9/aioble/l2cap.pyi
--rw-r--r--   0        0        0      927 2023-01-16 00:27:03.189532 micropython_rp2_stubs-1.19.1.post9/aioble/peripheral.pyi
--rw-r--r--   0        0        0     2002 2023-01-16 00:27:03.189532 micropython_rp2_stubs-1.19.1.post9/aioble/server.pyi
--rw-r--r--   0        0        0     1017 2023-01-16 00:27:03.189532 micropython_rp2_stubs-1.19.1.post9/array.pyi
--rw-r--r--   0        0        0     1365 2023-01-16 00:27:03.189532 micropython_rp2_stubs-1.19.1.post9/binascii.pyi
--rw-r--r--   0        0        0     1385 2023-01-16 00:27:03.189532 micropython_rp2_stubs-1.19.1.post9/cmath.pyi
--rw-r--r--   0        0        0      329 2023-01-16 00:27:03.181532 micropython_rp2_stubs-1.19.1.post9/dht.pyi
--rw-r--r--   0        0        0      389 2023-01-16 00:27:03.181532 micropython_rp2_stubs-1.19.1.post9/ds18x20.pyi
--rw-r--r--   0        0        0      676 2023-01-16 00:27:03.189532 micropython_rp2_stubs-1.19.1.post9/errno.pyi
--rw-r--r--   0        0        0     4787 2023-01-16 00:27:03.189532 micropython_rp2_stubs-1.19.1.post9/framebuf.pyi
--rw-r--r--   0        0        0     1935 2023-01-16 00:27:03.189532 micropython_rp2_stubs-1.19.1.post9/gc.pyi
--rw-r--r--   0        0        0     1600 2023-01-16 00:27:03.189532 micropython_rp2_stubs-1.19.1.post9/hashlib.pyi
--rw-r--r--   0        0        0      897 2023-01-16 00:27:03.189532 micropython_rp2_stubs-1.19.1.post9/heapq.pyi
--rw-r--r--   0        0        0     1339 2023-01-16 00:27:03.189532 micropython_rp2_stubs-1.19.1.post9/json.pyi
--rw-r--r--   0        0        0      522 2023-01-16 00:27:03.189532 micropython_rp2_stubs-1.19.1.post9/lsm6dsox.pyi
--rw-r--r--   0        0        0    43609 2023-01-16 00:27:03.189532 micropython_rp2_stubs-1.19.1.post9/machine.pyi
--rw-r--r--   0        0        0     4400 2023-01-16 00:27:03.189532 micropython_rp2_stubs-1.19.1.post9/math.pyi
--rw-r--r--   0        0        0     7055 2023-01-16 00:27:02.873534 micropython_rp2_stubs-1.19.1.post9/micropython.pyi
--rw-r--r--   0        0        0      433 2023-01-16 00:27:03.181532 micropython_rp2_stubs-1.19.1.post9/neopixel.pyi
--rw-r--r--   0        0        0     6799 2023-01-16 00:27:03.189532 micropython_rp2_stubs-1.19.1.post9/network.pyi
--rw-r--r--   0        0        0      596 2023-01-16 00:27:03.181532 micropython_rp2_stubs-1.19.1.post9/onewire.pyi
--rw-r--r--   0        0        0     9063 2023-01-16 00:27:03.189532 micropython_rp2_stubs-1.19.1.post9/os.pyi
--rw-r--r--   0        0        0     3644 2023-01-16 00:27:49.985316 micropython_rp2_stubs-1.19.1.post9/pyproject.toml
--rw-r--r--   0        0        0     2553 2023-01-16 00:27:03.189532 micropython_rp2_stubs-1.19.1.post9/random.pyi
--rw-r--r--   0        0        0     1856 2023-01-16 00:27:03.181532 micropython_rp2_stubs-1.19.1.post9/rp2.pyi
--rw-r--r--   0        0        0     3760 2023-01-16 00:27:03.189532 micropython_rp2_stubs-1.19.1.post9/select.pyi
--rw-r--r--   0        0        0     9304 2023-01-16 00:27:03.189532 micropython_rp2_stubs-1.19.1.post9/socket.pyi
--rw-r--r--   0        0        0     1521 2023-01-16 00:27:03.189532 micropython_rp2_stubs-1.19.1.post9/struct.pyi
--rw-r--r--   0        0        0      838 2023-01-16 00:27:03.189532 micropython_rp2_stubs-1.19.1.post9/sys.pyi
--rw-r--r--   0        0        0    12180 2023-01-16 00:27:03.189532 micropython_rp2_stubs-1.19.1.post9/time.pyi
--rw-r--r--   0        0        0     1017 2023-01-16 00:27:03.189532 micropython_rp2_stubs-1.19.1.post9/uarray.pyi
--rw-r--r--   0        0        0      125 2023-01-16 00:27:03.181532 micropython_rp2_stubs-1.19.1.post9/uasyncio/__init__.pyi
--rw-r--r--   0        0        0     1478 2023-01-16 00:27:03.181532 micropython_rp2_stubs-1.19.1.post9/uasyncio/core.pyi
--rw-r--r--   0        0        0      577 2023-01-16 00:27:03.181532 micropython_rp2_stubs-1.19.1.post9/uasyncio/event.pyi
--rw-r--r--   0        0        0      377 2023-01-16 00:27:03.181532 micropython_rp2_stubs-1.19.1.post9/uasyncio/funcs.pyi
--rw-r--r--   0        0        0      407 2023-01-16 00:27:03.181532 micropython_rp2_stubs-1.19.1.post9/uasyncio/lock.pyi
--rw-r--r--   0        0        0     1394 2023-01-16 00:27:03.181532 micropython_rp2_stubs-1.19.1.post9/uasyncio/stream.pyi
--rw-r--r--   0        0        0      760 2023-01-16 00:27:03.181532 micropython_rp2_stubs-1.19.1.post9/uasyncio/task.pyi
--rw-r--r--   0        0        0     1365 2023-01-16 00:27:03.189532 micropython_rp2_stubs-1.19.1.post9/ubinascii.pyi
--rw-r--r--   0        0        0    33322 2023-01-16 00:27:03.189532 micropython_rp2_stubs-1.19.1.post9/ubluetooth.pyi
--rw-r--r--   0        0        0     3526 2023-01-16 00:27:03.189532 micropython_rp2_stubs-1.19.1.post9/ucollections.pyi
--rw-r--r--   0        0        0     1608 2023-01-16 00:27:03.189532 micropython_rp2_stubs-1.19.1.post9/ucryptolib.pyi
--rw-r--r--   0        0        0     2277 2023-01-16 00:27:03.189532 micropython_rp2_stubs-1.19.1.post9/uctypes.pyi
--rw-r--r--   0        0        0      676 2023-01-16 00:27:03.189532 micropython_rp2_stubs-1.19.1.post9/uerrno.pyi
--rw-r--r--   0        0        0     1600 2023-01-16 00:27:03.189532 micropython_rp2_stubs-1.19.1.post9/uhashlib.pyi
--rw-r--r--   0        0        0      897 2023-01-16 00:27:03.189532 micropython_rp2_stubs-1.19.1.post9/uheapq.pyi
--rw-r--r--   0        0        0     3914 2023-01-16 00:27:03.189532 micropython_rp2_stubs-1.19.1.post9/uio.pyi
--rw-r--r--   0        0        0     1339 2023-01-16 00:27:03.189532 micropython_rp2_stubs-1.19.1.post9/ujson.pyi
--rw-r--r--   0        0        0    43609 2023-01-16 00:27:03.189532 micropython_rp2_stubs-1.19.1.post9/umachine.pyi
--rw-r--r--   0        0        0     9063 2023-01-16 00:27:03.189532 micropython_rp2_stubs-1.19.1.post9/uos.pyi
--rw-r--r--   0        0        0     2553 2023-01-16 00:27:03.189532 micropython_rp2_stubs-1.19.1.post9/urandom.pyi
--rw-r--r--   0        0        0      181 2023-01-16 00:27:03.189532 micropython_rp2_stubs-1.19.1.post9/ure.pyi
--rw-r--r--   0        0        0     3760 2023-01-16 00:27:03.189532 micropython_rp2_stubs-1.19.1.post9/uselect.pyi
--rw-r--r--   0        0        0     9304 2023-01-16 00:27:03.189532 micropython_rp2_stubs-1.19.1.post9/usocket.pyi
--rw-r--r--   0        0        0     1521 2023-01-16 00:27:03.189532 micropython_rp2_stubs-1.19.1.post9/ustruct.pyi
--rw-r--r--   0        0        0      838 2023-01-16 00:27:03.189532 micropython_rp2_stubs-1.19.1.post9/usys.pyi
--rw-r--r--   0        0        0    12180 2023-01-16 00:27:03.189532 micropython_rp2_stubs-1.19.1.post9/utime.pyi
--rw-r--r--   0        0        0      393 2023-01-16 00:27:03.189532 micropython_rp2_stubs-1.19.1.post9/uwebsocket.pyi
--rw-r--r--   0        0        0     1503 2023-01-16 00:27:03.189532 micropython_rp2_stubs-1.19.1.post9/uzlib.pyi
--rw-r--r--   0        0        0      393 2023-01-16 00:27:03.189532 micropython_rp2_stubs-1.19.1.post9/websocket.pyi
--rw-r--r--   0        0        0      136 2023-01-16 00:27:03.189532 micropython_rp2_stubs-1.19.1.post9/websocket_helper.pyi
--rw-r--r--   0        0        0     1503 2023-01-16 00:27:03.189532 micropython_rp2_stubs-1.19.1.post9/zlib.pyi
--rw-r--r--   0        0        0     3491 1970-01-01 00:00:00.000000 micropython_rp2_stubs-1.19.1.post9/setup.py
--rw-r--r--   0        0        0     3322 1970-01-01 00:00:00.000000 micropython_rp2_stubs-1.19.1.post9/PKG-INFO
+-rw-r--r--   0        0        0       71 2023-05-05 19:50:30.223053 micropython_rp2_stubs-1.20.0.post1/_boot.pyi
+-rw-r--r--   0        0        0       71 2023-05-05 19:50:30.228827 micropython_rp2_stubs-1.20.0.post1/_boot_fat.pyi
+-rw-r--r--   0        0        0      277 2023-05-04 20:38:22.139418 micropython_rp2_stubs-1.20.0.post1/_onewire.pyi
+-rw-r--r--   0        0        0     1364 2023-05-04 20:38:22.142263 micropython_rp2_stubs-1.20.0.post1/_rp2.pyi
+-rw-r--r--   0        0        0      848 2023-05-06 19:31:08.775982 micropython_rp2_stubs-1.20.0.post1/_thread.pyi
+-rw-r--r--   0        0        0      364 2023-05-04 20:38:22.145609 micropython_rp2_stubs-1.20.0.post1/_uasyncio.pyi
+-rw-r--r--   0        0        0     1003 2023-05-06 19:31:28.979362 micropython_rp2_stubs-1.20.0.post1/array.pyi
+-rw-r--r--   0        0        0     1408 2023-05-06 19:31:29.028068 micropython_rp2_stubs-1.20.0.post1/binascii.pyi
+-rw-r--r--   0        0        0     1454 2023-05-06 19:31:29.036316 micropython_rp2_stubs-1.20.0.post1/cmath.pyi
+-rw-r--r--   0        0        0     3640 2023-05-06 19:31:29.070228 micropython_rp2_stubs-1.20.0.post1/collections.pyi
+-rw-r--r--   0        0        0     1647 2023-05-06 19:31:10.219404 micropython_rp2_stubs-1.20.0.post1/cryptolib.pyi
+-rw-r--r--   0        0        0      344 2023-05-05 19:50:30.231380 micropython_rp2_stubs-1.20.0.post1/dht.pyi
+-rw-r--r--   0        0        0      404 2023-05-05 19:50:30.236017 micropython_rp2_stubs-1.20.0.post1/ds18x20.pyi
+-rw-r--r--   0        0        0      709 2023-05-06 19:31:10.498012 micropython_rp2_stubs-1.20.0.post1/errno.pyi
+-rw-r--r--   0        0        0     6349 2023-05-06 19:31:29.178071 micropython_rp2_stubs-1.20.0.post1/framebuf.pyi
+-rw-r--r--   0        0        0     1993 2023-05-06 19:31:29.162414 micropython_rp2_stubs-1.20.0.post1/gc.pyi
+-rw-r--r--   0        0        0     1642 2023-05-06 19:31:29.148884 micropython_rp2_stubs-1.20.0.post1/hashlib.pyi
+-rw-r--r--   0        0        0      930 2023-05-06 19:31:29.162414 micropython_rp2_stubs-1.20.0.post1/heapq.pyi
+-rw-r--r--   0        0        0     2471 2023-05-06 19:31:29.232670 micropython_rp2_stubs-1.20.0.post1/io.pyi
+-rw-r--r--   0        0        0     1384 2023-05-06 19:31:29.196570 micropython_rp2_stubs-1.20.0.post1/json.pyi
+-rw-r--r--   0        0        0     1092 2023-05-06 19:32:46.063067 micropython_rp2_stubs-1.20.0.post1/LICENSE.md
+-rw-r--r--   0        0        0      827 2023-05-04 20:38:22.175385 micropython_rp2_stubs-1.20.0.post1/logging.pyi
+-rw-r--r--   0        0        0    49175 2023-05-06 19:31:32.586145 micropython_rp2_stubs-1.20.0.post1/machine.pyi
+-rw-r--r--   0        0        0     4654 2023-05-06 19:31:29.337117 micropython_rp2_stubs-1.20.0.post1/math.pyi
+-rw-r--r--   0        0        0     7213 2023-04-05 11:07:45.360315 micropython_rp2_stubs-1.20.0.post1/micropython.pyi
+-rw-r--r--   0        0        0      448 2023-05-05 19:50:30.240555 micropython_rp2_stubs-1.20.0.post1/neopixel.pyi
+-rw-r--r--   0        0        0      617 2023-05-05 19:50:30.243943 micropython_rp2_stubs-1.20.0.post1/onewire.pyi
+-rw-r--r--   0        0        0     9307 2023-05-06 19:31:29.445220 micropython_rp2_stubs-1.20.0.post1/os.pyi
+-rw-r--r--   0        0        0     3180 2023-05-06 19:32:48.385750 micropython_rp2_stubs-1.20.0.post1/pyproject.toml
+-rw-r--r--   0        0        0     2638 2023-05-06 19:31:29.306217 micropython_rp2_stubs-1.20.0.post1/random.pyi
+-rw-r--r--   0        0        0     2003 2023-05-06 19:32:46.063067 micropython_rp2_stubs-1.20.0.post1/readme.md
+-rw-r--r--   0        0        0     1918 2023-05-05 19:52:04.734802 micropython_rp2_stubs-1.20.0.post1/rp2.pyi
+-rw-r--r--   0        0        0     3853 2023-05-06 19:31:18.024304 micropython_rp2_stubs-1.20.0.post1/select.pyi
+-rw-r--r--   0        0        0     4241 2023-05-06 19:31:29.468848 micropython_rp2_stubs-1.20.0.post1/struct.pyi
+-rw-r--r--   0        0        0      875 2023-05-06 19:31:29.468848 micropython_rp2_stubs-1.20.0.post1/sys.pyi
+-rw-r--r--   0        0        0    12515 2023-05-06 19:31:29.528505 micropython_rp2_stubs-1.20.0.post1/time.pyi
+-rw-r--r--   0        0        0     1003 2023-05-06 19:31:29.496080 micropython_rp2_stubs-1.20.0.post1/uarray.pyi
+-rw-r--r--   0        0        0      132 2023-05-05 19:50:30.186763 micropython_rp2_stubs-1.20.0.post1/uasyncio/__init__.pyi
+-rw-r--r--   0        0        0     1530 2023-05-05 19:50:30.194578 micropython_rp2_stubs-1.20.0.post1/uasyncio/core.pyi
+-rw-r--r--   0        0        0      625 2023-05-05 19:50:30.202589 micropython_rp2_stubs-1.20.0.post1/uasyncio/event.pyi
+-rw-r--r--   0        0        0      390 2023-05-05 19:50:30.205342 micropython_rp2_stubs-1.20.0.post1/uasyncio/funcs.pyi
+-rw-r--r--   0        0        0      414 2023-05-05 19:50:30.209858 micropython_rp2_stubs-1.20.0.post1/uasyncio/lock.pyi
+-rw-r--r--   0        0        0     1410 2023-05-05 19:52:04.843701 micropython_rp2_stubs-1.20.0.post1/uasyncio/stream.pyi
+-rw-r--r--   0        0        0      789 2023-05-05 19:50:30.218200 micropython_rp2_stubs-1.20.0.post1/uasyncio/task.pyi
+-rw-r--r--   0        0        0     1408 2023-05-06 19:31:29.559741 micropython_rp2_stubs-1.20.0.post1/ubinascii.pyi
+-rw-r--r--   0        0        0     3640 2023-05-06 19:31:29.607599 micropython_rp2_stubs-1.20.0.post1/ucollections.pyi
+-rw-r--r--   0        0        0     1647 2023-05-06 19:31:19.786605 micropython_rp2_stubs-1.20.0.post1/ucryptolib.pyi
+-rw-r--r--   0        0        0     2363 2023-05-06 19:31:29.652409 micropython_rp2_stubs-1.20.0.post1/uctypes.pyi
+-rw-r--r--   0        0        0      709 2023-05-06 19:31:20.411045 micropython_rp2_stubs-1.20.0.post1/uerrno.pyi
+-rw-r--r--   0        0        0     1642 2023-05-06 19:31:29.642242 micropython_rp2_stubs-1.20.0.post1/uhashlib.pyi
+-rw-r--r--   0        0        0      930 2023-05-06 19:31:29.656272 micropython_rp2_stubs-1.20.0.post1/uheapq.pyi
+-rw-r--r--   0        0        0     2471 2023-05-06 19:31:29.734546 micropython_rp2_stubs-1.20.0.post1/uio.pyi
+-rw-r--r--   0        0        0     1384 2023-05-06 19:31:29.687133 micropython_rp2_stubs-1.20.0.post1/ujson.pyi
+-rw-r--r--   0        0        0    49175 2023-05-06 19:31:35.124603 micropython_rp2_stubs-1.20.0.post1/umachine.pyi
+-rw-r--r--   0        0        0     9307 2023-05-06 19:31:29.832384 micropython_rp2_stubs-1.20.0.post1/uos.pyi
+-rw-r--r--   0        0        0     2638 2023-05-06 19:31:29.749565 micropython_rp2_stubs-1.20.0.post1/urandom.pyi
+-rw-r--r--   0        0        0      187 2023-05-04 20:38:22.241008 micropython_rp2_stubs-1.20.0.post1/ure.pyi
+-rw-r--r--   0        0        0     3853 2023-05-06 19:31:25.283656 micropython_rp2_stubs-1.20.0.post1/uselect.pyi
+-rw-r--r--   0        0        0     4241 2023-05-06 19:31:29.765396 micropython_rp2_stubs-1.20.0.post1/ustruct.pyi
+-rw-r--r--   0        0        0      875 2023-05-06 19:31:29.798104 micropython_rp2_stubs-1.20.0.post1/usys.pyi
+-rw-r--r--   0        0        0    12515 2023-05-06 19:31:29.860844 micropython_rp2_stubs-1.20.0.post1/utime.pyi
+-rw-r--r--   0        0        0     1535 2023-05-06 19:31:29.829832 micropython_rp2_stubs-1.20.0.post1/uzlib.pyi
+-rw-r--r--   0        0        0     1535 2023-05-06 19:31:29.860844 micropython_rp2_stubs-1.20.0.post1/zlib.pyi
+-rw-r--r--   0        0        0     3286 1970-01-01 00:00:00.000000 micropython_rp2_stubs-1.20.0.post1/setup.py
+-rw-r--r--   0        0        0     3252 1970-01-01 00:00:00.000000 micropython_rp2_stubs-1.20.0.post1/PKG-INFO
```

### Comparing `micropython_rp2_stubs-1.19.1.post9/README.md` & `micropython_rp2_stubs-1.20.0.post1/readme.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,38 @@
-# micropython-rp2-stubs
-
-
-This is a stub-only package for MicroPython.
-It is intended to be installed in a projects virtual environment to allow static type checkers and intellisense features to be used while writing Micropython code.
-
-The version of this package is alligned the the version of the MicroPython firmware.
- - Major, Minor and Patch levels are alligned to the same version as the firmware.  
- - The post release level is used to publish new releases of the stubs.
-
-For `Micropython 1.17` the stubs are published as `1.17.post1` ... `1.17.post2`  
-for `Micropython 1.18` the stubs are published as `1.18.post1` ... `1.18.post2`  
-
-To install the latest stubs:  
-`pip install -I  micropython-<port>-stubs` where port is the port of the MicroPython firmware.
-
-To install the stubs for an older version, such as MicroPython 1.17:  
-`pip install micropython-stm32-stubs==1.17.*` which will install the last post release of the stubs for MicroPython 1.17.
-
-
-As the creation of the stubs, and merging of the different types is still going though improvements, the stub packages are marked as Beta.
-To upgrade stubs to the latest stubs for a specific version use `pip install micropython-stm32-stubs==1.17.* --upgrade`
-
-If you have suggestions or find any issues with the stubs, please report them in the [MicroPython-stubs Discussions](https://github.com/Josverl/micropython-stubs/discussions)
-
-For an overview of  Micropython Stubs please see: https://micropython-stubs.readthedocs.io/en/main/ 
- * List of all stubs : https://micropython-stubs.readthedocs.io/en/main/firmware_grp.html
-
-Included stubs:
-* Merged stubs from `stubs/micropython-v1_19_1-rp2-merged`
-* Frozen stubs from `stubs/micropython-v1_19_1-frozen/rp2/GENERIC`
-* Core stubs from `stubs/cpython_core-pycopy`
-
-
-origin | Family | Port | Board | Version
--------|--------|------|-------|--------
-Firmware | micropython | rp2 | Arduino Nano RP2040 Connect with RP2040 | v1.19.1 
-Documentation | micropython | - | - | v1.19.1 
-Core | micropython | rp2 | - | v1.19.1 
+# micropython-rp2-stubs
+
+
+This is a stub-only package for MicroPython.
+It is intended to be installed in a projects virtual environment to allow static type checkers and intellisense features to be used while writing Micropython code.
+
+The version of this package is alligned the the version of the MicroPython firmware.
+ - Major, Minor and Patch levels are alligned to the same version as the firmware.  
+ - The post release level is used to publish new releases of the stubs.
+
+For `Micropython 1.17` the stubs are published as `1.17.post1` ... `1.17.post2`  
+for `Micropython 1.18` the stubs are published as `1.18.post1` ... `1.18.post2`  
+
+To install the latest stubs:  
+`pip install -I  micropython-<port>-stubs` where port is the port of the MicroPython firmware.
+
+To install the stubs for an older version, such as MicroPython 1.17:  
+`pip install micropython-stm32-stubs==1.17.*` which will install the last post release of the stubs for MicroPython 1.17.
+
+
+As the creation of the stubs, and merging of the different types is still going though improvements, the stub packages are marked as Beta.
+To upgrade stubs to the latest stubs for a specific version use `pip install micropython-stm32-stubs==1.17.* --upgrade`
+
+If you have suggestions or find any issues with the stubs, please report them in the [MicroPython-stubs Discussions](https://github.com/Josverl/micropython-stubs/discussions)
+
+For an overview of  Micropython Stubs please see: https://micropython-stubs.readthedocs.io/en/main/ 
+ * List of all stubs : https://micropython-stubs.readthedocs.io/en/main/firmware_grp.html
+
+Included stubs:
+* StubSource.MERGED from `stubs/micropython-v1_20_0-rp2-merged`
+* StubSource.FROZEN from `stubs/micropython-v1_20_0-frozen/rp2/GENERIC`
+* StubSource.CORE from `stubs/micropython-core`
+
+
+origin | Family | Port | Board | Version
+-------|--------|------|-------|--------
+Documentation | micropython | - | - | v1.20.0 
+Core | micropython | rp2 | - | v1.20.0
```

### Comparing `micropython_rp2_stubs-1.19.1.post9/_rp2.pyi` & `micropython_rp2_stubs-1.20.0.post1/_rp2.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -1,41 +1,41 @@
-from typing import Any
-
-def dht_readinto(*args, **kwargs) -> Any: ...
-
-class StateMachine:
-    def irq(self, *args, **kwargs) -> Any: ...
-    def put(self, *args, **kwargs) -> Any: ...
-    def restart(self, *args, **kwargs) -> Any: ...
-    def rx_fifo(self, *args, **kwargs) -> Any: ...
-    def tx_fifo(self, *args, **kwargs) -> Any: ...
-    def init(self, *args, **kwargs) -> Any: ...
-    def exec(self, *args, **kwargs) -> Any: ...
-    def get(self, *args, **kwargs) -> Any: ...
-    def active(self, *args, **kwargs) -> Any: ...
-    def __init__(self, *argv, **kwargs) -> None: ...
-
-class Flash:
-    def readblocks(self, *args, **kwargs) -> Any: ...
-    def writeblocks(self, *args, **kwargs) -> Any: ...
-    def ioctl(self, *args, **kwargs) -> Any: ...
-    def __init__(self, *argv, **kwargs) -> None: ...
-
-class PIO:
-    JOIN_TX: int
-    JOIN_NONE: int
-    JOIN_RX: int
-    SHIFT_LEFT: int
-    OUT_HIGH: int
-    OUT_LOW: int
-    SHIFT_RIGHT: int
-    IN_LOW: int
-    IRQ_SM3: int
-    IN_HIGH: int
-    IRQ_SM2: int
-    IRQ_SM0: int
-    IRQ_SM1: int
-    def state_machine(self, *args, **kwargs) -> Any: ...
-    def remove_program(self, *args, **kwargs) -> Any: ...
-    def irq(self, *args, **kwargs) -> Any: ...
-    def add_program(self, *args, **kwargs) -> Any: ...
-    def __init__(self, *argv, **kwargs) -> None: ...
+from typing import Any
+
+def bootsel_button(*args, **kwargs) -> Any: ...
+
+class StateMachine:
+    def irq(self, *args, **kwargs) -> Any: ...
+    def put(self, *args, **kwargs) -> Any: ...
+    def restart(self, *args, **kwargs) -> Any: ...
+    def rx_fifo(self, *args, **kwargs) -> Any: ...
+    def tx_fifo(self, *args, **kwargs) -> Any: ...
+    def init(self, *args, **kwargs) -> Any: ...
+    def exec(self, *args, **kwargs) -> Any: ...
+    def get(self, *args, **kwargs) -> Any: ...
+    def active(self, *args, **kwargs) -> Any: ...
+    def __init__(self, *argv, **kwargs) -> None: ...
+
+class Flash:
+    def readblocks(self, *args, **kwargs) -> Any: ...
+    def writeblocks(self, *args, **kwargs) -> Any: ...
+    def ioctl(self, *args, **kwargs) -> Any: ...
+    def __init__(self, *argv, **kwargs) -> None: ...
+
+class PIO:
+    JOIN_TX: int
+    JOIN_NONE: int
+    JOIN_RX: int
+    SHIFT_LEFT: int
+    OUT_HIGH: int
+    OUT_LOW: int
+    SHIFT_RIGHT: int
+    IN_LOW: int
+    IRQ_SM3: int
+    IN_HIGH: int
+    IRQ_SM2: int
+    IRQ_SM0: int
+    IRQ_SM1: int
+    def state_machine(self, *args, **kwargs) -> Any: ...
+    def remove_program(self, *args, **kwargs) -> Any: ...
+    def irq(self, *args, **kwargs) -> Any: ...
+    def add_program(self, *args, **kwargs) -> Any: ...
+    def __init__(self, *argv, **kwargs) -> None: ...
```

### Comparing `micropython_rp2_stubs-1.19.1.post9/aioble/central.pyi` & `micropython_rp2_stubs-1.20.0.post1/logging.pyi`

 * *Files 26% similar despite different names*

```diff
@@ -1,42 +1,26 @@
-from typing import Any
-
-def log_info(*args, **kwargs) -> Any: ...
-def log_warn(*args, **kwargs) -> Any: ...
-def log_error(*args, **kwargs) -> Any: ...
-def ensure_active(*args, **kwargs) -> Any: ...
-def register_irq_handler(*args, **kwargs) -> Any: ...
-def const(*args, **kwargs) -> Any: ...
-
-ble: Any
-
-class DeviceTimeout:
-    def __init__(self, *argv, **kwargs) -> None: ...
-
-class DeviceConnection:
-    def timeout(self, *args, **kwargs) -> Any: ...
-    def services(self, *args, **kwargs) -> Any: ...
-    def is_connected(self, *args, **kwargs) -> Any: ...
-    service: Any
-    pair: Any
-    exchange_mtu: Any
-    l2cap_accept: Any
-    disconnected: Any
-    disconnect: Any
-    l2cap_connect: Any
-    device_task: Any
-    def __init__(self, *argv, **kwargs) -> None: ...
-
-class ScanResult:
-    def name(self, *args, **kwargs) -> Any: ...
-    manufacturer: Any
-    services: Any
-    def __init__(self, *argv, **kwargs) -> None: ...
-
-class scan:
-    cancel: Any
-    def __init__(self, *argv, **kwargs) -> None: ...
-
-class Device:
-    def addr_hex(self, *args, **kwargs) -> Any: ...
-    connect: Any
-    def __init__(self, *argv, **kwargs) -> None: ...
+from typing import Any
+
+CRITICAL: int
+INFO: int
+DEBUG: int
+ERROR: int
+WARNING: int
+NOTSET: int
+
+def getLogger(*args, **kwargs) -> Any: ...
+def basicConfig(*args, **kwargs) -> Any: ...
+def info(*args, **kwargs) -> Any: ...
+def debug(*args, **kwargs) -> Any: ...
+
+class Logger:
+    level: int
+    def warning(self, *args, **kwargs) -> Any: ...
+    def critical(self, *args, **kwargs) -> Any: ...
+    def setLevel(self, *args, **kwargs) -> Any: ...
+    def isEnabledFor(self, *args, **kwargs) -> Any: ...
+    def exception(self, *args, **kwargs) -> Any: ...
+    def log(self, *args, **kwargs) -> Any: ...
+    def error(self, *args, **kwargs) -> Any: ...
+    def info(self, *args, **kwargs) -> Any: ...
+    def debug(self, *args, **kwargs) -> Any: ...
+    def __init__(self, *argv, **kwargs) -> None: ...
```

### Comparing `micropython_rp2_stubs-1.19.1.post9/array.pyi` & `micropython_rp2_stubs-1.20.0.post1/array.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,30 @@
-"""
-efficient arrays of numeric data. See: https://docs.micropython.org/en/v1.19.1/library/array.html
-
-|see_cpython_module| :mod:`python:array` https://docs.python.org/3/library/array.html .
-
-Supported format codes: ``b``, ``B``, ``h``, ``H``, ``i``, ``I``, ``l``,
-``L``, ``q``, ``Q``, ``f``, ``d`` (the latter 2 depending on the
-floating-point support).
-"""
-from typing import Optional, Any
-
-class array:
-    """
-    Create array with elements of given type. Initial contents of the
-    array are given by *iterable*. If it is not provided, an empty
-    array is created.
-    """
-
-    def extend(self, iterable) -> Any:
-        """
-        Append new elements as contained in *iterable* to the end of
-        array, growing it.
-        """
-        ...
-    def decode(self, *args, **kwargs) -> Any: ...
-    def append(self, val) -> Any:
-        """
-        Append new element *val* to the end of array, growing it.
-        """
-        ...
-    def __init__(self, typecode, iterable: Optional[Any] = None) -> None: ...
+"""
+efficient arrays of numeric data. See: https://docs.micropython.org/en/v1.20.0/library/array.html
+
+|see_cpython_module| :mod:`python:array` https://docs.python.org/3/library/array.html .
+
+Supported format codes: ``b``, ``B``, ``h``, ``H``, ``i``, ``I``, ``l``,
+``L``, ``q``, ``Q``, ``f``, ``d`` (the latter 2 depending on the
+floating-point support).
+"""
+from typing import List, Optional, Any
+
+class array:
+    """
+    Create array with elements of given type. Initial contents of the
+    array are given by *iterable*. If it is not provided, an empty
+    array is created.
+    """
+
+    def extend(self, iterable) -> Any:
+        """
+        Append new elements as contained in *iterable* to the end of
+        array, growing it.
+        """
+        ...
+    def append(self, val) -> Any:
+        """
+        Append new element *val* to the end of array, growing it.
+        """
+        ...
+    def __init__(self, typecode, iterable: Optional[Any] = None) -> None: ...
```

### Comparing `micropython_rp2_stubs-1.19.1.post9/binascii.pyi` & `micropython_rp2_stubs-1.20.0.post1/binascii.pyi`

 * *Files 13% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-"""
-binary/ASCII conversions. See: https://docs.micropython.org/en/v1.19.1/library/binascii.html
-
-|see_cpython_module| :mod:`python:binascii` https://docs.python.org/3/library/binascii.html .
-
-This module implements conversions between binary data and various
-encodings of it in ASCII form (in both directions).
-"""
-from typing import Optional, Any
-
-def crc32(*args, **kwargs) -> Any: ...
-def hexlify(data, sep: Optional[Any] = None) -> bytes:
-    """
-    Convert the bytes in the *data* object to a hexadecimal representation.
-    Returns a bytes object.
-
-    If the additional argument *sep* is supplied it is used as a separator
-    between hexadecimal values.
-    """
-    ...
-
-def unhexlify(data) -> bytes:
-    """
-    Convert hexadecimal data to binary representation. Returns bytes string.
-    (i.e. inverse of hexlify)
-    """
-    ...
-
-def b2a_base64(data, *, newline=True) -> bytes:
-    """
-    Encode binary data in base64 format, as in `RFC 3548
-    <https://tools.ietf.org/html/rfc3548.html>`_. Returns the encoded data
-    followed by a newline character if newline is true, as a bytes object.
-    """
-    ...
-
-def a2b_base64(data) -> bytes:
-    """
-    Decode base64-encoded data, ignoring invalid characters in the input.
-    Conforms to `RFC 2045 s.6.8 <https://tools.ietf.org/html/rfc2045#section-6.8>`_.
-    Returns a bytes object.
-    """
-    ...
+"""
+binary/ASCII conversions. See: https://docs.micropython.org/en/v1.20.0/library/binascii.html
+
+|see_cpython_module| :mod:`python:binascii` https://docs.python.org/3/library/binascii.html .
+
+This module implements conversions between binary data and various
+encodings of it in ASCII form (in both directions).
+"""
+from typing import Optional, Any
+
+def crc32(*args, **kwargs) -> Any: ...
+def hexlify(data, sep: Optional[Any] = None) -> bytes:
+    """
+    Convert the bytes in the *data* object to a hexadecimal representation.
+    Returns a bytes object.
+
+    If the additional argument *sep* is supplied it is used as a separator
+    between hexadecimal values.
+    """
+    ...
+
+def unhexlify(data) -> bytes:
+    """
+    Convert hexadecimal data to binary representation. Returns bytes string.
+    (i.e. inverse of hexlify)
+    """
+    ...
+
+def b2a_base64(data, *, newline=True) -> bytes:
+    """
+    Encode binary data in base64 format, as in `RFC 3548
+    <https://tools.ietf.org/html/rfc3548.html>`_. Returns the encoded data
+    followed by a newline character if newline is true, as a bytes object.
+    """
+    ...
+
+def a2b_base64(data) -> bytes:
+    """
+    Decode base64-encoded data, ignoring invalid characters in the input.
+    Conforms to `RFC 2045 s.6.8 <https://tools.ietf.org/html/rfc2045#section-6.8>`_.
+    Returns a bytes object.
+    """
+    ...
```

### Comparing `micropython_rp2_stubs-1.19.1.post9/framebuf.pyi` & `micropython_rp2_stubs-1.20.0.post1/framebuf.pyi`

 * *Files 23% similar despite different names*

```diff
@@ -1,110 +1,140 @@
-"""
-Frame buffer manipulation. See: https://docs.micropython.org/en/v1.19.1/library/framebuf.html
-
-This module provides a general frame buffer which can be used to create
-bitmap images, which can then be sent to a display.
-"""
-from typing import Optional, Any
-
-MONO_HMSB: int
-MONO_HLSB: int
-RGB565: int
-MONO_VLSB: int
-MVLSB: int
-GS2_HMSB: int
-GS8: int
-GS4_HMSB: int
-
-def FrameBuffer1(*args, **kwargs) -> Any: ...
-
-class FrameBuffer:
-    """
-    Construct a FrameBuffer object.  The parameters are:
-
-        - *buffer* is an object with a buffer protocol which must be large
-          enough to contain every pixel defined by the width, height and
-          format of the FrameBuffer.
-        - *width* is the width of the FrameBuffer in pixels
-        - *height* is the height of the FrameBuffer in pixels
-        - *format* specifies the type of pixel used in the FrameBuffer;
-          permissible values are listed under Constants below. These set the
-          number of bits used to encode a color value and the layout of these
-          bits in *buffer*.
-          Where a color value c is passed to a method, c is a small integer
-          with an encoding that is dependent on the format of the FrameBuffer.
-        - *stride* is the number of pixels between each horizontal line
-          of pixels in the FrameBuffer. This defaults to *width* but may
-          need adjustments when implementing a FrameBuffer within another
-          larger FrameBuffer or screen. The *buffer* size must accommodate
-          an increased step size.
-
-    One must specify valid *buffer*, *width*, *height*, *format* and
-    optionally *stride*.  Invalid *buffer* size or dimensions may lead to
-    unexpected errors.
-    """
-
-    def rect(self, x, y, w, h, c) -> Any: ...
-    def pixel(self, x, y, c: Optional[Any] = None) -> Any:
-        """
-        If *c* is not given, get the color value of the specified pixel.
-        If *c* is given, set the specified pixel to the given color.
-        """
-        ...
-    def vline(self, x, y, h, c) -> Any: ...
-    def scroll(self, xstep, ystep) -> Any:
-        """
-        Shift the contents of the FrameBuffer by the given vector. This may
-        leave a footprint of the previous colors in the FrameBuffer.
-        """
-        ...
-    def text(self, s, x, y, c: Optional[Any] = None) -> None:
-        """
-        Write text to the FrameBuffer using the the coordinates as the upper-left
-        corner of the text. The color of the text can be defined by the optional
-        argument but is otherwise a default value of 1. All characters have
-        dimensions of 8x8 pixels and there is currently no way to change the font.
-
-        """
-        ...
-    def fill(self, c) -> None:
-        """
-        Fill the entire FrameBuffer with the specified color.
-        """
-        ...
-    def blit(self, fbuf, x, y, key=-1, palette=None) -> None:
-        """
-        Draw another FrameBuffer on top of the current one at the given coordinates.
-        If *key* is specified then it should be a color integer and the
-        corresponding color will be considered transparent: all pixels with that
-        color value will not be drawn.
-
-        The *palette* argument enables blitting between FrameBuffers with differing
-        formats. Typical usage is to render a monochrome or grayscale glyph/icon to
-        a color display. The *palette* is a FrameBuffer instance whose format is
-        that of the current FrameBuffer. The *palette* height is one pixel and its
-        pixel width is the number of colors in the source FrameBuffer. The *palette*
-        for an N-bit source needs 2**N pixels; the *palette* for a monochrome source
-        would have 2 pixels representing background and foreground colors. The
-        application assigns a color to each pixel in the *palette*. The color of the
-        current pixel will be that of that *palette* pixel whose x position is the
-        color of the corresponding source pixel.
-        """
-        ...
-    def line(self, x1, y1, x2, y2, c) -> None:
-        """
-        Draw a line from a set of coordinates using the given color and
-        a thickness of 1 pixel. The `line` method draws the line up to
-        a second set of coordinates whereas the `hline` and `vline`
-        methods draw horizontal and vertical lines respectively up to
-        a given length.
-        """
-        ...
-    def fill_rect(self, x, y, w, h, c) -> None:
-        """
-        Draw a rectangle at the given location, size and color. The `rect`
-        method draws only a 1 pixel outline whereas the `fill_rect` method
-        draws both the outline and interior.
-        """
-        ...
-    def hline(self, x, y, w, c) -> Any: ...
-    def __init__(self, buffer, width, height, format, stride=-1, /) -> None: ...
+"""
+Frame buffer manipulation. See: https://docs.micropython.org/en/v1.20.0/library/framebuf.html
+
+This module provides a general frame buffer which can be used to create
+bitmap images, which can then be sent to a display.
+"""
+from typing import Optional, Any
+
+MONO_HMSB: int
+MONO_HLSB: int
+RGB565: int
+MONO_VLSB: int
+MVLSB: int
+GS2_HMSB: int
+GS8: int
+GS4_HMSB: int
+
+def FrameBuffer1(*args, **kwargs) -> Any: ...
+
+class FrameBuffer:
+    """
+    Construct a FrameBuffer object.  The parameters are:
+
+        - *buffer* is an object with a buffer protocol which must be large
+          enough to contain every pixel defined by the width, height and
+          format of the FrameBuffer.
+        - *width* is the width of the FrameBuffer in pixels
+        - *height* is the height of the FrameBuffer in pixels
+        - *format* specifies the type of pixel used in the FrameBuffer;
+          permissible values are listed under Constants below. These set the
+          number of bits used to encode a color value and the layout of these
+          bits in *buffer*.
+          Where a color value c is passed to a method, c is a small integer
+          with an encoding that is dependent on the format of the FrameBuffer.
+        - *stride* is the number of pixels between each horizontal line
+          of pixels in the FrameBuffer. This defaults to *width* but may
+          need adjustments when implementing a FrameBuffer within another
+          larger FrameBuffer or screen. The *buffer* size must accommodate
+          an increased step size.
+
+    One must specify valid *buffer*, *width*, *height*, *format* and
+    optionally *stride*.  Invalid *buffer* size or dimensions may lead to
+    unexpected errors.
+    """
+
+    def poly(self, x, y, coords, c, f: Optional[Any] = None) -> Any:
+        """
+        Given a list of coordinates, draw an arbitrary (convex or concave) closed
+        polygon at the given x, y location using the given color.
+
+        The *coords* must be specified as a :mod:`array` of integers, e.g.
+        ``array('h', [x0, y0, x1, y1, ... xn, yn])``.
+
+        The optional *f* parameter can be set to ``True`` to fill the polygon.
+        Otherwise just a one pixel outline is drawn.
+        """
+        ...
+    def vline(self, x, y, h, c) -> Any: ...
+    def pixel(self, x, y, c: Optional[Any] = None) -> Any:
+        """
+        If *c* is not given, get the color value of the specified pixel.
+        If *c* is given, set the specified pixel to the given color.
+        """
+        ...
+    def text(self, s, x, y, c: Optional[Any] = None) -> None:
+        """
+        Write text to the FrameBuffer using the the coordinates as the upper-left
+        corner of the text. The color of the text can be defined by the optional
+        argument but is otherwise a default value of 1. All characters have
+        dimensions of 8x8 pixels and there is currently no way to change the font.
+
+        """
+        ...
+    def rect(self, x, y, w, h, c, f: Optional[Any] = None) -> None:
+        """
+        Draw a rectangle at the given location, size and color.
+
+        The optional *f* parameter can be set to ``True`` to fill the rectangle.
+        Otherwise just a one pixel outline is drawn.
+        """
+        ...
+    def scroll(self, xstep, ystep) -> Any:
+        """
+        Shift the contents of the FrameBuffer by the given vector. This may
+        leave a footprint of the previous colors in the FrameBuffer.
+        """
+        ...
+    def ellipse(self, x, y, xr, yr, c, f, m: Optional[Any] = None) -> None:
+        """
+        Draw an ellipse at the given location. Radii *xr* and *yr* define the
+        geometry; equal values cause a circle to be drawn. The *c* parameter
+        defines the color.
+
+        The optional *f* parameter can be set to ``True`` to fill the ellipse.
+        Otherwise just a one pixel outline is drawn.
+
+        The optional *m* parameter enables drawing to be restricted to certain
+        quadrants of the ellipse. The LS four bits determine which quadrants are
+        to be drawn, with bit 0 specifying Q1, b1 Q2, b2 Q3 and b3 Q4. Quadrants
+        are numbered counterclockwise with Q1 being top right.
+        """
+        ...
+    def line(self, x1, y1, x2, y2, c) -> None:
+        """
+        Draw a line from a set of coordinates using the given color and
+        a thickness of 1 pixel. The `line` method draws the line up to
+        a second set of coordinates whereas the `hline` and `vline`
+        methods draw horizontal and vertical lines respectively up to
+        a given length.
+        """
+        ...
+    def blit(self, fbuf, x, y, key=-1, palette=None) -> None:
+        """
+        Draw another FrameBuffer on top of the current one at the given coordinates.
+        If *key* is specified then it should be a color integer and the
+        corresponding color will be considered transparent: all pixels with that
+        color value will not be drawn. (If the *palette* is specified then the *key*
+        is compared to the value from *palette*, not to the value directly from
+        *fbuf*.)
+
+        The *palette* argument enables blitting between FrameBuffers with differing
+        formats. Typical usage is to render a monochrome or grayscale glyph/icon to
+        a color display. The *palette* is a FrameBuffer instance whose format is
+        that of the current FrameBuffer. The *palette* height is one pixel and its
+        pixel width is the number of colors in the source FrameBuffer. The *palette*
+        for an N-bit source needs 2**N pixels; the *palette* for a monochrome source
+        would have 2 pixels representing background and foreground colors. The
+        application assigns a color to each pixel in the *palette*. The color of the
+        current pixel will be that of that *palette* pixel whose x position is the
+        color of the corresponding source pixel.
+        """
+        ...
+    def hline(self, x, y, w, c) -> Any: ...
+    def fill(self, c) -> None:
+        """
+        Fill the entire FrameBuffer with the specified color.
+        """
+        ...
+    def fill_rect(self, *args, **kwargs) -> Any: ...
+    def __init__(self, buffer, width, height, format, stride=-1, /) -> None: ...
```

### Comparing `micropython_rp2_stubs-1.19.1.post9/gc.pyi` & `micropython_rp2_stubs-1.20.0.post1/gc.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -1,58 +1,58 @@
-"""
-control the garbage collector. See: https://docs.micropython.org/en/v1.19.1/library/gc.html
-
-|see_cpython_module| :mod:`python:gc` https://docs.python.org/3/library/gc.html .
-"""
-from typing import Optional, Any
-
-def mem_alloc() -> int:
-    """
-    Return the number of bytes of heap RAM that are allocated.
-    """
-    ...
-
-def isenabled(*args, **kwargs) -> Any: ...
-def mem_free() -> int:
-    """
-    Return the number of bytes of available heap RAM, or -1 if this amount
-    is not known.
-    """
-    ...
-
-def threshold(amount: Optional[Any] = None) -> Any:
-    """
-    Set or query the additional GC allocation threshold. Normally, a collection
-    is triggered only when a new allocation cannot be satisfied, i.e. on an
-    out-of-memory (OOM) condition. If this function is called, in addition to
-    OOM, a collection will be triggered each time after *amount* bytes have been
-    allocated (in total, since the previous time such an amount of bytes
-    have been allocated). *amount* is usually specified as less than the
-    full heap size, with the intention to trigger a collection earlier than when the
-    heap becomes exhausted, and in the hope that an early collection will prevent
-    excessive memory fragmentation. This is a heuristic measure, the effect
-    of which will vary from application to application, as well as
-    the optimal value of the *amount* parameter.
-
-    Calling the function without argument will return the current value of
-    the threshold. A value of -1 means a disabled allocation threshold.
-    """
-    ...
-
-def collect() -> None:
-    """
-    Run a garbage collection.
-    """
-    ...
-
-def enable() -> None:
-    """
-    Enable automatic garbage collection.
-    """
-    ...
-
-def disable() -> None:
-    """
-    Disable automatic garbage collection.  Heap memory can still be allocated,
-    and garbage collection can still be initiated manually using :meth:`gc.collect`.
-    """
-    ...
+"""
+control the garbage collector. See: https://docs.micropython.org/en/v1.20.0/library/gc.html
+
+|see_cpython_module| :mod:`python:gc` https://docs.python.org/3/library/gc.html .
+"""
+from typing import Optional, Any
+
+def mem_alloc() -> int:
+    """
+    Return the number of bytes of heap RAM that are allocated.
+    """
+    ...
+
+def isenabled(*args, **kwargs) -> Any: ...
+def mem_free() -> int:
+    """
+    Return the number of bytes of available heap RAM, or -1 if this amount
+    is not known.
+    """
+    ...
+
+def threshold(amount: Optional[Any] = None) -> Any:
+    """
+    Set or query the additional GC allocation threshold. Normally, a collection
+    is triggered only when a new allocation cannot be satisfied, i.e. on an
+    out-of-memory (OOM) condition. If this function is called, in addition to
+    OOM, a collection will be triggered each time after *amount* bytes have been
+    allocated (in total, since the previous time such an amount of bytes
+    have been allocated). *amount* is usually specified as less than the
+    full heap size, with the intention to trigger a collection earlier than when the
+    heap becomes exhausted, and in the hope that an early collection will prevent
+    excessive memory fragmentation. This is a heuristic measure, the effect
+    of which will vary from application to application, as well as
+    the optimal value of the *amount* parameter.
+
+    Calling the function without argument will return the current value of
+    the threshold. A value of -1 means a disabled allocation threshold.
+    """
+    ...
+
+def collect() -> None:
+    """
+    Run a garbage collection.
+    """
+    ...
+
+def enable() -> None:
+    """
+    Enable automatic garbage collection.
+    """
+    ...
+
+def disable() -> None:
+    """
+    Disable automatic garbage collection.  Heap memory can still be allocated,
+    and garbage collection can still be initiated manually using :meth:`gc.collect`.
+    """
+    ...
```

### Comparing `micropython_rp2_stubs-1.19.1.post9/hashlib.pyi` & `micropython_rp2_stubs-1.20.0.post1/hashlib.pyi`

 * *Files 13% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-"""
-hashing algorithms. See: https://docs.micropython.org/en/v1.19.1/library/hashlib.html
-
-|see_cpython_module| :mod:`python:hashlib` https://docs.python.org/3/library/hashlib.html .
-
-This module implements binary data hashing algorithms. The exact inventory
-of available algorithms depends on a board. Among the algorithms which may
-be implemented:
-
-* SHA256 - The current generation, modern hashing algorithm (of SHA2 series).
-  It is suitable for cryptographically-secure purposes. Included in the
-  MicroPython core and any board is recommended to provide this, unless
-  it has particular code size constraints.
-
-* SHA1 - A previous generation algorithm. Not recommended for new usages,
-  but SHA1 is a part of number of Internet standards and existing
-  applications, so boards targeting network connectivity and
-  interoperability will try to provide this.
-
-* MD5 - A legacy algorithm, not considered cryptographically secure. Only
-  selected boards, targeting interoperability with legacy applications,
-  will offer this.
-"""
-from typing import Optional, Any
-
-class sha256:
-    """
-    Create an SHA256 hasher object and optionally feed ``data`` into it.
-    """
-
-    def digest(self, *args, **kwargs) -> Any: ...
-    def update(self, *args, **kwargs) -> Any: ...
-    def __init__(self, data: Optional[Any] = None) -> None: ...
-
-class sha1:
-    """
-    Create an SHA1 hasher object and optionally feed ``data`` into it.
-    """
-
-    def digest(self, *args, **kwargs) -> Any: ...
-    def update(self, *args, **kwargs) -> Any: ...
-    def __init__(self, data: Optional[Any] = None) -> None: ...
+"""
+hashing algorithms. See: https://docs.micropython.org/en/v1.20.0/library/hashlib.html
+
+|see_cpython_module| :mod:`python:hashlib` https://docs.python.org/3/library/hashlib.html .
+
+This module implements binary data hashing algorithms. The exact inventory
+of available algorithms depends on a board. Among the algorithms which may
+be implemented:
+
+* SHA256 - The current generation, modern hashing algorithm (of SHA2 series).
+  It is suitable for cryptographically-secure purposes. Included in the
+  MicroPython core and any board is recommended to provide this, unless
+  it has particular code size constraints.
+
+* SHA1 - A previous generation algorithm. Not recommended for new usages,
+  but SHA1 is a part of number of Internet standards and existing
+  applications, so boards targeting network connectivity and
+  interoperability will try to provide this.
+
+* MD5 - A legacy algorithm, not considered cryptographically secure. Only
+  selected boards, targeting interoperability with legacy applications,
+  will offer this.
+"""
+from typing import Optional, Any
+
+class sha256:
+    """
+    Create an SHA256 hasher object and optionally feed ``data`` into it.
+    """
+
+    def digest(self, *args, **kwargs) -> Any: ...
+    def update(self, *args, **kwargs) -> Any: ...
+    def __init__(self, data: Optional[Any] = None) -> None: ...
+
+class sha1:
+    """
+    Create an SHA1 hasher object and optionally feed ``data`` into it.
+    """
+
+    def digest(self, *args, **kwargs) -> Any: ...
+    def update(self, *args, **kwargs) -> Any: ...
+    def __init__(self, data: Optional[Any] = None) -> None: ...
```

### Comparing `micropython_rp2_stubs-1.19.1.post9/heapq.pyi` & `micropython_rp2_stubs-1.20.0.post1/heapq.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-"""
-heap queue algorithm. See: https://docs.micropython.org/en/v1.19.1/library/heapq.html
-
-|see_cpython_module| :mod:`python:heapq` https://docs.python.org/3/library/heapq.html .
-
-This module implements the
-`min heap queue algorithm <https://en.wikipedia.org/wiki/Heap_%28data_structure%29>`_.
-
-A heap queue is essentially a list that has its elements stored in such a way
-that the first item of the list is always the smallest.
-"""
-from typing import Any
-
-def heappop(heap) -> Any:
-    """
-    Pop the first item from the ``heap``, and return it.  Raise ``IndexError`` if
-    ``heap`` is empty.
-
-    The returned item will be the smallest item in the ``heap``.
-    """
-    ...
-
-def heappush(heap, item) -> Any:
-    """
-    Push the ``item`` onto the ``heap``.
-    """
-    ...
-
-def heapify(x) -> Any:
-    """
-    Convert the list ``x`` into a heap.  This is an in-place operation.
-    """
-    ...
+"""
+heap queue algorithm. See: https://docs.micropython.org/en/v1.20.0/library/heapq.html
+
+|see_cpython_module| :mod:`python:heapq` https://docs.python.org/3/library/heapq.html .
+
+This module implements the
+`min heap queue algorithm <https://en.wikipedia.org/wiki/Heap_%28data_structure%29>`_.
+
+A heap queue is essentially a list that has its elements stored in such a way
+that the first item of the list is always the smallest.
+"""
+from typing import Any
+
+def heappop(heap) -> Any:
+    """
+    Pop the first item from the ``heap``, and return it.  Raise ``IndexError`` if
+    ``heap`` is empty.
+
+    The returned item will be the smallest item in the ``heap``.
+    """
+    ...
+
+def heappush(heap, item) -> Any:
+    """
+    Push the ``item`` onto the ``heap``.
+    """
+    ...
+
+def heapify(x) -> Any:
+    """
+    Convert the list ``x`` into a heap.  This is an in-place operation.
+    """
+    ...
```

### Comparing `micropython_rp2_stubs-1.19.1.post9/machine.pyi` & `micropython_rp2_stubs-1.20.0.post1/machine.pyi`

 * *Files 19% similar despite different names*

```diff
@@ -1,1035 +1,1178 @@
-"""
-functions related to the hardware. See: https://docs.micropython.org/en/v1.19.1/library/machine.html
-
-The ``machine`` module contains specific functions related to the hardware
-on a particular board. Most functions in this module allow to achieve direct
-and unrestricted access to and control of hardware blocks on a system
-(like CPU, timers, buses, etc.). Used incorrectly, this can lead to
-malfunction, lockups, crashes of your board, and in extreme cases, hardware
-damage.
-"""
-from typing import Callable, List, NoReturn, Optional, Tuple, Union, Any
-
-WDT_RESET: int
-PWRON_RESET: int
-
-def disable_irq() -> Any:
-    """
-    Disable interrupt requests.
-    Returns the previous IRQ state which should be considered an opaque value.
-    This return value should be passed to the `enable_irq()` function to restore
-    interrupts to their original state, before `disable_irq()` was called.
-    """
-    ...
-
-def soft_reset() -> NoReturn:
-    """
-    Performs a soft reset of the interpreter, deleting all Python objects and
-    resetting the Python heap.  It tries to retain the method by which the user
-    is connected to the MicroPython REPL (eg serial, USB, Wifi).
-    """
-    ...
-
-def enable_irq(state) -> Any:
-    """
-    Re-enable interrupt requests.
-    The *state* parameter should be the value that was returned from the most
-    recent call to the `disable_irq()` function.
-    """
-    ...
-
-def bitstream(pin, encoding, timing, data, /) -> Any:
-    """
-    Transmits *data* by bit-banging the specified *pin*. The *encoding* argument
-    specifies how the bits are encoded, and *timing* is an encoding-specific timing
-    specification.
-
-    The supported encodings are:
-
-      - ``0`` for "high low" pulse duration modulation. This will transmit 0 and
-        1 bits as timed pulses, starting with the most significant bit.
-        The *timing* must be a four-tuple of nanoseconds in the format
-        ``(high_time_0, low_time_0, high_time_1, low_time_1)``. For example,
-        ``(400, 850, 800, 450)`` is the timing specification for WS2812 RGB LEDs
-        at 800kHz.
-
-    The accuracy of the timing varies between ports. On Cortex M0 at 48MHz, it is
-    at best +/- 120ns, however on faster MCUs (ESP8266, ESP32, STM32, Pyboard), it
-    will be closer to +/-30ns.
-
-    ``Note:`` For controlling WS2812 / NeoPixel strips, see the :mod:`neopixel`
-       module for a higher-level API.
-    """
-    ...
-
-def deepsleep(time_ms: Optional[Any] = None) -> NoReturn:
-    """
-    Stops execution in an attempt to enter a low power state.
-
-    If *time_ms* is specified then this will be the maximum time in milliseconds that
-    the sleep will last for.  Otherwise the sleep can last indefinitely.
-
-    With or without a timeout, execution may resume at any time if there are events
-    that require processing.  Such events, or wake sources, should be configured before
-    sleeping, like `Pin` change or `RTC` timeout.
-
-    The precise behaviour and power-saving capabilities of lightsleep and deepsleep is
-    highly dependent on the underlying hardware, but the general properties are:
-
-    * A lightsleep has full RAM and state retention.  Upon wake execution is resumed
-      from the point where the sleep was requested, with all subsystems operational.
-
-    * A deepsleep may not retain RAM or any other state of the system (for example
-      peripherals or network interfaces).  Upon wake execution is resumed from the main
-      script, similar to a hard or power-on reset. The `reset_cause()` function will
-      return `machine.DEEPSLEEP` and this can be used to distinguish a deepsleep wake
-      from other resets.
-    """
-    ...
-
-def bootloader(value: Optional[Any] = None) -> None:
-    """
-    Reset the device and enter its bootloader.  This is typically used to put the
-    device into a state where it can be programmed with new firmware.
-
-    Some ports support passing in an optional *value* argument which can control
-    which bootloader to enter, what to pass to it, or other things.
-    """
-    ...
-
-def reset() -> NoReturn:
-    """
-    Resets the device in a manner similar to pushing the external RESET
-    button.
-    """
-    ...
-
-def freq(hz: Optional[Any] = None) -> Any:
-    """
-    Returns the CPU frequency in hertz.
-
-    On some ports this can also be used to set the CPU frequency by passing in *hz*.
-    """
-    ...
-
-def reset_cause() -> int:
-    """
-    Get the reset cause. See :ref:`constants <machine_constants>` for the possible return values.
-    """
-    ...
-
-def idle() -> Any:
-    """
-    Gates the clock to the CPU, useful to reduce power consumption at any time during
-    short or long periods. Peripherals continue working and execution resumes as soon
-    as any interrupt is triggered (on many ports this includes system timer
-    interrupt occurring at regular intervals on the order of millisecond).
-    """
-    ...
-
-def time_pulse_us(pin, pulse_level, timeout_us=1000000, /) -> int:
-    """
-    Time a pulse on the given *pin*, and return the duration of the pulse in
-    microseconds.  The *pulse_level* argument should be 0 to time a low pulse
-    or 1 to time a high pulse.
-
-    If the current input value of the pin is different to *pulse_level*,
-    the function first (*) waits until the pin input becomes equal to *pulse_level*,
-    then (**) times the duration that the pin is equal to *pulse_level*.
-    If the pin is already equal to *pulse_level* then timing starts straight away.
-
-    The function will return -2 if there was timeout waiting for condition marked
-    (*) above, and -1 if there was timeout during the main measurement, marked (**)
-    above. The timeout is the same for both cases and given by *timeout_us* (which
-    is in microseconds).
-    """
-    ...
-
-def lightsleep(time_ms: Optional[Any] = None) -> Any:
-    """
-    Stops execution in an attempt to enter a low power state.
-
-    If *time_ms* is specified then this will be the maximum time in milliseconds that
-    the sleep will last for.  Otherwise the sleep can last indefinitely.
-
-    With or without a timeout, execution may resume at any time if there are events
-    that require processing.  Such events, or wake sources, should be configured before
-    sleeping, like `Pin` change or `RTC` timeout.
-
-    The precise behaviour and power-saving capabilities of lightsleep and deepsleep is
-    highly dependent on the underlying hardware, but the general properties are:
-
-    * A lightsleep has full RAM and state retention.  Upon wake execution is resumed
-      from the point where the sleep was requested, with all subsystems operational.
-
-    * A deepsleep may not retain RAM or any other state of the system (for example
-      peripherals or network interfaces).  Upon wake execution is resumed from the main
-      script, similar to a hard or power-on reset. The `reset_cause()` function will
-      return `machine.DEEPSLEEP` and this can be used to distinguish a deepsleep wake
-      from other resets.
-    """
-    ...
-
-def unique_id() -> bytes:
-    """
-    Returns a byte string with a unique identifier of a board/SoC. It will vary
-    from a board/SoC instance to another, if underlying hardware allows. Length
-    varies by hardware (so use substring of a full value if you expect a short
-    ID). In some MicroPython ports, ID corresponds to the network MAC address.
-    """
-    ...
-
-class WDT:
-    """
-    Create a WDT object and start it. The timeout must be given in milliseconds.
-    Once it is running the timeout cannot be changed and the WDT cannot be stopped either.
-
-    Notes: On the esp32 the minimum timeout is 1 second. On the esp8266 a timeout
-    cannot be specified, it is determined by the underlying system.
-    """
-
-    def feed(self) -> None:
-        """
-        Feed the WDT to prevent it from resetting the system. The application
-        should place this call in a sensible place ensuring that the WDT is
-        only fed after verifying that everything is functioning correctly.
-        """
-        ...
-    def __init__(self, id=0, timeout=5000) -> None: ...
-
-mem8: Any
-mem32: Any
-mem16: Any
-
-class PWM:
-    """
-    Construct and return a new PWM object using the following parameters:
-
-       - *dest* is the entity on which the PWM is output, which is usually a
-         :ref:`machine.Pin <machine.Pin>` object, but a port may allow other values,
-         like integers.
-       - *freq* should be an integer which sets the frequency in Hz for the
-         PWM cycle.
-       - *duty_u16* sets the duty cycle as a ratio ``duty_u16 / 65535``.
-       - *duty_ns* sets the pulse width in nanoseconds.
-
-    Setting *freq* may affect other PWM objects if the objects share the same
-    underlying PWM generator (this is hardware specific).
-    Only one of *duty_u16* and *duty_ns* should be specified at a time.
-    """
-
-    def freq(self, value: Optional[Any] = None) -> Any:
-        """
-        Get or set the current frequency of the PWM output.
-
-        With no arguments the frequency in Hz is returned.
-
-        With a single *value* argument the frequency is set to that value in Hz.  The
-        method may raise a ``ValueError`` if the frequency is outside the valid range.
-        """
-        ...
-    def duty_u16(self, value: Optional[Any] = None) -> int:
-        """
-        Get or set the current duty cycle of the PWM output, as an unsigned 16-bit
-        value in the range 0 to 65535 inclusive.
-
-        With no arguments the duty cycle is returned.
-
-        With a single *value* argument the duty cycle is set to that value, measured
-        as the ratio ``value / 65535``.
-        """
-        ...
-    def duty_ns(self, value: Optional[Any] = None) -> int:
-        """
-        Get or set the current pulse width of the PWM output, as a value in nanoseconds.
-
-        With no arguments the pulse width in nanoseconds is returned.
-
-        With a single *value* argument the pulse width is set to that value.
-        """
-        ...
-    def deinit(self) -> None:
-        """
-        Disable the PWM output.
-        """
-        ...
-    def __init__(self, dest, *, freq=0, duty=0, duty_u16=0, duty_ns=0) -> None: ...
-
-class ADC:
-    """
-    Access the ADC associated with a source identified by *id*.  This
-    *id* may be an integer (usually specifying a channel number), a
-    :ref:`Pin <machine.Pin>` object, or other value supported by the
-    underlying machine.
-
-    If additional keyword-arguments are given then they will configure
-    various aspects of the ADC.  If not given, these settings will take
-    previous or default values.  The settings are:
-
-      - *sample_ns* is the sampling time in nanoseconds.
-
-      - *atten* specifies the input attenuation.
-    """
-
-    CORE_TEMP: int
-    def read_u16(self) -> int:
-        """
-        Take an analog reading and return an integer in the range 0-65535.
-        The return value represents the raw reading taken by the ADC, scaled
-        such that the minimum value is 0 and the maximum value is 65535.
-        """
-        ...
-    def __init__(self, id, *, sample_ns: Optional[int] = 0, atten: Optional[int] = ATTN_0DB) -> None: ...
-
-class I2C:
-    """
-    Construct and return a new I2C object using the following parameters:
-
-       - *id* identifies a particular I2C peripheral.  Allowed values for
-         depend on the particular port/board
-       - *scl* should be a pin object specifying the pin to use for SCL.
-       - *sda* should be a pin object specifying the pin to use for SDA.
-       - *freq* should be an integer which sets the maximum frequency
-         for SCL.
-
-    Note that some ports/boards will have default values of *scl* and *sda*
-    that can be changed in this constructor.  Others will have fixed values
-    of *scl* and *sda* that cannot be changed.
-    """
-
-    def readfrom_mem_into(self, addr, memaddr, buf, *, addrsize=8) -> None:
-        """
-        Read into *buf* from the peripheral specified by *addr* starting from the
-        memory address specified by *memaddr*.  The number of bytes read is the
-        length of *buf*.
-        The argument *addrsize* specifies the address size in bits (on ESP8266
-        this argument is not recognised and the address size is always 8 bits).
-
-        The method returns ``None``.
-        """
-        ...
-    def readfrom_into(self, addr, buf, stop=True, /) -> None:
-        """
-        Read into *buf* from the peripheral specified by *addr*.
-        The number of bytes read will be the length of *buf*.
-        If *stop* is true then a STOP condition is generated at the end of the transfer.
-
-        The method returns ``None``.
-        """
-        ...
-    def readfrom_mem(self, addr, memaddr, nbytes, *, addrsize=8) -> bytes:
-        """
-        Read *nbytes* from the peripheral specified by *addr* starting from the memory
-        address specified by *memaddr*.
-        The argument *addrsize* specifies the address size in bits.
-        Returns a `bytes` object with the data read.
-        """
-        ...
-    def writeto_mem(self, addr, memaddr, buf, *, addrsize=8) -> None:
-        """
-        Write *buf* to the peripheral specified by *addr* starting from the
-        memory address specified by *memaddr*.
-        The argument *addrsize* specifies the address size in bits (on ESP8266
-        this argument is not recognised and the address size is always 8 bits).
-
-        The method returns ``None``.
-        """
-        ...
-    def scan(self) -> List:
-        """
-        Scan all I2C addresses between 0x08 and 0x77 inclusive and return a list of
-        those that respond.  A device responds if it pulls the SDA line low after
-        its address (including a write bit) is sent on the bus.
-        """
-        ...
-    def writeto(self, addr, buf, stop=True, /) -> int:
-        """
-        Write the bytes from *buf* to the peripheral specified by *addr*.  If a
-        NACK is received following the write of a byte from *buf* then the
-        remaining bytes are not sent.  If *stop* is true then a STOP condition is
-        generated at the end of the transfer, even if a NACK is received.
-        The function returns the number of ACKs that were received.
-        """
-        ...
-    def writevto(self, addr, vector, stop=True, /) -> int:
-        """
-        Write the bytes contained in *vector* to the peripheral specified by *addr*.
-        *vector* should be a tuple or list of objects with the buffer protocol.
-        The *addr* is sent once and then the bytes from each object in *vector*
-        are written out sequentially.  The objects in *vector* may be zero bytes
-        in length in which case they don't contribute to the output.
-
-        If a NACK is received following the write of a byte from one of the
-        objects in *vector* then the remaining bytes, and any remaining objects,
-        are not sent.  If *stop* is true then a STOP condition is generated at
-        the end of the transfer, even if a NACK is received.  The function
-        returns the number of ACKs that were received.
-        """
-        ...
-    def start(self) -> None:
-        """
-        Generate a START condition on the bus (SDA transitions to low while SCL is high).
-        """
-        ...
-    def readfrom(self, addr, nbytes, stop=True, /) -> bytes:
-        """
-        Read *nbytes* from the peripheral specified by *addr*.
-        If *stop* is true then a STOP condition is generated at the end of the transfer.
-        Returns a `bytes` object with the data read.
-        """
-        ...
-    def readinto(self, buf, nack=True, /) -> Any:
-        """
-        Reads bytes from the bus and stores them into *buf*.  The number of bytes
-        read is the length of *buf*.  An ACK will be sent on the bus after
-        receiving all but the last byte.  After the last byte is received, if *nack*
-        is true then a NACK will be sent, otherwise an ACK will be sent (and in this
-        case the peripheral assumes more bytes are going to be read in a later call).
-        """
-        ...
-    def init(self, scl, sda, *, freq=400000) -> None:
-        """
-        Initialise the I2C bus with the given arguments:
-
-           - *scl* is a pin object for the SCL line
-           - *sda* is a pin object for the SDA line
-           - *freq* is the SCL clock rate
-        """
-        ...
-    def stop(self) -> None:
-        """
-        Generate a STOP condition on the bus (SDA transitions to high while SCL is high).
-        """
-        ...
-    def write(self, buf) -> int:
-        """
-        Write the bytes from *buf* to the bus.  Checks that an ACK is received
-        after each byte and stops transmitting the remaining bytes if a NACK is
-        received.  The function returns the number of ACKs that were received.
-        """
-        ...
-    def __init__(
-        self, id: Union[int, str] = -1, *, scl: Optional[Union[Pin, str]] = None, sda: Optional[Union[Pin, str]] = None, freq=400_000
-    ) -> None: ...
-
-class I2S:
-    """
-    Construct an I2S object of the given id:
-
-    - ``id`` identifies a particular I2S bus; it is board and port specific
-
-    Keyword-only parameters that are supported on all ports:
-
-      - ``sck`` is a pin object for the serial clock line
-      - ``ws`` is a pin object for the word select line
-      - ``sd`` is a pin object for the serial data line
-      - ``mck`` is a pin object for the master clock line;
-        master clock frequency is sampling rate * 256
-      - ``mode`` specifies receive or transmit
-      - ``bits`` specifies sample size (bits), 16 or 32
-      - ``format`` specifies channel format, STEREO or MONO
-      - ``rate`` specifies audio sampling rate (Hz);
-        this is the frequency of the ``ws`` signal
-      - ``ibuf`` specifies internal buffer length (bytes)
-
-    For all ports, DMA runs continuously in the background and allows user applications to perform other operations while
-    sample data is transfered between the internal buffer and the I2S peripheral unit.
-    Increasing the size of the internal buffer has the potential to increase the time that user applications can perform non-I2S operations
-    before underflow (e.g. ``write`` method) or overflow (e.g. ``readinto`` method).
-    """
-
-    RX: int
-    MONO: int
-    STEREO: int
-    TX: int
-    @staticmethod
-    def shift(*, buf, bits, shift) -> Any:
-        """
-        bitwise shift of all samples contained in ``buf``. ``bits`` specifies sample size in bits. ``shift`` specifies the number of bits to shift each sample.
-        Positive for left shift, negative for right shift.
-        Typically used for volume control.  Each bit shift changes sample volume by 6dB.
-        """
-        ...
-    def init(self, sck, *args, **kwargs) -> Any:
-        """
-        see Constructor for argument descriptions
-        """
-        ...
-    def irq(self, handler) -> Any:
-        """
-        Set a callback. ``handler`` is called when ``buf`` is emptied (``write`` method) or becomes full (``readinto`` method).
-        Setting a callback changes the ``write`` and ``readinto`` methods to non-blocking operation.
-        ``handler`` is called in the context of the MicroPython scheduler.
-        """
-        ...
-    def readinto(self, buf) -> int:
-        """
-        Read audio samples into the buffer specified by ``buf``.  ``buf`` must support the buffer protocol, such as bytearray or array.
-        "buf" byte ordering is little-endian.  For Stereo format, left channel sample precedes right channel sample. For Mono format,
-        the left channel sample data is used.
-        Returns number of bytes read
-        """
-        ...
-    def deinit(self) -> Any:
-        """
-        Deinitialize the I2S bus
-        """
-        ...
-    def write(self, buf) -> int:
-        """
-        Write audio samples contained in ``buf``. ``buf`` must support the buffer protocol, such as bytearray or array.
-        "buf" byte ordering is little-endian.  For Stereo format, left channel sample precedes right channel sample. For Mono format,
-        the sample data is written to both the right and left channels.
-        Returns number of bytes written
-        """
-        ...
-    def __init__(self, id, *, sck, ws, sd, mck=None, mode, bits, format, rate, ibuf) -> None: ...
-
-class Pin:
-    """
-    Access the pin peripheral (GPIO pin) associated with the given ``id``.  If
-    additional arguments are given in the constructor then they are used to initialise
-    the pin.  Any settings that are not specified will remain in their previous state.
-
-    The arguments are:
-
-      - ``id`` is mandatory and can be an arbitrary object.  Among possible value
-        types are: int (an internal Pin identifier), str (a Pin name), and tuple
-        (pair of [port, pin]).
-
-      - ``mode`` specifies the pin mode, which can be one of:
-
-        - ``Pin.IN`` - Pin is configured for input.  If viewed as an output the pin
-          is in high-impedance state.
-
-        - ``Pin.OUT`` - Pin is configured for (normal) output.
-
-        - ``Pin.OPEN_DRAIN`` - Pin is configured for open-drain output. Open-drain
-          output works in the following way: if the output value is set to 0 the pin
-          is active at a low level; if the output value is 1 the pin is in a high-impedance
-          state.  Not all ports implement this mode, or some might only on certain pins.
-
-        - ``Pin.ALT`` - Pin is configured to perform an alternative function, which is
-          port specific.  For a pin configured in such a way any other Pin methods
-          (except :meth:`Pin.init`) are not applicable (calling them will lead to undefined,
-          or a hardware-specific, result).  Not all ports implement this mode.
-
-        - ``Pin.ALT_OPEN_DRAIN`` - The Same as ``Pin.ALT``, but the pin is configured as
-          open-drain.  Not all ports implement this mode.
-
-        - ``Pin.ANALOG`` - Pin is configured for analog input, see the :class:`ADC` class.
-
-      - ``pull`` specifies if the pin has a (weak) pull resistor attached, and can be
-        one of:
-
-        - ``None`` - No pull up or down resistor.
-        - ``Pin.PULL_UP`` - Pull up resistor enabled.
-        - ``Pin.PULL_DOWN`` - Pull down resistor enabled.
-
-      - ``value`` is valid only for Pin.OUT and Pin.OPEN_DRAIN modes and specifies initial
-        output pin value if given, otherwise the state of the pin peripheral remains
-        unchanged.
-
-      - ``drive`` specifies the output power of the pin and can be one of: ``Pin.DRIVE_0``,
-        ``Pin.DRIVE_1``, etc., increasing in drive strength.  The actual current driving
-        capabilities are port dependent.  Not all ports implement this argument.
-
-      - ``alt`` specifies an alternate function for the pin and the values it can take are
-        port dependent.  This argument is valid only for ``Pin.ALT`` and ``Pin.ALT_OPEN_DRAIN``
-        modes.  It may be used when a pin supports more than one alternate function.  If only
-        one pin alternate function is supported the this argument is not required.  Not all
-        ports implement this argument.
-
-    As specified above, the Pin class allows to set an alternate function for a particular
-    pin, but it does not specify any further operations on such a pin.  Pins configured in
-    alternate-function mode are usually not used as GPIO but are instead driven by other
-    hardware peripherals.  The only operation supported on such a pin is re-initialising,
-    by calling the constructor or :meth:`Pin.init` method.  If a pin that is configured in
-    alternate-function mode is re-initialised with ``Pin.IN``, ``Pin.OUT``, or
-    ``Pin.OPEN_DRAIN``, the alternate function will be removed from the pin.
-    """
-
-    PULL_DOWN: int
-    IRQ_RISING: int
-    OPEN_DRAIN: int
-    OUT: int
-    IRQ_FALLING: int
-    PULL_UP: int
-    ALT: int
-    IN: int
-    def toggle(self, *args, **kwargs) -> Any: ...
-    def low(self) -> None:
-        """
-        Set pin to "0" output level.
-
-        Availability: nrf, rp2, stm32 ports.
-        """
-        ...
-    def off(self) -> None:
-        """
-        Set pin to "0" output level.
-        """
-        ...
-    def on(self) -> None:
-        """
-        Set pin to "1" output level.
-        """
-        ...
-    def irq(self, handler=None, trigger=IRQ_FALLING, *, priority=1, wake=None, hard=False) -> Callable[..., Any]:
-        """
-           Configure an interrupt handler to be called when the trigger source of the
-           pin is active.  If the pin mode is ``Pin.IN`` then the trigger source is
-           the external value on the pin.  If the pin mode is ``Pin.OUT`` then the
-           trigger source is the output buffer of the pin.  Otherwise, if the pin mode
-           is ``Pin.OPEN_DRAIN`` then the trigger source is the output buffer for
-           state '0' and the external pin value for state '1'.
-
-           The arguments are:
-
-             - ``handler`` is an optional function to be called when the interrupt
-               triggers. The handler must take exactly one argument which is the
-               ``Pin`` instance.
-
-             - ``trigger`` configures the event which can generate an interrupt.
-               Possible values are:
-
-               - ``Pin.IRQ_FALLING`` interrupt on falling edge.
-               - ``Pin.IRQ_RISING`` interrupt on rising edge.
-               - ``Pin.IRQ_LOW_LEVEL`` interrupt on low level.
-               - ``Pin.IRQ_HIGH_LEVEL`` interrupt on high level.
-
-               These values can be OR'ed together to trigger on multiple events.
-
-             - ``priority`` sets the priority level of the interrupt.  The values it
-               can take are port-specific, but higher values always represent higher
-               priorities.
-
-             - ``wake`` selects the power mode in which this interrupt can wake up the
-               system.  It can be ``machine.IDLE``, ``machine.SLEEP`` or ``machine.DEEPSLEEP``.
-               These values can also be OR'ed together to make a pin generate interrupts in
-               more than one power mode.
-
-             - ``hard`` if true a hardware interrupt is used. This reduces the delay
-               between the pin change and the handler being called. Hard interrupt
-               handlers may not allocate memory; see :ref:`isr_rules`.
-               Not all ports support this argument.
-
-           This method returns a callback object.
-
-        The following methods are not part of the core Pin API and only implemented on certain ports.
-        """
-        ...
-    def value(self, x: Optional[Any] = None) -> int:
-        """
-        This method allows to set and get the value of the pin, depending on whether
-        the argument ``x`` is supplied or not.
-
-        If the argument is omitted then this method gets the digital logic level of
-        the pin, returning 0 or 1 corresponding to low and high voltage signals
-        respectively.  The behaviour of this method depends on the mode of the pin:
-
-          - ``Pin.IN`` - The method returns the actual input value currently present
-            on the pin.
-          - ``Pin.OUT`` - The behaviour and return value of the method is undefined.
-          - ``Pin.OPEN_DRAIN`` - If the pin is in state '0' then the behaviour and
-            return value of the method is undefined.  Otherwise, if the pin is in
-            state '1', the method returns the actual input value currently present
-            on the pin.
-
-        If the argument is supplied then this method sets the digital logic level of
-        the pin.  The argument ``x`` can be anything that converts to a boolean.
-        If it converts to ``True``, the pin is set to state '1', otherwise it is set
-        to state '0'.  The behaviour of this method depends on the mode of the pin:
-
-          - ``Pin.IN`` - The value is stored in the output buffer for the pin.  The
-            pin state does not change, it remains in the high-impedance state.  The
-            stored value will become active on the pin as soon as it is changed to
-            ``Pin.OUT`` or ``Pin.OPEN_DRAIN`` mode.
-          - ``Pin.OUT`` - The output buffer is set to the given value immediately.
-          - ``Pin.OPEN_DRAIN`` - If the value is '0' the pin is set to a low voltage
-            state.  Otherwise the pin is set to high-impedance state.
-
-        When setting the value this method returns ``None``.
-        """
-        ...
-    def high(self) -> None:
-        """
-        Set pin to "1" output level.
-
-        Availability: nrf, rp2, stm32 ports.
-        """
-        ...
-    def init(self, mode=-1, pull=-1, *, value=None, drive=0, alt=-1) -> None:
-        """
-        Re-initialise the pin using the given parameters.  Only those arguments that
-        are specified will be set.  The rest of the pin peripheral state will remain
-        unchanged.  See the constructor documentation for details of the arguments.
-
-        Returns ``None``.
-        """
-        ...
-    def __init__(self, id, mode=-1, pull=-1, *, value=None, drive=0, alt=-1) -> None: ...
-
-class SoftSPI:
-    """
-    Construct a new software SPI object.  Additional parameters must be
-    given, usually at least *sck*, *mosi* and *miso*, and these are used
-    to initialise the bus.  See `SPI.init` for a description of the parameters.
-    """
-
-    LSB: int
-    MSB: int
-    def deinit(self, *args, **kwargs) -> Any: ...
-    def init(self, *args, **kwargs) -> Any: ...
-    def write_readinto(self, *args, **kwargs) -> Any: ...
-    def read(self, *args, **kwargs) -> Any: ...
-    def write(self, *args, **kwargs) -> Any: ...
-    def readinto(self, *args, **kwargs) -> Any: ...
-    def __init__(self, baudrate=500000, *, polarity=0, phase=0, bits=8, firstbit=MSB, sck=None, mosi=None, miso=None) -> None: ...
-
-class Timer:
-    """
-    Construct a new timer object of the given ``id``. ``id`` of -1 constructs a
-    virtual timer (if supported by a board).
-    ``id`` shall not be passed as a keyword argument.
-
-    See ``init`` for parameters of initialisation.
-    """
-
-    PERIODIC: int
-    ONE_SHOT: int
-    def init(self, *, mode=PERIODIC, period=-1, callback=None) -> None:
-        """
-        Initialise the timer. Example::
-
-            def mycallback(t):
-                pass
-
-            # periodic with 100ms period
-            tim.init(period=100, callback=mycallback)
-
-            # one shot firing after 1000ms
-            tim.init(mode=Timer.ONE_SHOT, period=1000, callback=mycallback)
-
-        Keyword arguments:
-
-          - ``mode`` can be one of:
-
-            - ``Timer.ONE_SHOT`` - The timer runs once until the configured
-              period of the channel expires.
-            - ``Timer.PERIODIC`` - The timer runs periodically at the configured
-              frequency of the channel.
-
-          - ``period`` - The timer period, in milliseconds.
-
-          - ``callback`` - The callable to call upon expiration of the timer period.
-            The callback must take one argument, which is passed the Timer object.
-            The ``callback`` argument shall be specified. Otherwise an exception
-            will occurr upon timer expiration:
-            ``TypeError: 'NoneType' object isn't callable``
-        """
-        ...
-    def deinit(self) -> None:
-        """
-        Deinitialises the timer. Stops the timer, and disables the timer peripheral.
-        """
-        ...
-    def __init__(self, id=-1, *args, **kwargs) -> None: ...
-
-class UART:
-    """
-    Construct a UART object of the given id.
-    """
-
-    INV_TX: int
-    CTS: int
-    INV_RX: int
-    RTS: int
-    def deinit(self) -> None:
-        """
-        Turn off the UART bus.
-        """
-        ...
-    def init(self, baudrate=9600, bits=8, parity=None, stop=1, *args, **kwargs) -> None:
-        """
-        Initialise the UART bus with the given parameters:
-
-          - *baudrate* is the clock rate.
-          - *bits* is the number of bits per character, 7, 8 or 9.
-          - *parity* is the parity, ``None``, 0 (even) or 1 (odd).
-          - *stop* is the number of stop bits, 1 or 2.
-
-        Additional keyword-only parameters that may be supported by a port are:
-
-          - *tx* specifies the TX pin to use.
-          - *rx* specifies the RX pin to use.
-          - *rts* specifies the RTS (output) pin to use for hardware receive flow control.
-          - *cts* specifies the CTS (input) pin to use for hardware transmit flow control.
-          - *txbuf* specifies the length in characters of the TX buffer.
-          - *rxbuf* specifies the length in characters of the RX buffer.
-          - *timeout* specifies the time to wait for the first character (in ms).
-          - *timeout_char* specifies the time to wait between characters (in ms).
-          - *invert* specifies which lines to invert.
-
-              - ``0`` will not invert lines (idle state of both lines is logic high).
-              - ``UART.INV_TX`` will invert TX line (idle state of TX line now logic low).
-              - ``UART.INV_RX`` will invert RX line (idle state of RX line now logic low).
-              - ``UART.INV_TX | UART.INV_RX`` will invert both lines (idle state at logic low).
-
-          - *flow* specifies which hardware flow control signals to use. The value
-            is a bitmask.
-
-              - ``0`` will ignore hardware flow control signals.
-              - ``UART.RTS`` will enable receive flow control by using the RTS output pin to
-                signal if the receive FIFO has sufficient space to accept more data.
-              - ``UART.CTS`` will enable transmit flow control by pausing transmission when the
-                CTS input pin signals that the receiver is running low on buffer space.
-              - ``UART.RTS | UART.CTS`` will enable both, for full hardware flow control.
-
-        On the WiPy only the following keyword-only parameter is supported:
-
-          - *pins* is a 4 or 2 item list indicating the TX, RX, RTS and CTS pins (in that order).
-            Any of the pins can be None if one wants the UART to operate with limited functionality.
-            If the RTS pin is given the the RX pin must be given as well. The same applies to CTS.
-            When no pins are given, then the default set of TX and RX pins is taken, and hardware
-            flow control will be disabled. If *pins* is ``None``, no pin assignment will be made.
-        """
-        ...
-    def sendbreak(self) -> None:
-        """
-        Send a break condition on the bus. This drives the bus low for a duration
-        longer than required for a normal transmission of a character.
-        """
-        ...
-    def read(self, nbytes: Optional[Any] = None) -> bytes:
-        """
-        Read characters.  If ``nbytes`` is specified then read at most that many bytes,
-        otherwise read as much data as possible. It may return sooner if a timeout
-        is reached. The timeout is configurable in the constructor.
-
-        Return value: a bytes object containing the bytes read in.  Returns ``None``
-        on timeout.
-        """
-        ...
-    def any(self) -> int:
-        """
-        Returns an integer counting the number of characters that can be read without
-        blocking.  It will return 0 if there are no characters available and a positive
-        number if there are characters.  The method may return 1 even if there is more
-        than one character available for reading.
-
-        For more sophisticated querying of available characters use select.poll::
-
-         poll = select.poll()
-         poll.register(uart, select.POLLIN)
-         poll.poll(timeout)
-        """
-        ...
-    def write(self, buf) -> int:
-        """
-        Write the buffer of bytes to the bus.
-
-        Return value: number of bytes written or ``None`` on timeout.
-        """
-        ...
-    def readinto(self, buf, nbytes: Optional[Any] = None) -> int:
-        """
-        Read bytes into the ``buf``.  If ``nbytes`` is specified then read at most
-        that many bytes.  Otherwise, read at most ``len(buf)`` bytes. It may return sooner if a timeout
-        is reached. The timeout is configurable in the constructor.
-
-        Return value: number of bytes read and stored into ``buf`` or ``None`` on
-        timeout.
-        """
-        ...
-    def readline(self) -> None:
-        """
-        Read a line, ending in a newline character. It may return sooner if a timeout
-        is reached. The timeout is configurable in the constructor.
-
-        Return value: the line read or ``None`` on timeout.
-        """
-        ...
-    def __init__(self, id, *args, **kwargs) -> None: ...
-
-class SoftI2C:
-    """
-    Construct a new software I2C object.  The parameters are:
-
-       - *scl* should be a pin object specifying the pin to use for SCL.
-       - *sda* should be a pin object specifying the pin to use for SDA.
-       - *freq* should be an integer which sets the maximum frequency
-         for SCL.
-       - *timeout* is the maximum time in microseconds to wait for clock
-         stretching (SCL held low by another device on the bus), after
-         which an ``OSError(ETIMEDOUT)`` exception is raised.
-    """
-
-    def readfrom_mem_into(self, *args, **kwargs) -> Any: ...
-    def readfrom_into(self, *args, **kwargs) -> Any: ...
-    def readfrom_mem(self, *args, **kwargs) -> Any: ...
-    def writeto_mem(self, *args, **kwargs) -> Any: ...
-    def scan(self, *args, **kwargs) -> Any: ...
-    def writeto(self, *args, **kwargs) -> Any: ...
-    def writevto(self, *args, **kwargs) -> Any: ...
-    def start(self, *args, **kwargs) -> Any: ...
-    def readfrom(self, *args, **kwargs) -> Any: ...
-    def readinto(self, *args, **kwargs) -> Any: ...
-    def init(self, *args, **kwargs) -> Any: ...
-    def stop(self, *args, **kwargs) -> Any: ...
-    def write(self, *args, **kwargs) -> Any: ...
-    def __init__(self, scl, sda, *, freq=400000, timeout=50000) -> None: ...
-
-class RTC:
-    """
-    Create an RTC object. See init for parameters of initialization.
-    """
-
-    def datetime(self, datetimetuple: Optional[Any] = None) -> Tuple:
-        """
-        Get or set the date and time of the RTC.
-
-        With no arguments, this method returns an 8-tuple with the current
-        date and time.  With 1 argument (being an 8-tuple) it sets the date
-        and time.
-
-        The 8-tuple has the following format:
-
-            (year, month, day, weekday, hours, minutes, seconds, subseconds)
-
-        The meaning of the ``subseconds`` field is hardware dependent.
-        """
-        ...
-    def __init__(self, id=0, *args, **kwargs) -> None: ...
-
-class SPI:
-    """
-    Construct an SPI object on the given bus, *id*. Values of *id* depend
-    on a particular port and its hardware. Values 0, 1, etc. are commonly used
-    to select hardware SPI block #0, #1, etc.
-
-    With no additional parameters, the SPI object is created but not
-    initialised (it has the settings from the last initialisation of
-    the bus, if any).  If extra arguments are given, the bus is initialised.
-    See ``init`` for parameters of initialisation.
-    """
-
-    LSB: int
-    MSB: int
-    def deinit(self) -> None:
-        """
-        Turn off the SPI bus.
-        """
-        ...
-    def init(
-        self, baudrate=1000000, *, polarity=0, phase=0, bits=8, firstbit=MSB, sck=None, mosi=None, miso=None, pins: Optional[Tuple]
-    ) -> None:
-        """
-        Initialise the SPI bus with the given parameters:
-
-          - ``baudrate`` is the SCK clock rate.
-          - ``polarity`` can be 0 or 1, and is the level the idle clock line sits at.
-          - ``phase`` can be 0 or 1 to sample data on the first or second clock edge
-            respectively.
-          - ``bits`` is the width in bits of each transfer. Only 8 is guaranteed to be supported by all hardware.
-          - ``firstbit`` can be ``SPI.MSB`` or ``SPI.LSB``.
-          - ``sck``, ``mosi``, ``miso`` are pins (machine.Pin) objects to use for bus signals. For most
-            hardware SPI blocks (as selected by ``id`` parameter to the constructor), pins are fixed
-            and cannot be changed. In some cases, hardware blocks allow 2-3 alternative pin sets for
-            a hardware SPI block. Arbitrary pin assignments are possible only for a bitbanging SPI driver
-            (``id`` = -1).
-          - ``pins`` - WiPy port doesn't ``sck``, ``mosi``, ``miso`` arguments, and instead allows to
-            specify them as a tuple of ``pins`` parameter.
-
-        In the case of hardware SPI the actual clock frequency may be lower than the
-        requested baudrate. This is dependant on the platform hardware. The actual
-        rate may be determined by printing the SPI object.
-        """
-        ...
-    def write_readinto(self, write_buf, read_buf) -> int:
-        """
-        Write the bytes from ``write_buf`` while reading into ``read_buf``.  The
-        buffers can be the same or different, but both buffers must have the
-        same length.
-        Returns ``None``.
-
-        Note: on WiPy this function returns the number of bytes written.
-        """
-        ...
-    def read(self, nbytes, write=0x00) -> bytes:
-        """
-        Read a number of bytes specified by ``nbytes`` while continuously writing
-        the single byte given by ``write``.
-        Returns a ``bytes`` object with the data that was read.
-        """
-        ...
-    def write(self, buf) -> int:
-        """
-        Write the bytes contained in ``buf``.
-        Returns ``None``.
-
-        Note: on WiPy this function returns the number of bytes written.
-        """
-        ...
-    def readinto(self, buf, write=0x00) -> int:
-        """
-        Read into the buffer specified by ``buf`` while continuously writing the
-        single byte given by ``write``.
-        Returns ``None``.
-
-        Note: on WiPy this function returns the number of bytes read.
-        """
-        ...
-    def __init__(self, id, *args, **kwargs) -> None: ...
-
-class Signal:
-    """
-            Signal(pin_arguments..., *, invert=False)
-
-    Create a Signal object. There're two ways to create it:
-
-    * By wrapping existing Pin object - universal method which works for
-      any board.
-    * By passing required Pin parameters directly to Signal constructor,
-      skipping the need to create intermediate Pin object. Available on
-      many, but not all boards.
-
-    The arguments are:
-
-      - ``pin_obj`` is existing Pin object.
-
-      - ``pin_arguments`` are the same arguments as can be passed to Pin constructor.
-
-      - ``invert`` - if True, the signal will be inverted (active low).
-    """
-
-    def off(self) -> None:
-        """
-        Deactivate signal.
-        """
-        ...
-    def on(self) -> None:
-        """
-        Activate signal.
-        """
-        ...
-    def value(self, x: Optional[Any] = None) -> int:
-        """
-        This method allows to set and get the value of the signal, depending on whether
-        the argument ``x`` is supplied or not.
-
-        If the argument is omitted then this method gets the signal level, 1 meaning
-        signal is asserted (active) and 0 - signal inactive.
-
-        If the argument is supplied then this method sets the signal level. The
-        argument ``x`` can be anything that converts to a boolean. If it converts
-        to ``True``, the signal is active, otherwise it is inactive.
-
-        Correspondence between signal being active and actual logic level on the
-        underlying pin depends on whether signal is inverted (active-low) or not.
-        For non-inverted signal, active status corresponds to logical 1, inactive -
-        to logical 0. For inverted/active-low signal, active status corresponds
-        to logical 0, while inactive - to logical 1.
-        """
-        ...
-    def __init__(self, pin_obj, *args, invert=False) -> None: ...
+"""
+functions related to the hardware. See: https://docs.micropython.org/en/v1.20.0/library/machine.html
+
+The ``machine`` module contains specific functions related to the hardware
+on a particular board. Most functions in this module allow to achieve direct
+and unrestricted access to and control of hardware blocks on a system
+(like CPU, timers, buses, etc.). Used incorrectly, this can lead to
+malfunction, lockups, crashes of your board, and in extreme cases, hardware
+damage.
+"""
+from typing import Callable, List, NoReturn, Optional, Tuple, Union, Any
+
+WDT_RESET: int
+PWRON_RESET: int
+
+def dht_readinto(*args, **kwargs) -> Any: ...
+def enable_irq(state) -> Any:
+    """
+    Re-enable interrupt requests.
+    The *state* parameter should be the value that was returned from the most
+    recent call to the `disable_irq()` function.
+    """
+    ...
+
+def disable_irq() -> Any:
+    """
+    Disable interrupt requests.
+    Returns the previous IRQ state which should be considered an opaque value.
+    This return value should be passed to the `enable_irq()` function to restore
+    interrupts to their original state, before `disable_irq()` was called.
+    """
+    ...
+
+def bitstream(pin, encoding, timing, data, /) -> Any:
+    """
+    Transmits *data* by bit-banging the specified *pin*. The *encoding* argument
+    specifies how the bits are encoded, and *timing* is an encoding-specific timing
+    specification.
+
+    The supported encodings are:
+
+      - ``0`` for "high low" pulse duration modulation. This will transmit 0 and
+        1 bits as timed pulses, starting with the most significant bit.
+        The *timing* must be a four-tuple of nanoseconds in the format
+        ``(high_time_0, low_time_0, high_time_1, low_time_1)``. For example,
+        ``(400, 850, 800, 450)`` is the timing specification for WS2812 RGB LEDs
+        at 800kHz.
+
+    The accuracy of the timing varies between ports. On Cortex M0 at 48MHz, it is
+    at best +/- 120ns, however on faster MCUs (ESP8266, ESP32, STM32, Pyboard), it
+    will be closer to +/-30ns.
+
+    ``Note:`` For controlling WS2812 / NeoPixel strips, see the :mod:`neopixel`
+       module for a higher-level API.
+    """
+    ...
+
+def deepsleep(time_ms: Optional[Any] = None) -> NoReturn:
+    """
+    Stops execution in an attempt to enter a low power state.
+
+    If *time_ms* is specified then this will be the maximum time in milliseconds that
+    the sleep will last for.  Otherwise the sleep can last indefinitely.
+
+    With or without a timeout, execution may resume at any time if there are events
+    that require processing.  Such events, or wake sources, should be configured before
+    sleeping, like `Pin` change or `RTC` timeout.
+
+    The precise behaviour and power-saving capabilities of lightsleep and deepsleep is
+    highly dependent on the underlying hardware, but the general properties are:
+
+    * A lightsleep has full RAM and state retention.  Upon wake execution is resumed
+      from the point where the sleep was requested, with all subsystems operational.
+
+    * A deepsleep may not retain RAM or any other state of the system (for example
+      peripherals or network interfaces).  Upon wake execution is resumed from the main
+      script, similar to a hard or power-on reset. The `reset_cause()` function will
+      return `machine.DEEPSLEEP` and this can be used to distinguish a deepsleep wake
+      from other resets.
+    """
+    ...
+
+def bootloader(value: Optional[Any] = None) -> None:
+    """
+    Reset the device and enter its bootloader.  This is typically used to put the
+    device into a state where it can be programmed with new firmware.
+
+    Some ports support passing in an optional *value* argument which can control
+    which bootloader to enter, what to pass to it, or other things.
+    """
+    ...
+
+def soft_reset() -> NoReturn:
+    """
+    Performs a soft reset of the interpreter, deleting all Python objects and
+    resetting the Python heap.  It tries to retain the method by which the user
+    is connected to the MicroPython REPL (eg serial, USB, Wifi).
+    """
+    ...
+
+def reset() -> NoReturn:
+    """
+    Resets the device in a manner similar to pushing the external RESET
+    button.
+    """
+    ...
+
+def freq(hz: Optional[Any] = None) -> Any:
+    """
+    Returns the CPU frequency in hertz.
+
+    On some ports this can also be used to set the CPU frequency by passing in *hz*.
+    """
+    ...
+
+def reset_cause() -> int:
+    """
+    Get the reset cause. See :ref:`constants <machine_constants>` for the possible return values.
+    """
+    ...
+
+def idle() -> Any:
+    """
+    Gates the clock to the CPU, useful to reduce power consumption at any time during
+    short or long periods. Peripherals continue working and execution resumes as soon
+    as any interrupt is triggered (on many ports this includes system timer
+    interrupt occurring at regular intervals on the order of millisecond).
+    """
+    ...
+
+def time_pulse_us(pin, pulse_level, timeout_us=1000000, /) -> int:
+    """
+    Time a pulse on the given *pin*, and return the duration of the pulse in
+    microseconds.  The *pulse_level* argument should be 0 to time a low pulse
+    or 1 to time a high pulse.
+
+    If the current input value of the pin is different to *pulse_level*,
+    the function first (*) waits until the pin input becomes equal to *pulse_level*,
+    then (**) times the duration that the pin is equal to *pulse_level*.
+    If the pin is already equal to *pulse_level* then timing starts straight away.
+
+    The function will return -2 if there was timeout waiting for condition marked
+    (*) above, and -1 if there was timeout during the main measurement, marked (**)
+    above. The timeout is the same for both cases and given by *timeout_us* (which
+    is in microseconds).
+    """
+    ...
+
+def lightsleep(time_ms: Optional[Any] = None) -> Any:
+    """
+    Stops execution in an attempt to enter a low power state.
+
+    If *time_ms* is specified then this will be the maximum time in milliseconds that
+    the sleep will last for.  Otherwise the sleep can last indefinitely.
+
+    With or without a timeout, execution may resume at any time if there are events
+    that require processing.  Such events, or wake sources, should be configured before
+    sleeping, like `Pin` change or `RTC` timeout.
+
+    The precise behaviour and power-saving capabilities of lightsleep and deepsleep is
+    highly dependent on the underlying hardware, but the general properties are:
+
+    * A lightsleep has full RAM and state retention.  Upon wake execution is resumed
+      from the point where the sleep was requested, with all subsystems operational.
+
+    * A deepsleep may not retain RAM or any other state of the system (for example
+      peripherals or network interfaces).  Upon wake execution is resumed from the main
+      script, similar to a hard or power-on reset. The `reset_cause()` function will
+      return `machine.DEEPSLEEP` and this can be used to distinguish a deepsleep wake
+      from other resets.
+    """
+    ...
+
+def unique_id() -> bytes:
+    """
+    Returns a byte string with a unique identifier of a board/SoC. It will vary
+    from a board/SoC instance to another, if underlying hardware allows. Length
+    varies by hardware (so use substring of a full value if you expect a short
+    ID). In some MicroPython ports, ID corresponds to the network MAC address.
+    """
+    ...
+
+class WDT:
+    """
+    Create a WDT object and start it. The timeout must be given in milliseconds.
+    Once it is running the timeout cannot be changed and the WDT cannot be stopped either.
+
+    Notes: On the esp32 the minimum timeout is 1 second. On the esp8266 a timeout
+    cannot be specified, it is determined by the underlying system. On rp2040 devices,
+    the maximum timeout is 8388 ms.
+    """
+
+    def feed(self) -> None:
+        """
+        Feed the WDT to prevent it from resetting the system. The application
+        should place this call in a sensible place ensuring that the WDT is
+        only fed after verifying that everything is functioning correctly.
+        """
+        ...
+    def __init__(self, id=0, timeout=5000) -> None: ...
+
+mem8: Any
+mem32: Any
+mem16: Any
+
+class PWM:
+    """
+    Construct and return a new PWM object using the following parameters:
+
+       - *dest* is the entity on which the PWM is output, which is usually a
+         :ref:`machine.Pin <machine.Pin>` object, but a port may allow other values,
+         like integers.
+       - *freq* should be an integer which sets the frequency in Hz for the
+         PWM cycle.
+       - *duty_u16* sets the duty cycle as a ratio ``duty_u16 / 65535``.
+       - *duty_ns* sets the pulse width in nanoseconds.
+
+    Setting *freq* may affect other PWM objects if the objects share the same
+    underlying PWM generator (this is hardware specific).
+    Only one of *duty_u16* and *duty_ns* should be specified at a time.
+    """
+
+    def freq(self, value: Optional[Any] = None) -> Any:
+        """
+        Get or set the current frequency of the PWM output.
+
+        With no arguments the frequency in Hz is returned.
+
+        With a single *value* argument the frequency is set to that value in Hz.  The
+        method may raise a ``ValueError`` if the frequency is outside the valid range.
+        """
+        ...
+    def duty_u16(self, value: Optional[Any] = None) -> int:
+        """
+        Get or set the current duty cycle of the PWM output, as an unsigned 16-bit
+        value in the range 0 to 65535 inclusive.
+
+        With no arguments the duty cycle is returned.
+
+        With a single *value* argument the duty cycle is set to that value, measured
+        as the ratio ``value / 65535``.
+        """
+        ...
+    def duty_ns(self, value: Optional[Any] = None) -> int:
+        """
+        Get or set the current pulse width of the PWM output, as a value in nanoseconds.
+
+        With no arguments the pulse width in nanoseconds is returned.
+
+        With a single *value* argument the pulse width is set to that value.
+        """
+        ...
+    def deinit(self) -> None:
+        """
+        Disable the PWM output.
+        """
+        ...
+    def __init__(self, dest, *, freq=0, duty=0, duty_u16=0, duty_ns=0) -> None: ...
+
+class ADC:
+    """
+    Access the ADC associated with a source identified by *id*.  This
+    *id* may be an integer (usually specifying a channel number), a
+    :ref:`Pin <machine.Pin>` object, or other value supported by the
+    underlying machine.
+
+    If additional keyword-arguments are given then they will configure
+    various aspects of the ADC.  If not given, these settings will take
+    previous or default values.  The settings are:
+
+      - *sample_ns* is the sampling time in nanoseconds.
+
+      - *atten* specifies the input attenuation.
+    """
+
+    CORE_TEMP: int
+    def read_u16(self) -> int:
+        """
+        Take an analog reading and return an integer in the range 0-65535.
+        The return value represents the raw reading taken by the ADC, scaled
+        such that the minimum value is 0 and the maximum value is 65535.
+        """
+        ...
+    def __init__(self, id, *, sample_ns: Optional[int] = 0, atten: Optional[int] = ATTN_0DB) -> None: ...
+
+class I2C:
+    """
+    Construct and return a new I2C object using the following parameters:
+
+       - *id* identifies a particular I2C peripheral.  Allowed values for
+         depend on the particular port/board
+       - *scl* should be a pin object specifying the pin to use for SCL.
+       - *sda* should be a pin object specifying the pin to use for SDA.
+       - *freq* should be an integer which sets the maximum frequency
+         for SCL.
+       - *timeout* is the maximum time in microseconds to allow for I2C
+         transactions.  This parameter is not allowed on some ports.
+
+    Note that some ports/boards will have default values of *scl* and *sda*
+    that can be changed in this constructor.  Others will have fixed values
+    of *scl* and *sda* that cannot be changed.
+    """
+
+    def readfrom_mem_into(self, addr, memaddr, buf, *, addrsize=8) -> None:
+        """
+        Read into *buf* from the peripheral specified by *addr* starting from the
+        memory address specified by *memaddr*.  The number of bytes read is the
+        length of *buf*.
+        The argument *addrsize* specifies the address size in bits (on ESP8266
+        this argument is not recognised and the address size is always 8 bits).
+
+        The method returns ``None``.
+        """
+        ...
+    def readfrom_into(self, addr, buf, stop=True, /) -> None:
+        """
+        Read into *buf* from the peripheral specified by *addr*.
+        The number of bytes read will be the length of *buf*.
+        If *stop* is true then a STOP condition is generated at the end of the transfer.
+
+        The method returns ``None``.
+        """
+        ...
+    def readfrom_mem(self, addr, memaddr, nbytes, *, addrsize=8) -> bytes:
+        """
+        Read *nbytes* from the peripheral specified by *addr* starting from the memory
+        address specified by *memaddr*.
+        The argument *addrsize* specifies the address size in bits.
+        Returns a `bytes` object with the data read.
+        """
+        ...
+    def writeto_mem(self, addr, memaddr, buf, *, addrsize=8) -> None:
+        """
+        Write *buf* to the peripheral specified by *addr* starting from the
+        memory address specified by *memaddr*.
+        The argument *addrsize* specifies the address size in bits (on ESP8266
+        this argument is not recognised and the address size is always 8 bits).
+
+        The method returns ``None``.
+        """
+        ...
+    def scan(self) -> List:
+        """
+        Scan all I2C addresses between 0x08 and 0x77 inclusive and return a list of
+        those that respond.  A device responds if it pulls the SDA line low after
+        its address (including a write bit) is sent on the bus.
+        """
+        ...
+    def writeto(self, addr, buf, stop=True, /) -> int:
+        """
+        Write the bytes from *buf* to the peripheral specified by *addr*.  If a
+        NACK is received following the write of a byte from *buf* then the
+        remaining bytes are not sent.  If *stop* is true then a STOP condition is
+        generated at the end of the transfer, even if a NACK is received.
+        The function returns the number of ACKs that were received.
+        """
+        ...
+    def writevto(self, addr, vector, stop=True, /) -> int:
+        """
+        Write the bytes contained in *vector* to the peripheral specified by *addr*.
+        *vector* should be a tuple or list of objects with the buffer protocol.
+        The *addr* is sent once and then the bytes from each object in *vector*
+        are written out sequentially.  The objects in *vector* may be zero bytes
+        in length in which case they don't contribute to the output.
+
+        If a NACK is received following the write of a byte from one of the
+        objects in *vector* then the remaining bytes, and any remaining objects,
+        are not sent.  If *stop* is true then a STOP condition is generated at
+        the end of the transfer, even if a NACK is received.  The function
+        returns the number of ACKs that were received.
+        """
+        ...
+    def start(self) -> None:
+        """
+        Generate a START condition on the bus (SDA transitions to low while SCL is high).
+        """
+        ...
+    def readfrom(self, addr, nbytes, stop=True, /) -> bytes:
+        """
+        Read *nbytes* from the peripheral specified by *addr*.
+        If *stop* is true then a STOP condition is generated at the end of the transfer.
+        Returns a `bytes` object with the data read.
+        """
+        ...
+    def readinto(self, buf, nack=True, /) -> Any:
+        """
+        Reads bytes from the bus and stores them into *buf*.  The number of bytes
+        read is the length of *buf*.  An ACK will be sent on the bus after
+        receiving all but the last byte.  After the last byte is received, if *nack*
+        is true then a NACK will be sent, otherwise an ACK will be sent (and in this
+        case the peripheral assumes more bytes are going to be read in a later call).
+        """
+        ...
+    def init(self, scl, sda, *, freq=400000) -> None:
+        """
+        Initialise the I2C bus with the given arguments:
+
+           - *scl* is a pin object for the SCL line
+           - *sda* is a pin object for the SDA line
+           - *freq* is the SCL clock rate
+
+         In the case of hardware I2C the actual clock frequency may be lower than the
+         requested frequency. This is dependant on the platform hardware. The actual
+         rate may be determined by printing the I2C object.
+        """
+        ...
+    def stop(self) -> None:
+        """
+        Generate a STOP condition on the bus (SDA transitions to high while SCL is high).
+        """
+        ...
+    def write(self, buf) -> int:
+        """
+        Write the bytes from *buf* to the bus.  Checks that an ACK is received
+        after each byte and stops transmitting the remaining bytes if a NACK is
+        received.  The function returns the number of ACKs that were received.
+        """
+        ...
+    def __init__(
+        self,
+        id: Union[int, str] = -1,
+        *,
+        scl: Optional[Union[Pin, str]] = None,
+        sda: Optional[Union[Pin, str]] = None,
+        freq=400_000,
+        timeout=50000,
+    ) -> None: ...
+
+class I2S:
+    """
+    Construct an I2S object of the given id:
+
+    - ``id`` identifies a particular I2S bus; it is board and port specific
+
+    Keyword-only parameters that are supported on all ports:
+
+      - ``sck`` is a pin object for the serial clock line
+      - ``ws`` is a pin object for the word select line
+      - ``sd`` is a pin object for the serial data line
+      - ``mck`` is a pin object for the master clock line;
+        master clock frequency is sampling rate * 256
+      - ``mode`` specifies receive or transmit
+      - ``bits`` specifies sample size (bits), 16 or 32
+      - ``format`` specifies channel format, STEREO or MONO
+      - ``rate`` specifies audio sampling rate (Hz);
+        this is the frequency of the ``ws`` signal
+      - ``ibuf`` specifies internal buffer length (bytes)
+
+    For all ports, DMA runs continuously in the background and allows user applications to perform other operations while
+    sample data is transfered between the internal buffer and the I2S peripheral unit.
+    Increasing the size of the internal buffer has the potential to increase the time that user applications can perform non-I2S operations
+    before underflow (e.g. ``write`` method) or overflow (e.g. ``readinto`` method).
+    """
+
+    RX: int
+    MONO: int
+    STEREO: int
+    TX: int
+    @staticmethod
+    def shift(*, buf, bits, shift) -> Any:
+        """
+        bitwise shift of all samples contained in ``buf``. ``bits`` specifies sample size in bits. ``shift`` specifies the number of bits to shift each sample.
+        Positive for left shift, negative for right shift.
+        Typically used for volume control.  Each bit shift changes sample volume by 6dB.
+        """
+        ...
+    def init(self, sck, *args, **kwargs) -> Any:
+        """
+        see Constructor for argument descriptions
+        """
+        ...
+    def irq(self, handler) -> Any:
+        """
+        Set a callback. ``handler`` is called when ``buf`` is emptied (``write`` method) or becomes full (``readinto`` method).
+        Setting a callback changes the ``write`` and ``readinto`` methods to non-blocking operation.
+        ``handler`` is called in the context of the MicroPython scheduler.
+        """
+        ...
+    def readinto(self, buf) -> int:
+        """
+        Read audio samples into the buffer specified by ``buf``.  ``buf`` must support the buffer protocol, such as bytearray or array.
+        "buf" byte ordering is little-endian.  For Stereo format, left channel sample precedes right channel sample. For Mono format,
+        the left channel sample data is used.
+        Returns number of bytes read
+        """
+        ...
+    def deinit(self) -> Any:
+        """
+        Deinitialize the I2S bus
+        """
+        ...
+    def write(self, buf) -> int:
+        """
+        Write audio samples contained in ``buf``. ``buf`` must support the buffer protocol, such as bytearray or array.
+        "buf" byte ordering is little-endian.  For Stereo format, left channel sample precedes right channel sample. For Mono format,
+        the sample data is written to both the right and left channels.
+        Returns number of bytes written
+        """
+        ...
+    def __init__(self, id, *, sck, ws, sd, mck=None, mode, bits, format, rate, ibuf) -> None: ...
+
+class Pin:
+    """
+    Access the pin peripheral (GPIO pin) associated with the given ``id``.  If
+    additional arguments are given in the constructor then they are used to initialise
+    the pin.  Any settings that are not specified will remain in their previous state.
+
+    The arguments are:
+
+      - ``id`` is mandatory and can be an arbitrary object.  Among possible value
+        types are: int (an internal Pin identifier), str (a Pin name), and tuple
+        (pair of [port, pin]).
+
+      - ``mode`` specifies the pin mode, which can be one of:
+
+        - ``Pin.IN`` - Pin is configured for input.  If viewed as an output the pin
+          is in high-impedance state.
+
+        - ``Pin.OUT`` - Pin is configured for (normal) output.
+
+        - ``Pin.OPEN_DRAIN`` - Pin is configured for open-drain output. Open-drain
+          output works in the following way: if the output value is set to 0 the pin
+          is active at a low level; if the output value is 1 the pin is in a high-impedance
+          state.  Not all ports implement this mode, or some might only on certain pins.
+
+        - ``Pin.ALT`` - Pin is configured to perform an alternative function, which is
+          port specific.  For a pin configured in such a way any other Pin methods
+          (except :meth:`Pin.init`) are not applicable (calling them will lead to undefined,
+          or a hardware-specific, result).  Not all ports implement this mode.
+
+        - ``Pin.ALT_OPEN_DRAIN`` - The Same as ``Pin.ALT``, but the pin is configured as
+          open-drain.  Not all ports implement this mode.
+
+        - ``Pin.ANALOG`` - Pin is configured for analog input, see the :class:`ADC` class.
+
+      - ``pull`` specifies if the pin has a (weak) pull resistor attached, and can be
+        one of:
+
+        - ``None`` - No pull up or down resistor.
+        - ``Pin.PULL_UP`` - Pull up resistor enabled.
+        - ``Pin.PULL_DOWN`` - Pull down resistor enabled.
+
+      - ``value`` is valid only for Pin.OUT and Pin.OPEN_DRAIN modes and specifies initial
+        output pin value if given, otherwise the state of the pin peripheral remains
+        unchanged.
+
+      - ``drive`` specifies the output power of the pin and can be one of: ``Pin.DRIVE_0``,
+        ``Pin.DRIVE_1``, etc., increasing in drive strength.  The actual current driving
+        capabilities are port dependent.  Not all ports implement this argument.
+
+      - ``alt`` specifies an alternate function for the pin and the values it can take are
+        port dependent.  This argument is valid only for ``Pin.ALT`` and ``Pin.ALT_OPEN_DRAIN``
+        modes.  It may be used when a pin supports more than one alternate function.  If only
+        one pin alternate function is supported the this argument is not required.  Not all
+        ports implement this argument.
+
+    As specified above, the Pin class allows to set an alternate function for a particular
+    pin, but it does not specify any further operations on such a pin.  Pins configured in
+    alternate-function mode are usually not used as GPIO but are instead driven by other
+    hardware peripherals.  The only operation supported on such a pin is re-initialising,
+    by calling the constructor or :meth:`Pin.init` method.  If a pin that is configured in
+    alternate-function mode is re-initialised with ``Pin.IN``, ``Pin.OUT``, or
+    ``Pin.OPEN_DRAIN``, the alternate function will be removed from the pin.
+    """
+
+    ALT_SPI: int
+    IN: int
+    ALT_USB: int
+    ALT_UART: int
+    IRQ_FALLING: int
+    OUT: int
+    OPEN_DRAIN: int
+    IRQ_RISING: int
+    PULL_DOWN: int
+    ALT_SIO: int
+    ALT_GPCK: int
+    ALT: int
+    PULL_UP: int
+    ALT_I2C: int
+    ALT_PWM: int
+    ALT_PIO1: int
+    ALT_PIO0: int
+    def low(self) -> None:
+        """
+        Set pin to "0" output level.
+
+        Availability: nrf, rp2, stm32 ports.
+        """
+        ...
+    def irq(self, handler=None, trigger=IRQ_FALLING, *, priority=1, wake=None, hard=False) -> Callable[..., Any]:
+        """
+           Configure an interrupt handler to be called when the trigger source of the
+           pin is active.  If the pin mode is ``Pin.IN`` then the trigger source is
+           the external value on the pin.  If the pin mode is ``Pin.OUT`` then the
+           trigger source is the output buffer of the pin.  Otherwise, if the pin mode
+           is ``Pin.OPEN_DRAIN`` then the trigger source is the output buffer for
+           state '0' and the external pin value for state '1'.
+
+           The arguments are:
+
+             - ``handler`` is an optional function to be called when the interrupt
+               triggers. The handler must take exactly one argument which is the
+               ``Pin`` instance.
+
+             - ``trigger`` configures the event which can generate an interrupt.
+               Possible values are:
+
+               - ``Pin.IRQ_FALLING`` interrupt on falling edge.
+               - ``Pin.IRQ_RISING`` interrupt on rising edge.
+               - ``Pin.IRQ_LOW_LEVEL`` interrupt on low level.
+               - ``Pin.IRQ_HIGH_LEVEL`` interrupt on high level.
+
+               These values can be OR'ed together to trigger on multiple events.
+
+             - ``priority`` sets the priority level of the interrupt.  The values it
+               can take are port-specific, but higher values always represent higher
+               priorities.
+
+             - ``wake`` selects the power mode in which this interrupt can wake up the
+               system.  It can be ``machine.IDLE``, ``machine.SLEEP`` or ``machine.DEEPSLEEP``.
+               These values can also be OR'ed together to make a pin generate interrupts in
+               more than one power mode.
+
+             - ``hard`` if true a hardware interrupt is used. This reduces the delay
+               between the pin change and the handler being called. Hard interrupt
+               handlers may not allocate memory; see :ref:`isr_rules`.
+               Not all ports support this argument.
+
+           This method returns a callback object.
+
+        The following methods are not part of the core Pin API and only implemented on certain ports.
+        """
+        ...
+    def toggle(self, *args, **kwargs) -> Any: ...
+    def off(self) -> None:
+        """
+        Set pin to "0" output level.
+        """
+        ...
+    def on(self) -> None:
+        """
+        Set pin to "1" output level.
+        """
+        ...
+    def init(self, mode=-1, pull=-1, *, value=None, drive=0, alt=-1) -> None:
+        """
+        Re-initialise the pin using the given parameters.  Only those arguments that
+        are specified will be set.  The rest of the pin peripheral state will remain
+        unchanged.  See the constructor documentation for details of the arguments.
+
+        Returns ``None``.
+        """
+        ...
+    def value(self, x: Optional[Any] = None) -> int:
+        """
+        This method allows to set and get the value of the pin, depending on whether
+        the argument ``x`` is supplied or not.
+
+        If the argument is omitted then this method gets the digital logic level of
+        the pin, returning 0 or 1 corresponding to low and high voltage signals
+        respectively.  The behaviour of this method depends on the mode of the pin:
+
+          - ``Pin.IN`` - The method returns the actual input value currently present
+            on the pin.
+          - ``Pin.OUT`` - The behaviour and return value of the method is undefined.
+          - ``Pin.OPEN_DRAIN`` - If the pin is in state '0' then the behaviour and
+            return value of the method is undefined.  Otherwise, if the pin is in
+            state '1', the method returns the actual input value currently present
+            on the pin.
+
+        If the argument is supplied then this method sets the digital logic level of
+        the pin.  The argument ``x`` can be anything that converts to a boolean.
+        If it converts to ``True``, the pin is set to state '1', otherwise it is set
+        to state '0'.  The behaviour of this method depends on the mode of the pin:
+
+          - ``Pin.IN`` - The value is stored in the output buffer for the pin.  The
+            pin state does not change, it remains in the high-impedance state.  The
+            stored value will become active on the pin as soon as it is changed to
+            ``Pin.OUT`` or ``Pin.OPEN_DRAIN`` mode.
+          - ``Pin.OUT`` - The output buffer is set to the given value immediately.
+          - ``Pin.OPEN_DRAIN`` - If the value is '0' the pin is set to a low voltage
+            state.  Otherwise the pin is set to high-impedance state.
+
+        When setting the value this method returns ``None``.
+        """
+        ...
+    def high(self) -> None:
+        """
+        Set pin to "1" output level.
+
+        Availability: nrf, rp2, stm32 ports.
+        """
+        ...
+
+    class cpu:
+        GPIO26: Any
+        GPIO25: Any
+        GPIO27: Any
+        GPIO28: Any
+        GPIO22: Any
+        GPIO24: Any
+        GPIO23: Any
+        GPIO9: Any
+        GPIO7: Any
+        GPIO6: Any
+        GPIO8: Any
+        GPIO29: Any
+        GPIO3: Any
+        GPIO5: Any
+        GPIO4: Any
+        GPIO12: Any
+        GPIO11: Any
+        GPIO13: Any
+        GPIO14: Any
+        GPIO0: Any
+        GPIO10: Any
+        GPIO1: Any
+        GPIO21: Any
+        GPIO2: Any
+        GPIO19: Any
+        GPIO20: Any
+        GPIO15: Any
+        GPIO16: Any
+        GPIO18: Any
+        GPIO17: Any
+        def __init__(self, *argv, **kwargs) -> None: ...
+
+    class board:
+        GP27: Any
+        GP26: Any
+        GP28: Any
+        LED: Any
+        GP21: Any
+        GP25: Any
+        GP22: Any
+        GP8: Any
+        GP7: Any
+        GP9: Any
+        GP3: Any
+        GP4: Any
+        GP6: Any
+        GP5: Any
+        GP12: Any
+        GP11: Any
+        GP13: Any
+        GP20: Any
+        GP0: Any
+        GP10: Any
+        GP1: Any
+        GP19: Any
+        GP18: Any
+        GP2: Any
+        GP14: Any
+        GP15: Any
+        GP17: Any
+        GP16: Any
+        def __init__(self, *argv, **kwargs) -> None: ...
+
+    def __init__(self, id, mode=-1, pull=-1, *, value=None, drive=0, alt=-1) -> None: ...
+    def __call__(self, x: Optional[Any] = None) -> Any:
+        """
+        Pin objects are callable.  The call method provides a (fast) shortcut to set
+        and get the value of the pin.  It is equivalent to Pin.value([x]).
+        See :meth:`Pin.value` for more details.
+        """
+        ...
+
+class SoftSPI:
+    """
+    Construct a new software SPI object.  Additional parameters must be
+    given, usually at least *sck*, *mosi* and *miso*, and these are used
+    to initialise the bus.  See `SPI.init` for a description of the parameters.
+    """
+
+    LSB: int
+    MSB: int
+    def deinit(self, *args, **kwargs) -> Any: ...
+    def init(self, *args, **kwargs) -> Any: ...
+    def write_readinto(self, *args, **kwargs) -> Any: ...
+    def read(self, *args, **kwargs) -> Any: ...
+    def write(self, *args, **kwargs) -> Any: ...
+    def readinto(self, *args, **kwargs) -> Any: ...
+    def __init__(self, baudrate=500000, *, polarity=0, phase=0, bits=8, firstbit=MSB, sck=None, mosi=None, miso=None) -> None: ...
+
+class Timer:
+    """
+    Construct a new timer object of the given ``id``. ``id`` of -1 constructs a
+    virtual timer (if supported by a board).
+    ``id`` shall not be passed as a keyword argument.
+
+    See ``init`` for parameters of initialisation.
+    """
+
+    PERIODIC: int
+    ONE_SHOT: int
+    def init(self, *, mode=PERIODIC, freq=-1, period=-1, callback=None) -> None:
+        """
+        Initialise the timer. Example::
+
+            def mycallback(t):
+                pass
+
+            # periodic at 1kHz
+            tim.init(mode=Timer.PERIODIC, freq=1000, callback=mycallback)
+
+            # periodic with 100ms period
+            tim.init(period=100, callback=mycallback)
+
+            # one shot firing after 1000ms
+            tim.init(mode=Timer.ONE_SHOT, period=1000, callback=mycallback)
+
+        Keyword arguments:
+
+          - ``mode`` can be one of:
+
+            - ``Timer.ONE_SHOT`` - The timer runs once until the configured
+              period of the channel expires.
+            - ``Timer.PERIODIC`` - The timer runs periodically at the configured
+              frequency of the channel.
+
+          - ``freq`` - The timer frequency, in units of Hz.  The upper bound of
+            the frequency is dependent on the port.  When both the ``freq`` and
+            ``period`` arguments are given, ``freq`` has a higher priority and
+            ``period`` is ignored.
+
+          - ``period`` - The timer period, in milliseconds.
+
+          - ``callback`` - The callable to call upon expiration of the timer period.
+            The callback must take one argument, which is passed the Timer object.
+            The ``callback`` argument shall be specified. Otherwise an exception
+            will occurr upon timer expiration:
+            ``TypeError: 'NoneType' object isn't callable``
+        """
+        ...
+    def deinit(self) -> None:
+        """
+        Deinitialises the timer. Stops the timer, and disables the timer peripheral.
+        """
+        ...
+    def __init__(self, id=-1, *args, **kwargs) -> None: ...
+
+class UART:
+    """
+    Construct a UART object of the given id.
+    """
+
+    INV_TX: int
+    RTS: int
+    CTS: int
+    INV_RX: int
+    def deinit(self) -> None:
+        """
+        Turn off the UART bus.
+
+        .. note::
+          You will not be able to call ``init()`` on the object after ``deinit()``.
+          A new instance needs to be created in that case.
+        """
+        ...
+    def sendbreak(self) -> None:
+        """
+        Send a break condition on the bus. This drives the bus low for a duration
+        longer than required for a normal transmission of a character.
+        """
+        ...
+    def init(self, baudrate=9600, bits=8, parity=None, stop=1, *args, **kwargs) -> None:
+        """
+        Initialise the UART bus with the given parameters:
+
+          - *baudrate* is the clock rate.
+          - *bits* is the number of bits per character, 7, 8 or 9.
+          - *parity* is the parity, ``None``, 0 (even) or 1 (odd).
+          - *stop* is the number of stop bits, 1 or 2.
+
+        Additional keyword-only parameters that may be supported by a port are:
+
+          - *tx* specifies the TX pin to use.
+          - *rx* specifies the RX pin to use.
+          - *rts* specifies the RTS (output) pin to use for hardware receive flow control.
+          - *cts* specifies the CTS (input) pin to use for hardware transmit flow control.
+          - *txbuf* specifies the length in characters of the TX buffer.
+          - *rxbuf* specifies the length in characters of the RX buffer.
+          - *timeout* specifies the time to wait for the first character (in ms).
+          - *timeout_char* specifies the time to wait between characters (in ms).
+          - *invert* specifies which lines to invert.
+
+              - ``0`` will not invert lines (idle state of both lines is logic high).
+              - ``UART.INV_TX`` will invert TX line (idle state of TX line now logic low).
+              - ``UART.INV_RX`` will invert RX line (idle state of RX line now logic low).
+              - ``UART.INV_TX | UART.INV_RX`` will invert both lines (idle state at logic low).
+
+          - *flow* specifies which hardware flow control signals to use. The value
+            is a bitmask.
+
+              - ``0`` will ignore hardware flow control signals.
+              - ``UART.RTS`` will enable receive flow control by using the RTS output pin to
+                signal if the receive FIFO has sufficient space to accept more data.
+              - ``UART.CTS`` will enable transmit flow control by pausing transmission when the
+                CTS input pin signals that the receiver is running low on buffer space.
+              - ``UART.RTS | UART.CTS`` will enable both, for full hardware flow control.
+
+        On the WiPy only the following keyword-only parameter is supported:
+
+          - *pins* is a 4 or 2 item list indicating the TX, RX, RTS and CTS pins (in that order).
+            Any of the pins can be None if one wants the UART to operate with limited functionality.
+            If the RTS pin is given the the RX pin must be given as well. The same applies to CTS.
+            When no pins are given, then the default set of TX and RX pins is taken, and hardware
+            flow control will be disabled. If *pins* is ``None``, no pin assignment will be made.
+
+        .. note::
+          It is possible to call ``init()`` multiple times on the same object in
+          order to reconfigure  UART on the fly. That allows using single UART
+          peripheral to serve different devices attached to different GPIO pins.
+          Only one device can be served at a time in that case.
+          Also do not call ``deinit()`` as it will prevent calling ``init()``
+          again.
+        """
+        ...
+    def flush(self) -> Any:
+        """
+        Waits until all data has been sent. In case of a timeout, an exception is raised. The timeout
+        duration depends on the tx buffer size and the baud rate. Unless flow control is enabled, a timeout
+        should not occur.
+
+        .. note::
+
+            For the rp2, esp8266 and nrf ports the call returns while the last byte is sent.
+            If required, a one character wait time has to be added in the calling script.
+
+        Availability: rp2, esp32, esp8266, mimxrt, cc3200, stm32, nrf ports, renesas-ra
+        """
+        ...
+    def txdone(self) -> bool:
+        """
+        Tells whether all data has been sent or no data transfer is happening. In this case,
+        it returns ``True``. If a data transmission is ongoing it returns ``False``.
+
+        .. note::
+
+            For the rp2, esp8266 and nrf ports the call may return ``True`` even if the last byte
+            of a transfer is still being sent. If required, a one character wait time has to be
+            added in the calling script.
+
+        Availability: rp2, esp32, esp8266, mimxrt, cc3200, stm32, nrf ports, renesas-ra
+        """
+        ...
+    def read(self, nbytes: Optional[Any] = None) -> bytes:
+        """
+        Read characters.  If ``nbytes`` is specified then read at most that many bytes,
+        otherwise read as much data as possible. It may return sooner if a timeout
+        is reached. The timeout is configurable in the constructor.
+
+        Return value: a bytes object containing the bytes read in.  Returns ``None``
+        on timeout.
+        """
+        ...
+    def any(self) -> int:
+        """
+        Returns an integer counting the number of characters that can be read without
+        blocking.  It will return 0 if there are no characters available and a positive
+        number if there are characters.  The method may return 1 even if there is more
+        than one character available for reading.
+
+        For more sophisticated querying of available characters use select.poll::
+
+         poll = select.poll()
+         poll.register(uart, select.POLLIN)
+         poll.poll(timeout)
+        """
+        ...
+    def write(self, buf) -> int:
+        """
+        Write the buffer of bytes to the bus.
+
+        Return value: number of bytes written or ``None`` on timeout.
+        """
+        ...
+    def readinto(self, buf, nbytes: Optional[Any] = None) -> int:
+        """
+        Read bytes into the ``buf``.  If ``nbytes`` is specified then read at most
+        that many bytes.  Otherwise, read at most ``len(buf)`` bytes. It may return sooner if a timeout
+        is reached. The timeout is configurable in the constructor.
+
+        Return value: number of bytes read and stored into ``buf`` or ``None`` on
+        timeout.
+        """
+        ...
+    def readline(self) -> None:
+        """
+        Read a line, ending in a newline character. It may return sooner if a timeout
+        is reached. The timeout is configurable in the constructor.
+
+        Return value: the line read or ``None`` on timeout.
+        """
+        ...
+    def __init__(self, id, *args, **kwargs) -> None: ...
+
+class SoftI2C(I2C):
+    """
+    Construct a new software I2C object.  The parameters are:
+
+       - *scl* should be a pin object specifying the pin to use for SCL.
+       - *sda* should be a pin object specifying the pin to use for SDA.
+       - *freq* should be an integer which sets the maximum frequency
+         for SCL.
+       - *timeout* is the maximum time in microseconds to wait for clock
+         stretching (SCL held low by another device on the bus), after
+         which an ``OSError(ETIMEDOUT)`` exception is raised.
+    """
+
+    def readfrom_mem_into(self, *args, **kwargs) -> Any: ...
+    def readfrom_into(self, *args, **kwargs) -> Any: ...
+    def readfrom_mem(self, *args, **kwargs) -> Any: ...
+    def writeto_mem(self, *args, **kwargs) -> Any: ...
+    def scan(self, *args, **kwargs) -> Any: ...
+    def writeto(self, *args, **kwargs) -> Any: ...
+    def writevto(self, *args, **kwargs) -> Any: ...
+    def start(self, *args, **kwargs) -> Any: ...
+    def readfrom(self, *args, **kwargs) -> Any: ...
+    def readinto(self, *args, **kwargs) -> Any: ...
+    def init(self, *args, **kwargs) -> Any: ...
+    def stop(self, *args, **kwargs) -> Any: ...
+    def write(self, *args, **kwargs) -> Any: ...
+    def __init__(self, scl, sda, *, freq=400000, timeout=50000) -> None: ...
+
+class RTC:
+    """
+    Create an RTC object. See init for parameters of initialization.
+    """
+
+    def datetime(self, datetimetuple: Optional[Any] = None) -> Tuple:
+        """
+        Get or set the date and time of the RTC.
+
+        With no arguments, this method returns an 8-tuple with the current
+        date and time.  With 1 argument (being an 8-tuple) it sets the date
+        and time.
+
+        The 8-tuple has the following format:
+
+            (year, month, day, weekday, hours, minutes, seconds, subseconds)
+
+        The meaning of the ``subseconds`` field is hardware dependent.
+        """
+        ...
+    def __init__(self, id=0, *args, **kwargs) -> None: ...
+
+class SPI:
+    """
+    Construct an SPI object on the given bus, *id*. Values of *id* depend
+    on a particular port and its hardware. Values 0, 1, etc. are commonly used
+    to select hardware SPI block #0, #1, etc.
+
+    With no additional parameters, the SPI object is created but not
+    initialised (it has the settings from the last initialisation of
+    the bus, if any).  If extra arguments are given, the bus is initialised.
+    See ``init`` for parameters of initialisation.
+    """
+
+    LSB: int
+    MSB: int
+    def deinit(self) -> None:
+        """
+        Turn off the SPI bus.
+        """
+        ...
+    def init(
+        self, baudrate=1000000, *, polarity=0, phase=0, bits=8, firstbit=MSB, sck=None, mosi=None, miso=None, pins: Optional[Tuple]
+    ) -> None:
+        """
+        Initialise the SPI bus with the given parameters:
+
+          - ``baudrate`` is the SCK clock rate.
+          - ``polarity`` can be 0 or 1, and is the level the idle clock line sits at.
+          - ``phase`` can be 0 or 1 to sample data on the first or second clock edge
+            respectively.
+          - ``bits`` is the width in bits of each transfer. Only 8 is guaranteed to be supported by all hardware.
+          - ``firstbit`` can be ``SPI.MSB`` or ``SPI.LSB``.
+          - ``sck``, ``mosi``, ``miso`` are pins (machine.Pin) objects to use for bus signals. For most
+            hardware SPI blocks (as selected by ``id`` parameter to the constructor), pins are fixed
+            and cannot be changed. In some cases, hardware blocks allow 2-3 alternative pin sets for
+            a hardware SPI block. Arbitrary pin assignments are possible only for a bitbanging SPI driver
+            (``id`` = -1).
+          - ``pins`` - WiPy port doesn't ``sck``, ``mosi``, ``miso`` arguments, and instead allows to
+            specify them as a tuple of ``pins`` parameter.
+
+        In the case of hardware SPI the actual clock frequency may be lower than the
+        requested baudrate. This is dependant on the platform hardware. The actual
+        rate may be determined by printing the SPI object.
+        """
+        ...
+    def write_readinto(self, write_buf, read_buf) -> int:
+        """
+        Write the bytes from ``write_buf`` while reading into ``read_buf``.  The
+        buffers can be the same or different, but both buffers must have the
+        same length.
+        Returns ``None``.
+
+        Note: on WiPy this function returns the number of bytes written.
+        """
+        ...
+    def read(self, nbytes, write=0x00) -> bytes:
+        """
+        Read a number of bytes specified by ``nbytes`` while continuously writing
+        the single byte given by ``write``.
+        Returns a ``bytes`` object with the data that was read.
+        """
+        ...
+    def write(self, buf) -> int:
+        """
+        Write the bytes contained in ``buf``.
+        Returns ``None``.
+
+        Note: on WiPy this function returns the number of bytes written.
+        """
+        ...
+    def readinto(self, buf, write=0x00) -> int:
+        """
+        Read into the buffer specified by ``buf`` while continuously writing the
+        single byte given by ``write``.
+        Returns ``None``.
+
+        Note: on WiPy this function returns the number of bytes read.
+        """
+        ...
+    def __init__(self, id, *args, **kwargs) -> None: ...
+
+class Signal(Pin):
+    """
+            Signal(pin_arguments..., *, invert=False)
+
+    Create a Signal object. There're two ways to create it:
+
+    * By wrapping existing Pin object - universal method which works for
+      any board.
+    * By passing required Pin parameters directly to Signal constructor,
+      skipping the need to create intermediate Pin object. Available on
+      many, but not all boards.
+
+    The arguments are:
+
+      - ``pin_obj`` is existing Pin object.
+
+      - ``pin_arguments`` are the same arguments as can be passed to Pin constructor.
+
+      - ``invert`` - if True, the signal will be inverted (active low).
+    """
+
+    def off(self) -> None:
+        """
+        Deactivate signal.
+        """
+        ...
+    def on(self) -> None:
+        """
+        Activate signal.
+        """
+        ...
+    def value(self, x: Optional[Any] = None) -> int:
+        """
+        This method allows to set and get the value of the signal, depending on whether
+        the argument ``x`` is supplied or not.
+
+        If the argument is omitted then this method gets the signal level, 1 meaning
+        signal is asserted (active) and 0 - signal inactive.
+
+        If the argument is supplied then this method sets the signal level. The
+        argument ``x`` can be anything that converts to a boolean. If it converts
+        to ``True``, the signal is active, otherwise it is inactive.
+
+        Correspondence between signal being active and actual logic level on the
+        underlying pin depends on whether signal is inverted (active-low) or not.
+        For non-inverted signal, active status corresponds to logical 1, inactive -
+        to logical 0. For inverted/active-low signal, active status corresponds
+        to logical 0, while inactive - to logical 1.
+        """
+        ...
+    def __init__(self, pin_obj, *args, invert=False) -> None: ...
```

### Comparing `micropython_rp2_stubs-1.19.1.post9/micropython.pyi` & `micropython_rp2_stubs-1.20.0.post1/micropython.pyi`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,158 +1,158 @@
-"""
-access and control MicroPython internals. See: https://docs.micropython.org/en/v1.19.1/library/micropython.html
-"""
-from typing import Optional, Any, Callable
-
-def opt_level(level: Optional[Any] = None) -> Any:
-    """
-    If *level* is given then this function sets the optimisation level for subsequent
-    compilation of scripts, and returns ``None``.  Otherwise it returns the current
-    optimisation level.
-
-    The optimisation level controls the following compilation features:
-
-    - Assertions: at level 0 assertion statements are enabled and compiled into the
-      bytecode; at levels 1 and higher assertions are not compiled.
-    - Built-in ``__debug__`` variable: at level 0 this variable expands to ``True``;
-      at levels 1 and higher it expands to ``False``.
-    - Source-code line numbers: at levels 0, 1 and 2 source-code line number are
-      stored along with the bytecode so that exceptions can report the line number
-      they occurred at; at levels 3 and higher line numbers are not stored.
-
-    The default optimisation level is usually level 0.
-    """
-    ...
-
-def mem_info(verbose: Optional[Any] = None) -> None:
-    """
-    Print information about currently used memory.  If the *verbose* argument
-    is given then extra information is printed.
-
-    The information that is printed is implementation dependent, but currently
-    includes the amount of stack and heap used.  In verbose mode it prints out
-    the entire heap indicating which blocks are used and which are free.
-    """
-    ...
-
-def stack_use() -> int:
-    """
-    Return an integer representing the current amount of stack that is being
-    used.  The absolute value of this is not particularly useful, rather it
-    should be used to compute differences in stack usage at different points.
-    """
-    ...
-
-def qstr_info(verbose: Optional[Any] = None) -> None:
-    """
-    Print information about currently interned strings.  If the *verbose*
-    argument is given then extra information is printed.
-
-    The information that is printed is implementation dependent, but currently
-    includes the number of interned strings and the amount of RAM they use.  In
-    verbose mode it prints out the names of all RAM-interned strings.
-    """
-    ...
-
-def schedule(func, arg) -> Any:
-    """
-    Schedule the function *func* to be executed "very soon".  The function
-    is passed the value *arg* as its single argument.  "Very soon" means that
-    the MicroPython runtime will do its best to execute the function at the
-    earliest possible time, given that it is also trying to be efficient, and
-    that the following conditions hold:
-
-    - A scheduled function will never preempt another scheduled function.
-    - Scheduled functions are always executed "between opcodes" which means
-      that all fundamental Python operations (such as appending to a list)
-      are guaranteed to be atomic.
-    - A given port may define "critical regions" within which scheduled
-      functions will never be executed.  Functions may be scheduled within
-      a critical region but they will not be executed until that region
-      is exited.  An example of a critical region is a preempting interrupt
-      handler (an IRQ).
-
-    A use for this function is to schedule a callback from a preempting IRQ.
-    Such an IRQ puts restrictions on the code that runs in the IRQ (for example
-    the heap may be locked) and scheduling a function to call later will lift
-    those restrictions.
-
-    Note: If `schedule()` is called from a preempting IRQ, when memory
-    allocation is not allowed and the callback to be passed to `schedule()` is
-    a bound method, passing this directly will fail. This is because creating a
-    reference to a bound method causes memory allocation. A solution is to
-    create a reference to the method in the class constructor and to pass that
-    reference to `schedule()`. This is discussed in detail here
-    :ref:`reference documentation <isr_rules>` under "Creation of Python
-    objects".
-
-    There is a finite queue to hold the scheduled functions and `schedule()`
-    will raise a `RuntimeError` if the queue is full.
-    """
-    ...
-
-def alloc_emergency_exception_buf(size) -> Any:
-    """
-    Allocate *size* bytes of RAM for the emergency exception buffer (a good
-    size is around 100 bytes).  The buffer is used to create exceptions in cases
-    when normal RAM allocation would fail (eg within an interrupt handler) and
-    therefore give useful traceback information in these situations.
-
-    A good way to use this function is to put it at the start of your main script
-    (eg ``boot.py`` or ``main.py``) and then the emergency exception buffer will be active
-    for all the code following it.
-    """
-    ...
-
-def const(expr) -> int:
-    """
-    Used to declare that the expression is a constant so that the compile can
-    optimise it.  The use of this function should be as follows::
-
-     from micropython import const
-
-     CONST_X = const(123)
-     CONST_Y = const(2 * CONST_X + 1)
-
-    Constants declared this way are still accessible as global variables from
-    outside the module they are declared in.  On the other hand, if a constant
-    begins with an underscore then it is hidden, it is not available as a global
-    variable, and does not take up any memory during execution.
-
-    This `const` function is recognised directly by the MicroPython parser and is
-    provided as part of the :mod:`micropython` module mainly so that scripts can be
-    written which run under both CPython and MicroPython, by following the above
-    pattern.
-    """
-    ...
-
-def kbd_intr(chr) -> None:
-    """
-    Set the character that will raise a `KeyboardInterrupt` exception.  By
-    default this is set to 3 during script execution, corresponding to Ctrl-C.
-    Passing -1 to this function will disable capture of Ctrl-C, and passing 3
-    will restore it.
-
-    This function can be used to prevent the capturing of Ctrl-C on the
-    incoming stream of characters that is usually used for the REPL, in case
-    that stream is used for other purposes.
-    """
-    ...
-
-def heap_lock() -> Any: ...
-def heap_unlock() -> Any: ...
-def viper(func: Callable) -> Callable:
-    """
-    The Viper code emitter is not fully compliant. It supports special Viper native data types in pursuit of performance.
-    Integer processing is non-compliant because it uses machine words: arithmetic on 32 bit hardware is performed modulo 2**32.
-    Like the Native emitter Viper produces machine instructions but further optimisations are performed, substantially increasing
-    performance especially for integer arithmetic and bit manipulations.
-    """
-    ...
-
-def native(func: Callable) -> Callable:
-    """
-    This causes the MicroPython compiler to emit native CPU opcodes rather than bytecode.
-    It covers the bulk of the MicroPython functionality, so most functions will require no adaptation.
-    See: https://docs.micropython.org/en/latest/reference/speed_python.html?highlight=viper#the-native-code-emitter
-    """
-    ...
+"""
+access and control MicroPython internals. See: https://docs.micropython.org/en/v1.19.1/library/micropython.html
+"""
+from typing import Optional, Any, Callable
+
+def opt_level(level: Optional[Any] = None) -> Any:
+    """
+    If *level* is given then this function sets the optimisation level for subsequent
+    compilation of scripts, and returns ``None``.  Otherwise it returns the current
+    optimisation level.
+
+    The optimisation level controls the following compilation features:
+
+    - Assertions: at level 0 assertion statements are enabled and compiled into the
+      bytecode; at levels 1 and higher assertions are not compiled.
+    - Built-in ``__debug__`` variable: at level 0 this variable expands to ``True``;
+      at levels 1 and higher it expands to ``False``.
+    - Source-code line numbers: at levels 0, 1 and 2 source-code line number are
+      stored along with the bytecode so that exceptions can report the line number
+      they occurred at; at levels 3 and higher line numbers are not stored.
+
+    The default optimisation level is usually level 0.
+    """
+    ...
+
+def mem_info(verbose: Optional[Any] = None) -> None:
+    """
+    Print information about currently used memory.  If the *verbose* argument
+    is given then extra information is printed.
+
+    The information that is printed is implementation dependent, but currently
+    includes the amount of stack and heap used.  In verbose mode it prints out
+    the entire heap indicating which blocks are used and which are free.
+    """
+    ...
+
+def stack_use() -> int:
+    """
+    Return an integer representing the current amount of stack that is being
+    used.  The absolute value of this is not particularly useful, rather it
+    should be used to compute differences in stack usage at different points.
+    """
+    ...
+
+def qstr_info(verbose: Optional[Any] = None) -> None:
+    """
+    Print information about currently interned strings.  If the *verbose*
+    argument is given then extra information is printed.
+
+    The information that is printed is implementation dependent, but currently
+    includes the number of interned strings and the amount of RAM they use.  In
+    verbose mode it prints out the names of all RAM-interned strings.
+    """
+    ...
+
+def schedule(func, arg) -> Any:
+    """
+    Schedule the function *func* to be executed "very soon".  The function
+    is passed the value *arg* as its single argument.  "Very soon" means that
+    the MicroPython runtime will do its best to execute the function at the
+    earliest possible time, given that it is also trying to be efficient, and
+    that the following conditions hold:
+
+    - A scheduled function will never preempt another scheduled function.
+    - Scheduled functions are always executed "between opcodes" which means
+      that all fundamental Python operations (such as appending to a list)
+      are guaranteed to be atomic.
+    - A given port may define "critical regions" within which scheduled
+      functions will never be executed.  Functions may be scheduled within
+      a critical region but they will not be executed until that region
+      is exited.  An example of a critical region is a preempting interrupt
+      handler (an IRQ).
+
+    A use for this function is to schedule a callback from a preempting IRQ.
+    Such an IRQ puts restrictions on the code that runs in the IRQ (for example
+    the heap may be locked) and scheduling a function to call later will lift
+    those restrictions.
+
+    Note: If `schedule()` is called from a preempting IRQ, when memory
+    allocation is not allowed and the callback to be passed to `schedule()` is
+    a bound method, passing this directly will fail. This is because creating a
+    reference to a bound method causes memory allocation. A solution is to
+    create a reference to the method in the class constructor and to pass that
+    reference to `schedule()`. This is discussed in detail here
+    :ref:`reference documentation <isr_rules>` under "Creation of Python
+    objects".
+
+    There is a finite queue to hold the scheduled functions and `schedule()`
+    will raise a `RuntimeError` if the queue is full.
+    """
+    ...
+
+def alloc_emergency_exception_buf(size) -> Any:
+    """
+    Allocate *size* bytes of RAM for the emergency exception buffer (a good
+    size is around 100 bytes).  The buffer is used to create exceptions in cases
+    when normal RAM allocation would fail (eg within an interrupt handler) and
+    therefore give useful traceback information in these situations.
+
+    A good way to use this function is to put it at the start of your main script
+    (eg ``boot.py`` or ``main.py``) and then the emergency exception buffer will be active
+    for all the code following it.
+    """
+    ...
+
+def const(expr) -> int:
+    """
+    Used to declare that the expression is a constant so that the compile can
+    optimise it.  The use of this function should be as follows::
+
+     from micropython import const
+
+     CONST_X = const(123)
+     CONST_Y = const(2 * CONST_X + 1)
+
+    Constants declared this way are still accessible as global variables from
+    outside the module they are declared in.  On the other hand, if a constant
+    begins with an underscore then it is hidden, it is not available as a global
+    variable, and does not take up any memory during execution.
+
+    This `const` function is recognised directly by the MicroPython parser and is
+    provided as part of the :mod:`micropython` module mainly so that scripts can be
+    written which run under both CPython and MicroPython, by following the above
+    pattern.
+    """
+    ...
+
+def kbd_intr(chr) -> None:
+    """
+    Set the character that will raise a `KeyboardInterrupt` exception.  By
+    default this is set to 3 during script execution, corresponding to Ctrl-C.
+    Passing -1 to this function will disable capture of Ctrl-C, and passing 3
+    will restore it.
+
+    This function can be used to prevent the capturing of Ctrl-C on the
+    incoming stream of characters that is usually used for the REPL, in case
+    that stream is used for other purposes.
+    """
+    ...
+
+def heap_lock() -> Any: ...
+def heap_unlock() -> Any: ...
+def viper(func: Callable) -> Callable:
+    """
+    The Viper code emitter is not fully compliant. It supports special Viper native data types in pursuit of performance.
+    Integer processing is non-compliant because it uses machine words: arithmetic on 32 bit hardware is performed modulo 2**32.
+    Like the Native emitter Viper produces machine instructions but further optimisations are performed, substantially increasing
+    performance especially for integer arithmetic and bit manipulations.
+    """
+    ...
+
+def native(func: Callable) -> Callable:
+    """
+    This causes the MicroPython compiler to emit native CPU opcodes rather than bytecode.
+    It covers the bulk of the MicroPython functionality, so most functions will require no adaptation.
+    See: https://docs.micropython.org/en/latest/reference/speed_python.html?highlight=viper#the-native-code-emitter
+    """
+    ...
```

### Comparing `micropython_rp2_stubs-1.19.1.post9/onewire.pyi` & `micropython_rp2_stubs-1.20.0.post1/onewire.pyi`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-from _typeshed import Incomplete
-
-class OneWireError(Exception): ...
-
-class OneWire:
-    SEARCH_ROM: int
-    MATCH_ROM: int
-    SKIP_ROM: int
-    pin: Incomplete
-    def __init__(self, pin) -> None: ...
-    def reset(self, required: bool = ...): ...
-    def readbit(self): ...
-    def readbyte(self): ...
-    def readinto(self, buf) -> None: ...
-    def writebit(self, value): ...
-    def writebyte(self, value): ...
-    def write(self, buf) -> None: ...
-    def select_rom(self, rom) -> None: ...
-    def scan(self): ...
-    def _search_rom(self, l_rom, diff): ...
-    def crc8(self, data): ...
+from _typeshed import Incomplete
+
+class OneWireError(Exception): ...
+
+class OneWire:
+    SEARCH_ROM: int
+    MATCH_ROM: int
+    SKIP_ROM: int
+    pin: Incomplete
+    def __init__(self, pin) -> None: ...
+    def reset(self, required: bool = ...): ...
+    def readbit(self): ...
+    def readbyte(self): ...
+    def readinto(self, buf) -> None: ...
+    def writebit(self, value): ...
+    def writebyte(self, value): ...
+    def write(self, buf) -> None: ...
+    def select_rom(self, rom) -> None: ...
+    def scan(self): ...
+    def _search_rom(self, l_rom, diff): ...
+    def crc8(self, data): ...
```

### Comparing `micropython_rp2_stubs-1.19.1.post9/os.pyi` & `micropython_rp2_stubs-1.20.0.post1/os.pyi`

 * *Files 21% similar despite different names*

```diff
@@ -1,244 +1,244 @@
-"""
-basic "operating system" services. See: https://docs.micropython.org/en/v1.19.1/library/os.html
-
-|see_cpython_module| :mod:`python:os` https://docs.python.org/3/library/os.html .
-
-The ``os`` module contains functions for filesystem access and mounting,
-terminal redirection and duplication, and the ``uname`` and ``urandom``
-functions.
-"""
-from typing import IO, Iterator, Optional, Tuple, Any
-from stdlib.os import uname_result
-
-def stat(path) -> Any:
-    """
-    Get the status of a file or directory.
-    """
-    ...
-
-def rmdir(path) -> None:
-    """
-    Remove a directory.
-    """
-    ...
-
-def rename(old_path, new_path) -> None:
-    """
-    Rename a file.
-    """
-    ...
-
-def mount(fsobj, mount_point, *, readonly) -> Any:
-    """
-    Mount the filesystem object *fsobj* at the location in the VFS given by the
-    *mount_point* string.  *fsobj* can be a a VFS object that has a ``mount()``
-    method, or a block device.  If it's a block device then the filesystem type
-    is automatically detected (an exception is raised if no filesystem was
-    recognised).  *mount_point* may be ``'/'`` to mount *fsobj* at the root,
-    or ``'/<name>'`` to mount it at a subdirectory under the root.
-
-    If *readonly* is ``True`` then the filesystem is mounted read-only.
-
-    During the mount process the method ``mount()`` is called on the filesystem
-    object.
-
-    Will raise ``OSError(EPERM)`` if *mount_point* is already mounted.
-    """
-    ...
-
-def urandom(n) -> bytes:
-    """
-    Return a bytes object with *n* random bytes. Whenever possible, it is
-    generated by the hardware random number generator.
-    """
-    ...
-
-def statvfs(path) -> Tuple:
-    """
-    Get the status of a fileystem.
-
-    Returns a tuple with the filesystem information in the following order:
-
-         * ``f_bsize`` -- file system block size
-         * ``f_frsize`` -- fragment size
-         * ``f_blocks`` -- size of fs in f_frsize units
-         * ``f_bfree`` -- number of free blocks
-         * ``f_bavail`` -- number of free blocks for unprivileged users
-         * ``f_files`` -- number of inodes
-         * ``f_ffree`` -- number of free inodes
-         * ``f_favail`` -- number of free inodes for unprivileged users
-         * ``f_flag`` -- mount flags
-         * ``f_namemax`` -- maximum filename length
-
-    Parameters related to inodes: ``f_files``, ``f_ffree``, ``f_avail``
-    and the ``f_flags`` parameter may return ``0`` as they can be unavailable
-    in a port-specific implementation.
-    """
-    ...
-
-def unlink(*args, **kwargs) -> Any: ...
-def uname() -> uname_result:
-    """
-    Return a tuple (possibly a named tuple) containing information about the
-    underlying machine and/or its operating system.  The tuple has five fields
-    in the following order, each of them being a string:
-
-         * ``sysname`` -- the name of the underlying system
-         * ``nodename`` -- the network name (can be the same as ``sysname``)
-         * ``release`` -- the version of the underlying system
-         * ``version`` -- the MicroPython version and build date
-         * ``machine`` -- an identifier for the underlying hardware (eg board, CPU)
-    """
-    ...
-
-def umount(mount_point) -> Any:
-    """
-    Unmount a filesystem. *mount_point* can be a string naming the mount location,
-    or a previously-mounted filesystem object.  During the unmount process the
-    method ``umount()`` is called on the filesystem object.
-
-    Will raise ``OSError(EINVAL)`` if *mount_point* is not found.
-    """
-    ...
-
-def chdir(path) -> Any:
-    """
-    Change current directory.
-    """
-    ...
-
-def dupterm(stream_object, index=0, /) -> IO:
-    """
-    Duplicate or switch the MicroPython terminal (the REPL) on the given `stream`-like
-    object. The *stream_object* argument must be a native stream object, or derive
-    from ``io.IOBase`` and implement the ``readinto()`` and
-    ``write()`` methods.  The stream should be in non-blocking mode and
-    ``readinto()`` should return ``None`` if there is no data available for reading.
-
-    After calling this function all terminal output is repeated on this stream,
-    and any input that is available on the stream is passed on to the terminal input.
-
-    The *index* parameter should be a non-negative integer and specifies which
-    duplication slot is set.  A given port may implement more than one slot (slot 0
-    will always be available) and in that case terminal input and output is
-    duplicated on all the slots that are set.
-
-    If ``None`` is passed as the *stream_object* then duplication is cancelled on
-    the slot given by *index*.
-
-    The function returns the previous stream-like object in the given slot.
-    """
-    ...
-
-def remove(path) -> None:
-    """
-    Remove a file.
-    """
-    ...
-
-def mkdir(path) -> Any:
-    """
-    Create a new directory.
-    """
-    ...
-
-def getcwd() -> Any:
-    """
-    Get the current directory.
-    """
-    ...
-
-def listdir(dir: Optional[Any] = None) -> Any:
-    """
-    With no argument, list the current directory.  Otherwise list the given directory.
-    """
-    ...
-
-def ilistdir(dir: Optional[Any] = None) -> Iterator[Tuple]:
-    """
-    This function returns an iterator which then yields tuples corresponding to
-    the entries in the directory that it is listing.  With no argument it lists the
-    current directory, otherwise it lists the directory given by *dir*.
-
-    The tuples have the form *(name, type, inode[, size])*:
-
-     - *name* is a string (or bytes if *dir* is a bytes object) and is the name of
-       the entry;
-     - *type* is an integer that specifies the type of the entry, with 0x4000 for
-       directories and 0x8000 for regular files;
-     - *inode* is an integer corresponding to the inode of the file, and may be 0
-       for filesystems that don't have such a notion.
-     - Some platforms may return a 4-tuple that includes the entry's *size*.  For
-       file entries, *size* is an integer representing the size of the file
-       or -1 if unknown.  Its meaning is currently undefined for directory
-       entries.
-    """
-    ...
-
-class VfsLfs2:
-    """
-    Create a filesystem object that uses the `littlefs v2 filesystem format`_.
-    Storage of the littlefs filesystem is provided by *block_dev*, which must
-    support the :ref:`extended interface <block-device-interface>`.
-    Objects created by this constructor can be mounted using :func:`mount`.
-
-    The *mtime* argument enables modification timestamps for files, stored using
-    littlefs attributes.  This option can be disabled or enabled differently each
-    mount time and timestamps will only be added or updated if *mtime* is enabled,
-    otherwise the timestamps will remain untouched.  Littlefs v2 filesystems without
-    timestamps will work without reformatting and timestamps will be added
-    transparently to existing files once they are opened for writing.  When *mtime*
-    is enabled `os.stat` on files without timestamps will return 0 for the timestamp.
-
-    See :ref:`filesystem` for more information.
-    """
-
-    def rename(self, *args, **kwargs) -> Any: ...
-    @staticmethod
-    def mkfs(block_dev, readsize=32, progsize=32, lookahead=32) -> None:
-        """
-            Build a Lfs2 filesystem on *block_dev*.
-
-        ``Note:`` There are reports of littlefs v2 failing in certain situations,
-                  for details see `littlefs issue 295`_.
-        """
-        ...
-    def mount(self, *args, **kwargs) -> Any: ...
-    def statvfs(self, *args, **kwargs) -> Any: ...
-    def rmdir(self, *args, **kwargs) -> Any: ...
-    def stat(self, *args, **kwargs) -> Any: ...
-    def umount(self, *args, **kwargs) -> Any: ...
-    def remove(self, *args, **kwargs) -> Any: ...
-    def mkdir(self, *args, **kwargs) -> Any: ...
-    def open(self, *args, **kwargs) -> Any: ...
-    def ilistdir(self, *args, **kwargs) -> Any: ...
-    def chdir(self, *args, **kwargs) -> Any: ...
-    def getcwd(self, *args, **kwargs) -> Any: ...
-    def __init__(self, block_dev, readsize=32, progsize=32, lookahead=32, mtime=True) -> None: ...
-
-class VfsFat:
-    """
-    Create a filesystem object that uses the FAT filesystem format.  Storage of
-    the FAT filesystem is provided by *block_dev*.
-    Objects created by this constructor can be mounted using :func:`mount`.
-    """
-
-    def rename(self, *args, **kwargs) -> Any: ...
-    @staticmethod
-    def mkfs(block_dev) -> None:
-        """
-        Build a FAT filesystem on *block_dev*.
-        """
-        ...
-    def mount(self, *args, **kwargs) -> Any: ...
-    def statvfs(self, *args, **kwargs) -> Any: ...
-    def rmdir(self, *args, **kwargs) -> Any: ...
-    def stat(self, *args, **kwargs) -> Any: ...
-    def umount(self, *args, **kwargs) -> Any: ...
-    def remove(self, *args, **kwargs) -> Any: ...
-    def mkdir(self, *args, **kwargs) -> Any: ...
-    def open(self, *args, **kwargs) -> Any: ...
-    def ilistdir(self, *args, **kwargs) -> Any: ...
-    def chdir(self, *args, **kwargs) -> Any: ...
-    def getcwd(self, *args, **kwargs) -> Any: ...
-    def __init__(self, block_dev) -> None: ...
+"""
+basic "operating system" services. See: https://docs.micropython.org/en/v1.20.0/library/os.html
+
+|see_cpython_module| :mod:`python:os` https://docs.python.org/3/library/os.html .
+
+The ``os`` module contains functions for filesystem access and mounting,
+terminal redirection and duplication, and the ``uname`` and ``urandom``
+functions.
+"""
+from typing import IO, Iterator, Optional, Tuple, Any
+from stdlib.os import uname_result
+
+def stat(path) -> Any:
+    """
+    Get the status of a file or directory.
+    """
+    ...
+
+def rmdir(path) -> None:
+    """
+    Remove a directory.
+    """
+    ...
+
+def rename(old_path, new_path) -> None:
+    """
+    Rename a file.
+    """
+    ...
+
+def mount(fsobj, mount_point, *, readonly) -> Any:
+    """
+    Mount the filesystem object *fsobj* at the location in the VFS given by the
+    *mount_point* string.  *fsobj* can be a a VFS object that has a ``mount()``
+    method, or a block device.  If it's a block device then the filesystem type
+    is automatically detected (an exception is raised if no filesystem was
+    recognised).  *mount_point* may be ``'/'`` to mount *fsobj* at the root,
+    or ``'/<name>'`` to mount it at a subdirectory under the root.
+
+    If *readonly* is ``True`` then the filesystem is mounted read-only.
+
+    During the mount process the method ``mount()`` is called on the filesystem
+    object.
+
+    Will raise ``OSError(EPERM)`` if *mount_point* is already mounted.
+    """
+    ...
+
+def urandom(n) -> bytes:
+    """
+    Return a bytes object with *n* random bytes. Whenever possible, it is
+    generated by the hardware random number generator.
+    """
+    ...
+
+def statvfs(path) -> Tuple:
+    """
+    Get the status of a fileystem.
+
+    Returns a tuple with the filesystem information in the following order:
+
+         * ``f_bsize`` -- file system block size
+         * ``f_frsize`` -- fragment size
+         * ``f_blocks`` -- size of fs in f_frsize units
+         * ``f_bfree`` -- number of free blocks
+         * ``f_bavail`` -- number of free blocks for unprivileged users
+         * ``f_files`` -- number of inodes
+         * ``f_ffree`` -- number of free inodes
+         * ``f_favail`` -- number of free inodes for unprivileged users
+         * ``f_flag`` -- mount flags
+         * ``f_namemax`` -- maximum filename length
+
+    Parameters related to inodes: ``f_files``, ``f_ffree``, ``f_avail``
+    and the ``f_flags`` parameter may return ``0`` as they can be unavailable
+    in a port-specific implementation.
+    """
+    ...
+
+def unlink(*args, **kwargs) -> Any: ...
+def uname() -> uname_result:
+    """
+    Return a tuple (possibly a named tuple) containing information about the
+    underlying machine and/or its operating system.  The tuple has five fields
+    in the following order, each of them being a string:
+
+         * ``sysname`` -- the name of the underlying system
+         * ``nodename`` -- the network name (can be the same as ``sysname``)
+         * ``release`` -- the version of the underlying system
+         * ``version`` -- the MicroPython version and build date
+         * ``machine`` -- an identifier for the underlying hardware (eg board, CPU)
+    """
+    ...
+
+def umount(mount_point) -> Any:
+    """
+    Unmount a filesystem. *mount_point* can be a string naming the mount location,
+    or a previously-mounted filesystem object.  During the unmount process the
+    method ``umount()`` is called on the filesystem object.
+
+    Will raise ``OSError(EINVAL)`` if *mount_point* is not found.
+    """
+    ...
+
+def chdir(path) -> Any:
+    """
+    Change current directory.
+    """
+    ...
+
+def dupterm(stream_object, index=0, /) -> IO:
+    """
+    Duplicate or switch the MicroPython terminal (the REPL) on the given `stream`-like
+    object. The *stream_object* argument must be a native stream object, or derive
+    from ``io.IOBase`` and implement the ``readinto()`` and
+    ``write()`` methods.  The stream should be in non-blocking mode and
+    ``readinto()`` should return ``None`` if there is no data available for reading.
+
+    After calling this function all terminal output is repeated on this stream,
+    and any input that is available on the stream is passed on to the terminal input.
+
+    The *index* parameter should be a non-negative integer and specifies which
+    duplication slot is set.  A given port may implement more than one slot (slot 0
+    will always be available) and in that case terminal input and output is
+    duplicated on all the slots that are set.
+
+    If ``None`` is passed as the *stream_object* then duplication is cancelled on
+    the slot given by *index*.
+
+    The function returns the previous stream-like object in the given slot.
+    """
+    ...
+
+def remove(path) -> None:
+    """
+    Remove a file.
+    """
+    ...
+
+def mkdir(path) -> Any:
+    """
+    Create a new directory.
+    """
+    ...
+
+def getcwd() -> Any:
+    """
+    Get the current directory.
+    """
+    ...
+
+def listdir(dir: Optional[Any] = None) -> Any:
+    """
+    With no argument, list the current directory.  Otherwise list the given directory.
+    """
+    ...
+
+def ilistdir(dir: Optional[Any] = None) -> Iterator[Tuple]:
+    """
+    This function returns an iterator which then yields tuples corresponding to
+    the entries in the directory that it is listing.  With no argument it lists the
+    current directory, otherwise it lists the directory given by *dir*.
+
+    The tuples have the form *(name, type, inode[, size])*:
+
+     - *name* is a string (or bytes if *dir* is a bytes object) and is the name of
+       the entry;
+     - *type* is an integer that specifies the type of the entry, with 0x4000 for
+       directories and 0x8000 for regular files;
+     - *inode* is an integer corresponding to the inode of the file, and may be 0
+       for filesystems that don't have such a notion.
+     - Some platforms may return a 4-tuple that includes the entry's *size*.  For
+       file entries, *size* is an integer representing the size of the file
+       or -1 if unknown.  Its meaning is currently undefined for directory
+       entries.
+    """
+    ...
+
+class VfsLfs2:
+    """
+    Create a filesystem object that uses the `littlefs v2 filesystem format`_.
+    Storage of the littlefs filesystem is provided by *block_dev*, which must
+    support the :ref:`extended interface <block-device-interface>`.
+    Objects created by this constructor can be mounted using :func:`mount`.
+
+    The *mtime* argument enables modification timestamps for files, stored using
+    littlefs attributes.  This option can be disabled or enabled differently each
+    mount time and timestamps will only be added or updated if *mtime* is enabled,
+    otherwise the timestamps will remain untouched.  Littlefs v2 filesystems without
+    timestamps will work without reformatting and timestamps will be added
+    transparently to existing files once they are opened for writing.  When *mtime*
+    is enabled `os.stat` on files without timestamps will return 0 for the timestamp.
+
+    See :ref:`filesystem` for more information.
+    """
+
+    def rename(self, *args, **kwargs) -> Any: ...
+    @staticmethod
+    def mkfs(block_dev, readsize=32, progsize=32, lookahead=32) -> None:
+        """
+            Build a Lfs2 filesystem on *block_dev*.
+
+        ``Note:`` There are reports of littlefs v2 failing in certain situations,
+                  for details see `littlefs issue 295`_.
+        """
+        ...
+    def mount(self, *args, **kwargs) -> Any: ...
+    def statvfs(self, *args, **kwargs) -> Any: ...
+    def rmdir(self, *args, **kwargs) -> Any: ...
+    def stat(self, *args, **kwargs) -> Any: ...
+    def umount(self, *args, **kwargs) -> Any: ...
+    def remove(self, *args, **kwargs) -> Any: ...
+    def mkdir(self, *args, **kwargs) -> Any: ...
+    def open(self, *args, **kwargs) -> Any: ...
+    def ilistdir(self, *args, **kwargs) -> Any: ...
+    def chdir(self, *args, **kwargs) -> Any: ...
+    def getcwd(self, *args, **kwargs) -> Any: ...
+    def __init__(self, block_dev, readsize=32, progsize=32, lookahead=32, mtime=True) -> None: ...
+
+class VfsFat:
+    """
+    Create a filesystem object that uses the FAT filesystem format.  Storage of
+    the FAT filesystem is provided by *block_dev*.
+    Objects created by this constructor can be mounted using :func:`mount`.
+    """
+
+    def rename(self, *args, **kwargs) -> Any: ...
+    @staticmethod
+    def mkfs(block_dev) -> None:
+        """
+        Build a FAT filesystem on *block_dev*.
+        """
+        ...
+    def mount(self, *args, **kwargs) -> Any: ...
+    def statvfs(self, *args, **kwargs) -> Any: ...
+    def rmdir(self, *args, **kwargs) -> Any: ...
+    def stat(self, *args, **kwargs) -> Any: ...
+    def umount(self, *args, **kwargs) -> Any: ...
+    def remove(self, *args, **kwargs) -> Any: ...
+    def mkdir(self, *args, **kwargs) -> Any: ...
+    def open(self, *args, **kwargs) -> Any: ...
+    def ilistdir(self, *args, **kwargs) -> Any: ...
+    def chdir(self, *args, **kwargs) -> Any: ...
+    def getcwd(self, *args, **kwargs) -> Any: ...
+    def __init__(self, block_dev) -> None: ...
```

### Comparing `micropython_rp2_stubs-1.19.1.post9/pyproject.toml` & `micropython_rp2_stubs-1.20.0.post1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "micropython-rp2-stubs"
-version = "1.19.1.post9"
+version = "1.20.0.post1"
 description = "MicroPython stubs"
 authors = [
     "josverl <josverl@users.noreply.github.com>",
 ]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/josverl/micropython-stubs#micropython-stubs"
@@ -34,79 +34,67 @@
 packages = [
     { include = "_boot.pyi" },
     { include = "_boot_fat.pyi" },
     { include = "_onewire.pyi" },
     { include = "_rp2.pyi" },
     { include = "_thread.pyi" },
     { include = "_uasyncio.pyi" },
-    { include = "aioble/__init__.pyi" },
-    { include = "aioble/central.pyi" },
-    { include = "aioble/client.pyi" },
-    { include = "aioble/core.pyi" },
-    { include = "aioble/device.pyi" },
-    { include = "aioble/l2cap.pyi" },
-    { include = "aioble/peripheral.pyi" },
-    { include = "aioble/server.pyi" },
     { include = "array.pyi" },
     { include = "binascii.pyi" },
     { include = "cmath.pyi" },
+    { include = "collections.pyi" },
+    { include = "cryptolib.pyi" },
     { include = "dht.pyi" },
     { include = "ds18x20.pyi" },
     { include = "errno.pyi" },
     { include = "framebuf.pyi" },
     { include = "gc.pyi" },
     { include = "hashlib.pyi" },
     { include = "heapq.pyi" },
+    { include = "io.pyi" },
     { include = "json.pyi" },
-    { include = "lsm6dsox.pyi" },
+    { include = "logging.pyi" },
     { include = "machine.pyi" },
     { include = "math.pyi" },
     { include = "micropython.pyi" },
     { include = "neopixel.pyi" },
-    { include = "network.pyi" },
     { include = "onewire.pyi" },
     { include = "os.pyi" },
     { include = "random.pyi" },
     { include = "rp2.pyi" },
     { include = "select.pyi" },
-    { include = "socket.pyi" },
     { include = "struct.pyi" },
     { include = "sys.pyi" },
     { include = "time.pyi" },
     { include = "uarray.pyi" },
     { include = "uasyncio/__init__.pyi" },
     { include = "uasyncio/core.pyi" },
     { include = "uasyncio/event.pyi" },
     { include = "uasyncio/funcs.pyi" },
     { include = "uasyncio/lock.pyi" },
     { include = "uasyncio/stream.pyi" },
     { include = "uasyncio/task.pyi" },
     { include = "ubinascii.pyi" },
-    { include = "ubluetooth.pyi" },
     { include = "ucollections.pyi" },
     { include = "ucryptolib.pyi" },
     { include = "uctypes.pyi" },
     { include = "uerrno.pyi" },
     { include = "uhashlib.pyi" },
     { include = "uheapq.pyi" },
     { include = "uio.pyi" },
     { include = "ujson.pyi" },
     { include = "umachine.pyi" },
     { include = "uos.pyi" },
     { include = "urandom.pyi" },
     { include = "ure.pyi" },
     { include = "uselect.pyi" },
-    { include = "usocket.pyi" },
     { include = "ustruct.pyi" },
     { include = "usys.pyi" },
     { include = "utime.pyi" },
-    { include = "uwebsocket.pyi" },
     { include = "uzlib.pyi" },
-    { include = "websocket.pyi" },
-    { include = "websocket_helper.pyi" },
     { include = "zlib.pyi" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 micropython-stdlib-stubs = ">=0.9.0"
```

### Comparing `micropython_rp2_stubs-1.19.1.post9/select.pyi` & `micropython_rp2_stubs-1.20.0.post1/select.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -1,93 +1,93 @@
-"""
-wait for events on a set of streams. See: https://docs.micropython.org/en/v1.19.1/library/select.html
-
-|see_cpython_module| :mod:`python:select` https://docs.python.org/3/library/select.html .
-
-This module provides functions to efficiently wait for events on multiple
-`streams <stream>` (select streams which are ready for operations).
-"""
-from typing import Iterator, List, Optional, Tuple, Any
-
-POLLOUT: int
-POLLIN: int
-POLLHUP: int
-POLLERR: int
-
-class select:
-    """
-    Wait for activity on a set of objects.
-
-    This function is provided by some MicroPython ports for compatibility
-    and is not efficient. Usage of :class:`Poll` is recommended instead.
-    """
-
-    def __init__(self, rlist, wlist, xlist, timeout: Optional[Any] = None) -> None: ...
-
-class poll:
-    """
-    Create an instance of the Poll class.
-    """
-
-    def __init__(self) -> None: ...
-    def register(self, obj, eventmask: Optional[Any] = None) -> None:
-        """
-        Register `stream` *obj* for polling. *eventmask* is logical OR of:
-
-        * ``select.POLLIN``  - data available for reading
-        * ``select.POLLOUT`` - more data can be written
-
-        Note that flags like ``select.POLLHUP`` and ``select.POLLERR`` are
-        *not* valid as input eventmask (these are unsolicited events which
-        will be returned from `poll()` regardless of whether they are asked
-        for). This semantics is per POSIX.
-
-        *eventmask* defaults to ``select.POLLIN | select.POLLOUT``.
-
-        It is OK to call this function multiple times for the same *obj*.
-        Successive calls will update *obj*'s eventmask to the value of
-        *eventmask* (i.e. will behave as `modify()`).
-        """
-        ...
-    def unregister(self, obj) -> Any:
-        """
-        Unregister *obj* from polling.
-        """
-        ...
-    def modify(self, obj, eventmask) -> None:
-        """
-        Modify the *eventmask* for *obj*. If *obj* is not registered, `OSError`
-        is raised with error of ENOENT.
-        """
-        ...
-    def poll(self, timeout=-1, /) -> List:
-        """
-        Wait for at least one of the registered objects to become ready or have an
-        exceptional condition, with optional timeout in milliseconds (if *timeout*
-        arg is not specified or -1, there is no timeout).
-
-        Returns list of (``obj``, ``event``, ...) tuples. There may be other elements in
-        tuple, depending on a platform and version, so don't assume that its size is 2.
-        The ``event`` element specifies which events happened with a stream and
-        is a combination of ``select.POLL*`` constants described above. Note that
-        flags ``select.POLLHUP`` and ``select.POLLERR`` can be returned at any time
-        (even if were not asked for), and must be acted on accordingly (the
-        corresponding stream unregistered from poll and likely closed), because
-        otherwise all further invocations of `poll()` may return immediately with
-        these flags set for this stream again.
-
-        In case of timeout, an empty list is returned.
-        """
-        ...
-    def ipoll(self, timeout=-1, flags=0, /) -> Iterator[Tuple]:
-        """
-        Like :meth:`poll.poll`, but instead returns an iterator which yields a
-        `callee-owned tuple`. This function provides an efficient, allocation-free
-        way to poll on streams.
-
-        If *flags* is 1, one-shot behaviour for events is employed: streams for
-        which events happened will have their event masks automatically reset
-        (equivalent to ``poll.modify(obj, 0)``), so new events for such a stream
-        won't be processed until new mask is set with `poll.modify()`. This
-        behaviour is useful for asynchronous I/O schedulers.
-        """
-        ...
+"""
+wait for events on a set of streams. See: https://docs.micropython.org/en/v1.20.0/library/select.html
+
+|see_cpython_module| :mod:`python:select` https://docs.python.org/3/library/select.html .
+
+This module provides functions to efficiently wait for events on multiple
+`streams <stream>` (select streams which are ready for operations).
+"""
+from typing import Iterator, List, Optional, Tuple, Any
+
+POLLOUT: int
+POLLIN: int
+POLLHUP: int
+POLLERR: int
+
+class select:
+    """
+    Wait for activity on a set of objects.
+
+    This function is provided by some MicroPython ports for compatibility
+    and is not efficient. Usage of :class:`Poll` is recommended instead.
+    """
+
+    def __init__(self, rlist, wlist, xlist, timeout: Optional[Any] = None) -> None: ...
+
+class poll:
+    """
+    Create an instance of the Poll class.
+    """
+
+    def __init__(self) -> None: ...
+    def register(self, obj, eventmask: Optional[Any] = None) -> None:
+        """
+        Register `stream` *obj* for polling. *eventmask* is logical OR of:
+
+        * ``select.POLLIN``  - data available for reading
+        * ``select.POLLOUT`` - more data can be written
+
+        Note that flags like ``select.POLLHUP`` and ``select.POLLERR`` are
+        *not* valid as input eventmask (these are unsolicited events which
+        will be returned from `poll()` regardless of whether they are asked
+        for). This semantics is per POSIX.
+
+        *eventmask* defaults to ``select.POLLIN | select.POLLOUT``.
+
+        It is OK to call this function multiple times for the same *obj*.
+        Successive calls will update *obj*'s eventmask to the value of
+        *eventmask* (i.e. will behave as `modify()`).
+        """
+        ...
+    def unregister(self, obj) -> Any:
+        """
+        Unregister *obj* from polling.
+        """
+        ...
+    def modify(self, obj, eventmask) -> None:
+        """
+        Modify the *eventmask* for *obj*. If *obj* is not registered, `OSError`
+        is raised with error of ENOENT.
+        """
+        ...
+    def poll(self, timeout=-1, /) -> List:
+        """
+        Wait for at least one of the registered objects to become ready or have an
+        exceptional condition, with optional timeout in milliseconds (if *timeout*
+        arg is not specified or -1, there is no timeout).
+
+        Returns list of (``obj``, ``event``, ...) tuples. There may be other elements in
+        tuple, depending on a platform and version, so don't assume that its size is 2.
+        The ``event`` element specifies which events happened with a stream and
+        is a combination of ``select.POLL*`` constants described above. Note that
+        flags ``select.POLLHUP`` and ``select.POLLERR`` can be returned at any time
+        (even if were not asked for), and must be acted on accordingly (the
+        corresponding stream unregistered from poll and likely closed), because
+        otherwise all further invocations of `poll()` may return immediately with
+        these flags set for this stream again.
+
+        In case of timeout, an empty list is returned.
+        """
+        ...
+    def ipoll(self, timeout=-1, flags=0, /) -> Iterator[Tuple]:
+        """
+        Like :meth:`poll.poll`, but instead returns an iterator which yields a
+        `callee-owned tuple`. This function provides an efficient, allocation-free
+        way to poll on streams.
+
+        If *flags* is 1, one-shot behaviour for events is employed: streams for
+        which events happened will have their event masks automatically reset
+        (equivalent to ``poll.modify(obj, 0)``), so new events for such a stream
+        won't be processed until new mask is set with `poll.modify()`. This
+        behaviour is useful for asynchronous I/O schedulers.
+        """
+        ...
```

### Comparing `micropython_rp2_stubs-1.19.1.post9/sys.pyi` & `micropython_rp2_stubs-1.20.0.post1/sys.pyi`

 * *Files 22% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-"""
-system specific functions. See: https://docs.micropython.org/en/v1.19.1/library/sys.html
-
-|see_cpython_module| :mod:`python:sys` https://docs.python.org/3/library/sys.html .
-"""
-from typing import Dict, List, Tuple, Any
-
-platform: str
-version_info: tuple
-path: list
-version: str
-ps1: str
-ps2: str
-byteorder: str
-modules: dict
-argv: list
-implementation: tuple
-maxsize: int
-
-def print_exception(exc, file=stdout, /) -> None:
-    """
-    Print exception with a traceback to a file-like object *file* (or
-    `sys.stdout` by default).
-    """
-    ...
-
-def exit(retval=0, /) -> Any:
-    """
-    Terminate current program with a given exit code. Underlyingly, this
-    function raise as `SystemExit` exception. If an argument is given, its
-    value given as an argument to `SystemExit`.
-    """
-    ...
-
-stderr: Any
-stdout: Any
-stdin: Any
+"""
+system specific functions. See: https://docs.micropython.org/en/v1.20.0/library/sys.html
+
+|see_cpython_module| :mod:`python:sys` https://docs.python.org/3/library/sys.html .
+"""
+from typing import Dict, List, Tuple, Any
+
+platform: str
+version_info: tuple
+path: list
+version: str
+ps1: str
+ps2: str
+byteorder: str
+modules: dict
+argv: list
+implementation: tuple
+maxsize: int
+
+def print_exception(exc, file=stdout, /) -> None:
+    """
+    Print exception with a traceback to a file-like object *file* (or
+    `sys.stdout` by default).
+    """
+    ...
+
+def exit(retval=0, /) -> Any:
+    """
+    Terminate current program with a given exit code. Underlyingly, this
+    function raise as `SystemExit` exception. If an argument is given, its
+    value given as an argument to `SystemExit`.
+    """
+    ...
+
+stderr: Any
+stdout: Any
+stdin: Any
```

### Comparing `micropython_rp2_stubs-1.19.1.post9/time.pyi` & `micropython_rp2_stubs-1.20.0.post1/time.pyi`

 * *Files 22% similar despite different names*

```diff
@@ -1,278 +1,278 @@
-"""
-time related functions. See: https://docs.micropython.org/en/v1.19.1/library/time.html
-
-|see_cpython_module| :mod:`python:time` https://docs.python.org/3/library/time.html .
-
-The ``time`` module provides functions for getting the current time and date,
-measuring time intervals, and for delays.
-
-**Time Epoch**: Unix port uses standard for POSIX systems epoch of
-1970-01-01 00:00:00 UTC. However, embedded ports use epoch of
-2000-01-01 00:00:00 UTC.
-
-**Maintaining actual calendar date/time**: This requires a
-Real Time Clock (RTC). On systems with underlying OS (including some
-RTOS), an RTC may be implicit. Setting and maintaining actual calendar
-time is responsibility of OS/RTOS and is done outside of MicroPython,
-it just uses OS API to query date/time. On baremetal ports however
-system time depends on ``machine.RTC()`` object. The current calendar time
-may be set using ``machine.RTC().datetime(tuple)`` function, and maintained
-by following means:
-
-* By a backup battery (which may be an additional, optional component for
-  a particular board).
-* Using networked time protocol (requires setup by a port/user).
-* Set manually by a user on each power-up (many boards then maintain
-  RTC time across hard resets, though some may require setting it again
-  in such case).
-
-If actual calendar time is not maintained with a system/MicroPython RTC,
-functions below which require reference to current absolute time may
-behave not as expected.
-"""
-from typing import Optional, Tuple, Any
-
-def ticks_diff(ticks1, ticks2) -> int:
-    """
-    Measure ticks difference between values returned from `ticks_ms()`, `ticks_us()`,
-    or `ticks_cpu()` functions, as a signed value which may wrap around.
-
-    The argument order is the same as for subtraction
-    operator, ``ticks_diff(ticks1, ticks2)`` has the same meaning as ``ticks1 - ticks2``.
-    However, values returned by `ticks_ms()`, etc. functions may wrap around, so
-    directly using subtraction on them will produce incorrect result. That is why
-    `ticks_diff()` is needed, it implements modular (or more specifically, ring)
-    arithmetics to produce correct result even for wrap-around values (as long as they not
-    too distant inbetween, see below). The function returns **signed** value in the range
-    [*-TICKS_PERIOD/2* .. *TICKS_PERIOD/2-1*] (that's a typical range definition for
-    two's-complement signed binary integers). If the result is negative, it means that
-    *ticks1* occurred earlier in time than *ticks2*. Otherwise, it means that
-    *ticks1* occurred after *ticks2*. This holds **only** if *ticks1* and *ticks2*
-    are apart from each other for no more than *TICKS_PERIOD/2-1* ticks. If that does
-    not hold, incorrect result will be returned. Specifically, if two tick values are
-    apart for *TICKS_PERIOD/2-1* ticks, that value will be returned by the function.
-    However, if *TICKS_PERIOD/2* of real-time ticks has passed between them, the
-    function will return *-TICKS_PERIOD/2* instead, i.e. result value will wrap around
-    to the negative range of possible values.
-
-    Informal rationale of the constraints above: Suppose you are locked in a room with no
-    means to monitor passing of time except a standard 12-notch clock. Then if you look at
-    dial-plate now, and don't look again for another 13 hours (e.g., if you fall for a
-    long sleep), then once you finally look again, it may seem to you that only 1 hour
-    has passed. To avoid this mistake, just look at the clock regularly. Your application
-    should do the same. "Too long sleep" metaphor also maps directly to application
-    behaviour: don't let your application run any single task for too long. Run tasks
-    in steps, and do time-keeping inbetween.
-
-    `ticks_diff()` is designed to accommodate various usage patterns, among them:
-
-    * Polling with timeout. In this case, the order of events is known, and you will deal
-      only with positive results of `ticks_diff()`::
-
-         # Wait for GPIO pin to be asserted, but at most 500us
-         start = time.ticks_us()
-         while pin.value() == 0:
-             if time.ticks_diff(time.ticks_us(), start) > 500:
-                 raise TimeoutError
-
-    * Scheduling events. In this case, `ticks_diff()` result may be negative
-      if an event is overdue::
-
-         # This code snippet is not optimized
-         now = time.ticks_ms()
-         scheduled_time = task.scheduled_time()
-         if ticks_diff(scheduled_time, now) > 0:
-             print("Too early, let's nap")
-             sleep_ms(ticks_diff(scheduled_time, now))
-             task.run()
-         elif ticks_diff(scheduled_time, now) == 0:
-             print("Right at time!")
-             task.run()
-         elif ticks_diff(scheduled_time, now) < 0:
-             print("Oops, running late, tell task to run faster!")
-             task.run(run_faster=true)
-
-    Note: Do not pass `time()` values to `ticks_diff()`, you should use
-    normal mathematical operations on them. But note that `time()` may (and will)
-    also overflow. This is known as https://en.wikipedia.org/wiki/Year_2038_problem .
-
-    """
-    ...
-
-def ticks_add(ticks, delta) -> Any:
-    """
-    Offset ticks value by a given number, which can be either positive or negative.
-    Given a *ticks* value, this function allows to calculate ticks value *delta*
-    ticks before or after it, following modular-arithmetic definition of tick values
-    (see `ticks_ms()` above). *ticks* parameter must be a direct result of call
-    to `ticks_ms()`, `ticks_us()`, or `ticks_cpu()` functions (or from previous
-    call to `ticks_add()`). However, *delta* can be an arbitrary integer number
-    or numeric expression. `ticks_add()` is useful for calculating deadlines for
-    events/tasks. (Note: you must use `ticks_diff()` function to work with
-    deadlines.)
-
-    Examples::
-
-         # Find out what ticks value there was 100ms ago
-         print(ticks_add(time.ticks_ms(), -100))
-
-         # Calculate deadline for operation and test for it
-         deadline = ticks_add(time.ticks_ms(), 200)
-         while ticks_diff(deadline, time.ticks_ms()) > 0:
-             do_a_little_of_something()
-
-         # Find out TICKS_MAX used by this port
-         print(ticks_add(0, -1))
-
-    """
-    ...
-
-def ticks_cpu() -> Any:
-    """
-    Similar to `ticks_ms()` and `ticks_us()`, but with the highest possible resolution
-    in the system. This is usually CPU clocks, and that's why the function is named that
-    way. But it doesn't have to be a CPU clock, some other timing source available in a
-    system (e.g. high-resolution timer) can be used instead. The exact timing unit
-    (resolution) of this function is not specified on ``time`` module level, but
-    documentation for a specific port may provide more specific information. This
-    function is intended for very fine benchmarking or very tight real-time loops.
-    Avoid using it in portable code.
-
-    Availability: Not every port implements this function.
-
-    """
-    ...
-
-class time:
-    """
-    Returns the number of seconds, as an integer, since the Epoch, assuming that
-    underlying RTC is set and maintained as described above. If an RTC is not set, this
-    function returns number of seconds since a port-specific reference point in time (for
-    embedded boards without a battery-backed RTC, usually since power up or reset). If you
-    want to develop portable MicroPython application, you should not rely on this function
-    to provide higher than second precision.  If you need higher precision, absolute
-    timestamps, use `time_ns()`.  If relative times are acceptable then use the
-    `ticks_ms()` and `ticks_us()` functions.  If you need calendar time, `gmtime()` or
-    `localtime()` without an argument is a better choice.
-    """
-
-    def __init__(self) -> None: ...
-
-def ticks_ms() -> int:
-    """
-    Returns an increasing millisecond counter with an arbitrary reference point, that
-    wraps around after some value.
-
-    The wrap-around value is not explicitly exposed, but we will
-    refer to it as *TICKS_MAX* to simplify discussion. Period of the values is
-    *TICKS_PERIOD = TICKS_MAX + 1*. *TICKS_PERIOD* is guaranteed to be a power of
-    two, but otherwise may differ from port to port. The same period value is used
-    for all of `ticks_ms()`, `ticks_us()`, `ticks_cpu()` functions (for
-    simplicity). Thus, these functions will return a value in range [*0* ..
-    *TICKS_MAX*], inclusive, total *TICKS_PERIOD* values. Note that only
-    non-negative values are used. For the most part, you should treat values returned
-    by these functions as opaque. The only operations available for them are
-    `ticks_diff()` and `ticks_add()` functions described below.
-
-    Note: Performing standard mathematical operations (+, -) or relational
-    operators (<, <=, >, >=) directly on these value will lead to invalid
-    result. Performing mathematical operations and then passing their results
-    as arguments to `ticks_diff()` or `ticks_add()` will also lead to
-    invalid results from the latter functions.
-    """
-    ...
-
-def ticks_us() -> Any:
-    """
-    Just like `ticks_ms()` above, but in microseconds.
-    """
-    ...
-
-def time_ns() -> int:
-    """
-    Similar to `time()` but returns nanoseconds since the Epoch, as an integer (usually
-    a big integer, so will allocate on the heap).
-    """
-    ...
-
-def localtime(secs: Optional[Any] = None) -> Tuple:
-    """
-    Convert the time *secs* expressed in seconds since the Epoch (see above) into an
-    8-tuple which contains: ``(year, month, mday, hour, minute, second, weekday, yearday)``
-    If *secs* is not provided or None, then the current time from the RTC is used.
-
-    The `gmtime()` function returns a date-time tuple in UTC, and `localtime()` returns a
-    date-time tuple in local time.
-
-    The format of the entries in the 8-tuple are:
-
-    * year includes the century (for example 2014).
-    * month   is 1-12
-    * mday    is 1-31
-    * hour    is 0-23
-    * minute  is 0-59
-    * second  is 0-59
-    * weekday is 0-6 for Mon-Sun
-    * yearday is 1-366
-    """
-    ...
-
-def sleep_us(us) -> None:
-    """
-    Delay for given number of microseconds, should be positive or 0.
-
-    This function attempts to provide an accurate delay of at least *us*
-    microseconds, but it may take longer if the system has other higher priority
-    processing to perform.
-    """
-    ...
-
-def gmtime(secs: Optional[Any] = None) -> Tuple:
-    """
-    Convert the time *secs* expressed in seconds since the Epoch (see above) into an
-    8-tuple which contains: ``(year, month, mday, hour, minute, second, weekday, yearday)``
-    If *secs* is not provided or None, then the current time from the RTC is used.
-
-    The `gmtime()` function returns a date-time tuple in UTC, and `localtime()` returns a
-    date-time tuple in local time.
-
-    The format of the entries in the 8-tuple are:
-
-    * year includes the century (for example 2014).
-    * month   is 1-12
-    * mday    is 1-31
-    * hour    is 0-23
-    * minute  is 0-59
-    * second  is 0-59
-    * weekday is 0-6 for Mon-Sun
-    * yearday is 1-366
-    """
-    ...
-
-def sleep_ms(ms) -> None:
-    """
-    Delay for given number of milliseconds, should be positive or 0.
-
-    This function will delay for at least the given number of milliseconds, but
-    may take longer than that if other processing must take place, for example
-    interrupt handlers or other threads.  Passing in 0 for *ms* will still allow
-    this other processing to occur.  Use `sleep_us()` for more precise delays.
-    """
-    ...
-
-def mktime() -> int:
-    """
-    This is inverse function of localtime. It's argument is a full 8-tuple
-    which expresses a time as per localtime. It returns an integer which is
-    the number of seconds since Jan 1, 2000.
-    """
-    ...
-
-def sleep(seconds) -> Any:
-    """
-    Sleep for the given number of seconds. Some boards may accept *seconds* as a
-    floating-point number to sleep for a fractional number of seconds. Note that
-    other boards may not accept a floating-point argument, for compatibility with
-    them use `sleep_ms()` and `sleep_us()` functions.
-    """
-    ...
+"""
+time related functions. See: https://docs.micropython.org/en/v1.20.0/library/time.html
+
+|see_cpython_module| :mod:`python:time` https://docs.python.org/3/library/time.html .
+
+The ``time`` module provides functions for getting the current time and date,
+measuring time intervals, and for delays.
+
+**Time Epoch**: Unix port uses standard for POSIX systems epoch of
+1970-01-01 00:00:00 UTC. However, some embedded ports use epoch of
+2000-01-01 00:00:00 UTC. Epoch year may be determined with ``gmtime(0)[0]``.
+
+**Maintaining actual calendar date/time**: This requires a
+Real Time Clock (RTC). On systems with underlying OS (including some
+RTOS), an RTC may be implicit. Setting and maintaining actual calendar
+time is responsibility of OS/RTOS and is done outside of MicroPython,
+it just uses OS API to query date/time. On baremetal ports however
+system time depends on ``machine.RTC()`` object. The current calendar time
+may be set using ``machine.RTC().datetime(tuple)`` function, and maintained
+by following means:
+
+* By a backup battery (which may be an additional, optional component for
+  a particular board).
+* Using networked time protocol (requires setup by a port/user).
+* Set manually by a user on each power-up (many boards then maintain
+  RTC time across hard resets, though some may require setting it again
+  in such case).
+
+If actual calendar time is not maintained with a system/MicroPython RTC,
+functions below which require reference to current absolute time may
+behave not as expected.
+"""
+from typing import Optional, Tuple, Any
+
+def ticks_diff(ticks1, ticks2) -> int:
+    """
+    Measure ticks difference between values returned from `ticks_ms()`, `ticks_us()`,
+    or `ticks_cpu()` functions, as a signed value which may wrap around.
+
+    The argument order is the same as for subtraction
+    operator, ``ticks_diff(ticks1, ticks2)`` has the same meaning as ``ticks1 - ticks2``.
+    However, values returned by `ticks_ms()`, etc. functions may wrap around, so
+    directly using subtraction on them will produce incorrect result. That is why
+    `ticks_diff()` is needed, it implements modular (or more specifically, ring)
+    arithmetics to produce correct result even for wrap-around values (as long as they not
+    too distant inbetween, see below). The function returns **signed** value in the range
+    [*-TICKS_PERIOD/2* .. *TICKS_PERIOD/2-1*] (that's a typical range definition for
+    two's-complement signed binary integers). If the result is negative, it means that
+    *ticks1* occurred earlier in time than *ticks2*. Otherwise, it means that
+    *ticks1* occurred after *ticks2*. This holds **only** if *ticks1* and *ticks2*
+    are apart from each other for no more than *TICKS_PERIOD/2-1* ticks. If that does
+    not hold, incorrect result will be returned. Specifically, if two tick values are
+    apart for *TICKS_PERIOD/2-1* ticks, that value will be returned by the function.
+    However, if *TICKS_PERIOD/2* of real-time ticks has passed between them, the
+    function will return *-TICKS_PERIOD/2* instead, i.e. result value will wrap around
+    to the negative range of possible values.
+
+    Informal rationale of the constraints above: Suppose you are locked in a room with no
+    means to monitor passing of time except a standard 12-notch clock. Then if you look at
+    dial-plate now, and don't look again for another 13 hours (e.g., if you fall for a
+    long sleep), then once you finally look again, it may seem to you that only 1 hour
+    has passed. To avoid this mistake, just look at the clock regularly. Your application
+    should do the same. "Too long sleep" metaphor also maps directly to application
+    behaviour: don't let your application run any single task for too long. Run tasks
+    in steps, and do time-keeping inbetween.
+
+    `ticks_diff()` is designed to accommodate various usage patterns, among them:
+
+    * Polling with timeout. In this case, the order of events is known, and you will deal
+      only with positive results of `ticks_diff()`::
+
+         # Wait for GPIO pin to be asserted, but at most 500us
+         start = time.ticks_us()
+         while pin.value() == 0:
+             if time.ticks_diff(time.ticks_us(), start) > 500:
+                 raise TimeoutError
+
+    * Scheduling events. In this case, `ticks_diff()` result may be negative
+      if an event is overdue::
+
+         # This code snippet is not optimized
+         now = time.ticks_ms()
+         scheduled_time = task.scheduled_time()
+         if ticks_diff(scheduled_time, now) > 0:
+             print("Too early, let's nap")
+             sleep_ms(ticks_diff(scheduled_time, now))
+             task.run()
+         elif ticks_diff(scheduled_time, now) == 0:
+             print("Right at time!")
+             task.run()
+         elif ticks_diff(scheduled_time, now) < 0:
+             print("Oops, running late, tell task to run faster!")
+             task.run(run_faster=true)
+
+    Note: Do not pass `time()` values to `ticks_diff()`, you should use
+    normal mathematical operations on them. But note that `time()` may (and will)
+    also overflow. This is known as https://en.wikipedia.org/wiki/Year_2038_problem .
+
+    """
+    ...
+
+def ticks_add(ticks, delta) -> Any:
+    """
+    Offset ticks value by a given number, which can be either positive or negative.
+    Given a *ticks* value, this function allows to calculate ticks value *delta*
+    ticks before or after it, following modular-arithmetic definition of tick values
+    (see `ticks_ms()` above). *ticks* parameter must be a direct result of call
+    to `ticks_ms()`, `ticks_us()`, or `ticks_cpu()` functions (or from previous
+    call to `ticks_add()`). However, *delta* can be an arbitrary integer number
+    or numeric expression. `ticks_add()` is useful for calculating deadlines for
+    events/tasks. (Note: you must use `ticks_diff()` function to work with
+    deadlines.)
+
+    Examples::
+
+         # Find out what ticks value there was 100ms ago
+         print(ticks_add(time.ticks_ms(), -100))
+
+         # Calculate deadline for operation and test for it
+         deadline = ticks_add(time.ticks_ms(), 200)
+         while ticks_diff(deadline, time.ticks_ms()) > 0:
+             do_a_little_of_something()
+
+         # Find out TICKS_MAX used by this port
+         print(ticks_add(0, -1))
+
+    """
+    ...
+
+def ticks_cpu() -> Any:
+    """
+    Similar to `ticks_ms()` and `ticks_us()`, but with the highest possible resolution
+    in the system. This is usually CPU clocks, and that's why the function is named that
+    way. But it doesn't have to be a CPU clock, some other timing source available in a
+    system (e.g. high-resolution timer) can be used instead. The exact timing unit
+    (resolution) of this function is not specified on ``time`` module level, but
+    documentation for a specific port may provide more specific information. This
+    function is intended for very fine benchmarking or very tight real-time loops.
+    Avoid using it in portable code.
+
+    Availability: Not every port implements this function.
+
+    """
+    ...
+
+class time:
+    """
+    Returns the number of seconds, as an integer, since the Epoch, assuming that
+    underlying RTC is set and maintained as described above. If an RTC is not set, this
+    function returns number of seconds since a port-specific reference point in time (for
+    embedded boards without a battery-backed RTC, usually since power up or reset). If you
+    want to develop portable MicroPython application, you should not rely on this function
+    to provide higher than second precision.  If you need higher precision, absolute
+    timestamps, use `time_ns()`.  If relative times are acceptable then use the
+    `ticks_ms()` and `ticks_us()` functions.  If you need calendar time, `gmtime()` or
+    `localtime()` without an argument is a better choice.
+    """
+
+    def __init__(self) -> None: ...
+
+def ticks_ms() -> int:
+    """
+    Returns an increasing millisecond counter with an arbitrary reference point, that
+    wraps around after some value.
+
+    The wrap-around value is not explicitly exposed, but we will
+    refer to it as *TICKS_MAX* to simplify discussion. Period of the values is
+    *TICKS_PERIOD = TICKS_MAX + 1*. *TICKS_PERIOD* is guaranteed to be a power of
+    two, but otherwise may differ from port to port. The same period value is used
+    for all of `ticks_ms()`, `ticks_us()`, `ticks_cpu()` functions (for
+    simplicity). Thus, these functions will return a value in range [*0* ..
+    *TICKS_MAX*], inclusive, total *TICKS_PERIOD* values. Note that only
+    non-negative values are used. For the most part, you should treat values returned
+    by these functions as opaque. The only operations available for them are
+    `ticks_diff()` and `ticks_add()` functions described below.
+
+    Note: Performing standard mathematical operations (+, -) or relational
+    operators (<, <=, >, >=) directly on these value will lead to invalid
+    result. Performing mathematical operations and then passing their results
+    as arguments to `ticks_diff()` or `ticks_add()` will also lead to
+    invalid results from the latter functions.
+    """
+    ...
+
+def ticks_us() -> Any:
+    """
+    Just like `ticks_ms()` above, but in microseconds.
+    """
+    ...
+
+def time_ns() -> int:
+    """
+    Similar to `time()` but returns nanoseconds since the Epoch, as an integer (usually
+    a big integer, so will allocate on the heap).
+    """
+    ...
+
+def localtime(secs: Optional[Any] = None) -> Tuple:
+    """
+    Convert the time *secs* expressed in seconds since the Epoch (see above) into an
+    8-tuple which contains: ``(year, month, mday, hour, minute, second, weekday, yearday)``
+    If *secs* is not provided or None, then the current time from the RTC is used.
+
+    The `gmtime()` function returns a date-time tuple in UTC, and `localtime()` returns a
+    date-time tuple in local time.
+
+    The format of the entries in the 8-tuple are:
+
+    * year includes the century (for example 2014).
+    * month   is 1-12
+    * mday    is 1-31
+    * hour    is 0-23
+    * minute  is 0-59
+    * second  is 0-59
+    * weekday is 0-6 for Mon-Sun
+    * yearday is 1-366
+    """
+    ...
+
+def sleep_us(us) -> None:
+    """
+    Delay for given number of microseconds, should be positive or 0.
+
+    This function attempts to provide an accurate delay of at least *us*
+    microseconds, but it may take longer if the system has other higher priority
+    processing to perform.
+    """
+    ...
+
+def gmtime(secs: Optional[Any] = None) -> Tuple:
+    """
+    Convert the time *secs* expressed in seconds since the Epoch (see above) into an
+    8-tuple which contains: ``(year, month, mday, hour, minute, second, weekday, yearday)``
+    If *secs* is not provided or None, then the current time from the RTC is used.
+
+    The `gmtime()` function returns a date-time tuple in UTC, and `localtime()` returns a
+    date-time tuple in local time.
+
+    The format of the entries in the 8-tuple are:
+
+    * year includes the century (for example 2014).
+    * month   is 1-12
+    * mday    is 1-31
+    * hour    is 0-23
+    * minute  is 0-59
+    * second  is 0-59
+    * weekday is 0-6 for Mon-Sun
+    * yearday is 1-366
+    """
+    ...
+
+def sleep_ms(ms) -> None:
+    """
+    Delay for given number of milliseconds, should be positive or 0.
+
+    This function will delay for at least the given number of milliseconds, but
+    may take longer than that if other processing must take place, for example
+    interrupt handlers or other threads.  Passing in 0 for *ms* will still allow
+    this other processing to occur.  Use `sleep_us()` for more precise delays.
+    """
+    ...
+
+def mktime() -> int:
+    """
+    This is inverse function of localtime. It's argument is a full 8-tuple
+    which expresses a time as per localtime. It returns an integer which is
+    the number of seconds since Jan 1, 2000.
+    """
+    ...
+
+def sleep(seconds) -> Any:
+    """
+    Sleep for the given number of seconds. Some boards may accept *seconds* as a
+    floating-point number to sleep for a fractional number of seconds. Note that
+    other boards may not accept a floating-point argument, for compatibility with
+    them use `sleep_ms()` and `sleep_us()` functions.
+    """
+    ...
```

### Comparing `micropython_rp2_stubs-1.19.1.post9/uarray.pyi` & `micropython_rp2_stubs-1.20.0.post1/uarray.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,30 @@
-"""
-efficient arrays of numeric data. See: https://docs.micropython.org/en/v1.19.1/library/array.html
-
-|see_cpython_module| :mod:`python:array` https://docs.python.org/3/library/array.html .
-
-Supported format codes: ``b``, ``B``, ``h``, ``H``, ``i``, ``I``, ``l``,
-``L``, ``q``, ``Q``, ``f``, ``d`` (the latter 2 depending on the
-floating-point support).
-"""
-from typing import Optional, Any
-
-class array:
-    """
-    Create array with elements of given type. Initial contents of the
-    array are given by *iterable*. If it is not provided, an empty
-    array is created.
-    """
-
-    def extend(self, iterable) -> Any:
-        """
-        Append new elements as contained in *iterable* to the end of
-        array, growing it.
-        """
-        ...
-    def decode(self, *args, **kwargs) -> Any: ...
-    def append(self, val) -> Any:
-        """
-        Append new element *val* to the end of array, growing it.
-        """
-        ...
-    def __init__(self, typecode, iterable: Optional[Any] = None) -> None: ...
+"""
+efficient arrays of numeric data. See: https://docs.micropython.org/en/v1.20.0/library/array.html
+
+|see_cpython_module| :mod:`python:array` https://docs.python.org/3/library/array.html .
+
+Supported format codes: ``b``, ``B``, ``h``, ``H``, ``i``, ``I``, ``l``,
+``L``, ``q``, ``Q``, ``f``, ``d`` (the latter 2 depending on the
+floating-point support).
+"""
+from typing import List, Optional, Any
+
+class array:
+    """
+    Create array with elements of given type. Initial contents of the
+    array are given by *iterable*. If it is not provided, an empty
+    array is created.
+    """
+
+    def extend(self, iterable) -> Any:
+        """
+        Append new elements as contained in *iterable* to the end of
+        array, growing it.
+        """
+        ...
+    def append(self, val) -> Any:
+        """
+        Append new element *val* to the end of array, growing it.
+        """
+        ...
+    def __init__(self, typecode, iterable: Optional[Any] = None) -> None: ...
```

### Comparing `micropython_rp2_stubs-1.19.1.post9/uasyncio/core.pyi` & `micropython_rp2_stubs-1.20.0.post1/rp2.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -1,52 +1,62 @@
-from .task import Task as Task, TaskQueue as TaskQueue
-from _typeshed import Incomplete
-
-class CancelledError(BaseException): ...
-class TimeoutError(Exception): ...
-
-_exc_context: Incomplete
-
-class SingletonGenerator:
-    state: Incomplete
-    exc: Incomplete
-    def __init__(self) -> None: ...
-    def __iter__(self): ...
-    def __next__(self) -> None: ...
-
-def sleep_ms(t, sgen=...): ...
-def sleep(t): ...
-
-class IOQueue:
-    poller: Incomplete
-    map: Incomplete
-    def __init__(self) -> None: ...
-    def _enqueue(self, s, idx) -> None: ...
-    def _dequeue(self, s) -> None: ...
-    def queue_read(self, s) -> None: ...
-    def queue_write(self, s) -> None: ...
-    def remove(self, task) -> None: ...
-    def wait_io_event(self, dt) -> None: ...
-
-def _promote_to_task(aw): ...
-def create_task(coro): ...
-def run_until_complete(main_task: Incomplete | None = ...): ...
-def run(coro): ...
-async def _stopper() -> None: ...
-
-_stop_task: Incomplete
-
-class Loop:
-    _exc_handler: Incomplete
-    def create_task(coro): ...
-    def run_forever() -> None: ...
-    def run_until_complete(aw): ...
-    def stop() -> None: ...
-    def close() -> None: ...
-    def set_exception_handler(handler) -> None: ...
-    def get_exception_handler(): ...
-    def default_exception_handler(loop, context) -> None: ...
-    def call_exception_handler(context) -> None: ...
-
-def get_event_loop(runq_len: int = ..., waitq_len: int = ...): ...
-def current_task(): ...
-def new_event_loop(): ...
+from _rp2 import *
+from _typeshed import Incomplete
+
+_PROG_DATA: Incomplete
+_PROG_OFFSET_PIO0: Incomplete
+_PROG_OFFSET_PIO1: Incomplete
+_PROG_EXECCTRL: Incomplete
+_PROG_SHIFTCTRL: Incomplete
+_PROG_OUT_PINS: Incomplete
+_PROG_SET_PINS: Incomplete
+_PROG_SIDESET_PINS: Incomplete
+_PROG_MAX_FIELDS: Incomplete
+
+class PIOASMError(Exception): ...
+
+class PIOASMEmit:
+    labels: Incomplete
+    prog: Incomplete
+    wrap_used: bool
+    sideset_count: int
+    def __init__(
+        self,
+        *,
+        out_init: Incomplete | None = ...,
+        set_init: Incomplete | None = ...,
+        sideset_init: Incomplete | None = ...,
+        in_shiftdir: int = ...,
+        out_shiftdir: int = ...,
+        autopush: bool = ...,
+        autopull: bool = ...,
+        push_thresh: int = ...,
+        pull_thresh: int = ...,
+        fifo_join: int = ...,
+    ) -> None: ...
+    delay_max: int
+    sideset_opt: Incomplete
+    pass_: Incomplete
+    num_instr: int
+    num_sideset: int
+    def start_pass(self, pass_) -> None: ...
+    def __getitem__(self, key): ...
+    def delay(self, delay): ...
+    def side(self, value): ...
+    def wrap_target(self) -> None: ...
+    def wrap(self) -> None: ...
+    def label(self, label) -> None: ...
+    def word(self, instr, label: Incomplete | None = ...): ...
+    def nop(self): ...
+    def jmp(self, cond, label: Incomplete | None = ...): ...
+    def wait(self, polarity, src, index): ...
+    def in_(self, src, data): ...
+    def out(self, dest, data): ...
+    def push(self, value: int = ..., value2: int = ...): ...
+    def pull(self, value: int = ..., value2: int = ...): ...
+    def mov(self, dest, src): ...
+    def irq(self, mod, index: Incomplete | None = ...): ...
+    def set(self, dest, data): ...
+
+_pio_funcs: Incomplete
+
+def asm_pio(**kw): ...
+def asm_pio_encode(instr, sideset_count, sideset_opt: bool = ...): ...
```

### Comparing `micropython_rp2_stubs-1.19.1.post9/uasyncio/event.pyi` & `micropython_rp2_stubs-1.20.0.post1/uasyncio/event.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,21 @@
-import uio
-from . import core as core
-from _typeshed import Incomplete
-from collections.abc import Generator
-
-class Event:
-    state: bool
-    waiting: Incomplete
-    def __init__(self) -> None: ...
-    def is_set(self): ...
-    def set(self) -> None: ...
-    def clear(self) -> None: ...
-    async def wait(self) -> Generator[None, None, Incomplete]: ...
-
-class ThreadSafeFlag(uio.IOBase):
-    _flag: int
-    def __init__(self) -> None: ...
-    def ioctl(self, req, flags): ...
-    def set(self) -> None: ...
-    async def wait(self) -> Generator[Incomplete, None, None]: ...
+import uio
+from . import core as core
+from _typeshed import Incomplete
+from collections.abc import Generator
+
+class Event:
+    state: bool
+    waiting: Incomplete
+    def __init__(self) -> None: ...
+    def is_set(self): ...
+    def set(self) -> None: ...
+    def clear(self) -> None: ...
+    def wait(self) -> Generator[None, None, Incomplete]: ...
+
+class ThreadSafeFlag(uio.IOBase):
+    state: int
+    def __init__(self) -> None: ...
+    def ioctl(self, req, flags): ...
+    def set(self) -> None: ...
+    def clear(self) -> None: ...
+    async def wait(self) -> Generator[Incomplete, None, None]: ...
```

### Comparing `micropython_rp2_stubs-1.19.1.post9/uasyncio/stream.pyi` & `micropython_rp2_stubs-1.20.0.post1/uasyncio/stream.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-from . import core as core
-from _typeshed import Incomplete
-from collections.abc import Generator
-
-class Stream:
-    s: Incomplete
-    e: Incomplete
-    out_buf: bytes
-    def __init__(self, s, e=...) -> None: ...
-    def get_extra_info(self, v): ...
-    async def __aenter__(self): ...
-    async def __aexit__(self, exc_type, exc, tb) -> None: ...
-    def close(self) -> None: ...
-    async def wait_closed(self) -> None: ...
-    async def read(self, n) -> Generator[Incomplete, None, Incomplete]: ...
-    async def readinto(self, buf) -> Generator[Incomplete, None, Incomplete]: ...
-    async def readexactly(self, n) -> Generator[Incomplete, None, Incomplete]: ...
-    async def readline(self) -> Generator[Incomplete, None, Incomplete]: ...
-    def write(self, buf) -> None: ...
-    async def drain(self) -> Generator[Incomplete, None, None]: ...
-
-StreamReader = Stream
-StreamWriter = Stream
-
-async def open_connection(host, port) -> Generator[Incomplete, None, Incomplete]: ...
-
-class Server:
-    async def __aenter__(self): ...
-    async def __aexit__(self, exc_type, exc, tb) -> None: ...
-    def close(self) -> None: ...
-    async def wait_closed(self) -> None: ...
-    async def _serve(self, s, cb) -> Generator[Incomplete, None, None]: ...
-
-async def start_server(cb, host, port, backlog: int = ...): ...
-async def stream_awrite(self, buf, off: int = ..., sz: int = ...) -> None: ...
+from . import core as core
+from _typeshed import Incomplete
+from collections.abc import Generator
+
+class Stream:
+    s: Incomplete
+    e: Incomplete
+    out_buf: bytes
+    def __init__(self, s, e=...) -> None: ...
+    def get_extra_info(self, v): ...
+    async def __aenter__(self): ...
+    async def __aexit__(self, exc_type, exc, tb) -> None: ...
+    def close(self) -> None: ...
+    async def wait_closed(self) -> None: ...
+    def read(self, n: int = ...) -> Generator[Incomplete, None, Incomplete]: ...
+    def readinto(self, buf) -> Generator[Incomplete, None, Incomplete]: ...
+    def readexactly(self, n) -> Generator[Incomplete, None, Incomplete]: ...
+    def readline(self) -> Generator[Incomplete, None, Incomplete]: ...
+    def write(self, buf) -> None: ...
+    def drain(self) -> Generator[Incomplete, None, Incomplete]: ...
+
+StreamReader = Stream
+StreamWriter = Stream
+
+def open_connection(host, port) -> Generator[Incomplete, None, Incomplete]: ...
+
+class Server:
+    async def __aenter__(self): ...
+    async def __aexit__(self, exc_type, exc, tb) -> None: ...
+    def close(self) -> None: ...
+    async def wait_closed(self) -> None: ...
+    async def _serve(self, s, cb) -> Generator[Incomplete, None, None]: ...
+
+async def start_server(cb, host, port, backlog: int = ...): ...
+async def stream_awrite(self, buf, off: int = ..., sz: int = ...) -> None: ...
```

### Comparing `micropython_rp2_stubs-1.19.1.post9/ubinascii.pyi` & `micropython_rp2_stubs-1.20.0.post1/ubinascii.pyi`

 * *Files 13% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-"""
-binary/ASCII conversions. See: https://docs.micropython.org/en/v1.19.1/library/binascii.html
-
-|see_cpython_module| :mod:`python:binascii` https://docs.python.org/3/library/binascii.html .
-
-This module implements conversions between binary data and various
-encodings of it in ASCII form (in both directions).
-"""
-from typing import Optional, Any
-
-def crc32(*args, **kwargs) -> Any: ...
-def hexlify(data, sep: Optional[Any] = None) -> bytes:
-    """
-    Convert the bytes in the *data* object to a hexadecimal representation.
-    Returns a bytes object.
-
-    If the additional argument *sep* is supplied it is used as a separator
-    between hexadecimal values.
-    """
-    ...
-
-def unhexlify(data) -> bytes:
-    """
-    Convert hexadecimal data to binary representation. Returns bytes string.
-    (i.e. inverse of hexlify)
-    """
-    ...
-
-def b2a_base64(data, *, newline=True) -> bytes:
-    """
-    Encode binary data in base64 format, as in `RFC 3548
-    <https://tools.ietf.org/html/rfc3548.html>`_. Returns the encoded data
-    followed by a newline character if newline is true, as a bytes object.
-    """
-    ...
-
-def a2b_base64(data) -> bytes:
-    """
-    Decode base64-encoded data, ignoring invalid characters in the input.
-    Conforms to `RFC 2045 s.6.8 <https://tools.ietf.org/html/rfc2045#section-6.8>`_.
-    Returns a bytes object.
-    """
-    ...
+"""
+binary/ASCII conversions. See: https://docs.micropython.org/en/v1.20.0/library/binascii.html
+
+|see_cpython_module| :mod:`python:binascii` https://docs.python.org/3/library/binascii.html .
+
+This module implements conversions between binary data and various
+encodings of it in ASCII form (in both directions).
+"""
+from typing import Optional, Any
+
+def crc32(*args, **kwargs) -> Any: ...
+def hexlify(data, sep: Optional[Any] = None) -> bytes:
+    """
+    Convert the bytes in the *data* object to a hexadecimal representation.
+    Returns a bytes object.
+
+    If the additional argument *sep* is supplied it is used as a separator
+    between hexadecimal values.
+    """
+    ...
+
+def unhexlify(data) -> bytes:
+    """
+    Convert hexadecimal data to binary representation. Returns bytes string.
+    (i.e. inverse of hexlify)
+    """
+    ...
+
+def b2a_base64(data, *, newline=True) -> bytes:
+    """
+    Encode binary data in base64 format, as in `RFC 3548
+    <https://tools.ietf.org/html/rfc3548.html>`_. Returns the encoded data
+    followed by a newline character if newline is true, as a bytes object.
+    """
+    ...
+
+def a2b_base64(data) -> bytes:
+    """
+    Decode base64-encoded data, ignoring invalid characters in the input.
+    Conforms to `RFC 2045 s.6.8 <https://tools.ietf.org/html/rfc2045#section-6.8>`_.
+    Returns a bytes object.
+    """
+    ...
```

### Comparing `micropython_rp2_stubs-1.19.1.post9/ucollections.pyi` & `micropython_rp2_stubs-1.20.0.post1/collections.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -1,101 +1,101 @@
-"""
-collection and container types. See: https://docs.micropython.org/en/v1.19.1/library/collections.html
-
-|see_cpython_module| :mod:`python:collections` https://docs.python.org/3/library/collections.html .
-
-This module implements advanced collection and container types to
-hold/accumulate various objects.
-"""
-from typing import Optional, Any
-from queue import Queue
-
-def namedtuple(name, fields) -> Any:
-    """
-    This is factory function to create a new namedtuple type with a specific
-    name and set of fields. A namedtuple is a subclass of tuple which allows
-    to access its fields not just by numeric index, but also with an attribute
-    access syntax using symbolic field names. Fields is a sequence of strings
-    specifying field names. For compatibility with CPython it can also be a
-    a string with space-separated field named (but this is less efficient).
-    Example of use::
-
-        from collections import namedtuple
-
-        MyTuple = namedtuple("MyTuple", ("id", "name"))
-        t1 = MyTuple(1, "foo")
-        t2 = MyTuple(2, "bar")
-        print(t1.name)
-        assert t2.name == t2[1]
-    """
-    ...
-
-class OrderedDict:
-    """
-    ``dict`` type subclass which remembers and preserves the order of keys
-    added. When ordered dict is iterated over, keys/items are returned in
-    the order they were added::
-
-        from collections import OrderedDict
-
-        # To make benefit of ordered keys, OrderedDict should be initialized
-        # from sequence of (key, value) pairs.
-        d = OrderedDict([("z", 1), ("a", 2)])
-        # More items can be added as usual
-        d["w"] = 5
-        d["b"] = 3
-        for k, v in d.items():
-            print(k, v)
-
-    Output::
-
-        z 1
-        a 2
-        w 5
-        b 3
-    """
-
-    def popitem(self, *args, **kwargs) -> Any: ...
-    def pop(self, *args, **kwargs) -> Any: ...
-    def values(self, *args, **kwargs) -> Any: ...
-    def setdefault(self, *args, **kwargs) -> Any: ...
-    def update(self, *args, **kwargs) -> Any: ...
-    def copy(self, *args, **kwargs) -> Any: ...
-    def clear(self, *args, **kwargs) -> Any: ...
-    def keys(self, *args, **kwargs) -> Any: ...
-    def get(self, *args, **kwargs) -> Any: ...
-    def items(self, *args, **kwargs) -> Any: ...
-    @classmethod
-    def fromkeys(cls, *args, **kwargs) -> Any: ...
-    def __init__(self, *args, **kwargs) -> None: ...
-
-class deque:
-    """
-    Deques (double-ended queues) are a list-like container that support O(1)
-    appends and pops from either side of the deque.  New deques are created
-    using the following arguments:
-
-        - *iterable* must be the empty tuple, and the new deque is created empty.
-
-        - *maxlen* must be specified and the deque will be bounded to this
-          maximum length.  Once the deque is full, any new items added will
-          discard items from the opposite end.
-
-        - The optional *flags* can be 1 to check for overflow when adding items.
-
-    As well as supporting `bool` and `len`, deque objects have the following
-    methods:
-    """
-
-    def popleft(self) -> Any:
-        """
-        Remove and return an item from the left side of the deque.
-        Raises IndexError if no items are present.
-        """
-        ...
-    def append(self, x) -> Any:
-        """
-        Add *x* to the right side of the deque.
-        Raises IndexError if overflow checking is enabled and there is no more room left.
-        """
-        ...
-    def __init__(self, iterable, maxlen, flags: Optional[Any] = None) -> None: ...
+"""
+collection and container types. See: https://docs.micropython.org/en/v1.20.0/library/collections.html
+
+|see_cpython_module| :mod:`python:collections` https://docs.python.org/3/library/collections.html .
+
+This module implements advanced collection and container types to
+hold/accumulate various objects.
+"""
+from typing import Optional, Any
+from queue import Queue
+
+def namedtuple(name, fields) -> Any:
+    """
+    This is factory function to create a new namedtuple type with a specific
+    name and set of fields. A namedtuple is a subclass of tuple which allows
+    to access its fields not just by numeric index, but also with an attribute
+    access syntax using symbolic field names. Fields is a sequence of strings
+    specifying field names. For compatibility with CPython it can also be a
+    a string with space-separated field named (but this is less efficient).
+    Example of use::
+
+        from collections import namedtuple
+
+        MyTuple = namedtuple("MyTuple", ("id", "name"))
+        t1 = MyTuple(1, "foo")
+        t2 = MyTuple(2, "bar")
+        print(t1.name)
+        assert t2.name == t2[1]
+    """
+    ...
+
+class OrderedDict(dict):
+    """
+    ``dict`` type subclass which remembers and preserves the order of keys
+    added. When ordered dict is iterated over, keys/items are returned in
+    the order they were added::
+
+        from collections import OrderedDict
+
+        # To make benefit of ordered keys, OrderedDict should be initialized
+        # from sequence of (key, value) pairs.
+        d = OrderedDict([("z", 1), ("a", 2)])
+        # More items can be added as usual
+        d["w"] = 5
+        d["b"] = 3
+        for k, v in d.items():
+            print(k, v)
+
+    Output::
+
+        z 1
+        a 2
+        w 5
+        b 3
+    """
+
+    def popitem(self, *args, **kwargs) -> Any: ...
+    def pop(self, *args, **kwargs) -> Any: ...
+    def values(self, *args, **kwargs) -> Any: ...
+    def setdefault(self, *args, **kwargs) -> Any: ...
+    def update(self, *args, **kwargs) -> Any: ...
+    def copy(self, *args, **kwargs) -> Any: ...
+    def clear(self, *args, **kwargs) -> Any: ...
+    def keys(self, *args, **kwargs) -> Any: ...
+    def get(self, *args, **kwargs) -> Any: ...
+    def items(self, *args, **kwargs) -> Any: ...
+    @classmethod
+    def fromkeys(cls, *args, **kwargs) -> Any: ...
+    def __init__(self, *args, **kwargs) -> None: ...
+
+class deque(Queue):
+    """
+    Deques (double-ended queues) are a list-like container that support O(1)
+    appends and pops from either side of the deque.  New deques are created
+    using the following arguments:
+
+        - *iterable* must be the empty tuple, and the new deque is created empty.
+
+        - *maxlen* must be specified and the deque will be bounded to this
+          maximum length.  Once the deque is full, any new items added will
+          discard items from the opposite end.
+
+        - The optional *flags* can be 1 to check for overflow when adding items.
+
+    As well as supporting `bool` and `len`, deque objects have the following
+    methods:
+    """
+
+    def popleft(self) -> Any:
+        """
+        Remove and return an item from the left side of the deque.
+        Raises IndexError if no items are present.
+        """
+        ...
+    def append(self, x) -> Any:
+        """
+        Add *x* to the right side of the deque.
+        Raises IndexError if overflow checking is enabled and there is no more room left.
+        """
+        ...
+    def __init__(self, iterable, maxlen, flags: Optional[Any] = None) -> None: ...
```

### Comparing `micropython_rp2_stubs-1.19.1.post9/ucryptolib.pyi` & `micropython_rp2_stubs-1.20.0.post1/cryptolib.pyi`

 * *Files 26% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-"""
-cryptographic ciphers. See: https://docs.micropython.org/en/v1.19.1/library/cryptolib.html
-"""
-from typing import Optional, Any
-
-class aes:
-    def encrypt(self, in_buf, out_buf: Optional[Any] = None) -> Any:
-        """
-        Encrypt *in_buf*. If no *out_buf* is given result is returned as a
-        newly allocated `bytes` object. Otherwise, result is written into
-        mutable buffer *out_buf*. *in_buf* and *out_buf* can also refer
-        to the same mutable buffer, in which case data is encrypted in-place.
-        """
-        ...
-    def decrypt(self, in_buf, out_buf: Optional[Any] = None) -> Any:
-        """
-        Like `encrypt()`, but for decryption.
-        """
-        ...
-    def __init__(self, key, mode, IV: Optional[Any] = None) -> None:
-        """
-        Initialize cipher object, suitable for encryption/decryption. Note:
-        after initialization, cipher object can be use only either for
-        encryption or decryption. Running decrypt() operation after encrypt()
-        or vice versa is not supported.
-
-        Parameters are:
-
-            * *key* is an encryption/decryption key (bytes-like).
-            * *mode* is:
-
-                * ``1`` (or ``cryptolib.MODE_ECB`` if it exists) for Electronic Code Book (ECB).
-                * ``2`` (or ``cryptolib.MODE_CBC`` if it exists) for Cipher Block Chaining (CBC).
-                * ``6`` (or ``cryptolib.MODE_CTR`` if it exists) for Counter mode (CTR).
-
-            * *IV* is an initialization vector for CBC mode.
-            * For Counter mode, *IV* is the initial value for the counter.
-        """
-        ...
+"""
+cryptographic ciphers. See: https://docs.micropython.org/en/v1.20.0/library/cryptolib.html
+"""
+from typing import Optional, Any
+
+class aes:
+    def encrypt(self, in_buf, out_buf: Optional[Any] = None) -> Any:
+        """
+        Encrypt *in_buf*. If no *out_buf* is given result is returned as a
+        newly allocated `bytes` object. Otherwise, result is written into
+        mutable buffer *out_buf*. *in_buf* and *out_buf* can also refer
+        to the same mutable buffer, in which case data is encrypted in-place.
+        """
+        ...
+    def decrypt(self, in_buf, out_buf: Optional[Any] = None) -> Any:
+        """
+        Like `encrypt()`, but for decryption.
+        """
+        ...
+    def __init__(self, key, mode, IV: Optional[Any] = None) -> None:
+        """
+        Initialize cipher object, suitable for encryption/decryption. Note:
+        after initialization, cipher object can be use only either for
+        encryption or decryption. Running decrypt() operation after encrypt()
+        or vice versa is not supported.
+
+        Parameters are:
+
+            * *key* is an encryption/decryption key (bytes-like).
+            * *mode* is:
+
+                * ``1`` (or ``cryptolib.MODE_ECB`` if it exists) for Electronic Code Book (ECB).
+                * ``2`` (or ``cryptolib.MODE_CBC`` if it exists) for Cipher Block Chaining (CBC).
+                * ``6`` (or ``cryptolib.MODE_CTR`` if it exists) for Counter mode (CTR).
+
+            * *IV* is an initialization vector for CBC mode.
+            * For Counter mode, *IV* is the initial value for the counter.
+        """
+        ...
```

### Comparing `micropython_rp2_stubs-1.19.1.post9/uctypes.pyi` & `micropython_rp2_stubs-1.20.0.post1/uctypes.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -1,86 +1,86 @@
-"""
-access binary data in a structured way. See: https://docs.micropython.org/en/v1.19.1/library/uctypes.html
-
-This module implements "foreign data interface" for MicroPython. The idea
-behind it is similar to CPython's ``ctypes`` modules, but the actual API is
-different, streamlined and optimized for small size. The basic idea of the
-module is to define data structure layout with about the same power as the
-C language allows, and then access it using familiar dot-syntax to reference
-sub-fields.
-"""
-from typing import Any
-
-VOID: int
-NATIVE: int
-PTR: int
-SHORT: int
-LONGLONG: int
-INT8: int
-LITTLE_ENDIAN: int
-LONG: int
-UINT: int
-ULONG: int
-ULONGLONG: int
-USHORT: int
-UINT8: int
-UINT16: int
-UINT32: int
-UINT64: int
-INT64: int
-BFUINT16: int
-BFUINT32: int
-BFUINT8: int
-BFINT8: int
-ARRAY: int
-BFINT16: int
-BFINT32: int
-BF_LEN: int
-INT: int
-INT16: int
-INT32: int
-FLOAT64: int
-BF_POS: int
-BIG_ENDIAN: int
-FLOAT32: int
-
-def sizeof(struct, layout_type=NATIVE, /) -> int:
-    """
-    Return size of data structure in bytes. The *struct* argument can be
-    either a structure class or a specific instantiated structure object
-    (or its aggregate field).
-    """
-    ...
-
-def bytes_at(addr, size) -> bytes:
-    """
-    Capture memory at the given address and size as bytes object. As bytes
-    object is immutable, memory is actually duplicated and copied into
-    bytes object, so if memory contents change later, created object
-    retains original value.
-    """
-    ...
-
-def bytearray_at(addr, size) -> bytearray:
-    """
-    Capture memory at the given address and size as bytearray object.
-    Unlike bytes_at() function above, memory is captured by reference,
-    so it can be both written too, and you will access current value
-    at the given memory address.
-    """
-    ...
-
-def addressof(obj) -> int:
-    """
-    Return address of an object. Argument should be bytes, bytearray or
-    other object supporting buffer protocol (and address of this buffer
-    is what actually returned).
-    """
-    ...
-
-class struct:
-    """
-    Instantiate a "foreign data structure" object based on structure address in
-    memory, descriptor (encoded as a dictionary), and layout type (see below).
-    """
-
-    def __init__(self, addr, descriptor, layout_type=NATIVE, /) -> None: ...
+"""
+access binary data in a structured way. See: https://docs.micropython.org/en/v1.20.0/library/uctypes.html
+
+This module implements "foreign data interface" for MicroPython. The idea
+behind it is similar to CPython's ``ctypes`` modules, but the actual API is
+different, streamlined and optimized for small size. The basic idea of the
+module is to define data structure layout with about the same power as the
+C language allows, and then access it using familiar dot-syntax to reference
+sub-fields.
+"""
+from typing import Any
+
+VOID: int
+NATIVE: int
+PTR: int
+SHORT: int
+LONGLONG: int
+INT8: int
+LITTLE_ENDIAN: int
+LONG: int
+UINT: int
+ULONG: int
+ULONGLONG: int
+USHORT: int
+UINT8: int
+UINT16: int
+UINT32: int
+UINT64: int
+INT64: int
+BFUINT16: int
+BFUINT32: int
+BFUINT8: int
+BFINT8: int
+ARRAY: int
+BFINT16: int
+BFINT32: int
+BF_LEN: int
+INT: int
+INT16: int
+INT32: int
+FLOAT64: int
+BF_POS: int
+BIG_ENDIAN: int
+FLOAT32: int
+
+def sizeof(struct, layout_type=NATIVE, /) -> int:
+    """
+    Return size of data structure in bytes. The *struct* argument can be
+    either a structure class or a specific instantiated structure object
+    (or its aggregate field).
+    """
+    ...
+
+def bytes_at(addr, size) -> bytes:
+    """
+    Capture memory at the given address and size as bytes object. As bytes
+    object is immutable, memory is actually duplicated and copied into
+    bytes object, so if memory contents change later, created object
+    retains original value.
+    """
+    ...
+
+def bytearray_at(addr, size) -> bytearray:
+    """
+    Capture memory at the given address and size as bytearray object.
+    Unlike bytes_at() function above, memory is captured by reference,
+    so it can be both written too, and you will access current value
+    at the given memory address.
+    """
+    ...
+
+def addressof(obj) -> int:
+    """
+    Return address of an object. Argument should be bytes, bytearray or
+    other object supporting buffer protocol (and address of this buffer
+    is what actually returned).
+    """
+    ...
+
+class struct:
+    """
+    Instantiate a "foreign data structure" object based on structure address in
+    memory, descriptor (encoded as a dictionary), and layout type (see below).
+    """
+
+    def __init__(self, addr, descriptor, layout_type=NATIVE, /) -> None: ...
```

### Comparing `micropython_rp2_stubs-1.19.1.post9/uhashlib.pyi` & `micropython_rp2_stubs-1.20.0.post1/uhashlib.pyi`

 * *Files 13% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-"""
-hashing algorithms. See: https://docs.micropython.org/en/v1.19.1/library/hashlib.html
-
-|see_cpython_module| :mod:`python:hashlib` https://docs.python.org/3/library/hashlib.html .
-
-This module implements binary data hashing algorithms. The exact inventory
-of available algorithms depends on a board. Among the algorithms which may
-be implemented:
-
-* SHA256 - The current generation, modern hashing algorithm (of SHA2 series).
-  It is suitable for cryptographically-secure purposes. Included in the
-  MicroPython core and any board is recommended to provide this, unless
-  it has particular code size constraints.
-
-* SHA1 - A previous generation algorithm. Not recommended for new usages,
-  but SHA1 is a part of number of Internet standards and existing
-  applications, so boards targeting network connectivity and
-  interoperability will try to provide this.
-
-* MD5 - A legacy algorithm, not considered cryptographically secure. Only
-  selected boards, targeting interoperability with legacy applications,
-  will offer this.
-"""
-from typing import Optional, Any
-
-class sha256:
-    """
-    Create an SHA256 hasher object and optionally feed ``data`` into it.
-    """
-
-    def digest(self, *args, **kwargs) -> Any: ...
-    def update(self, *args, **kwargs) -> Any: ...
-    def __init__(self, data: Optional[Any] = None) -> None: ...
-
-class sha1:
-    """
-    Create an SHA1 hasher object and optionally feed ``data`` into it.
-    """
-
-    def digest(self, *args, **kwargs) -> Any: ...
-    def update(self, *args, **kwargs) -> Any: ...
-    def __init__(self, data: Optional[Any] = None) -> None: ...
+"""
+hashing algorithms. See: https://docs.micropython.org/en/v1.20.0/library/hashlib.html
+
+|see_cpython_module| :mod:`python:hashlib` https://docs.python.org/3/library/hashlib.html .
+
+This module implements binary data hashing algorithms. The exact inventory
+of available algorithms depends on a board. Among the algorithms which may
+be implemented:
+
+* SHA256 - The current generation, modern hashing algorithm (of SHA2 series).
+  It is suitable for cryptographically-secure purposes. Included in the
+  MicroPython core and any board is recommended to provide this, unless
+  it has particular code size constraints.
+
+* SHA1 - A previous generation algorithm. Not recommended for new usages,
+  but SHA1 is a part of number of Internet standards and existing
+  applications, so boards targeting network connectivity and
+  interoperability will try to provide this.
+
+* MD5 - A legacy algorithm, not considered cryptographically secure. Only
+  selected boards, targeting interoperability with legacy applications,
+  will offer this.
+"""
+from typing import Optional, Any
+
+class sha256:
+    """
+    Create an SHA256 hasher object and optionally feed ``data`` into it.
+    """
+
+    def digest(self, *args, **kwargs) -> Any: ...
+    def update(self, *args, **kwargs) -> Any: ...
+    def __init__(self, data: Optional[Any] = None) -> None: ...
+
+class sha1:
+    """
+    Create an SHA1 hasher object and optionally feed ``data`` into it.
+    """
+
+    def digest(self, *args, **kwargs) -> Any: ...
+    def update(self, *args, **kwargs) -> Any: ...
+    def __init__(self, data: Optional[Any] = None) -> None: ...
```

### Comparing `micropython_rp2_stubs-1.19.1.post9/uheapq.pyi` & `micropython_rp2_stubs-1.20.0.post1/uheapq.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-"""
-heap queue algorithm. See: https://docs.micropython.org/en/v1.19.1/library/heapq.html
-
-|see_cpython_module| :mod:`python:heapq` https://docs.python.org/3/library/heapq.html .
-
-This module implements the
-`min heap queue algorithm <https://en.wikipedia.org/wiki/Heap_%28data_structure%29>`_.
-
-A heap queue is essentially a list that has its elements stored in such a way
-that the first item of the list is always the smallest.
-"""
-from typing import Any
-
-def heappop(heap) -> Any:
-    """
-    Pop the first item from the ``heap``, and return it.  Raise ``IndexError`` if
-    ``heap`` is empty.
-
-    The returned item will be the smallest item in the ``heap``.
-    """
-    ...
-
-def heappush(heap, item) -> Any:
-    """
-    Push the ``item`` onto the ``heap``.
-    """
-    ...
-
-def heapify(x) -> Any:
-    """
-    Convert the list ``x`` into a heap.  This is an in-place operation.
-    """
-    ...
+"""
+heap queue algorithm. See: https://docs.micropython.org/en/v1.20.0/library/heapq.html
+
+|see_cpython_module| :mod:`python:heapq` https://docs.python.org/3/library/heapq.html .
+
+This module implements the
+`min heap queue algorithm <https://en.wikipedia.org/wiki/Heap_%28data_structure%29>`_.
+
+A heap queue is essentially a list that has its elements stored in such a way
+that the first item of the list is always the smallest.
+"""
+from typing import Any
+
+def heappop(heap) -> Any:
+    """
+    Pop the first item from the ``heap``, and return it.  Raise ``IndexError`` if
+    ``heap`` is empty.
+
+    The returned item will be the smallest item in the ``heap``.
+    """
+    ...
+
+def heappush(heap, item) -> Any:
+    """
+    Push the ``item`` onto the ``heap``.
+    """
+    ...
+
+def heapify(x) -> Any:
+    """
+    Convert the list ``x`` into a heap.  This is an in-place operation.
+    """
+    ...
```

### Comparing `micropython_rp2_stubs-1.19.1.post9/umachine.pyi` & `micropython_rp2_stubs-1.20.0.post1/umachine.pyi`

 * *Files 19% similar despite different names*

```diff
@@ -1,1035 +1,1178 @@
-"""
-functions related to the hardware. See: https://docs.micropython.org/en/v1.19.1/library/machine.html
-
-The ``machine`` module contains specific functions related to the hardware
-on a particular board. Most functions in this module allow to achieve direct
-and unrestricted access to and control of hardware blocks on a system
-(like CPU, timers, buses, etc.). Used incorrectly, this can lead to
-malfunction, lockups, crashes of your board, and in extreme cases, hardware
-damage.
-"""
-from typing import Callable, List, NoReturn, Optional, Tuple, Union, Any
-
-WDT_RESET: int
-PWRON_RESET: int
-
-def disable_irq() -> Any:
-    """
-    Disable interrupt requests.
-    Returns the previous IRQ state which should be considered an opaque value.
-    This return value should be passed to the `enable_irq()` function to restore
-    interrupts to their original state, before `disable_irq()` was called.
-    """
-    ...
-
-def soft_reset() -> NoReturn:
-    """
-    Performs a soft reset of the interpreter, deleting all Python objects and
-    resetting the Python heap.  It tries to retain the method by which the user
-    is connected to the MicroPython REPL (eg serial, USB, Wifi).
-    """
-    ...
-
-def enable_irq(state) -> Any:
-    """
-    Re-enable interrupt requests.
-    The *state* parameter should be the value that was returned from the most
-    recent call to the `disable_irq()` function.
-    """
-    ...
-
-def bitstream(pin, encoding, timing, data, /) -> Any:
-    """
-    Transmits *data* by bit-banging the specified *pin*. The *encoding* argument
-    specifies how the bits are encoded, and *timing* is an encoding-specific timing
-    specification.
-
-    The supported encodings are:
-
-      - ``0`` for "high low" pulse duration modulation. This will transmit 0 and
-        1 bits as timed pulses, starting with the most significant bit.
-        The *timing* must be a four-tuple of nanoseconds in the format
-        ``(high_time_0, low_time_0, high_time_1, low_time_1)``. For example,
-        ``(400, 850, 800, 450)`` is the timing specification for WS2812 RGB LEDs
-        at 800kHz.
-
-    The accuracy of the timing varies between ports. On Cortex M0 at 48MHz, it is
-    at best +/- 120ns, however on faster MCUs (ESP8266, ESP32, STM32, Pyboard), it
-    will be closer to +/-30ns.
-
-    ``Note:`` For controlling WS2812 / NeoPixel strips, see the :mod:`neopixel`
-       module for a higher-level API.
-    """
-    ...
-
-def deepsleep(time_ms: Optional[Any] = None) -> NoReturn:
-    """
-    Stops execution in an attempt to enter a low power state.
-
-    If *time_ms* is specified then this will be the maximum time in milliseconds that
-    the sleep will last for.  Otherwise the sleep can last indefinitely.
-
-    With or without a timeout, execution may resume at any time if there are events
-    that require processing.  Such events, or wake sources, should be configured before
-    sleeping, like `Pin` change or `RTC` timeout.
-
-    The precise behaviour and power-saving capabilities of lightsleep and deepsleep is
-    highly dependent on the underlying hardware, but the general properties are:
-
-    * A lightsleep has full RAM and state retention.  Upon wake execution is resumed
-      from the point where the sleep was requested, with all subsystems operational.
-
-    * A deepsleep may not retain RAM or any other state of the system (for example
-      peripherals or network interfaces).  Upon wake execution is resumed from the main
-      script, similar to a hard or power-on reset. The `reset_cause()` function will
-      return `machine.DEEPSLEEP` and this can be used to distinguish a deepsleep wake
-      from other resets.
-    """
-    ...
-
-def bootloader(value: Optional[Any] = None) -> None:
-    """
-    Reset the device and enter its bootloader.  This is typically used to put the
-    device into a state where it can be programmed with new firmware.
-
-    Some ports support passing in an optional *value* argument which can control
-    which bootloader to enter, what to pass to it, or other things.
-    """
-    ...
-
-def reset() -> NoReturn:
-    """
-    Resets the device in a manner similar to pushing the external RESET
-    button.
-    """
-    ...
-
-def freq(hz: Optional[Any] = None) -> Any:
-    """
-    Returns the CPU frequency in hertz.
-
-    On some ports this can also be used to set the CPU frequency by passing in *hz*.
-    """
-    ...
-
-def reset_cause() -> int:
-    """
-    Get the reset cause. See :ref:`constants <machine_constants>` for the possible return values.
-    """
-    ...
-
-def idle() -> Any:
-    """
-    Gates the clock to the CPU, useful to reduce power consumption at any time during
-    short or long periods. Peripherals continue working and execution resumes as soon
-    as any interrupt is triggered (on many ports this includes system timer
-    interrupt occurring at regular intervals on the order of millisecond).
-    """
-    ...
-
-def time_pulse_us(pin, pulse_level, timeout_us=1000000, /) -> int:
-    """
-    Time a pulse on the given *pin*, and return the duration of the pulse in
-    microseconds.  The *pulse_level* argument should be 0 to time a low pulse
-    or 1 to time a high pulse.
-
-    If the current input value of the pin is different to *pulse_level*,
-    the function first (*) waits until the pin input becomes equal to *pulse_level*,
-    then (**) times the duration that the pin is equal to *pulse_level*.
-    If the pin is already equal to *pulse_level* then timing starts straight away.
-
-    The function will return -2 if there was timeout waiting for condition marked
-    (*) above, and -1 if there was timeout during the main measurement, marked (**)
-    above. The timeout is the same for both cases and given by *timeout_us* (which
-    is in microseconds).
-    """
-    ...
-
-def lightsleep(time_ms: Optional[Any] = None) -> Any:
-    """
-    Stops execution in an attempt to enter a low power state.
-
-    If *time_ms* is specified then this will be the maximum time in milliseconds that
-    the sleep will last for.  Otherwise the sleep can last indefinitely.
-
-    With or without a timeout, execution may resume at any time if there are events
-    that require processing.  Such events, or wake sources, should be configured before
-    sleeping, like `Pin` change or `RTC` timeout.
-
-    The precise behaviour and power-saving capabilities of lightsleep and deepsleep is
-    highly dependent on the underlying hardware, but the general properties are:
-
-    * A lightsleep has full RAM and state retention.  Upon wake execution is resumed
-      from the point where the sleep was requested, with all subsystems operational.
-
-    * A deepsleep may not retain RAM or any other state of the system (for example
-      peripherals or network interfaces).  Upon wake execution is resumed from the main
-      script, similar to a hard or power-on reset. The `reset_cause()` function will
-      return `machine.DEEPSLEEP` and this can be used to distinguish a deepsleep wake
-      from other resets.
-    """
-    ...
-
-def unique_id() -> bytes:
-    """
-    Returns a byte string with a unique identifier of a board/SoC. It will vary
-    from a board/SoC instance to another, if underlying hardware allows. Length
-    varies by hardware (so use substring of a full value if you expect a short
-    ID). In some MicroPython ports, ID corresponds to the network MAC address.
-    """
-    ...
-
-class WDT:
-    """
-    Create a WDT object and start it. The timeout must be given in milliseconds.
-    Once it is running the timeout cannot be changed and the WDT cannot be stopped either.
-
-    Notes: On the esp32 the minimum timeout is 1 second. On the esp8266 a timeout
-    cannot be specified, it is determined by the underlying system.
-    """
-
-    def feed(self) -> None:
-        """
-        Feed the WDT to prevent it from resetting the system. The application
-        should place this call in a sensible place ensuring that the WDT is
-        only fed after verifying that everything is functioning correctly.
-        """
-        ...
-    def __init__(self, id=0, timeout=5000) -> None: ...
-
-mem8: Any
-mem32: Any
-mem16: Any
-
-class PWM:
-    """
-    Construct and return a new PWM object using the following parameters:
-
-       - *dest* is the entity on which the PWM is output, which is usually a
-         :ref:`machine.Pin <machine.Pin>` object, but a port may allow other values,
-         like integers.
-       - *freq* should be an integer which sets the frequency in Hz for the
-         PWM cycle.
-       - *duty_u16* sets the duty cycle as a ratio ``duty_u16 / 65535``.
-       - *duty_ns* sets the pulse width in nanoseconds.
-
-    Setting *freq* may affect other PWM objects if the objects share the same
-    underlying PWM generator (this is hardware specific).
-    Only one of *duty_u16* and *duty_ns* should be specified at a time.
-    """
-
-    def freq(self, value: Optional[Any] = None) -> Any:
-        """
-        Get or set the current frequency of the PWM output.
-
-        With no arguments the frequency in Hz is returned.
-
-        With a single *value* argument the frequency is set to that value in Hz.  The
-        method may raise a ``ValueError`` if the frequency is outside the valid range.
-        """
-        ...
-    def duty_u16(self, value: Optional[Any] = None) -> int:
-        """
-        Get or set the current duty cycle of the PWM output, as an unsigned 16-bit
-        value in the range 0 to 65535 inclusive.
-
-        With no arguments the duty cycle is returned.
-
-        With a single *value* argument the duty cycle is set to that value, measured
-        as the ratio ``value / 65535``.
-        """
-        ...
-    def duty_ns(self, value: Optional[Any] = None) -> int:
-        """
-        Get or set the current pulse width of the PWM output, as a value in nanoseconds.
-
-        With no arguments the pulse width in nanoseconds is returned.
-
-        With a single *value* argument the pulse width is set to that value.
-        """
-        ...
-    def deinit(self) -> None:
-        """
-        Disable the PWM output.
-        """
-        ...
-    def __init__(self, dest, *, freq=0, duty=0, duty_u16=0, duty_ns=0) -> None: ...
-
-class ADC:
-    """
-    Access the ADC associated with a source identified by *id*.  This
-    *id* may be an integer (usually specifying a channel number), a
-    :ref:`Pin <machine.Pin>` object, or other value supported by the
-    underlying machine.
-
-    If additional keyword-arguments are given then they will configure
-    various aspects of the ADC.  If not given, these settings will take
-    previous or default values.  The settings are:
-
-      - *sample_ns* is the sampling time in nanoseconds.
-
-      - *atten* specifies the input attenuation.
-    """
-
-    CORE_TEMP: int
-    def read_u16(self) -> int:
-        """
-        Take an analog reading and return an integer in the range 0-65535.
-        The return value represents the raw reading taken by the ADC, scaled
-        such that the minimum value is 0 and the maximum value is 65535.
-        """
-        ...
-    def __init__(self, id, *, sample_ns: Optional[int] = 0, atten: Optional[int] = ATTN_0DB) -> None: ...
-
-class I2C:
-    """
-    Construct and return a new I2C object using the following parameters:
-
-       - *id* identifies a particular I2C peripheral.  Allowed values for
-         depend on the particular port/board
-       - *scl* should be a pin object specifying the pin to use for SCL.
-       - *sda* should be a pin object specifying the pin to use for SDA.
-       - *freq* should be an integer which sets the maximum frequency
-         for SCL.
-
-    Note that some ports/boards will have default values of *scl* and *sda*
-    that can be changed in this constructor.  Others will have fixed values
-    of *scl* and *sda* that cannot be changed.
-    """
-
-    def readfrom_mem_into(self, addr, memaddr, buf, *, addrsize=8) -> None:
-        """
-        Read into *buf* from the peripheral specified by *addr* starting from the
-        memory address specified by *memaddr*.  The number of bytes read is the
-        length of *buf*.
-        The argument *addrsize* specifies the address size in bits (on ESP8266
-        this argument is not recognised and the address size is always 8 bits).
-
-        The method returns ``None``.
-        """
-        ...
-    def readfrom_into(self, addr, buf, stop=True, /) -> None:
-        """
-        Read into *buf* from the peripheral specified by *addr*.
-        The number of bytes read will be the length of *buf*.
-        If *stop* is true then a STOP condition is generated at the end of the transfer.
-
-        The method returns ``None``.
-        """
-        ...
-    def readfrom_mem(self, addr, memaddr, nbytes, *, addrsize=8) -> bytes:
-        """
-        Read *nbytes* from the peripheral specified by *addr* starting from the memory
-        address specified by *memaddr*.
-        The argument *addrsize* specifies the address size in bits.
-        Returns a `bytes` object with the data read.
-        """
-        ...
-    def writeto_mem(self, addr, memaddr, buf, *, addrsize=8) -> None:
-        """
-        Write *buf* to the peripheral specified by *addr* starting from the
-        memory address specified by *memaddr*.
-        The argument *addrsize* specifies the address size in bits (on ESP8266
-        this argument is not recognised and the address size is always 8 bits).
-
-        The method returns ``None``.
-        """
-        ...
-    def scan(self) -> List:
-        """
-        Scan all I2C addresses between 0x08 and 0x77 inclusive and return a list of
-        those that respond.  A device responds if it pulls the SDA line low after
-        its address (including a write bit) is sent on the bus.
-        """
-        ...
-    def writeto(self, addr, buf, stop=True, /) -> int:
-        """
-        Write the bytes from *buf* to the peripheral specified by *addr*.  If a
-        NACK is received following the write of a byte from *buf* then the
-        remaining bytes are not sent.  If *stop* is true then a STOP condition is
-        generated at the end of the transfer, even if a NACK is received.
-        The function returns the number of ACKs that were received.
-        """
-        ...
-    def writevto(self, addr, vector, stop=True, /) -> int:
-        """
-        Write the bytes contained in *vector* to the peripheral specified by *addr*.
-        *vector* should be a tuple or list of objects with the buffer protocol.
-        The *addr* is sent once and then the bytes from each object in *vector*
-        are written out sequentially.  The objects in *vector* may be zero bytes
-        in length in which case they don't contribute to the output.
-
-        If a NACK is received following the write of a byte from one of the
-        objects in *vector* then the remaining bytes, and any remaining objects,
-        are not sent.  If *stop* is true then a STOP condition is generated at
-        the end of the transfer, even if a NACK is received.  The function
-        returns the number of ACKs that were received.
-        """
-        ...
-    def start(self) -> None:
-        """
-        Generate a START condition on the bus (SDA transitions to low while SCL is high).
-        """
-        ...
-    def readfrom(self, addr, nbytes, stop=True, /) -> bytes:
-        """
-        Read *nbytes* from the peripheral specified by *addr*.
-        If *stop* is true then a STOP condition is generated at the end of the transfer.
-        Returns a `bytes` object with the data read.
-        """
-        ...
-    def readinto(self, buf, nack=True, /) -> Any:
-        """
-        Reads bytes from the bus and stores them into *buf*.  The number of bytes
-        read is the length of *buf*.  An ACK will be sent on the bus after
-        receiving all but the last byte.  After the last byte is received, if *nack*
-        is true then a NACK will be sent, otherwise an ACK will be sent (and in this
-        case the peripheral assumes more bytes are going to be read in a later call).
-        """
-        ...
-    def init(self, scl, sda, *, freq=400000) -> None:
-        """
-        Initialise the I2C bus with the given arguments:
-
-           - *scl* is a pin object for the SCL line
-           - *sda* is a pin object for the SDA line
-           - *freq* is the SCL clock rate
-        """
-        ...
-    def stop(self) -> None:
-        """
-        Generate a STOP condition on the bus (SDA transitions to high while SCL is high).
-        """
-        ...
-    def write(self, buf) -> int:
-        """
-        Write the bytes from *buf* to the bus.  Checks that an ACK is received
-        after each byte and stops transmitting the remaining bytes if a NACK is
-        received.  The function returns the number of ACKs that were received.
-        """
-        ...
-    def __init__(
-        self, id: Union[int, str] = -1, *, scl: Optional[Union[Pin, str]] = None, sda: Optional[Union[Pin, str]] = None, freq=400_000
-    ) -> None: ...
-
-class I2S:
-    """
-    Construct an I2S object of the given id:
-
-    - ``id`` identifies a particular I2S bus; it is board and port specific
-
-    Keyword-only parameters that are supported on all ports:
-
-      - ``sck`` is a pin object for the serial clock line
-      - ``ws`` is a pin object for the word select line
-      - ``sd`` is a pin object for the serial data line
-      - ``mck`` is a pin object for the master clock line;
-        master clock frequency is sampling rate * 256
-      - ``mode`` specifies receive or transmit
-      - ``bits`` specifies sample size (bits), 16 or 32
-      - ``format`` specifies channel format, STEREO or MONO
-      - ``rate`` specifies audio sampling rate (Hz);
-        this is the frequency of the ``ws`` signal
-      - ``ibuf`` specifies internal buffer length (bytes)
-
-    For all ports, DMA runs continuously in the background and allows user applications to perform other operations while
-    sample data is transfered between the internal buffer and the I2S peripheral unit.
-    Increasing the size of the internal buffer has the potential to increase the time that user applications can perform non-I2S operations
-    before underflow (e.g. ``write`` method) or overflow (e.g. ``readinto`` method).
-    """
-
-    RX: int
-    MONO: int
-    STEREO: int
-    TX: int
-    @staticmethod
-    def shift(*, buf, bits, shift) -> Any:
-        """
-        bitwise shift of all samples contained in ``buf``. ``bits`` specifies sample size in bits. ``shift`` specifies the number of bits to shift each sample.
-        Positive for left shift, negative for right shift.
-        Typically used for volume control.  Each bit shift changes sample volume by 6dB.
-        """
-        ...
-    def init(self, sck, *args, **kwargs) -> Any:
-        """
-        see Constructor for argument descriptions
-        """
-        ...
-    def irq(self, handler) -> Any:
-        """
-        Set a callback. ``handler`` is called when ``buf`` is emptied (``write`` method) or becomes full (``readinto`` method).
-        Setting a callback changes the ``write`` and ``readinto`` methods to non-blocking operation.
-        ``handler`` is called in the context of the MicroPython scheduler.
-        """
-        ...
-    def readinto(self, buf) -> int:
-        """
-        Read audio samples into the buffer specified by ``buf``.  ``buf`` must support the buffer protocol, such as bytearray or array.
-        "buf" byte ordering is little-endian.  For Stereo format, left channel sample precedes right channel sample. For Mono format,
-        the left channel sample data is used.
-        Returns number of bytes read
-        """
-        ...
-    def deinit(self) -> Any:
-        """
-        Deinitialize the I2S bus
-        """
-        ...
-    def write(self, buf) -> int:
-        """
-        Write audio samples contained in ``buf``. ``buf`` must support the buffer protocol, such as bytearray or array.
-        "buf" byte ordering is little-endian.  For Stereo format, left channel sample precedes right channel sample. For Mono format,
-        the sample data is written to both the right and left channels.
-        Returns number of bytes written
-        """
-        ...
-    def __init__(self, id, *, sck, ws, sd, mck=None, mode, bits, format, rate, ibuf) -> None: ...
-
-class Pin:
-    """
-    Access the pin peripheral (GPIO pin) associated with the given ``id``.  If
-    additional arguments are given in the constructor then they are used to initialise
-    the pin.  Any settings that are not specified will remain in their previous state.
-
-    The arguments are:
-
-      - ``id`` is mandatory and can be an arbitrary object.  Among possible value
-        types are: int (an internal Pin identifier), str (a Pin name), and tuple
-        (pair of [port, pin]).
-
-      - ``mode`` specifies the pin mode, which can be one of:
-
-        - ``Pin.IN`` - Pin is configured for input.  If viewed as an output the pin
-          is in high-impedance state.
-
-        - ``Pin.OUT`` - Pin is configured for (normal) output.
-
-        - ``Pin.OPEN_DRAIN`` - Pin is configured for open-drain output. Open-drain
-          output works in the following way: if the output value is set to 0 the pin
-          is active at a low level; if the output value is 1 the pin is in a high-impedance
-          state.  Not all ports implement this mode, or some might only on certain pins.
-
-        - ``Pin.ALT`` - Pin is configured to perform an alternative function, which is
-          port specific.  For a pin configured in such a way any other Pin methods
-          (except :meth:`Pin.init`) are not applicable (calling them will lead to undefined,
-          or a hardware-specific, result).  Not all ports implement this mode.
-
-        - ``Pin.ALT_OPEN_DRAIN`` - The Same as ``Pin.ALT``, but the pin is configured as
-          open-drain.  Not all ports implement this mode.
-
-        - ``Pin.ANALOG`` - Pin is configured for analog input, see the :class:`ADC` class.
-
-      - ``pull`` specifies if the pin has a (weak) pull resistor attached, and can be
-        one of:
-
-        - ``None`` - No pull up or down resistor.
-        - ``Pin.PULL_UP`` - Pull up resistor enabled.
-        - ``Pin.PULL_DOWN`` - Pull down resistor enabled.
-
-      - ``value`` is valid only for Pin.OUT and Pin.OPEN_DRAIN modes and specifies initial
-        output pin value if given, otherwise the state of the pin peripheral remains
-        unchanged.
-
-      - ``drive`` specifies the output power of the pin and can be one of: ``Pin.DRIVE_0``,
-        ``Pin.DRIVE_1``, etc., increasing in drive strength.  The actual current driving
-        capabilities are port dependent.  Not all ports implement this argument.
-
-      - ``alt`` specifies an alternate function for the pin and the values it can take are
-        port dependent.  This argument is valid only for ``Pin.ALT`` and ``Pin.ALT_OPEN_DRAIN``
-        modes.  It may be used when a pin supports more than one alternate function.  If only
-        one pin alternate function is supported the this argument is not required.  Not all
-        ports implement this argument.
-
-    As specified above, the Pin class allows to set an alternate function for a particular
-    pin, but it does not specify any further operations on such a pin.  Pins configured in
-    alternate-function mode are usually not used as GPIO but are instead driven by other
-    hardware peripherals.  The only operation supported on such a pin is re-initialising,
-    by calling the constructor or :meth:`Pin.init` method.  If a pin that is configured in
-    alternate-function mode is re-initialised with ``Pin.IN``, ``Pin.OUT``, or
-    ``Pin.OPEN_DRAIN``, the alternate function will be removed from the pin.
-    """
-
-    PULL_DOWN: int
-    IRQ_RISING: int
-    OPEN_DRAIN: int
-    OUT: int
-    IRQ_FALLING: int
-    PULL_UP: int
-    ALT: int
-    IN: int
-    def toggle(self, *args, **kwargs) -> Any: ...
-    def low(self) -> None:
-        """
-        Set pin to "0" output level.
-
-        Availability: nrf, rp2, stm32 ports.
-        """
-        ...
-    def off(self) -> None:
-        """
-        Set pin to "0" output level.
-        """
-        ...
-    def on(self) -> None:
-        """
-        Set pin to "1" output level.
-        """
-        ...
-    def irq(self, handler=None, trigger=IRQ_FALLING, *, priority=1, wake=None, hard=False) -> Callable[..., Any]:
-        """
-           Configure an interrupt handler to be called when the trigger source of the
-           pin is active.  If the pin mode is ``Pin.IN`` then the trigger source is
-           the external value on the pin.  If the pin mode is ``Pin.OUT`` then the
-           trigger source is the output buffer of the pin.  Otherwise, if the pin mode
-           is ``Pin.OPEN_DRAIN`` then the trigger source is the output buffer for
-           state '0' and the external pin value for state '1'.
-
-           The arguments are:
-
-             - ``handler`` is an optional function to be called when the interrupt
-               triggers. The handler must take exactly one argument which is the
-               ``Pin`` instance.
-
-             - ``trigger`` configures the event which can generate an interrupt.
-               Possible values are:
-
-               - ``Pin.IRQ_FALLING`` interrupt on falling edge.
-               - ``Pin.IRQ_RISING`` interrupt on rising edge.
-               - ``Pin.IRQ_LOW_LEVEL`` interrupt on low level.
-               - ``Pin.IRQ_HIGH_LEVEL`` interrupt on high level.
-
-               These values can be OR'ed together to trigger on multiple events.
-
-             - ``priority`` sets the priority level of the interrupt.  The values it
-               can take are port-specific, but higher values always represent higher
-               priorities.
-
-             - ``wake`` selects the power mode in which this interrupt can wake up the
-               system.  It can be ``machine.IDLE``, ``machine.SLEEP`` or ``machine.DEEPSLEEP``.
-               These values can also be OR'ed together to make a pin generate interrupts in
-               more than one power mode.
-
-             - ``hard`` if true a hardware interrupt is used. This reduces the delay
-               between the pin change and the handler being called. Hard interrupt
-               handlers may not allocate memory; see :ref:`isr_rules`.
-               Not all ports support this argument.
-
-           This method returns a callback object.
-
-        The following methods are not part of the core Pin API and only implemented on certain ports.
-        """
-        ...
-    def value(self, x: Optional[Any] = None) -> int:
-        """
-        This method allows to set and get the value of the pin, depending on whether
-        the argument ``x`` is supplied or not.
-
-        If the argument is omitted then this method gets the digital logic level of
-        the pin, returning 0 or 1 corresponding to low and high voltage signals
-        respectively.  The behaviour of this method depends on the mode of the pin:
-
-          - ``Pin.IN`` - The method returns the actual input value currently present
-            on the pin.
-          - ``Pin.OUT`` - The behaviour and return value of the method is undefined.
-          - ``Pin.OPEN_DRAIN`` - If the pin is in state '0' then the behaviour and
-            return value of the method is undefined.  Otherwise, if the pin is in
-            state '1', the method returns the actual input value currently present
-            on the pin.
-
-        If the argument is supplied then this method sets the digital logic level of
-        the pin.  The argument ``x`` can be anything that converts to a boolean.
-        If it converts to ``True``, the pin is set to state '1', otherwise it is set
-        to state '0'.  The behaviour of this method depends on the mode of the pin:
-
-          - ``Pin.IN`` - The value is stored in the output buffer for the pin.  The
-            pin state does not change, it remains in the high-impedance state.  The
-            stored value will become active on the pin as soon as it is changed to
-            ``Pin.OUT`` or ``Pin.OPEN_DRAIN`` mode.
-          - ``Pin.OUT`` - The output buffer is set to the given value immediately.
-          - ``Pin.OPEN_DRAIN`` - If the value is '0' the pin is set to a low voltage
-            state.  Otherwise the pin is set to high-impedance state.
-
-        When setting the value this method returns ``None``.
-        """
-        ...
-    def high(self) -> None:
-        """
-        Set pin to "1" output level.
-
-        Availability: nrf, rp2, stm32 ports.
-        """
-        ...
-    def init(self, mode=-1, pull=-1, *, value=None, drive=0, alt=-1) -> None:
-        """
-        Re-initialise the pin using the given parameters.  Only those arguments that
-        are specified will be set.  The rest of the pin peripheral state will remain
-        unchanged.  See the constructor documentation for details of the arguments.
-
-        Returns ``None``.
-        """
-        ...
-    def __init__(self, id, mode=-1, pull=-1, *, value=None, drive=0, alt=-1) -> None: ...
-
-class SoftSPI:
-    """
-    Construct a new software SPI object.  Additional parameters must be
-    given, usually at least *sck*, *mosi* and *miso*, and these are used
-    to initialise the bus.  See `SPI.init` for a description of the parameters.
-    """
-
-    LSB: int
-    MSB: int
-    def deinit(self, *args, **kwargs) -> Any: ...
-    def init(self, *args, **kwargs) -> Any: ...
-    def write_readinto(self, *args, **kwargs) -> Any: ...
-    def read(self, *args, **kwargs) -> Any: ...
-    def write(self, *args, **kwargs) -> Any: ...
-    def readinto(self, *args, **kwargs) -> Any: ...
-    def __init__(self, baudrate=500000, *, polarity=0, phase=0, bits=8, firstbit=MSB, sck=None, mosi=None, miso=None) -> None: ...
-
-class Timer:
-    """
-    Construct a new timer object of the given ``id``. ``id`` of -1 constructs a
-    virtual timer (if supported by a board).
-    ``id`` shall not be passed as a keyword argument.
-
-    See ``init`` for parameters of initialisation.
-    """
-
-    PERIODIC: int
-    ONE_SHOT: int
-    def init(self, *, mode=PERIODIC, period=-1, callback=None) -> None:
-        """
-        Initialise the timer. Example::
-
-            def mycallback(t):
-                pass
-
-            # periodic with 100ms period
-            tim.init(period=100, callback=mycallback)
-
-            # one shot firing after 1000ms
-            tim.init(mode=Timer.ONE_SHOT, period=1000, callback=mycallback)
-
-        Keyword arguments:
-
-          - ``mode`` can be one of:
-
-            - ``Timer.ONE_SHOT`` - The timer runs once until the configured
-              period of the channel expires.
-            - ``Timer.PERIODIC`` - The timer runs periodically at the configured
-              frequency of the channel.
-
-          - ``period`` - The timer period, in milliseconds.
-
-          - ``callback`` - The callable to call upon expiration of the timer period.
-            The callback must take one argument, which is passed the Timer object.
-            The ``callback`` argument shall be specified. Otherwise an exception
-            will occurr upon timer expiration:
-            ``TypeError: 'NoneType' object isn't callable``
-        """
-        ...
-    def deinit(self) -> None:
-        """
-        Deinitialises the timer. Stops the timer, and disables the timer peripheral.
-        """
-        ...
-    def __init__(self, id=-1, *args, **kwargs) -> None: ...
-
-class UART:
-    """
-    Construct a UART object of the given id.
-    """
-
-    INV_TX: int
-    CTS: int
-    INV_RX: int
-    RTS: int
-    def deinit(self) -> None:
-        """
-        Turn off the UART bus.
-        """
-        ...
-    def init(self, baudrate=9600, bits=8, parity=None, stop=1, *args, **kwargs) -> None:
-        """
-        Initialise the UART bus with the given parameters:
-
-          - *baudrate* is the clock rate.
-          - *bits* is the number of bits per character, 7, 8 or 9.
-          - *parity* is the parity, ``None``, 0 (even) or 1 (odd).
-          - *stop* is the number of stop bits, 1 or 2.
-
-        Additional keyword-only parameters that may be supported by a port are:
-
-          - *tx* specifies the TX pin to use.
-          - *rx* specifies the RX pin to use.
-          - *rts* specifies the RTS (output) pin to use for hardware receive flow control.
-          - *cts* specifies the CTS (input) pin to use for hardware transmit flow control.
-          - *txbuf* specifies the length in characters of the TX buffer.
-          - *rxbuf* specifies the length in characters of the RX buffer.
-          - *timeout* specifies the time to wait for the first character (in ms).
-          - *timeout_char* specifies the time to wait between characters (in ms).
-          - *invert* specifies which lines to invert.
-
-              - ``0`` will not invert lines (idle state of both lines is logic high).
-              - ``UART.INV_TX`` will invert TX line (idle state of TX line now logic low).
-              - ``UART.INV_RX`` will invert RX line (idle state of RX line now logic low).
-              - ``UART.INV_TX | UART.INV_RX`` will invert both lines (idle state at logic low).
-
-          - *flow* specifies which hardware flow control signals to use. The value
-            is a bitmask.
-
-              - ``0`` will ignore hardware flow control signals.
-              - ``UART.RTS`` will enable receive flow control by using the RTS output pin to
-                signal if the receive FIFO has sufficient space to accept more data.
-              - ``UART.CTS`` will enable transmit flow control by pausing transmission when the
-                CTS input pin signals that the receiver is running low on buffer space.
-              - ``UART.RTS | UART.CTS`` will enable both, for full hardware flow control.
-
-        On the WiPy only the following keyword-only parameter is supported:
-
-          - *pins* is a 4 or 2 item list indicating the TX, RX, RTS and CTS pins (in that order).
-            Any of the pins can be None if one wants the UART to operate with limited functionality.
-            If the RTS pin is given the the RX pin must be given as well. The same applies to CTS.
-            When no pins are given, then the default set of TX and RX pins is taken, and hardware
-            flow control will be disabled. If *pins* is ``None``, no pin assignment will be made.
-        """
-        ...
-    def sendbreak(self) -> None:
-        """
-        Send a break condition on the bus. This drives the bus low for a duration
-        longer than required for a normal transmission of a character.
-        """
-        ...
-    def read(self, nbytes: Optional[Any] = None) -> bytes:
-        """
-        Read characters.  If ``nbytes`` is specified then read at most that many bytes,
-        otherwise read as much data as possible. It may return sooner if a timeout
-        is reached. The timeout is configurable in the constructor.
-
-        Return value: a bytes object containing the bytes read in.  Returns ``None``
-        on timeout.
-        """
-        ...
-    def any(self) -> int:
-        """
-        Returns an integer counting the number of characters that can be read without
-        blocking.  It will return 0 if there are no characters available and a positive
-        number if there are characters.  The method may return 1 even if there is more
-        than one character available for reading.
-
-        For more sophisticated querying of available characters use select.poll::
-
-         poll = select.poll()
-         poll.register(uart, select.POLLIN)
-         poll.poll(timeout)
-        """
-        ...
-    def write(self, buf) -> int:
-        """
-        Write the buffer of bytes to the bus.
-
-        Return value: number of bytes written or ``None`` on timeout.
-        """
-        ...
-    def readinto(self, buf, nbytes: Optional[Any] = None) -> int:
-        """
-        Read bytes into the ``buf``.  If ``nbytes`` is specified then read at most
-        that many bytes.  Otherwise, read at most ``len(buf)`` bytes. It may return sooner if a timeout
-        is reached. The timeout is configurable in the constructor.
-
-        Return value: number of bytes read and stored into ``buf`` or ``None`` on
-        timeout.
-        """
-        ...
-    def readline(self) -> None:
-        """
-        Read a line, ending in a newline character. It may return sooner if a timeout
-        is reached. The timeout is configurable in the constructor.
-
-        Return value: the line read or ``None`` on timeout.
-        """
-        ...
-    def __init__(self, id, *args, **kwargs) -> None: ...
-
-class SoftI2C:
-    """
-    Construct a new software I2C object.  The parameters are:
-
-       - *scl* should be a pin object specifying the pin to use for SCL.
-       - *sda* should be a pin object specifying the pin to use for SDA.
-       - *freq* should be an integer which sets the maximum frequency
-         for SCL.
-       - *timeout* is the maximum time in microseconds to wait for clock
-         stretching (SCL held low by another device on the bus), after
-         which an ``OSError(ETIMEDOUT)`` exception is raised.
-    """
-
-    def readfrom_mem_into(self, *args, **kwargs) -> Any: ...
-    def readfrom_into(self, *args, **kwargs) -> Any: ...
-    def readfrom_mem(self, *args, **kwargs) -> Any: ...
-    def writeto_mem(self, *args, **kwargs) -> Any: ...
-    def scan(self, *args, **kwargs) -> Any: ...
-    def writeto(self, *args, **kwargs) -> Any: ...
-    def writevto(self, *args, **kwargs) -> Any: ...
-    def start(self, *args, **kwargs) -> Any: ...
-    def readfrom(self, *args, **kwargs) -> Any: ...
-    def readinto(self, *args, **kwargs) -> Any: ...
-    def init(self, *args, **kwargs) -> Any: ...
-    def stop(self, *args, **kwargs) -> Any: ...
-    def write(self, *args, **kwargs) -> Any: ...
-    def __init__(self, scl, sda, *, freq=400000, timeout=50000) -> None: ...
-
-class RTC:
-    """
-    Create an RTC object. See init for parameters of initialization.
-    """
-
-    def datetime(self, datetimetuple: Optional[Any] = None) -> Tuple:
-        """
-        Get or set the date and time of the RTC.
-
-        With no arguments, this method returns an 8-tuple with the current
-        date and time.  With 1 argument (being an 8-tuple) it sets the date
-        and time.
-
-        The 8-tuple has the following format:
-
-            (year, month, day, weekday, hours, minutes, seconds, subseconds)
-
-        The meaning of the ``subseconds`` field is hardware dependent.
-        """
-        ...
-    def __init__(self, id=0, *args, **kwargs) -> None: ...
-
-class SPI:
-    """
-    Construct an SPI object on the given bus, *id*. Values of *id* depend
-    on a particular port and its hardware. Values 0, 1, etc. are commonly used
-    to select hardware SPI block #0, #1, etc.
-
-    With no additional parameters, the SPI object is created but not
-    initialised (it has the settings from the last initialisation of
-    the bus, if any).  If extra arguments are given, the bus is initialised.
-    See ``init`` for parameters of initialisation.
-    """
-
-    LSB: int
-    MSB: int
-    def deinit(self) -> None:
-        """
-        Turn off the SPI bus.
-        """
-        ...
-    def init(
-        self, baudrate=1000000, *, polarity=0, phase=0, bits=8, firstbit=MSB, sck=None, mosi=None, miso=None, pins: Optional[Tuple]
-    ) -> None:
-        """
-        Initialise the SPI bus with the given parameters:
-
-          - ``baudrate`` is the SCK clock rate.
-          - ``polarity`` can be 0 or 1, and is the level the idle clock line sits at.
-          - ``phase`` can be 0 or 1 to sample data on the first or second clock edge
-            respectively.
-          - ``bits`` is the width in bits of each transfer. Only 8 is guaranteed to be supported by all hardware.
-          - ``firstbit`` can be ``SPI.MSB`` or ``SPI.LSB``.
-          - ``sck``, ``mosi``, ``miso`` are pins (machine.Pin) objects to use for bus signals. For most
-            hardware SPI blocks (as selected by ``id`` parameter to the constructor), pins are fixed
-            and cannot be changed. In some cases, hardware blocks allow 2-3 alternative pin sets for
-            a hardware SPI block. Arbitrary pin assignments are possible only for a bitbanging SPI driver
-            (``id`` = -1).
-          - ``pins`` - WiPy port doesn't ``sck``, ``mosi``, ``miso`` arguments, and instead allows to
-            specify them as a tuple of ``pins`` parameter.
-
-        In the case of hardware SPI the actual clock frequency may be lower than the
-        requested baudrate. This is dependant on the platform hardware. The actual
-        rate may be determined by printing the SPI object.
-        """
-        ...
-    def write_readinto(self, write_buf, read_buf) -> int:
-        """
-        Write the bytes from ``write_buf`` while reading into ``read_buf``.  The
-        buffers can be the same or different, but both buffers must have the
-        same length.
-        Returns ``None``.
-
-        Note: on WiPy this function returns the number of bytes written.
-        """
-        ...
-    def read(self, nbytes, write=0x00) -> bytes:
-        """
-        Read a number of bytes specified by ``nbytes`` while continuously writing
-        the single byte given by ``write``.
-        Returns a ``bytes`` object with the data that was read.
-        """
-        ...
-    def write(self, buf) -> int:
-        """
-        Write the bytes contained in ``buf``.
-        Returns ``None``.
-
-        Note: on WiPy this function returns the number of bytes written.
-        """
-        ...
-    def readinto(self, buf, write=0x00) -> int:
-        """
-        Read into the buffer specified by ``buf`` while continuously writing the
-        single byte given by ``write``.
-        Returns ``None``.
-
-        Note: on WiPy this function returns the number of bytes read.
-        """
-        ...
-    def __init__(self, id, *args, **kwargs) -> None: ...
-
-class Signal:
-    """
-            Signal(pin_arguments..., *, invert=False)
-
-    Create a Signal object. There're two ways to create it:
-
-    * By wrapping existing Pin object - universal method which works for
-      any board.
-    * By passing required Pin parameters directly to Signal constructor,
-      skipping the need to create intermediate Pin object. Available on
-      many, but not all boards.
-
-    The arguments are:
-
-      - ``pin_obj`` is existing Pin object.
-
-      - ``pin_arguments`` are the same arguments as can be passed to Pin constructor.
-
-      - ``invert`` - if True, the signal will be inverted (active low).
-    """
-
-    def off(self) -> None:
-        """
-        Deactivate signal.
-        """
-        ...
-    def on(self) -> None:
-        """
-        Activate signal.
-        """
-        ...
-    def value(self, x: Optional[Any] = None) -> int:
-        """
-        This method allows to set and get the value of the signal, depending on whether
-        the argument ``x`` is supplied or not.
-
-        If the argument is omitted then this method gets the signal level, 1 meaning
-        signal is asserted (active) and 0 - signal inactive.
-
-        If the argument is supplied then this method sets the signal level. The
-        argument ``x`` can be anything that converts to a boolean. If it converts
-        to ``True``, the signal is active, otherwise it is inactive.
-
-        Correspondence between signal being active and actual logic level on the
-        underlying pin depends on whether signal is inverted (active-low) or not.
-        For non-inverted signal, active status corresponds to logical 1, inactive -
-        to logical 0. For inverted/active-low signal, active status corresponds
-        to logical 0, while inactive - to logical 1.
-        """
-        ...
-    def __init__(self, pin_obj, *args, invert=False) -> None: ...
+"""
+functions related to the hardware. See: https://docs.micropython.org/en/v1.20.0/library/machine.html
+
+The ``machine`` module contains specific functions related to the hardware
+on a particular board. Most functions in this module allow to achieve direct
+and unrestricted access to and control of hardware blocks on a system
+(like CPU, timers, buses, etc.). Used incorrectly, this can lead to
+malfunction, lockups, crashes of your board, and in extreme cases, hardware
+damage.
+"""
+from typing import Callable, List, NoReturn, Optional, Tuple, Union, Any
+
+WDT_RESET: int
+PWRON_RESET: int
+
+def dht_readinto(*args, **kwargs) -> Any: ...
+def enable_irq(state) -> Any:
+    """
+    Re-enable interrupt requests.
+    The *state* parameter should be the value that was returned from the most
+    recent call to the `disable_irq()` function.
+    """
+    ...
+
+def disable_irq() -> Any:
+    """
+    Disable interrupt requests.
+    Returns the previous IRQ state which should be considered an opaque value.
+    This return value should be passed to the `enable_irq()` function to restore
+    interrupts to their original state, before `disable_irq()` was called.
+    """
+    ...
+
+def bitstream(pin, encoding, timing, data, /) -> Any:
+    """
+    Transmits *data* by bit-banging the specified *pin*. The *encoding* argument
+    specifies how the bits are encoded, and *timing* is an encoding-specific timing
+    specification.
+
+    The supported encodings are:
+
+      - ``0`` for "high low" pulse duration modulation. This will transmit 0 and
+        1 bits as timed pulses, starting with the most significant bit.
+        The *timing* must be a four-tuple of nanoseconds in the format
+        ``(high_time_0, low_time_0, high_time_1, low_time_1)``. For example,
+        ``(400, 850, 800, 450)`` is the timing specification for WS2812 RGB LEDs
+        at 800kHz.
+
+    The accuracy of the timing varies between ports. On Cortex M0 at 48MHz, it is
+    at best +/- 120ns, however on faster MCUs (ESP8266, ESP32, STM32, Pyboard), it
+    will be closer to +/-30ns.
+
+    ``Note:`` For controlling WS2812 / NeoPixel strips, see the :mod:`neopixel`
+       module for a higher-level API.
+    """
+    ...
+
+def deepsleep(time_ms: Optional[Any] = None) -> NoReturn:
+    """
+    Stops execution in an attempt to enter a low power state.
+
+    If *time_ms* is specified then this will be the maximum time in milliseconds that
+    the sleep will last for.  Otherwise the sleep can last indefinitely.
+
+    With or without a timeout, execution may resume at any time if there are events
+    that require processing.  Such events, or wake sources, should be configured before
+    sleeping, like `Pin` change or `RTC` timeout.
+
+    The precise behaviour and power-saving capabilities of lightsleep and deepsleep is
+    highly dependent on the underlying hardware, but the general properties are:
+
+    * A lightsleep has full RAM and state retention.  Upon wake execution is resumed
+      from the point where the sleep was requested, with all subsystems operational.
+
+    * A deepsleep may not retain RAM or any other state of the system (for example
+      peripherals or network interfaces).  Upon wake execution is resumed from the main
+      script, similar to a hard or power-on reset. The `reset_cause()` function will
+      return `machine.DEEPSLEEP` and this can be used to distinguish a deepsleep wake
+      from other resets.
+    """
+    ...
+
+def bootloader(value: Optional[Any] = None) -> None:
+    """
+    Reset the device and enter its bootloader.  This is typically used to put the
+    device into a state where it can be programmed with new firmware.
+
+    Some ports support passing in an optional *value* argument which can control
+    which bootloader to enter, what to pass to it, or other things.
+    """
+    ...
+
+def soft_reset() -> NoReturn:
+    """
+    Performs a soft reset of the interpreter, deleting all Python objects and
+    resetting the Python heap.  It tries to retain the method by which the user
+    is connected to the MicroPython REPL (eg serial, USB, Wifi).
+    """
+    ...
+
+def reset() -> NoReturn:
+    """
+    Resets the device in a manner similar to pushing the external RESET
+    button.
+    """
+    ...
+
+def freq(hz: Optional[Any] = None) -> Any:
+    """
+    Returns the CPU frequency in hertz.
+
+    On some ports this can also be used to set the CPU frequency by passing in *hz*.
+    """
+    ...
+
+def reset_cause() -> int:
+    """
+    Get the reset cause. See :ref:`constants <machine_constants>` for the possible return values.
+    """
+    ...
+
+def idle() -> Any:
+    """
+    Gates the clock to the CPU, useful to reduce power consumption at any time during
+    short or long periods. Peripherals continue working and execution resumes as soon
+    as any interrupt is triggered (on many ports this includes system timer
+    interrupt occurring at regular intervals on the order of millisecond).
+    """
+    ...
+
+def time_pulse_us(pin, pulse_level, timeout_us=1000000, /) -> int:
+    """
+    Time a pulse on the given *pin*, and return the duration of the pulse in
+    microseconds.  The *pulse_level* argument should be 0 to time a low pulse
+    or 1 to time a high pulse.
+
+    If the current input value of the pin is different to *pulse_level*,
+    the function first (*) waits until the pin input becomes equal to *pulse_level*,
+    then (**) times the duration that the pin is equal to *pulse_level*.
+    If the pin is already equal to *pulse_level* then timing starts straight away.
+
+    The function will return -2 if there was timeout waiting for condition marked
+    (*) above, and -1 if there was timeout during the main measurement, marked (**)
+    above. The timeout is the same for both cases and given by *timeout_us* (which
+    is in microseconds).
+    """
+    ...
+
+def lightsleep(time_ms: Optional[Any] = None) -> Any:
+    """
+    Stops execution in an attempt to enter a low power state.
+
+    If *time_ms* is specified then this will be the maximum time in milliseconds that
+    the sleep will last for.  Otherwise the sleep can last indefinitely.
+
+    With or without a timeout, execution may resume at any time if there are events
+    that require processing.  Such events, or wake sources, should be configured before
+    sleeping, like `Pin` change or `RTC` timeout.
+
+    The precise behaviour and power-saving capabilities of lightsleep and deepsleep is
+    highly dependent on the underlying hardware, but the general properties are:
+
+    * A lightsleep has full RAM and state retention.  Upon wake execution is resumed
+      from the point where the sleep was requested, with all subsystems operational.
+
+    * A deepsleep may not retain RAM or any other state of the system (for example
+      peripherals or network interfaces).  Upon wake execution is resumed from the main
+      script, similar to a hard or power-on reset. The `reset_cause()` function will
+      return `machine.DEEPSLEEP` and this can be used to distinguish a deepsleep wake
+      from other resets.
+    """
+    ...
+
+def unique_id() -> bytes:
+    """
+    Returns a byte string with a unique identifier of a board/SoC. It will vary
+    from a board/SoC instance to another, if underlying hardware allows. Length
+    varies by hardware (so use substring of a full value if you expect a short
+    ID). In some MicroPython ports, ID corresponds to the network MAC address.
+    """
+    ...
+
+class WDT:
+    """
+    Create a WDT object and start it. The timeout must be given in milliseconds.
+    Once it is running the timeout cannot be changed and the WDT cannot be stopped either.
+
+    Notes: On the esp32 the minimum timeout is 1 second. On the esp8266 a timeout
+    cannot be specified, it is determined by the underlying system. On rp2040 devices,
+    the maximum timeout is 8388 ms.
+    """
+
+    def feed(self) -> None:
+        """
+        Feed the WDT to prevent it from resetting the system. The application
+        should place this call in a sensible place ensuring that the WDT is
+        only fed after verifying that everything is functioning correctly.
+        """
+        ...
+    def __init__(self, id=0, timeout=5000) -> None: ...
+
+mem8: Any
+mem32: Any
+mem16: Any
+
+class PWM:
+    """
+    Construct and return a new PWM object using the following parameters:
+
+       - *dest* is the entity on which the PWM is output, which is usually a
+         :ref:`machine.Pin <machine.Pin>` object, but a port may allow other values,
+         like integers.
+       - *freq* should be an integer which sets the frequency in Hz for the
+         PWM cycle.
+       - *duty_u16* sets the duty cycle as a ratio ``duty_u16 / 65535``.
+       - *duty_ns* sets the pulse width in nanoseconds.
+
+    Setting *freq* may affect other PWM objects if the objects share the same
+    underlying PWM generator (this is hardware specific).
+    Only one of *duty_u16* and *duty_ns* should be specified at a time.
+    """
+
+    def freq(self, value: Optional[Any] = None) -> Any:
+        """
+        Get or set the current frequency of the PWM output.
+
+        With no arguments the frequency in Hz is returned.
+
+        With a single *value* argument the frequency is set to that value in Hz.  The
+        method may raise a ``ValueError`` if the frequency is outside the valid range.
+        """
+        ...
+    def duty_u16(self, value: Optional[Any] = None) -> int:
+        """
+        Get or set the current duty cycle of the PWM output, as an unsigned 16-bit
+        value in the range 0 to 65535 inclusive.
+
+        With no arguments the duty cycle is returned.
+
+        With a single *value* argument the duty cycle is set to that value, measured
+        as the ratio ``value / 65535``.
+        """
+        ...
+    def duty_ns(self, value: Optional[Any] = None) -> int:
+        """
+        Get or set the current pulse width of the PWM output, as a value in nanoseconds.
+
+        With no arguments the pulse width in nanoseconds is returned.
+
+        With a single *value* argument the pulse width is set to that value.
+        """
+        ...
+    def deinit(self) -> None:
+        """
+        Disable the PWM output.
+        """
+        ...
+    def __init__(self, dest, *, freq=0, duty=0, duty_u16=0, duty_ns=0) -> None: ...
+
+class ADC:
+    """
+    Access the ADC associated with a source identified by *id*.  This
+    *id* may be an integer (usually specifying a channel number), a
+    :ref:`Pin <machine.Pin>` object, or other value supported by the
+    underlying machine.
+
+    If additional keyword-arguments are given then they will configure
+    various aspects of the ADC.  If not given, these settings will take
+    previous or default values.  The settings are:
+
+      - *sample_ns* is the sampling time in nanoseconds.
+
+      - *atten* specifies the input attenuation.
+    """
+
+    CORE_TEMP: int
+    def read_u16(self) -> int:
+        """
+        Take an analog reading and return an integer in the range 0-65535.
+        The return value represents the raw reading taken by the ADC, scaled
+        such that the minimum value is 0 and the maximum value is 65535.
+        """
+        ...
+    def __init__(self, id, *, sample_ns: Optional[int] = 0, atten: Optional[int] = ATTN_0DB) -> None: ...
+
+class I2C:
+    """
+    Construct and return a new I2C object using the following parameters:
+
+       - *id* identifies a particular I2C peripheral.  Allowed values for
+         depend on the particular port/board
+       - *scl* should be a pin object specifying the pin to use for SCL.
+       - *sda* should be a pin object specifying the pin to use for SDA.
+       - *freq* should be an integer which sets the maximum frequency
+         for SCL.
+       - *timeout* is the maximum time in microseconds to allow for I2C
+         transactions.  This parameter is not allowed on some ports.
+
+    Note that some ports/boards will have default values of *scl* and *sda*
+    that can be changed in this constructor.  Others will have fixed values
+    of *scl* and *sda* that cannot be changed.
+    """
+
+    def readfrom_mem_into(self, addr, memaddr, buf, *, addrsize=8) -> None:
+        """
+        Read into *buf* from the peripheral specified by *addr* starting from the
+        memory address specified by *memaddr*.  The number of bytes read is the
+        length of *buf*.
+        The argument *addrsize* specifies the address size in bits (on ESP8266
+        this argument is not recognised and the address size is always 8 bits).
+
+        The method returns ``None``.
+        """
+        ...
+    def readfrom_into(self, addr, buf, stop=True, /) -> None:
+        """
+        Read into *buf* from the peripheral specified by *addr*.
+        The number of bytes read will be the length of *buf*.
+        If *stop* is true then a STOP condition is generated at the end of the transfer.
+
+        The method returns ``None``.
+        """
+        ...
+    def readfrom_mem(self, addr, memaddr, nbytes, *, addrsize=8) -> bytes:
+        """
+        Read *nbytes* from the peripheral specified by *addr* starting from the memory
+        address specified by *memaddr*.
+        The argument *addrsize* specifies the address size in bits.
+        Returns a `bytes` object with the data read.
+        """
+        ...
+    def writeto_mem(self, addr, memaddr, buf, *, addrsize=8) -> None:
+        """
+        Write *buf* to the peripheral specified by *addr* starting from the
+        memory address specified by *memaddr*.
+        The argument *addrsize* specifies the address size in bits (on ESP8266
+        this argument is not recognised and the address size is always 8 bits).
+
+        The method returns ``None``.
+        """
+        ...
+    def scan(self) -> List:
+        """
+        Scan all I2C addresses between 0x08 and 0x77 inclusive and return a list of
+        those that respond.  A device responds if it pulls the SDA line low after
+        its address (including a write bit) is sent on the bus.
+        """
+        ...
+    def writeto(self, addr, buf, stop=True, /) -> int:
+        """
+        Write the bytes from *buf* to the peripheral specified by *addr*.  If a
+        NACK is received following the write of a byte from *buf* then the
+        remaining bytes are not sent.  If *stop* is true then a STOP condition is
+        generated at the end of the transfer, even if a NACK is received.
+        The function returns the number of ACKs that were received.
+        """
+        ...
+    def writevto(self, addr, vector, stop=True, /) -> int:
+        """
+        Write the bytes contained in *vector* to the peripheral specified by *addr*.
+        *vector* should be a tuple or list of objects with the buffer protocol.
+        The *addr* is sent once and then the bytes from each object in *vector*
+        are written out sequentially.  The objects in *vector* may be zero bytes
+        in length in which case they don't contribute to the output.
+
+        If a NACK is received following the write of a byte from one of the
+        objects in *vector* then the remaining bytes, and any remaining objects,
+        are not sent.  If *stop* is true then a STOP condition is generated at
+        the end of the transfer, even if a NACK is received.  The function
+        returns the number of ACKs that were received.
+        """
+        ...
+    def start(self) -> None:
+        """
+        Generate a START condition on the bus (SDA transitions to low while SCL is high).
+        """
+        ...
+    def readfrom(self, addr, nbytes, stop=True, /) -> bytes:
+        """
+        Read *nbytes* from the peripheral specified by *addr*.
+        If *stop* is true then a STOP condition is generated at the end of the transfer.
+        Returns a `bytes` object with the data read.
+        """
+        ...
+    def readinto(self, buf, nack=True, /) -> Any:
+        """
+        Reads bytes from the bus and stores them into *buf*.  The number of bytes
+        read is the length of *buf*.  An ACK will be sent on the bus after
+        receiving all but the last byte.  After the last byte is received, if *nack*
+        is true then a NACK will be sent, otherwise an ACK will be sent (and in this
+        case the peripheral assumes more bytes are going to be read in a later call).
+        """
+        ...
+    def init(self, scl, sda, *, freq=400000) -> None:
+        """
+        Initialise the I2C bus with the given arguments:
+
+           - *scl* is a pin object for the SCL line
+           - *sda* is a pin object for the SDA line
+           - *freq* is the SCL clock rate
+
+         In the case of hardware I2C the actual clock frequency may be lower than the
+         requested frequency. This is dependant on the platform hardware. The actual
+         rate may be determined by printing the I2C object.
+        """
+        ...
+    def stop(self) -> None:
+        """
+        Generate a STOP condition on the bus (SDA transitions to high while SCL is high).
+        """
+        ...
+    def write(self, buf) -> int:
+        """
+        Write the bytes from *buf* to the bus.  Checks that an ACK is received
+        after each byte and stops transmitting the remaining bytes if a NACK is
+        received.  The function returns the number of ACKs that were received.
+        """
+        ...
+    def __init__(
+        self,
+        id: Union[int, str] = -1,
+        *,
+        scl: Optional[Union[Pin, str]] = None,
+        sda: Optional[Union[Pin, str]] = None,
+        freq=400_000,
+        timeout=50000,
+    ) -> None: ...
+
+class I2S:
+    """
+    Construct an I2S object of the given id:
+
+    - ``id`` identifies a particular I2S bus; it is board and port specific
+
+    Keyword-only parameters that are supported on all ports:
+
+      - ``sck`` is a pin object for the serial clock line
+      - ``ws`` is a pin object for the word select line
+      - ``sd`` is a pin object for the serial data line
+      - ``mck`` is a pin object for the master clock line;
+        master clock frequency is sampling rate * 256
+      - ``mode`` specifies receive or transmit
+      - ``bits`` specifies sample size (bits), 16 or 32
+      - ``format`` specifies channel format, STEREO or MONO
+      - ``rate`` specifies audio sampling rate (Hz);
+        this is the frequency of the ``ws`` signal
+      - ``ibuf`` specifies internal buffer length (bytes)
+
+    For all ports, DMA runs continuously in the background and allows user applications to perform other operations while
+    sample data is transfered between the internal buffer and the I2S peripheral unit.
+    Increasing the size of the internal buffer has the potential to increase the time that user applications can perform non-I2S operations
+    before underflow (e.g. ``write`` method) or overflow (e.g. ``readinto`` method).
+    """
+
+    RX: int
+    MONO: int
+    STEREO: int
+    TX: int
+    @staticmethod
+    def shift(*, buf, bits, shift) -> Any:
+        """
+        bitwise shift of all samples contained in ``buf``. ``bits`` specifies sample size in bits. ``shift`` specifies the number of bits to shift each sample.
+        Positive for left shift, negative for right shift.
+        Typically used for volume control.  Each bit shift changes sample volume by 6dB.
+        """
+        ...
+    def init(self, sck, *args, **kwargs) -> Any:
+        """
+        see Constructor for argument descriptions
+        """
+        ...
+    def irq(self, handler) -> Any:
+        """
+        Set a callback. ``handler`` is called when ``buf`` is emptied (``write`` method) or becomes full (``readinto`` method).
+        Setting a callback changes the ``write`` and ``readinto`` methods to non-blocking operation.
+        ``handler`` is called in the context of the MicroPython scheduler.
+        """
+        ...
+    def readinto(self, buf) -> int:
+        """
+        Read audio samples into the buffer specified by ``buf``.  ``buf`` must support the buffer protocol, such as bytearray or array.
+        "buf" byte ordering is little-endian.  For Stereo format, left channel sample precedes right channel sample. For Mono format,
+        the left channel sample data is used.
+        Returns number of bytes read
+        """
+        ...
+    def deinit(self) -> Any:
+        """
+        Deinitialize the I2S bus
+        """
+        ...
+    def write(self, buf) -> int:
+        """
+        Write audio samples contained in ``buf``. ``buf`` must support the buffer protocol, such as bytearray or array.
+        "buf" byte ordering is little-endian.  For Stereo format, left channel sample precedes right channel sample. For Mono format,
+        the sample data is written to both the right and left channels.
+        Returns number of bytes written
+        """
+        ...
+    def __init__(self, id, *, sck, ws, sd, mck=None, mode, bits, format, rate, ibuf) -> None: ...
+
+class Pin:
+    """
+    Access the pin peripheral (GPIO pin) associated with the given ``id``.  If
+    additional arguments are given in the constructor then they are used to initialise
+    the pin.  Any settings that are not specified will remain in their previous state.
+
+    The arguments are:
+
+      - ``id`` is mandatory and can be an arbitrary object.  Among possible value
+        types are: int (an internal Pin identifier), str (a Pin name), and tuple
+        (pair of [port, pin]).
+
+      - ``mode`` specifies the pin mode, which can be one of:
+
+        - ``Pin.IN`` - Pin is configured for input.  If viewed as an output the pin
+          is in high-impedance state.
+
+        - ``Pin.OUT`` - Pin is configured for (normal) output.
+
+        - ``Pin.OPEN_DRAIN`` - Pin is configured for open-drain output. Open-drain
+          output works in the following way: if the output value is set to 0 the pin
+          is active at a low level; if the output value is 1 the pin is in a high-impedance
+          state.  Not all ports implement this mode, or some might only on certain pins.
+
+        - ``Pin.ALT`` - Pin is configured to perform an alternative function, which is
+          port specific.  For a pin configured in such a way any other Pin methods
+          (except :meth:`Pin.init`) are not applicable (calling them will lead to undefined,
+          or a hardware-specific, result).  Not all ports implement this mode.
+
+        - ``Pin.ALT_OPEN_DRAIN`` - The Same as ``Pin.ALT``, but the pin is configured as
+          open-drain.  Not all ports implement this mode.
+
+        - ``Pin.ANALOG`` - Pin is configured for analog input, see the :class:`ADC` class.
+
+      - ``pull`` specifies if the pin has a (weak) pull resistor attached, and can be
+        one of:
+
+        - ``None`` - No pull up or down resistor.
+        - ``Pin.PULL_UP`` - Pull up resistor enabled.
+        - ``Pin.PULL_DOWN`` - Pull down resistor enabled.
+
+      - ``value`` is valid only for Pin.OUT and Pin.OPEN_DRAIN modes and specifies initial
+        output pin value if given, otherwise the state of the pin peripheral remains
+        unchanged.
+
+      - ``drive`` specifies the output power of the pin and can be one of: ``Pin.DRIVE_0``,
+        ``Pin.DRIVE_1``, etc., increasing in drive strength.  The actual current driving
+        capabilities are port dependent.  Not all ports implement this argument.
+
+      - ``alt`` specifies an alternate function for the pin and the values it can take are
+        port dependent.  This argument is valid only for ``Pin.ALT`` and ``Pin.ALT_OPEN_DRAIN``
+        modes.  It may be used when a pin supports more than one alternate function.  If only
+        one pin alternate function is supported the this argument is not required.  Not all
+        ports implement this argument.
+
+    As specified above, the Pin class allows to set an alternate function for a particular
+    pin, but it does not specify any further operations on such a pin.  Pins configured in
+    alternate-function mode are usually not used as GPIO but are instead driven by other
+    hardware peripherals.  The only operation supported on such a pin is re-initialising,
+    by calling the constructor or :meth:`Pin.init` method.  If a pin that is configured in
+    alternate-function mode is re-initialised with ``Pin.IN``, ``Pin.OUT``, or
+    ``Pin.OPEN_DRAIN``, the alternate function will be removed from the pin.
+    """
+
+    ALT_SPI: int
+    IN: int
+    ALT_USB: int
+    ALT_UART: int
+    IRQ_FALLING: int
+    OUT: int
+    OPEN_DRAIN: int
+    IRQ_RISING: int
+    PULL_DOWN: int
+    ALT_SIO: int
+    ALT_GPCK: int
+    ALT: int
+    PULL_UP: int
+    ALT_I2C: int
+    ALT_PWM: int
+    ALT_PIO1: int
+    ALT_PIO0: int
+    def low(self) -> None:
+        """
+        Set pin to "0" output level.
+
+        Availability: nrf, rp2, stm32 ports.
+        """
+        ...
+    def irq(self, handler=None, trigger=IRQ_FALLING, *, priority=1, wake=None, hard=False) -> Callable[..., Any]:
+        """
+           Configure an interrupt handler to be called when the trigger source of the
+           pin is active.  If the pin mode is ``Pin.IN`` then the trigger source is
+           the external value on the pin.  If the pin mode is ``Pin.OUT`` then the
+           trigger source is the output buffer of the pin.  Otherwise, if the pin mode
+           is ``Pin.OPEN_DRAIN`` then the trigger source is the output buffer for
+           state '0' and the external pin value for state '1'.
+
+           The arguments are:
+
+             - ``handler`` is an optional function to be called when the interrupt
+               triggers. The handler must take exactly one argument which is the
+               ``Pin`` instance.
+
+             - ``trigger`` configures the event which can generate an interrupt.
+               Possible values are:
+
+               - ``Pin.IRQ_FALLING`` interrupt on falling edge.
+               - ``Pin.IRQ_RISING`` interrupt on rising edge.
+               - ``Pin.IRQ_LOW_LEVEL`` interrupt on low level.
+               - ``Pin.IRQ_HIGH_LEVEL`` interrupt on high level.
+
+               These values can be OR'ed together to trigger on multiple events.
+
+             - ``priority`` sets the priority level of the interrupt.  The values it
+               can take are port-specific, but higher values always represent higher
+               priorities.
+
+             - ``wake`` selects the power mode in which this interrupt can wake up the
+               system.  It can be ``machine.IDLE``, ``machine.SLEEP`` or ``machine.DEEPSLEEP``.
+               These values can also be OR'ed together to make a pin generate interrupts in
+               more than one power mode.
+
+             - ``hard`` if true a hardware interrupt is used. This reduces the delay
+               between the pin change and the handler being called. Hard interrupt
+               handlers may not allocate memory; see :ref:`isr_rules`.
+               Not all ports support this argument.
+
+           This method returns a callback object.
+
+        The following methods are not part of the core Pin API and only implemented on certain ports.
+        """
+        ...
+    def toggle(self, *args, **kwargs) -> Any: ...
+    def off(self) -> None:
+        """
+        Set pin to "0" output level.
+        """
+        ...
+    def on(self) -> None:
+        """
+        Set pin to "1" output level.
+        """
+        ...
+    def init(self, mode=-1, pull=-1, *, value=None, drive=0, alt=-1) -> None:
+        """
+        Re-initialise the pin using the given parameters.  Only those arguments that
+        are specified will be set.  The rest of the pin peripheral state will remain
+        unchanged.  See the constructor documentation for details of the arguments.
+
+        Returns ``None``.
+        """
+        ...
+    def value(self, x: Optional[Any] = None) -> int:
+        """
+        This method allows to set and get the value of the pin, depending on whether
+        the argument ``x`` is supplied or not.
+
+        If the argument is omitted then this method gets the digital logic level of
+        the pin, returning 0 or 1 corresponding to low and high voltage signals
+        respectively.  The behaviour of this method depends on the mode of the pin:
+
+          - ``Pin.IN`` - The method returns the actual input value currently present
+            on the pin.
+          - ``Pin.OUT`` - The behaviour and return value of the method is undefined.
+          - ``Pin.OPEN_DRAIN`` - If the pin is in state '0' then the behaviour and
+            return value of the method is undefined.  Otherwise, if the pin is in
+            state '1', the method returns the actual input value currently present
+            on the pin.
+
+        If the argument is supplied then this method sets the digital logic level of
+        the pin.  The argument ``x`` can be anything that converts to a boolean.
+        If it converts to ``True``, the pin is set to state '1', otherwise it is set
+        to state '0'.  The behaviour of this method depends on the mode of the pin:
+
+          - ``Pin.IN`` - The value is stored in the output buffer for the pin.  The
+            pin state does not change, it remains in the high-impedance state.  The
+            stored value will become active on the pin as soon as it is changed to
+            ``Pin.OUT`` or ``Pin.OPEN_DRAIN`` mode.
+          - ``Pin.OUT`` - The output buffer is set to the given value immediately.
+          - ``Pin.OPEN_DRAIN`` - If the value is '0' the pin is set to a low voltage
+            state.  Otherwise the pin is set to high-impedance state.
+
+        When setting the value this method returns ``None``.
+        """
+        ...
+    def high(self) -> None:
+        """
+        Set pin to "1" output level.
+
+        Availability: nrf, rp2, stm32 ports.
+        """
+        ...
+
+    class cpu:
+        GPIO26: Any
+        GPIO25: Any
+        GPIO27: Any
+        GPIO28: Any
+        GPIO22: Any
+        GPIO24: Any
+        GPIO23: Any
+        GPIO9: Any
+        GPIO7: Any
+        GPIO6: Any
+        GPIO8: Any
+        GPIO29: Any
+        GPIO3: Any
+        GPIO5: Any
+        GPIO4: Any
+        GPIO12: Any
+        GPIO11: Any
+        GPIO13: Any
+        GPIO14: Any
+        GPIO0: Any
+        GPIO10: Any
+        GPIO1: Any
+        GPIO21: Any
+        GPIO2: Any
+        GPIO19: Any
+        GPIO20: Any
+        GPIO15: Any
+        GPIO16: Any
+        GPIO18: Any
+        GPIO17: Any
+        def __init__(self, *argv, **kwargs) -> None: ...
+
+    class board:
+        GP27: Any
+        GP26: Any
+        GP28: Any
+        LED: Any
+        GP21: Any
+        GP25: Any
+        GP22: Any
+        GP8: Any
+        GP7: Any
+        GP9: Any
+        GP3: Any
+        GP4: Any
+        GP6: Any
+        GP5: Any
+        GP12: Any
+        GP11: Any
+        GP13: Any
+        GP20: Any
+        GP0: Any
+        GP10: Any
+        GP1: Any
+        GP19: Any
+        GP18: Any
+        GP2: Any
+        GP14: Any
+        GP15: Any
+        GP17: Any
+        GP16: Any
+        def __init__(self, *argv, **kwargs) -> None: ...
+
+    def __init__(self, id, mode=-1, pull=-1, *, value=None, drive=0, alt=-1) -> None: ...
+    def __call__(self, x: Optional[Any] = None) -> Any:
+        """
+        Pin objects are callable.  The call method provides a (fast) shortcut to set
+        and get the value of the pin.  It is equivalent to Pin.value([x]).
+        See :meth:`Pin.value` for more details.
+        """
+        ...
+
+class SoftSPI:
+    """
+    Construct a new software SPI object.  Additional parameters must be
+    given, usually at least *sck*, *mosi* and *miso*, and these are used
+    to initialise the bus.  See `SPI.init` for a description of the parameters.
+    """
+
+    LSB: int
+    MSB: int
+    def deinit(self, *args, **kwargs) -> Any: ...
+    def init(self, *args, **kwargs) -> Any: ...
+    def write_readinto(self, *args, **kwargs) -> Any: ...
+    def read(self, *args, **kwargs) -> Any: ...
+    def write(self, *args, **kwargs) -> Any: ...
+    def readinto(self, *args, **kwargs) -> Any: ...
+    def __init__(self, baudrate=500000, *, polarity=0, phase=0, bits=8, firstbit=MSB, sck=None, mosi=None, miso=None) -> None: ...
+
+class Timer:
+    """
+    Construct a new timer object of the given ``id``. ``id`` of -1 constructs a
+    virtual timer (if supported by a board).
+    ``id`` shall not be passed as a keyword argument.
+
+    See ``init`` for parameters of initialisation.
+    """
+
+    PERIODIC: int
+    ONE_SHOT: int
+    def init(self, *, mode=PERIODIC, freq=-1, period=-1, callback=None) -> None:
+        """
+        Initialise the timer. Example::
+
+            def mycallback(t):
+                pass
+
+            # periodic at 1kHz
+            tim.init(mode=Timer.PERIODIC, freq=1000, callback=mycallback)
+
+            # periodic with 100ms period
+            tim.init(period=100, callback=mycallback)
+
+            # one shot firing after 1000ms
+            tim.init(mode=Timer.ONE_SHOT, period=1000, callback=mycallback)
+
+        Keyword arguments:
+
+          - ``mode`` can be one of:
+
+            - ``Timer.ONE_SHOT`` - The timer runs once until the configured
+              period of the channel expires.
+            - ``Timer.PERIODIC`` - The timer runs periodically at the configured
+              frequency of the channel.
+
+          - ``freq`` - The timer frequency, in units of Hz.  The upper bound of
+            the frequency is dependent on the port.  When both the ``freq`` and
+            ``period`` arguments are given, ``freq`` has a higher priority and
+            ``period`` is ignored.
+
+          - ``period`` - The timer period, in milliseconds.
+
+          - ``callback`` - The callable to call upon expiration of the timer period.
+            The callback must take one argument, which is passed the Timer object.
+            The ``callback`` argument shall be specified. Otherwise an exception
+            will occurr upon timer expiration:
+            ``TypeError: 'NoneType' object isn't callable``
+        """
+        ...
+    def deinit(self) -> None:
+        """
+        Deinitialises the timer. Stops the timer, and disables the timer peripheral.
+        """
+        ...
+    def __init__(self, id=-1, *args, **kwargs) -> None: ...
+
+class UART:
+    """
+    Construct a UART object of the given id.
+    """
+
+    INV_TX: int
+    RTS: int
+    CTS: int
+    INV_RX: int
+    def deinit(self) -> None:
+        """
+        Turn off the UART bus.
+
+        .. note::
+          You will not be able to call ``init()`` on the object after ``deinit()``.
+          A new instance needs to be created in that case.
+        """
+        ...
+    def sendbreak(self) -> None:
+        """
+        Send a break condition on the bus. This drives the bus low for a duration
+        longer than required for a normal transmission of a character.
+        """
+        ...
+    def init(self, baudrate=9600, bits=8, parity=None, stop=1, *args, **kwargs) -> None:
+        """
+        Initialise the UART bus with the given parameters:
+
+          - *baudrate* is the clock rate.
+          - *bits* is the number of bits per character, 7, 8 or 9.
+          - *parity* is the parity, ``None``, 0 (even) or 1 (odd).
+          - *stop* is the number of stop bits, 1 or 2.
+
+        Additional keyword-only parameters that may be supported by a port are:
+
+          - *tx* specifies the TX pin to use.
+          - *rx* specifies the RX pin to use.
+          - *rts* specifies the RTS (output) pin to use for hardware receive flow control.
+          - *cts* specifies the CTS (input) pin to use for hardware transmit flow control.
+          - *txbuf* specifies the length in characters of the TX buffer.
+          - *rxbuf* specifies the length in characters of the RX buffer.
+          - *timeout* specifies the time to wait for the first character (in ms).
+          - *timeout_char* specifies the time to wait between characters (in ms).
+          - *invert* specifies which lines to invert.
+
+              - ``0`` will not invert lines (idle state of both lines is logic high).
+              - ``UART.INV_TX`` will invert TX line (idle state of TX line now logic low).
+              - ``UART.INV_RX`` will invert RX line (idle state of RX line now logic low).
+              - ``UART.INV_TX | UART.INV_RX`` will invert both lines (idle state at logic low).
+
+          - *flow* specifies which hardware flow control signals to use. The value
+            is a bitmask.
+
+              - ``0`` will ignore hardware flow control signals.
+              - ``UART.RTS`` will enable receive flow control by using the RTS output pin to
+                signal if the receive FIFO has sufficient space to accept more data.
+              - ``UART.CTS`` will enable transmit flow control by pausing transmission when the
+                CTS input pin signals that the receiver is running low on buffer space.
+              - ``UART.RTS | UART.CTS`` will enable both, for full hardware flow control.
+
+        On the WiPy only the following keyword-only parameter is supported:
+
+          - *pins* is a 4 or 2 item list indicating the TX, RX, RTS and CTS pins (in that order).
+            Any of the pins can be None if one wants the UART to operate with limited functionality.
+            If the RTS pin is given the the RX pin must be given as well. The same applies to CTS.
+            When no pins are given, then the default set of TX and RX pins is taken, and hardware
+            flow control will be disabled. If *pins* is ``None``, no pin assignment will be made.
+
+        .. note::
+          It is possible to call ``init()`` multiple times on the same object in
+          order to reconfigure  UART on the fly. That allows using single UART
+          peripheral to serve different devices attached to different GPIO pins.
+          Only one device can be served at a time in that case.
+          Also do not call ``deinit()`` as it will prevent calling ``init()``
+          again.
+        """
+        ...
+    def flush(self) -> Any:
+        """
+        Waits until all data has been sent. In case of a timeout, an exception is raised. The timeout
+        duration depends on the tx buffer size and the baud rate. Unless flow control is enabled, a timeout
+        should not occur.
+
+        .. note::
+
+            For the rp2, esp8266 and nrf ports the call returns while the last byte is sent.
+            If required, a one character wait time has to be added in the calling script.
+
+        Availability: rp2, esp32, esp8266, mimxrt, cc3200, stm32, nrf ports, renesas-ra
+        """
+        ...
+    def txdone(self) -> bool:
+        """
+        Tells whether all data has been sent or no data transfer is happening. In this case,
+        it returns ``True``. If a data transmission is ongoing it returns ``False``.
+
+        .. note::
+
+            For the rp2, esp8266 and nrf ports the call may return ``True`` even if the last byte
+            of a transfer is still being sent. If required, a one character wait time has to be
+            added in the calling script.
+
+        Availability: rp2, esp32, esp8266, mimxrt, cc3200, stm32, nrf ports, renesas-ra
+        """
+        ...
+    def read(self, nbytes: Optional[Any] = None) -> bytes:
+        """
+        Read characters.  If ``nbytes`` is specified then read at most that many bytes,
+        otherwise read as much data as possible. It may return sooner if a timeout
+        is reached. The timeout is configurable in the constructor.
+
+        Return value: a bytes object containing the bytes read in.  Returns ``None``
+        on timeout.
+        """
+        ...
+    def any(self) -> int:
+        """
+        Returns an integer counting the number of characters that can be read without
+        blocking.  It will return 0 if there are no characters available and a positive
+        number if there are characters.  The method may return 1 even if there is more
+        than one character available for reading.
+
+        For more sophisticated querying of available characters use select.poll::
+
+         poll = select.poll()
+         poll.register(uart, select.POLLIN)
+         poll.poll(timeout)
+        """
+        ...
+    def write(self, buf) -> int:
+        """
+        Write the buffer of bytes to the bus.
+
+        Return value: number of bytes written or ``None`` on timeout.
+        """
+        ...
+    def readinto(self, buf, nbytes: Optional[Any] = None) -> int:
+        """
+        Read bytes into the ``buf``.  If ``nbytes`` is specified then read at most
+        that many bytes.  Otherwise, read at most ``len(buf)`` bytes. It may return sooner if a timeout
+        is reached. The timeout is configurable in the constructor.
+
+        Return value: number of bytes read and stored into ``buf`` or ``None`` on
+        timeout.
+        """
+        ...
+    def readline(self) -> None:
+        """
+        Read a line, ending in a newline character. It may return sooner if a timeout
+        is reached. The timeout is configurable in the constructor.
+
+        Return value: the line read or ``None`` on timeout.
+        """
+        ...
+    def __init__(self, id, *args, **kwargs) -> None: ...
+
+class SoftI2C(I2C):
+    """
+    Construct a new software I2C object.  The parameters are:
+
+       - *scl* should be a pin object specifying the pin to use for SCL.
+       - *sda* should be a pin object specifying the pin to use for SDA.
+       - *freq* should be an integer which sets the maximum frequency
+         for SCL.
+       - *timeout* is the maximum time in microseconds to wait for clock
+         stretching (SCL held low by another device on the bus), after
+         which an ``OSError(ETIMEDOUT)`` exception is raised.
+    """
+
+    def readfrom_mem_into(self, *args, **kwargs) -> Any: ...
+    def readfrom_into(self, *args, **kwargs) -> Any: ...
+    def readfrom_mem(self, *args, **kwargs) -> Any: ...
+    def writeto_mem(self, *args, **kwargs) -> Any: ...
+    def scan(self, *args, **kwargs) -> Any: ...
+    def writeto(self, *args, **kwargs) -> Any: ...
+    def writevto(self, *args, **kwargs) -> Any: ...
+    def start(self, *args, **kwargs) -> Any: ...
+    def readfrom(self, *args, **kwargs) -> Any: ...
+    def readinto(self, *args, **kwargs) -> Any: ...
+    def init(self, *args, **kwargs) -> Any: ...
+    def stop(self, *args, **kwargs) -> Any: ...
+    def write(self, *args, **kwargs) -> Any: ...
+    def __init__(self, scl, sda, *, freq=400000, timeout=50000) -> None: ...
+
+class RTC:
+    """
+    Create an RTC object. See init for parameters of initialization.
+    """
+
+    def datetime(self, datetimetuple: Optional[Any] = None) -> Tuple:
+        """
+        Get or set the date and time of the RTC.
+
+        With no arguments, this method returns an 8-tuple with the current
+        date and time.  With 1 argument (being an 8-tuple) it sets the date
+        and time.
+
+        The 8-tuple has the following format:
+
+            (year, month, day, weekday, hours, minutes, seconds, subseconds)
+
+        The meaning of the ``subseconds`` field is hardware dependent.
+        """
+        ...
+    def __init__(self, id=0, *args, **kwargs) -> None: ...
+
+class SPI:
+    """
+    Construct an SPI object on the given bus, *id*. Values of *id* depend
+    on a particular port and its hardware. Values 0, 1, etc. are commonly used
+    to select hardware SPI block #0, #1, etc.
+
+    With no additional parameters, the SPI object is created but not
+    initialised (it has the settings from the last initialisation of
+    the bus, if any).  If extra arguments are given, the bus is initialised.
+    See ``init`` for parameters of initialisation.
+    """
+
+    LSB: int
+    MSB: int
+    def deinit(self) -> None:
+        """
+        Turn off the SPI bus.
+        """
+        ...
+    def init(
+        self, baudrate=1000000, *, polarity=0, phase=0, bits=8, firstbit=MSB, sck=None, mosi=None, miso=None, pins: Optional[Tuple]
+    ) -> None:
+        """
+        Initialise the SPI bus with the given parameters:
+
+          - ``baudrate`` is the SCK clock rate.
+          - ``polarity`` can be 0 or 1, and is the level the idle clock line sits at.
+          - ``phase`` can be 0 or 1 to sample data on the first or second clock edge
+            respectively.
+          - ``bits`` is the width in bits of each transfer. Only 8 is guaranteed to be supported by all hardware.
+          - ``firstbit`` can be ``SPI.MSB`` or ``SPI.LSB``.
+          - ``sck``, ``mosi``, ``miso`` are pins (machine.Pin) objects to use for bus signals. For most
+            hardware SPI blocks (as selected by ``id`` parameter to the constructor), pins are fixed
+            and cannot be changed. In some cases, hardware blocks allow 2-3 alternative pin sets for
+            a hardware SPI block. Arbitrary pin assignments are possible only for a bitbanging SPI driver
+            (``id`` = -1).
+          - ``pins`` - WiPy port doesn't ``sck``, ``mosi``, ``miso`` arguments, and instead allows to
+            specify them as a tuple of ``pins`` parameter.
+
+        In the case of hardware SPI the actual clock frequency may be lower than the
+        requested baudrate. This is dependant on the platform hardware. The actual
+        rate may be determined by printing the SPI object.
+        """
+        ...
+    def write_readinto(self, write_buf, read_buf) -> int:
+        """
+        Write the bytes from ``write_buf`` while reading into ``read_buf``.  The
+        buffers can be the same or different, but both buffers must have the
+        same length.
+        Returns ``None``.
+
+        Note: on WiPy this function returns the number of bytes written.
+        """
+        ...
+    def read(self, nbytes, write=0x00) -> bytes:
+        """
+        Read a number of bytes specified by ``nbytes`` while continuously writing
+        the single byte given by ``write``.
+        Returns a ``bytes`` object with the data that was read.
+        """
+        ...
+    def write(self, buf) -> int:
+        """
+        Write the bytes contained in ``buf``.
+        Returns ``None``.
+
+        Note: on WiPy this function returns the number of bytes written.
+        """
+        ...
+    def readinto(self, buf, write=0x00) -> int:
+        """
+        Read into the buffer specified by ``buf`` while continuously writing the
+        single byte given by ``write``.
+        Returns ``None``.
+
+        Note: on WiPy this function returns the number of bytes read.
+        """
+        ...
+    def __init__(self, id, *args, **kwargs) -> None: ...
+
+class Signal(Pin):
+    """
+            Signal(pin_arguments..., *, invert=False)
+
+    Create a Signal object. There're two ways to create it:
+
+    * By wrapping existing Pin object - universal method which works for
+      any board.
+    * By passing required Pin parameters directly to Signal constructor,
+      skipping the need to create intermediate Pin object. Available on
+      many, but not all boards.
+
+    The arguments are:
+
+      - ``pin_obj`` is existing Pin object.
+
+      - ``pin_arguments`` are the same arguments as can be passed to Pin constructor.
+
+      - ``invert`` - if True, the signal will be inverted (active low).
+    """
+
+    def off(self) -> None:
+        """
+        Deactivate signal.
+        """
+        ...
+    def on(self) -> None:
+        """
+        Activate signal.
+        """
+        ...
+    def value(self, x: Optional[Any] = None) -> int:
+        """
+        This method allows to set and get the value of the signal, depending on whether
+        the argument ``x`` is supplied or not.
+
+        If the argument is omitted then this method gets the signal level, 1 meaning
+        signal is asserted (active) and 0 - signal inactive.
+
+        If the argument is supplied then this method sets the signal level. The
+        argument ``x`` can be anything that converts to a boolean. If it converts
+        to ``True``, the signal is active, otherwise it is inactive.
+
+        Correspondence between signal being active and actual logic level on the
+        underlying pin depends on whether signal is inverted (active-low) or not.
+        For non-inverted signal, active status corresponds to logical 1, inactive -
+        to logical 0. For inverted/active-low signal, active status corresponds
+        to logical 0, while inactive - to logical 1.
+        """
+        ...
+    def __init__(self, pin_obj, *args, invert=False) -> None: ...
```

### Comparing `micropython_rp2_stubs-1.19.1.post9/uos.pyi` & `micropython_rp2_stubs-1.20.0.post1/uos.pyi`

 * *Files 21% similar despite different names*

```diff
@@ -1,244 +1,244 @@
-"""
-basic "operating system" services. See: https://docs.micropython.org/en/v1.19.1/library/os.html
-
-|see_cpython_module| :mod:`python:os` https://docs.python.org/3/library/os.html .
-
-The ``os`` module contains functions for filesystem access and mounting,
-terminal redirection and duplication, and the ``uname`` and ``urandom``
-functions.
-"""
-from typing import IO, Iterator, Optional, Tuple, Any
-from stdlib.os import uname_result
-
-def stat(path) -> Any:
-    """
-    Get the status of a file or directory.
-    """
-    ...
-
-def rmdir(path) -> None:
-    """
-    Remove a directory.
-    """
-    ...
-
-def rename(old_path, new_path) -> None:
-    """
-    Rename a file.
-    """
-    ...
-
-def mount(fsobj, mount_point, *, readonly) -> Any:
-    """
-    Mount the filesystem object *fsobj* at the location in the VFS given by the
-    *mount_point* string.  *fsobj* can be a a VFS object that has a ``mount()``
-    method, or a block device.  If it's a block device then the filesystem type
-    is automatically detected (an exception is raised if no filesystem was
-    recognised).  *mount_point* may be ``'/'`` to mount *fsobj* at the root,
-    or ``'/<name>'`` to mount it at a subdirectory under the root.
-
-    If *readonly* is ``True`` then the filesystem is mounted read-only.
-
-    During the mount process the method ``mount()`` is called on the filesystem
-    object.
-
-    Will raise ``OSError(EPERM)`` if *mount_point* is already mounted.
-    """
-    ...
-
-def urandom(n) -> bytes:
-    """
-    Return a bytes object with *n* random bytes. Whenever possible, it is
-    generated by the hardware random number generator.
-    """
-    ...
-
-def statvfs(path) -> Tuple:
-    """
-    Get the status of a fileystem.
-
-    Returns a tuple with the filesystem information in the following order:
-
-         * ``f_bsize`` -- file system block size
-         * ``f_frsize`` -- fragment size
-         * ``f_blocks`` -- size of fs in f_frsize units
-         * ``f_bfree`` -- number of free blocks
-         * ``f_bavail`` -- number of free blocks for unprivileged users
-         * ``f_files`` -- number of inodes
-         * ``f_ffree`` -- number of free inodes
-         * ``f_favail`` -- number of free inodes for unprivileged users
-         * ``f_flag`` -- mount flags
-         * ``f_namemax`` -- maximum filename length
-
-    Parameters related to inodes: ``f_files``, ``f_ffree``, ``f_avail``
-    and the ``f_flags`` parameter may return ``0`` as they can be unavailable
-    in a port-specific implementation.
-    """
-    ...
-
-def unlink(*args, **kwargs) -> Any: ...
-def uname() -> uname_result:
-    """
-    Return a tuple (possibly a named tuple) containing information about the
-    underlying machine and/or its operating system.  The tuple has five fields
-    in the following order, each of them being a string:
-
-         * ``sysname`` -- the name of the underlying system
-         * ``nodename`` -- the network name (can be the same as ``sysname``)
-         * ``release`` -- the version of the underlying system
-         * ``version`` -- the MicroPython version and build date
-         * ``machine`` -- an identifier for the underlying hardware (eg board, CPU)
-    """
-    ...
-
-def umount(mount_point) -> Any:
-    """
-    Unmount a filesystem. *mount_point* can be a string naming the mount location,
-    or a previously-mounted filesystem object.  During the unmount process the
-    method ``umount()`` is called on the filesystem object.
-
-    Will raise ``OSError(EINVAL)`` if *mount_point* is not found.
-    """
-    ...
-
-def chdir(path) -> Any:
-    """
-    Change current directory.
-    """
-    ...
-
-def dupterm(stream_object, index=0, /) -> IO:
-    """
-    Duplicate or switch the MicroPython terminal (the REPL) on the given `stream`-like
-    object. The *stream_object* argument must be a native stream object, or derive
-    from ``io.IOBase`` and implement the ``readinto()`` and
-    ``write()`` methods.  The stream should be in non-blocking mode and
-    ``readinto()`` should return ``None`` if there is no data available for reading.
-
-    After calling this function all terminal output is repeated on this stream,
-    and any input that is available on the stream is passed on to the terminal input.
-
-    The *index* parameter should be a non-negative integer and specifies which
-    duplication slot is set.  A given port may implement more than one slot (slot 0
-    will always be available) and in that case terminal input and output is
-    duplicated on all the slots that are set.
-
-    If ``None`` is passed as the *stream_object* then duplication is cancelled on
-    the slot given by *index*.
-
-    The function returns the previous stream-like object in the given slot.
-    """
-    ...
-
-def remove(path) -> None:
-    """
-    Remove a file.
-    """
-    ...
-
-def mkdir(path) -> Any:
-    """
-    Create a new directory.
-    """
-    ...
-
-def getcwd() -> Any:
-    """
-    Get the current directory.
-    """
-    ...
-
-def listdir(dir: Optional[Any] = None) -> Any:
-    """
-    With no argument, list the current directory.  Otherwise list the given directory.
-    """
-    ...
-
-def ilistdir(dir: Optional[Any] = None) -> Iterator[Tuple]:
-    """
-    This function returns an iterator which then yields tuples corresponding to
-    the entries in the directory that it is listing.  With no argument it lists the
-    current directory, otherwise it lists the directory given by *dir*.
-
-    The tuples have the form *(name, type, inode[, size])*:
-
-     - *name* is a string (or bytes if *dir* is a bytes object) and is the name of
-       the entry;
-     - *type* is an integer that specifies the type of the entry, with 0x4000 for
-       directories and 0x8000 for regular files;
-     - *inode* is an integer corresponding to the inode of the file, and may be 0
-       for filesystems that don't have such a notion.
-     - Some platforms may return a 4-tuple that includes the entry's *size*.  For
-       file entries, *size* is an integer representing the size of the file
-       or -1 if unknown.  Its meaning is currently undefined for directory
-       entries.
-    """
-    ...
-
-class VfsLfs2:
-    """
-    Create a filesystem object that uses the `littlefs v2 filesystem format`_.
-    Storage of the littlefs filesystem is provided by *block_dev*, which must
-    support the :ref:`extended interface <block-device-interface>`.
-    Objects created by this constructor can be mounted using :func:`mount`.
-
-    The *mtime* argument enables modification timestamps for files, stored using
-    littlefs attributes.  This option can be disabled or enabled differently each
-    mount time and timestamps will only be added or updated if *mtime* is enabled,
-    otherwise the timestamps will remain untouched.  Littlefs v2 filesystems without
-    timestamps will work without reformatting and timestamps will be added
-    transparently to existing files once they are opened for writing.  When *mtime*
-    is enabled `os.stat` on files without timestamps will return 0 for the timestamp.
-
-    See :ref:`filesystem` for more information.
-    """
-
-    def rename(self, *args, **kwargs) -> Any: ...
-    @staticmethod
-    def mkfs(block_dev, readsize=32, progsize=32, lookahead=32) -> None:
-        """
-            Build a Lfs2 filesystem on *block_dev*.
-
-        ``Note:`` There are reports of littlefs v2 failing in certain situations,
-                  for details see `littlefs issue 295`_.
-        """
-        ...
-    def mount(self, *args, **kwargs) -> Any: ...
-    def statvfs(self, *args, **kwargs) -> Any: ...
-    def rmdir(self, *args, **kwargs) -> Any: ...
-    def stat(self, *args, **kwargs) -> Any: ...
-    def umount(self, *args, **kwargs) -> Any: ...
-    def remove(self, *args, **kwargs) -> Any: ...
-    def mkdir(self, *args, **kwargs) -> Any: ...
-    def open(self, *args, **kwargs) -> Any: ...
-    def ilistdir(self, *args, **kwargs) -> Any: ...
-    def chdir(self, *args, **kwargs) -> Any: ...
-    def getcwd(self, *args, **kwargs) -> Any: ...
-    def __init__(self, block_dev, readsize=32, progsize=32, lookahead=32, mtime=True) -> None: ...
-
-class VfsFat:
-    """
-    Create a filesystem object that uses the FAT filesystem format.  Storage of
-    the FAT filesystem is provided by *block_dev*.
-    Objects created by this constructor can be mounted using :func:`mount`.
-    """
-
-    def rename(self, *args, **kwargs) -> Any: ...
-    @staticmethod
-    def mkfs(block_dev) -> None:
-        """
-        Build a FAT filesystem on *block_dev*.
-        """
-        ...
-    def mount(self, *args, **kwargs) -> Any: ...
-    def statvfs(self, *args, **kwargs) -> Any: ...
-    def rmdir(self, *args, **kwargs) -> Any: ...
-    def stat(self, *args, **kwargs) -> Any: ...
-    def umount(self, *args, **kwargs) -> Any: ...
-    def remove(self, *args, **kwargs) -> Any: ...
-    def mkdir(self, *args, **kwargs) -> Any: ...
-    def open(self, *args, **kwargs) -> Any: ...
-    def ilistdir(self, *args, **kwargs) -> Any: ...
-    def chdir(self, *args, **kwargs) -> Any: ...
-    def getcwd(self, *args, **kwargs) -> Any: ...
-    def __init__(self, block_dev) -> None: ...
+"""
+basic "operating system" services. See: https://docs.micropython.org/en/v1.20.0/library/os.html
+
+|see_cpython_module| :mod:`python:os` https://docs.python.org/3/library/os.html .
+
+The ``os`` module contains functions for filesystem access and mounting,
+terminal redirection and duplication, and the ``uname`` and ``urandom``
+functions.
+"""
+from typing import IO, Iterator, Optional, Tuple, Any
+from stdlib.os import uname_result
+
+def stat(path) -> Any:
+    """
+    Get the status of a file or directory.
+    """
+    ...
+
+def rmdir(path) -> None:
+    """
+    Remove a directory.
+    """
+    ...
+
+def rename(old_path, new_path) -> None:
+    """
+    Rename a file.
+    """
+    ...
+
+def mount(fsobj, mount_point, *, readonly) -> Any:
+    """
+    Mount the filesystem object *fsobj* at the location in the VFS given by the
+    *mount_point* string.  *fsobj* can be a a VFS object that has a ``mount()``
+    method, or a block device.  If it's a block device then the filesystem type
+    is automatically detected (an exception is raised if no filesystem was
+    recognised).  *mount_point* may be ``'/'`` to mount *fsobj* at the root,
+    or ``'/<name>'`` to mount it at a subdirectory under the root.
+
+    If *readonly* is ``True`` then the filesystem is mounted read-only.
+
+    During the mount process the method ``mount()`` is called on the filesystem
+    object.
+
+    Will raise ``OSError(EPERM)`` if *mount_point* is already mounted.
+    """
+    ...
+
+def urandom(n) -> bytes:
+    """
+    Return a bytes object with *n* random bytes. Whenever possible, it is
+    generated by the hardware random number generator.
+    """
+    ...
+
+def statvfs(path) -> Tuple:
+    """
+    Get the status of a fileystem.
+
+    Returns a tuple with the filesystem information in the following order:
+
+         * ``f_bsize`` -- file system block size
+         * ``f_frsize`` -- fragment size
+         * ``f_blocks`` -- size of fs in f_frsize units
+         * ``f_bfree`` -- number of free blocks
+         * ``f_bavail`` -- number of free blocks for unprivileged users
+         * ``f_files`` -- number of inodes
+         * ``f_ffree`` -- number of free inodes
+         * ``f_favail`` -- number of free inodes for unprivileged users
+         * ``f_flag`` -- mount flags
+         * ``f_namemax`` -- maximum filename length
+
+    Parameters related to inodes: ``f_files``, ``f_ffree``, ``f_avail``
+    and the ``f_flags`` parameter may return ``0`` as they can be unavailable
+    in a port-specific implementation.
+    """
+    ...
+
+def unlink(*args, **kwargs) -> Any: ...
+def uname() -> uname_result:
+    """
+    Return a tuple (possibly a named tuple) containing information about the
+    underlying machine and/or its operating system.  The tuple has five fields
+    in the following order, each of them being a string:
+
+         * ``sysname`` -- the name of the underlying system
+         * ``nodename`` -- the network name (can be the same as ``sysname``)
+         * ``release`` -- the version of the underlying system
+         * ``version`` -- the MicroPython version and build date
+         * ``machine`` -- an identifier for the underlying hardware (eg board, CPU)
+    """
+    ...
+
+def umount(mount_point) -> Any:
+    """
+    Unmount a filesystem. *mount_point* can be a string naming the mount location,
+    or a previously-mounted filesystem object.  During the unmount process the
+    method ``umount()`` is called on the filesystem object.
+
+    Will raise ``OSError(EINVAL)`` if *mount_point* is not found.
+    """
+    ...
+
+def chdir(path) -> Any:
+    """
+    Change current directory.
+    """
+    ...
+
+def dupterm(stream_object, index=0, /) -> IO:
+    """
+    Duplicate or switch the MicroPython terminal (the REPL) on the given `stream`-like
+    object. The *stream_object* argument must be a native stream object, or derive
+    from ``io.IOBase`` and implement the ``readinto()`` and
+    ``write()`` methods.  The stream should be in non-blocking mode and
+    ``readinto()`` should return ``None`` if there is no data available for reading.
+
+    After calling this function all terminal output is repeated on this stream,
+    and any input that is available on the stream is passed on to the terminal input.
+
+    The *index* parameter should be a non-negative integer and specifies which
+    duplication slot is set.  A given port may implement more than one slot (slot 0
+    will always be available) and in that case terminal input and output is
+    duplicated on all the slots that are set.
+
+    If ``None`` is passed as the *stream_object* then duplication is cancelled on
+    the slot given by *index*.
+
+    The function returns the previous stream-like object in the given slot.
+    """
+    ...
+
+def remove(path) -> None:
+    """
+    Remove a file.
+    """
+    ...
+
+def mkdir(path) -> Any:
+    """
+    Create a new directory.
+    """
+    ...
+
+def getcwd() -> Any:
+    """
+    Get the current directory.
+    """
+    ...
+
+def listdir(dir: Optional[Any] = None) -> Any:
+    """
+    With no argument, list the current directory.  Otherwise list the given directory.
+    """
+    ...
+
+def ilistdir(dir: Optional[Any] = None) -> Iterator[Tuple]:
+    """
+    This function returns an iterator which then yields tuples corresponding to
+    the entries in the directory that it is listing.  With no argument it lists the
+    current directory, otherwise it lists the directory given by *dir*.
+
+    The tuples have the form *(name, type, inode[, size])*:
+
+     - *name* is a string (or bytes if *dir* is a bytes object) and is the name of
+       the entry;
+     - *type* is an integer that specifies the type of the entry, with 0x4000 for
+       directories and 0x8000 for regular files;
+     - *inode* is an integer corresponding to the inode of the file, and may be 0
+       for filesystems that don't have such a notion.
+     - Some platforms may return a 4-tuple that includes the entry's *size*.  For
+       file entries, *size* is an integer representing the size of the file
+       or -1 if unknown.  Its meaning is currently undefined for directory
+       entries.
+    """
+    ...
+
+class VfsLfs2:
+    """
+    Create a filesystem object that uses the `littlefs v2 filesystem format`_.
+    Storage of the littlefs filesystem is provided by *block_dev*, which must
+    support the :ref:`extended interface <block-device-interface>`.
+    Objects created by this constructor can be mounted using :func:`mount`.
+
+    The *mtime* argument enables modification timestamps for files, stored using
+    littlefs attributes.  This option can be disabled or enabled differently each
+    mount time and timestamps will only be added or updated if *mtime* is enabled,
+    otherwise the timestamps will remain untouched.  Littlefs v2 filesystems without
+    timestamps will work without reformatting and timestamps will be added
+    transparently to existing files once they are opened for writing.  When *mtime*
+    is enabled `os.stat` on files without timestamps will return 0 for the timestamp.
+
+    See :ref:`filesystem` for more information.
+    """
+
+    def rename(self, *args, **kwargs) -> Any: ...
+    @staticmethod
+    def mkfs(block_dev, readsize=32, progsize=32, lookahead=32) -> None:
+        """
+            Build a Lfs2 filesystem on *block_dev*.
+
+        ``Note:`` There are reports of littlefs v2 failing in certain situations,
+                  for details see `littlefs issue 295`_.
+        """
+        ...
+    def mount(self, *args, **kwargs) -> Any: ...
+    def statvfs(self, *args, **kwargs) -> Any: ...
+    def rmdir(self, *args, **kwargs) -> Any: ...
+    def stat(self, *args, **kwargs) -> Any: ...
+    def umount(self, *args, **kwargs) -> Any: ...
+    def remove(self, *args, **kwargs) -> Any: ...
+    def mkdir(self, *args, **kwargs) -> Any: ...
+    def open(self, *args, **kwargs) -> Any: ...
+    def ilistdir(self, *args, **kwargs) -> Any: ...
+    def chdir(self, *args, **kwargs) -> Any: ...
+    def getcwd(self, *args, **kwargs) -> Any: ...
+    def __init__(self, block_dev, readsize=32, progsize=32, lookahead=32, mtime=True) -> None: ...
+
+class VfsFat:
+    """
+    Create a filesystem object that uses the FAT filesystem format.  Storage of
+    the FAT filesystem is provided by *block_dev*.
+    Objects created by this constructor can be mounted using :func:`mount`.
+    """
+
+    def rename(self, *args, **kwargs) -> Any: ...
+    @staticmethod
+    def mkfs(block_dev) -> None:
+        """
+        Build a FAT filesystem on *block_dev*.
+        """
+        ...
+    def mount(self, *args, **kwargs) -> Any: ...
+    def statvfs(self, *args, **kwargs) -> Any: ...
+    def rmdir(self, *args, **kwargs) -> Any: ...
+    def stat(self, *args, **kwargs) -> Any: ...
+    def umount(self, *args, **kwargs) -> Any: ...
+    def remove(self, *args, **kwargs) -> Any: ...
+    def mkdir(self, *args, **kwargs) -> Any: ...
+    def open(self, *args, **kwargs) -> Any: ...
+    def ilistdir(self, *args, **kwargs) -> Any: ...
+    def chdir(self, *args, **kwargs) -> Any: ...
+    def getcwd(self, *args, **kwargs) -> Any: ...
+    def __init__(self, block_dev) -> None: ...
```

### Comparing `micropython_rp2_stubs-1.19.1.post9/uselect.pyi` & `micropython_rp2_stubs-1.20.0.post1/uselect.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -1,93 +1,93 @@
-"""
-wait for events on a set of streams. See: https://docs.micropython.org/en/v1.19.1/library/select.html
-
-|see_cpython_module| :mod:`python:select` https://docs.python.org/3/library/select.html .
-
-This module provides functions to efficiently wait for events on multiple
-`streams <stream>` (select streams which are ready for operations).
-"""
-from typing import Iterator, List, Optional, Tuple, Any
-
-POLLOUT: int
-POLLIN: int
-POLLHUP: int
-POLLERR: int
-
-class select:
-    """
-    Wait for activity on a set of objects.
-
-    This function is provided by some MicroPython ports for compatibility
-    and is not efficient. Usage of :class:`Poll` is recommended instead.
-    """
-
-    def __init__(self, rlist, wlist, xlist, timeout: Optional[Any] = None) -> None: ...
-
-class poll:
-    """
-    Create an instance of the Poll class.
-    """
-
-    def __init__(self) -> None: ...
-    def register(self, obj, eventmask: Optional[Any] = None) -> None:
-        """
-        Register `stream` *obj* for polling. *eventmask* is logical OR of:
-
-        * ``select.POLLIN``  - data available for reading
-        * ``select.POLLOUT`` - more data can be written
-
-        Note that flags like ``select.POLLHUP`` and ``select.POLLERR`` are
-        *not* valid as input eventmask (these are unsolicited events which
-        will be returned from `poll()` regardless of whether they are asked
-        for). This semantics is per POSIX.
-
-        *eventmask* defaults to ``select.POLLIN | select.POLLOUT``.
-
-        It is OK to call this function multiple times for the same *obj*.
-        Successive calls will update *obj*'s eventmask to the value of
-        *eventmask* (i.e. will behave as `modify()`).
-        """
-        ...
-    def unregister(self, obj) -> Any:
-        """
-        Unregister *obj* from polling.
-        """
-        ...
-    def modify(self, obj, eventmask) -> None:
-        """
-        Modify the *eventmask* for *obj*. If *obj* is not registered, `OSError`
-        is raised with error of ENOENT.
-        """
-        ...
-    def poll(self, timeout=-1, /) -> List:
-        """
-        Wait for at least one of the registered objects to become ready or have an
-        exceptional condition, with optional timeout in milliseconds (if *timeout*
-        arg is not specified or -1, there is no timeout).
-
-        Returns list of (``obj``, ``event``, ...) tuples. There may be other elements in
-        tuple, depending on a platform and version, so don't assume that its size is 2.
-        The ``event`` element specifies which events happened with a stream and
-        is a combination of ``select.POLL*`` constants described above. Note that
-        flags ``select.POLLHUP`` and ``select.POLLERR`` can be returned at any time
-        (even if were not asked for), and must be acted on accordingly (the
-        corresponding stream unregistered from poll and likely closed), because
-        otherwise all further invocations of `poll()` may return immediately with
-        these flags set for this stream again.
-
-        In case of timeout, an empty list is returned.
-        """
-        ...
-    def ipoll(self, timeout=-1, flags=0, /) -> Iterator[Tuple]:
-        """
-        Like :meth:`poll.poll`, but instead returns an iterator which yields a
-        `callee-owned tuple`. This function provides an efficient, allocation-free
-        way to poll on streams.
-
-        If *flags* is 1, one-shot behaviour for events is employed: streams for
-        which events happened will have their event masks automatically reset
-        (equivalent to ``poll.modify(obj, 0)``), so new events for such a stream
-        won't be processed until new mask is set with `poll.modify()`. This
-        behaviour is useful for asynchronous I/O schedulers.
-        """
-        ...
+"""
+wait for events on a set of streams. See: https://docs.micropython.org/en/v1.20.0/library/select.html
+
+|see_cpython_module| :mod:`python:select` https://docs.python.org/3/library/select.html .
+
+This module provides functions to efficiently wait for events on multiple
+`streams <stream>` (select streams which are ready for operations).
+"""
+from typing import Iterator, List, Optional, Tuple, Any
+
+POLLOUT: int
+POLLIN: int
+POLLHUP: int
+POLLERR: int
+
+class select:
+    """
+    Wait for activity on a set of objects.
+
+    This function is provided by some MicroPython ports for compatibility
+    and is not efficient. Usage of :class:`Poll` is recommended instead.
+    """
+
+    def __init__(self, rlist, wlist, xlist, timeout: Optional[Any] = None) -> None: ...
+
+class poll:
+    """
+    Create an instance of the Poll class.
+    """
+
+    def __init__(self) -> None: ...
+    def register(self, obj, eventmask: Optional[Any] = None) -> None:
+        """
+        Register `stream` *obj* for polling. *eventmask* is logical OR of:
+
+        * ``select.POLLIN``  - data available for reading
+        * ``select.POLLOUT`` - more data can be written
+
+        Note that flags like ``select.POLLHUP`` and ``select.POLLERR`` are
+        *not* valid as input eventmask (these are unsolicited events which
+        will be returned from `poll()` regardless of whether they are asked
+        for). This semantics is per POSIX.
+
+        *eventmask* defaults to ``select.POLLIN | select.POLLOUT``.
+
+        It is OK to call this function multiple times for the same *obj*.
+        Successive calls will update *obj*'s eventmask to the value of
+        *eventmask* (i.e. will behave as `modify()`).
+        """
+        ...
+    def unregister(self, obj) -> Any:
+        """
+        Unregister *obj* from polling.
+        """
+        ...
+    def modify(self, obj, eventmask) -> None:
+        """
+        Modify the *eventmask* for *obj*. If *obj* is not registered, `OSError`
+        is raised with error of ENOENT.
+        """
+        ...
+    def poll(self, timeout=-1, /) -> List:
+        """
+        Wait for at least one of the registered objects to become ready or have an
+        exceptional condition, with optional timeout in milliseconds (if *timeout*
+        arg is not specified or -1, there is no timeout).
+
+        Returns list of (``obj``, ``event``, ...) tuples. There may be other elements in
+        tuple, depending on a platform and version, so don't assume that its size is 2.
+        The ``event`` element specifies which events happened with a stream and
+        is a combination of ``select.POLL*`` constants described above. Note that
+        flags ``select.POLLHUP`` and ``select.POLLERR`` can be returned at any time
+        (even if were not asked for), and must be acted on accordingly (the
+        corresponding stream unregistered from poll and likely closed), because
+        otherwise all further invocations of `poll()` may return immediately with
+        these flags set for this stream again.
+
+        In case of timeout, an empty list is returned.
+        """
+        ...
+    def ipoll(self, timeout=-1, flags=0, /) -> Iterator[Tuple]:
+        """
+        Like :meth:`poll.poll`, but instead returns an iterator which yields a
+        `callee-owned tuple`. This function provides an efficient, allocation-free
+        way to poll on streams.
+
+        If *flags* is 1, one-shot behaviour for events is employed: streams for
+        which events happened will have their event masks automatically reset
+        (equivalent to ``poll.modify(obj, 0)``), so new events for such a stream
+        won't be processed until new mask is set with `poll.modify()`. This
+        behaviour is useful for asynchronous I/O schedulers.
+        """
+        ...
```

### Comparing `micropython_rp2_stubs-1.19.1.post9/usys.pyi` & `micropython_rp2_stubs-1.20.0.post1/usys.pyi`

 * *Files 22% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-"""
-system specific functions. See: https://docs.micropython.org/en/v1.19.1/library/sys.html
-
-|see_cpython_module| :mod:`python:sys` https://docs.python.org/3/library/sys.html .
-"""
-from typing import Dict, List, Tuple, Any
-
-platform: str
-version_info: tuple
-path: list
-version: str
-ps1: str
-ps2: str
-byteorder: str
-modules: dict
-argv: list
-implementation: tuple
-maxsize: int
-
-def print_exception(exc, file=stdout, /) -> None:
-    """
-    Print exception with a traceback to a file-like object *file* (or
-    `sys.stdout` by default).
-    """
-    ...
-
-def exit(retval=0, /) -> Any:
-    """
-    Terminate current program with a given exit code. Underlyingly, this
-    function raise as `SystemExit` exception. If an argument is given, its
-    value given as an argument to `SystemExit`.
-    """
-    ...
-
-stderr: Any
-stdout: Any
-stdin: Any
+"""
+system specific functions. See: https://docs.micropython.org/en/v1.20.0/library/sys.html
+
+|see_cpython_module| :mod:`python:sys` https://docs.python.org/3/library/sys.html .
+"""
+from typing import Dict, List, Tuple, Any
+
+platform: str
+version_info: tuple
+path: list
+version: str
+ps1: str
+ps2: str
+byteorder: str
+modules: dict
+argv: list
+implementation: tuple
+maxsize: int
+
+def print_exception(exc, file=stdout, /) -> None:
+    """
+    Print exception with a traceback to a file-like object *file* (or
+    `sys.stdout` by default).
+    """
+    ...
+
+def exit(retval=0, /) -> Any:
+    """
+    Terminate current program with a given exit code. Underlyingly, this
+    function raise as `SystemExit` exception. If an argument is given, its
+    value given as an argument to `SystemExit`.
+    """
+    ...
+
+stderr: Any
+stdout: Any
+stdin: Any
```

### Comparing `micropython_rp2_stubs-1.19.1.post9/utime.pyi` & `micropython_rp2_stubs-1.20.0.post1/utime.pyi`

 * *Files 22% similar despite different names*

```diff
@@ -1,278 +1,278 @@
-"""
-time related functions. See: https://docs.micropython.org/en/v1.19.1/library/time.html
-
-|see_cpython_module| :mod:`python:time` https://docs.python.org/3/library/time.html .
-
-The ``time`` module provides functions for getting the current time and date,
-measuring time intervals, and for delays.
-
-**Time Epoch**: Unix port uses standard for POSIX systems epoch of
-1970-01-01 00:00:00 UTC. However, embedded ports use epoch of
-2000-01-01 00:00:00 UTC.
-
-**Maintaining actual calendar date/time**: This requires a
-Real Time Clock (RTC). On systems with underlying OS (including some
-RTOS), an RTC may be implicit. Setting and maintaining actual calendar
-time is responsibility of OS/RTOS and is done outside of MicroPython,
-it just uses OS API to query date/time. On baremetal ports however
-system time depends on ``machine.RTC()`` object. The current calendar time
-may be set using ``machine.RTC().datetime(tuple)`` function, and maintained
-by following means:
-
-* By a backup battery (which may be an additional, optional component for
-  a particular board).
-* Using networked time protocol (requires setup by a port/user).
-* Set manually by a user on each power-up (many boards then maintain
-  RTC time across hard resets, though some may require setting it again
-  in such case).
-
-If actual calendar time is not maintained with a system/MicroPython RTC,
-functions below which require reference to current absolute time may
-behave not as expected.
-"""
-from typing import Optional, Tuple, Any
-
-def ticks_diff(ticks1, ticks2) -> int:
-    """
-    Measure ticks difference between values returned from `ticks_ms()`, `ticks_us()`,
-    or `ticks_cpu()` functions, as a signed value which may wrap around.
-
-    The argument order is the same as for subtraction
-    operator, ``ticks_diff(ticks1, ticks2)`` has the same meaning as ``ticks1 - ticks2``.
-    However, values returned by `ticks_ms()`, etc. functions may wrap around, so
-    directly using subtraction on them will produce incorrect result. That is why
-    `ticks_diff()` is needed, it implements modular (or more specifically, ring)
-    arithmetics to produce correct result even for wrap-around values (as long as they not
-    too distant inbetween, see below). The function returns **signed** value in the range
-    [*-TICKS_PERIOD/2* .. *TICKS_PERIOD/2-1*] (that's a typical range definition for
-    two's-complement signed binary integers). If the result is negative, it means that
-    *ticks1* occurred earlier in time than *ticks2*. Otherwise, it means that
-    *ticks1* occurred after *ticks2*. This holds **only** if *ticks1* and *ticks2*
-    are apart from each other for no more than *TICKS_PERIOD/2-1* ticks. If that does
-    not hold, incorrect result will be returned. Specifically, if two tick values are
-    apart for *TICKS_PERIOD/2-1* ticks, that value will be returned by the function.
-    However, if *TICKS_PERIOD/2* of real-time ticks has passed between them, the
-    function will return *-TICKS_PERIOD/2* instead, i.e. result value will wrap around
-    to the negative range of possible values.
-
-    Informal rationale of the constraints above: Suppose you are locked in a room with no
-    means to monitor passing of time except a standard 12-notch clock. Then if you look at
-    dial-plate now, and don't look again for another 13 hours (e.g., if you fall for a
-    long sleep), then once you finally look again, it may seem to you that only 1 hour
-    has passed. To avoid this mistake, just look at the clock regularly. Your application
-    should do the same. "Too long sleep" metaphor also maps directly to application
-    behaviour: don't let your application run any single task for too long. Run tasks
-    in steps, and do time-keeping inbetween.
-
-    `ticks_diff()` is designed to accommodate various usage patterns, among them:
-
-    * Polling with timeout. In this case, the order of events is known, and you will deal
-      only with positive results of `ticks_diff()`::
-
-         # Wait for GPIO pin to be asserted, but at most 500us
-         start = time.ticks_us()
-         while pin.value() == 0:
-             if time.ticks_diff(time.ticks_us(), start) > 500:
-                 raise TimeoutError
-
-    * Scheduling events. In this case, `ticks_diff()` result may be negative
-      if an event is overdue::
-
-         # This code snippet is not optimized
-         now = time.ticks_ms()
-         scheduled_time = task.scheduled_time()
-         if ticks_diff(scheduled_time, now) > 0:
-             print("Too early, let's nap")
-             sleep_ms(ticks_diff(scheduled_time, now))
-             task.run()
-         elif ticks_diff(scheduled_time, now) == 0:
-             print("Right at time!")
-             task.run()
-         elif ticks_diff(scheduled_time, now) < 0:
-             print("Oops, running late, tell task to run faster!")
-             task.run(run_faster=true)
-
-    Note: Do not pass `time()` values to `ticks_diff()`, you should use
-    normal mathematical operations on them. But note that `time()` may (and will)
-    also overflow. This is known as https://en.wikipedia.org/wiki/Year_2038_problem .
-
-    """
-    ...
-
-def ticks_add(ticks, delta) -> Any:
-    """
-    Offset ticks value by a given number, which can be either positive or negative.
-    Given a *ticks* value, this function allows to calculate ticks value *delta*
-    ticks before or after it, following modular-arithmetic definition of tick values
-    (see `ticks_ms()` above). *ticks* parameter must be a direct result of call
-    to `ticks_ms()`, `ticks_us()`, or `ticks_cpu()` functions (or from previous
-    call to `ticks_add()`). However, *delta* can be an arbitrary integer number
-    or numeric expression. `ticks_add()` is useful for calculating deadlines for
-    events/tasks. (Note: you must use `ticks_diff()` function to work with
-    deadlines.)
-
-    Examples::
-
-         # Find out what ticks value there was 100ms ago
-         print(ticks_add(time.ticks_ms(), -100))
-
-         # Calculate deadline for operation and test for it
-         deadline = ticks_add(time.ticks_ms(), 200)
-         while ticks_diff(deadline, time.ticks_ms()) > 0:
-             do_a_little_of_something()
-
-         # Find out TICKS_MAX used by this port
-         print(ticks_add(0, -1))
-
-    """
-    ...
-
-def ticks_cpu() -> Any:
-    """
-    Similar to `ticks_ms()` and `ticks_us()`, but with the highest possible resolution
-    in the system. This is usually CPU clocks, and that's why the function is named that
-    way. But it doesn't have to be a CPU clock, some other timing source available in a
-    system (e.g. high-resolution timer) can be used instead. The exact timing unit
-    (resolution) of this function is not specified on ``time`` module level, but
-    documentation for a specific port may provide more specific information. This
-    function is intended for very fine benchmarking or very tight real-time loops.
-    Avoid using it in portable code.
-
-    Availability: Not every port implements this function.
-
-    """
-    ...
-
-class time:
-    """
-    Returns the number of seconds, as an integer, since the Epoch, assuming that
-    underlying RTC is set and maintained as described above. If an RTC is not set, this
-    function returns number of seconds since a port-specific reference point in time (for
-    embedded boards without a battery-backed RTC, usually since power up or reset). If you
-    want to develop portable MicroPython application, you should not rely on this function
-    to provide higher than second precision.  If you need higher precision, absolute
-    timestamps, use `time_ns()`.  If relative times are acceptable then use the
-    `ticks_ms()` and `ticks_us()` functions.  If you need calendar time, `gmtime()` or
-    `localtime()` without an argument is a better choice.
-    """
-
-    def __init__(self) -> None: ...
-
-def ticks_ms() -> int:
-    """
-    Returns an increasing millisecond counter with an arbitrary reference point, that
-    wraps around after some value.
-
-    The wrap-around value is not explicitly exposed, but we will
-    refer to it as *TICKS_MAX* to simplify discussion. Period of the values is
-    *TICKS_PERIOD = TICKS_MAX + 1*. *TICKS_PERIOD* is guaranteed to be a power of
-    two, but otherwise may differ from port to port. The same period value is used
-    for all of `ticks_ms()`, `ticks_us()`, `ticks_cpu()` functions (for
-    simplicity). Thus, these functions will return a value in range [*0* ..
-    *TICKS_MAX*], inclusive, total *TICKS_PERIOD* values. Note that only
-    non-negative values are used. For the most part, you should treat values returned
-    by these functions as opaque. The only operations available for them are
-    `ticks_diff()` and `ticks_add()` functions described below.
-
-    Note: Performing standard mathematical operations (+, -) or relational
-    operators (<, <=, >, >=) directly on these value will lead to invalid
-    result. Performing mathematical operations and then passing their results
-    as arguments to `ticks_diff()` or `ticks_add()` will also lead to
-    invalid results from the latter functions.
-    """
-    ...
-
-def ticks_us() -> Any:
-    """
-    Just like `ticks_ms()` above, but in microseconds.
-    """
-    ...
-
-def time_ns() -> int:
-    """
-    Similar to `time()` but returns nanoseconds since the Epoch, as an integer (usually
-    a big integer, so will allocate on the heap).
-    """
-    ...
-
-def localtime(secs: Optional[Any] = None) -> Tuple:
-    """
-    Convert the time *secs* expressed in seconds since the Epoch (see above) into an
-    8-tuple which contains: ``(year, month, mday, hour, minute, second, weekday, yearday)``
-    If *secs* is not provided or None, then the current time from the RTC is used.
-
-    The `gmtime()` function returns a date-time tuple in UTC, and `localtime()` returns a
-    date-time tuple in local time.
-
-    The format of the entries in the 8-tuple are:
-
-    * year includes the century (for example 2014).
-    * month   is 1-12
-    * mday    is 1-31
-    * hour    is 0-23
-    * minute  is 0-59
-    * second  is 0-59
-    * weekday is 0-6 for Mon-Sun
-    * yearday is 1-366
-    """
-    ...
-
-def sleep_us(us) -> None:
-    """
-    Delay for given number of microseconds, should be positive or 0.
-
-    This function attempts to provide an accurate delay of at least *us*
-    microseconds, but it may take longer if the system has other higher priority
-    processing to perform.
-    """
-    ...
-
-def gmtime(secs: Optional[Any] = None) -> Tuple:
-    """
-    Convert the time *secs* expressed in seconds since the Epoch (see above) into an
-    8-tuple which contains: ``(year, month, mday, hour, minute, second, weekday, yearday)``
-    If *secs* is not provided or None, then the current time from the RTC is used.
-
-    The `gmtime()` function returns a date-time tuple in UTC, and `localtime()` returns a
-    date-time tuple in local time.
-
-    The format of the entries in the 8-tuple are:
-
-    * year includes the century (for example 2014).
-    * month   is 1-12
-    * mday    is 1-31
-    * hour    is 0-23
-    * minute  is 0-59
-    * second  is 0-59
-    * weekday is 0-6 for Mon-Sun
-    * yearday is 1-366
-    """
-    ...
-
-def sleep_ms(ms) -> None:
-    """
-    Delay for given number of milliseconds, should be positive or 0.
-
-    This function will delay for at least the given number of milliseconds, but
-    may take longer than that if other processing must take place, for example
-    interrupt handlers or other threads.  Passing in 0 for *ms* will still allow
-    this other processing to occur.  Use `sleep_us()` for more precise delays.
-    """
-    ...
-
-def mktime() -> int:
-    """
-    This is inverse function of localtime. It's argument is a full 8-tuple
-    which expresses a time as per localtime. It returns an integer which is
-    the number of seconds since Jan 1, 2000.
-    """
-    ...
-
-def sleep(seconds) -> Any:
-    """
-    Sleep for the given number of seconds. Some boards may accept *seconds* as a
-    floating-point number to sleep for a fractional number of seconds. Note that
-    other boards may not accept a floating-point argument, for compatibility with
-    them use `sleep_ms()` and `sleep_us()` functions.
-    """
-    ...
+"""
+time related functions. See: https://docs.micropython.org/en/v1.20.0/library/time.html
+
+|see_cpython_module| :mod:`python:time` https://docs.python.org/3/library/time.html .
+
+The ``time`` module provides functions for getting the current time and date,
+measuring time intervals, and for delays.
+
+**Time Epoch**: Unix port uses standard for POSIX systems epoch of
+1970-01-01 00:00:00 UTC. However, some embedded ports use epoch of
+2000-01-01 00:00:00 UTC. Epoch year may be determined with ``gmtime(0)[0]``.
+
+**Maintaining actual calendar date/time**: This requires a
+Real Time Clock (RTC). On systems with underlying OS (including some
+RTOS), an RTC may be implicit. Setting and maintaining actual calendar
+time is responsibility of OS/RTOS and is done outside of MicroPython,
+it just uses OS API to query date/time. On baremetal ports however
+system time depends on ``machine.RTC()`` object. The current calendar time
+may be set using ``machine.RTC().datetime(tuple)`` function, and maintained
+by following means:
+
+* By a backup battery (which may be an additional, optional component for
+  a particular board).
+* Using networked time protocol (requires setup by a port/user).
+* Set manually by a user on each power-up (many boards then maintain
+  RTC time across hard resets, though some may require setting it again
+  in such case).
+
+If actual calendar time is not maintained with a system/MicroPython RTC,
+functions below which require reference to current absolute time may
+behave not as expected.
+"""
+from typing import Optional, Tuple, Any
+
+def ticks_diff(ticks1, ticks2) -> int:
+    """
+    Measure ticks difference between values returned from `ticks_ms()`, `ticks_us()`,
+    or `ticks_cpu()` functions, as a signed value which may wrap around.
+
+    The argument order is the same as for subtraction
+    operator, ``ticks_diff(ticks1, ticks2)`` has the same meaning as ``ticks1 - ticks2``.
+    However, values returned by `ticks_ms()`, etc. functions may wrap around, so
+    directly using subtraction on them will produce incorrect result. That is why
+    `ticks_diff()` is needed, it implements modular (or more specifically, ring)
+    arithmetics to produce correct result even for wrap-around values (as long as they not
+    too distant inbetween, see below). The function returns **signed** value in the range
+    [*-TICKS_PERIOD/2* .. *TICKS_PERIOD/2-1*] (that's a typical range definition for
+    two's-complement signed binary integers). If the result is negative, it means that
+    *ticks1* occurred earlier in time than *ticks2*. Otherwise, it means that
+    *ticks1* occurred after *ticks2*. This holds **only** if *ticks1* and *ticks2*
+    are apart from each other for no more than *TICKS_PERIOD/2-1* ticks. If that does
+    not hold, incorrect result will be returned. Specifically, if two tick values are
+    apart for *TICKS_PERIOD/2-1* ticks, that value will be returned by the function.
+    However, if *TICKS_PERIOD/2* of real-time ticks has passed between them, the
+    function will return *-TICKS_PERIOD/2* instead, i.e. result value will wrap around
+    to the negative range of possible values.
+
+    Informal rationale of the constraints above: Suppose you are locked in a room with no
+    means to monitor passing of time except a standard 12-notch clock. Then if you look at
+    dial-plate now, and don't look again for another 13 hours (e.g., if you fall for a
+    long sleep), then once you finally look again, it may seem to you that only 1 hour
+    has passed. To avoid this mistake, just look at the clock regularly. Your application
+    should do the same. "Too long sleep" metaphor also maps directly to application
+    behaviour: don't let your application run any single task for too long. Run tasks
+    in steps, and do time-keeping inbetween.
+
+    `ticks_diff()` is designed to accommodate various usage patterns, among them:
+
+    * Polling with timeout. In this case, the order of events is known, and you will deal
+      only with positive results of `ticks_diff()`::
+
+         # Wait for GPIO pin to be asserted, but at most 500us
+         start = time.ticks_us()
+         while pin.value() == 0:
+             if time.ticks_diff(time.ticks_us(), start) > 500:
+                 raise TimeoutError
+
+    * Scheduling events. In this case, `ticks_diff()` result may be negative
+      if an event is overdue::
+
+         # This code snippet is not optimized
+         now = time.ticks_ms()
+         scheduled_time = task.scheduled_time()
+         if ticks_diff(scheduled_time, now) > 0:
+             print("Too early, let's nap")
+             sleep_ms(ticks_diff(scheduled_time, now))
+             task.run()
+         elif ticks_diff(scheduled_time, now) == 0:
+             print("Right at time!")
+             task.run()
+         elif ticks_diff(scheduled_time, now) < 0:
+             print("Oops, running late, tell task to run faster!")
+             task.run(run_faster=true)
+
+    Note: Do not pass `time()` values to `ticks_diff()`, you should use
+    normal mathematical operations on them. But note that `time()` may (and will)
+    also overflow. This is known as https://en.wikipedia.org/wiki/Year_2038_problem .
+
+    """
+    ...
+
+def ticks_add(ticks, delta) -> Any:
+    """
+    Offset ticks value by a given number, which can be either positive or negative.
+    Given a *ticks* value, this function allows to calculate ticks value *delta*
+    ticks before or after it, following modular-arithmetic definition of tick values
+    (see `ticks_ms()` above). *ticks* parameter must be a direct result of call
+    to `ticks_ms()`, `ticks_us()`, or `ticks_cpu()` functions (or from previous
+    call to `ticks_add()`). However, *delta* can be an arbitrary integer number
+    or numeric expression. `ticks_add()` is useful for calculating deadlines for
+    events/tasks. (Note: you must use `ticks_diff()` function to work with
+    deadlines.)
+
+    Examples::
+
+         # Find out what ticks value there was 100ms ago
+         print(ticks_add(time.ticks_ms(), -100))
+
+         # Calculate deadline for operation and test for it
+         deadline = ticks_add(time.ticks_ms(), 200)
+         while ticks_diff(deadline, time.ticks_ms()) > 0:
+             do_a_little_of_something()
+
+         # Find out TICKS_MAX used by this port
+         print(ticks_add(0, -1))
+
+    """
+    ...
+
+def ticks_cpu() -> Any:
+    """
+    Similar to `ticks_ms()` and `ticks_us()`, but with the highest possible resolution
+    in the system. This is usually CPU clocks, and that's why the function is named that
+    way. But it doesn't have to be a CPU clock, some other timing source available in a
+    system (e.g. high-resolution timer) can be used instead. The exact timing unit
+    (resolution) of this function is not specified on ``time`` module level, but
+    documentation for a specific port may provide more specific information. This
+    function is intended for very fine benchmarking or very tight real-time loops.
+    Avoid using it in portable code.
+
+    Availability: Not every port implements this function.
+
+    """
+    ...
+
+class time:
+    """
+    Returns the number of seconds, as an integer, since the Epoch, assuming that
+    underlying RTC is set and maintained as described above. If an RTC is not set, this
+    function returns number of seconds since a port-specific reference point in time (for
+    embedded boards without a battery-backed RTC, usually since power up or reset). If you
+    want to develop portable MicroPython application, you should not rely on this function
+    to provide higher than second precision.  If you need higher precision, absolute
+    timestamps, use `time_ns()`.  If relative times are acceptable then use the
+    `ticks_ms()` and `ticks_us()` functions.  If you need calendar time, `gmtime()` or
+    `localtime()` without an argument is a better choice.
+    """
+
+    def __init__(self) -> None: ...
+
+def ticks_ms() -> int:
+    """
+    Returns an increasing millisecond counter with an arbitrary reference point, that
+    wraps around after some value.
+
+    The wrap-around value is not explicitly exposed, but we will
+    refer to it as *TICKS_MAX* to simplify discussion. Period of the values is
+    *TICKS_PERIOD = TICKS_MAX + 1*. *TICKS_PERIOD* is guaranteed to be a power of
+    two, but otherwise may differ from port to port. The same period value is used
+    for all of `ticks_ms()`, `ticks_us()`, `ticks_cpu()` functions (for
+    simplicity). Thus, these functions will return a value in range [*0* ..
+    *TICKS_MAX*], inclusive, total *TICKS_PERIOD* values. Note that only
+    non-negative values are used. For the most part, you should treat values returned
+    by these functions as opaque. The only operations available for them are
+    `ticks_diff()` and `ticks_add()` functions described below.
+
+    Note: Performing standard mathematical operations (+, -) or relational
+    operators (<, <=, >, >=) directly on these value will lead to invalid
+    result. Performing mathematical operations and then passing their results
+    as arguments to `ticks_diff()` or `ticks_add()` will also lead to
+    invalid results from the latter functions.
+    """
+    ...
+
+def ticks_us() -> Any:
+    """
+    Just like `ticks_ms()` above, but in microseconds.
+    """
+    ...
+
+def time_ns() -> int:
+    """
+    Similar to `time()` but returns nanoseconds since the Epoch, as an integer (usually
+    a big integer, so will allocate on the heap).
+    """
+    ...
+
+def localtime(secs: Optional[Any] = None) -> Tuple:
+    """
+    Convert the time *secs* expressed in seconds since the Epoch (see above) into an
+    8-tuple which contains: ``(year, month, mday, hour, minute, second, weekday, yearday)``
+    If *secs* is not provided or None, then the current time from the RTC is used.
+
+    The `gmtime()` function returns a date-time tuple in UTC, and `localtime()` returns a
+    date-time tuple in local time.
+
+    The format of the entries in the 8-tuple are:
+
+    * year includes the century (for example 2014).
+    * month   is 1-12
+    * mday    is 1-31
+    * hour    is 0-23
+    * minute  is 0-59
+    * second  is 0-59
+    * weekday is 0-6 for Mon-Sun
+    * yearday is 1-366
+    """
+    ...
+
+def sleep_us(us) -> None:
+    """
+    Delay for given number of microseconds, should be positive or 0.
+
+    This function attempts to provide an accurate delay of at least *us*
+    microseconds, but it may take longer if the system has other higher priority
+    processing to perform.
+    """
+    ...
+
+def gmtime(secs: Optional[Any] = None) -> Tuple:
+    """
+    Convert the time *secs* expressed in seconds since the Epoch (see above) into an
+    8-tuple which contains: ``(year, month, mday, hour, minute, second, weekday, yearday)``
+    If *secs* is not provided or None, then the current time from the RTC is used.
+
+    The `gmtime()` function returns a date-time tuple in UTC, and `localtime()` returns a
+    date-time tuple in local time.
+
+    The format of the entries in the 8-tuple are:
+
+    * year includes the century (for example 2014).
+    * month   is 1-12
+    * mday    is 1-31
+    * hour    is 0-23
+    * minute  is 0-59
+    * second  is 0-59
+    * weekday is 0-6 for Mon-Sun
+    * yearday is 1-366
+    """
+    ...
+
+def sleep_ms(ms) -> None:
+    """
+    Delay for given number of milliseconds, should be positive or 0.
+
+    This function will delay for at least the given number of milliseconds, but
+    may take longer than that if other processing must take place, for example
+    interrupt handlers or other threads.  Passing in 0 for *ms* will still allow
+    this other processing to occur.  Use `sleep_us()` for more precise delays.
+    """
+    ...
+
+def mktime() -> int:
+    """
+    This is inverse function of localtime. It's argument is a full 8-tuple
+    which expresses a time as per localtime. It returns an integer which is
+    the number of seconds since Jan 1, 2000.
+    """
+    ...
+
+def sleep(seconds) -> Any:
+    """
+    Sleep for the given number of seconds. Some boards may accept *seconds* as a
+    floating-point number to sleep for a fractional number of seconds. Note that
+    other boards may not accept a floating-point argument, for compatibility with
+    them use `sleep_ms()` and `sleep_us()` functions.
+    """
+    ...
```

### Comparing `micropython_rp2_stubs-1.19.1.post9/uzlib.pyi` & `micropython_rp2_stubs-1.20.0.post1/uzlib.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-"""
-zlib decompression. See: https://docs.micropython.org/en/v1.19.1/library/zlib.html
-
-|see_cpython_module| :mod:`python:zlib` https://docs.python.org/3/library/zlib.html .
-
-This module allows to decompress binary data compressed with
-`DEFLATE algorithm <https://en.wikipedia.org/wiki/DEFLATE>`_
-(commonly used in zlib library and gzip archiver). Compression
-is not yet implemented.
-"""
-from typing import IO, Any
-
-def decompress(data, wbits=0, bufsize=0, /) -> bytes:
-    """
-    Return decompressed *data* as bytes. *wbits* is DEFLATE dictionary window
-    size used during compression (8-15, the dictionary size is power of 2 of
-    that value). Additionally, if value is positive, *data* is assumed to be
-    zlib stream (with zlib header). Otherwise, if it's negative, it's assumed
-    to be raw DEFLATE stream. *bufsize* parameter is for compatibility with
-    CPython and is ignored.
-    """
-    ...
-
-class DecompIO:
-    """
-    Create a `stream` wrapper which allows transparent decompression of
-    compressed data in another *stream*. This allows to process compressed
-    streams with data larger than available heap size. In addition to
-    values described in :func:`decompress`, *wbits* may take values
-    24..31 (16 + 8..15), meaning that input stream has gzip header.
-    """
-
-    def readinto(self, *args, **kwargs) -> Any: ...
-    def readline(self, *args, **kwargs) -> Any: ...
-    def read(self, *args, **kwargs) -> Any: ...
-    def __init__(self, stream, wbits=0, /) -> None: ...
+"""
+zlib decompression. See: https://docs.micropython.org/en/v1.20.0/library/zlib.html
+
+|see_cpython_module| :mod:`python:zlib` https://docs.python.org/3/library/zlib.html .
+
+This module allows to decompress binary data compressed with
+`DEFLATE algorithm <https://en.wikipedia.org/wiki/DEFLATE>`_
+(commonly used in zlib library and gzip archiver). Compression
+is not yet implemented.
+"""
+from typing import Any
+
+def decompress(data, wbits=0, bufsize=0, /) -> bytes:
+    """
+    Return decompressed *data* as bytes. *wbits* is DEFLATE dictionary window
+    size used during compression (8-15, the dictionary size is power of 2 of
+    that value). Additionally, if value is positive, *data* is assumed to be
+    zlib stream (with zlib header). Otherwise, if it's negative, it's assumed
+    to be raw DEFLATE stream. *bufsize* parameter is for compatibility with
+    CPython and is ignored.
+    """
+    ...
+
+class DecompIO:
+    """
+    Create a `stream` wrapper which allows transparent decompression of
+    compressed data in another *stream*. This allows to process compressed
+    streams with data larger than available heap size. In addition to
+    values described in :func:`decompress`, *wbits* may take values
+    24..31 (16 + 8..15), meaning that input stream has gzip header.
+    """
+
+    def readinto(self, *args, **kwargs) -> Any: ...
+    def readline(self, *args, **kwargs) -> Any: ...
+    def read(self, *args, **kwargs) -> Any: ...
+    def __init__(self, stream, wbits=0, /) -> None: ...
```

### Comparing `micropython_rp2_stubs-1.19.1.post9/zlib.pyi` & `micropython_rp2_stubs-1.20.0.post1/zlib.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-"""
-zlib decompression. See: https://docs.micropython.org/en/v1.19.1/library/zlib.html
-
-|see_cpython_module| :mod:`python:zlib` https://docs.python.org/3/library/zlib.html .
-
-This module allows to decompress binary data compressed with
-`DEFLATE algorithm <https://en.wikipedia.org/wiki/DEFLATE>`_
-(commonly used in zlib library and gzip archiver). Compression
-is not yet implemented.
-"""
-from typing import IO, Any
-
-def decompress(data, wbits=0, bufsize=0, /) -> bytes:
-    """
-    Return decompressed *data* as bytes. *wbits* is DEFLATE dictionary window
-    size used during compression (8-15, the dictionary size is power of 2 of
-    that value). Additionally, if value is positive, *data* is assumed to be
-    zlib stream (with zlib header). Otherwise, if it's negative, it's assumed
-    to be raw DEFLATE stream. *bufsize* parameter is for compatibility with
-    CPython and is ignored.
-    """
-    ...
-
-class DecompIO:
-    """
-    Create a `stream` wrapper which allows transparent decompression of
-    compressed data in another *stream*. This allows to process compressed
-    streams with data larger than available heap size. In addition to
-    values described in :func:`decompress`, *wbits* may take values
-    24..31 (16 + 8..15), meaning that input stream has gzip header.
-    """
-
-    def readinto(self, *args, **kwargs) -> Any: ...
-    def readline(self, *args, **kwargs) -> Any: ...
-    def read(self, *args, **kwargs) -> Any: ...
-    def __init__(self, stream, wbits=0, /) -> None: ...
+"""
+zlib decompression. See: https://docs.micropython.org/en/v1.20.0/library/zlib.html
+
+|see_cpython_module| :mod:`python:zlib` https://docs.python.org/3/library/zlib.html .
+
+This module allows to decompress binary data compressed with
+`DEFLATE algorithm <https://en.wikipedia.org/wiki/DEFLATE>`_
+(commonly used in zlib library and gzip archiver). Compression
+is not yet implemented.
+"""
+from typing import Any
+
+def decompress(data, wbits=0, bufsize=0, /) -> bytes:
+    """
+    Return decompressed *data* as bytes. *wbits* is DEFLATE dictionary window
+    size used during compression (8-15, the dictionary size is power of 2 of
+    that value). Additionally, if value is positive, *data* is assumed to be
+    zlib stream (with zlib header). Otherwise, if it's negative, it's assumed
+    to be raw DEFLATE stream. *bufsize* parameter is for compatibility with
+    CPython and is ignored.
+    """
+    ...
+
+class DecompIO:
+    """
+    Create a `stream` wrapper which allows transparent decompression of
+    compressed data in another *stream*. This allows to process compressed
+    streams with data larger than available heap size. In addition to
+    values described in :func:`decompress`, *wbits* may take values
+    24..31 (16 + 8..15), meaning that input stream has gzip header.
+    """
+
+    def readinto(self, *args, **kwargs) -> Any: ...
+    def readline(self, *args, **kwargs) -> Any: ...
+    def read(self, *args, **kwargs) -> Any: ...
+    def __init__(self, stream, wbits=0, /) -> None: ...
```

### Comparing `micropython_rp2_stubs-1.19.1.post9/setup.py` & `micropython_rp2_stubs-1.20.0.post1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,86 +4,76 @@
 modules = \
 ['_boot',
  '_boot_fat',
  '_onewire',
  '_rp2',
  '_thread',
  '_uasyncio',
- '__init__',
- 'central',
- 'client',
- 'core',
- 'device',
- 'l2cap',
- 'peripheral',
- 'server',
  'array',
  'binascii',
  'cmath',
+ 'collections',
+ 'cryptolib',
  'dht',
  'ds18x20',
  'errno',
  'framebuf',
  'gc',
  'hashlib',
  'heapq',
+ 'io',
  'json',
- 'lsm6dsox',
+ 'logging',
  'machine',
  'math',
  'micropython',
  'neopixel',
- 'network',
  'onewire',
  'os',
  'random',
  'rp2',
  'select',
- 'socket',
  'struct',
  'sys',
  'time',
  'uarray',
+ '__init__',
+ 'core',
  'event',
  'funcs',
  'lock',
  'stream',
  'task',
  'ubinascii',
- 'ubluetooth',
  'ucollections',
  'ucryptolib',
  'uctypes',
  'uerrno',
  'uhashlib',
  'uheapq',
  'uio',
  'ujson',
  'umachine',
  'uos',
  'urandom',
  'ure',
  'uselect',
- 'usocket',
  'ustruct',
  'usys',
  'utime',
- 'uwebsocket',
  'uzlib',
- 'websocket',
- 'websocket_helper',
  'zlib']
 install_requires = \
 ['micropython-stdlib-stubs>=0.9.0']
 
 setup_kwargs = {
     'name': 'micropython-rp2-stubs',
-    'version': '1.19.1.post9',
+    'version': '1.20.0.post1',
     'description': 'MicroPython stubs',
-    'long_description': '# micropython-rp2-stubs\n\n\nThis is a stub-only package for MicroPython.\nIt is intended to be installed in a projects virtual environment to allow static type checkers and intellisense features to be used while writing Micropython code.\n\nThe version of this package is alligned the the version of the MicroPython firmware.\n - Major, Minor and Patch levels are alligned to the same version as the firmware.  \n - The post release level is used to publish new releases of the stubs.\n\nFor `Micropython 1.17` the stubs are published as `1.17.post1` ... `1.17.post2`  \nfor `Micropython 1.18` the stubs are published as `1.18.post1` ... `1.18.post2`  \n\nTo install the latest stubs:  \n`pip install -I  micropython-<port>-stubs` where port is the port of the MicroPython firmware.\n\nTo install the stubs for an older version, such as MicroPython 1.17:  \n`pip install micropython-stm32-stubs==1.17.*` which will install the last post release of the stubs for MicroPython 1.17.\n\n\nAs the creation of the stubs, and merging of the different types is still going though improvements, the stub packages are marked as Beta.\nTo upgrade stubs to the latest stubs for a specific version use `pip install micropython-stm32-stubs==1.17.* --upgrade`\n\nIf you have suggestions or find any issues with the stubs, please report them in the [MicroPython-stubs Discussions](https://github.com/Josverl/micropython-stubs/discussions)\n\nFor an overview of  Micropython Stubs please see: https://micropython-stubs.readthedocs.io/en/main/ \n * List of all stubs : https://micropython-stubs.readthedocs.io/en/main/firmware_grp.html\n\nIncluded stubs:\n* Merged stubs from `stubs/micropython-v1_19_1-rp2-merged`\n* Frozen stubs from `stubs/micropython-v1_19_1-frozen/rp2/GENERIC`\n* Core stubs from `stubs/cpython_core-pycopy`\n\n\norigin | Family | Port | Board | Version\n-------|--------|------|-------|--------\nFirmware | micropython | rp2 | Arduino Nano RP2040 Connect with RP2040 | v1.19.1 \nDocumentation | micropython | - | - | v1.19.1 \nCore | micropython | rp2 | - | v1.19.1 \n',
+    'long_description': '# micropython-rp2-stubs\n\n\nThis is a stub-only package for MicroPython.\nIt is intended to be installed in a projects virtual environment to allow static type checkers and intellisense features to be used while writing Micropython code.\n\nThe version of this package is alligned the the version of the MicroPython firmware.\n - Major, Minor and Patch levels are alligned to the same version as the firmware.  \n - The post release level is used to publish new releases of the stubs.\n\nFor `Micropython 1.17` the stubs are published as `1.17.post1` ... `1.17.post2`  \nfor `Micropython 1.18` the stubs are published as `1.18.post1` ... `1.18.post2`  \n\nTo install the latest stubs:  \n`pip install -I  micropython-<port>-stubs` where port is the port of the MicroPython firmware.\n\nTo install the stubs for an older version, such as MicroPython 1.17:  \n`pip install micropython-stm32-stubs==1.17.*` which will install the last post release of the stubs for MicroPython 1.17.\n\n\nAs the creation of the stubs, and merging of the different types is still going though improvements, the stub packages are marked as Beta.\nTo upgrade stubs to the latest stubs for a specific version use `pip install micropython-stm32-stubs==1.17.* --upgrade`\n\nIf you have suggestions or find any issues with the stubs, please report them in the [MicroPython-stubs Discussions](https://github.com/Josverl/micropython-stubs/discussions)\n\nFor an overview of  Micropython Stubs please see: https://micropython-stubs.readthedocs.io/en/main/ \n * List of all stubs : https://micropython-stubs.readthedocs.io/en/main/firmware_grp.html\n\nIncluded stubs:\n* StubSource.MERGED from `stubs/micropython-v1_20_0-rp2-merged`\n* StubSource.FROZEN from `stubs/micropython-v1_20_0-frozen/rp2/GENERIC`\n* StubSource.CORE from `stubs/micropython-core`\n\n\norigin | Family | Port | Board | Version\n-------|--------|------|-------|--------\nDocumentation | micropython | - | - | v1.20.0 \nCore | micropython | rp2 | - | v1.20.0 \n',
     'author': 'josverl',
     'author_email': 'josverl@users.noreply.github.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/josverl/micropython-stubs#micropython-stubs',
     'py_modules': modules,
     'install_requires': install_requires,
```

### Comparing `micropython_rp2_stubs-1.19.1.post9/PKG-INFO` & `micropython_rp2_stubs-1.20.0.post1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micropython-rp2-stubs
-Version: 1.19.1.post9
+Version: 1.20.0.post1
 Summary: MicroPython stubs
 Home-page: https://github.com/josverl/micropython-stubs#micropython-stubs
 License: MIT
 Author: josverl
 Author-email: josverl@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -52,18 +52,17 @@
 
 If you have suggestions or find any issues with the stubs, please report them in the [MicroPython-stubs Discussions](https://github.com/Josverl/micropython-stubs/discussions)
 
 For an overview of  Micropython Stubs please see: https://micropython-stubs.readthedocs.io/en/main/ 
  * List of all stubs : https://micropython-stubs.readthedocs.io/en/main/firmware_grp.html
 
 Included stubs:
-* Merged stubs from `stubs/micropython-v1_19_1-rp2-merged`
-* Frozen stubs from `stubs/micropython-v1_19_1-frozen/rp2/GENERIC`
-* Core stubs from `stubs/cpython_core-pycopy`
+* StubSource.MERGED from `stubs/micropython-v1_20_0-rp2-merged`
+* StubSource.FROZEN from `stubs/micropython-v1_20_0-frozen/rp2/GENERIC`
+* StubSource.CORE from `stubs/micropython-core`
 
 
 origin | Family | Port | Board | Version
 -------|--------|------|-------|--------
-Firmware | micropython | rp2 | Arduino Nano RP2040 Connect with RP2040 | v1.19.1 
-Documentation | micropython | - | - | v1.19.1 
-Core | micropython | rp2 | - | v1.19.1 
+Documentation | micropython | - | - | v1.20.0 
+Core | micropython | rp2 | - | v1.20.0
```

