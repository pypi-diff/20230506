# Comparing `tmp/fixa-0.4.1.tar.gz` & `tmp/fixa-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fixa-0.4.1.tar", last modified: Sat Feb 25 16:51:32 2023, max compression
+gzip compressed data, was "fixa-0.5.1.tar", last modified: Sat May  6 03:38:02 2023, max compression
```

## Comparing `fixa-0.4.1.tar` & `fixa-0.5.1.tar`

### file list

```diff
@@ -1,30 +1,51 @@
-drwxr-xr-x   0 sanhehu    (505) staff       (20)        0 2023-02-25 16:51:32.224871 fixa-0.4.1/
--rw-r--r--   0 sanhehu    (505) staff       (20)      509 2023-02-04 06:58:32.000000 fixa-0.4.1/AUTHORS.rst
--rw-r--r--   0 sanhehu    (505) staff       (20)     1114 2023-02-04 06:58:32.000000 fixa-0.4.1/LICENSE.txt
--rw-r--r--   0 sanhehu    (505) staff       (20)      312 2023-02-04 06:58:32.000000 fixa-0.4.1/MANIFEST.in
--rw-r--r--   0 sanhehu    (505) staff       (20)     4095 2023-02-25 16:51:32.224664 fixa-0.4.1/PKG-INFO
--rw-r--r--   0 sanhehu    (505) staff       (20)     2986 2023-02-25 16:51:20.000000 fixa-0.4.1/README.rst
-drwxr-xr-x   0 sanhehu    (505) staff       (20)        0 2023-02-25 16:51:32.223090 fixa-0.4.1/fixa/
--rw-r--r--   0 sanhehu    (505) staff       (20)      317 2023-02-04 08:38:19.000000 fixa-0.4.1/fixa/__init__.py
--rw-r--r--   0 sanhehu    (505) staff       (20)       93 2023-02-25 16:47:53.000000 fixa-0.4.1/fixa/_version.py
--rw-r--r--   0 sanhehu    (505) staff       (20)     6675 2023-02-04 07:55:59.000000 fixa-0.4.1/fixa/binarysearch.py
-drwxr-xr-x   0 sanhehu    (505) staff       (20)        0 2023-02-25 16:51:32.224340 fixa-0.4.1/fixa/docs/
--rw-r--r--   0 sanhehu    (505) staff       (20)       43 2023-02-04 06:58:32.000000 fixa-0.4.1/fixa/docs/__init__.py
--rw-r--r--   0 sanhehu    (505) staff       (20)     5877 2023-02-25 16:28:35.000000 fixa-0.4.1/fixa/hashes.py
--rw-r--r--   0 sanhehu    (505) staff       (20)    12244 2023-02-04 08:21:48.000000 fixa-0.4.1/fixa/iterable.py
--rw-r--r--   0 sanhehu    (505) staff       (20)    15555 2023-02-25 16:15:11.000000 fixa-0.4.1/fixa/nest_logger.py
--rw-r--r--   0 sanhehu    (505) staff       (20)     3112 2023-02-04 08:54:02.000000 fixa-0.4.1/fixa/rnd.py
--rw-r--r--   0 sanhehu    (505) staff       (20)     4757 2023-02-25 16:36:33.000000 fixa-0.4.1/fixa/timer.py
-drwxr-xr-x   0 sanhehu    (505) staff       (20)        0 2023-02-25 16:51:32.224181 fixa-0.4.1/fixa.egg-info/
--rw-r--r--   0 sanhehu    (505) staff       (20)     4095 2023-02-25 16:51:32.000000 fixa-0.4.1/fixa.egg-info/PKG-INFO
--rw-r--r--   0 sanhehu    (505) staff       (20)      450 2023-02-25 16:51:32.000000 fixa-0.4.1/fixa.egg-info/SOURCES.txt
--rw-r--r--   0 sanhehu    (505) staff       (20)        1 2023-02-25 16:51:32.000000 fixa-0.4.1/fixa.egg-info/dependency_links.txt
--rw-r--r--   0 sanhehu    (505) staff       (20)      171 2023-02-25 16:51:32.000000 fixa-0.4.1/fixa.egg-info/requires.txt
--rw-r--r--   0 sanhehu    (505) staff       (20)        5 2023-02-25 16:51:32.000000 fixa-0.4.1/fixa.egg-info/top_level.txt
--rw-r--r--   0 sanhehu    (505) staff       (20)     1466 2023-02-25 16:47:46.000000 fixa-0.4.1/release-history.rst
--rw-r--r--   0 sanhehu    (505) staff       (20)      295 2023-02-06 03:46:34.000000 fixa-0.4.1/requirements-dev.txt
--rw-r--r--   0 sanhehu    (505) staff       (20)      621 2023-02-04 06:58:32.000000 fixa-0.4.1/requirements-doc.txt
--rw-r--r--   0 sanhehu    (505) staff       (20)      183 2023-02-04 06:58:32.000000 fixa-0.4.1/requirements-test.txt
--rw-r--r--   0 sanhehu    (505) staff       (20)        0 2023-02-04 06:58:32.000000 fixa-0.4.1/requirements.txt
--rw-r--r--   0 sanhehu    (505) staff       (20)       38 2023-02-25 16:51:32.224950 fixa-0.4.1/setup.cfg
--rw-r--r--   0 sanhehu    (505) staff       (20)     7699 2023-02-04 06:58:32.000000 fixa-0.4.1/setup.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-06 03:38:02.808993 fixa-0.5.1/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      509 2023-05-06 00:03:13.000000 fixa-0.5.1/AUTHORS.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1114 2023-05-06 00:03:13.000000 fixa-0.5.1/LICENSE.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      312 2023-05-06 00:03:13.000000 fixa-0.5.1/MANIFEST.in
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4095 2023-05-06 03:38:02.808829 fixa-0.5.1/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2986 2023-05-06 00:03:13.000000 fixa-0.5.1/README.rst
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-06 03:38:02.804586 fixa-0.5.1/fixa/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      317 2023-05-06 00:03:13.000000 fixa-0.5.1/fixa/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-05-06 03:25:53.000000 fixa-0.5.1/fixa/_version.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4273 2023-05-06 03:16:26.000000 fixa-0.5.1/fixa/better_enum.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      533 2023-05-06 03:13:06.000000 fixa-0.5.1/fixa/better_pathlib.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     6675 2023-05-06 00:03:13.000000 fixa-0.5.1/fixa/binarysearch.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1333 2023-05-06 03:12:23.000000 fixa-0.5.1/fixa/dataclass_dataframe.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-06 03:38:02.805281 fixa-0.5.1/fixa/docs/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-05-06 00:03:13.000000 fixa-0.5.1/fixa/docs/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2383 2023-05-06 03:09:12.000000 fixa-0.5.1/fixa/git_cli.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     5877 2023-05-06 00:03:13.000000 fixa-0.5.1/fixa/hashes.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)    12219 2023-05-06 01:55:53.000000 fixa-0.5.1/fixa/iterable.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)    15702 2023-05-06 03:32:05.000000 fixa-0.5.1/fixa/nest_logger.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      469 2023-05-06 03:18:07.000000 fixa-0.5.1/fixa/os_platform.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3572 2023-05-06 03:24:32.000000 fixa-0.5.1/fixa/pytest_cov_helper.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3145 2023-05-06 01:57:52.000000 fixa-0.5.1/fixa/rnd.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1933 2023-05-06 03:17:46.000000 fixa-0.5.1/fixa/runtime.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-06 03:38:02.805531 fixa-0.5.1/fixa/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      539 2023-05-06 01:41:58.000000 fixa-0.5.1/fixa/tests/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4757 2023-05-06 00:03:13.000000 fixa-0.5.1/fixa/timer.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-06 03:38:02.805169 fixa-0.5.1/fixa.egg-info/
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4095 2023-05-06 03:38:02.000000 fixa-0.5.1/fixa.egg-info/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)      889 2023-05-06 03:38:02.000000 fixa-0.5.1/fixa.egg-info/SOURCES.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-05-06 03:38:02.000000 fixa-0.5.1/fixa.egg-info/dependency_links.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      171 2023-05-06 03:38:02.000000 fixa-0.5.1/fixa.egg-info/requires.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)        5 2023-05-06 03:38:02.000000 fixa-0.5.1/fixa.egg-info/top_level.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1814 2023-05-06 03:36:57.000000 fixa-0.5.1/release-history.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)      295 2023-05-06 00:03:13.000000 fixa-0.5.1/requirements-dev.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      621 2023-05-06 00:03:13.000000 fixa-0.5.1/requirements-doc.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      183 2023-05-06 00:03:13.000000 fixa-0.5.1/requirements-test.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)        0 2023-05-06 00:03:13.000000 fixa-0.5.1/requirements.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-05-06 03:38:02.809045 fixa-0.5.1/setup.cfg
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7699 2023-05-06 00:03:13.000000 fixa-0.5.1/setup.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-06 03:38:02.808483 fixa-0.5.1/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3615 2023-05-06 02:40:34.000000 fixa-0.5.1/tests/test_better_enum.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      663 2023-05-06 02:16:38.000000 fixa-0.5.1/tests/test_better_pathlib.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1633 2023-05-06 01:48:18.000000 fixa-0.5.1/tests/test_binarysearch.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      692 2023-05-06 01:42:50.000000 fixa-0.5.1/tests/test_dataclass_dataframe.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      740 2023-05-06 03:08:57.000000 fixa-0.5.1/tests/test_git_cli.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2178 2023-05-06 01:48:41.000000 fixa-0.5.1/tests/test_hashes.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      214 2023-05-06 01:48:59.000000 fixa-0.5.1/tests/test_import.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     6529 2023-05-06 01:56:07.000000 fixa-0.5.1/tests/test_iterable.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3581 2023-05-06 03:36:08.000000 fixa-0.5.1/tests/test_nest_logger.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      661 2023-05-06 01:58:16.000000 fixa-0.5.1/tests/test_rnd.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3432 2023-05-06 02:03:21.000000 fixa-0.5.1/tests/test_timer.py
```

### Comparing `fixa-0.4.1/LICENSE.txt` & `fixa-0.5.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fixa-0.4.1/PKG-INFO` & `fixa-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: fixa
-Version: 0.4.1
+Version: 0.5.1
 Summary: Like the Ikea FIXA, it is my toolbox to fix things.
 Home-page: https://github.com/MacHu-GWU/fixa-project
