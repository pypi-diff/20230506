# Comparing `tmp/savestate-0.1.0.tar.gz` & `tmp/savestate-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "savestate-0.1.0.tar", max compression
+gzip compressed data, was "savestate-0.1.1.tar", max compression
```

## Comparing `savestate-0.1.0.tar` & `savestate-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0     1069 2022-02-05 00:36:04.438125 savestate-0.1.0/LICENSE
--rw-r--r--   0        0        0     4099 2022-02-05 00:36:04.438125 savestate-0.1.0/README.md
--rw-r--r--   0        0        0     2559 2022-02-05 00:36:04.438125 savestate-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      138 2022-02-05 00:36:04.438125 savestate-0.1.0/savestate/__init__.py
--rw-r--r--   0        0        0    29074 2022-02-05 00:36:04.438125 savestate-0.1.0/savestate/savestate.py
--rw-r--r--   0        0        0     4686 2022-02-05 00:36:42.901828 savestate-0.1.0/setup.py
--rw-r--r--   0        0        0     4914 2022-02-05 00:36:42.902313 savestate-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-06 17:07:07.610102 savestate-0.1.1/LICENSE
+-rw-r--r--   0        0        0     4035 2023-05-06 17:07:07.610102 savestate-0.1.1/README.md
+-rw-r--r--   0        0        0     2442 2023-05-06 17:07:07.610102 savestate-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      224 2023-05-06 17:07:07.610102 savestate-0.1.1/savestate/__init__.py
+-rw-r--r--   0        0        0    29384 2023-05-06 17:07:07.610102 savestate-0.1.1/savestate/savestate.py
+-rw-r--r--   0        0        0     5180 1970-01-01 00:00:00.000000 savestate-0.1.1/PKG-INFO
```

### Comparing `savestate-0.1.0/LICENSE` & `savestate-0.1.1/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2021 Matti Lamppu
+Copyright (c) 2023 Matti Lamppu
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `savestate-0.1.0/README.md` & `savestate-0.1.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,79 +1,79 @@
-# SaveState
-
-[![Coverage Status][coverage-badge]][coverage]
-[![GitHub Workflow Status][status-badge]][status]
-[![PyPI][pypi-badge]][pypi]
-[![GitHub][licence-badge]][licence]
-[![GitHub Last Commit][repo-badge]][repo]
-[![GitHub Issues][issues-badge]][issues]
-[![Python Version][version-badge]][pypi]
-
-```shell
-pip install savestate
-```
-
----
-
-**Documentation**: [https://mrthearman.github.io/savestate/](https://mrthearman.github.io/savestate/)
-
-**Source Code**: [https://github.com/MrThearMan/savestate/](https://github.com/MrThearMan/savestate/)
-
----
-
-SaveState is a cross-platform fast file storage for arbitrary python objects. 
-It's similar to python's builtin [shelve][shelve] module, but aims to be more
-performant on Windows while being cross-platform compatible.
-
-Savestate is inspired by [semidbm2][semidbm2], with a more modern interface.
-mapping-like functions, a context manager, and support for 
-arbitrary python objects.
-
-### Implementation details:
-- Pure python
-- No requirements or dependencies
-- A dict-like interface (no unions)
-- Same, single file on Windows and Linux (unlike shelve)
-- Key and value integrity can be evaluated with a checksum, which will detect data corruption on key access.
-- Recovery from missing bytes at the end of the file, or small amounts of corrupted data in the middle
-- Both values AND keys put in savestate must support [pickling][pickling].
-Note the [security implications][security] of this!
-  - This means that you can use arbitrary objects as keys if they support pickle (unlike shelve)
-- All the keys of the savestate are kept in memory, which limits the savestate size (not a problem for most applications)
-- NOT Thread safe, so cannot be accessed by multiple processes
-- File is append-only, so the more non-read operations you do, the more the file size is going to balloon
-  - However, you can *compact* the savestate, usually on *savestate.close()*, which will replace the savestate with a new file with only the current non-deleted data.
-  This will impact performance a little, but not by much
-  
-### Performance:
-- About 50-60% of the performance of shelve with [gdbm][gdbm] (linux), 
-  but >5000% compared to shelve with [dumbdbm][dumbdbm] (windows) (>20000% for deletes!)
-  - Performance is more favorable with large keys and values when compared to gdbm, 
-    but gdbm is still faster on subsequent reads/writes thanks to its caching
-- A dbm-mode for about double the speed of regular mode, but only string-type keys and values
-  - This is about 25-30% of the performance of gdbm on its own.
-  - Note: Values will be returned in bytes form!
-  
-> Source code includes a benchmark that you can run to get more accurate performance on your specific machine.
-
-
-[shelve]: https://docs.python.org/3/library/shelve.html
-[semidbm2]: https://github.com/quora/semidbm2
-[pickling]: https://docs.python.org/3/library/pickle.html#module-pickle
-[security]: https://docs.python.org/3/library/pickle.html#module-pickle
-[gdbm]: https://docs.python.org/3/library/dbm.html#module-dbm.gnu
-[dumbdbm]: https://docs.python.org/3/library/dbm.html#module-dbm.dumb
-
-[coverage-badge]: https://coveralls.io/repos/github/MrThearMan/savestate/badge.svg?branch=main
-[status-badge]: https://img.shields.io/github/workflow/status/MrThearMan/savestate/Tests
-[pypi-badge]: https://img.shields.io/pypi/v/savestate
-[licence-badge]: https://img.shields.io/github/license/MrThearMan/savestate
-[repo-badge]: https://img.shields.io/github/last-commit/MrThearMan/savestate
-[issues-badge]: https://img.shields.io/github/issues-raw/MrThearMan/savestate
-[version-badge]: https://img.shields.io/pypi/pyversions/savestate
-
-[coverage]: https://coveralls.io/github/MrThearMan/savestate?branch=main
-[status]: https://github.com/MrThearMan/savestate/actions/workflows/main.yml
-[pypi]: https://pypi.org/project/savestate
-[licence]: https://github.com/MrThearMan/savestate/blob/main/LICENSE
-[repo]: https://github.com/MrThearMan/savestate/commits/main
-[issues]: https://github.com/MrThearMan/savestate/issues
+# SaveState
+
+[![Coverage Status][coverage-badge]][coverage]
+[![GitHub Workflow Status][status-badge]][status]
+[![PyPI][pypi-badge]][pypi]
+[![GitHub][licence-badge]][licence]
+[![GitHub Last Commit][repo-badge]][repo]
+[![GitHub Issues][issues-badge]][issues]
+[![Python Version][version-badge]][pypi]
+
+```shell
+pip install savestate
+```
+
+---
+
+**Documentation**: [https://mrthearman.github.io/savestate/](https://mrthearman.github.io/savestate/)
+
+**Source Code**: [https://github.com/MrThearMan/savestate/](https://github.com/MrThearMan/savestate/)
+
+---
+
+SaveState is a cross-platform fast file storage for arbitrary python objects.
+It's similar to python's builtin [shelve][shelve] module, but aims to be more
+performant on Windows while being cross-platform compatible.
+
+Savestate is inspired by [semidbm2][semidbm2], with a more modern interface.
+mapping-like functions, a context manager, and support for
+arbitrary python objects.
+
+### Implementation details:
+- Pure python
+- No requirements or dependencies
+- A dict-like interface (no unions)
+- Same, single file on Windows and Linux (unlike shelve)
+- Key and value integrity can be evaluated with a checksum, which will detect data corruption on key access.
+- Recovery from missing bytes at the end of the file, or small amounts of corrupted data in the middle
+- Both values AND keys put in savestate must support [pickling][pickling].
+Note the [security implications][security] of this!
+  - This means that you can use arbitrary objects as keys if they support pickle (unlike shelve)
+- All the keys of the savestate are kept in memory, which limits the savestate size (not a problem for most applications)
+- NOT Thread safe, so cannot be accessed by multiple processes
+- File is append-only, so the more non-read operations you do, the more the file size is going to balloon
+  - However, you can *compact* the savestate, usually on *savestate.close()*, which will replace the savestate with a new file with only the current non-deleted data.
+  This will impact performance a little, but not by much
+
+### Performance:
+- About 50-60% of the performance of shelve with [gdbm][gdbm] (linux),
+  but >5000% compared to shelve with [dumbdbm][dumbdbm] (windows) (>20000% for deletes!)
+  - Performance is more favorable with large keys and values when compared to gdbm,
+    but gdbm is still faster on subsequent reads/writes thanks to its caching
+- A dbm-mode for about double the speed of regular mode, but only string-type keys and values
+  - This is about 25-30% of the performance of gdbm on its own.
+  - Note: Values will be returned in bytes form!
+
+> Source code includes a benchmark that you can run to get more accurate performance on your specific machine.
+
+
+[shelve]: https://docs.python.org/3/library/shelve.html
+[semidbm2]: https://github.com/quora/semidbm2
+[pickling]: https://docs.python.org/3/library/pickle.html#module-pickle
+[security]: https://docs.python.org/3/library/pickle.html#module-pickle
+[gdbm]: https://docs.python.org/3/library/dbm.html#module-dbm.gnu
+[dumbdbm]: https://docs.python.org/3/library/dbm.html#module-dbm.dumb
+
+[coverage-badge]: https://coveralls.io/repos/github/MrThearMan/savestate/badge.svg?branch=main
+[status-badge]: https://img.shields.io/github/actions/workflow/status/MrThearMan/savestate/test.yml?branch=main
+[pypi-badge]: https://img.shields.io/pypi/v/savestate
+[licence-badge]: https://img.shields.io/github/license/MrThearMan/savestate
+[repo-badge]: https://img.shields.io/github/last-commit/MrThearMan/savestate
+[issues-badge]: https://img.shields.io/github/issues-raw/MrThearMan/savestate
+[version-badge]: https://img.shields.io/pypi/pyversions/savestate
+
+[coverage]: https://coveralls.io/github/MrThearMan/savestate?branch=main
+[status]: https://github.com/MrThearMan/savestate/actions/workflows/test.yml
+[pypi]: https://pypi.org/project/savestate
+[licence]: https://github.com/MrThearMan/savestate/blob/main/LICENSE
+[repo]: https://github.com/MrThearMan/savestate/commits/main
+[issues]: https://github.com/MrThearMan/savestate/issues
```