-Download-URL: https://pypi.python.org/pypi/fixa/0.4.1#downloads
+Download-URL: https://pypi.python.org/pypi/fixa/0.5.1#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Unknown
 License: MIT
 Platform: Windows
 Platform: MacOS
 Platform: Unix
```

### Comparing `fixa-0.4.1/README.rst` & `fixa-0.5.1/README.rst`

 * *Files identical despite different names*

### Comparing `fixa-0.4.1/fixa/binarysearch.py` & `fixa-0.5.1/fixa/binarysearch.py`

 * *Files identical despite different names*

### Comparing `fixa-0.4.1/fixa/hashes.py` & `fixa-0.5.1/fixa/hashes.py`

 * *Files identical despite different names*

### Comparing `fixa-0.4.1/fixa/iterable.py` & `fixa-0.5.1/fixa/iterable.py`

 * *Files 3% similar despite different names*

```diff
@@ -227,15 +227,15 @@
     fifo = collections.deque(maxlen=size)
     for i in lst:
         fifo.append(i)
         if len(fifo) == size:
             yield list(fifo)
 
 
-def cycle_running_window(iterable, size):
+def cycle_running_window(lst: list, size: int) -> list:
     """
     Generate n-size cycle running window.
 
     Example::
 
         >>> for i in cycle_running_window([1, 2, 3, 4, 5], size=3):
         ...     print(i)
@@ -245,45 +245,43 @@
         [4, 5, 1]
         [5, 1, 2]
 
     **中文文档**
 
     循环位移滑窗函数.
     """
-    if size > len(iterable):
+    if size > len(lst):
         raise ValueError("size can not be greater than length of iterable.")
 
     fifo = collections.deque(maxlen=size)
-    cycle = itertools.cycle(iterable)
+    cycle = itertools.cycle(lst)
     counter = itertools.count(1)
-    length = len(iterable)
+    length = len(lst)
     for i in cycle:
         fifo.append(i)
         if len(fifo) == size:
             yield list(fifo)
             if next(counter) == length:
                 break
 
 
 # --- Cycle ---
-def cycle_slice(sliceable: list, start: int, end: int):
+def cycle_slice(sliceable: list, start: int, end: int) -> list:
     """
     Given a list, return the right-hand cycle direction slice from start to end.
 
     Example::
 
         >>> array = [0, 1, 2, 3]
         >>> cycle_slice(array, 1, 3) # from array[1] to array[3]
         [1, 2]
 
         >>> cycle_slice(array, 3, 1) # from array[3] to array[1]
         [3, 0]
     """
-    if type(sliceable) != list:
-        sliceable = list(sliceable)
     length = len(sliceable)
 
     if length == 0:
         raise ValueError("sliceable cannot be empty!")
     start = start % length
     end = end % length
 
@@ -325,15 +323,15 @@
     dist = abs(x - y) % perimeter
     if dist > 0.5 * perimeter:
         dist = perimeter - dist
     return dist
 
 
 # --- Shift ---