### Comparing `savestate-0.1.0/savestate/savestate.py` & `savestate-0.1.1/savestate/savestate.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 r"""Persistent storage for arbitrary python objects inspired by SemiDBM and Shelve.
 
 Data structure and byte sizes are as follows:
 
 Header:⠀<file_identifier: 9 bytes> <file_format_version: 2 bytes> <pickle_version: 2 bytes>
-Data:⠀⠀⠀<keysize: 4 bytes> <valsize: 4 bytes> <key: 'keysize' bytes> <val: 'valsize' bytes> <checksum: 4 bytes>
-⠀⠀⠀⠀⠀⠀⠀⠀<keysize: 4 bytes> <valsize: 4 bytes> <key: 'keysize' bytes> <val: 'valsize' bytes> <checksum: 4 bytes>
+Data:⠀⠀⠀<key_size: 4 bytes> <val_size: 4 bytes> <key: 'key_size' bytes> <val: 'val_size' bytes> <checksum: 4 bytes>
+⠀⠀⠀⠀⠀⠀⠀⠀<key_size: 4 bytes> <key_size: 4 bytes> <key: 'key_size' bytes> <val: 'val_size' bytes> <checksum: 4 bytes>
 
 """
 
 import builtins
 import mmap
 import ntpath
 import os
@@ -31,16 +31,20 @@
     MutableMapping,
     Reversible,
     Tuple,
     Type,
     Union,
 )
 
-
-__all__ = ["open", "SaveStateError", "SaveStateLoadError", "SaveStateChecksumError"]
+__all__ = [
+    "open",
+    "SaveStateError",
+    "SaveStateLoadError",
+    "SaveStateChecksumError",
+]
 
 
 class SaveStateError(Exception):
     pass
 
 
 class SaveStateLoadError(SaveStateError):
@@ -60,15 +64,15 @@
     DATA_OPEN_FLAGS = os.O_RDWR | os.O_CREAT | os.O_APPEND | os.O_BINARY
     DATA_OPEN_FLAGS_READONLY = os.O_RDONLY | os.O_BINARY
 else:  # pragma: no cover
     DATA_OPEN_FLAGS = os.O_RDWR | os.O_CREAT | os.O_APPEND
     DATA_OPEN_FLAGS_READONLY = os.O_RDONLY
 
 DELETED: int = 0
-"""Signifies item has been deleated from the savestate."""
+"""Signifies item has been deleted from the savestate."""
 
 # Header Info
 FILE_IDENTIFIER: bytes = b"savestate"
 """Magic identifier for this file."""
 FILE_SUFFIX = f".{FILE_IDENTIFIER.decode()}"
 """File suffix"""
 FILE_FORMAT_VERSION: int = 1
@@ -106,15 +110,15 @@
 
         self._savestate_name = filename
         self._dbm_mode = dbm_mode
         self._data_flags = DATA_OPEN_FLAGS_READONLY
         self._verify_checksums = verify_checksums
 
         self._index: Dict[bytes, Tuple[int, int]] = self._load_index(self._savestate_name)
-        """The in memory index. Index 'key' is the name of the stored value in bytes and index 'value' is a Tuple 
+        """The in memory index. Index 'key' is the name of the stored value in bytes and index 'value' is a Tuple
         of the offset in bytes in the file to the stored value, and the size of the stored value in bytes."""
 
         self._data_file_descriptor: int = os.open(self._savestate_name, self._data_flags)
         self._current_offset: int = os.lseek(self._data_file_descriptor, 0, os.SEEK_END)
 
     def __getitem__(self, key: Any) -> Any:
         """Load value from the savestate.
@@ -236,42 +240,44 @@
             self._verify_header(header=f.read(HEADER_SIZE))
 
             offset: int = HEADER_SIZE
             missing_bytes: int = 0
             contents: bytes
             with mmap.mmap(fileno=f.fileno(), length=0, access=mmap.ACCESS_READ) as contents:
                 while True:
-
                     if offset >= len(contents):
                         break  # End of file, so stop reading values
 
                     try:
                         key_size, val_size = struct.unpack(
                             KEYVAL_IND_FORMAT, contents[offset : offset + KEYVAL_IND_SIZE]
                         )
                         if key_size == 0:
                             warnings.warn(
                                 f"Zero key size at position {offset}/{len(contents)}. "
                                 f"Could not continue to read data.",
                                 category=BytesWarning,
+                                stacklevel=2,
                             )
                             break
                     except struct.error:
                         warnings.warn(
                             f"Key and value size indicators could not be unpacked from file "
                             f"at position {offset}/{len(contents)}.",
                             category=BytesWarning,
+                            stacklevel=2,
                         )
                         break
 
                     missing_bytes = (offset + KEYVAL_IND_SIZE + key_size + val_size + CHECKSUM_SIZE) - len(contents)
                     if missing_bytes > 0:
                         warnings.warn(
-                            f"Some data is missing at the end of the file. Compaction necessary.",
+                            "Some data is missing at the end of the file. Compaction necessary.",
                             category=BytesWarning,
+                            stacklevel=2,
                         )
                         break
 
                     offset += KEYVAL_IND_SIZE
                     key = contents[offset : offset + key_size]
                     offset += key_size
 
@@ -281,19 +287,20 @@
                         )
                         yield key, offset, val_size
 
                     except SaveStateChecksumError:
                         warnings.warn(
                             f"Data was corrupted at position {offset}/{len(contents)}. Compaction necessary.",
                             category=BytesWarning,
+                            stacklevel=2,
                         )
 
                     offset += val_size + CHECKSUM_SIZE
 
-        # If file doesn't have enought bytes, fill with blank data to
+        # If file doesn't have enough bytes, fill with blank data to
         # recover from errors that would arise when writing more data to the file.
         if missing_bytes > 0:
             with builtins.open(filename, "ab+") as f:
                 f.write(b"\x00" * missing_bytes)
 
     def _load_index(self, filename: Path) -> Dict[bytes, Tuple[int, int]]:
         """This method is only used upon instantiation to populate the in memory index."""
@@ -316,15 +323,15 @@
 
     @staticmethod
     def _convert_to_bytes(value: Any) -> bytes:
         return pickle.dumps(value, protocol=PICKLE_PROTOCOL)
 
     @staticmethod
     def _convert_from_bytes(value: bytes) -> Any:
-        return pickle.loads(value)
+        return pickle.loads(value)  # noqa: S301
 
     @staticmethod
     def _verify_header(header: bytes):
         """Check file is correct type and compatible version.
 
         :raises SaveStateError: File was incorrect type or incompatible version.
         """
@@ -384,15 +391,15 @@
         self._savestate_name = filename
         self._dbm_mode = dbm_mode
         self._compact = compact
         self._data_flags = DATA_OPEN_FLAGS
         self._verify_checksums = verify_checksums
 
         self._index: Dict[bytes, Tuple[int, int]] = self._load_index(self._savestate_name)
-        """The in memory index. Index 'key' is the name of the stored value in bytes and index 'value' is a Tuple 
+        """The in memory index. Index 'key' is the name of the stored value in bytes and index 'value' is a Tuple
         of the offset in bytes in the file to the stored value, and the size of the stored value in bytes."""
 
         self._data_file_descriptor: int = os.open(self._savestate_name, self._data_flags)
         self._current_offset: int = os.lseek(self._data_file_descriptor, 0, os.SEEK_END)
 
     def __setitem__(self, key: Any, value: Any):
         """Save value in the savestate.
@@ -560,15 +567,15 @@
         value = self.pop(key)
         return key, value
 
     def copy(self, new_filename: Path) -> Union["_SaveStateCreate", "_SaveStateReadWrite", "_SaveStateNew"]:
         """Creates a copy of this savestate by writing all the keys from this savestate to the new savestate."""
 
         new_filename = _add_file_identifier(new_filename)
-        assert new_filename != self._savestate_name, "Copy can't have the same filename as the original."
+        assert new_filename != self._savestate_name, "Copy can't have the same filename as the original."  # noqa
 
         new_savestate = self.__class__(
             filename=new_filename,
             verify_checksums=self._verify_checksums,
             compact=self._compact,
         )
 
@@ -593,19 +600,19 @@
         :raises OSError: File can't be renamed. Possibly being used by another process.
         """
 
         if sys.platform.startswith("win"):  # pragma: no cover
             import ctypes
             from ctypes.wintypes import DWORD, LPVOID
 