-def cyclic_shift(array: list, shift: int):
+def cyclic_shift(array: list, shift: int) -> list:
     """
 
     :params array: list like iterable object
     :params shift: number of movement
 
     Example::
 
@@ -347,15 +345,15 @@
 
     循环位移函数.
     """
     shift = shift % len(array)
     return array[-shift:] + array[:-shift]
 
 
-def shift_and_trim(array: list, shift: int):
+def shift_and_trim(array: list, shift: int) -> list:
     """
     Shift and trim unneeded item.
 
     :params array: list like iterable object
     :params shift: number of movement
 
     Example::
@@ -387,15 +385,15 @@
         return array[-shift:]
     elif shift > 0:
         return array[:-shift]
     else:
         return list(array)
 
 
-def shift_and_pad(array: list, shift: int, pad="__null__"):
+def shift_and_pad(array: list, shift: int, pad: T.Any = "__null__") -> list:
     """
     Shift and pad with item.
 
     :params array: list like iterable object
     :params shift: number of movement
     :params pad: any value
 
@@ -449,16 +447,16 @@
         return (
             array[-shift:]
             + [
                 padding_item,
             ]
             * -shift
         )
-    else:  # Never get in this logic
-        raise Exception
+    else:  # pragma: no cover
+        raise NotImplementedError
 
 
 def size_of_generator(generator: T.Iterable, memory_efficient=True) -> int:
     """Get number of items in a generator function.
 
     - memory_efficient = True, 3 times slower, but memory_efficient.
     - memory_efficient = False, faster, but cost more memory.
```

### Comparing `fixa-0.4.1/fixa/nest_logger.py` & `fixa-0.5.1/fixa/nest_logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,26 +54,29 @@
     formatter = logging.Formatter(
         fmt=log_format,
         datefmt=datetime_format,
     )
     stream_handler.setFormatter(formatter)
 
     logger.addHandler(stream_handler)
+
+    logger.parent = None  # disable handler from parent logger, only use stream handler
+
     return logger
 
 
 tab = " " * 2
 
 
 def encode_pipe(pipe: str) -> str:
     if len(pipe) == 1:
         return pipe + " "
     elif len(pipe) == 2 and pipe[1] == " ":
         return pipe
-    else:
+    else: # pragma: no cover
         raise ValueError
 
 
 DEFAULT_PIPE = encode_pipe("| ")
 
 
 def format_line(
@@ -197,15 +200,15 @@
         if logger is None:
             self._logger = create_logger(
                 name=name,
                 level=level,
                 log_format=log_format,
                 datetime_format=datetime_format,
             )
-        else:
+        else: # pragma: no cover
             self._logger = logger
 
         # ``_nest`` stores the current level of nesting
         self._nest = 0
         # ``_pipes`` is a first in last out stack data structure that stores
         # the list of pipe character for different level of nesting
         self._pipes = [
@@ -330,15 +333,15 @@
         self,
         pipe: T.Optional[str] = None,
     ):
         self._nest += 1
 
         if pipe is None:
             self._pipes.append(DEFAULT_PIPE)
-        else:
+        else: # pragma: no cover
             self._pipes.append(encode_pipe(pipe))
 
     def _nested_end(self):
         self._nest -= 1
         self._pipes.pop()
 
     @contextlib.contextmanager
```

### Comparing `fixa-0.4.1/fixa/rnd.py` & `fixa-0.5.1/fixa/rnd.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,14 +87,15 @@
 
         >>> rand_pwd(12)
         TlhM$^jzculH
     """
     if length < 8:
         raise ValueError("minimal password length is 8!")
 
+    # first letter always letter
     first = random.choice(CHARSET_PASSWORD_LOWER + CHARSET_PASSWORD_UPPER)
     chars = [
         random.choice(CHARSET_PASSWORD_LOWER),
         random.choice(CHARSET_PASSWORD_UPPER),
         random.choice(CHARSET_PASSWORD_DIGITS),
     ]
     if special_char:
```

### Comparing `fixa-0.4.1/fixa/timer.py` & `fixa-0.5.1/fixa/timer.py`

 * *Files identical despite different names*

### Comparing `fixa-0.4.1/fixa.egg-info/PKG-INFO` & `fixa-0.5.1/fixa.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: fixa
-Version: 0.4.1
+Version: 0.5.1
 Summary: Like the Ikea FIXA, it is my toolbox to fix things.
 Home-page: https://github.com/MacHu-GWU/fixa-project
-Download-URL: https://pypi.python.org/pypi/fixa/0.4.1#downloads
+Download-URL: https://pypi.python.org/pypi/fixa/0.5.1#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Unknown
 License: MIT
 Platform: Windows
 Platform: MacOS
 Platform: Unix
```

### Comparing `fixa-0.4.1/release-history.rst` & `fixa-0.5.1/release-history.rst`

 * *Files 26% similar despite different names*

```diff
@@ -11,14 +11,31 @@
 **Minor Improvements**
 
 **Bugfixes**
 
 **Miscellaneous**
 
 
+0.5.1 (2023-05-05)
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+**Features and Improvements**
+
+- add ``better_pathlib``
+- add ``dataclass_dataframe``
+- add ``pytest_cov_helper``
+- add ``better_enum``
+- add ``runtime``
+- add ``os_platform``
+- add ``git_cli``
+
+**Minor Improvements**
+
+- improve code coverage test
+
+
 0.4.1 (2023-02-25)
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 **Features and Improvements**
 
 - add ``nested_logger.block``
 
 **Miscellaneous**
```

### Comparing `fixa-0.4.1/requirements-doc.txt` & `fixa-0.5.1/requirements-doc.txt`

 * *Files identical despite different names*

### Comparing `fixa-0.4.1/setup.py` & `fixa-0.5.1/setup.py`

 * *Files identical despite different names*