-            lpctstr = ctypes.c_wchar_p
+            lpct_str = ctypes.c_wchar_p
             kernel32 = ctypes.windll.kernel32
-            kernel32.ReplaceFile.argtypes = [lpctstr, lpctstr, lpctstr, DWORD, LPVOID, LPVOID]
+            kernel32.ReplaceFile.argtypes = [lpct_str, lpct_str, lpct_str, DWORD, LPVOID, LPVOID]
 
-            rc = kernel32.ReplaceFile(lpctstr(str(to_file)), lpctstr(str(from_file)), None, 0, None, None)
+            rc = kernel32.ReplaceFile(lpct_str(str(to_file)), lpct_str(str(from_file)), None, 0, None, None)
             if rc == 0:
                 raise OSError(f"Can't rename file, error: {kernel32.GetLastError()}")
 
         else:  # pragma: no cover
             os.rename(from_file, to_file)
 
     @staticmethod
@@ -658,15 +665,15 @@
         )
 
     def copy(self, new_filename: Path):
         # File needs to be opened in 'create' mode so that '__init__' does not raise 'SaveStateError' for the copy.
         # After copying, both of them can be closed and opened in 'read-write' mode.
 
         new_filename = _add_file_identifier(new_filename)
-        assert new_filename != self._savestate_name, "Copy can't have the same filename as the original."
+        assert new_filename != self._savestate_name, "Copy can't have the same filename as the original."  # noqa
 
         self.close()
         same_savestate = open(
             filename=self._savestate_name,
             flag="c",
             verify_checksums=self._verify_checksums,
             compact=self._compact,
@@ -719,22 +726,22 @@
             verify_checksums=verify_checksums,
             compact=compact,
             dbm_mode=dbm_mode,
         )
 
 
 def _add_file_identifier(filename: Path) -> Path:
-    """Adds savestat file identifier to the path."""
+    """Adds savestate file identifier to the path."""
     if filename.suffix == FILE_SUFFIX:
         return filename
     return filename.with_suffix(FILE_SUFFIX)
 
 
 def open(  # noqa
-    filename: Path,
+    filename: Union[str, Path],
     flag: Literal["r", "w", "c", "n"] = "r",
     verify_checksums: bool = False,
     compact: bool = False,
     dbm_mode: bool = False,
 ) -> Union[_SaveStateReadOnly, _SaveStateCreate, _SaveStateReadWrite, _SaveStateNew]:
     """Open a Savestate file.
 
@@ -748,14 +755,17 @@
     :param verify_checksums: Verify that the checksum for a key and value pair is correct on every __getitem__ call
     :param compact: Indicate whether to compact the savestate before closing it. No effect in read only mode.
     :param dbm_mode: Operate in dbm mode. This is faster, but only allows strings for keys and values.
     :raises ValueError: Flag argument incorrect.
     :raises SaveStateError: If flag is "r" or "w", and Savestate file does not exist.
     """
 
+    if isinstance(filename, str):
+        filename = Path(filename)
+
     filename = _add_file_identifier(filename)
 
     if flag == "r":
         return _SaveStateReadOnly(
             filename,
             verify_checksums=verify_checksums,
             dbm_mode=dbm_mode,
```

### Comparing `savestate-0.1.0/setup.py` & `savestate-0.1.1/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,26 +1,108 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: savestate
+Version: 0.1.1
+Summary: Persistent storage of arbitrary python objects
+Home-page: https://mrthearman.github.io/savestate/
+License: MIT
+Keywords: savestate
+Author: Matti Lamppu
+Author-email: lamppu.matti.akseli@gmail.com
+Requires-Python: >=3.9,<4
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.9
+Project-URL: Bug Tracker, https://github.com/MrThearMan/savestate/issues
+Project-URL: Repository, https://github.com/MrThearMan/savestate
+Description-Content-Type: text/markdown
 
-packages = \
-['savestate']
+# SaveState
 
-package_data = \
-{'': ['*']}
+[![Coverage Status][coverage-badge]][coverage]
+[![GitHub Workflow Status][status-badge]][status]
+[![PyPI][pypi-badge]][pypi]
+[![GitHub][licence-badge]][licence]
+[![GitHub Last Commit][repo-badge]][repo]
+[![GitHub Issues][issues-badge]][issues]
+[![Python Version][version-badge]][pypi]
 
-setup_kwargs = {
-    'name': 'savestate',
-    'version': '0.1.0',
-    'description': 'Persistent storage of arbitrary python objects',
-    'long_description': "# SaveState\n\n[![Coverage Status][coverage-badge]][coverage]\n[![GitHub Workflow Status][status-badge]][status]\n[![PyPI][pypi-badge]][pypi]\n[![GitHub][licence-badge]][licence]\n[![GitHub Last Commit][repo-badge]][repo]\n[![GitHub Issues][issues-badge]][issues]\n[![Python Version][version-badge]][pypi]\n\n```shell\npip install savestate\n```\n\n---\n\n**Documentation**: [https://mrthearman.github.io/savestate/](https://mrthearman.github.io/savestate/)\n\n**Source Code**: [https://github.com/MrThearMan/savestate/](https://github.com/MrThearMan/savestate/)\n\n---\n\nSaveState is a cross-platform fast file storage for arbitrary python objects. \nIt's similar to python's builtin [shelve][shelve] module, but aims to be more\nperformant on Windows while being cross-platform compatible.\n\nSavestate is inspired by [semidbm2][semidbm2], with a more modern interface.\nmapping-like functions, a context manager, and support for \narbitrary python objects.\n\n### Implementation details:\n- Pure python\n- No requirements or dependencies\n- A dict-like interface (no unions)\n- Same, single file on Windows and Linux (unlike shelve)\n- Key and value integrity can be evaluated with a checksum, which will detect data corruption on key access.\n- Recovery from missing bytes at the end of the file, or small amounts of corrupted data in the middle\n- Both values AND keys put in savestate must support [pickling][pickling].\nNote the [security implications][security] of this!\n  - This means that you can use arbitrary objects as keys if they support pickle (unlike shelve)\n- All the keys of the savestate are kept in memory, which limits the savestate size (not a problem for most applications)\n- NOT Thread safe, so cannot be accessed by multiple processes\n- File is append-only, so the more non-read operations you do, the more the file size is going to balloon\n  - However, you can *compact* the savestate, usually on *savestate.close()*, which will replace the savestate with a new file with only the current non-deleted data.\n  This will impact performance a little, but not by much\n  \n### Performance:\n- About 50-60% of the performance of shelve with [gdbm][gdbm] (linux), \n  but >5000% compared to shelve with [dumbdbm][dumbdbm] (windows) (>20000% for deletes!)\n  - Performance is more favorable with large keys and values when compared to gdbm, \n    but gdbm is still faster on subsequent reads/writes thanks to its caching\n- A dbm-mode for about double the speed of regular mode, but only string-type keys and values\n  - This is about 25-30% of the performance of gdbm on its own.\n  - Note: Values will be returned in bytes form!\n  \n> Source code includes a benchmark that you can run to get more accurate performance on your specific machine.\n\n\n[shelve]: https://docs.python.org/3/library/shelve.html\n[semidbm2]: https://github.com/quora/semidbm2\n[pickling]: https://docs.python.org/3/library/pickle.html#module-pickle\n[security]: https://docs.python.org/3/library/pickle.html#module-pickle\n[gdbm]: https://docs.python.org/3/library/dbm.html#module-dbm.gnu\n[dumbdbm]: https://docs.python.org/3/library/dbm.html#module-dbm.dumb\n\n[coverage-badge]: https://coveralls.io/repos/github/MrThearMan/savestate/badge.svg?branch=main\n[status-badge]: https://img.shields.io/github/workflow/status/MrThearMan/savestate/Tests\n[pypi-badge]: https://img.shields.io/pypi/v/savestate\n[licence-badge]: https://img.shields.io/github/license/MrThearMan/savestate\n[repo-badge]: https://img.shields.io/github/last-commit/MrThearMan/savestate\n[issues-badge]: https://img.shields.io/github/issues-raw/MrThearMan/savestate\n[version-badge]: https://img.shields.io/pypi/pyversions/savestate\n\n[coverage]: https://coveralls.io/github/MrThearMan/savestate?branch=main\n[status]: https://github.com/MrThearMan/savestate/actions/workflows/main.yml\n[pypi]: https://pypi.org/project/savestate\n[licence]: https://github.com/MrThearMan/savestate/blob/main/LICENSE\n[repo]: https://github.com/MrThearMan/savestate/commits/main\n[issues]: https://github.com/MrThearMan/savestate/issues\n",
-    'author': 'Matti Lamppu',
-    'author_email': 'lamppu.matti.akseli@gmail.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://mrthearman.github.io/savestate/',
-    'packages': packages,
-    'package_data': package_data,
-    'python_requires': '>=3.9,<4',
-}
+```shell
+pip install savestate
+```
 
+---
+
+**Documentation**: [https://mrthearman.github.io/savestate/](https://mrthearman.github.io/savestate/)
+
+**Source Code**: [https://github.com/MrThearMan/savestate/](https://github.com/MrThearMan/savestate/)
+
+---
+
+SaveState is a cross-platform fast file storage for arbitrary python objects.
+It's similar to python's builtin [shelve][shelve] module, but aims to be more
+performant on Windows while being cross-platform compatible.
+
+Savestate is inspired by [semidbm2][semidbm2], with a more modern interface.
+mapping-like functions, a context manager, and support for
+arbitrary python objects.
+
+### Implementation details:
+- Pure python
+- No requirements or dependencies
+- A dict-like interface (no unions)
+- Same, single file on Windows and Linux (unlike shelve)
+- Key and value integrity can be evaluated with a checksum, which will detect data corruption on key access.
+- Recovery from missing bytes at the end of the file, or small amounts of corrupted data in the middle
+- Both values AND keys put in savestate must support [pickling][pickling].
+Note the [security implications][security] of this!
+  - This means that you can use arbitrary objects as keys if they support pickle (unlike shelve)
+- All the keys of the savestate are kept in memory, which limits the savestate size (not a problem for most applications)
+- NOT Thread safe, so cannot be accessed by multiple processes
+- File is append-only, so the more non-read operations you do, the more the file size is going to balloon
+  - However, you can *compact* the savestate, usually on *savestate.close()*, which will replace the savestate with a new file with only the current non-deleted data.
+  This will impact performance a little, but not by much
+
+### Performance:
+- About 50-60% of the performance of shelve with [gdbm][gdbm] (linux),
+  but >5000% compared to shelve with [dumbdbm][dumbdbm] (windows) (>20000% for deletes!)
+  - Performance is more favorable with large keys and values when compared to gdbm,
+    but gdbm is still faster on subsequent reads/writes thanks to its caching
+- A dbm-mode for about double the speed of regular mode, but only string-type keys and values
+  - This is about 25-30% of the performance of gdbm on its own.
+  - Note: Values will be returned in bytes form!
+
+> Source code includes a benchmark that you can run to get more accurate performance on your specific machine.
+
+
+[shelve]: https://docs.python.org/3/library/shelve.html
+[semidbm2]: https://github.com/quora/semidbm2
+[pickling]: https://docs.python.org/3/library/pickle.html#module-pickle
+[security]: https://docs.python.org/3/library/pickle.html#module-pickle
+[gdbm]: https://docs.python.org/3/library/dbm.html#module-dbm.gnu
+[dumbdbm]: https://docs.python.org/3/library/dbm.html#module-dbm.dumb
+
+[coverage-badge]: https://coveralls.io/repos/github/MrThearMan/savestate/badge.svg?branch=main
+[status-badge]: https://img.shields.io/github/actions/workflow/status/MrThearMan/savestate/test.yml?branch=main
+[pypi-badge]: https://img.shields.io/pypi/v/savestate
+[licence-badge]: https://img.shields.io/github/license/MrThearMan/savestate
+[repo-badge]: https://img.shields.io/github/last-commit/MrThearMan/savestate
+[issues-badge]: https://img.shields.io/github/issues-raw/MrThearMan/savestate
+[version-badge]: https://img.shields.io/pypi/pyversions/savestate
+
+[coverage]: https://coveralls.io/github/MrThearMan/savestate?branch=main
+[status]: https://github.com/MrThearMan/savestate/actions/workflows/test.yml
+[pypi]: https://pypi.org/project/savestate
+[licence]: https://github.com/MrThearMan/savestate/blob/main/LICENSE
+[repo]: https://github.com/MrThearMan/savestate/commits/main
+[issues]: https://github.com/MrThearMan/savestate/issues
 
-setup(**setup_kwargs)
```

