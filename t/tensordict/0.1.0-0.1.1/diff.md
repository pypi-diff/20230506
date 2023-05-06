# Comparing `tmp/tensordict-0.1.0-py3-none-any.whl.zip` & `tmp/tensordict-0.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,26 +1,29 @@
-Zip file size: 102448 bytes, number of entries: 24
--rw-r--r--  2.0 unx      859 b- defN 23-Mar-16 12:18 tensordict/__init__.py
--rw-r--r--  2.0 unx    28442 b- defN 23-Mar-16 12:18 tensordict/memmap.py
--rw-r--r--  2.0 unx   228528 b- defN 23-Mar-16 12:18 tensordict/tensordict.py
--rw-r--r--  2.0 unx    24542 b- defN 23-Mar-16 12:18 tensordict/utils.py
--rw-r--r--  2.0 unx       79 b- defN 23-Mar-16 12:27 tensordict/version.py
--rw-r--r--  2.0 unx     1034 b- defN 23-Mar-16 12:18 tensordict/nn/__init__.py
--rw-r--r--  2.0 unx    18445 b- defN 23-Mar-16 12:18 tensordict/nn/common.py
--rw-r--r--  2.0 unx    14639 b- defN 23-Mar-16 12:18 tensordict/nn/functional_modules.py
--rw-r--r--  2.0 unx    18684 b- defN 23-Mar-16 12:18 tensordict/nn/probabilistic.py
--rw-r--r--  2.0 unx    10925 b- defN 23-Mar-16 12:18 tensordict/nn/sequence.py
--rw-r--r--  2.0 unx     3198 b- defN 23-Mar-16 12:18 tensordict/nn/utils.py
--rw-r--r--  2.0 unx      499 b- defN 23-Mar-16 12:18 tensordict/nn/distributions/__init__.py
--rw-r--r--  2.0 unx     7073 b- defN 23-Mar-16 12:18 tensordict/nn/distributions/continuous.py
--rw-r--r--  2.0 unx     2580 b- defN 23-Mar-16 12:18 tensordict/nn/distributions/discrete.py
--rw-r--r--  2.0 unx     6504 b- defN 23-Mar-16 12:18 tensordict/nn/distributions/truncated_normal.py
--rw-r--r--  2.0 unx     1226 b- defN 23-Mar-16 12:18 tensordict/nn/distributions/utils.py
--rw-r--r--  2.0 unx      382 b- defN 23-Mar-16 12:18 tensordict/prototype/__init__.py
--rw-r--r--  2.0 unx     7507 b- defN 23-Mar-16 12:18 tensordict/prototype/fx.py
--rw-r--r--  2.0 unx    32673 b- defN 23-Mar-16 12:18 tensordict/prototype/tensorclass.py
--rw-r--r--  2.0 unx     1098 b- defN 23-Mar-16 12:27 tensordict-0.1.0.dist-info/LICENSE
--rw-r--r--  2.0 unx    14118 b- defN 23-Mar-16 12:27 tensordict-0.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Mar-16 12:27 tensordict-0.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-Mar-16 12:27 tensordict-0.1.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     2050 b- defN 23-Mar-16 12:27 tensordict-0.1.0.dist-info/RECORD
-24 files, 425188 bytes uncompressed, 99132 bytes compressed:  76.7%
+Zip file size: 129598 bytes, number of entries: 27
+-rw-r--r--  2.0 unx     1088 b- defN 23-May-06 20:59 tensordict/__init__.py
+-rw-r--r--  2.0 unx     6000 b- defN 23-May-06 20:59 tensordict/_contextlib.py
+-rw-r--r--  2.0 unx    29601 b- defN 23-May-06 20:59 tensordict/memmap.py
+-rw-r--r--  2.0 unx    33049 b- defN 23-May-06 20:59 tensordict/persistent.py
+-rw-r--r--  2.0 unx    30420 b- defN 23-May-06 20:59 tensordict/tensorclass.py
+-rw-r--r--  2.0 unx   267125 b- defN 23-May-06 20:59 tensordict/tensordict.py
+-rw-r--r--  2.0 unx    26209 b- defN 23-May-06 20:59 tensordict/utils.py
+-rw-r--r--  2.0 unx       79 b- defN 23-May-06 21:07 tensordict/version.py
+-rw-r--r--  2.0 unx     1314 b- defN 23-May-06 20:59 tensordict/nn/__init__.py
+-rw-r--r--  2.0 unx    35649 b- defN 23-May-06 20:59 tensordict/nn/common.py
+-rw-r--r--  2.0 unx    19188 b- defN 23-May-06 20:59 tensordict/nn/functional_modules.py
+-rw-r--r--  2.0 unx    22301 b- defN 23-May-06 20:59 tensordict/nn/probabilistic.py
+-rw-r--r--  2.0 unx    19564 b- defN 23-May-06 20:59 tensordict/nn/sequence.py
+-rw-r--r--  2.0 unx    10621 b- defN 23-May-06 20:59 tensordict/nn/utils.py
+-rw-r--r--  2.0 unx      499 b- defN 23-May-06 20:59 tensordict/nn/distributions/__init__.py
+-rw-r--r--  2.0 unx     7073 b- defN 23-May-06 20:59 tensordict/nn/distributions/continuous.py
+-rw-r--r--  2.0 unx     2580 b- defN 23-May-06 20:59 tensordict/nn/distributions/discrete.py
+-rw-r--r--  2.0 unx     6504 b- defN 23-May-06 20:59 tensordict/nn/distributions/truncated_normal.py
+-rw-r--r--  2.0 unx     1226 b- defN 23-May-06 20:59 tensordict/nn/distributions/utils.py
+-rw-r--r--  2.0 unx      381 b- defN 23-May-06 20:59 tensordict/prototype/__init__.py
+-rw-r--r--  2.0 unx     7507 b- defN 23-May-06 20:59 tensordict/prototype/fx.py
+-rw-r--r--  2.0 unx      739 b- defN 23-May-06 20:59 tensordict/prototype/tensorclass.py
+-rw-r--r--  2.0 unx     1098 b- defN 23-May-06 21:07 tensordict-0.1.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx    15197 b- defN 23-May-06 21:07 tensordict-0.1.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-06 21:07 tensordict-0.1.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-May-06 21:07 tensordict-0.1.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     2297 b- defN 23-May-06 21:07 tensordict-0.1.1.dist-info/RECORD
+27 files, 547412 bytes uncompressed, 125906 bytes compressed:  77.0%
```

## zipnote {}

```diff
@@ -1,13 +1,22 @@
 Filename: tensordict/__init__.py
 Comment: 
 
+Filename: tensordict/_contextlib.py
+Comment: 
+
 Filename: tensordict/memmap.py
 Comment: 
 
+Filename: tensordict/persistent.py
+Comment: 
+
+Filename: tensordict/tensorclass.py
+Comment: 
+
 Filename: tensordict/tensordict.py
 Comment: 
 
 Filename: tensordict/utils.py
 Comment: 
 
 Filename: tensordict/version.py
@@ -51,23 +60,23 @@
 
 Filename: tensordict/prototype/fx.py
 Comment: 
 
 Filename: tensordict/prototype/tensorclass.py
 Comment: 
 
-Filename: tensordict-0.1.0.dist-info/LICENSE
+Filename: tensordict-0.1.1.dist-info/LICENSE
 Comment: 
 
-Filename: tensordict-0.1.0.dist-info/METADATA
+Filename: tensordict-0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: tensordict-0.1.0.dist-info/WHEEL
+Filename: tensordict-0.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: tensordict-0.1.0.dist-info/top_level.txt
+Filename: tensordict-0.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: tensordict-0.1.0.dist-info/RECORD
+Filename: tensordict-0.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tensordict/__init__.py

```diff
@@ -1,39 +1,46 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
 from tensordict.memmap import MemmapTensor, set_transfer_ownership
+from tensordict.persistent import PersistentTensorDict
+from tensordict.tensorclass import is_tensorclass, tensorclass
 from tensordict.tensordict import (
     is_batchedtensor,
     is_memmap,
     is_tensor_collection,
     LazyStackedTensorDict,
     make_tensordict,
     merge_tensordicts,
     pad,
     pad_sequence,
     SubTensorDict,
     TensorDict,
+    TensorDictBase,
 )
 
 try:
     from tensordict.version import __version__
 except ImportError:
     __version__ = None
 
 
 __all__ = [
     "LazyStackedTensorDict",
     "MemmapTensor",
     "SubTensorDict",
     "TensorDict",
+    "TensorDictBase",
     "merge_tensordicts",
     "set_transfer_ownership",
     "pad_sequence",
     "make_tensordict",
     "is_memmap",
     "is_batchedtensor",
     "is_tensor_collection",
     "pad",
+    "PersistentTensorDict",
+    "is_tensorclass",
+    "tensorclass",
 ]
```

## tensordict/memmap.py

```diff
@@ -7,14 +7,15 @@
 
 import functools
 import os
 import tempfile
 import warnings
 from copy import copy, deepcopy
 from pathlib import Path
+from sys import getrefcount
 from tempfile import _TemporaryFileWrapper
 from typing import Any, Callable, Sequence
 
 import numpy as np
 import torch
 
 from tensordict.utils import (
@@ -30,14 +31,17 @@
 
 
 NoneType = type(None)
 EllipsisType = type(Ellipsis)
 
 
 MEMMAP_HANDLED_FN: dict[Callable, Callable] = {}
+HAS_OWNERSHIP = {}
+# HAD_OWNERSHIP = {}
+TRANSFER_OWNERSHIP = {}
 
 
 def implements_for_memmap(torch_function: Callable) -> Callable:
     """Register a torch function override for ScalarTensor."""
 
     @functools.wraps(torch_function)
     def decorator(func: Callable) -> Callable:
@@ -161,15 +165,15 @@
                 prefix=prefix, delete=False, mode="r+"
             )
         else:
             # if filename doesn't exist we must create it
             Path(filename).touch(exist_ok=True)
             self.file = open(filename, mode="r+")
 
-        self.filename = self.file.name
+        self.filename = copy(self.file.name)
         self.file.close()  # we close the file for now, but don't delete it
 
         if isinstance(size[0], (torch.Tensor, MemmapTensor, np.ndarray)):
             raise NotImplementedError(
                 "Creating a Memmap array from a tensor is not permitted anymore. "
                 "Call MemmapTensor.from_tensor(tensor) instead."
             )
@@ -276,16 +280,18 @@
         memmap_copy = copy(memmap_tensor)
         if memmap_copy._index is None:
             memmap_copy._index = []
         else:
             # avoid extending someone else's index
             memmap_copy._index = deepcopy(memmap_copy._index)
         memmap_copy._index.append(index)
-        memmap_copy.transfer_ownership = False
+        # memmap_copy.transfer_ownership = False
         memmap_copy._shape_indexed = None
+        memmap_copy.file = memmap_tensor.file
+
         return memmap_copy
 
     def __iter__(self):
         for i in range(self.shape[0]):
             yield self[i]
 
     def _init_shape(
@@ -294,21 +300,22 @@
         device: DeviceType,
         dtype: torch.dtype,
         transfer_ownership: bool,
     ):
         self._device = device
         self._shape = shape
         self._shape_indexed = None
-        self.transfer_ownership = transfer_ownership
         self.np_shape = tuple(self._shape)
         self._dtype = dtype
         self._ndim = len(shape)
         self._numel = prod(shape)
-        self._has_ownership = True
-        self._had_ownership = True
+
+        TRANSFER_OWNERSHIP[self.filename] = transfer_ownership
+        HAS_OWNERSHIP[self.filename] = True
+        # HAD_OWNERSHIP[self.filename] = True
 
         self._tensor_dir = torch.zeros(0, device=device, dtype=dtype).__dir__()
         self._save_item(shape)
 
     def _get_memmap_array(self) -> np.memmap:
         if self._memmap_array is None:
             self._memmap_array = np.memmap(
@@ -520,29 +527,38 @@
 
         """
         if not isinstance(value, bool):
             raise TypeError(
                 f"value provided to set_transfer_ownership should be a "
                 f"boolean, got {type(value)}"
             )
-        self.transfer_ownership = value
+        TRANSFER_OWNERSHIP[self.filename] = value
         return self
 
     def __deepcopy__(self, memo: dict[int, Any] | None = None) -> MemmapTensor:
         warnings.warn(
             "calling deepcopy on a memmap tensor involves loading it in memory "
             "and recreating a memmap tensor from scratch (as no file destination "
             "can be passed to deepcopy(...).",
             stacklevel=2,
         )
         return MemmapTensor.from_tensor(self.clone())
 
     def __del__(self) -> None:
-        if "_has_ownership" in self.__dir__() and self._has_ownership:
-            if isinstance(self.file, tempfile._TemporaryFileWrapper):
+        if not hasattr(self, "file"):
+            return
+        # for some reason Memmap keeps 2 refs to the file
+        if (
+            HAS_OWNERSHIP
+            and HAS_OWNERSHIP.get(self.filename, False)
+            and getrefcount(self.file) <= 2
+        ):
+            if isinstance(self.file, tempfile._TemporaryFileWrapper) and os.path.isfile(
+                self.filename
+            ):
                 # only delete file if we created a temporary file. Otherwise file should
                 # persist on disk
                 os.unlink(self.filename)
             del self.file
 
     def __eq__(self, other: Any) -> torch.Tensor:
         return self._tensor == other
@@ -616,45 +632,56 @@
                 idx = tuple(
                     _idx.cpu() if isinstance(_idx, torch.Tensor) else _idx
                     for _idx in idx
                 )
             self.memmap_array[idx] = to_numpy(value)
 
     def __setstate__(self, state: dict[str, Any]) -> None:
+        filename = state["filename"]
         if state["file"] is None:
             # state["_had_ownership"] = state["_had_ownership"]
             # state["_has_ownership"] = delete
             # tmpfile = tempfile.NamedTemporaryFile(delete=False)
             # tmpfile.close()
-            tmpfile = _TemporaryFileWrapper(None, state["filename"], delete=True)
-            tmpfile.name = state["filename"]
-            tmpfile._closer.name = state["filename"]
+            tmpfile = _TemporaryFileWrapper(None, filename, delete=True)
+            tmpfile.name = filename
+            tmpfile._closer.name = filename
             state["file"] = tmpfile
+
+        # We only set the ownership if it's not set
+        if state["transfer_ownership"]:
+            TRANSFER_OWNERSHIP[filename] = True
+        else:
+            TRANSFER_OWNERSHIP.setdefault(filename, state["transfer_ownership"])
+        if state["_has_ownership"]:
+            HAS_OWNERSHIP[filename] = True
+        else:
+            HAS_OWNERSHIP.setdefault(filename, state["_has_ownership"])
         self.__dict__.update(state)
 
     def __getstate__(self) -> dict[str, Any]:
         state = self.__dict__.copy()
+        id_file = state["filename"]
         state["file"] = None
         state["_memmap_array"] = None
         state["_fake"] = None
-        state["_has_ownership"] = (
-            state["transfer_ownership"] and state["_had_ownership"]
-        )
-        self._had_ownership = self._has_ownership
+
+        # we are abandoning ownership if we need to transfer it and if we have it
+        if HAS_OWNERSHIP[id_file] and TRANSFER_OWNERSHIP[id_file]:
+            state["_has_ownership"] = True
+            state["transfer_ownership"] = True
+            HAS_OWNERSHIP[id_file] = False
+            TRANSFER_OWNERSHIP[id_file] = False
+        else:
+            state["_has_ownership"] = False
+            state["transfer_ownership"] = False
+
         # self._had_ownership = self._has_ownership = state["_had_ownership"]
         return state
 
-    def __reduce__(self) -> tuple[Any, ...]:
-        if self.transfer_ownership and self._has_ownership:
-            self._has_ownership = False
-            # those values should already be False
-            # self.file.delete = False
-            # self.file._closer.delete = False
-        return super().__reduce__()
-
     def to(
         self,
         dest: DeviceType | torch.dtype,
         non_blocking: bool = False,
     ) -> torch.Tensor | MemmapTensor:
         """Maps a MemmapTensor to a given dtype or device.
 
@@ -714,14 +741,27 @@
             )
         return tensor_from_memoryview(
             dtype=self.dtype,
             shape=list(self.shape),
             mv=memoryview(self.memmap_array),
         )
 
+    # backward compatibility
+    @property
+    def _has_ownership(self):
+        return HAS_OWNERSHIP[self.filename]
+
+    # @property
+    # def _had_ownership(self):
+    #     return HAD_OWNERSHIP[self.filename]
+
+    @property
+    def transfer_ownership(self):
+        return TRANSFER_OWNERSHIP[self.filename]
+
 
 def tensor_from_memoryview(
     mv: memoryview, dtype: torch.dtype, shape: Sequence[int]
 ) -> torch.Tensor:
     # From torchsnapshot
     # PyTorch issues a warning if the given memoryview is non-writable. This is
     # not a concern for torchsnapshot, as tensors created from non-writable
```

## tensordict/tensordict.py

```diff
@@ -35,15 +35,15 @@
 from tensordict.memmap import memmap_tensor_as_tensor, MemmapTensor
 from tensordict.utils import (
     _device,
     _dtype,
     _get_item,
     _getitem_batch_size,
     _is_shared,
-    _nested_key_type_check,
+    _nested_key_check,
     _set_item,
     _shape,
     _sub_index,
     convert_ellipsis_to_idx,
     DeviceType,
     expand_as_right,
     expand_right,
@@ -126,15 +126,15 @@
         ... class MyClass:
         ...     pass
         ...
         >>> is_tensor_collection(MyClass)  # True
         >>> is_tensor_collection(MyClass(batch_size=[]))  # True
 
     """
-    from tensordict.prototype import is_tensorclass
+    from tensordict.tensorclass import is_tensorclass
 
     return (
         issubclass(datatype, TensorDictBase)
         if isinstance(datatype, type)
         else isinstance(datatype, TensorDictBase)
     ) or is_tensorclass(datatype)
 
@@ -226,15 +226,15 @@
 
     def __len__(self) -> int:
         return sum(1 for _ in self)
 
     def _items(
         self, tensordict: TensorDict | None = None
     ) -> Iterable[tuple[NestedKey, CompatibleType]]:
-        from tensordict.prototype import is_tensorclass
+        from tensordict.tensorclass import is_tensorclass
 
         if tensordict is None:
             tensordict = self.tensordict
         if isinstance(tensordict, TensorDict) or is_tensorclass(tensordict):
             return tensordict._tensordict.items()
         elif isinstance(tensordict, LazyStackedTensorDict):
             return _iter_items_lazystack(tensordict)
@@ -356,14 +356,160 @@
 
         Returns:
             a torch.Size object describing the TensorDict batch size.
 
         """
         raise NotImplementedError
 
+    @property
+    def names(self):
+        names = self._names
+        if names is None:
+            return [None for _ in range(self.batch_dims)]
+        return names
+
+    @names.setter
+    def names(self, value):
+        # we don't run checks on types for efficiency purposes
+        if value is None:
+            self._names = None
+            return
+        num_none = sum(v is None for v in value)
+        if num_none:
+            num_none -= 1
+        if len(set(value)) != len(value) - num_none:
+            raise ValueError(f"Some dimension names are non-unique: {value}.")
+        if len(value) != self.batch_dims:
+            raise ValueError(
+                "the length of the dimension names must equate the tensordict batch_dims attribute. "
+                f"Got {value} for batch_dims {self.batch_dims}."
+            )
+        self._rename_subtds(value)
+        self._names = list(value)
+
+    @abc.abstractmethod
+    def _rename_subtds(self, value):
+        # renames all the sub-tensordicts dimension according to value.
+        # If value has less dimensions than the TD, the rest is just assumed to be None
+        raise NotImplementedError
+
+    def _check_dim_name(self, name):
+        if name is None:
+            return False
+        if self._names is not None and name in self._names:
+            return True
+        for key in self.keys():
+            if is_tensor_collection(self.entry_class(key)):
+                if self.get(key)._check_dim_name(name):
+                    return True
+        else:
+            return False
+
+    def refine_names(self, *names):
+        """Refines the dimension names of self according to names.
+
+        Refining is a special case of renaming that “lifts” unnamed dimensions.
+        A None dim can be refined to have any name; a named dim can only be
+        refined to have the same name.
+
+        Because named tensors can coexist with unnamed tensors, refining names
+        gives a nice way to write named-tensor-aware code that works with both
+        named and unnamed tensors.
+
+        names may contain up to one Ellipsis (...). The Ellipsis is expanded
+        greedily; it is expanded in-place to fill names to the same length as
+        self.dim() using names from the corresponding indices of self.names.
+
+        Returns: the tensordict with dimensions named accordingly.
+
+        """
+        # replace ellipsis if any
+        names_copy = copy(names)
+        if any(name is Ellipsis for name in names):
+            ellipsis_name = [NO_DEFAULT for _ in range(self.ndim - len(names) + 1)]
+            names = []
+            for name in names_copy:
+                if name is Ellipsis:
+                    names += ellipsis_name
+                else:
+                    names.append(name)
+        # check that the names that are set are either None or identical
+        curr_names = self.names
+        for i, name in enumerate(names):
+            if name is NO_DEFAULT:
+                # whatever value is ok
+                names[i] = curr_names[i]
+                continue
+            else:
+                if curr_names[i] is None:
+                    continue
+                if self.names[i] == name:
+                    continue
+                else:
+                    raise RuntimeError(
+                        f"refine_names: cannot coerce TensorDict names {self.names} with {names_copy}."
+                    )
+        self.names = names
+        # we also need to rename the sub-tensordicts
+        self._rename_subtds(self.names)
+        return self
+
+    def rename(self, *names, **rename_map):
+        clone = self.clone(recurse=False)
+        if len(names) == 1 and names[0] is None:
+            clone.names = None
+        if rename_map and names:
+            raise ValueError(
+                "Passed both a name map and a name list. Only one is accepted."
+            )
+        elif not rename_map and not names:
+            raise ValueError(
+                "Neither a name map nor a name list was passed. "
+                "Only one is accepted."
+            )
+        elif rename_map:
+            for i, name in enumerate(clone.names):
+                new_name = rename_map.pop(name, NO_DEFAULT)
+                if new_name is not NO_DEFAULT:
+                    clone._names[i] = new_name
+            if rename_map:
+                raise ValueError(
+                    f"Some names to be renamed were not part of the tensordict names: {rename_map.keys()} vs {self.names}."
+                )
+        else:
+            clone.names = names
+        return clone
+
+    def rename_(self, *names, **rename_map):
+        if len(names) == 1 and names[0] is None:
+            self.names = None
+        if rename_map and names:
+            raise ValueError(
+                "Passed both a name map and a name list. " "Only one is accepted."
+            )
+        elif not rename_map and not names and self.batch_dims:
+            raise ValueError(
+                "Neither a name map nor a name list was passed. "
+                "Only one is accepted."
+            )
+        elif rename_map:
+            _names = copy(self.names)
+            for i, name in enumerate(_names):
+                new_name = rename_map.pop(name, NO_DEFAULT)
+                if new_name is not NO_DEFAULT:
+                    _names[i] = new_name
+            if rename_map:
+                raise ValueError(
+                    f"Some names to be renamed were not part of the tensordict names: {rename_map.keys()} vs {self.names}."
+                )
+            self.names = _names
+        else:
+            self.names = names
+        return self
+
     def size(self, dim: int | None = None) -> torch.Size | int:
         """Returns the size of the dimension indicated by :obj:`dim`.
 
         If dim is not specified, returns the batch_size (or shape) of the TensorDict.
 
         """
         if dim is None:
@@ -380,27 +526,32 @@
         if self._lazy:
             raise RuntimeError(
                 "modifying the batch size of a lazy repesentation of a "
                 "tensordict is not permitted. Consider instantiating the "
                 "tensordict first by calling `td = td.to_tensordict()` before "
                 "resetting the batch size."
             )
-        if self.batch_size == new_batch_size:
-            return
         if not isinstance(new_batch_size, torch.Size):
             new_batch_size = torch.Size(new_batch_size)
         for key in self.keys():
             if is_tensor_collection(self.entry_class(key)):
                 tensordict = self.get(key)
                 if len(tensordict.batch_size) < len(new_batch_size):
                     # document as edge case
                     tensordict.batch_size = new_batch_size
                     self._set(key, tensordict)
         self._check_new_batch_size(new_batch_size)
         self._change_batch_size(new_batch_size)
+        if self._names is not None:
+            if len(self._names) < len(new_batch_size):
+                self.names = self._names + [None] * (
+                    len(new_batch_size) - len(self._names)
+                )
+            else:
+                self.names = self._names[: self.batch_dims]
 
     @property
     def batch_dims(self) -> int:
         """Length of the tensordict batch size.
 
         Returns:
             int describing the number of dimensions of the tensordict.
@@ -531,21 +682,23 @@
         raise NotImplementedError(f"{self.__class__.__name__}")
 
     @abc.abstractmethod
     def entry_class(self, key: NestedKey) -> type:
         """Returns the class of an entry, avoiding a call to `isinstance(td.get(key), type)`."""
         raise NotImplementedError(f"{self.__class__.__name__}")
 
+    @abc.abstractmethod
     def set(
         self, key: NestedKey, item: CompatibleType, inplace: bool = False, **kwargs: Any
     ) -> TensorDictBase:
         """Sets a new key-value pair.
 
         Args:
-            key (str): name of the value
+            key (str, tuple of str): name of the key to be set.
+                If tuple of str it is equivalent to chained calls of getattr
             item (torch.Tensor): value to be stored in the tensordict
             inplace (bool, optional): if True and if a key matches an existing
                 key in the tensordict, then the update will occur in-place
                 for that key-value pair. Default is :obj:`False`.
 
         Returns:
             self
@@ -972,24 +1125,69 @@
             else:
                 raise NotImplementedError(f"Type {type(value)} is not supported.")
             if not pseudo_rand:
                 _tag += 1
             else:
                 _tag = int_generator(_tag + 1)
             _future_list.append(dist.irecv(value, src=src, tag=_tag))
-            self.set(key, value, inplace=True)
         if not root:
             return _tag, _future_list
         elif return_premature:
             return _future_list
         else:
             for future in _future_list:
                 future.wait()
             return
 
+    def reduce(self, dst, op=dist.ReduceOp.SUM, async_op=False, return_premature=False):
+        """Reduces the tensordict across all machines.
+
+        Only the process with ``rank`` dst is going to receive the final result.
+
+        """
+        return self._reduce(dst, op, async_op, return_premature)
+
+    def _reduce(
+        self,
+        dst,
+        op=dist.ReduceOp.SUM,
+        async_op=False,
+        return_premature=False,
+        _future_list=None,
+    ):
+        root = False
+        if _future_list is None:
+            _future_list = []
+            root = True
+        for key in self.sorted_keys:
+            value = self.get(key)
+            if is_tensor_collection(value):
+                _future_list = value._reduce(
+                    dst=dst,
+                    op=op,
+                    async_op=async_op,
+                    _future_list=_future_list,
+                )
+                continue
+            elif isinstance(value, MemmapTensor):
+                value = value.as_tensor()
+            elif isinstance(value, Tensor):
+                pass
+            else:
+                raise NotImplementedError(f"Type {type(value)} is not supported.")
+            _future_list.append(dist.reduce(value, dst=dst, op=op, async_op=async_op))
+        if not root:
+            return _future_list
+        elif async_op and return_premature:
+            return _future_list
+        elif async_op:
+            for future in _future_list:
+                future.wait()
+            return
+
     def _stack_onto_at_(
         self,
         key: str,
         list_item: list[CompatibleType],
         dim: int,
         idx: IndexType,
     ) -> TensorDictBase:
@@ -1011,41 +1209,42 @@
             raise KeyError(
                 f'key "{key}" not found in {self.__class__.__name__} with '
                 f"keys {sorted(self.keys())}"
             )
 
     @abc.abstractmethod
     def get(
-        self, key: NestedKey, default: str | CompatibleType = "_no_default_"
+        self, key: NestedKey, default: str | CompatibleType = NO_DEFAULT
     ) -> CompatibleType:
         """Gets the value stored with the input key.
 
         Args:
-            key (str): key to be queried.
+            key (str, tuple of str): key to be queried. If tuple of str it is
+                equivalent to chained calls of getattr.
             default: default value if the key is not found in the tensordict.
 
         """
         raise NotImplementedError(f"{self.__class__.__name__}")
 
     def pop(
-        self, key: NestedKey, default: str | CompatibleType = "_no_default_"
+        self, key: NestedKey, default: str | CompatibleType = NO_DEFAULT
     ) -> CompatibleType:
-        _nested_key_type_check(key)
+        _nested_key_check(key)
         try:
             # using try/except for get/del is suboptimal, but
             # this is faster that checkink if key in self keys
             out = self.get(key, default)
             self.del_(key)
-        except KeyError:
+        except KeyError as err:
             # if default provided, 'out' value will return, else raise error
-            if default == "_no_default_":
+            if default == NO_DEFAULT:
                 raise KeyError(
-                    f"You are trying to pop key `{key}` which is not in dict"
+                    f"You are trying to pop key `{key}` which is not in dict "
                     f"without providing default value."
-                )
+                ) from err
         return out
 
     def apply_(self, fn: Callable) -> TensorDictBase:
         """Applies a callable to all values stored in the tensordict and re-writes them in-place.
 
         Args:
             fn (Callable): function to be applied to the tensors in the
@@ -1058,14 +1257,15 @@
         return self.apply(fn, inplace=True)
 
     def apply(
         self,
         fn: Callable,
         *others: TensorDictBase,
         batch_size: Sequence[int] | None = None,
+        names: Sequence[str] | None = None,
         inplace: bool = False,
         **constructor_kwargs,
     ) -> TensorDictBase:
         """Applies a callable to all values stored in the tensordict and sets them in a new tensordict.
 
         The apply method will return an TensorDict instance, regardless of the
         input type. To keep the same type, one can execute
@@ -1080,14 +1280,16 @@
                 current tensordict. The :obj:`fn` argument should receive as many
                 inputs as the number of tensordicts, including the one where apply is
                 being called.
             batch_size (sequence of int, optional): if provided,
                 the resulting TensorDict will have the desired batch_size.
                 The :obj:`batch_size` argument should match the batch_size after
                 the transformation. This is a keyword only argument.
+            names (list of str, optional): the new dimension names, in case the
+                batch_size is modified.
             inplace (bool, optional): if True, changes are made in-place.
                 Default is False. This is a keyword only argument.
             **constructor_kwargs: additional keyword arguments to be passed to the
                 TensorDict constructor.
 
         Returns:
             a new tensordict with transformed_in tensors.
@@ -1102,24 +1304,26 @@
             >>> assert (td_2["b", "c"] == 2).all()
         """
         if inplace:
             out = self
         elif batch_size is not None:
             out = TensorDict(
                 {},
-                batch_size=batch_size,
+                batch_size=torch.Size(batch_size),
+                names=names,
                 device=self.device,
                 _run_checks=False,
                 **constructor_kwargs,
             )
         else:
             out = TensorDict(
                 {},
                 batch_size=self.batch_size,
                 device=self.device,
+                names=self._names,
                 _run_checks=False,
                 **constructor_kwargs,
             )
 
         is_locked = out.is_locked
         if not inplace and is_locked:
             out.unlock_()
@@ -1144,14 +1348,29 @@
                 else:
                     out._set(key, item_trsf, inplace=inplace)
 
         if not inplace and is_locked:
             out.lock_()
         return out
 
+    def as_tensor(self):
+        """Calls as_tensor on all the tensors contained in the object.
+
+        This is reserved to classes that contain exclusively MemmapTensors,
+        and will raise an exception in all other cases.
+
+        """
+        try:
+            return self.apply(lambda x: x.as_tensor())
+        except AttributeError as err:
+            raise AttributeError(
+                f"{self.__class__.__name__} does not have an 'as_tensor' method "
+                f"because at least one of its tensors does not support this method."
+            ) from err
+
     def update(
         self,
         input_dict_or_td: dict[str, CompatibleType] | TensorDictBase,
         clone: bool = False,
         inplace: bool = False,
     ) -> TensorDictBase:
         """Updates the TensorDict with values from either a dictionary or another TensorDict.
@@ -1280,27 +1499,29 @@
                 )
             if clone:
                 value = value.clone()
             self.set_at_(key, value, idx)
         return self
 
     def _convert_to_tensor(self, array: np.ndarray) -> Tensor | MemmapTensor:
+        if isinstance(array, np.bool_):
+            array = array.item()
         return torch.as_tensor(array, device=self.device)
 
     def _convert_to_tensordict(self, dict_value: dict[str, Any]) -> TensorDictBase:
         return TensorDict(
             dict_value,
             batch_size=self.batch_size,
             device=self.device,
             _is_shared=self._is_shared,
             _is_memmap=self._is_memmap,
         )
 
     def _validate_key(self, key: NestedKey) -> NestedKey:
-        _nested_key_type_check(key)
+        _nested_key_check(key)
 
         if isinstance(key, tuple) and len(key) == 1:
             key = key[0]
 
         return key
 
     def _validate_value(
@@ -1331,14 +1552,28 @@
                 value.batch_size = self.batch_size
             else:
                 raise RuntimeError(
                     f"batch dimension mismatch, got self.batch_size"
                     f"={self.batch_size} and value.shape[:self.batch_dims]"
                     f"={_shape(value)[: self.batch_dims]} with value {value}"
                 )
+        if (
+            self._names is not None
+            and is_tensor_collection(value)
+            and check_shape
+            and value.names[: self.ndim] != self.names
+        ):
+            value = value.clone(False).refine_names(*self.names)
+        elif (
+            self._names is None
+            and check_shape
+            and is_tensor_collection(value)
+            and value._names is not None
+        ):
+            self.names = value.names[: self.batch_dims]
 
         return value
 
     @abc.abstractmethod
     def pin_memory(self) -> TensorDictBase:
         """Calls :obj:`pin_memory` on the stored tensors."""
         raise NotImplementedError(f"{self.__class__.__name__}")
@@ -1426,19 +1661,125 @@
             last_n_dims = tensor_dims - tensordict_dims
             if last_n_dims > 0:
                 d[key] = value.expand((*shape, *value.shape[-last_n_dims:]))
             else:
                 d[key] = value.expand(shape)
         return TensorDict(
             source=d,
-            batch_size=shape,
+            batch_size=torch.Size(shape),
             device=self.device,
             _run_checks=False,
         )
 
+    def flatten(self, start_dim=0, end_dim=-1):
+        """Flattens all the tensors of a tensordict.
+
+        Args:
+            start_dim (int) – the first dim to flatten
+            end_dim (int) – the last dim to flatten
+
+        Examples:
+            >>> td = TensorDict({"a": torch.arange(60).view(3, 4, 5), "b": torch.arange(12).view(3, 4)}, [3, 4])
+            >>> td_flat = td.flatten(0, 1)
+            >>> td_flat.batch_size
+            torch.Size([12])
+            >>> td_flat["a"]
+            tensor([[ 0,  1,  2,  3,  4],
+                    [ 5,  6,  7,  8,  9],
+                    [10, 11, 12, 13, 14],
+                    [15, 16, 17, 18, 19],
+                    [20, 21, 22, 23, 24],
+                    [25, 26, 27, 28, 29],
+                    [30, 31, 32, 33, 34],
+                    [35, 36, 37, 38, 39],
+                    [40, 41, 42, 43, 44],
+                    [45, 46, 47, 48, 49],
+                    [50, 51, 52, 53, 54],
+                    [55, 56, 57, 58, 59]])
+            >>> td_flat["b"]
+            tensor([ 0,  1,  2,  3,  4,  5,  6,  7,  8,  9, 10, 11])
+
+        """
+        if end_dim < 0:
+            end_dim = self.ndim + end_dim
+            if end_dim < 0:
+                raise ValueError(
+                    f"Incompatible end_dim {end_dim} for tensordict with shape {self.shape}."
+                )
+        if end_dim <= start_dim:
+            raise ValueError(
+                "The end dimension must be strictly greater than the start dim."
+            )
+
+        def flatten(tensor):
+            return torch.flatten(tensor, start_dim, end_dim)
+
+        nelt = prod(self.batch_size[start_dim : end_dim + 1])
+        if start_dim > 0:
+            batch_size = (
+                list(self.batch_size)[:start_dim]
+                + [nelt]
+                + list(self.batch_size[end_dim + 1 :])
+            )
+        else:
+            batch_size = [nelt] + list(self.batch_size[end_dim + 1 :])
+        out = self.apply(flatten, batch_size=batch_size)
+        if self._names is not None:
+            names = [
+                name
+                for i, name in enumerate(self._names)
+                if (i < start_dim or i > end_dim)
+            ]
+            names.insert(start_dim, None)
+            out.names = names
+        return out
+
+    def unflatten(self, dim, unflattened_size):
+        """Unflattens a tensordict dim expanding it to a desired shape.
+
+        Args:
+            dim (int): specifies the dimension of the input tensor to be unflattened.
+            unflattened_size (shape): is the new shape of the unflattened dimension of the tensordict.
+
+        Examples:
+            >>> td = TensorDict({"a": torch.arange(60).view(3, 4, 5), "b": torch.arange(12).view(3, 4)}, [3, 4])
+            >>> td_flat = td.flatten(0, 1)
+            >>> td_unflat = td_flat.unflatten(0, [3, 4])
+            >>> assert (td == td_unflat).all()
+        """
+        if dim < 0:
+            dim = self.ndim + dim
+            if dim < 0:
+                raise ValueError(
+                    f"Incompatible dim {dim} for tensordict with shape {self.shape}."
+                )
+
+        def unflatten(tensor):
+            return torch.unflatten(
+                tensor,
+                dim,
+                unflattened_size,
+            )
+
+        if dim > 0:
+            batch_size = (
+                list(self.batch_size)[:dim]
+                + list(unflattened_size)
+                + list(self.batch_size[dim + 1 :])
+            )
+        else:
+            batch_size = list(unflattened_size) + list(self.batch_size[1:])
+        out = self.apply(unflatten, batch_size=batch_size)
+        if self._names is not None:
+            names = copy(self._names)
+            for _ in range(len(unflattened_size) - 1):
+                names.insert(dim, None)
+            out.names = names
+        return out
+
     def __bool__(self) -> bool:
         raise ValueError("Converting a tensordict to boolean value is not permitted")
 
     def __ne__(self, other: object) -> TensorDictBase:
         """XOR operation over two tensordicts, for evey key.
 
         The two tensordicts must have the same key set.
@@ -1448,15 +1789,15 @@
 
         Returns:
             a new TensorDict instance with all tensors are boolean
             tensors of the same shape as the original tensors.
 
         """
         # avoiding circular imports
-        from tensordict.prototype import is_tensorclass
+        from tensordict.tensorclass import is_tensorclass
 
         if is_tensorclass(other):
             return other != self
         if isinstance(other, (dict,)) or is_tensor_collection(other):
             keys1 = set(self.keys())
             keys2 = set(other.keys())
             if len(keys1.difference(keys2)) or len(keys1) != len(keys2):
@@ -1480,15 +1821,15 @@
 
         Returns:
             a new TensorDict instance with all tensors are boolean
             tensors of the same shape as the original tensors.
 
         """
         # avoiding circular imports
-        from tensordict.prototype import is_tensorclass
+        from tensordict.tensorclass import is_tensorclass
 
         if is_tensorclass(other):
             return other == self
         if isinstance(other, (dict,)) or is_tensor_collection(other):
             keys1 = set(self.keys())
             keys2 = set(other.keys())
             if len(keys1.difference(keys2)) or len(keys1) != len(keys2):
@@ -1558,15 +1899,15 @@
     @abc.abstractmethod
     def set_at_(
         self, key: NestedKey, value: CompatibleType, idx: IndexType
     ) -> TensorDictBase:
         """Sets the values in-place at the index indicated by :obj:`idx`.
 
         Args:
-            key (str): key to be modified.
+            key (str, tuple of str): key to be modified.
             value (torch.Tensor): value to be set at the index `idx`
             idx (int, tensor or tuple): index where to write the values.
 
         Returns:
             self
 
         """
@@ -1577,32 +1918,35 @@
         return self.update_(tensordict)
 
     def copy_at_(self, tensordict: TensorDictBase, idx: IndexType) -> TensorDictBase:
         """See :obj:`TensorDictBase.update_at_`."""
         return self.update_at_(tensordict, idx)
 
     def get_at(
-        self, key: str, idx: IndexType, default: CompatibleType = "_no_default_"
+        self, key: NestedKey, idx: IndexType, default: CompatibleType = NO_DEFAULT
     ) -> CompatibleType:
         """Get the value of a tensordict from the key `key` at the index `idx`.
 
         Args:
-            key (str): key to be retrieved.
+            key (str, tuple of str): key to be retrieved.
             idx (int, slice, torch.Tensor, iterable): index of the tensor.
             default (torch.Tensor): default value to return if the key is
                 not present in the tensordict.
 
         Returns:
             indexed tensor.
 
         """
-        value = self.get(key, default=default)
-        if value is not default:
-            return value[idx]
-        return value
+        # TODO: this is NOT explicitely tested. Make a test
+        try:
+            return self.get(key, NO_DEFAULT)[idx]
+        except KeyError:
+            if default is NO_DEFAULT:
+                raise
+            return default
 
     @abc.abstractmethod
     def share_memory_(self) -> TensorDictBase:
         """Places all the tensors in shared memory.
 
         The TensorDict is then locked, meaning that the only writing operations that
         can be executed must be done in-place.
@@ -1668,15 +2012,17 @@
                 prefix / "meta.pt",
             )
         if not self.keys():
             raise Exception(
                 "memmap_like() must be called when the TensorDict is (partially) "
                 "populated. Set a tensor first."
             )
-        tensordict = TensorDict({}, self.batch_size, device=self.device)
+        tensordict = TensorDict(
+            {}, self.batch_size, device=self.device, names=self._names
+        )
         for key, value in self.items():
             if is_tensor_collection(value):
                 if prefix is not None:
                     # ensure subdirectory exists
                     (prefix / key).mkdir(exist_ok=True)
                     tensordict[key] = value.memmap_like(
                         prefix=prefix / key,
@@ -1725,17 +2071,74 @@
             a new tensordict with no tensor requiring gradient.
 
         """
         return TensorDict(
             {key: item.detach() for key, item in self.items()},
             batch_size=self.batch_size,
             device=self.device,
+            names=self._names,
             _run_checks=False,
         )
 
+    def to_h5(
+        self,
+        filename,
+        **kwargs,
+    ):
+        """Converts a tensordict to a PersistentTensorDict with the h5 backend.
+
+        Args:
+            filename (str or path): path to the h5 file.
+            device (torch.device or compatible, optional): the device where to
+                expect the tensor once they are returned. Defaults to ``None``
+                (on cpu by default).
+            **kwargs: kwargs to be passed to :meth:`h5py.File.create_dataset`.
+
+        Returns:
+            A :class:`PersitentTensorDict` instance linked to the newly created file.
+
+        Examples:
+            >>> import tempfile
+            >>> import timeit
+            >>>
+            >>> from tensordict import TensorDict, MemmapTensor
+            >>> td = TensorDict({
+            ...     "a": MemmapTensor(1_000_000),
+            ...     "b": {"c": MemmapTensor(1_000_000, 3)},
+            ... }, [1_000_000])
+            >>>
+            >>> file = tempfile.NamedTemporaryFile()
+            >>> td_h5 = td.to_h5(file.name, compression="gzip", compression_opts=9)
+            >>> print(td_h5)
+            PersistentTensorDict(
+                fields={
+                    a: Tensor(shape=torch.Size([1000000]), device=cpu, dtype=torch.float32, is_shared=False),
+                    b: PersistentTensorDict(
+                        fields={
+                            c: Tensor(shape=torch.Size([1000000, 3]), device=cpu, dtype=torch.float32, is_shared=False)},
+                        batch_size=torch.Size([1000000]),
+                        device=None,
+                        is_shared=False)},
+                batch_size=torch.Size([1000000]),
+                device=None,
+                is_shared=False)
+
+
+        """
+        from .persistent import PersistentTensorDict
+
+        out = PersistentTensorDict.from_dict(
+            self,
+            filename=filename,
+            **kwargs,
+        )
+        if self._names is not None:
+            out.names = self._names
+        return out
+
     def to_tensordict(self):
         """Returns a regular TensorDict instance from the TensorDictBase.
 
         Returns:
             a new TensorDict object containing the same values.
 
         """
@@ -1744,14 +2147,15 @@
                 key: value.clone()
                 if not is_tensor_collection(value)
                 else value.to_tensordict()
                 for key, value in self.items()
             },
             device=self.device,
             batch_size=self.batch_size,
+            names=self._names,
         )
 
     def zero_(self) -> TensorDictBase:
         """Zeros all tensors in the tensordict in-place."""
         for key in self.keys():
             self.fill_(key, 0)
         return self
@@ -1765,22 +2169,29 @@
         idx = [
             ((*tuple(slice(None) for _ in range(dim)), i))
             for i in range(self.shape[dim])
         ]
         if dim < 0:
             dim = self.batch_dims + dim
         batch_size = torch.Size([s for i, s in enumerate(self.batch_size) if i != dim])
+        names = self._names
+        if names is not None:
+            names = copy(names)
+            names = [name for i, name in enumerate(names) if i != dim]
         out = []
         for _idx in idx:
             out.append(
                 self.apply(
                     lambda tensor, idx=_idx: tensor[idx],
                     batch_size=batch_size,
                 )
             )
+            if names is not None:
+                for item in out:
+                    item.names = names
             if self.is_shared():
                 out[-1].share_memory_()
             elif self.is_memmap():
                 out[-1].memmap_()
         return tuple(out)
 
     def chunk(self, chunks: int, dim: int = 0) -> tuple[TensorDictBase, ...]:
@@ -1820,14 +2231,15 @@
                 TensorDict will be copied too. Default is `True`.
 
         """
         return TensorDict(
             source={key: _clone_value(value, recurse) for key, value in self.items()},
             batch_size=self.batch_size,
             device=self.device,
+            names=copy(self._names),
             _run_checks=False,
             _is_shared=self.is_shared() if not recurse else False,
             _is_memmap=self.is_memmap() if not recurse else False,
         )
 
     @classmethod
     def __torch_function__(
@@ -1955,15 +2367,18 @@
             while mask.ndimension() > self.batch_dims:
                 mask_expand = mask.squeeze(-1)
             else:
                 mask_expand = mask
             value_select = value[mask_expand]
             d[key] = value_select
         dim = int(mask.sum().item())
-        return TensorDict(device=self.device, source=d, batch_size=torch.Size([dim]))
+        other_dim = self.shape[mask.ndim :]
+        return TensorDict(
+            device=self.device, source=d, batch_size=torch.Size([dim, *other_dim])
+        )
 
     @abc.abstractmethod
     def is_contiguous(self) -> bool:
         """Returns a boolean indicating if all the tensors are contiguous."""
         raise NotImplementedError
 
     @abc.abstractmethod
@@ -2056,31 +2471,31 @@
             size: iterable
 
         Returns:
             A TensorDict with reshaped keys
 
         """
         if len(shape) == 0 and size is not None:
-            return self.view(*size)
+            return self.reshape(*size)
         elif len(shape) == 1 and isinstance(shape[0], (list, tuple, torch.Size)):
-            return self.view(*shape[0])
+            return self.reshape(*shape[0])
         elif not isinstance(shape, torch.Size):
             shape = torch.Size(shape)
 
         d = {}
         for key, item in self.items():
-            d[key] = item.reshape(*shape, *item.shape[self.ndimension() :])
+            d[key] = item.reshape((*shape, *item.shape[self.ndimension() :]))
         if d:
             batch_size = d[key].shape[: len(shape)]
         else:
             if any(not isinstance(i, int) or i < 0 for i in shape):
                 raise RuntimeError(
                     "Implicit reshaping is not permitted with empty " "tensordicts"
                 )
-            batch_size = shape
+            batch_size = torch.Size(shape)
         return TensorDict(d, batch_size, device=self.device, _run_checks=False)
 
     def split(self, split_size: int | list[int], dim: int = 0) -> list[TensorDictBase]:
         """Splits each tensor in the TensorDict with the specified size in the given dimension, like `torch.split`.
 
         Returns a list of TensorDict with the view of split chunks of items. Nested TensorDicts will remain nested.
 
@@ -2101,54 +2516,64 @@
             raise IndexError(
                 f"Dimension out of range (expected to be in range of [-{self.batch_dims}, {self.batch_dims - 1}], but got {dim})"
             )
         if dim < 0:
             dim += self.batch_dims
         if isinstance(split_size, int):
             rep, remainder = divmod(self.batch_size[dim], split_size)
-            rep_shape = [
-                split_size if idx == dim else size
-                for (idx, size) in enumerate(self.batch_size)
-            ]
+            rep_shape = torch.Size(
+                [
+                    split_size if idx == dim else size
+                    for (idx, size) in enumerate(self.batch_size)
+                ]
+            )
             batch_sizes = [rep_shape for _ in range(rep)]
             if remainder:
                 batch_sizes.append(
-                    [
-                        remainder if dim_idx == dim else dim_size
-                        for (dim_idx, dim_size) in enumerate(self.batch_size)
-                    ]
+                    torch.Size(
+                        [
+                            remainder if dim_idx == dim else dim_size
+                            for (dim_idx, dim_size) in enumerate(self.batch_size)
+                        ]
+                    )
                 )
         elif isinstance(split_size, list) and all(
             isinstance(element, int) for element in split_size
         ):
             if sum(split_size) != self.batch_size[dim]:
                 raise RuntimeError(
                     f"Split method expects split_size to sum exactly to {self.batch_size[dim]} (tensor's size at dimension {dim}), but got split_size={split_size}"
                 )
             for i in split_size:
                 batch_sizes.append(
-                    [
-                        i if dim_idx == dim else dim_size
-                        for (dim_idx, dim_size) in enumerate(self.batch_size)
-                    ]
+                    torch.Size(
+                        [
+                            i if dim_idx == dim else dim_size
+                            for (dim_idx, dim_size) in enumerate(self.batch_size)
+                        ]
+                    )
                 )
         else:
             raise TypeError(
                 "split(): argument 'split_size' must be int or list of ints"
             )
         dictionaries = [{} for _ in range(len(batch_sizes))]
         for key, item in self.items():
             split_tensors = torch.split(item, split_size, dim)
             for idx, split_tensor in enumerate(split_tensors):
                 dictionaries[idx][key] = split_tensor
+        names = self._names
+        if names is not None:
+            names = copy(names)
         return [
             TensorDict(
                 dictionaries[i],
                 batch_sizes[i],
                 device=self.device,
+                names=names,
                 _run_checks=False,
                 _is_shared=self.is_shared(),
                 _is_memmap=self.is_memmap(),
             )
             for i in range(len(dictionaries))
         ]
 
@@ -2183,14 +2608,21 @@
                         batch_size=torch.Size([3, 2, 5]),
                         device=None,
                         is_shared=False)},
                 batch_size=torch.Size([3, 2]),
                 device=None,
                 is_shared=False)
 
+        Gather keeps the dimension names.
+
+        Examples:
+            >>> td.names = ["a", "b"]
+            >>> td_gather = td.gather(dim=1, index=index)
+            >>> td_gather.names
+            ["a", "b"]
         """
         return torch.gather(self, dim, index, out=out)
 
     def view(
         self,
         *shape: int,
         size: list | tuple | torch.Size | None = None,
@@ -2333,18 +2765,25 @@
             raise RuntimeError(
                 "dim must be greater than or equal to -tensordict.batch_dims and "
                 "smaller than tensordict.batch_dims"
             )
         if dim is not None:
             if dim < 0:
                 dim = self.batch_dims + dim
+
+            names = self._names
+            if names is not None:
+                names = copy(names)
+                names = [name for i, name in enumerate(names) if i != dim]
+
             return TensorDict(
                 source={key: value.all(dim=dim) for key, value in self.items()},
                 batch_size=[b for i, b in enumerate(self.batch_size) if i != dim],
                 device=self.device,
+                names=names,
             )
         return all(value.all() for value in self.values())
 
     def any(self, dim: int = None) -> bool | TensorDictBase:
         """Checks if any value is True/non-null in the tensordict.
 
         Args:
@@ -2359,18 +2798,25 @@
             raise RuntimeError(
                 "dim must be greater than or equal to -tensordict.batch_dims and "
                 "smaller than tensordict.batch_dims"
             )
         if dim is not None:
             if dim < 0:
                 dim = self.batch_dims + dim
+
+            names = self._names
+            if names is not None:
+                names = copy(names)
+                names = [name for i, name in enumerate(names) if i != dim]
+
             return TensorDict(
                 source={key: value.any(dim=dim) for key, value in self.items()},
                 batch_size=[b for i, b in enumerate(self.batch_size) if i != dim],
                 device=self.device,
+                names=names,
             )
         return any([value.any() for value in self.values()])
 
     def get_sub_tensordict(self, idx: IndexType) -> TensorDictBase:
         """Returns a SubTensorDict with the desired index."""
         return SubTensorDict(source=self, idx=idx)
 
@@ -2485,19 +2931,64 @@
         # direct the user to use TensorDict.keys() instead
         raise NotImplementedError(
             "TensorDict does not support membership checks with the `in` keyword. If "
             "you want to check if a particular key is in your TensorDict, please use "
             "`key in tensordict.keys()` instead."
         )
 
+    def _get_names_idx(self, idx):
+        if self._names is None:
+            names = None
+        else:
+
+            def is_boolean(idx):
+                if isinstance(idx, tuple) and len(idx) == 1:
+                    return is_boolean(idx[0])
+                if hasattr(idx, "dtype") and idx.dtype is torch.bool:
+                    return idx.ndim
+                return None
+
+            num_boolean_dim = is_boolean(idx)
+            if num_boolean_dim:
+                names = [None] + self._names[num_boolean_dim:]
+            else:
+
+                def is_int(subidx):
+                    if isinstance(subidx, Number):
+                        return True
+                    if isinstance(subidx, Tensor) and len(subidx.shape) == 0:
+                        return True
+                    return False
+
+                if not isinstance(idx, tuple):
+                    idx = (idx,)
+                if len(idx) < self.ndim:
+                    idx = (*idx, Ellipsis)
+                idx_names = convert_ellipsis_to_idx(idx, self.batch_size)
+                # this will convert a [None, :, :, 0, None, 0] in [None, 0, 1, None, 3]
+                count = 0
+                idx_to_take = []
+                for _idx in idx_names:
+                    if _idx is None:
+                        idx_to_take.append(None)
+                    elif _is_number(_idx):
+                        count += 1
+                    else:
+                        idx_to_take.append(count)
+                        count += 1
+                names = [self._names[i] if i is not None else None for i in idx_to_take]
+        return names
+
     def _index_tensordict(self, idx: IndexType) -> TensorDictBase:
+        names = self._get_names_idx(idx)
         return TensorDict(
             source={key: _get_item(item, idx) for key, item in self.items()},
             batch_size=_getitem_batch_size(self.batch_size, idx),
             device=self.device,
+            names=names,
             _run_checks=False,
             _is_shared=self.is_shared(),
             _is_memmap=self.is_memmap(),
         )
 
     def __getitem__(self, idx: IndexType) -> TensorDictBase:
         """Indexes all tensors according to the provided index.
@@ -2515,25 +3006,27 @@
             >>> subtd.set("a", torch.ones(1,4,5))
             >>> print(td.get("a"))  # first row is full of 1
             >>> # Warning: this will not work as expected
             >>> subtd.get("a")[:] = 2.0
             >>> print(td.get("a"))  # values have not changed
 
         """
+        if isinstance(idx, tuple) and len(idx) == 1:
+            idx = idx[0]
         if isinstance(idx, str) or (
             isinstance(idx, tuple) and all(isinstance(sub_idx, str) for sub_idx in idx)
         ):
             return self.get(idx)
 
         if not self.batch_size:
             raise RuntimeError(
                 "indexing a tensordict with td.batch_dims==0 is not permitted"
             )
 
-        if isinstance(idx, Number):
+        if _is_number(idx):
             return self._index_tensordict((idx,))
 
         if isinstance(idx, list):
             idx = torch.tensor(idx, device=self.device)
             return self._index_tensordict(idx)
 
         if isinstance(idx, np.ndarray):
@@ -2618,19 +3111,23 @@
         if isinstance(value, (TensorDictBase, dict)):
             indexed_bs = _getitem_batch_size(self.batch_size, index)
             if isinstance(value, dict):
                 value = TensorDict(
                     value, batch_size=indexed_bs, device=self.device, _run_checks=False
                 )
             if value.batch_size != indexed_bs:
-                raise RuntimeError(
-                    f"indexed destination TensorDict batch size is {indexed_bs} "
-                    f"(batch_size = {self.batch_size}, index={index}), "
-                    f"which differs from the source batch size {value.batch_size}"
-                )
+                # try to expand
+                try:
+                    value = value.expand(indexed_bs)
+                except RuntimeError as err:
+                    raise RuntimeError(
+                        f"indexed destination TensorDict batch size is {indexed_bs} "
+                        f"(batch_size = {self.batch_size}, index={index}), "
+                        f"which differs from the source batch size {value.batch_size}"
+                    ) from err
 
             keys = set(self.keys())
             if not all(key in keys for key in value.keys()):
                 subtd = self.get_sub_tensordict(index)
             for key, item in value.items():
                 if key in keys:
                     self.set_at_(key, item, index)
@@ -2642,15 +3139,15 @@
 
     def __delitem__(self, index: IndexType) -> TensorDictBase:
         # if isinstance(index, str):
         return self.del_(index)
         # raise IndexError(f"Index has to a string but received {index}.")
 
     @abc.abstractmethod
-    def rename_key(
+    def rename_key_(
         self, old_key: str, new_key: str, safe: bool = False
     ) -> TensorDictBase:
         """Renames a key with a new string.
 
         Args:
             old_key (str): key to be renamed
             new_key (str): new name
@@ -2689,20 +3186,14 @@
         return self.select()
 
     def is_empty(self) -> bool:
         for _ in self.keys():
             return False
         return True
 
-    def set_default(
-        self, key: NestedKey, default: CompatibleType, inplace: bool = False
-    ) -> CompatibleType:
-        warn("set_default has been deprecated. Use setdefault instead")
-        return self.setdefault(key, default, inplace=inplace)
-
     def setdefault(
         self, key: NestedKey, default: CompatibleType, inplace: bool = False
     ) -> CompatibleType:
         """Insert key with a value of default if key is not in the dictionary.
 
         Return the value for key if key is in the dictionary, else default.
 
@@ -2812,14 +3303,18 @@
         batch_size (iterable of int, optional): a batch size for the
             tensordict. The batch size is immutable and can only be modified
             by calling operations that create a new TensorDict. Unless the
             source is another TensorDict, the batch_size argument must be
             provided as it won't be inferred from the data.
         device (torch.device or compatible type, optional): a device for the
             TensorDict.
+        names (lsit of str, optional): the names of the dimensions of the
+            tensordict. If provided, its length must match the one of the
+            ``batch_size``. Defaults to ``None`` (no dimension name, or ``None``
+            for every dimension).
 
     Examples:
         >>> import torch
         >>> from tensordict import TensorDict
         >>> source = {'random': torch.randn(3, 4),
         ...     'zeros': torch.zeros(3, 4, 5)}
         >>> batch_size = [3]
@@ -2834,94 +3329,190 @@
         >>> print(td_unqueeze.view(-1).shape)
         torch.Size([3])
         >>> print((td.clone()==td).all())
         True
 
     """
 
+    __slots__ = (
+        "_tensordict",
+        "_batch_size",
+        "_is_shared",
+        "_is_memmap",
+        "_device",
+        "_is_locked",
+        "_names",
+    )
+
     def __new__(cls, *args: Any, **kwargs: Any) -> TensorDict:
         cls._is_shared = False
         cls._is_memmap = False
+        cls._names = None
         return super().__new__(cls, *args, _safe=True, _lazy=False, **kwargs)
 
     def __init__(
         self,
         source: TensorDictBase | dict[str, CompatibleType],
         batch_size: Sequence[int] | torch.Size | int | None = None,
         device: DeviceType | None = None,
+        names: Sequence[str] | None = None,
         _run_checks: bool = True,
         _is_shared: bool | None = False,
         _is_memmap: bool | None = False,
     ) -> None:
         self._is_shared = _is_shared
         self._is_memmap = _is_memmap
         if device is not None:
             device = torch.device(device)
         self._device = device
 
         if not _run_checks:
-            if isinstance(source, dict):
-                self._tensordict: dict = copy(source)
-            else:
-                self._tensordict: dict = dict(source)
-            self._batch_size = torch.Size(batch_size)
+            self._tensordict: dict = dict(source)
+            self._batch_size = batch_size
             upd_dict = {}
             for key, value in self._tensordict.items():
                 if isinstance(value, dict):
                     value = TensorDict(
                         value,
                         batch_size=self._batch_size,
                         device=self._device,
                         _run_checks=_run_checks,
                         _is_shared=_is_shared,
                         _is_memmap=_is_memmap,
                     )
                     upd_dict[key] = value
             if upd_dict:
                 self._tensordict.update(upd_dict)
+            self._names = names
         else:
             self._tensordict = {}
             if not isinstance(source, (TensorDictBase, dict)):
                 raise ValueError(
                     "A TensorDict source is expected to be a TensorDictBase "
                     f"sub-type or a dictionary, found type(source)={type(source)}."
                 )
             self._batch_size = self._parse_batch_size(source, batch_size)
 
+            self.names = names
+
             if source is not None:
                 for key, value in source.items():
                     self.set(key, value)
 
+    @classmethod
+    def from_dict(cls, input_dict, batch_size=None, device=None):
+        """Returns a TensorDict created from a dictionary or another :class:`TensorDict`.
+
+        If ``batch_size`` is not specified, returns the maximum batch size possible.
+
+        This function works on nested dictionaries too, or can be used to determine the
+        batch-size of a nested tensordict.
+
+        Args:
+            input_dict (dictionary, optional): a dictionary to use as a data source
+                (nested keys compatible).
+            batch_size (iterable of int, optional): a batch size for the tensordict.
+            device (torch.device or compatible type, optional): a device for the TensorDict.
+
+        Examples:
+            >>> input_dict = {"a": torch.randn(3, 4), "b": torch.randn(3)}
+            >>> print(TensorDict.from_dict(input_dict))
+            TensorDict(
+                fields={
+                    a: Tensor(shape=torch.Size([3, 4]), device=cpu, dtype=torch.float32, is_shared=False),
+                    b: Tensor(shape=torch.Size([3]), device=cpu, dtype=torch.float32, is_shared=False)},
+                batch_size=torch.Size([3]),
+                device=None,
+                is_shared=False)
+            >>> # nested dict: the nested TensorDict can have a different batch-size
+            >>> # as long as its leading dims match.
+            >>> input_dict = {"a": torch.randn(3), "b": {"c": torch.randn(3, 4)}}
+            >>> print(TensorDict.from_dict(input_dict))
+            TensorDict(
+                fields={
+                    a: Tensor(shape=torch.Size([3]), device=cpu, dtype=torch.float32, is_shared=False),
+                    b: TensorDict(
+                        fields={
+                            c: Tensor(shape=torch.Size([3, 4]), device=cpu, dtype=torch.float32, is_shared=False)},
+                        batch_size=torch.Size([3, 4]),
+                        device=None,
+                        is_shared=False)},
+                batch_size=torch.Size([3]),
+                device=None,
+                is_shared=False)
+            >>> # we can also use this to work out the batch sie of a tensordict
+            >>> input_td = TensorDict({"a": torch.randn(3), "b": {"c": torch.randn(3, 4)}}, [])
+            >>> print(TensorDict.from_dict(input_td))
+            TensorDict(
+                fields={
+                    a: Tensor(shape=torch.Size([3]), device=cpu, dtype=torch.float32, is_shared=False),
+                    b: TensorDict(
+                        fields={
+                            c: Tensor(shape=torch.Size([3, 4]), device=cpu, dtype=torch.float32, is_shared=False)},
+                        batch_size=torch.Size([3, 4]),
+                        device=None,
+                        is_shared=False)},
+                batch_size=torch.Size([3]),
+                device=None,
+                is_shared=False)
+
+        """
+        batch_size_set = [] if batch_size is None else batch_size
+        for key, value in list(input_dict.items()):
+            if isinstance(value, (dict,)):
+                input_dict[key] = TensorDict(value, batch_size_set, device=device)
+        # _run_checks=False breaks because a tensor may have the same batch-size as the tensordict
+        out = cls(
+            input_dict,
+            batch_size=batch_size_set,
+            device=device,
+        )
+        if batch_size is None:
+            _set_max_batch_size(out)
+        else:
+            out.batch_size = batch_size
+        return out
+
     @staticmethod
     def _parse_batch_size(
         source: TensorDictBase | dict,
         batch_size: Sequence[int] | torch.Size | int | None = None,
     ) -> torch.Size:
-        if isinstance(batch_size, Sequence):
+        try:
             return torch.Size(batch_size)
-        elif isinstance(batch_size, Number):
-            return torch.Size([batch_size])
-        elif isinstance(source, TensorDictBase):
-            return source.batch_size
-        raise ValueError(
-            "batch size was not specified when creating the TensorDict "
-            "instance and it could not be retrieved from source."
-        )
+        except Exception as err:
+            if isinstance(batch_size, Number):
+                return torch.Size([batch_size])
+            elif isinstance(source, TensorDictBase):
+                return source.batch_size
+            raise ValueError(
+                "batch size was not specified when creating the TensorDict "
+                "instance and it could not be retrieved from source."
+            ) from err
 
     @property
     def batch_dims(self) -> int:
         return len(self.batch_size)
 
     @batch_dims.setter
     def batch_dims(self, value: int) -> None:
         raise RuntimeError(
             f"Setting batch dims on {self.__class__.__name__} instances is "
             f"not allowed."
         )
 
+    def _rename_subtds(self, names):
+        if names is None:
+            names = [None] * self.ndim
+        for item in self._tensordict.values():
+            if is_tensor_collection(item):
+                item_names = item.names
+                td_names = list(names) + item_names[len(names) :]
+                item.rename_(*td_names)
+
     @property
     def device(self) -> torch.device | None:
         """Device of the tensordict.
 
         Returns `None` if device hasn't been provided in the constructor or set via `tensordict.to(device)`.
 
         """
@@ -2984,20 +3575,23 @@
             raise RuntimeError(
                 f"TensorDict.device is {self._device}, but elements have "
                 f"device values {devices}. If TensorDict.device is set then "
                 "all elements must share that device."
             )
 
     def _index_tensordict(self, idx: IndexType) -> TensorDictBase:
+        names = self._get_names_idx(idx)
         self_copy = copy(self)
+        # self_copy = self.clone(False)
         self_copy._tensordict = {
             key: _get_item(item, idx) for key, item in self.items()
         }
         self_copy._batch_size = _getitem_batch_size(self_copy.batch_size, idx)
         self_copy._device = self.device
+        self_copy.names = names
         return self_copy
 
     def pin_memory(self) -> TensorDictBase:
         def pin_mem(tensor):
             return tensor.pin_memory()
 
         return self.apply(pin_mem)
@@ -3036,20 +3630,23 @@
         for key, value in self.items():
             tensor_dims = len(value.shape)
             last_n_dims = tensor_dims - tensordict_dims
             if last_n_dims > 0:
                 d[key] = value.expand(*shape, *value.shape[-last_n_dims:])
             else:
                 d[key] = value.expand(*shape)
-        return TensorDict(
+        out = TensorDict(
             source=d,
-            batch_size=[*shape],
+            batch_size=torch.Size(shape),
             device=self.device,
             _run_checks=False,
         )
+        if self._names is not None:
+            out.refine_names(..., *self.names)
+        return out
 
     def _set(self, key: str, value, inplace: bool = False) -> TensorDictBase:
         if isinstance(key, tuple):
             td, subkey = _get_leaf_tensordict(
                 self, key, _default_hook if not inplace else None
             )
         else:
@@ -3060,16 +3657,15 @@
             except KeyError as err:
                 raise err
             except Exception as err:
                 raise ValueError(
                     f"Failed to update '{subkey}' in tensordict {td}"
                 ) from err
         else:
-            if td._tensordict.get(subkey, None) is not value:
-                td._tensordict[subkey] = value
+            td._tensordict[subkey] = value
 
         return self
 
     def set(
         self,
         key: NestedKey,
         value: dict[str, CompatibleType] | CompatibleType,
@@ -3210,17 +3806,17 @@
             tensor_in.copy_(value)
         else:
             _set_item(tensor_in, idx, value)
 
         return self
 
     def get(
-        self, key: str, default: str | CompatibleType = "_no_default_"
+        self, key: NestedKey, default: str | CompatibleType = NO_DEFAULT
     ) -> CompatibleType:
-        _nested_key_type_check(key)
+        _nested_key_check(key)
 
         try:
             if isinstance(key, tuple):
                 if len(key) > 1:
                     first_lev = self.get(key[0])
                     if len(key) == 2 and isinstance(first_lev, KeyedJaggedTensor):
                         return first_lev[key[1]]
@@ -3382,25 +3978,28 @@
         return out
 
     def to(self, dest: DeviceType | torch.Size | type, **kwargs: Any) -> TensorDictBase:
         if isinstance(dest, type) and issubclass(dest, TensorDictBase):
             if isinstance(self, dest):
                 return self
             td = dest(source=self, **kwargs)
+            if self._names is not None:
+                td.names = self._names
             return td
         elif isinstance(dest, (torch.device, str, int)):
             # must be device
             dest = torch.device(dest)
             if self.device is not None and dest == self.device:
                 return self
 
             self_copy = TensorDict(
                 {key: value.to(dest, **kwargs) for key, value in self.items()},
                 batch_size=self.batch_size,
                 device=dest,
+                names=self._names,
             )
             return self_copy
         elif isinstance(dest, torch.Size):
             self.batch_size = dest
             return self
         else:
             raise NotImplementedError(
@@ -3455,14 +4054,15 @@
                         *val, strict=strict, inplace=inplace
                     )
 
         out = TensorDict(
             device=self.device,
             batch_size=self.batch_size,
             source=source,
+            names=self._names,
             _run_checks=False,
             _is_memmap=self._is_memmap,
             _is_shared=self._is_shared,
         )
         if inplace:
             self._tensordict = out._tensordict
             return self
@@ -3471,14 +4071,21 @@
     def keys(
         self, include_nested: bool = False, leaves_only: bool = False
     ) -> _TensorDictKeysView:
         return _TensorDictKeysView(
             self, include_nested=include_nested, leaves_only=leaves_only
         )
 
+    def __getstate__(self):
+        return {slot: getattr(self, slot) for slot in self.__slots__}
+
+    def __setstate__(self, state):
+        for slot, value in state.items():
+            setattr(self, slot, value)
+
 
 class _ErrorInteceptor:
     """Context manager for catching errors and modifying message.
 
     Intended for use with stacking / concatenation operations applied to TensorDicts.
 
     """
@@ -3652,17 +4259,21 @@
         target_shape = list(tensor.shape)
         target_shape[dim] = index_expand.shape[dim]
         index_expand = index_expand.expand(target_shape)
         out = torch.gather(tensor, dim, index_expand, out=dest)
         return out
 
     if out is None:
+
+        names = input._names
+
         return TensorDict(
             {key: _gather_tensor(value) for key, value in input.items()},
             batch_size=index.shape,
+            names=names,
         )
     TensorDict(
         {key: _gather_tensor(value, out[key]) for key, value in input.items()},
         batch_size=index.shape,
     )
     return out
 
@@ -3746,21 +4357,18 @@
     list_of_tensordicts: Sequence[TensorDictBase],
     dim: int = 0,
     device: DeviceType | None = None,
     out: TensorDictBase | None = None,
 ) -> TensorDictBase:
     if not list_of_tensordicts:
         raise RuntimeError("list_of_tensordicts cannot be empty")
-    if dim < 0:
-        raise RuntimeError(
-            f"negative dim in torch.dim(list_of_tensordicts, dim=dim) not "
-            f"allowed, got dim={dim}"
-        )
 
     batch_size = list(list_of_tensordicts[0].batch_size)
+    if dim < 0:
+        dim = len(batch_size) + dim
     if dim >= len(batch_size):
         raise RuntimeError(
             f"dim must be in the range 0 <= dim < len(batch_size), got dim"
             f"={dim} and batch_size={batch_size}"
         )
     batch_size[dim] = sum([td.batch_size[dim] for td in list_of_tensordicts])
     batch_size = torch.Size(batch_size)
@@ -3778,15 +4386,18 @@
             device = list_of_tensordicts[0].device
             for td in list_of_tensordicts[1:]:
                 if device == td.device:
                     continue
                 else:
                     device = None
                     break
-        return TensorDict(out, device=device, batch_size=batch_size, _run_checks=False)
+        names = list_of_tensordicts[0]._names
+        return TensorDict(
+            out, device=device, batch_size=batch_size, _run_checks=False, names=names
+        )
     else:
         if out.batch_size != batch_size:
             raise RuntimeError(
                 "out.batch_size and cat batch size must match, "
                 f"got out.batch_size={out.batch_size} and batch_size"
                 f"={batch_size}"
             )
@@ -3962,15 +4573,17 @@
     for i in range(len(pad_size)):
         new_batch_size[i // 2] += pad_size[i]
 
     reverse_pad = pad_size[::-1]
     for i in range(0, len(reverse_pad), 2):
         reverse_pad[i], reverse_pad[i + 1] = reverse_pad[i + 1], reverse_pad[i]
 
-    out = TensorDict({}, new_batch_size, device=tensordict.device, _run_checks=False)
+    out = TensorDict(
+        {}, torch.Size(new_batch_size), device=tensordict.device, _run_checks=False
+    )
     for key, tensor in tensordict.items():
         cur_pad = reverse_pad
         if len(pad_size) < len(_shape(tensor)) * 2:
             cur_pad = [0] * (len(_shape(tensor)) * 2 - len(pad_size)) + reverse_pad
 
         if is_tensor_collection(tensor):
             padded = pad(tensor, pad_size, value)
@@ -3983,26 +4596,29 @@
 
 def pad_sequence(
     list_of_tensordicts: Sequence[TensorDictBase],
     batch_first: bool = True,
     padding_value: float = 0.0,
     out: TensorDictBase | None = None,
     device: DeviceType | None = None,
+    return_mask: bool | None = False,
 ) -> TensorDictBase:
     """Pads a list of tensordicts in order for them to be stacked together in a contiguous format.
 
     Args:
         list_of_tensordicts (List[TensorDictBase]): the list of instances to pad and stack.
         batch_first (bool, optional): the ``batch_first`` correspondant of :func:`torch.nn.utils.rnn.pad_sequence`.
             Defaults to ``True``.
         padding_value (number, optional): the padding value. Defaults to ``0.0``.
         out (TensorDictBase, optional): if provided, the destination where the data will be
             written.
         device (device compatible type, optional): if provded, the device where the
             TensorDict output will be created.
+        return_mask (bool, optional): if ``True``, a "mask" entry will be returned.
+            It contains the mask of valid values in the stacked tensordict.
 
     Examples:
         >>> list_td = [
         ...     TensorDict({"a": torch.zeros((3,))}, []),
         ...     TensorDict({"a": torch.zeros((4,))}, []),
         ...     ]
         >>> padded_td = pad_sequence(list_td)
@@ -4013,33 +4629,45 @@
             batch_size=torch.Size([]),
             device=None,
             is_shared=False)
     """
     if not list_of_tensordicts:
         raise RuntimeError("list_of_tensordicts cannot be empty")
     # check that all tensordict match
+    if return_mask:
+        list_of_tensordicts = [
+            td.clone(False).set("mask", torch.ones(td.shape, dtype=torch.bool))
+            for td in list_of_tensordicts
+        ]
     keys = _check_keys(list_of_tensordicts, leaves_only=True, include_nested=True)
-    shape = list_of_tensordicts[0].shape
-    if batch_first:
-        shape = [len(list_of_tensordicts), *shape]
-    elif len(shape):
-        shape = [shape[0], len(list_of_tensordicts), *shape[1:]]
+    shape = max(len(td) for td in list_of_tensordicts)
+    if shape == 0:
+        shape = [
+            len(list_of_tensordicts),
+        ]
+    elif batch_first:
+        shape = [len(list_of_tensordicts), shape]
     else:
-        shape = []
+        shape = [shape, len(list_of_tensordicts)]
     if out is None:
-        out = TensorDict({}, shape, device=device, _run_checks=False)
+        out = TensorDict(
+            {}, batch_size=torch.Size(shape), device=device, _run_checks=False
+        )
         for key in keys:
-            out.set(
-                key,
-                torch.nn.utils.rnn.pad_sequence(
-                    [td.get(key) for td in list_of_tensordicts],
-                    batch_first=batch_first,
-                    padding_value=padding_value,
-                ),
-            )
+            try:
+                out.set(
+                    key,
+                    torch.nn.utils.rnn.pad_sequence(
+                        [td.get(key) for td in list_of_tensordicts],
+                        batch_first=batch_first,
+                        padding_value=padding_value,
+                    ),
+                )
+            except Exception as err:
+                raise RuntimeError(f"pad_sequence failed for key {key}") from err
         return out
     else:
         for key in keys:
             out.set_(
                 key,
                 torch.nn.utils.rnn.pad_sequence(
                     [td.get(key) for td in list_of_tensordicts],
@@ -4125,41 +4753,100 @@
     ) -> None:
         if not isinstance(source, TensorDictBase):
             raise TypeError(
                 f"Expected source to be a subclass of TensorDictBase, "
                 f"got {type(source)}"
             )
         self._source = source
-        idx = (idx,) if not isinstance(idx, (tuple, list, range)) else tuple(idx)
+        idx = (
+            (idx,)
+            if not isinstance(
+                idx,
+                (
+                    tuple,
+                    list,
+                ),
+            )
+            else tuple(idx)
+        )
+        self._batch_size = _getitem_batch_size(self._source.batch_size, idx)
+        if any(item is Ellipsis for item in idx):
+            idx = convert_ellipsis_to_idx(idx, self._source.batch_size)
         self.idx = idx
-        self._batch_size = _getitem_batch_size(self._source.batch_size, self.idx)
+
         if batch_size is not None and batch_size != self.batch_size:
             raise RuntimeError("batch_size does not match self.batch_size.")
 
+    # @staticmethod
+    # def _convert_range(idx):
+    #     return tuple(list(_idx) if isinstance(_idx, range) else _idx for _idx in idx)
+
+    @staticmethod
+    def _convert_ellipsis(idx, shape):
+        if any(_idx is Ellipsis for _idx in idx):
+            new_idx = []
+            cursor = -1
+            for _idx in idx:
+                if _idx is Ellipsis:
+                    if cursor == len(idx) - 1:
+                        # then we can just skip
+                        continue
+                    n_upcoming = len(idx) - cursor - 1
+                    while cursor < len(shape) - n_upcoming:
+                        cursor += 1
+                        new_idx.append(slice(None))
+                else:
+                    new_idx.append(_idx)
+            return tuple(new_idx)
+        return idx
+
     def exclude(self, *keys: str, inplace: bool = False) -> TensorDictBase:
         if inplace:
             return super().exclude(*keys, inplace=True)
         return TensorDict(
             {key: value for key, value in self.items()},
             batch_size=self.batch_size,
             device=self.device,
+            names=self._names,
             _run_checks=False,
             _is_memmap=self.is_memmap(),
             _is_shared=self.is_shared(),
         ).exclude(*keys, inplace=True)
 
     @property
     def batch_size(self) -> torch.Size:
         return self._batch_size
 
     @batch_size.setter
     def batch_size(self, new_size: torch.Size) -> None:
         self._batch_size_setter(new_size)
 
     @property
+    def names(self):
+        names = self._source._get_names_idx(self.idx)
+        if names is None:
+            return [None] * self.batch_dims
+        return names
+
+    @property
+    def _names(self):
+        return self.names
+
+    @names.setter
+    def names(self, value):
+        raise RuntimeError(
+            "Names of a subtensordict cannot be modified. Instantiate the tensordict first."
+        )
+
+    def _rename_subtds(self, names):
+        for key in self.keys():
+            if is_tensor_collection(self.entry_class(key)):
+                raise RuntimeError("Cannot rename nested sub-tensordict dimensions.")
+
+    @property
     def device(self) -> None | torch.device:
         return self._source.device
 
     @device.setter
     def device(self, value: DeviceType) -> None:
         self._source.device = value
 
@@ -4283,17 +4970,20 @@
         self._source._stack_onto_at_(key, list_item, dim=dim, idx=self.idx)
         return self
 
     def to(self, dest: DeviceType | torch.Size | type, **kwargs: Any) -> TensorDictBase:
         if isinstance(dest, type) and issubclass(dest, TensorDictBase):
             if isinstance(self, dest):
                 return self
-            return dest(
+            out = dest(
                 source=self.clone(),
             )
+            if self._names is not None:
+                out.names = self._names
+            return out
         elif isinstance(dest, (torch.device, str, int)):
             dest = torch.device(dest)
             # try:
             if self.device is not None and dest == self.device:
                 return self
             td = self.to_tensordict().to(dest, **kwargs)
             # must be device
@@ -4314,15 +5004,15 @@
         elif self._orig_batch_size == new_size:
             del self._orig_batch_size
         self._batch_size = new_size
 
     def get(
         self,
         key: NestedKey,
-        default: Tensor | str | None = "_no_default_",
+        default: Tensor | str | None = NO_DEFAULT,
     ) -> CompatibleType:
         return self._source.get_at(key, self.idx, default=default)
 
     def set_at_(
         self,
         key: NestedKey,
         value: dict[str, CompatibleType] | CompatibleType,
@@ -4342,15 +5032,15 @@
         return self
 
     def get_at(
         self,
         key: str,
         idx: IndexType,
         discard_idx_attr: bool = False,
-        default: Tensor | str | None = "_no_default_",
+        default: Tensor | str | None = NO_DEFAULT,
     ) -> CompatibleType:
         if not isinstance(idx, tuple):
             idx = (idx,)
         if discard_idx_attr:
             return self._source.get_at(key, idx, default=default)
         else:
             out = self._source.get_at(key, self.idx, default=default)
@@ -4448,92 +5138,41 @@
 
     def clone(self, recurse: bool = True) -> SubTensorDict:
         if not recurse:
             return copy(self)
         return SubTensorDict(source=self._source, idx=self.idx)
 
     def is_contiguous(self) -> bool:
-        return all([value.is_contiguous() for _, value in self.items()])
+        return all(value.is_contiguous() for value in self.values())
 
     def contiguous(self) -> TensorDictBase:
         if self.is_contiguous():
             return self
         return TensorDict(
             batch_size=self.batch_size,
             source={key: value for key, value in self.items()},
             device=self.device,
+            names=self.names,
             _run_checks=False,
         )
 
     def select(
         self, *keys: str, inplace: bool = False, strict: bool = True
     ) -> TensorDictBase:
         if inplace:
             self._source = self._source.select(*keys, strict=strict)
             return self
         return self._source.select(*keys, strict=strict)[self.idx]
 
     def expand(self, *shape: int, inplace: bool = False) -> TensorDictBase:
         if len(shape) == 1 and isinstance(shape[0], Sequence):
             shape = tuple(shape[0])
-
-        idx = self.idx
-        if isinstance(idx, Tensor) and idx.dtype is torch.double:
-            # check that idx is not a mask, otherwise throw an error
-            raise ValueError("Cannot expand a TensorDict masked using SubTensorDict")
-        elif not isinstance(idx, tuple):
-            # create an tuple idx with length equal to this TensorDict's number of dims
-            idx = (idx,) + (slice(None),) * (self._source.ndimension() - 1)
-        elif isinstance(idx, tuple) and len(idx) < self._source.ndimension():
-            # create an tuple idx with length equal to this TensorDict's number of dims
-            idx = idx + (slice(None),) * (self._source.ndimension() - len(idx))
-        # now that idx has the same length as the source's number of dims, we can work with it
-
-        source_shape = self._source.shape
-        num_integer_types = 0
-        for i in idx:
-            if isinstance(i, (int, np.integer)) or (
-                isinstance(i, Tensor) and i.ndimension() == 0
-            ):
-                num_integer_types += 1
-        number_of_extra_dim = len(source_shape) - len(shape) + num_integer_types
-        if number_of_extra_dim > 0:
-            new_source_shape = [shape[i] for i in range(number_of_extra_dim)]
-            shape = shape[len(new_source_shape) :]
-        else:
-            new_source_shape = []
-        new_idx = [slice(None) for _ in range(len(new_source_shape))]
-        for _idx, _s in zip(idx, source_shape):
-            # we're iterating through the source shape and the index
-            # we want to get the new index and the new source shape
-
-            if isinstance(_idx, (int, np.integer)) or (
-                isinstance(_idx, Tensor) and _idx.ndimension() == 0
-            ):
-                # if the index is an integer, do nothing, i.e. keep the index and the shape
-                new_source_shape.append(_s)
-                new_idx.append(_idx)
-            elif _s == 1:
-                # if the source shape at this dim is 1, expand that source dim to the size that is required
-                new_idx.append(slice(None))
-                new_source_shape.append(shape[0])
-                shape = shape[1:]
-            else:
-                # in this case, the source shape must be different than 1. The index is going to be identical.
-                new_idx.append(_idx)
-                new_source_shape.append(shape[0])
-                shape = shape[1:]
-        assert not len(shape)
-        new_source = self._source.expand(*new_source_shape)
-        new_idx = tuple(new_idx)
-        if inplace:
-            self._source = new_source
-            self.idx = new_idx
-            self.batch_size = _getitem_batch_size(new_source_shape, new_idx)
-        return new_source[new_idx]
+        return self.apply(
+            lambda x: x.expand((*shape, *x.shape[self.ndim :])), batch_size=shape
+        )
 
     def is_shared(self) -> bool:
         return self._source.is_shared()
 
     def is_memmap(self) -> bool:
         return self._source.is_memmap()
 
@@ -4623,14 +5262,15 @@
         torch.Size([3, 10, 4])
         >>> print(td_stack[:, 0] is tds[0])
         True
 
     """
 
     def __new__(cls, *args: Any, **kwargs: Any) -> LazyStackedTensorDict:
+        cls._names = None
         return super().__new__(cls, *args, _safe=False, _lazy=True, **kwargs)
 
     def __init__(
         self,
         *tensordicts: TensorDictBase,
         stack_dim: int = 0,
         batch_size: Sequence[int] | None = None,  # TODO: remove
@@ -4700,14 +5340,46 @@
     def batch_size(self) -> torch.Size:
         return self._batch_size
 
     @batch_size.setter
     def batch_size(self, new_size: torch.Size) -> None:
         return self._batch_size_setter(new_size)
 
+    @property
+    def names(self):
+        if self._names is None:
+            names = copy(self.tensordicts[0].names)
+            names.insert(self.stack_dim, None)
+            self._names = names
+        return self._names
+
+    @names.setter
+    def names(self, value):
+        if value is None:
+            for td in self.tensordicts:
+                td.names = None
+            self._names = None
+        else:
+            names_c = list(value)
+            self._names = copy(names_c)
+            name = names_c[self.stack_dim]
+            names_c = list(names_c)
+            del names_c[self.stack_dim]
+            for td in self.tensordicts:
+                if td._check_dim_name(name):
+                    raise ValueError(f"The dimension name {name} is already taken.")
+                td.rename_(*names_c)
+
+    def _rename_subtds(self, names):
+        # remove the name of the stack dim
+        names = list(names)
+        del names[self.stack_dim]
+        for td in self.tensordicts:
+            td.names = names
+
     def is_shared(self) -> bool:
         are_shared = [td.is_shared() for td in self.tensordicts]
         are_shared = [value for value in are_shared if value is not None]
         if not len(are_shared):
             return None
         if any(are_shared) and not all(are_shared):
             raise RuntimeError(
@@ -4765,16 +5437,17 @@
     def set(
         self,
         key: NestedKey,
         tensor: dict[str, CompatibleType] | CompatibleType,
         inplace: bool = False,
     ) -> TensorDictBase:
         key = self._validate_key(key)
-        if self.is_locked:
-            raise RuntimeError(TensorDictBase.LOCK_ERROR)
+        # we don't need this as locked lazy stacks have locked nested tds so the error will be captured in the loop
+        # if self.is_locked:
+        #     raise RuntimeError(TensorDictBase.LOCK_ERROR)
 
         tensor = self._validate_value(tensor)
         for td, _item in zip(self.tensordicts, tensor.unbind(self.stack_dim)):
             td.set(key, _item, inplace=inplace)
 
         first_key = key if (isinstance(key, str)) else key[0]
         if key not in self._valid_keys:
@@ -4803,16 +5476,18 @@
             return tuple(self.tensordicts)
         else:
             return super().unbind(dim)
 
     def set_at_(
         self, key: str, value: dict | CompatibleType, idx: IndexType
     ) -> TensorDictBase:
-        sub_td = self[idx]
-        sub_td.set_(key, value)
+        # this generalizes across all types of indices
+        item = self.get(key)
+        item[idx] = self._validate_value(value, check_shape=False)
+        self.set(key, item, inplace=True)
         return self
 
     def _stack_onto_(
         self,
         key: str,
         list_item: list[CompatibleType],
         dim: int,
@@ -4824,15 +5499,15 @@
             # we must stack and unbind, there is no way to make it more efficient
             self.set_(key, torch.stack(list_item, dim))
         return self
 
     def get(
         self,
         key: NestedKey,
-        default: str | CompatibleType = "_no_default_",
+        default: str | CompatibleType = NO_DEFAULT,
     ) -> CompatibleType:
         # TODO: the stacking logic below works for nested keys, but the key in
         # self.valid_keys check will fail and we'll return the default instead.
         # For now we'll advise user that nested keys aren't supported, but it should be
         # fairly easy to add support if we could add nested keys to valid_keys.
 
         # we can handle the case where the key is a tuple of length 1
@@ -4852,33 +5527,45 @@
             keys = self.valid_keys
 
         if key not in keys:
             return self._default_get(key, default)
 
         tensors = [td.get(key, default=default) for td in self.tensordicts]
         try:
-            return torch.stack(tensors, self.stack_dim)
+            out = torch.stack(tensors, self.stack_dim)
+            if is_tensor_collection(out) and self._names is not None:
+                out.refine_names(*self.names, *out.names[self.ndim :])
+            return out
         except RuntimeError as err:
             if "stack expects each tensor to be equal size" in str(err):
                 shapes = {_shape(tensor) for tensor in tensors}
                 raise RuntimeError(
                     f"Found more than one unique shape in the tensors to be "
                     f"stacked ({shapes}). This is likely due to a modification "
                     f"of one of the stacked TensorDicts, where a key has been "
                     f"updated/created with an uncompatible shape. If the entries "
                     f"are intended to have a different shape, use the get_nestedtensor "
                     f"method instead."
                 )
             else:
                 raise err
 
+    def get_at(self, key, index, default=NO_DEFAULT):
+        item = self.get(key, default=default)
+        if item is default and default is not NO_DEFAULT:
+            return item
+        if isinstance(item, TensorDictBase):
+            return SubTensorDict(item, index)
+        else:
+            return item[index]
+
     def get_nestedtensor(
         self,
         key: NestedKey,
-        default: str | CompatibleType = "_no_default_",
+        default: str | CompatibleType = NO_DEFAULT,
     ) -> CompatibleType:
         # disallow getting nested tensor if the stacking dimension is not 0
         if self.stack_dim != 0:
             raise RuntimeError(
                 "Because nested tensors can only be stacked along their first "
                 "dimension, LazyStackedTensorDict.get_nestedtensor can only be called "
                 "when the stack_dim is 0."
@@ -4915,42 +5602,50 @@
         source = {key: value.contiguous() for key, value in self.items()}
         batch_size = self.batch_size
         device = self.device
         out = TensorDict(
             source=source,
             batch_size=batch_size,
             device=device,
+            names=self.names,
             _run_checks=False,
         )
         return out
 
     def clone(self, recurse: bool = True) -> TensorDictBase:
         if recurse:
             # This could be optimized using copy but we must be careful with
             # metadata (_is_shared etc)
-            return LazyStackedTensorDict(
+            out = LazyStackedTensorDict(
                 *[td.clone() for td in self.tensordicts],
                 stack_dim=self.stack_dim,
             )
-        return LazyStackedTensorDict(
-            *[td.clone(recurse=False) for td in self.tensordicts],
-            stack_dim=self.stack_dim,
-        )
+        else:
+            out = LazyStackedTensorDict(
+                *[td.clone(recurse=False) for td in self.tensordicts],
+                stack_dim=self.stack_dim,
+            )
+        if self._names is not None:
+            out.names = self.names
+        return out
 
     def pin_memory(self) -> TensorDictBase:
         for td in self.tensordicts:
             td.pin_memory()
         return self
 
     def to(self, dest: DeviceType | type, **kwargs) -> TensorDictBase:
         if isinstance(dest, type) and issubclass(dest, TensorDictBase):
             if isinstance(self, dest):
                 return self
             kwargs.update({"batch_size": self.batch_size})
-            return dest(source=self, **kwargs)
+            out = dest(source=self, **kwargs)
+            if self._names is not None:
+                out.names = self._names
+            return out
         elif isinstance(dest, (torch.device, str, int)):
             dest = torch.device(dest)
             if self.device is not None and dest == self.device:
                 return self
             td = self.to_tensordict().to(dest, **kwargs)
             return td
 
@@ -5058,93 +5753,125 @@
         return super().__setitem__(item, value)
 
     def __contains__(self, item: IndexType) -> bool:
         if isinstance(item, TensorDictBase):
             return any(item is td for td in self.tensordicts)
         return super().__contains__(item)
 
-    def __getitem__(self, item: IndexType) -> TensorDictBase:
-        if item is Ellipsis or (isinstance(item, tuple) and Ellipsis in item):
-            item = convert_ellipsis_to_idx(item, self.batch_size)
-        if isinstance(item, tuple) and sum(
-            isinstance(_item, str) for _item in item
+    def __getitem__(self, index: IndexType) -> TensorDictBase:
+        if isinstance(index, tuple) and len(index) == 1:
+            index = index[0]
+        if index is Ellipsis or (isinstance(index, tuple) and Ellipsis in index):
+            index = convert_ellipsis_to_idx(index, self.batch_size)
+        if index is None:
+            return self.unsqueeze(0)
+        if isinstance(index, tuple) and sum(
+            isinstance(_item, str) for _item in index
         ) not in [
-            len(item),
+            len(index),
             0,
         ]:
             raise IndexError(_STR_MIXED_INDEX_ERROR)
-        if isinstance(item, (list, range)):
-            item = torch.tensor(item, device=self.device)
-        if isinstance(item, tuple) and any(
-            isinstance(sub_index, (list, range)) for sub_index in item
+        if isinstance(index, (list, range)):
+            index = torch.tensor(index, device=self.device)
+        if isinstance(index, tuple) and any(
+            isinstance(sub_index, (list, range)) for sub_index in index
         ):
-            item = tuple(
+            index = tuple(
                 torch.tensor(sub_index, device=self.device)
                 if isinstance(sub_index, (list, range))
                 else sub_index
-                for sub_index in item
+                for sub_index in index
             )
-        if isinstance(item, str):
-            return self.get(item)
-        elif isinstance(item, tuple) and all(
-            isinstance(sub_item, str) for sub_item in item
+        if isinstance(index, str):
+            return self.get(index)
+        elif isinstance(index, tuple) and all(
+            isinstance(sub_item, str) for sub_item in index
         ):
-            out = self.get(item[0])
-            if len(item) > 1:
+            out = self.get(index[0])
+            if len(index) > 1:
                 if not isinstance(out, TensorDictBase):
                     raise RuntimeError(
                         f"Got a {type(out)} when a TensorDictBase instance was expected."
                     )
-                return out.get(item[1:])
+                return out.get(index[1:])
             else:
                 return out
-        elif isinstance(item, Tensor) and item.dtype == torch.bool:
-            return self.masked_select(item)
-        elif (
-            isinstance(item, (Number,))
-            or (isinstance(item, Tensor) and item.ndimension() == 0)
-        ) and self.stack_dim == 0:
-            return self.tensordicts[item]
-        elif isinstance(item, (Tensor, list)) and self.stack_dim == 0:
+        elif isinstance(index, Tensor) and index.dtype == torch.bool:
+            return self.masked_select(index)
+        elif _is_number(index) and self.stack_dim == 0:
+            return self.tensordicts[index]
+        elif isinstance(index, (Tensor, list)) and self.stack_dim == 0:
             out = LazyStackedTensorDict(
-                *[self.tensordicts[_item] for _item in item],
+                *[self.tensordicts[_item] for _item in index],
                 stack_dim=self.stack_dim,
             )
             return out
-        elif isinstance(item, (Tensor, list)) and self.stack_dim != 0:
+        elif isinstance(index, (Tensor, list)) and self.stack_dim != 0:
+            tds = [tensordict[index] for tensordict in self.tensordicts]
+            dim_drop = self.tensordicts[0].ndim - tds[0].ndim
             out = LazyStackedTensorDict(
-                *[tensordict[item] for tensordict in self.tensordicts],
-                stack_dim=self.stack_dim,
+                *tds,
+                stack_dim=self.stack_dim - dim_drop,
+            )
+            if self._names is not None:
+                out.names = [
+                    name if i != out.stack_dim else self.names[self.stack_dim]
+                    for i, name in enumerate(out.names)
+                ]
+            return out
+        elif isinstance(index, slice) and self.stack_dim == 0:
+            out = LazyStackedTensorDict(
+                *self.tensordicts[index], stack_dim=self.stack_dim
             )
+            if self._names is not None:
+                out.names = [
+                    name if i != out.stack_dim else self.names[self.stack_dim]
+                    for i, name in enumerate(out.names)
+                ]
             return out
-        elif isinstance(item, slice) and self.stack_dim == 0:
-            return LazyStackedTensorDict(
-                *self.tensordicts[item], stack_dim=self.stack_dim
-            )
-        elif isinstance(item, slice) and self.stack_dim != 0:
-            return LazyStackedTensorDict(
-                *[tensordict[item] for tensordict in self.tensordicts],
+        elif isinstance(index, slice) and self.stack_dim != 0:
+            out = LazyStackedTensorDict(
+                *[tensordict[index] for tensordict in self.tensordicts],
                 stack_dim=self.stack_dim,
             )
-        elif isinstance(item, (slice, Number)):
+            if self._names is not None:
+                out.names = [
+                    name if i != out.stack_dim else self.names[self.stack_dim]
+                    for i, name in enumerate(out.names)
+                ]
+            return out
+        elif isinstance(index, (slice, Number)):
             new_stack_dim = (
-                self.stack_dim - 1 if isinstance(item, Number) else self.stack_dim
+                self.stack_dim - 1 if isinstance(index, Number) else self.stack_dim
             )
-            return LazyStackedTensorDict(
-                *[td[item] for td in self.tensordicts],
+            out = LazyStackedTensorDict(
+                *[td[index] for td in self.tensordicts],
                 stack_dim=new_stack_dim,
             )
-        elif isinstance(item, tuple):
+            if self._names is not None:
+                out.names = [
+                    name if i != out.stack_dim else self.names[self.stack_dim]
+                    for i, name in enumerate(out.names)
+                ]
+            return out
+        elif isinstance(index, tuple):
+            for i, item in enumerate(index):
+                if item is None:
+                    truncated = tuple(
+                        item if j != i else slice(None) for j, item in enumerate(index)
+                    )
+                    return self.unsqueeze(i).__getitem__(truncated)
             # select sub tensordicts
             _sub_item = tuple(
-                _item for i, _item in enumerate(item) if i != self.stack_dim
+                _item for i, _item in enumerate(index) if i != self.stack_dim
             )
 
-            if self.stack_dim < len(item):
-                idx = item[self.stack_dim]
+            if self.stack_dim < len(index):
+                idx = index[self.stack_dim]
                 if isinstance(idx, (Number, slice)):
                     tensordicts = self.tensordicts[idx]
                 elif isinstance(idx, Tensor):
                     tensordicts = [self.tensordicts[i] for i in idx]
                 else:
                     raise TypeError(
                         "Invalid index used for stack dimension. Expected number, "
@@ -5155,30 +5882,235 @@
                         return tensordicts[_sub_item]
                     return tensordicts
             else:
                 tensordicts = self.tensordicts
 
             if len(_sub_item):
                 tensordicts = [td[_sub_item] for td in tensordicts]
+            index_to_stack = []
+            count = 0
+            for item in index:
+                if item is None:
+                    index_to_stack += [item]
+                if count == self.stack_dim:
+                    break
+                count += 1
+                if item is not None:
+                    index_to_stack += [item]
             new_stack_dim = self.stack_dim - sum(
-                [isinstance(_item, Number) for _item in item[: self.stack_dim]]
+                int(_is_number(_item)) - int(_item is None) for _item in index_to_stack
             )
-            return torch.stack(list(tensordicts), dim=new_stack_dim)
+            out = torch.stack(list(tensordicts), dim=new_stack_dim)
+            if self._names is not None:
+                out.names = [
+                    name if i != out.stack_dim else self.names[self.stack_dim]
+                    for i, name in enumerate(out.names)
+                ]
+            return out
         else:
             raise NotImplementedError(
                 f"selecting StackedTensorDicts with type "
-                f"{item.__class__.__name__} is not supported yet"
+                f"{index.__class__.__name__} is not supported yet"
+            )
+
+    def __eq__(self, other):
+        # avoiding circular imports
+        from tensordict.tensorclass import is_tensorclass
+
+        if is_tensorclass(other):
+            return other == self
+        if isinstance(other, (dict,)) or is_tensor_collection(other):
+            if (
+                isinstance(other, LazyStackedTensorDict)
+                and other.stack_dim == self.stack_dim
+            ):
+                if self.shape != other.shape:
+                    raise RuntimeError(
+                        "Cannot compare LazyStackedTensorDict instances of different shape."
+                    )
+                # in this case, we iterate over the tensordicts
+                return torch.stack(
+                    [
+                        td1 == td2
+                        for td1, td2 in zip(self.tensordicts, other.tensordicts)
+                    ],
+                    self.stack_dim,
+                )
+            keys1 = set(self.keys())
+            keys2 = set(other.keys())
+            if len(keys1.difference(keys2)) or len(keys1) != len(keys2):
+                raise KeyError(f"keys in tensordicts mismatch, got {keys1} and {keys2}")
+            d = {}
+            for key, item1 in self.items():
+                d[key] = item1 == other.get(key)
+            return TensorDict(batch_size=self.batch_size, source=d, device=self.device)
+        if isinstance(other, (numbers.Number, Tensor)):
+            return torch.stack(
+                [td == other for td in self.tensordicts],
+                self.stack_dim,
+            )
+        return False
+
+    def __ne__(self, other):
+        # avoiding circular imports
+        from tensordict.tensorclass import is_tensorclass
+
+        if is_tensorclass(other):
+            return other != self
+        if isinstance(other, (dict,)) or is_tensor_collection(other):
+            if (
+                isinstance(other, LazyStackedTensorDict)
+                and other.stack_dim == self.stack_dim
+            ):
+                if self.shape != other.shape:
+                    raise RuntimeError(
+                        "Cannot compare LazyStackedTensorDict instances of different shape."
+                    )
+                # in this case, we iterate over the tensordicts
+                return torch.stack(
+                    [
+                        td1 != td2
+                        for td1, td2 in zip(self.tensordicts, other.tensordicts)
+                    ],
+                    self.stack_dim,
+                )
+            keys1 = set(self.keys())
+            keys2 = set(other.keys())
+            if len(keys1.difference(keys2)) or len(keys1) != len(keys2):
+                raise KeyError(f"keys in tensordicts mismatch, got {keys1} and {keys2}")
+            d = {}
+            for key, item1 in self.items():
+                d[key] = item1 != other.get(key)
+            return TensorDict(batch_size=self.batch_size, source=d, device=self.device)
+        if isinstance(other, (numbers.Number, Tensor)):
+            return torch.stack(
+                [td != other for td in self.tensordicts],
+                self.stack_dim,
+            )
+        return True
+
+    def all(self, dim: int = None) -> bool | TensorDictBase:
+        if dim is not None and (dim >= self.batch_dims or dim < -self.batch_dims):
+            raise RuntimeError(
+                "dim must be greater than or equal to -tensordict.batch_dims and "
+                "smaller than tensordict.batch_dims"
+            )
+        if dim is not None:
+            # TODO: we need to adapt this to LazyStackedTensorDict too
+            if dim < 0:
+                dim = self.batch_dims + dim
+            return TensorDict(
+                source={key: value.all(dim=dim) for key, value in self.items()},
+                batch_size=[b for i, b in enumerate(self.batch_size) if i != dim],
+                device=self.device,
             )
+        return all(value.all() for value in self.tensordicts)
+
+    def any(self, dim: int = None) -> bool | TensorDictBase:
+        if dim is not None and (dim >= self.batch_dims or dim < -self.batch_dims):
+            raise RuntimeError(
+                "dim must be greater than or equal to -tensordict.batch_dims and "
+                "smaller than tensordict.batch_dims"
+            )
+        if dim is not None:
+            # TODO: we need to adapt this to LazyStackedTensorDict too
+            if dim < 0:
+                dim = self.batch_dims + dim
+            return TensorDict(
+                source={key: value.any(dim=dim) for key, value in self.items()},
+                batch_size=[b for i, b in enumerate(self.batch_size) if i != dim],
+                device=self.device,
+            )
+        return any(value.any() for value in self.tensordicts)
+
+    def _send(self, dst: int, _tag: int = -1, pseudo_rand: bool = False) -> int:
+        for td in self.tensordicts:
+            _tag = td._send(dst, _tag=_tag, pseudo_rand=pseudo_rand)
+        return _tag
+
+    def _isend(
+        self,
+        dst: int,
+        _tag: int = -1,
+        _futures: list[torch.Future] | None = None,
+        pseudo_rand: bool = False,
+    ) -> int:
+
+        if _futures is None:
+            is_root = True
+            _futures = []
+        else:
+            is_root = False
+        for td in self.tensordicts:
+            _tag = td._isend(dst, _tag=_tag, pseudo_rand=pseudo_rand, _futures=_futures)
+        if is_root:
+            for future in _futures:
+                future.wait()
+        return _tag
+
+    def _recv(self, src: int, _tag: int = -1, pseudo_rand: bool = False) -> int:
+        for td in self.tensordicts:
+            _tag = td._recv(src, _tag=_tag, pseudo_rand=pseudo_rand)
+        return _tag
+
+    def _irecv(
+        self,
+        src: int,
+        return_premature: bool = False,
+        _tag: int = -1,
+        _future_list: list[torch.Future] = None,
+        pseudo_rand: bool = False,
+    ) -> tuple[int, list[torch.Future]] | list[torch.Future] | None:
+        root = False
+        if _future_list is None:
+            _future_list = []
+            root = True
+        for td in self.tensordicts:
+            _tag, _future_list = td._irecv(
+                src=src,
+                return_premature=return_premature,
+                _tag=_tag,
+                _future_list=_future_list,
+                pseudo_rand=pseudo_rand,
+            )
+
+        if not root:
+            return _tag, _future_list
+        elif return_premature:
+            return _future_list
+        else:
+            for future in _future_list:
+                future.wait()
+            return
 
     def del_(self, key: str, **kwargs: Any) -> TensorDictBase:
         for td in self.tensordicts:
             td.del_(key, **kwargs)
         self._valid_keys.remove(key)
         return self
 
+    def pop(
+        self, key: NestedKey, default: str | CompatibleType = NO_DEFAULT
+    ) -> CompatibleType:
+
+        try:
+            # using try/except for get/del is suboptimal, but
+            # this is faster that checkink if key in self keys
+            out = self.get(key, default)
+            if key in self.valid_keys:
+                self._valid_keys.remove(key)
+        except KeyError as err:
+            # if default provided, 'out' value will return, else raise error
+            if default == NO_DEFAULT:
+                raise KeyError(
+                    f"You are trying to pop key `{key}` which is not in dict "
+                    f"without providing default value."
+                ) from err
+        return out
+
     def share_memory_(self) -> TensorDictBase:
         for td in self.tensordicts:
             td.share_memory_()
         self._is_shared = True
         self.lock_()
         return self
 
@@ -5532,25 +6464,34 @@
             )(**self.custom_op_kwargs).shape
         return self._batch_size
 
     @batch_size.setter
     def batch_size(self, new_size: torch.Size) -> None:
         self._batch_size_setter(new_size)
 
+    def _rename_subtds(self, names):
+        for key in self.keys():
+            if is_tensor_collection(self.entry_class(key)):
+                raise RuntimeError(
+                    "Cannot rename dimensions of a lazy TensorDict with "
+                    "nested collections. Convert the instance to a regular "
+                    "tensordict by using the `to_tensordict()` method first."
+                )
+
     def _change_batch_size(self, new_size: torch.Size) -> None:
         if not hasattr(self, "_orig_batch_size"):
             self._orig_batch_size = self.batch_size
         elif self._orig_batch_size == new_size:
             del self._orig_batch_size
         self._batch_size = new_size
 
     def get(
         self,
         key: NestedKey,
-        default: str | CompatibleType = "_no_default_",
+        default: str | CompatibleType = NO_DEFAULT,
         _return_original_tensor: bool = False,
     ) -> CompatibleType:
         # TODO: temporary hack while SavedTensorDict and LazyStackedTensorDict don't
         # support nested iteration
         include_nested = not isinstance(self._source, (LazyStackedTensorDict,))
 
         if key in self._source.keys(include_nested=include_nested):
@@ -5682,14 +6623,15 @@
     def clone(self, recurse: bool = True) -> TensorDictBase:
         if not recurse:
             return copy(self)
         return TensorDict(
             source=self.to_dict(),
             batch_size=self.batch_size,
             device=self.device,
+            names=self._names,
             _run_checks=False,
         )
 
     def is_contiguous(self) -> bool:
         return all([value.is_contiguous() for _, value in self.items()])
 
     def contiguous(self) -> TensorDictBase:
@@ -5709,15 +6651,18 @@
         self._source = self._source.del_(key)
         return self
 
     def to(self, dest: DeviceType | type, **kwargs) -> TensorDictBase:
         if isinstance(dest, type) and issubclass(dest, TensorDictBase):
             if isinstance(self, dest):
                 return self
-            return dest(source=self)
+            out = dest(source=self)
+            if self._names is not None:
+                out.names = self._names
+            return out
         elif isinstance(dest, (torch.device, str, int)):
             if self.device is not None and torch.device(dest) == self.device:
                 return self
             td = self._source.to(dest, **kwargs)
             self_copy = copy(self)
             self_copy._source = td
             return self_copy
@@ -5784,14 +6729,21 @@
 
     def share_memory_(self) -> _CustomOpTensorDict:
         self._source.share_memory_()
         self._is_shared = True
         self.lock_()
         return self
 
+    @property
+    def _names(self):
+        # we also want for _names to be accurate
+        if self._source._names is None:
+            return None
+        return self.names
+
 
 class _UnsqueezedTensorDict(_CustomOpTensorDict):
     """A lazy view on an unsqueezed TensorDict.
 
     When calling `tensordict.unsqueeze(dim)`, a lazy view of this operation is
     returned such that the following code snippet works without raising an
     exception:
@@ -5825,14 +6777,27 @@
         unsqueezed_dim = self.custom_op_kwargs["dim"]
         diff_to_apply = 1 if dim < unsqueezed_dim else 0
         list_item_unsqueeze = [
             item.squeeze(unsqueezed_dim - diff_to_apply) for item in list_item
         ]
         return self._source._stack_onto_(key, list_item_unsqueeze, dim)
 
+    @property
+    def names(self):
+        names = copy(self._source.names)
+        dim = self.custom_op_kwargs.get("dim")
+        names.insert(dim, None)
+        return names
+
+    @names.setter
+    def names(self, value):
+        raise RuntimeError(
+            "Names of a lazy tensordict cannot be modified. Call to_tensordict() first."
+        )
+
 
 class _SqueezedTensorDict(_CustomOpTensorDict):
     """A lazy view on a squeezed TensorDict.
 
     See the `UnsqueezedTensorDict` class documentation for more information.
 
     """
@@ -5859,14 +6824,28 @@
         # dim=2, squeezed_dim=2, [3, 4, 5] [3, 4, 1, 5] [[3, 4], [3, 4], ...] => unsq 2
         diff_to_apply = 1 if dim < squeezed_dim else 0
         list_item_unsqueeze = [
             item.unsqueeze(squeezed_dim - diff_to_apply) for item in list_item
         ]
         return self._source._stack_onto_(key, list_item_unsqueeze, dim)
 
+    @property
+    def names(self):
+        names = copy(self._source.names)
+        dim = self.custom_op_kwargs["dim"]
+        if self._source.batch_size[dim] == 1:
+            del names[dim]
+        return names
+
+    @names.setter
+    def names(self, value):
+        raise RuntimeError(
+            "Names of a lazy tensordict cannot be modified. Call to_tensordict() first."
+        )
+
 
 class _ViewedTensorDict(_CustomOpTensorDict):
     def _update_custom_op_kwargs(self, source_tensor: Tensor) -> dict[str, Any]:
         new_dim_list = list(self.custom_op_kwargs.get("size"))
         new_dim_list += list(source_tensor.shape[self._source.batch_dims :])
         new_dim = torch.Size(new_dim_list)
         new_dict = deepcopy(self.custom_op_kwargs)
@@ -5891,14 +6870,24 @@
         elif not isinstance(shape, torch.Size):
             shape = infer_size_impl(shape, self.numel())
             shape = torch.Size(shape)
         if shape == self._source.batch_size:
             return self._source
         return super().view(*shape)
 
+    @property
+    def names(self):
+        return [None] * self.ndim
+
+    @names.setter
+    def names(self, value):
+        raise RuntimeError(
+            "Names of a lazy tensordict cannot be modified. Call to_tensordict() first."
+        )
+
 
 class _PermutedTensorDict(_CustomOpTensorDict):
     """A lazy view on a TensorDict with the batch dimensions permuted.
 
     When calling `tensordict.permute(dims_list, dim)`, a lazy view of this operation is
     returned such that the following code snippet works without raising an
     exception:
@@ -5983,14 +6972,25 @@
             perm = list(inv_permute_dims) + list(
                 range(self.batch_dims - 1, item.ndimension())
             )
             list_permuted_items.append(item.permute(*perm))
         self._source._stack_onto_(key, list_permuted_items, new_dim)
         return self
 
+    @property
+    def names(self):
+        names = copy(self._source.names)
+        return [names[i] for i in self.custom_op_kwargs["dims"]]
+
+    @names.setter
+    def names(self, value):
+        raise RuntimeError(
+            "Names of a lazy tensordict cannot be modified. Call to_tensordict() first."
+        )
+
 
 def _get_repr(tensor: Tensor) -> str:
     s = ", ".join(
         [
             f"shape={_shape(tensor)}",
             f"device={_device(tensor)}",
             f"dtype={_dtype(tensor)}",
@@ -6082,53 +7082,99 @@
 
 def make_tensordict(
     input_dict: dict[str, CompatibleType] | None = None,
     batch_size: Sequence[int] | torch.Size | int | None = None,
     device: DeviceType | None = None,
     **kwargs: CompatibleType,  # source
 ) -> TensorDict:
-    """Returns a TensorDict created from the keyword arguments.
+    """Returns a TensorDict created from the keyword arguments or an input dictionary.
 
-    If batch_size is not specified, returns the maximum batch size possible
+    If ``batch_size`` is not specified, returns the maximum batch size possible.
+
+    This function works on nested dictionaries too, or can be used to determine the
+    batch-size of a nested tensordict.
 
     Args:
         input_dict (dictionary, optional): a dictionary to use as a data source
             (nested keys compatible).
         **kwargs (TensorDict or torch.Tensor): keyword arguments as data source
             (incompatible with nested keys).
         batch_size (iterable of int, optional): a batch size for the tensordict.
         device (torch.device or compatible type, optional): a device for the TensorDict.
 
+    Examples:
+        >>> input_dict = {"a": torch.randn(3, 4), "b": torch.randn(3)}
+        >>> print(make_tensordict(input_dict))
+        TensorDict(
+            fields={
+                a: Tensor(shape=torch.Size([3, 4]), device=cpu, dtype=torch.float32, is_shared=False),
+                b: Tensor(shape=torch.Size([3]), device=cpu, dtype=torch.float32, is_shared=False)},
+            batch_size=torch.Size([3]),
+            device=None,
+            is_shared=False)
+        >>> # alternatively
+        >>> td = make_tensordict(**input_dict)
+        >>> # nested dict: the nested TensorDict can have a different batch-size
+        >>> # as long as its leading dims match.
+        >>> input_dict = {"a": torch.randn(3), "b": {"c": torch.randn(3, 4)}}
+        >>> print(make_tensordict(input_dict))
+        TensorDict(
+            fields={
+                a: Tensor(shape=torch.Size([3]), device=cpu, dtype=torch.float32, is_shared=False),
+                b: TensorDict(
+                    fields={
+                        c: Tensor(shape=torch.Size([3, 4]), device=cpu, dtype=torch.float32, is_shared=False)},
+                    batch_size=torch.Size([3, 4]),
+                    device=None,
+                    is_shared=False)},
+            batch_size=torch.Size([3]),
+            device=None,
+            is_shared=False)
+        >>> # we can also use this to work out the batch sie of a tensordict
+        >>> input_td = TensorDict({"a": torch.randn(3), "b": {"c": torch.randn(3, 4)}}, [])
+        >>> print(make_tensordict(input_td))
+        TensorDict(
+            fields={
+                a: Tensor(shape=torch.Size([3]), device=cpu, dtype=torch.float32, is_shared=False),
+                b: TensorDict(
+                    fields={
+                        c: Tensor(shape=torch.Size([3, 4]), device=cpu, dtype=torch.float32, is_shared=False)},
+                    batch_size=torch.Size([3, 4]),
+                    device=None,
+                    is_shared=False)},
+            batch_size=torch.Size([3]),
+            device=None,
+            is_shared=False)
     """
     if input_dict is not None:
         kwargs.update(input_dict)
-    if batch_size is None:
-        batch_size = _find_max_batch_size(kwargs)
-    # _run_checks=False breaks because a tensor may have the same batch-size as the tensordict
-    return TensorDict(
-        kwargs,
-        batch_size=batch_size,
-        device=device,
-    )  # _run_checks=False)
+    return TensorDict.from_dict(kwargs, batch_size=batch_size, device=device)
 
 
-def _find_max_batch_size(source: TensorDictBase | dict) -> list[int]:
+def _set_max_batch_size(source: TensorDictBase):
+    """Updates a tensordict with its maximium batch size."""
     tensor_data = list(source.values())
+    for val in tensor_data:
+        if is_tensor_collection(val):
+            _set_max_batch_size(val)
     batch_size = []
     if not tensor_data:  # when source is empty
-        return batch_size
+        source.batch_size = batch_size
+        return
     curr_dim = 0
     while True:
         if tensor_data[0].dim() > curr_dim:
             curr_dim_size = tensor_data[0].size(curr_dim)
         else:
-            return batch_size
+            source.batch_size = batch_size
+            return
         for tensor in tensor_data[1:]:
             if tensor.dim() <= curr_dim or tensor.size(curr_dim) != curr_dim_size:
-                return batch_size
+                source.batch_size = batch_size
+                return
         batch_size.append(curr_dim_size)
         curr_dim += 1
 
 
 def _iter_items_lazystack(
     tensordict: LazyStackedTensorDict,
 ) -> Iterator[tuple[str, CompatibleType]]:
@@ -6143,7 +7189,15 @@
 def _clone_value(value: CompatibleType, recurse: bool) -> CompatibleType:
     if recurse:
         return value.clone()
     elif is_tensor_collection(value):
         return value.clone(recurse=False)
     else:
         return value
+
+
+def _is_number(item):
+    if isinstance(item, Number):
+        return True
+    if isinstance(item, Tensor) and item.ndim == 0:
+        return True
+    return False
```

### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

## tensordict/utils.py

```diff
@@ -71,33 +71,45 @@
     expensive operation.
     Args:
         shape (torch.Size): Input shape
         items (index): Index of the hypothetical tensor
 
     Returns:
         Size of the resulting object (tensor or tensordict)
+
+    Examples:
+        >>> idx = (None, ..., None)
+        >>> torch.zeros(4, 3, 2, 1)[idx].shape
+        torch.Size([1, 4, 3, 2, 1, 1])
+        >>> _getitem_batch_size([4, 3, 2, 1], idx)
+        torch.Size([1, 4, 3, 2, 1, 1])
     """
     # let's start with simple cases
     if isinstance(items, tuple) and len(items) == 1:
         items = items[0]
     if isinstance(items, int):
         return shape[1:]
     if isinstance(items, torch.Tensor) and items.dtype is torch.bool:
         return torch.Size([items.sum(), *shape[items.ndimension() :]])
     if (
         isinstance(items, (torch.Tensor, np.ndarray)) and len(items.shape) <= 1
     ) or isinstance(items, list):
+        if isinstance(items, torch.Tensor) and not items.shape:
+            return shape[1:]
         if len(items):
             return torch.Size([len(items), *shape[1:]])
         else:
             return shape[1:]
 
     if not isinstance(items, tuple):
         items = (items,)
 
+    if any(item is Ellipsis for item in items):
+        items = convert_ellipsis_to_idx(items, shape)
+
     sanitized_items = []
     for _item in items:
         if isinstance(_item, (list, np.ndarray)):
             _item = torch.tensor(_item)
         elif isinstance(_item, torch.Tensor):
             # np.broadcast will complain if we give it CUDA tensors
             _item = _item.cpu()
@@ -116,45 +128,49 @@
     # to extract diagonal entries of the array.
     # if the tensor indices are contiguous, or separated by scalars, they are replaced
     # in-place by the broadcast shape. if they are separated by non-scalar indices, the
     # broadcast shape is prepended to the new batch size
     # https://numpy.org/doc/stable/user/basics.indexing.html#integer-array-indexing
     tensor_indices = []
     contiguous, prev = True, None
-
     for i, _item in enumerate(sanitized_items):
         if isinstance(_item, torch.Tensor):
             tensor_indices.append(_item)
             if prev is not None and i != prev + 1:
                 contiguous = False
             prev = i
         elif isinstance(_item, Number) and prev is not None and i == prev + 1:
             prev = i
 
     bs = []
     if tensor_indices:
         try:
             b = np.broadcast(*tensor_indices)
-        except ValueError:
+        except ValueError as err:
             raise ValueError(
                 "When indexing with tensor-like indices, each of those indices must be "
-                "broadcastable to a common shape."
-            )
+                f"broadcastable to a common shape. Got indices: {tensor_indices}."
+            ) from err
         if not contiguous:
             bs.extend(b.shape)
             b = None
     else:
         b = None
 
     iter_bs = iter(shape)
 
+    cursor = -1
     for _item in sanitized_items:
+        cursor += 1
         if isinstance(_item, slice):
             batch = next(iter_bs)
             bs.append(len(range(*_item.indices(batch))))
+        elif isinstance(_item, range):
+            batch = next(iter_bs)
+            bs.append(min(batch, len(_item)))
         elif isinstance(_item, (list, torch.Tensor, np.ndarray)):
             batch = next(iter_bs)
             if b is not None:
                 # we haven't yet accounted for tensor indices, so we insert in-place
                 bs.extend(b.shape)
                 b = None
         elif _item is None:
@@ -163,14 +179,23 @@
             try:
                 batch = next(iter_bs)
             except StopIteration:
                 raise RuntimeError(
                     f"The shape {shape} is incompatible with " f"the index {items}."
                 )
             continue
+        elif _item is Ellipsis:
+            if cursor == len(sanitized_items) - 1:
+                # then we can just skip
+                continue
+            n_upcoming = len(sanitized_items) - cursor - 1
+            while cursor < len(shape) - n_upcoming:
+                batch = next(iter_bs)
+                bs.append(batch)
+                cursor += 1
         else:
             raise NotImplementedError(
                 f"batch dim cannot be computed for type {type(_item)}"
             )
 
     list_iter_bs = list(iter_bs)
     bs += list_iter_bs
@@ -197,30 +222,37 @@
         new_index (tuple): Output index
     """
     new_index = ()
     num_dims = len(batch_size)
 
     if idx is Ellipsis:
         idx = (...,)
+
     num_ellipsis = sum(_idx is Ellipsis for _idx in idx)
-    if num_dims < (len(idx) - num_ellipsis):
+    if num_dims < (len(idx) - num_ellipsis - sum(item is None for item in idx)):
         raise RuntimeError("Not enough dimensions in TensorDict for index provided.")
 
     start_pos, after_ellipsis_length = None, 0
     for i, item in enumerate(idx):
         if item is Ellipsis:
             if start_pos is not None:
                 raise RuntimeError("An index can only have one ellipsis at most.")
             else:
                 start_pos = i
         if item is not Ellipsis and start_pos is not None:
             after_ellipsis_length += 1
+        if item is None:
+            # unsqueeze
+            num_dims += 1
 
     before_ellipsis_length = start_pos
-    ellipsis_length = num_dims - after_ellipsis_length - before_ellipsis_length
+    if start_pos is None:
+        return idx
+    else:
+        ellipsis_length = num_dims - after_ellipsis_length - before_ellipsis_length
 
     new_index += idx[:start_pos]
 
     ellipsis_start = start_pos
     ellipsis_end = start_pos + ellipsis_length
     new_index += (slice(None),) * (ellipsis_end - ellipsis_start)
 
@@ -380,25 +412,41 @@
     np.dtype("complex128"): torch.complex128,
 }
 TORCH_TO_NUMPY_DTYPE_DICT = {
     value: key for key, value in NUMPY_TO_TORCH_DTYPE_DICT.items()
 }
 
 
-def _nested_key_type_check(key: NestedKey) -> None:
-    msg = "Expected key to be a string or non-empty tuple of strings, but found {}."
-    if type(key) is str:
-        return
-    is_tuple = type(key) is tuple
-    if not is_tuple:
-        raise TypeError(msg.format(type(key)))
-    else:
-        for subkey in key:
-            if type(subkey) is not str:
-                raise TypeError(msg.format(type(subkey)))
+def is_nested_key(key: NestedKey) -> bool:
+    """Returns True if key is a NestedKey."""
+    if isinstance(key, str):
+        return True
+    if key and isinstance(key, (list, tuple)):
+        return all(isinstance(subkey, str) for subkey in key)
+    return False
+
+
+def is_seq_of_nested_key(seq: Sequence[NestedKey]) -> bool:
+    """Returns True if seq is a Sequence[NestedKey]."""
+    if seq and isinstance(seq, Sequence):
+        return all(is_nested_key(k) for k in seq)
+    elif isinstance(seq, Sequence):
+        # we allow empty inputs
+        return True
+    return False
+
+
+def _seq_of_nested_key_check(seq: Sequence[NestedKey]) -> None:
+    if not is_seq_of_nested_key(seq):
+        raise ValueError(f"seq should be a Sequence[NestedKey]. Got {seq}")
+
+
+def _nested_key_check(key: NestedKey) -> None:
+    if not is_nested_key(key):
+        raise ValueError(f"key should be a Sequence[NestedKey]. Got {key}")
 
 
 def _normalize_key(key: NestedKey) -> NestedKey:
     # normalises tuples of length one to their string contents
     return key if not isinstance(key, tuple) or len(key) > 1 else key[0]
 
 
@@ -595,15 +643,15 @@
         return 1
     else:
         return tensor.ndimension()
 
 
 def _shape(tensor: torch.Tensor) -> torch.Size:
     try:
-        return tensor.shape
+        return torch.Size(tensor.shape)
     except AttributeError as err:
         if type(tensor) is KeyedJaggedTensor:
             return torch.Size([len(tensor.lengths()) // len(tensor.keys())])
         raise err
 
 
 def _device(tensor: torch.Tensor) -> torch.device:
```

## tensordict/version.py

```diff
@@ -1,2 +1,2 @@
-__version__ = '0.1.0'
-git_version = '223e04b846f8e60675eb380428a9b854c633642c'
+__version__ = '0.1.1'
+git_version = '7cebb2ab5745641d3e5bded35c9512905508649f'
```

## tensordict/nn/__init__.py

```diff
@@ -3,37 +3,50 @@
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
 from tensordict.nn.common import (
     dispatch,
     make_tensordict,
     TensorDictModule,
+    TensorDictModuleBase,
     TensorDictModuleWrapper,
 )
+from tensordict.nn.distributions import NormalParamExtractor
 from tensordict.nn.functional_modules import (
     get_functional,
+    is_functional,
     make_functional,
     repopulate_module,
 )
 from tensordict.nn.probabilistic import (
+    InteractionType,
     ProbabilisticTensorDictModule,
     ProbabilisticTensorDictSequential,
     set_interaction_mode,
+    set_interaction_type,
 )
 from tensordict.nn.sequence import TensorDictSequential
-from tensordict.nn.utils import biased_softplus, inv_softplus
+from tensordict.nn.utils import (
+    biased_softplus,
+    inv_softplus,
+    set_skip_existing,
+    skip_existing,
+)
 
 __all__ = [
     "dispatch",
     "TensorDictModule",
     "TensorDictModuleWrapper",
     "get_functional",
     "make_functional",
     "repopulate_module",
+    "InteractionType",
     "ProbabilisticTensorDictModule",
     "ProbabilisticTensorDictSequential",
     "set_interaction_mode",
+    "set_interaction_type",
     "TensorDictSequential",
     "make_tensordict",
     "biased_softplus",
     "inv_softplus",
+    "is_functional",
 ]
```

## tensordict/nn/common.py

```diff
@@ -5,20 +5,22 @@
 
 from __future__ import annotations
 
 import functools
 import inspect
 import warnings
 from textwrap import indent
-from typing import Any, Callable, Iterable, Sequence
+from typing import Any, Callable, Iterable, List, Sequence, Tuple, Union
 
 import torch
+from tensordict.nn.functional_modules import make_functional
 
-from tensordict.tensordict import make_tensordict, TensorDictBase
-from tensordict.utils import _nested_key_type_check, _normalize_key, NestedKey
+from tensordict.nn.utils import set_skip_existing
+from tensordict.tensordict import is_tensor_collection, make_tensordict, TensorDictBase
+from tensordict.utils import _normalize_key, _seq_of_nested_key_check, NestedKey
 from torch import nn, Tensor
 
 try:
     from functorch import FunctionalModule, FunctionalModuleWithBuffers
 
     _has_functorch = True
 except ImportError:
@@ -33,33 +35,14 @@
 
 __all__ = [
     "TensorDictModule",
     "TensorDictModuleWrapper",
 ]
 
 
-def _check_all_str(sequence_of_str: Sequence[str]) -> None:
-    if isinstance(sequence_of_str, str):
-        raise RuntimeError(
-            f"Expected a sequence of strings but got a string: {sequence_of_str}"
-        )
-    if any(not isinstance(key, str) for key in sequence_of_str):
-        raise TypeError(f"Expected a sequence of strings but got: {sequence_of_str}")
-
-
-def _check_all_nested(sequence_of_keys: Sequence[NestedKey]) -> None:
-    if isinstance(sequence_of_keys, str):
-        raise RuntimeError(
-            "Expected a sequence of strings, or tuples of strings but got a string: "
-            f"{sequence_of_keys}"
-        )
-    for key in sequence_of_keys:
-        _nested_key_type_check(key)
-
-
 class dispatch:
     """Allows for a function expecting a TensorDict to be called using kwargs.
 
     :func:`dispatch` must be used within modules that have an ``in_keys`` (or
     another source of keys indicated by the ``source`` keyword argument) and
     ``out_keys`` (or another ``dest`` key list) attributes indicating what keys
     to be read and written from the tensordict. The wrapped function should
@@ -84,14 +67,18 @@
             :class:`~.TensorDictModule` list of input keys.
         dest (str or list of keys, optional): if a string is provided,
             it points to the module attribute that contains the
             list of output keys to be used. If a list is provided instead, it
             will contain the keys used as output to the module.
             Defaults to ``"out_keys"`` which is the attribute name of
             :class:`~.TensorDictModule` list of output keys.
+        auto_batch_size (bool, optional): if ``True``, the batch-size of the
+            input tensordict is determined automatically as the maximum number
+            of common dimensions across all the input tensors.
+            Defaults to ``True``.
 
     Examples:
         >>> class MyModule(nn.Module):
         ...     in_keys = ["a"]
         ...     out_keys = ["b"]
         ...
         ...     @dispatch
@@ -199,30 +186,39 @@
     """
 
     DEFAULT_SEPARATOR = "_"
     DEFAULT_SOURCE = "in_keys"
     DEFAULT_DEST = "out_keys"
 
     def __new__(
-        cls, separator=DEFAULT_SEPARATOR, source=DEFAULT_SOURCE, dest=DEFAULT_DEST
+        cls,
+        separator=DEFAULT_SEPARATOR,
+        source=DEFAULT_SOURCE,
+        dest=DEFAULT_DEST,
+        auto_batch_size: bool = True,
     ):
         if callable(separator):
             func = separator
             separator = dispatch.DEFAULT_SEPARATOR
             self = super().__new__(cls)
             self.__init__(separator, source, dest)
             return self.__call__(func)
         return super().__new__(cls)
 
     def __init__(
-        self, separator=DEFAULT_SEPARATOR, source=DEFAULT_SOURCE, dest=DEFAULT_DEST
+        self,
+        separator=DEFAULT_SEPARATOR,
+        source=DEFAULT_SOURCE,
+        dest=DEFAULT_DEST,
+        auto_batch_size: bool = True,
     ):
         self.separator = separator
         self.source = source
         self.dest = dest
+        self.auto_batch_size = auto_batch_size
 
     def __call__(self, func: Callable) -> Callable:
         # sanity check
         for i, key in enumerate(inspect.signature(func).parameters):
             if i == 0:
                 # skip self
                 continue
@@ -231,22 +227,21 @@
                     "the first argument of the wrapped function must be "
                     "named 'tensordict'."
                 )
             break
 
         @functools.wraps(func)
         def wrapper(_self, *args: Any, **kwargs: Any) -> Any:
+
             source = self.source
             if isinstance(source, str):
                 source = getattr(_self, source)
             tensordict = None
             if len(args):
-                if not isinstance(args[0], TensorDictBase):
-                    pass
-                else:
+                if is_tensor_collection(args[0]):
                     tensordict, args = args[0], args[1:]
             if tensordict is None:
                 tensordict_values = {}
                 dest = self.dest
                 if isinstance(dest, str):
                     dest = getattr(_self, dest)
                 for key in source:
@@ -264,124 +259,487 @@
                         try:
                             tensordict_values[key] = kwargs.pop(expected_key)
                         except KeyError:
                             raise KeyError(
                                 f"The key {expected_key} wasn't found in the keyword arguments "
                                 f"but is expected to execute that function."
                             )
-                tensordict = make_tensordict(tensordict_values)
+                tensordict = make_tensordict(
+                    tensordict_values,
+                    batch_size=torch.Size([]) if not self.auto_batch_size else None,
+                )
                 out = func(_self, tensordict, *args, **kwargs)
                 out = tuple(out[key] for key in dest)
                 return out[0] if len(out) == 1 else out
             return func(_self, tensordict, *args, **kwargs)
 
         return wrapper
 
 
-class TensorDictModule(nn.Module):
+class _OutKeysSelect:
+    def __init__(self, out_keys):
+        self.out_keys = out_keys
+        self._initialized = False
+
+    def _init(self, module):
+        if self._initialized:
+            return
+        self._initialized = True
+        self.module = module
+        module.out_keys = list(self.out_keys)
+
+    def __call__(
+        self,
+        module: TensorDictModuleBase,
+        tensordict_in: TensorDictBase,
+        tensordict_out: TensorDictBase,
+    ):
+        # detect dispatch calls
+        in_keys = module.in_keys
+        is_dispatched = self._detect_dispatch(tensordict_in, in_keys)
+        out_keys = self.out_keys
+        # if dispatch filtered the out keys as they should we're happy
+        if is_dispatched:
+            if (not isinstance(tensordict_out, tuple) and len(out_keys) == 1) or (
+                len(out_keys) == len(tensordict_out)
+            ):
+                return tensordict_out
+        self._init(module)
+        if is_dispatched:
+            # it might be the case that dispatch was not aware of what the out-keys were.
+            if isinstance(tensordict_out, tuple):
+                out = tuple(
+                    item
+                    for i, item in enumerate(tensordict_out)
+                    if module._out_keys[i] in module.out_keys
+                )
+                if len(out) == 1:
+                    return out[0]
+                return out
+            elif module._out_keys[0] in module.out_keys and len(module._out_keys) == 1:
+                return tensordict_out
+            elif (
+                module._out_keys[0] not in module.out_keys
+                and len(module._out_keys) == 1
+            ):
+                return ()
+            else:
+                raise RuntimeError(
+                    f"Selecting out-keys failed. Original out_keys: {module._out_keys}, selected: {module.out_keys}."
+                )
+        if tensordict_out is tensordict_in:
+            return tensordict_out.select(
+                *in_keys,
+                *out_keys,
+                inplace=True,
+            )
+        else:
+            return tensordict_out.select(
+                *in_keys,
+                *out_keys,
+                inplace=True,
+                strict=False,
+            )
+
+    def _detect_dispatch(self, tensordict_in, in_keys):
+        if isinstance(tensordict_in, TensorDictBase) and all(
+            key in tensordict_in.keys() for key in in_keys
+        ):
+            return False
+        elif isinstance(tensordict_in, tuple):
+            if len(tensordict_in):
+                if isinstance(tensordict_in[0], TensorDictBase):
+                    return self._detect_dispatch(tensordict_in[0], in_keys)
+                return True
+            return not len(in_keys)
+        # not a TDBase: must be True
+        return True
+
+    def remove(self):
+        # reset ground truth
+        self.module.out_keys = self.module._out_keys
+
+    def __del__(self):
+        self.remove()
+
+
+class TensorDictModuleBase(nn.Module):
+    """Base class to TensorDict modules.
+
+    TensorDictModule subclasses are characterized by ``in_keys`` and ``out_keys``
+    key-lists that indicate what input entries are to be read and what output
+    entries should be expected to be written.
+
+    The forward method input/output signature should always follow the
+    convention:
+
+        >>> tensordict_out = module.forward(tensordict_in)
+
+    """
+
+    def __new__(cls, *args, **kwargs):
+        # check the out_keys and in_keys in the dict
+        if "in_keys" in cls.__dict__ and not isinstance(
+            cls.__dict__.get("in_keys"), property
+        ):
+            in_keys = cls.__dict__.get("in_keys")
+            # now let's remove it
+            delattr(cls, "in_keys")
+            cls._in_keys = in_keys
+            cls.in_keys = TensorDictModuleBase.in_keys
+        if "out_keys" in cls.__dict__ and not isinstance(
+            cls.__dict__.get("out_keys"), property
+        ):
+            out_keys = cls.__dict__.get("out_keys")
+            # now let's remove it
+            delattr(cls, "out_keys")
+            cls._out_keys = out_keys
+            cls._out_keys_apparent = out_keys
+            cls.out_keys = TensorDictModuleBase.out_keys
+        out = super().__new__(cls)
+        return out
+
+    @property
+    def in_keys(self):
+        return self._in_keys
+
+    @in_keys.setter
+    def in_keys(self, value: List[Union[str, Tuple[str]]]):
+        self._in_keys = value
+
+    @property
+    def out_keys(self):
+        return self._out_keys_apparent
+
+    @property
+    def out_keys_source(self):
+        return self._out_keys
+
+    @out_keys.setter
+    def out_keys(self, value: List[Union[str, Tuple[str]]]):
+        # the first time out_keys are set, they are marked as ground truth
+        if not hasattr(self, "_out_keys"):
+            self._out_keys = value
+        self._out_keys_apparent = value
+
+    def select_out_keys(self, *out_keys):
+        """Selects the keys that will be found in the output tensordict.
+
+        This is useful whenever one wants to get rid of intermediate keys in a
+        complicated graph, or when the presence of these keys may trigger unexpected
+        behaviours.
+
+        The original ``out_keys`` can still be accessed via ``module.out_keys_source``.
+
+        Args:
+            *out_keys (a sequence of strings or tuples of strings): the
+                out_keys that should be found in the output tensordict.
+
+        Returns: the same module, modified in-place with updated ``out_keys``.
+
+        The simplest usage is with :class:`~.TensorDictModule`:
+
+        Examples:
+            >>> from tensordict import TensorDict
+            >>> from tensordict.nn import TensorDictModule, TensorDictSequential
+            >>> import torch
+            >>> mod = TensorDictModule(lambda x, y: (x+2, y+2), in_keys=["a", "b"], out_keys=["c", "d"])
+            >>> td = TensorDict({"a": torch.zeros(()), "b": torch.ones(())}, [])
+            >>> mod(td)
+            TensorDict(
+                fields={
+                    a: Tensor(shape=torch.Size([]), device=cpu, dtype=torch.float32, is_shared=False),
+                    b: Tensor(shape=torch.Size([]), device=cpu, dtype=torch.float32, is_shared=False),
+                    c: Tensor(shape=torch.Size([]), device=cpu, dtype=torch.float32, is_shared=False),
+                    d: Tensor(shape=torch.Size([]), device=cpu, dtype=torch.float32, is_shared=False)},
+                batch_size=torch.Size([]),
+                device=None,
+                is_shared=False)
+            >>> mod.select_out_keys("d")
+            >>> td = TensorDict({"a": torch.zeros(()), "b": torch.ones(())}, [])
+            >>> mod(td)
+            TensorDict(
+                fields={
+                    a: Tensor(shape=torch.Size([]), device=cpu, dtype=torch.float32, is_shared=False),
+                    b: Tensor(shape=torch.Size([]), device=cpu, dtype=torch.float32, is_shared=False),
+                    d: Tensor(shape=torch.Size([]), device=cpu, dtype=torch.float32, is_shared=False)},
+                batch_size=torch.Size([]),
+                device=None,
+                is_shared=False)
+
+        This feature will also work with dispatched arguments:
+        Examples:
+            >>> mod(torch.zeros(()), torch.ones(()))
+            tensor(2.)
+
+        This change will occur in-place (ie the same module will be returned
+        with an updated list of out_keys). It can be reverted using the
+        :meth:`TensorDictModuleBase.reset_out_keys` method.
+
+        Examples:
+            >>> mod.reset_out_keys()
+            >>> mod(TensorDict({"a": torch.zeros(()), "b": torch.ones(())}, []))
+            TensorDict(
+                fields={
+                    a: Tensor(shape=torch.Size([]), device=cpu, dtype=torch.float32, is_shared=False),
+                    b: Tensor(shape=torch.Size([]), device=cpu, dtype=torch.float32, is_shared=False),
+                    c: Tensor(shape=torch.Size([]), device=cpu, dtype=torch.float32, is_shared=False),
+                    d: Tensor(shape=torch.Size([]), device=cpu, dtype=torch.float32, is_shared=False)},
+                batch_size=torch.Size([]),
+                device=None,
+                is_shared=False)
+
+        This will work with other classes too, such as Sequential:
+        Examples:
+            >>> from tensordict.nn import TensorDictSequential
+            >>> seq = TensorDictSequential(
+            ...     TensorDictModule(lambda x: x+1, in_keys=["x"], out_keys=["y"]),
+            ...     TensorDictModule(lambda x: x+1, in_keys=["y"], out_keys=["z"]),
+            ... )
+            >>> td = TensorDict({"x": torch.zeros(())}, [])
+            >>> seq(td)
+            TensorDict(
+                fields={
+                    x: Tensor(shape=torch.Size([]), device=cpu, dtype=torch.float32, is_shared=False),
+                    y: Tensor(shape=torch.Size([]), device=cpu, dtype=torch.float32, is_shared=False),
+                    z: Tensor(shape=torch.Size([]), device=cpu, dtype=torch.float32, is_shared=False)},
+                batch_size=torch.Size([]),
+                device=None,
+                is_shared=False)
+            >>> seq.select_out_keys("z")
+            >>> td = TensorDict({"x": torch.zeros(())}, [])
+            >>> seq(td)
+            TensorDict(
+                fields={
+                    x: Tensor(shape=torch.Size([]), device=cpu, dtype=torch.float32, is_shared=False),
+                    z: Tensor(shape=torch.Size([]), device=cpu, dtype=torch.float32, is_shared=False)},
+                batch_size=torch.Size([]),
+                device=None,
+                is_shared=False)
+
+        """
+        self.register_forward_hook(_OutKeysSelect(out_keys))
+        for hook in self._forward_hooks.values():
+            hook._init(self)
+        return self
+
+    def reset_out_keys(self):
+        """Resets the ``out_keys`` attribute to its orignal value.
+
+        Returns: the same module, with its original ``out_keys`` values.
+
+        Examples:
+            >>> from tensordict import TensorDict
+            >>> from tensordict.nn import TensorDictModule, TensorDictSequential
+            >>> import torch
+            >>> mod = TensorDictModule(lambda x, y: (x+2, y+2), in_keys=["a", "b"], out_keys=["c", "d"])
+            >>> mod.select_out_keys("d")
+            >>> td = TensorDict({"a": torch.zeros(()), "b": torch.ones(())}, [])
+            >>> mod(td)
+            TensorDict(
+                fields={
+                    a: Tensor(shape=torch.Size([]), device=cpu, dtype=torch.float32, is_shared=False),
+                    b: Tensor(shape=torch.Size([]), device=cpu, dtype=torch.float32, is_shared=False),
+                    d: Tensor(shape=torch.Size([]), device=cpu, dtype=torch.float32, is_shared=False)},
+                batch_size=torch.Size([]),
+                device=None,
+                is_shared=False)
+            >>> mod.reset_out_keys()
+            >>> mod(td)
+            TensorDict(
+                fields={
+                    a: Tensor(shape=torch.Size([]), device=cpu, dtype=torch.float32, is_shared=False),
+                    b: Tensor(shape=torch.Size([]), device=cpu, dtype=torch.float32, is_shared=False),
+                    c: Tensor(shape=torch.Size([]), device=cpu, dtype=torch.float32, is_shared=False),
+                    d: Tensor(shape=torch.Size([]), device=cpu, dtype=torch.float32, is_shared=False)},
+                batch_size=torch.Size([]),
+                device=None,
+                is_shared=False)
+        """
+        for i, hook in list(self._forward_hooks.items()):
+            if isinstance(hook, _OutKeysSelect):
+                del self._forward_hooks[i]
+        return self
+
+
+class TensorDictModule(TensorDictModuleBase):
     """A TensorDictModule, is a python wrapper around a :obj:`nn.Module` that reads and writes to a TensorDict.
 
+    By default, :class:`TensorDictModule` subclasses are always functional,
+    meaning that they support the ``td_module(input, params=params)`` function
+    call signature.
+
     Args:
-        module (nn.Module): a nn.Module used to map the input to the output parameter space. Can be a functional
-            module (FunctionalModule or FunctionalModuleWithBuffers), in which case the :obj:`forward` method will expect
-            the params (and possibly) buffers keyword arguments.
+        module (Callable): a callable, typically a :class:`torch.nn.Module`,
+            used to map the input to the output parameter space. Its forward method
+            can return a single tensor, a tuple of tensors or even a dictionary.
+            In the latter case, the output keys of the :class:`TensorDictModule`
+            will be used to populate the output tensordict (ie. the keys present
+            in ``out_keys`` should be present in the dictionary returned by the
+            ``module`` forward method).
         in_keys (iterable of str): keys to be read from input tensordict and passed to the module. If it
             contains more than one element, the values will be passed in the order given by the in_keys iterable.
         out_keys (iterable of str): keys to be written to the input tensordict. The length of out_keys must match the
             number of tensors returned by the embedded module. Using "_" as a key avoid writing tensor to output.
 
     Embedding a neural network in a TensorDictModule only requires to specify the input
     and output keys. TensorDictModule support functional and regular :obj:`nn.Module`
     objects. In the functional case, the 'params' (and 'buffers') keyword argument must
     be specified:
 
     Examples:
+        >>> from tensordict import TensorDict
+        >>> # one can wrap regular nn.Module
+        >>> module = TensorDictModule(nn.Transformer(128), in_keys=["input", "tgt"], out_keys=["out"])
+        >>> input = torch.ones(2, 3, 128)
+        >>> tgt = torch.zeros(2, 3, 128)
+        >>> data = TensorDict({"input": input, "tgt": tgt}, batch_size=[2, 3])
+        >>> data = module(data)
+        >>> print(data)
+        TensorDict(
+            fields={
+                input: Tensor(shape=torch.Size([2, 3, 128]), device=cpu, dtype=torch.float32, is_shared=False),
+                out: Tensor(shape=torch.Size([2, 3, 128]), device=cpu, dtype=torch.float32, is_shared=False),
+                tgt: Tensor(shape=torch.Size([2, 3, 128]), device=cpu, dtype=torch.float32, is_shared=False)},
+            batch_size=torch.Size([2, 3]),
+            device=None,
+            is_shared=False)
+        >>> # we can also pass directly the tensors
+        >>> out = module(input, tgt)
+        >>> assert out.shape == input.shape
+        >>> # we can also wrap regular functions
+        >>> module = TensorDictModule(lambda x: (x-1, x+1), in_keys=[("input", "x")], out_keys=[("output", "x-1"), ("output", "x+1")])
+        >>> module(TensorDict({("input", "x"): torch.zeros(())}, batch_size=[]))
+        TensorDict(
+            fields={
+                input: TensorDict(
+                    fields={
+                        x: Tensor(shape=torch.Size([]), device=cpu, dtype=torch.float32, is_shared=False)},
+                    batch_size=torch.Size([]),
+                    device=None,
+                    is_shared=False),
+                output: TensorDict(
+                    fields={
+                        x+1: Tensor(shape=torch.Size([]), device=cpu, dtype=torch.float32, is_shared=False),
+                        x-1: Tensor(shape=torch.Size([]), device=cpu, dtype=torch.float32, is_shared=False)},
+                    batch_size=torch.Size([]),
+                    device=None,
+                    is_shared=False)},
+            batch_size=torch.Size([]),
+            device=None,
+            is_shared=False)
+        >>> # we can use TensorDictModule to populate a tensordict
+        >>> module = TensorDictModule(lambda: torch.randn(3), in_keys=[], out_keys=["x"])
+        >>> print(module(TensorDict({}, batch_size=[])))
+        TensorDict(
+            fields={
+                x: Tensor(shape=torch.Size([3]), device=cpu, dtype=torch.float32, is_shared=False)},
+            batch_size=torch.Size([]),
+            device=None,
+            is_shared=False)
+
+    Functional calls to a tensordict module is easy:
+    Examples:
         >>> import torch
         >>> from tensordict import TensorDict
         >>> from tensordict.nn import TensorDictModule
         >>> from tensordict.nn.functional_modules import make_functional
         >>> td = TensorDict({"input": torch.randn(3, 4), "hidden": torch.randn(3, 8)}, [3,])
         >>> module = torch.nn.GRUCell(4, 8)
-        >>> fmodule, params, buffers = functorch.make_functional_with_buffers(module)
-        >>> td_fmodule = TensorDictModule(
-        ...    module=torch.nn.GRUCell(4, 8), in_keys=["input", "hidden"], out_keys=["output"]
+        >>> td_module = TensorDictModule(
+        ...    module=module, in_keys=["input", "hidden"], out_keys=["output"]
         ... )
-        >>> params = make_functional(td_fmodule)
-        >>> td_functional = td_fmodule(td.clone(), params=params)
+        >>> params = make_functional(td_module)
+        >>> td_functional = td_module(td.clone(), params=params)
         >>> print(td_functional)
         TensorDict(
             fields={
-                hidden: Tensor(torch.Size([3, 8]), dtype=torch.float32),
-                input: Tensor(torch.Size([3, 4]), dtype=torch.float32),
-                output: Tensor(torch.Size([3, 8]), dtype=torch.float32)},
-            shared=False,
+                hidden: Tensor(shape=torch.Size([3, 8]), device=cpu, dtype=torch.float32, is_shared=False),
+                input: Tensor(shape=torch.Size([3, 4]), device=cpu, dtype=torch.float32, is_shared=False),
+                output: Tensor(shape=torch.Size([3, 8]), device=cpu, dtype=torch.float32, is_shared=False)},
             batch_size=torch.Size([3]),
             device=None,
             is_shared=False)
 
     In the stateful case:
+        >>> module = torch.nn.GRUCell(4, 8)
         >>> td_module = TensorDictModule(
-        ...    module=torch.nn.GRUCell(4, 8), in_keys=["input", "hidden"], out_keys=["output"]
+        ...    module=module, in_keys=["input", "hidden"], out_keys=["output"]
         ... )
         >>> td_stateful = td_module(td.clone())
         >>> print(td_stateful)
         TensorDict(
             fields={
-                hidden: Tensor(torch.Size([3, 8]), dtype=torch.float32),
-                input: Tensor(torch.Size([3, 4]), dtype=torch.float32),
-                output: Tensor(torch.Size([3, 8]), dtype=torch.float32)},
+                hidden: Tensor(shape=torch.Size([3, 8]), device=cpu, dtype=torch.float32, is_shared=False),
+                input: Tensor(shape=torch.Size([3, 4]), device=cpu, dtype=torch.float32, is_shared=False),
+                output: Tensor(shape=torch.Size([3, 8]), device=cpu, dtype=torch.float32, is_shared=False)},
             batch_size=torch.Size([3]),
             device=None,
             is_shared=False)
 
     One can use a vmap operator to call the functional module.
-        >>> from functorch import vmap
+        >>> from torch import vmap
+        >>> from tensordict.nn.functional_modules import extract_weights_and_buffers
+        >>> params = extract_weights_and_buffers(td_module)
         >>> params_repeat = params.expand(4)
-        >>> td_vmap = vmap(td_fmodule, (None, 0))(td.clone(), params_repeat)
+        >>> print(params_repeat)
+        TensorDict(
+            fields={
+                module: TensorDict(
+                    fields={
+                        bias_hh: Tensor(shape=torch.Size([4, 24]), device=cpu, dtype=torch.float32, is_shared=False),
+                        bias_ih: Tensor(shape=torch.Size([4, 24]), device=cpu, dtype=torch.float32, is_shared=False),
+                        weight_hh: Tensor(shape=torch.Size([4, 24, 8]), device=cpu, dtype=torch.float32, is_shared=False),
+                        weight_ih: Tensor(shape=torch.Size([4, 24, 4]), device=cpu, dtype=torch.float32, is_shared=False)},
+                    batch_size=torch.Size([4]),
+                    device=None,
+                    is_shared=False)},
+            batch_size=torch.Size([4]),
+            device=None,
+            is_shared=False)
+        >>> td_vmap = vmap(td_module, (None, 0))(td.clone(), params_repeat)
         >>> print(td_vmap)
         TensorDict(
             fields={
-                hidden: Tensor(torch.Size([4, 3, 8]), dtype=torch.float32),
-                input: Tensor(torch.Size([4, 3, 4]), dtype=torch.float32),
-                output: Tensor(torch.Size([4, 3, 8]), dtype=torch.float32)},
+                hidden: Tensor(shape=torch.Size([4, 3, 8]), device=cpu, dtype=torch.float32, is_shared=False),
+                input: Tensor(shape=torch.Size([4, 3, 4]), device=cpu, dtype=torch.float32, is_shared=False),
+                output: Tensor(shape=torch.Size([4, 3, 8]), device=cpu, dtype=torch.float32, is_shared=False)},
             batch_size=torch.Size([4, 3]),
             device=None,
             is_shared=False)
 
     """
 
     def __init__(
         self,
-        module: (
-            FunctionalModule
-            | FunctionalModuleWithBuffers
-            | TensorDictModule
-            | nn.Module
-        ),
+        module: Callable,
         in_keys: Sequence[NestedKey],
         out_keys: Sequence[NestedKey],
     ) -> None:
         super().__init__()
 
-        if not out_keys:
-            raise RuntimeError(f"out_keys were not passed to {self.__class__.__name__}")
-        if not in_keys:
-            raise RuntimeError(f"in_keys were not passed to {self.__class__.__name__}")
-        _check_all_nested(out_keys)
+        _seq_of_nested_key_check(out_keys)
+        _seq_of_nested_key_check(in_keys)
+
+        if type(module) is type or not callable(module):
+            raise ValueError(
+                f"Module {module} if type {type(module)} is not callable. "
+                f"Typical accepted types are nn.Module or TensorDictModule."
+            )
         self.out_keys = [_normalize_key(key) for key in out_keys]
-        _check_all_nested(in_keys)
         self.in_keys = [_normalize_key(key) for key in in_keys]
 
         if "_" in in_keys:
             warnings.warn(
                 'key "_" is for ignoring output, it should not be used in input keys',
                 stacklevel=2,
             )
 
         self.module = module
+        make_functional(self, keep_params=True, return_params=False)
 
     @property
     def is_functional(self) -> bool:
         return _has_functorch and isinstance(
             self.module,
             (FunctionalModule, FunctionalModuleWithBuffers),
         )
@@ -390,36 +748,55 @@
         self,
         tensordict: TensorDictBase,
         tensors: list[Tensor],
         tensordict_out: TensorDictBase | None = None,
         out_keys: Iterable[NestedKey] | None = None,
     ) -> TensorDictBase:
         if out_keys is None:
-            out_keys = self.out_keys
+            out_keys = self.out_keys_source
         if tensordict_out is None:
             tensordict_out = tensordict
         for _out_key, _tensor in zip(out_keys, tensors):
             if _out_key != "_":
                 tensordict_out.set(_out_key, _tensor)
         return tensordict_out
 
     def _call_module(
         self, tensors: Sequence[Tensor], **kwargs: Any
     ) -> Tensor | Sequence[Tensor]:
         out = self.module(*tensors, **kwargs)
         return out
 
-    @dispatch
+    @dispatch(auto_batch_size=False)
+    @set_skip_existing(None)
     def forward(
         self,
         tensordict: TensorDictBase,
+        *args,
         tensordict_out: TensorDictBase | None = None,
         **kwargs: Any,
     ) -> TensorDictBase:
         """When the tensordict parameter is not set, kwargs are used to create an instance of TensorDict."""
+        if len(args):
+            tensordict_out = args[0]
+            args = args[1:]
+            # we will get rid of tensordict_out as a regular arg, because it
+            # blocks us when using vmap
+            # with stateful but functional modules: the functional module checks if
+            # it still contains parameters. If so it considers that only a "params" kwarg
+            # is indicative of what the params are, when we could potentially make a
+            # special rule for TensorDictModule that states that the second arg is
+            # likely to be the module params.
+            warnings.warn(
+                "tensordict_out will be deprecated soon.", category=DeprecationWarning
+            )
+        if len(args):
+            raise ValueError(
+                "Got a non-empty list of extra agruments, when none was expected."
+            )
         tensors = tuple(tensordict.get(in_key, None) for in_key in self.in_keys)
         try:
             tensors = self._call_module(tensors, **kwargs)
         except Exception as err:
             if any(tensor is None for tensor in tensors) and "None" in str(err):
                 none_set = {
                     key for key, tensor in zip(self.in_keys, tensors) if tensor is None
@@ -427,14 +804,16 @@
                 raise KeyError(
                     "Some tensors that are necessary for the module call may "
                     "not have not been found in the input tensordict: "
                     f"the following inputs are None: {none_set}."
                 ) from err
             else:
                 raise err
+        if isinstance(tensors, (dict, TensorDictBase)):
+            tensors = tuple(tensors.get(key, None) for key in self.out_keys)
         if not isinstance(tensors, tuple):
             tensors = (tensors,)
         tensordict_out = self._write_to_tensordict(tensordict, tensors, tensordict_out)
         return tensordict_out
 
     @property
     def device(self) -> torch.device:
@@ -449,19 +828,29 @@
             f"in_keys={self.in_keys},\n"
             f"out_keys={self.out_keys}",
             4 * " ",
         )
 
         return f"{self.__class__.__name__}(\n{fields})"
 
+    def __getattr__(self, name: str) -> Any:
+        try:
+            return super().__getattr__(name)
+        except AttributeError as err1:
+            try:
+                return getattr(super().__getattr__("module"), name)
+            except Exception as err2:
+                raise err2 from err1
+
 
-class TensorDictModuleWrapper(nn.Module):
+class TensorDictModuleWrapper(TensorDictModuleBase):
     """Wrapper class for TensorDictModule objects.
 
-    Once created, a TensorDictModuleWrapper will behave exactly as the TensorDictModule it contains except for the methods that are
+    Once created, a TensorDictModuleWrapper will behave exactly as the
+    TensorDictModule it contains except for the methods that are
     overwritten.
 
     Args:
         td_module (TensorDictModule): operator to be wrapped.
 
     """
```

## tensordict/nn/functional_modules.py

```diff
@@ -2,24 +2,37 @@
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
 from __future__ import annotations
 
 import inspect
+import re
 import types
+import warnings
 from copy import deepcopy
 from functools import wraps
 from typing import Any, Callable, Iterable
 
 import torch
 from tensordict import TensorDict
-from tensordict.tensordict import TensorDictBase
+from tensordict.tensordict import is_tensor_collection, TensorDictBase
 from torch import nn
 
+
+def set_tensor(module: "torch.nn.Module", name: str, tensor: torch.Tensor) -> None:
+    """Simplified version of torch.nn.utils._named_member_accessor."""
+    if name in module._parameters:
+        module._parameters[name] = tensor  # type: ignore[assignment]
+    elif name in module._buffers:
+        module._buffers[name] = tensor
+    else:
+        setattr(module, name, tensor)
+
+
 _RESET_OLD_TENSORDICT = True
 try:
     import torch._functorch.vmap as vmap_src
     from torch._functorch.vmap import (
         _add_batch_dim,
         _broadcast_to_and_flatten,
         _get_name,
@@ -122,14 +135,15 @@
         # the batched tensors. This will be added in _unwrap_batched
         batched_inputs = [
             arg
             if in_dim is None
             else arg.apply(
                 lambda _arg, in_dim=in_dim: _add_batch_dim(_arg, in_dim, vmap_level),
                 batch_size=[b for i, b in enumerate(arg.batch_size) if i != in_dim],
+                names=[name for i, name in enumerate(arg.names) if i != in_dim],
             )
             if isinstance(arg, TensorDictBase)
             else _add_batch_dim(arg, in_dim, vmap_level)
             for in_dim, arg in zip(flat_in_dims, flat_args)
         ]
         return tree_unflatten(batched_inputs, args_spec)
 
@@ -180,33 +194,68 @@
         flat_outputs = []
         for batched_output, out_dim in zip(flat_batched_outputs, flat_out_dims):
             if not isinstance(batched_output, TensorDictBase):
                 out = _remove_batch_dim(batched_output, vmap_level, batch_size, out_dim)
             else:
                 new_batch_size = list(batched_output.batch_size)
                 new_batch_size.insert(out_dim, batch_size)
+                new_names = list(batched_output.names)
+                new_names.insert(out_dim, None)
+                print(batched_output.names)
                 out = batched_output.apply(
                     lambda x, out_dim=out_dim: _remove_batch_dim(
                         x, vmap_level, batch_size, out_dim
                     ),
                     batch_size=new_batch_size,
+                    names=new_names,
                 )
+                print(new_batch_size, out_dim, batch_size, flat_out_dims, out.names)
             flat_outputs.append(out)
         return tree_unflatten(flat_outputs, output_spec)
 
     vmap_src._unwrap_batched = _unwrap_batched
 
 
 # Tensordict-compatible Functional modules
 
 
-def extract_weights_and_buffers(
+def _decorate_funs(
     model: nn.Module,
+    make_stateless: bool,
     funs_to_decorate: Iterable[str] | None = None,
-    recurse: bool = True,
+) -> None:
+    if funs_to_decorate is None:
+        funs_to_decorate = ["forward"]
+    _is_functional = model.__dict__.get("_functionalized", False)
+    if not _is_functional:
+        model.__dict__["_functionalized"] = True
+        model.__dict__["_decorated_funs"] = set()
+
+    for fun_to_decorate in funs_to_decorate:
+        if fun_to_decorate in model.__dict__["_decorated_funs"]:
+            continue
+        try:
+            setattr(
+                model,
+                fun_to_decorate,
+                types.MethodType(_make_decorator(model, fun_to_decorate), model),
+            )
+            model.__dict__["_decorated_funs"].add(fun_to_decorate)
+        except AttributeError:
+            continue
+    if not model.__dict__.get("_is_stateless", False):
+        model.__dict__["_is_stateless"] = make_stateless
+
+    for module in model.children():
+        # we decorate forward for the sub-modules
+        _decorate_funs(module, make_stateless=make_stateless)
+
+
+def extract_weights_and_buffers(
+    model: nn.Module,
 ) -> TensorDict:
     """Extracts the weights and buffers of a model in a tensordict, and adapts the modules to read those inputs."""
     tensordict = {}
     for name, param in list(model.named_parameters(recurse=False)):
         setattr(model, name, None)
         tensordict[name] = param
 
@@ -214,42 +263,31 @@
         setattr(model, name, None)
         tensordict[name] = param
 
     for name, module in model.named_children():
         module_tensordict = extract_weights_and_buffers(module)
         if module_tensordict is not None:
             tensordict[name] = module_tensordict
-
-    if funs_to_decorate is None:
-        funs_to_decorate = ["forward"]
-
-    if not model.__dict__.get("_functionalized", False):
-        for fun_to_decorate in funs_to_decorate:
-            try:
-                setattr(
-                    model,
-                    fun_to_decorate,
-                    types.MethodType(_make_decorator(model, fun_to_decorate), model),
-                )
-            except AttributeError:
-                continue
-    model.__dict__["_functionalized"] = True
     model.__dict__["_is_stateless"] = True
-    return TensorDict(tensordict, [], _run_checks=False)
+    return TensorDict(tensordict, batch_size=torch.Size([]), _run_checks=False)
 
 
 def _swap_state(
     model: nn.Module,
     tensordict: TensorDict,
     is_stateless: bool,
     return_old_tensordict: bool = False,
     old_tensordict: dict[str, torch.Tensor] | TensorDict | None = None,
 ) -> dict[str, torch.Tensor] | TensorDict | None:
+    was_stateless = model.__dict__.get("_is_stateless", None)
+    if was_stateless is None:
+        raise Exception(f"{model}\nhas no stateless attribute.")
     model.__dict__["_is_stateless"] = is_stateless
-    if return_old_tensordict and old_tensordict is None:
+    # return_old_tensordict = return_old_tensordict and not was_stateless
+    if old_tensordict is None:
         old_tensordict = {}
     keys = set(tensordict.keys())
     children = []
     for key, child in model.named_children():
         try:
             keys.remove(key)
         except KeyError:
@@ -258,47 +296,85 @@
             pass
         children.append(key)
         value = tensordict.get(key, None)
         if value is None:
             # faster than get(key, Tensordict(...))
             value = {}
 
-        _old_value = old_tensordict.get(key, None) if return_old_tensordict else None
+        _old_value = old_tensordict.get(key, None)
         _old_value = _swap_state(
             child,
             value,
             return_old_tensordict=return_old_tensordict,
             old_tensordict=_old_value,
             is_stateless=is_stateless,
         )
-        if old_tensordict is not None:
-            old_tensordict[key] = _old_value
+        old_tensordict[key] = _old_value
     for key in keys:
         value = tensordict.get(key)
         is_param = key in model.__dict__.get("_parameters")
         if return_old_tensordict:
             old_attr = getattr(model, key)
             if old_attr is None:
                 old_attr = torch.zeros(*value.shape, 0)
             old_tensordict[key] = old_attr
         if is_param:
             delattr(model, key)
-        setattr(model, key, value)
-    if return_old_tensordict:
+        set_tensor(model, key, value)
+    if was_stateless or not return_old_tensordict:
         return old_tensordict
-    return None
+    else:
+        return TensorDict(old_tensordict, [])
+
+
+def is_functional(module: nn.Module):
+    """Checks if :func:`make_functional` has been called on the module."""
+    return "_functionalized" in module.__dict__
 
 
 def make_functional(
     module: nn.Module,
     funs_to_decorate: Iterable[str] | None = None,
+    keep_params: bool = False,
+    return_params: bool = True,
 ) -> TensorDict:
-    """Converts a nn.Module to a functional module in-place, and returns its params."""
-    params = extract_weights_and_buffers(module, funs_to_decorate=funs_to_decorate)
-    return params
+    """Converts a nn.Module to a functional module in-place, and returns its params.
+
+    Args:
+        module (torch.nn.Module): module that is to be made functional.
+        funs_to_decorate (iterable of str, optional): each string must correspond
+            to a function belonging to module. For nested modules, the
+            :meth:`torch.nn.Module.forward` method will be decorated.
+            Defaults to ``"forward"``.
+        keep_params (bool, optional): if ``True``, the module will keep its
+            parameters. Defaults to ``False``.
+        return_params (bool, optional): if ``True``, the parameters will
+            be collected in a nested tensordict and returned. If ``False``,
+            the module will be made functional but still be stateful.
+
+    """
+    _is_stateless = module.__dict__.get("_is_stateless", False)
+    _decorate_funs(
+        module,
+        funs_to_decorate=funs_to_decorate,
+        make_stateless=not keep_params,
+    )
+    if return_params and not _is_stateless:
+        params = extract_weights_and_buffers(
+            module,
+        )
+        if keep_params:
+            repopulate_module(module, params)
+        return params
+    elif return_params and _is_stateless:
+        raise RuntimeError(
+            "Calling make_functional with return_params=True on a functional, stateless module. "
+        )
+    elif not keep_params:
+        extract_weights_and_buffers(module)
 
 
 def get_functional(
     module: nn.Module,
     funs_to_decorate: Iterable[str] | None = None,
 ) -> nn.Module:
     """Converts a nn.Module to a functional module in-place, and returns a stateful version of this module that can be used in functional settings."""
@@ -306,14 +382,72 @@
     out = deepcopy(module)
     repopulate_module(module, params)
     return out
 
 
 def _make_decorator(module: nn.Module, fun_name: str) -> Callable:
     fun = getattr(module, fun_name)
+
+    @wraps(fun)
+    def new_fun(self, *args, **kwargs):
+        # 3 use cases: (1) params is the last arg, (2) params is in kwargs, (3) no params
+        _is_stateless = self.__dict__.get("_is_stateless", False)
+        params = kwargs.pop("params", None)
+
+        from tensordict.nn.common import TensorDictModuleBase
+
+        if isinstance(self, TensorDictModuleBase):
+            if (
+                params is None
+                and len(args) == 2
+                and all(is_tensor_collection(item) for item in args)
+            ):
+                params = args[1]
+                args = args[:1]
+        elif (len(args) and is_tensor_collection(args[0])) or "tensordict" in kwargs:
+            warnings.warn(
+                "You are passing a tensordict/tensorclass instance to a module that "
+                "does not inherit from TensorDictModuleBase. This may lead to unexpected "
+                "behaviours with functional calls."
+            )
+        if _is_stateless or params is not None:
+            if params is None:
+                params = args[-1]
+                args = args[:-1]
+                # get the previous params, and tell the submodules not to look for params anymore
+            old_params = _assign_params(
+                self, params, make_stateless=False, return_old_tensordict=True
+            )
+            try:
+                out = getattr(type(self), fun_name)(self, *args, **kwargs)
+            finally:
+                # reset the previous params, and tell the submodules to look for params
+                _assign_params(
+                    self,
+                    old_params,
+                    make_stateless=_is_stateless,
+                    return_old_tensordict=False,
+                )
+            return out
+        else:
+            try:
+                return getattr(type(self), fun_name)(self, *args, **kwargs)
+            except TypeError as err:
+                pattern = r".*takes \d+ positional arguments but \d+ were given|got multiple values for argument"
+                pattern = re.compile(pattern)
+                if pattern.search(str(err)) and isinstance(args[-1], TensorDictBase):
+                    # this is raised whenever the module is an nn.Module (not a TensorDictModuleBase)
+                    raise TypeError(
+                        "It seems you tried to provide the parameters as an argument to the module when the module was not stateless. "
+                        "If this is the case, this error should vanish by providing the parameters using the ``module(..., params=params)`` "
+                        "syntax."
+                    ) from err
+                else:
+                    raise err
+
     # we need to update the signature so that params can be the last positional arg
     oldsig = inspect.signature(fun)
     if "_forward_unimplemented" in fun.__name__:
         raise AttributeError("_forward_unimplemented not supported")
     # search if a VAR_POSITIONAL or VAR_KEYWORD is present
     # if yes insert step parameter before it, else insert it in last position
     params = list(oldsig.parameters.values())
@@ -342,52 +476,27 @@
     while name in oldsig.parameters:
         name += "_"
     newparam = inspect.Parameter(name, out_type, default=None)
     params.insert(i, newparam)
     # we can now build the signature for the wrapper function
     sig = oldsig.replace(parameters=params)
 
-    @wraps(fun)
-    def new_fun(self, *args, **kwargs):
-        # 3 use cases: (1) params is the last arg, (2) params is in kwargs, (3) no params
-        if self.__dict__.get("_is_stateless", False):
-            params = kwargs.pop("params", None)
-            if params is None:
-                params = args[-1]
-                args = args[:-1]
-                # get the previous params, and tell the submodules not to look for params anymore
-            old_params = _assign_params(
-                self, params, make_stateless=False, return_old_tensordict=True
-            )
-            try:
-                out = getattr(type(self), fun_name)(self, *args, **kwargs)
-            finally:
-                # reset the previous params, and tell the submodules to look for params
-                _assign_params(
-                    self, old_params, make_stateless=True, return_old_tensordict=True
-                )
-            return out
-        else:
-            return getattr(type(self), fun_name)(self, *args, **kwargs)
-
     new_fun.__signature__ = sig
     return new_fun
 
 
 def _assign_params(
     module: nn.Module,
     params: TensorDict,
     make_stateless: bool,
     return_old_tensordict: bool,
 ) -> TensorDict | None:
     if params is not None:
-        out = _swap_state(module, params, make_stateless, return_old_tensordict)
-        if out is not None:
-            return TensorDict(out, [], _run_checks=False)
-        return None
+        return _swap_state(module, params, make_stateless, return_old_tensordict)
+
     return None
 
 
 def repopulate_module(model: nn.Module, tensordict: TensorDict) -> nn.Module:
     """Repopulates a module with its parameters, presented as a nested TensorDict."""
     _swap_state(model, tensordict, is_stateless=False)
     return model
```

## tensordict/nn/probabilistic.py

```diff
@@ -2,70 +2,135 @@
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
 from __future__ import annotations
 
 import re
+from enum import auto, Enum
 from textwrap import indent
-from typing import Any, Sequence
+from typing import Any, Callable, Sequence
+from warnings import warn
 
-import torch.nn as nn
-from tensordict.nn.common import _check_all_nested, _check_all_str, TensorDictModule
+from tensordict._contextlib import _DecoratorContextManager
+
+from tensordict.nn.common import dispatch, TensorDictModule, TensorDictModuleBase
 from tensordict.nn.distributions import Delta, distributions_maps
-from tensordict.nn.functional_modules import repopulate_module
 from tensordict.nn.sequence import TensorDictSequential
+
+from tensordict.nn.utils import set_skip_existing
 from tensordict.tensordict import TensorDictBase
+from tensordict.utils import _seq_of_nested_key_check
 from torch import distributions as D, Tensor
-from torch.autograd.grad_mode import _DecoratorContextManager
 
 __all__ = ["ProbabilisticTensorDictModule", "ProbabilisticTensorDictSequential"]
 
 
-_INTERACTION_MODE = None
+class InteractionType(Enum):
+    MODE = auto()
+    MEDIAN = auto()
+    MEAN = auto()
+    RANDOM = auto()
+
+    @classmethod
+    def from_str(cls, type_str: str) -> InteractionType:
+        """Return the interaction_type with name matched to the provided string (case insensitive)."""
+        for member_type in cls:
+            if member_type.name == type_str.upper():
+                return member_type
+        raise ValueError(f"The provided interaction type {type_str} is unsupported!")
+
+
+_INTERACTION_TYPE: InteractionType | None = None
+
+
+def _insert_interaction_mode_deprecation_warning(
+    prefix: str = "",
+) -> Callable[[str, Warning, int], None]:
+    return warn(
+        (
+            f"{prefix}interaction_mode is deprecated for naming clarity. "
+            f"Please use {prefix}interaction_type with InteractionType enum instead."
+        ),
+        DeprecationWarning,
+        stacklevel=2,
+    )
+
+
+def interaction_type() -> InteractionType | None:
+    """Returns the current sampling type."""
+    return _INTERACTION_TYPE
 
 
 def interaction_mode() -> str | None:
-    """Returns the current sampling mode."""
-    return _INTERACTION_MODE
+    """*Deprecated* Returns the current sampling mode."""
+    _insert_interaction_mode_deprecation_warning()
+    type = interaction_type()
+    return type.name.lower() if type else None
 
 
 class set_interaction_mode(_DecoratorContextManager):
-    """Sets the sampling mode of all ProbabilisticTDModules to the desired mode.
+    """*Deprecated* Sets the sampling mode of all ProbabilisticTDModules to the desired mode.
 
     Args:
         mode (str): mode to use when the policy is being called.
     """
 
-    def __init__(self, mode: str = "mode") -> None:
+    def __init__(self, mode: str | None = "mode") -> None:
+        _insert_interaction_mode_deprecation_warning("set_")
         super().__init__()
-        self.mode = mode
+        self.mode = InteractionType.from_str(mode) if mode else None
 
     def clone(self) -> set_interaction_mode:
         # override this method if your children class takes __init__ parameters
         return self.__class__(self.mode)
 
     def __enter__(self) -> None:
-        global _INTERACTION_MODE
-        self.prev = _INTERACTION_MODE
-        _INTERACTION_MODE = self.mode
+        global _INTERACTION_TYPE
+        self.prev = _INTERACTION_TYPE
+        _INTERACTION_TYPE = self.mode
+
+    def __exit__(self, exc_type: Any, exc_value: Any, traceback: Any) -> None:
+        global _INTERACTION_TYPE
+        _INTERACTION_TYPE = self.prev
+
+
+class set_interaction_type(_DecoratorContextManager):
+    """Sets all ProbabilisticTDModules sampling to the desired type.
+
+    Args:
+        type (InteractionType): sampling type to use when the policy is being called.
+    """
+
+    def __init__(self, type: InteractionType | None = InteractionType.MODE) -> None:
+        super().__init__()
+        self.type = type
+
+    def clone(self) -> set_interaction_type:
+        # override this method if your children class takes __init__ parameters
+        return self.__class__(self.type)
+
+    def __enter__(self) -> None:
+        global _INTERACTION_TYPE
+        self.prev = _INTERACTION_TYPE
+        _INTERACTION_TYPE = self.type
 
     def __exit__(self, exc_type: Any, exc_value: Any, traceback: Any) -> None:
-        global _INTERACTION_MODE
-        _INTERACTION_MODE = self.prev
+        global _INTERACTION_TYPE
+        _INTERACTION_TYPE = self.prev
 
 
-class ProbabilisticTensorDictModule(nn.Module):
+class ProbabilisticTensorDictModule(TensorDictModuleBase):
     """A probabilistic TD Module.
 
     `ProbabilisticTensorDictModule` is a non-parametric module representing a
     probability distribution. It reads the distribution parameters from an input
     TensorDict using the specified `in_keys`. The output is sampled given some rule,
-    specified by the input :obj:`default_interaction_mode` argument and the
-    :obj:`interaction_mode()` global function.
+    specified by the input :obj:`default_interaction_type` argument and the
+    :obj:`interaction_type()` global function.
 
     :obj:`ProbabilisticTensorDictModule` can be used to construct the distribution
     (through the :obj:`get_dist()` method) and/or sampling from this distribution
     (through a regular :obj:`__call__()` to the module).
 
     A :obj:`ProbabilisticTensorDictModule` instance has two main features:
     - It reads and writes TensorDict objects
@@ -88,38 +153,47 @@
             the distribution class of interest, e.g. :obj:`"loc"` and :obj:`"scale"` for
             the Normal distribution and similar. If in_keys is a dictionary,, the keys
             are the keys of the distribution and the values are the keys in the
             tensordict that will get match to the corresponding distribution keys.
         out_keys (str or iterable of str): keys where the sampled values will be
             written. Importantly, if these keys are found in the input TensorDict, the
             sampling step will be skipped.
-        default_interaction_mode (str, optional): default method to be used to retrieve
-            the output value. Should be one of: 'mode', 'median', 'mean' or 'random'
+        default_interaction_mode (str, optional): *Deprecated* keyword-only argument.
+            Please use default_interaction_type instead.
+        default_interaction_type (InteractionType, optional): keyword-only argument.
+            Default method to be used to retrieve
+            the output value. Should be one of InteractionType: MODE, MEDIAN, MEAN or RANDOM
             (in which case the value is sampled randomly from the distribution). Default
-            is 'mode'.
+            is MODE.
             Note: When a sample is drawn, the :obj:`ProbabilisticTDModule` instance will
-            first look for the interaction mode dictated by the `interaction_mode()`
+            first look for the interaction mode dictated by the `interaction_type()`
             global function. If this returns `None` (its default value), then the
-            `default_interaction_mode` of the `ProbabilisticTDModule` instance will be
-            used. Note that DataCollector instances will use `set_interaction_mode` to
-            `"random"` by default.
-        distribution_class (Type, optional): a torch.distributions.Distribution class to
-            be used for sampling. Default is Delta.
-        distribution_kwargs (dict, optional): kwargs to be passed to the distribution.
-        return_log_prob (bool, optional): if True, the log-probability of the
+            `default_interaction_type` of the `ProbabilisticTDModule` instance will be
+            used. Note that DataCollector instances will use `set_interaction_type` to
+            `RANDOM` by default.
+        distribution_class (Type, optional): keyword-only argument.
+            A :class:`torch.distributions.Distribution` class to
+            be used for sampling.
+            Default is :class:`tensordict.nn.distributions.Delta`.
+        distribution_kwargs (dict, optional): keyword-only argument.
+            Keyword-argument pairs to be passed to the distribution.
+        return_log_prob (bool, optional): keyword-only argument.
+            If ``True``, the log-probability of the
             distribution sample will be written in the tensordict with the key
-            `'sample_log_prob'`. Default is `False`.
-        cache_dist (bool, optional): EXPERIMENTAL: if True, the parameters of the
+            `'sample_log_prob'`. Default is ``False``.
+        cache_dist (bool, optional): keyword-only argument.
+            EXPERIMENTAL: if ``True``, the parameters of the
             distribution (i.e. the output of the module) will be written to the
             tensordict along with the sample. Those parameters can be used to re-compute
             the original distribution later on (e.g. to compute the divergence between
             the distribution used to sample the action and the updated distribution in
-            PPO). Default is `False`.
-        n_empirical_estimate (int, optional): number of samples to compute the empirical
-            mean when it is not available. Default is 1000
+            PPO). Default is ``False``.
+        n_empirical_estimate (int, optional): keyword-only argument.
+            Number of samples to compute the empirical
+            mean when it is not available. Defaults to 1000.
 
     Examples:
         >>> import torch
         >>> from tensordict import TensorDict
         >>> from tensordict.nn import (
         ...     ProbabilisticTensorDictModule,
         ...     ProbabilisticTensorDictSequential,
@@ -162,15 +236,15 @@
             batch_size=torch.Size([3]),
             device=None,
             is_shared=False)
         >>> dist = td_module.get_dist(td, params=params)
         >>> print(dist)
         Normal(loc: torch.Size([3, 4]), scale: torch.Size([3, 4]))
         >>> # we can also apply the module to the TensorDict with vmap
-        >>> from functorch import vmap
+        >>> from torch import vmap
         >>> params = params.expand(4)
         >>> td_vmap = vmap(td_module, (None, 0))(td, params)
         >>> print(td_vmap)
         TensorDict(
             fields={
                 action: Tensor(torch.Size([4, 3, 4]), dtype=torch.float32),
                 hidden: Tensor(torch.Size([4, 3, 8]), dtype=torch.float32),
@@ -181,53 +255,71 @@
                 scale: Tensor(torch.Size([4, 3, 4]), dtype=torch.float32)},
             batch_size=torch.Size([4, 3]),
             device=None,
             is_shared=False)
 
     """
 
+    SAMPLE_LOG_PROB_KEY = "sample_log_prob"
+
     def __init__(
         self,
         in_keys: str | Sequence[str] | dict,
         out_keys: str | Sequence[str] | None = None,
-        default_interaction_mode: str = "mode",
+        *,
+        default_interaction_mode: str | None = None,
+        default_interaction_type: InteractionType = InteractionType.MODE,
         distribution_class: type = Delta,
         distribution_kwargs: dict | None = None,
         return_log_prob: bool = False,
         cache_dist: bool = False,
         n_empirical_estimate: int = 1000,
     ) -> None:
         super().__init__()
         if isinstance(in_keys, str):
             in_keys = [in_keys]
         if isinstance(out_keys, str):
             out_keys = [out_keys]
         elif out_keys is None:
-            out_keys = []
+            out_keys = ["_"]
         if not isinstance(in_keys, dict):
             in_keys = {param_key: param_key for param_key in in_keys}
+        else:
+            # keys must be strings
+            if not all(isinstance(v, str) for v in in_keys.keys()):
+                raise ValueError(
+                    f"in_keys keys should all be strings. "
+                    f"{self.__class__.__name__} got {in_keys}"
+                )
 
+        _seq_of_nested_key_check(out_keys)
+        _seq_of_nested_key_check(tuple(in_keys.values()))
         self.out_keys = out_keys
-        _check_all_nested(self.out_keys)
         self.in_keys = in_keys
-        # arguments must be strings
-        _check_all_str(self.in_keys.keys())
-        _check_all_nested(self.in_keys.values())
 
-        self.default_interaction_mode = default_interaction_mode
+        if default_interaction_mode is not None:
+            _insert_interaction_mode_deprecation_warning("default_")
+            self.default_interaction_type = InteractionType.from_str(
+                default_interaction_mode
+            )
+        else:
+            self.default_interaction_type = default_interaction_type
+
         if isinstance(distribution_class, str):
             distribution_class = distributions_maps.get(distribution_class.lower())
         self.distribution_class = distribution_class
         self.distribution_kwargs = (
             distribution_kwargs if distribution_kwargs is not None else {}
         )
         self.n_empirical_estimate = n_empirical_estimate
         self._dist = None
         self.cache_dist = cache_dist if hasattr(distribution_class, "update") else False
         self.return_log_prob = return_log_prob
+        if self.return_log_prob:
+            self.out_keys.append(self.SAMPLE_LOG_PROB_KEY)
 
     def get_dist(self, tensordict: TensorDictBase) -> D.Distribution:
         try:
             dist_kwargs = {
                 dist_key: tensordict[td_key]
                 for dist_key, td_key in self.in_keys.items()
             }
@@ -242,99 +334,103 @@
                 raise TypeError(
                     f"TensorDict with keys {tensordict.keys()} does not match the distribution {self.distribution_class} keywords."
                 )
             else:
                 raise err
         return dist
 
+    @dispatch(auto_batch_size=False)
+    @set_skip_existing(None)
     def forward(
         self,
         tensordict: TensorDictBase,
         tensordict_out: TensorDictBase | None = None,
         _requires_sample: bool = True,
     ) -> TensorDictBase:
         if tensordict_out is None:
             tensordict_out = tensordict
 
         dist = self.get_dist(tensordict)
         if _requires_sample:
-            out_tensors = self._dist_sample(dist, interaction_mode=interaction_mode())
+            out_tensors = self._dist_sample(dist, interaction_type=interaction_type())
             if isinstance(out_tensors, Tensor):
                 out_tensors = (out_tensors,)
             tensordict_out.update(
                 {key: value for key, value in zip(self.out_keys, out_tensors)}
             )
             if self.return_log_prob:
                 log_prob = dist.log_prob(*out_tensors)
-                tensordict_out.set("sample_log_prob", log_prob)
+                tensordict_out.set(self.SAMPLE_LOG_PROB_KEY, log_prob)
         elif self.return_log_prob:
-            out_tensors = [tensordict.get(key) for key in self.out_keys]
+            out_tensors = [
+                tensordict.get(key)
+                for key in self.out_keys
+                if key != self.SAMPLE_LOG_PROB_KEY
+            ]
             log_prob = dist.log_prob(*out_tensors)
-            tensordict_out.set("sample_log_prob", log_prob)
+            tensordict_out.set(self.SAMPLE_LOG_PROB_KEY, log_prob)
             # raise RuntimeError(
             #     "ProbabilisticTensorDictModule.return_log_prob = True is incompatible with settings in which "
             #     "the submodule is responsible for sampling. To manually gather the log-probability, call first "
             #     "\n>>> dist, tensordict = tensordict_module.get_dist(tensordict)"
             #     "\n>>> tensordict.set('sample_log_prob', dist.log_prob(tensordict.get(sample_key))"
             # )
         return tensordict_out
 
     def _dist_sample(
         self,
         dist: D.Distribution,
-        interaction_mode: bool = None,
+        interaction_type: InteractionType | None = None,
     ) -> tuple[Tensor, ...] | Tensor:
-        if interaction_mode is None or interaction_mode == "":
-            interaction_mode = self.default_interaction_mode
-        if not isinstance(dist, D.Distribution):
-            raise TypeError(f"type {type(dist)} not recognised by _dist_sample")
+        if interaction_type is None:
+            interaction_type = self.default_interaction_type
 
-        if interaction_mode == "mode":
-            if hasattr(dist, "mode"):
+        if interaction_type is InteractionType.MODE:
+            try:
                 return dist.mode
-            else:
+            except AttributeError:
                 raise NotImplementedError(
                     f"method {type(dist)}.mode is not implemented"
                 )
 
-        elif interaction_mode == "median":
-            if hasattr(dist, "median"):
+        elif interaction_type is InteractionType.MEDIAN:
+            try:
                 return dist.median
-            else:
+            except AttributeError:
                 raise NotImplementedError(
                     f"method {type(dist)}.median is not implemented"
                 )
 
-        elif interaction_mode == "mean":
+        elif interaction_type is InteractionType.MEAN:
             try:
                 return dist.mean
             except (AttributeError, NotImplementedError):
                 if dist.has_rsample:
                     return dist.rsample((self.n_empirical_estimate,)).mean(0)
                 else:
                     return dist.sample((self.n_empirical_estimate,)).mean(0)
 
-        elif interaction_mode == "random":
+        elif interaction_type is InteractionType.RANDOM:
             if dist.has_rsample:
                 return dist.rsample()
             else:
                 return dist.sample()
         else:
-            raise NotImplementedError(f"unknown interaction_mode {interaction_mode}")
+            raise NotImplementedError(f"unknown interaction_type {interaction_type}")
 
 
 class ProbabilisticTensorDictSequential(TensorDictSequential):
     """A sequence of TensorDictModules ending in a ProbabilistictTensorDictModule.
 
     Similarly to :obj:`TensorDictSequential`, but enforces that the final module in the
     sequence is an :obj:`ProbabilisticTensorDictModule` and also exposes ``get_dist``
     method to recover the distribution object from the ``ProbabilisticTensorDictModule``
 
     Args:
-         modules (iterable of TensorDictModules): ordered sequence of TensorDictModule
+         modules (sequence of TensorDictModules): ordered sequence of TensorDictModule
             instances, terminating in ProbabilisticTensorDictModule, to be run
             sequentially.
          partial_tolerant (bool, optional): if True, the input tensordict can miss some
             of the input keys. If so, the only module that will be executed are those
             who can be executed given the keys that are present. Also, if the input
             tensordict is a lazy stack of tensordicts AND if partial_tolerant is
             :obj:`True` AND if the stack does not have the required keys, then
@@ -366,27 +462,32 @@
         # key we wont be sampling it again, in that case
         # ProbabilisticTensorDictSequential is presumably used to return the
         # distribution using `get_dist` or to sample log_probabilities
         _, out_keys = self._compute_in_and_out_keys(modules[:-1])
         self._requires_sample = modules[-1].out_keys[0] not in set(out_keys)
         super().__init__(*modules, partial_tolerant=partial_tolerant)
 
+    @property
+    def det_part(self):
+        if not hasattr(self, "_det_part"):
+            # we use a list to avoid having the submodules listed in module.modules()
+            self._det_part = [TensorDictSequential(*self.module[:-1])]
+        return self._det_part[0]
+
     def get_dist_params(
         self,
         tensordict: TensorDictBase,
         tensordict_out: TensorDictBase | None = None,
         **kwargs,
     ) -> tuple[D.Distribution, TensorDictBase]:
-        tds = TensorDictSequential(*self.module[:-1])
-        if self.__dict__.get("_is_stateless", False):
-            tds = repopulate_module(tds, kwargs.pop("params"))
-        mode = interaction_mode()
-        if mode is None:
-            mode = self.module[-1].default_interaction_mode
-        with set_interaction_mode(mode):
+        tds = self.det_part
+        type = interaction_type()
+        if type is None:
+            type = self.module[-1].default_interaction_type
+        with set_interaction_type(type):
             return tds(tensordict, tensordict_out, **kwargs)
 
     def get_dist(
         self,
         tensordict: TensorDictBase,
         tensordict_out: TensorDictBase | None = None,
         **kwargs,
@@ -395,14 +496,16 @@
         tensordict_out = self.get_dist_params(tensordict, tensordict_out, **kwargs)
         return self.build_dist_from_params(tensordict_out)
 
     def build_dist_from_params(self, tensordict: TensorDictBase) -> D.Distribution:
         """Construct a distribution from the input parameters. Other modules in the sequence are not evaluated."""
         return self.module[-1].get_dist(tensordict)
 
+    @dispatch(auto_batch_size=False)
+    @set_skip_existing(None)
     def forward(
         self,
         tensordict: TensorDictBase,
         tensordict_out: TensorDictBase | None = None,
         **kwargs,
     ) -> TensorDictBase:
         tensordict_out = self.get_dist_params(tensordict, tensordict_out, **kwargs)
```

## tensordict/nn/sequence.py

```diff
@@ -4,14 +4,16 @@
 # LICENSE file in the root directory of this source tree.
 
 from __future__ import annotations
 
 from copy import deepcopy
 from typing import Any, Iterable
 
+from tensordict.nn.utils import set_skip_existing
+
 _has_functorch = False
 try:
     import functorch
 
     _has_functorch = True
 except ImportError:
     print(
@@ -29,28 +31,57 @@
 
 __all__ = ["TensorDictSequential"]
 
 
 class TensorDictSequential(TensorDictModule):
     """A sequence of TensorDictModules.
 
+    By default, :class:`TensorDictSequential` subclasses are always functional,
+    meaning that they support the ``td_module(input, params=params)`` function
+    call signature.
+
     Similarly to :obj:`nn.Sequence` which passes a tensor through a chain of mappings that read and write a single tensor
     each, this module will read and write over a tensordict by querying each of the input modules.
     When calling a :obj:`TensorDictSequencial` instance with a functional module, it is expected that the parameter lists (and
     buffers) will be concatenated in a single list.
 
     Args:
          modules (iterable of TensorDictModules): ordered sequence of TensorDictModule instances to be run sequentially.
          partial_tolerant (bool, optional): if True, the input tensordict can miss some of the input keys.
             If so, the only module that will be executed are those who can be executed given the keys that
             are present.
             Also, if the input tensordict is a lazy stack of tensordicts AND if partial_tolerant is :obj:`True` AND if the
             stack does not have the required keys, then TensorDictSequential will scan through the sub-tensordicts
             looking for those that have the required keys, if any.
 
+    Examples:
+        >>> import torch
+        >>> from tensordict import TensorDict
+        >>> from tensordict.nn import TensorDictModule, TensorDictSequential
+        >>> torch.manual_seed(0)
+        >>> module = TensorDictSequential(
+        ...     TensorDictModule(lambda x: x+1, in_keys=["x"], out_keys=["x+1"]),
+        ...     TensorDictModule(nn.Linear(3, 4), in_keys=["x+1"], out_keys=["w*(x+1)+b"]),
+        ... )
+        >>> # with tensordict input
+        >>> print(module(TensorDict({"x": torch.zeros(3)}, [])))
+        TensorDict(
+            fields={
+                w*(x+1)+b: Tensor(shape=torch.Size([4]), device=cpu, dtype=torch.float32, is_shared=False),
+                x+1: Tensor(shape=torch.Size([3]), device=cpu, dtype=torch.float32, is_shared=False),
+                x: Tensor(shape=torch.Size([3]), device=cpu, dtype=torch.float32, is_shared=False)},
+            batch_size=torch.Size([]),
+            device=None,
+            is_shared=False)
+        >>> # with tensor input: returns all the output keys in the order of the modules, ie "x+1" and "w*(x+1)+b"
+        >>> module(x=torch.zeros(3))
+        (tensor([1., 1., 1.]), tensor([-0.7214, -0.8748,  0.1571, -0.1138], grad_fn=<AddBackward0>))
+        >>> module(torch.zeros(3))
+        (tensor([1., 1., 1.]), tensor([-0.7214, -0.8748,  0.1571, -0.1138], grad_fn=<AddBackward0>))
+
     TensorDictSequence supports functional, modular and vmap coding:
     Examples:
         >>> import torch
         >>> from tensordict import TensorDict
         >>> from tensordict.nn import (
         ...     ProbabilisticTensorDictModule,
         ...     ProbabilisticTensorDictSequential,
@@ -60,16 +91,16 @@
         >>> from tensordict.nn.distributions import NormalParamExtractor
         >>> from tensordict.nn.functional_modules import make_functional
         >>> from torch.distributions import Normal
         >>> td = TensorDict({"input": torch.randn(3, 4)}, [3,])
         >>> net1 = torch.nn.Linear(4, 8)
         >>> module1 = TensorDictModule(net1, in_keys=["input"], out_keys=["params"])
         >>> normal_params = TensorDictModule(
-                NormalParamExtractor(), in_keys=["params"], out_keys=["loc", "scale"]
-            )
+        ...      NormalParamExtractor(), in_keys=["params"], out_keys=["loc", "scale"]
+        ...  )
         >>> td_module1 = ProbabilisticTensorDictSequential(
         ...     module1,
         ...     normal_params,
         ...     ProbabilisticTensorDictModule(
         ...         in_keys=["loc", "scale"],
         ...         out_keys=["hidden"],
         ...         distribution_class=Normal,
@@ -82,39 +113,39 @@
         ... )
         >>> td_module = TensorDictSequential(td_module1, td_module2)
         >>> params = make_functional(td_module)
         >>> _ = td_module(td, params=params)
         >>> print(td)
         TensorDict(
             fields={
-                hidden: Tensor(torch.Size([3, 4]), dtype=torch.float32),
-                input: Tensor(torch.Size([3, 4]), dtype=torch.float32),
-                loc: Tensor(torch.Size([3, 4]), dtype=torch.float32),
-                output: Tensor(torch.Size([3, 8]), dtype=torch.float32),
-                params: Tensor(torch.Size([3, 8]), dtype=torch.float32),
-                sample_log_prob: Tensor(torch.Size([3, 4]), dtype=torch.float32),
-                scale: Tensor(torch.Size([3, 4]), dtype=torch.float32)},
+                hidden: Tensor(shape=torch.Size([3, 4]), device=cpu, dtype=torch.float32, is_shared=False),
+                input: Tensor(shape=torch.Size([3, 4]), device=cpu, dtype=torch.float32, is_shared=False),
+                loc: Tensor(shape=torch.Size([3, 4]), device=cpu, dtype=torch.float32, is_shared=False),
+                output: Tensor(shape=torch.Size([3, 8]), device=cpu, dtype=torch.float32, is_shared=False),
+                params: Tensor(shape=torch.Size([3, 8]), device=cpu, dtype=torch.float32, is_shared=False),
+                sample_log_prob: Tensor(shape=torch.Size([3, 4]), device=cpu, dtype=torch.float32, is_shared=False),
+                scale: Tensor(shape=torch.Size([3, 4]), device=cpu, dtype=torch.float32, is_shared=False)},
             batch_size=torch.Size([3]),
             device=None,
             is_shared=False)
 
     In the vmap case:
-        >>> from functorch import vmap
+        >>> from torch import vmap
         >>> params = params.expand(4)
         >>> td_vmap = vmap(td_module, (None, 0))(td, params)
         >>> print(td_vmap)
         TensorDict(
             fields={
-                hidden: Tensor(torch.Size([4, 3, 4]), dtype=torch.float32),
-                input: Tensor(torch.Size([4, 3, 4]), dtype=torch.float32),
-                loc: Tensor(torch.Size([4, 3, 4]), dtype=torch.float32),
-                output: Tensor(torch.Size([4, 3, 8]), dtype=torch.float32),
-                params: Tensor(torch.Size([4, 3, 8]), dtype=torch.float32),
-                sample_log_prob: Tensor(torch.Size([4, 3, 4]), dtype=torch.float32),
-                scale: Tensor(torch.Size([4, 3, 4]), dtype=torch.float32)},
+                hidden: Tensor(shape=torch.Size([4, 3, 4]), device=cpu, dtype=torch.float32, is_shared=False),
+                input: Tensor(shape=torch.Size([4, 3, 4]), device=cpu, dtype=torch.float32, is_shared=False),
+                loc: Tensor(shape=torch.Size([4, 3, 4]), device=cpu, dtype=torch.float32, is_shared=False),
+                output: Tensor(shape=torch.Size([4, 3, 8]), device=cpu, dtype=torch.float32, is_shared=False),
+                params: Tensor(shape=torch.Size([4, 3, 8]), device=cpu, dtype=torch.float32, is_shared=False),
+                sample_log_prob: Tensor(shape=torch.Size([4, 3, 4]), device=cpu, dtype=torch.float32, is_shared=False),
+                scale: Tensor(shape=torch.Size([4, 3, 4]), device=cpu, dtype=torch.float32, is_shared=False)},
             batch_size=torch.Size([4, 3]),
             device=None,
             is_shared=False)
 
     """
 
     module: nn.ModuleList
@@ -174,83 +205,233 @@
         self,
         in_keys: Iterable[NestedKey] | None = None,
         out_keys: Iterable[NestedKey] | None = None,
     ) -> TensorDictSequential:
         """Returns a new TensorDictSequential with only the modules that are necessary to compute the given output keys with the given input keys.
 
         Args:
-            in_keys: input keys of the subsequence we want to select
-            out_keys: output keys of the subsequence we want to select
+            in_keys: input keys of the subsequence we want to select.
+                All the keys absent from ``in_keys`` will be considered as
+                non-relevant, and modules that *just* take these keys as inputs
+                will be discarded.
+                The resulting sequential module will follow the pattern "all
+                the modules which output will be affected by a different value
+                for any in <in_keys>".
+                If none is provided, the module's ``in_keys`` are assumed.
+            out_keys: output keys of the subsequence we want to select.
+                Only the modules that are necessary to get the ``out_keys``
+                will be found in the resulting sequence.
+                The resulting sequential module will follow the pattern "all
+                the modules that condition the value or <out_keys> entries."
+                If none is provided, the module's ``out_keys`` are assumed.
 
         Returns:
             A new TensorDictSequential with only the modules that are necessary acording to the given input and output keys.
+
+        Examples:
+            >>> from tensordict.nn import TensorDictSequential as Seq, TensorDictModule as Mod
+            >>> idn = lambda x: x
+            >>> module = Seq(
+            ...     Mod(idn, in_keys=["a"], out_keys=["b"]),
+            ...     Mod(idn, in_keys=["b"], out_keys=["c"]),
+            ...     Mod(idn, in_keys=["c"], out_keys=["d"]),
+            ...     Mod(idn, in_keys=["a"], out_keys=["e"]),
+            ... )
+            >>> # select all modules whose output depend on "a"
+            >>> module.select_subsequence(in_keys=["a"])
+            TensorDictSequential(
+                module=ModuleList(
+                  (0): TensorDictModule(
+                      module=<function <lambda> at 0x126ed1ca0>,
+                      device=cpu,
+                      in_keys=['a'],
+                      out_keys=['b'])
+                  (1): TensorDictModule(
+                      module=<function <lambda> at 0x126ed1ca0>,
+                      device=cpu,
+                      in_keys=['b'],
+                      out_keys=['c'])
+                  (2): TensorDictModule(
+                      module=<function <lambda> at 0x126ed1ca0>,
+                      device=cpu,
+                      in_keys=['c'],
+                      out_keys=['d'])
+                  (3): TensorDictModule(
+                      module=<function <lambda> at 0x126ed1ca0>,
+                      device=cpu,
+                      in_keys=['a'],
+                      out_keys=['e'])
+                ),
+                device=cpu,
+                in_keys=['a'],
+                out_keys=['b', 'c', 'd', 'e'])
+            >>> # select all modules whose output depend on "c"
+            >>> module.select_subsequence(in_keys=["c"])
+            TensorDictSequential(
+                module=ModuleList(
+                  (0): TensorDictModule(
+                      module=<function <lambda> at 0x126ed1ca0>,
+                      device=cpu,
+                      in_keys=['c'],
+                      out_keys=['d'])
+                ),
+                device=cpu,
+                in_keys=['c'],
+                out_keys=['d'])
+            >>> # select all modules that affect the value of "c"
+            >>> module.select_subsequence(out_keys=["c"])
+            TensorDictSequential(
+                module=ModuleList(
+                  (0): TensorDictModule(
+                      module=<function <lambda> at 0x126ed1ca0>,
+                      device=cpu,
+                      in_keys=['a'],
+                      out_keys=['b'])
+                  (1): TensorDictModule(
+                      module=<function <lambda> at 0x126ed1ca0>,
+                      device=cpu,
+                      in_keys=['b'],
+                      out_keys=['c'])
+                ),
+                device=cpu,
+                in_keys=['a'],
+                out_keys=['b', 'c'])
+            >>> # select all modules that affect the value of "e"
+            >>> module.select_subsequence(out_keys=["e"])
+            TensorDictSequential(
+                module=ModuleList(
+                  (0): TensorDictModule(
+                      module=<function <lambda> at 0x126ed1ca0>,
+                      device=cpu,
+                      in_keys=['a'],
+                      out_keys=['e'])
+                ),
+                device=cpu,
+                in_keys=['a'],
+                out_keys=['e'])
+
+        This method propagates to nested sequential:
+
+            >>> module = Seq(
+            ...     Seq(
+            ...         Mod(idn, in_keys=["a"], out_keys=["b"]),
+            ...         Mod(idn, in_keys=["b"], out_keys=["c"]),
+            ...     ),
+            ...     Seq(
+            ...         Mod(idn, in_keys=["b"], out_keys=["d"]),
+            ...         Mod(idn, in_keys=["d"], out_keys=["e"]),
+            ...     ),
+            ... )
+            >>> # select submodules whose output will be affected by a change in "b" or "d" AND which output is "e"
+            >>> module.select_subsequence(in_keys=["b", "d"], out_keys=["e"])
+            TensorDictSequential(
+                module=ModuleList(
+                  (0): TensorDictSequential(
+                      module=ModuleList(
+                        (0): TensorDictModule(
+                            module=<function <lambda> at 0x129efae50>,
+                            device=cpu,
+                            in_keys=['b'],
+                            out_keys=['d'])
+                        (1): TensorDictModule(
+                            module=<function <lambda> at 0x129efae50>,
+                            device=cpu,
+                            in_keys=['d'],
+                            out_keys=['e'])
+                      ),
+                      device=cpu,
+                      in_keys=['b'],
+                      out_keys=['d', 'e'])
+                ),
+                device=cpu,
+                in_keys=['b'],
+                out_keys=['d', 'e'])
+
         """
         if in_keys is None:
             in_keys = deepcopy(self.in_keys)
         else:
             in_keys = [_normalize_key(key) for key in in_keys]
         if out_keys is None:
             out_keys = deepcopy(self.out_keys)
         else:
             out_keys = [_normalize_key(key) for key in out_keys]
-        id_to_keep = set(range(len(self.module)))
-        for i, module in enumerate(self.module):
+        module_list = list(self.module)
+        id_to_keep = set(range(len(module_list)))
+        for i, module in enumerate(module_list):
+            if (
+                type(module) is TensorDictSequential
+            ):  # no isinstance because we don't want to mess up subclasses
+                try:
+                    module = module_list[i] = module.select_subsequence(in_keys=in_keys)
+                except ValueError:
+                    # then the module can be removed
+                    id_to_keep.remove(i)
+                    continue
+
             if all(key in in_keys for key in module.in_keys):
                 in_keys.extend(module.out_keys)
             else:
                 id_to_keep.remove(i)
-        for i, module in reversed(list(enumerate(self.module))):
+        for i, module in reversed(list(enumerate(module_list))):
             if i in id_to_keep:
                 if any(key in out_keys for key in module.out_keys):
+                    if (
+                        type(module) is TensorDictSequential
+                    ):  # no isinstance because we don't want to mess up subclasses
+                        module = module_list[i] = module.select_subsequence(
+                            out_keys=out_keys
+                        )
                     out_keys.extend(module.in_keys)
                 else:
                     id_to_keep.remove(i)
         id_to_keep = sorted(id_to_keep)
 
-        modules = [self.module[i] for i in id_to_keep]
+        modules = [module_list[i] for i in id_to_keep]
 
         if modules == []:
             raise ValueError(
                 "No modules left after selection. Make sure that in_keys and out_keys are coherent."
             )
 
         return self.__class__(*modules)
 
     def _run_module(
         self,
         module: TensorDictModule,
         tensordict: TensorDictBase,
         **kwargs: Any,
     ) -> Any:
-        tensordict_keys = set(tensordict.keys(include_nested=True))
         if not self.partial_tolerant or all(
-            key in tensordict_keys for key in module.in_keys
+            key in tensordict.keys(include_nested=True) for key in module.in_keys
         ):
             tensordict = module(tensordict, **kwargs)
         elif self.partial_tolerant and isinstance(tensordict, LazyStackedTensorDict):
             for sub_td in tensordict.tensordicts:
-                tensordict_keys = set(sub_td.keys(include_nested=True))
-                if all(key in tensordict_keys for key in module.in_keys):
+                if all(
+                    key in sub_td.keys(include_nested=True) for key in module.in_keys
+                ):
                     module(sub_td, **kwargs)
             tensordict._update_valid_keys()
         return tensordict
 
-    @dispatch
+    @dispatch(auto_batch_size=False)
+    @set_skip_existing(None)
     def forward(
         self,
         tensordict: TensorDictBase,
         tensordict_out: TensorDictBase | None = None,
         **kwargs: Any,
     ) -> TensorDictBase:
         if not len(kwargs):
             for module in self.module:
                 tensordict = self._run_module(module, tensordict, **kwargs)
         else:
             raise RuntimeError(
-                "TensorDictSequential does not support keyword arguments other than 'tensordict_out', 'in_keys' and 'out_keys'"
+                f"TensorDictSequential does not support keyword arguments other than 'tensordict_out' or in_keys: {self.in_keys}. Got {kwargs.keys()} instead."
             )
         if tensordict_out is not None:
             tensordict_out.update(tensordict, inplace=True)
             return tensordict_out
         return tensordict
 
     def __len__(self) -> int:
```

## tensordict/nn/utils.py

```diff
@@ -1,20 +1,25 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
 from __future__ import annotations
 
-from typing import Callable
+import functools
+import inspect
+from typing import Any, Callable
 
 import torch
 from torch import nn
 
 __all__ = ["mappings", "inv_softplus", "biased_softplus"]
+_SKIP_EXISTING = False
+
+from tensordict._contextlib import _DecoratorContextManager
 
 
 def inv_softplus(bias: float | torch.Tensor) -> float | torch.Tensor:
     """Inverse softplus function.
 
     Args:
         bias (float or tensor): the value to be softplus-inverted.
@@ -84,7 +89,187 @@
                 float(stripped_key[-2]), min_val=float(stripped_key[-1])
             )
         else:
             raise ValueError(f"Invalid number of args in  {key}")
 
     else:
         raise NotImplementedError(f"Unknown mapping {key}")
+
+
+class set_skip_existing(_DecoratorContextManager):
+    """A context manager for skipping existing nodes in a TensorDict graph.
+
+    When used as a context manager, it will set the `skip_existing()` value
+    to the ``mode`` indicated, leaving the user able to code up methods that
+    will check the global value and execute the code accordingly.
+
+    When used as a method decorator, it will check the tensordict input keys
+    and if the ``skip_existing()`` call returns ``True``, it will skip the method
+    if all the output keys are already present.
+    This not not expected to be used as a decorator for methods that do not
+    respect the following signature: ``def fun(self, tensordict, *args, **kwargs)``.
+
+    Args:
+        mode (bool, optional):
+            If ``True``, it indicates that existing entries in the graph
+            won't be overwritten, unless they are only partially present. :func:`~.skip_existing`
+            will return ``True``.
+            If ``False``, no check will be performed.
+            If ``None``, the value of :func:`~.skip_existing` will not be
+            changed. This is intended to be used exclusively for decorating
+            methods and allow their behaviour to depend on the same class
+            when used as a context manager (see example below).
+            Defaults to ``True``.
+        in_key_attr (str, optional): the name of the input key list attribute
+            in the module's method being decorated. Defaults to ``in_keys``.
+        out_key_attr (str, optional): the name of the output key list attribute
+            in the module's method being decorated. Defaults to ``out_keys``.
+
+    Examples:
+        >>> with set_skip_existing():
+        ...     if skip_existing():
+        ...         print("True")
+        ...     else:
+        ...         print("False")
+        ...
+        True
+        >>> print("calling from outside:", skip_existing())
+        calling from outside: False
+
+    This class can also be used as a decorator:
+    Examples:
+        >>> from tensordict import TensorDict
+        >>> from tensordict.nn import set_skip_existing, skip_existing, TensorDictModuleBase
+        >>> class MyModule(TensorDictModuleBase):
+        ...     in_keys = []
+        ...     out_keys = ["out"]
+        ...     @set_skip_existing()
+        ...     def forward(self, tensordict):
+        ...         print("hello")
+        ...         tensordict.set("out", torch.zeros(()))
+        ...         return tensordict
+        >>> module = MyModule()
+        >>> module(TensorDict({"out": torch.zeros(())}, []))  # does not print anything
+        TensorDict(
+            fields={
+                out: Tensor(shape=torch.Size([]), device=cpu, dtype=torch.float32, is_shared=False)},
+            batch_size=torch.Size([]),
+            device=None,
+            is_shared=False)
+        >>> module(TensorDict({}, []))  # prints hello
+        hello
+        TensorDict(
+            fields={
+                out: Tensor(shape=torch.Size([]), device=cpu, dtype=torch.float32, is_shared=False)},
+            batch_size=torch.Size([]),
+            device=None,
+            is_shared=False)
+
+    Decorating a method with the mode set to ``None`` is useful whenever one
+    wants ot let the context manager take care of skipping things from the outside:
+        >>> from tensordict import TensorDict
+        >>> from tensordict.nn import set_skip_existing, skip_existing, TensorDictModuleBase
+        >>> class MyModule(TensorDictModuleBase):
+        ...     in_keys = []
+        ...     out_keys = ["out"]
+        ...     @set_skip_existing(None)
+        ...     def forward(self, tensordict):
+        ...         print("hello")
+        ...         tensordict.set("out", torch.zeros(()))
+        ...         return tensordict
+        >>> module = MyModule()
+        >>> _ = module(TensorDict({"out": torch.zeros(())}, []))  # prints "hello"
+        hello
+        >>> with set_skip_existing(True):
+        ...     _ = module(TensorDict({"out": torch.zeros(())}, []))  # no print
+
+
+    .. note::
+        To allow for modules to have the same input and output keys and not
+        mistakenly ignoring subgraphs, ``@set_skip_existing(True)`` will be
+        deactivated whenever the output keys are also the input keys:
+
+            >>> class MyModule(TensorDictModuleBase):
+            ...     in_keys = ["out"]
+            ...     out_keys = ["out"]
+            ...     @set_skip_existing()
+            ...     def forward(self, tensordict):
+            ...         print("calling the method!")
+            ...         return tensordict
+            ...
+            >>> module = MyModule()
+            >>> module(TensorDict({"out": torch.zeros(())}, []))  # does not print anything
+            calling the method!
+            TensorDict(
+                fields={
+                    out: Tensor(shape=torch.Size([]), device=cpu, dtype=torch.float32, is_shared=False)},
+                batch_size=torch.Size([]),
+                device=None,
+                is_shared=False)
+
+
+    """
+
+    def __init__(
+        self, mode: bool | None = True, in_key_attr="in_keys", out_key_attr="out_keys"
+    ):
+        self.mode = mode
+        self.in_key_attr = in_key_attr
+        self.out_key_attr = out_key_attr
+        self._called = False
+
+    def clone(self) -> set_skip_existing:
+        # override this method if your children class takes __init__ parameters
+        out = self.__class__(self.mode)
+        out._called = self._called
+        return out
+
+    def __call__(self, func: Callable):
+
+        self._called = True
+
+        # sanity check
+        for i, key in enumerate(inspect.signature(func).parameters):
+            if i == 0:
+                # skip self
+                continue
+            if key != "tensordict":
+                raise RuntimeError(
+                    "the first argument of the wrapped function must be "
+                    "named 'tensordict'."
+                )
+            break
+
+        @functools.wraps(func)
+        def wrapper(_self, tensordict, *args: Any, **kwargs: Any) -> Any:
+            in_keys = getattr(_self, self.in_key_attr)
+            out_keys = getattr(_self, self.out_key_attr)
+            # we use skip_existing to allow users to override the mode internally
+            if (
+                skip_existing()
+                and all(key in tensordict.keys(True) for key in out_keys)
+                and not any(key in out_keys for key in in_keys)
+            ):
+                return tensordict
+            return func(_self, tensordict, *args, **kwargs)
+
+        return super().__call__(wrapper)
+
+    def __enter__(self) -> None:
+        global _SKIP_EXISTING
+        self.prev = _SKIP_EXISTING
+        if self.mode is not None:
+            _SKIP_EXISTING = self.mode
+        elif not self._called:
+            raise RuntimeError(
+                f"It seems you are using {self.__class__.__name__} as a decorator with ``None`` input. "
+                f"This behaviour is not allowed."
+            )
+
+    def __exit__(self, exc_type: Any, exc_value: Any, traceback: Any) -> None:
+        global _SKIP_EXISTING
+        _SKIP_EXISTING = self.prev
+
+
+def skip_existing():
+    """Returns whether or not existing entries in a tensordict should be re-computed by a module."""
+    return _SKIP_EXISTING
```

## tensordict/prototype/__init__.py

```diff
@@ -1,12 +1,11 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
-
 from tensordict.prototype.fx import symbolic_trace
 from tensordict.prototype.tensorclass import is_tensorclass, tensorclass
 
 __all__ = [
     "is_tensorclass",
     "symbolic_trace",
     "tensorclass",
```

## tensordict/prototype/tensorclass.py

```diff
@@ -1,921 +1,25 @@
-# Copyright (c) Meta Platforms, Inc. and affiliates.
-#
-# This source code is licensed under the MIT license found in the
-# LICENSE file in the root directory of this source tree.
-
-from __future__ import annotations
-
-import dataclasses
-import functools
-import inspect
-import numbers
-import re
-import sys
-import typing
 import warnings
-from copy import copy
-from dataclasses import dataclass
-from textwrap import indent
-from typing import Any, Callable, Sequence, TypeVar, Union
-
-import tensordict as tensordict_lib
+from functools import wraps
 
-import torch
-
-from tensordict.memmap import MemmapTensor
-from tensordict.tensordict import (
-    _get_repr,
-    is_tensor_collection,
-    TD_HANDLED_FUNCTIONS,
-    TensorDict,
-    TensorDictBase,
+from tensordict import (  # no_qa
+    is_tensorclass as is_tensorclass_true,
+    tensorclass as tensorclass_true,
 )
-from tensordict.utils import DeviceType, NestedKey
-from torch import Tensor
-
-T = TypeVar("T", bound=TensorDictBase)
-PY37 = sys.version_info < (3, 8)
-
-# We keep a dict of str -> class to call the class based on the string
-CLASSES_DICT: dict[str, type] = {}
-
-# Regex precompiled patterns
-OPTIONAL_PATTERN = re.compile(r"Optional\[(.*?)\]")
-UNION_PATTERN = re.compile(r"Union\[(.*?)\]")
-
-# methods where non_tensordict data should be cleared in the return value
-_CLEAR_METADATA = {"all", "any"}
-# torch functions where we can wrap the corresponding TensorDict version
-_TD_PASS_THROUGH = {
-    torch.unbind,
-    torch.full_like,
-    torch.zeros_like,
-    torch.ones_like,
-    torch.clone,
-    torch.squeeze,
-    torch.unsqueeze,
-    torch.split,
-    torch.permute,
-    torch.split,
-    torch.stack,
-    torch.cat,
-    torch.gather,
-}
-
-
-def is_tensorclass(obj: type | Any) -> bool:
-    """Returns True if obj is either a tensorclass or an instance of a tensorclass."""
-    cls = obj if isinstance(obj, type) else type(obj)
-    return dataclasses.is_dataclass(cls) and cls.__name__ in CLASSES_DICT
-
-
-def tensorclass(cls: T) -> T:
-    """A decorator to create :obj:`tensorclass` classes.
-
-    :obj:`tensorclass` classes are specialized :obj:`dataclass` instances that
-    can execute some pre-defined tensor operations out of the box, such as
-    indexing, item assignment, reshaping, casting to device or storage and many
-    others.
-
-    Examples:
-        >>> from tensordict.prototype import tensorclass
-        >>> import torch
-        >>> from typing import Optional
-        >>>
-        >>> @tensorclass
-        ... class MyData:
-        ...     X: torch.Tensor
-        ...     y: torch.Tensor
-        ...     z: str
-        ...     def expand_and_mask(self):
-        ...         X = self.X.unsqueeze(-1).expand_as(self.y)
-        ...         X = X[self.y]
-        ...         return X
-        ...
-        >>> data = MyData(
-        ...     X=torch.ones(3, 4, 1),
-        ...     y=torch.zeros(3, 4, 2, 2, dtype=torch.bool),
-        ...     z="test"
-        ...     batch_size=[3, 4])
-        >>> print(data)
-        MyData(
-            X=Tensor(torch.Size([3, 4, 1]), dtype=torch.float32),
-            y=Tensor(torch.Size([3, 4, 2, 2]), dtype=torch.bool),
-            z="test"
-            batch_size=[3, 4],
-            device=None,
-            is_shared=False)
-        >>> print(data.expand_and_mask())
-        tensor([])
-
-    It is also possible to nest tensorclasses instances within each other:
-        Examples:
-        >>> from tensordict.prototype import tensorclass
-        >>> import torch
-        >>> from typing import Optional
-        >>>
-        >>> @tensorclass
-        ... class NestingMyData:
-        ...     nested: MyData
-        ...
-        >>> nesting_data = NestingMyData(nested=data, batch_size=[3, 4])
-        >>> # although the data is stored as a TensorDict, the type hint helps us
-        >>> # to appropriately cast the data to the right type
-        >>> assert isinstance(nesting_data.nested, type(data))
-
-
-    """
-
-    def __torch_function__(
-        cls,
-        func: Callable,
-        types: tuple[type, ...],
-        args: tuple[Any, ...] = (),
-        kwargs: dict[str, Any] | None = None,
-    ) -> Callable:
-        if func not in _TD_PASS_THROUGH or not all(
-            issubclass(t, (Tensor, cls)) for t in types
-        ):
-            return NotImplemented
-
-        if kwargs is None:
-            kwargs = {}
 
-        # get the output type from the arguments / keyword arguments
-        if len(args) > 0:
-            tc = args[0]
-        else:
-            tc = kwargs.get("input", kwargs["tensors"])
-        if isinstance(tc, (tuple, list)):
-            tc = tc[0]
 
-        args = tuple(_arg_to_tensordict(arg) for arg in args)
-        kwargs = {key: _arg_to_tensordict(value) for key, value in kwargs.items()}
-
-        res = TD_HANDLED_FUNCTIONS[func](*args, **kwargs)
-        if isinstance(res, (list, tuple)):
-            return res.__class__(_from_tensordict_with_copy(tc, td) for td in res)
-        return _from_tensordict_with_copy(tc, res)
-
-    cls = dataclass(cls)
-    expected_keys = set(cls.__dataclass_fields__)
-
-    for attr in cls.__dataclass_fields__:
-        if attr in dir(TensorDict):
-            raise AttributeError(
-                f"Attribute name {attr} can't be used with @tensorclass"
-            )
-
-    cls.__init__ = _init_wrapper(cls.__init__)
-    cls._from_tensordict = classmethod(_from_tensordict_wrapper(expected_keys))
-    cls.__torch_function__ = classmethod(__torch_function__)
-    cls.__getstate__ = _getstate
-    cls.__setstate__ = _setstate
-    cls.__getattribute__ = _getattribute_wrapper(cls.__getattribute__)
-    cls.__setattr__ = _setattr_wrapper(cls.__setattr__, expected_keys)
-    cls.__getattr__ = _getattr
-    cls.__getitem__ = _getitem
-    cls.__getitems__ = _getitem
-    cls.__setitem__ = _setitem
-    cls.__repr__ = _repr
-    cls.__len__ = _len
-    cls.__eq__ = __eq__
-    cls.__ne__ = __ne__
-    cls.state_dict = _state_dict
-    cls.load_state_dict = _load_state_dict
-
-    cls.to_tensordict = _to_tensordict
-    cls.device = property(_device, _device_setter)
-    cls.batch_size = property(_batch_size, _batch_size_setter)
-
-    cls.__doc__ = f"{cls.__name__}{inspect.signature(cls)}"
-
-    CLASSES_DICT[cls.__name__] = cls
-    tensordict_lib.tensordict._ACCEPTED_CLASSES += [cls]
-    return cls
-
-
-def _arg_to_tensordict(arg):
-    # if arg is a tensorclass or sequence of tensorclasses, extract the underlying
-    # tensordicts and return those instead
-    if is_tensorclass(arg):
-        return arg._tensordict
-    elif isinstance(arg, (tuple, list)) and all(is_tensorclass(item) for item in arg):
-        return arg.__class__(item._tensordict for item in arg)
-    return arg
-
-
-def _from_tensordict_with_copy(tc, tensordict):
-    # creates a new tensorclass with the same type as tc, and a copy of the
-    # non_tensordict data
-    return tc._from_tensordict(
-        tensordict=tensordict, non_tensordict=copy(tc._non_tensordict)
+@wraps(tensorclass_true)
+def tensorclass(*args, **kwargs):  # noqa: D103
+    warnings.warn(
+        "tensorclass is not a prototype anymore and can be imported directly from tensordict root.",
+        category=DeprecationWarning,
     )
+    return tensorclass_true(*args, **kwargs)
 
 
-def _from_tensordict_with_none(tc, tensordict):
-    # creates a new tensorclass with the same type as tc, and all non_tensordict entries
-    # set to None
-    return tc._from_tensordict(
-        tensordict=tensordict,
-        non_tensordict={key: None for key in tc._non_tensordict},
+@wraps(is_tensorclass_true)
+def is_tensorclass(*args, **kwargs):  # noqa: D103
+    warnings.warn(
+        "is_tensorclass is not a prototype anymore and can be imported directly from tensordict root.",
+        category=DeprecationWarning,
     )
-
-
-def _init_wrapper(init: Callable) -> Callable:
-    init_sig = inspect.signature(init)
-    params = list(init_sig.parameters.values())
-    # drop first entry of params which corresponds to self and isn't passed by the user
-    required_params = [p.name for p in params[1:] if p.default is inspect._empty]
-
-    @functools.wraps(init)
-    def wrapper(
-        self,
-        *args: Any,
-        batch_size: Sequence[int] | torch.Size | int,
-        device: DeviceType | None = None,
-        **kwargs,
-    ):
-        for value, key in zip(args, self.__dataclass_fields__):
-            if key in kwargs:
-                raise ValueError(f"The key {key} is already set in kwargs")
-            kwargs[key] = value
-
-        for key, field in self.__dataclass_fields__.items():
-            if field.default_factory is not dataclasses.MISSING:
-                default = field.default_factory()
-            else:
-                default = field.default
-            if default not in (None, dataclasses.MISSING):
-                kwargs.setdefault(key, default)
-
-        missing_params = [p for p in required_params if p not in kwargs]
-        if missing_params:
-            n_missing = len(missing_params)
-            raise TypeError(
-                f"{self.__class__.__name__}.__init__() missing {n_missing} "
-                f"required positional argument{'' if n_missing == 1 else 's'}: "
-                f"""{", ".join(f"'{name}'" for name in missing_params)}"""
-            )
-
-        self._tensordict = TensorDict(
-            {}, batch_size=batch_size, device=device, _run_checks=False
-        )
-        # To save non tensor data (Nested tensor classes also go here)
-        self._non_tensordict = {}
-        init(self, **{key: value for key, value in kwargs.items()})
-
-    new_params = [
-        inspect.Parameter("batch_size", inspect.Parameter.KEYWORD_ONLY),
-        inspect.Parameter("device", inspect.Parameter.KEYWORD_ONLY, default=None),
-    ]
-    wrapper.__signature__ = init_sig.replace(parameters=params + new_params)
-
-    return wrapper
-
-
-def _from_tensordict_wrapper(expected_keys):
-    def wrapper(cls, tensordict, non_tensordict=None):  # noqa: D417
-        """Tensor class wrapper to instantiate a new tensor class object.
-
-        Args:
-            tensordict (TensorDict): Dictionary of tensor types
-            non_tensordict (dict): Dictionary with non-tensor and nested tensor class objects
-
-        """
-        if not isinstance(tensordict, TensorDictBase):
-            raise RuntimeError(
-                f"Expected a TensorDictBase instance but got {type(tensordict)}"
-            )
-        # Validating keys of tensordict
-        for key in tensordict.keys():
-            if key not in expected_keys:
-                raise ValueError(
-                    f"Keys from the tensordict ({set(tensordict.keys())}) must "
-                    f"correspond to the class attributes ({expected_keys})."
-                )
-
-        # Validating non-tensor keys and for key clash
-        tensor_keys = set(tensordict.keys())
-        if non_tensordict is not None:
-            for key in non_tensordict.keys():
-                if key not in expected_keys:
-                    raise ValueError(
-                        f"Keys from the non-tensor data ({set(non_tensordict.keys())}) must "
-                        f"correspond to the class attributes ({expected_keys})."
-                    )
-                if key in tensor_keys:
-                    raise KeyError(
-                        f"{key} is present in both tensor and non-tensor dicts"
-                    )
-        # bypass initialisation. this means we don't incur any overhead creating an
-        # empty tensordict and writing values to it. we can skip this because we already
-        # have a tensordict to use as the underlying tensordict
-        tc = cls.__new__(cls)
-        tc.__dict__["_tensordict"] = tensordict
-
-        tc.__dict__["_non_tensordict"] = (
-            non_tensordict if non_tensordict is not None else {}
-        )
-        # since we aren't calling the dataclass init method, we need to manually check
-        # whether a __post_init__ method has been defined and invoke it if so
-        if hasattr(tc, "__post_init__"):
-            tc.__post_init__()
-        return tc
-
-    return wrapper
-
-
-def _getstate(self) -> dict[str, Any]:
-    """Returns a state dict which consists of tensor and non_tensor dicts for serialization.
-
-    Returns:
-        dictionary of state of tensor class
-
-    """
-    return {"tensordict": self._tensordict, "non_tensordict": self._non_tensordict}
-
-
-def _setstate(self, state: dict[str, Any]) -> None:  # noqa: D417
-    """Used to set the state of an object using state parameter.
-
-    Args:
-        state (dict): State parameter to set the object
-    """
-    self._tensordict = state.get("tensordict", None)
-    self._non_tensordict = state.get("non_tensordict", None)
-
-
-def _getattribute_wrapper(getattribute: Callable) -> Callable:
-    """Retrieve the value of an object's attribute or raise AttributeError.
-
-    Args:
-        item (str) : name of the attribute to retrieve
-
-    Returns:
-        value of the attribute
-
-    """
-
-    @functools.wraps(getattribute)
-    def wrapper(self, item: str) -> Any:
-        if not item.startswith("__"):
-            if (
-                "_tensordict" in self.__dict__
-                and item in self.__dict__["_tensordict"].keys()
-            ):
-                out = self._tensordict[item]
-                expected_type = self.__dataclass_fields__[item].type
-                out = _get_typed_output(out, expected_type)
-                return out
-            elif (
-                "_non_tensordict" in self.__dict__
-                and item in self.__dict__["_non_tensordict"]
-            ):
-                out = self._non_tensordict[item]
-                return out
-        return getattribute(self, item)
-
-    return wrapper
-
-
-def _setattr_wrapper(setattr_: Callable, expected_keys: set[str]) -> Callable:
-    @functools.wraps(setattr_)
-    def wrapper(self, key: str, value: Any) -> None:  # noqa: D417
-        """Set the value of an attribute for the tensor class object.
-
-        Args:
-            key (str): the name of the attribute to set
-            value (any): the value to set for the attribute
-
-        """
-        if (
-            "_tensordict" not in self.__dict__
-            or "_non_tensordict" not in self.__dict__
-            or key in ("batch_size", "device")
-        ):
-            return setattr_(self, key, value)
-        if key not in expected_keys:
-            raise AttributeError(
-                f"Cannot set the attribute '{key}', expected attributes are {expected_keys}."
-            )
-
-        if isinstance(value, tuple(tensordict_lib.tensordict._ACCEPTED_CLASSES)):
-            # Avoiding key clash, honoring the user input to assign tensor type data to the key
-            if key in self._non_tensordict.keys():
-                del self._non_tensordict[key]
-            self._tensordict[key] = value
-        else:
-            # Avoiding key clash, honoring the user input to assign non-tensor data to the key
-            if key in self._tensordict.keys():
-                del self._tensordict[key]
-            # Saving all non-tensor attributes
-            self._non_tensordict[key] = value
-        return None
-
-    return wrapper
-
-
-def _getattr(self, attr: str) -> Any:
-    """Retrieve the value of an object's attribute, or a method output if attr is callable.
-
-    Args:
-        attr: name of the attribute to retrieve or function to compute
-
-    Returns:
-        value of the attribute, or a method output applied on the instance
-
-    """
-    res = getattr(self._tensordict, attr)
-    if not callable(res):
-        return res
-    func = res
-
-    @functools.wraps(func)
-    def wrapped_func(*args, **kwargs):
-        args = tuple(_arg_to_tensordict(arg) for arg in args)
-        kwargs = {key: _arg_to_tensordict(value) for key, value in kwargs.items()}
-        res = func(*args, **kwargs)
-        if isinstance(res, TensorDictBase):
-            if attr.endswith("_"):
-                # in-place operation, return the current object
-                return self
-            elif attr in _CLEAR_METADATA:
-                # this is an attribute where copying the metadata makes no sense, e.g.
-                # .all or .any, so we replace all values with None
-                return self._from_tensordict(
-                    res, {k: None for k in self._non_tensordict}
-                )
-            # create a new tensorclass from res and copy the metadata from self
-            return self._from_tensordict(res, copy(self._non_tensordict))
-        return res
-
-    return wrapped_func
-
-
-def _getitem(self, item: NestedKey) -> Any:
-    """Retrieve the class object at the given index. Indexing will happen for nested tensors as well.
-
-    Args:
-       item (int or any other valid index type): index of the object to retrieve
-
-    Returns:
-        Tensor class object at the given index
-
-    """
-    if isinstance(item, str) or (
-        isinstance(item, tuple) and all(isinstance(_item, str) for _item in item)
-    ):
-        raise ValueError(f"Invalid indexing arguments: {item}.")
-    tensor_res = self._tensordict[item]
-    return _from_tensordict_with_copy(self, tensor_res)  # device=res.device)
-
-
-def _setitem(self, item: NestedKey, value: Any) -> None:  # noqa: D417
-    """Set the value of the Tensor class object at the given index. Note that there is no strict validation on non-tensor values.
-
-    Args:
-        item (int or any other valid index type): index of the object to set
-        value (any): value to set for the item
-
-    """
-    if isinstance(item, str) or (
-        isinstance(item, tuple) and all(isinstance(_item, str) for _item in item)
-    ):
-        raise ValueError("Invalid indexing arguments.")
-
-    if not is_tensorclass(value) and not isinstance(
-        value, (TensorDictBase, numbers.Number, Tensor, MemmapTensor)
-    ):
-        raise ValueError(
-            f"__setitem__ only supports tensorclasses, tensordicts,"
-            f" numeric scalars and tensors. Got {type(value)}"
-        )
-
-    if is_tensorclass(value):
-        if not isinstance(value, self.__class__):
-            self_keys = set().union(self._non_tensordict, self._tensordict.keys())
-            value_keys = set().union(value._non_tensordict, value._tensordict.keys())
-            if self_keys != value_keys:
-                # if tensorclass but different class ensure that all keys are equal
-                raise ValueError(
-                    "__setitem__ is only allowed for same-class or "
-                    "compatible class (i.e. same members) assignment"
-                )
-
-        # Validating the non-tensor data before setting the item
-        for key, val in value._non_tensordict.items():
-            # Raise a warning if non_tensor data doesn't match
-            if (
-                key in self._non_tensordict.keys()
-                and val is not self._non_tensordict[key]
-            ):
-                warnings.warn(
-                    f"Meta data at {repr(key)} may or may not be equal, "
-                    f"this may result in undefined behaviours",
-                    category=UserWarning,
-                    stacklevel=2,
-                )
-
-        for key in value._tensordict.keys():
-            # Making sure that the key-clashes won't happen, if the key is present
-            # in tensor data in value we will honor that and remove the key-value
-            # pair from non-tensor data
-            if key in self._non_tensordict.keys():
-                del self._non_tensordict[key]
-
-        self._tensordict[item] = value._tensordict
-    else:  # it is one of accepted "broadcast" types
-        # attempt broadcast on all tensordata and nested tensorclasses
-        self._tensordict[item] = value
-        for key, val in self._non_tensordict.items():
-            if is_tensorclass(val):
-                _setitem(self._non_tensordict[key], item, value)
-
-
-def _repr(self) -> str:
-    """Return a string representation of Tensor class object."""
-    fields = _all_td_fields_as_str(self._tensordict)
-    field_str = fields
-    non_tensor_fields = _all_non_td_fields_as_str(self._non_tensordict)
-    batch_size_str = indent(f"batch_size={self.batch_size}", 4 * " ")
-    device_str = indent(f"device={self.device}", 4 * " ")
-    is_shared_str = indent(f"is_shared={self.is_shared()}", 4 * " ")
-    if len(non_tensor_fields) > 0:
-        non_tensor_field_str = indent(
-            ",\n".join(non_tensor_fields),
-            4 * " ",
-        )
-        string = ",\n".join(
-            [field_str, non_tensor_field_str, batch_size_str, device_str, is_shared_str]
-        )
-    else:
-        string = ",\n".join([field_str, batch_size_str, device_str, is_shared_str])
-    return f"{self.__class__.__name__}(\n{string})"
-
-
-def _len(self) -> int:
-    """Returns the length of first dimension, if there is, otherwise 0."""
-    return len(self._tensordict)
-
-
-def _to_tensordict(self) -> TensorDict:
-    """Convert the tensorclass into a regular TensorDict.
-
-    Makes a copy of all entries. Memmap and shared memory tensors are converted to
-    regular tensors.
-
-    Returns:
-        A new TensorDict object containing the same values as the tensorclass.
-
-    """
-    td = self._tensordict.to_tensordict()
-    return td
-
-
-def _device(self) -> torch.device:
-    """Retrieves the device type of tensor class."""
-    return self._tensordict.device
-
-
-def _device_setter(self, value: DeviceType) -> None:
-    raise RuntimeError(
-        "device cannot be set using tensorclass.device = device, "
-        "because device cannot be updated in-place. To update device, use "
-        "tensorclass.to(new_device), which will return a new tensorclass "
-        "on the new device."
-    )
-
-
-def _batch_size(self) -> torch.Size:
-    """Retrieves the batch size for the tensor class.
-
-    Returns:
-        batch size (torch.Size)
-
-    """
-    return self._tensordict.batch_size
-
-
-def _batch_size_setter(self, new_size: torch.Size) -> None:  # noqa: D417
-    """Set the value of batch_size.
-
-    Args:
-        new_size (torch.Size): new_batch size to be set
-
-    """
-    self._tensordict._batch_size_setter(new_size)
-
-
-def _state_dict(self) -> dict[str, Any]:
-    """Returns a state_dict dictionary that can be used to save and load data from a tensorclass."""
-    state_dict = {"_tensordict": self._tensordict.state_dict()}
-    state_dict["_non_tensordict"] = copy(self._non_tensordict)
-    return state_dict
-
-
-def _load_state_dict(self, state_dict: dict[str, Any]):
-    """Loads a state_dict attemptedly in-place on the destination tensorclass."""
-    for key, item in state_dict.items():
-        # keys will never be nested which facilitates everything, but let's
-        # double check in case someone does something nasty
-        if not isinstance(key, str):
-            raise TypeError("Only str keys are allowed when calling load_state_dict.")
-        if key == "_non_tensordict":
-            for sub_key, sub_item in item.items():
-                # sub_item is the state dict of a tensorclass
-                if isinstance(sub_item, dict) and "_non_tensordict" in sub_item:
-                    raise RuntimeError(
-                        "Loading a saved tensorclass on a uninitialized tensorclass is not allowed"
-                    )
-                else:
-                    # check that sub_key is part of the tensorclass
-                    if sub_key not in self.__class__.__dataclass_fields__:
-                        raise KeyError(
-                            f"Key '{sub_key}' wasn't expected in the state-dict."
-                        )
-                    self._non_tensordict[sub_key] = sub_item
-        elif key == "_tensordict":
-            for sub_key in item.keys():
-                if (
-                    sub_key not in self.__class__.__dataclass_fields__
-                    and sub_key not in ("__batch_size", "__device")
-                ):
-                    raise KeyError(
-                        f"Key '{sub_key}' wasn't expected in the state-dict."
-                    )
-
-            self._tensordict.load_state_dict(item)
-        else:
-            raise KeyError(f"Key '{key}' wasn't expected in the state-dict.")
-
-    return self
-
-
-def __eq__(self, other: object) -> bool:
-    """Compares the Tensor class object to another object for equality. However, the equality check for non-tensor data is not performed.
-
-    Args:
-        other: object to compare to this object. Can be a tensorclass, a
-            tensordict or any compatible type (int, float or tensor), in
-            which case the equality check will be propagated to the leaves.
-
-    Returns:
-        False if the objects are of different class types, Tensorclass of boolean
-        values for tensor attributes and None for non-tensor attributes
-
-    Examples:
-        >>> @tensorclass
-        ... class MyClass:
-        ...     x: Tensor
-        ...     y: "MyClass"
-        ...     z: str
-        ...
-        >>> c1 = MyClass(
-        ...     x=torch.randn(3, 4),
-        ...     y=MyClass(
-        ...         x=torch.randn(3, 4, 1),
-        ...         y=None,
-        ...         z="bar",
-        ...         batch_size=[3, 4, 1],
-        ...     ),
-        ...     z="foo",
-        ...     batch_size=[3, 4],
-        ... )
-        >>> c2 = c1.clone()
-        >>> print(c1 == c2)
-        MyClass(
-            x=Tensor(shape=torch.Size([3, 4]), device=cpu, dtype=torch.bool, is_shared=False),
-            y=MyClass(
-                x=Tensor(shape=torch.Size([3, 4, 1]), device=cpu, dtype=torch.bool, is_shared=False),
-                y=None,
-                z=None,
-                batch_size=torch.Size([3, 4, 1]),
-                device=None,
-                is_shared=False),
-            z=None,
-            batch_size=torch.Size([3, 4]),
-            device=None,
-            is_shared=False)
-        >>> assert (c1 == c2).all()
-        >>> assert (c1[:2] == c2[:2]).all()
-        >>> assert not (c1 == c2.apply(lambda x: x+1)).all()
-
-    """
-    if not is_tensor_collection(other) and not isinstance(
-        other, (dict, numbers.Number, Tensor, MemmapTensor)
-    ):
-        return False
-    if is_tensorclass(other):
-        tensor = self._tensordict == other._tensordict
-    else:
-        tensor = self._tensordict == other
-    return _from_tensordict_with_none(self, tensor)
-
-
-def __ne__(self, other: object) -> bool:
-    """Compare the Tensor class object to another object for inequality. However, the equality check for non-tensor data is not performed.
-
-    Args:
-        other: object to compare to this object
-
-    Returns:
-        False if the objects are of different class types, Tensorclass of boolean values for tensor attributes and None for non-tensor attributes
-
-    Examples:
-        >>> @tensorclass
-        ... class MyClass:
-        ...     x: Tensor
-        ...     y: "MyClass"
-        ...     z: str
-        ...
-        >>> c1 = MyClass(
-        ...     x=torch.randn(3, 4),
-        ...     y=MyClass(
-        ...         x=torch.randn(3, 4, 1),
-        ...         y=None,
-        ...         z="bar",
-        ...         batch_size=[3, 4, 1],
-        ...     ),
-        ...     z="foo",
-        ...     batch_size=[3, 4],
-        ... )
-        >>> c2 = c1.clone()
-        >>> print(c1 != c2)
-        MyClass(
-            x=Tensor(shape=torch.Size([3, 4]), device=cpu, dtype=torch.bool, is_shared=False),
-            y=MyClass(
-                x=Tensor(shape=torch.Size([3, 4, 1]), device=cpu, dtype=torch.bool, is_shared=False),
-                y=None,
-                z=None,
-                batch_size=torch.Size([3, 4, 1]),
-                device=None,
-                is_shared=False),
-            z=None,
-            batch_size=torch.Size([3, 4]),
-            device=None,
-            is_shared=False)
-        >>> c2 = c2.apply(lambda x: x+1)
-        >>> assert (c1 != c2).all()
-
-    """
-    if not is_tensor_collection(other) and not isinstance(
-        other, (dict, numbers.Number, Tensor, MemmapTensor)
-    ):
-        return True
-    if is_tensorclass(other):
-        tensor = self._tensordict != other._tensordict
-    else:
-        tensor = self._tensordict != other
-    return _from_tensordict_with_none(self, tensor)
-
-
-def _get_typed_output(out, expected_type: str | type):
-    # from __future__ import annotations turns types in strings. For those we use CLASSES_DICT.
-    # Otherwise, if the output is some TensorDictBase subclass, we check the type and if it
-    # does not match, we map it. In all other cases, just return what has been gathered.
-    if isinstance(expected_type, str) and expected_type in CLASSES_DICT:
-        if isinstance(out, CLASSES_DICT[expected_type]):
-            return out
-        out = CLASSES_DICT[expected_type]._from_tensordict(out)
-    elif (
-        isinstance(expected_type, type)
-        and not isinstance(out, expected_type)
-        and isinstance(out, TensorDictBase)
-    ):
-        out = expected_type._from_tensordict(out)
-    elif isinstance(out, TensorDictBase):
-        dest_dtype = _check_td_out_type(expected_type)
-        if dest_dtype is not None:
-            out = dest_dtype._from_tensordict(out)
-
-    return out
-
-
-def _single_td_field_as_str(key, item, tensordict):
-    """Returns a string as a  key-value pair of tensordict.
-
-    Args:
-        key (str): key of tensor dict item
-        item (tensor type): value to be returned for key
-        tensordict (Tensordict): Tensordict object
-
-    Returns:
-        String representation of a key-value pair
-
-    """
-    if is_tensor_collection(type(item)):
-        return f"{key}={repr(tensordict[key])}"
-    return f"{key}={_get_repr(item)}"
-
-
-def _all_td_fields_as_str(td: TensorDictBase) -> str:
-    """Returns indented representation of tensor dict values as a key-value pairs.
-
-    Args:
-        td (TensorDict) : Tensordict object
-
-    Returns:
-        String representation of all tensor data
-
-    """
-    return indent(
-        ",\n".join(
-            sorted([_single_td_field_as_str(key, item, td) for key, item in td.items()])
-        ),
-        4 * " ",
-    )
-
-
-def _all_non_td_fields_as_str(src_dict) -> list:
-    """Returns a list of string representation of non-tensor key-value pairs.
-
-    Args:
-        src_dict (dict): non_tensor_dict
-
-    Returns:
-        result (list): list of strings with key-value representation
-
-    """
-    result = []
-    for key, val in src_dict.items():
-        if not is_tensor_collection(val):
-            result.append(f"{key}={repr(val)}")
-
-    return result
-
-
-def _check_td_out_type(field_def):
-    """This function determines the type of attributes in the tensorclass.
-
-    in order that results from calls to the underlying tensordict
-    can be cast to the expected type before being returned
-    """
-    if PY37:
-        field_def = str(field_def)
-    if isinstance(field_def, str):
-        optional_match = OPTIONAL_PATTERN.search(field_def)
-        union_match = UNION_PATTERN.search(field_def)
-        if optional_match is not None:
-            args = [optional_match.group(1)]
-        elif union_match is not None:
-            args = union_match.group(1).split(", ")
-        else:
-            args = None
-        if args:
-            args = [arg for arg in args if arg not in ("NoneType",)]
-        # skip all Any or TensorDict or Optional[TensorDict] or Union[TensorDict] or Optional[Any]
-        if (args is None and (field_def == "Any" or "TensorDict" in field_def)) or (
-            args and len(args) == 1 and args[0] == "Any"
-        ):
-            return None
-        if args and len(args) == 1 and "TensorDict" in args[0]:
-            return None
-        elif args:
-            # remove the NoneType from args
-            if len(args) == 1 and args[0] in CLASSES_DICT:
-                return CLASSES_DICT[args[0]]
-            if len(args) == 1 and ("TensorDict" in args[0] or args[0] == "Any"):
-                return None
-            else:
-                raise TypeError(
-                    f"{field_def} has args {args} which can't be deterministically cast."
-                )
-        elif args is None:
-            return None
-        else:
-            raise TypeError(
-                f"{field_def} has args {args} which can't be deterministically cast."
-            )
-    else:
-        if typing.get_origin(field_def) is Union:
-            args = typing.get_args(field_def)
-            # remove the NoneType from args
-            args = [arg for arg in args if arg not in (type(None),)]
-            if len(args) == 1 and (
-                typing.Any is not args[0]
-                and args[0] is not TensorDictBase
-                and TensorDictBase not in args[0].__bases__
-            ):
-                # If there is just one type in Union or Optional, we return that type
-                return args[0]
-            elif len(args) == 1 and (
-                typing.Any is args[0]
-                or args[0] is TensorDictBase
-                or TensorDictBase in args[0].__bases__
-            ):
-                # Any or any TensorDictBase subclass are always ok if alone
-                return None
-            else:
-                raise TypeError(
-                    f"{field_def} has args {args} which can't be deterministically cast."
-                )
-        elif (
-            field_def is typing.Any
-            or field_def is TensorDictBase
-            or TensorDictBase in field_def.__bases__
-        ):
-            # Any or any TensorDictBase subclass are alway ok if alone
-            return None
-        else:
-            raise TypeError(f"{field_def} can't be deterministically cast.")
+    return is_tensorclass_true(*args, **kwargs)
```

## Comparing `tensordict-0.1.0.dist-info/LICENSE` & `tensordict-0.1.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `tensordict-0.1.0.dist-info/METADATA` & `tensordict-0.1.1.dist-info/METADATA`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensordict
-Version: 0.1.0
+Version: 0.1.1
 Home-page: https://github.com/pytorch-labs/tensordict
 Author: tensordict contributors
 Author-email: vmoens@fb.com
 License: BSD
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -13,30 +13,50 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: torch
 Requires-Dist: numpy
 Requires-Dist: cloudpickle
 Provides-Extra: checkpointing
 Requires-Dist: torchsnapshot-nightly ; extra == 'checkpointing'
+Provides-Extra: h5
+Requires-Dist: h5py (>=3.8) ; extra == 'h5'
 Provides-Extra: tests
 Requires-Dist: pytest ; extra == 'tests'
 Requires-Dist: pyyaml ; extra == 'tests'
 Requires-Dist: pytest-instafail ; extra == 'tests'
 Requires-Dist: pytest-rerunfailures ; extra == 'tests'
+Requires-Dist: pytest-benchmark ; extra == 'tests'
 
+<!--- BADGES: START --->
+<!---
 [![Documentation](https://img.shields.io/badge/Documentation-blue.svg?style=flat)](https://pytorch-labs.github.io/tensordict/)
-[![Benchmarks](https://img.shields.io/badge/Benchmarks-blue.svg)](https://pytorch-labs.github.io/tensordict/dev/bench/)
+--->
+[![Docs - GitHub.io](https://img.shields.io/static/v1?logo=github&style=flat&color=pink&label=docs&message=tensordict)][#docs-package]
+[![Benchmarks](https://img.shields.io/badge/Benchmarks-blue.svg)][#docs-package-benchmark]
 [![Python version](https://img.shields.io/pypi/pyversions/tensordict.svg)](https://www.python.org/downloads/)
-[![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/pytorch-labs/tensordict/blob/main/LICENSE)
+[![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg)][#github-license]
 <a href="https://pypi.org/project/tensordict"><img src="https://img.shields.io/pypi/v/tensordict" alt="pypi version"></a>
 <a href="https://pypi.org/project/tensordict-nightly"><img src="https://img.shields.io/pypi/v/tensordict-nightly?label=nightly" alt="pypi nightly version"></a>
-[![Downloads](https://static.pepy.tech/personalized-badge/tensordict?period=total&units=international_system&left_color=blue&right_color=orange&left_text=Downloads)](https://pepy.tech/project/tensordict)
-[![Downloads](https://static.pepy.tech/personalized-badge/tensordict-nightly?period=total&units=international_system&left_color=blue&right_color=orange&left_text=Downloads%20(nightly))](https://pepy.tech/project/tensordict-nightly)
-[![codecov](https://codecov.io/gh/pytorch-labs/tensordict/branch/main/graph/badge.svg?token=9QTUG6NAGQ)](https://codecov.io/gh/pytorch-labs/tensordict)
-[![pytorch](https://circleci.com/gh/pytorch-labs/tensordict.svg?style=shield)](https://circleci.com/gh/pytorch-labs/tensordict)
+[![Downloads](https://static.pepy.tech/personalized-badge/tensordict?period=total&units=international_system&left_color=blue&right_color=orange&left_text=Downloads)][#pepy-package]
+[![Downloads](https://static.pepy.tech/personalized-badge/tensordict-nightly?period=total&units=international_system&left_color=blue&right_color=orange&left_text=Downloads%20(nightly))][#pepy-package-nightly]
+[![codecov](https://codecov.io/gh/pytorch-labs/tensordict/branch/main/graph/badge.svg?token=9QTUG6NAGQ)][#codecov-package]
+[![circleci](https://circleci.com/gh/pytorch-labs/tensordict.svg?style=shield)][#circleci-package]
+[![Conda - Platform](https://img.shields.io/conda/pn/conda-forge/tensordict?logo=anaconda&style=flat)][#conda-forge-package]
+[![Conda (channel only)](https://img.shields.io/conda/vn/conda-forge/tensordict?logo=anaconda&style=flat&color=orange)][#conda-forge-package]
+
+[#docs-package]: https://pytorch-labs.github.io/tensordict/
+[#docs-package-benchmark]: https://pytorch-labs.github.io/tensordict/dev/bench/
+[#github-license]: https://github.com/pytorch-labs/tensordict/blob/main/LICENSE
+[#pepy-package]: https://pepy.tech/project/tensordict
+[#pepy-package-nightly]: https://pepy.tech/project/tensordict-nightly
+[#codecov-package]: https://codecov.io/gh/pytorch-labs/tensordict
+[#circleci-package]: https://circleci.com/gh/pytorch-labs/tensordict
+[#conda-forge-package]: https://anaconda.org/conda-forge/tensordict
+
+<!--- BADGES: END --->
 
 # TensorDict
 
 [**Installation**](#installation) | [**General features**](#general) |
 [**Tensor-like features**](#tensor-like-features) |  [**Distributed capabilities**](#distributed-capabilities) |
 [**TensorDict for functional programming using FuncTorch**](#tensordict-for-functional-programming-using-functorch) |
 [**Lazy preallocation**](#lazy-preallocation) | [**Nesting TensorDicts**](#nesting-tensordicts) | [**TensorClass**](#tensorclass)
@@ -159,15 +179,15 @@
 We also provide an API to use TensorDict in conjunction with [FuncTorch](https://pytorch.org/functorch).
 For instance, TensorDict makes it easy to concatenate model weights to do model ensembling:
 ```python
 >>> from torch import nn
 >>> from tensordict import TensorDict
 >>> from tensordict.nn import make_functional
 >>> import torch
->>> from functorch import vmap
+>>> from torch import vmap
 >>> layer1 = nn.Linear(3, 4)
 >>> layer2 = nn.Linear(4, 4)
 >>> model = nn.Sequential(layer1, layer2)
 >>> # we represent the weights hierarchically
 >>> weights1 = TensorDict(layer1.state_dict(), []).unflatten_keys(".")
 >>> weights2 = TensorDict(layer2.state_dict(), []).unflatten_keys(".")
 >>> params = make_functional(model)
@@ -305,34 +325,48 @@
 arbitrary functions through the `apply` method (and many more).
 
 Tensorclasses support nesting and, in fact, all the TensorDict features.
 
 
 ## Installation
 
+**With Pip**:
+
 To install the latest stable version of tensordict, simply run
+
 ```bash
 pip install tensordict
 ```
+
 This will work with Python 3.7 and upward as well as PyTorch 1.12 and upward.
 
 To enjoy the latest features, one can use
+
 ```bash
 pip install tensordict-nightly
 ```
 
+**With Conda**:
+
+Install `tensordict` from `conda-forge` channel.
+
+```sh
+conda install -c conda-forge tensordict
+```
+
+
 ## Citation
 
 If you're using TensorDict, please refer to this BibTeX entry to cite this work:
 ```
 @software{TensorDict,
   author = {Moens, Vincent},
   title = {{TensorDict: your PyTorch universal data carrier}},
   url = {https://github.com/pytorch-labs/tensordict},
-  version = {0.1.0},
+  version = {0.1.1},
   year = {2023}
 }
 ```
 
 ## Disclaimer
 
 TensorDict is at the *beta*-stage, meaning that there may be bc-breaking changes introduced, but
```

### html2text {}

```diff
@@ -1,113 +1,124 @@
-Metadata-Version: 2.1 Name: tensordict Version: 0.1.0 Home-page: https://
+Metadata-Version: 2.1 Name: tensordict Version: 0.1.1 Home-page: https://
 github.com/pytorch-labs/tensordict Author: tensordict contributors Author-
 email: vmoens@fb.com License: BSD Classifier: Programming Language :: Python ::
 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Development Status :: 4 - Beta Description-Content-Type: text/
 markdown License-File: LICENSE Requires-Dist: torch Requires-Dist: numpy
 Requires-Dist: cloudpickle Provides-Extra: checkpointing Requires-Dist:
-torchsnapshot-nightly ; extra == 'checkpointing' Provides-Extra: tests
-Requires-Dist: pytest ; extra == 'tests' Requires-Dist: pyyaml ; extra ==
-'tests' Requires-Dist: pytest-instafail ; extra == 'tests' Requires-Dist:
-pytest-rerunfailures ; extra == 'tests' [![Documentation](https://
-img.shields.io/badge/Documentation-blue.svg?style=flat)](https://pytorch-
-labs.github.io/tensordict/) [![Benchmarks](https://img.shields.io/badge/
-Benchmarks-blue.svg)](https://pytorch-labs.github.io/tensordict/dev/bench/) [!
-[Python version](https://img.shields.io/pypi/pyversions/tensordict.svg)](https:
-//www.python.org/downloads/) [![GitHub license](https://img.shields.io/badge/
-license-MIT-blue.svg)](https://github.com/pytorch-labs/tensordict/blob/main/
-LICENSE) [pypi_version] [pypi_nightly_version] [![Downloads](https://
-static.pepy.tech/personalized-badge/
+torchsnapshot-nightly ; extra == 'checkpointing' Provides-Extra: h5 Requires-
+Dist: h5py (>=3.8) ; extra == 'h5' Provides-Extra: tests Requires-Dist: pytest
+; extra == 'tests' Requires-Dist: pyyaml ; extra == 'tests' Requires-Dist:
+pytest-instafail ; extra == 'tests' Requires-Dist: pytest-rerunfailures ; extra
+== 'tests' Requires-Dist: pytest-benchmark ; extra == 'tests'   [![Docs -
+GitHub.io](https://img.shields.io/static/
+v1?logo=github&style=flat&color=pink&label=docs&message=tensordict)][#docs-
+package] [![Benchmarks](https://img.shields.io/badge/Benchmarks-blue.svg)]
+[#docs-package-benchmark] [![Python version](https://img.shields.io/pypi/
+pyversions/tensordict.svg)](https://www.python.org/downloads/) [![GitHub
+license](https://img.shields.io/badge/license-MIT-blue.svg)][#github-license]
+[pypi_version] [pypi_nightly_version] [![Downloads](https://static.pepy.tech/
+personalized-badge/
 tensordict?period=total&units=international_system&left_color=blue&right_color=orange&left_text=Downloads)]
-(https://pepy.tech/project/tensordict) [![Downloads](https://static.pepy.tech/
-personalized-badge/tensordict-
+[#pepy-package] [![Downloads](https://static.pepy.tech/personalized-badge/
+tensordict-
 nightly?period=total&units=international_system&left_color=blue&right_color=orange&left_text=Downloads%20
-(nightly))](https://pepy.tech/project/tensordict-nightly) [![codecov](https://
-codecov.io/gh/pytorch-labs/tensordict/branch/main/graph/
-badge.svg?token=9QTUG6NAGQ)](https://codecov.io/gh/pytorch-labs/tensordict) [!
-[pytorch](https://circleci.com/gh/pytorch-labs/tensordict.svg?style=shield)]
-(https://circleci.com/gh/pytorch-labs/tensordict) # TensorDict
-[**Installation**](#installation) | [**General features**](#general) |
-[**Tensor-like features**](#tensor-like-features) | [**Distributed
-capabilities**](#distributed-capabilities) | [**TensorDict for functional
-programming using FuncTorch**](#tensordict-for-functional-programming-using-
-functorch) | [**Lazy preallocation**](#lazy-preallocation) | [**Nesting
-TensorDicts**](#nesting-tensordicts) | [**TensorClass**](#tensorclass)
-`TensorDict` is a dictionary-like class that inherits properties from tensors,
-such as indexing, shape operations, casting to device or point-to-point
-communication in distributed settings. The main purpose of TensorDict is to
-make code-bases more _readable_ and _modular_ by abstracting away tailored
-operations: ```python for i, tensordict in enumerate(dataset): # the model
-reads and writes tensordicts tensordict = model(tensordict) loss = loss_module
-(tensordict) loss.backward() optimizer.step() optimizer.zero_grad() ``` With
-this level of abstraction, one can recycle a training loop for highly
-heterogeneous task. Each individual step of the training loop (data collection
-and transform, model prediction, loss computation etc.) can be tailored to the
-use case at hand without impacting the others. For instance, the above example
-can be easily used across classification and segmentation tasks, among many
-others. ## Features ### General A tensordict is primarily defined by its
-`batch_size` (or `shape`) and its key-value pairs: ```python >>> from
-tensordict import TensorDict >>> import torch >>> tensordict = TensorDict({ ...
-"key 1": torch.ones(3, 4, 5), ... "key 2": torch.zeros(3, 4, 5,
-dtype=torch.bool), ... }, batch_size=[3, 4]) ``` The `batch_size` and the first
-dimensions of each of the tensors must be compliant. The tensors can be of any
-dtype and device. Optionally, one can restrict a tensordict to live on a
-dedicated device, which will send each tensor that is written there: ```python
->>> tensordict = TensorDict({ ... "key 1": torch.ones(3, 4, 5), ... "key 2":
-torch.zeros(3, 4, 5, dtype=torch.bool), ... }, batch_size=[3, 4], device="cuda:
-0") >>> tensordict["key 3"] = torch.randn(3, 4, device="cpu") >>> assert
-tensordict["key 3"].device is torch.device("cuda:0") ``` ### Tensor-like
-features TensorDict objects can be indexed exactly like tensors. The resulting
-of indexing a TensorDict is another TensorDict containing tensors indexed along
-the required dimension: ```python >>> tensordict = TensorDict({ ... "key 1":
-torch.ones(3, 4, 5), ... "key 2": torch.zeros(3, 4, 5, dtype=torch.bool), ...
-}, batch_size=[3, 4]) >>> sub_tensordict = tensordict[..., :2] >>> assert
-sub_tensordict.shape == torch.Size([3, 2]) >>> assert sub_tensordict["key
-1"].shape == torch.Size([3, 2, 5]) ``` Similarly, one can build tensordicts by
-stacking or concatenating single tensordicts: ```python >>> tensordicts =
-[TensorDict({ ... "key 1": torch.ones(3, 4, 5), ... "key 2": torch.zeros(3, 4,
-5, dtype=torch.bool), ... }, batch_size=[3, 4]) for _ in range(2)] >>>
-stack_tensordict = torch.stack(tensordicts, 1) >>> assert
-stack_tensordict.shape == torch.Size([3, 2, 4]) >>> assert stack_tensordict
-["key 1"].shape == torch.Size([3, 2, 4, 5]) >>> cat_tensordict = torch.cat
-(tensordicts, 0) >>> assert cat_tensordict.shape == torch.Size([6, 4]) >>>
-assert cat_tensordict["key 1"].shape == torch.Size([6, 4, 5]) ``` TensorDict
-instances can also be reshaped, viewed, squeezed and unsqueezed: ```python >>>
+(nightly))][#pepy-package-nightly] [![codecov](https://codecov.io/gh/pytorch-
+labs/tensordict/branch/main/graph/badge.svg?token=9QTUG6NAGQ)][#codecov-
+package] [![circleci](https://circleci.com/gh/pytorch-labs/
+tensordict.svg?style=shield)][#circleci-package] [![Conda - Platform](https://
+img.shields.io/conda/pn/conda-forge/tensordict?logo=anaconda&style=flat)]
+[#conda-forge-package] [![Conda (channel only)](https://img.shields.io/conda/
+vn/conda-forge/tensordict?logo=anaconda&style=flat&color=orange)][#conda-forge-
+package] [#docs-package]: https://pytorch-labs.github.io/tensordict/ [#docs-
+package-benchmark]: https://pytorch-labs.github.io/tensordict/dev/bench/
+[#github-license]: https://github.com/pytorch-labs/tensordict/blob/main/LICENSE
+[#pepy-package]: https://pepy.tech/project/tensordict [#pepy-package-nightly]:
+https://pepy.tech/project/tensordict-nightly [#codecov-package]: https://
+codecov.io/gh/pytorch-labs/tensordict [#circleci-package]: https://
+circleci.com/gh/pytorch-labs/tensordict [#conda-forge-package]: https://
+anaconda.org/conda-forge/tensordict  # TensorDict [**Installation**]
+(#installation) | [**General features**](#general) | [**Tensor-like features**]
+(#tensor-like-features) | [**Distributed capabilities**](#distributed-
+capabilities) | [**TensorDict for functional programming using FuncTorch**]
+(#tensordict-for-functional-programming-using-functorch) | [**Lazy
+preallocation**](#lazy-preallocation) | [**Nesting TensorDicts**](#nesting-
+tensordicts) | [**TensorClass**](#tensorclass) `TensorDict` is a dictionary-
+like class that inherits properties from tensors, such as indexing, shape
+operations, casting to device or point-to-point communication in distributed
+settings. The main purpose of TensorDict is to make code-bases more _readable_
+and _modular_ by abstracting away tailored operations: ```python for i,
+tensordict in enumerate(dataset): # the model reads and writes tensordicts
+tensordict = model(tensordict) loss = loss_module(tensordict) loss.backward()
+optimizer.step() optimizer.zero_grad() ``` With this level of abstraction, one
+can recycle a training loop for highly heterogeneous task. Each individual step
+of the training loop (data collection and transform, model prediction, loss
+computation etc.) can be tailored to the use case at hand without impacting the
+others. For instance, the above example can be easily used across
+classification and segmentation tasks, among many others. ## Features ###
+General A tensordict is primarily defined by its `batch_size` (or `shape`) and
+its key-value pairs: ```python >>> from tensordict import TensorDict >>> import
+torch >>> tensordict = TensorDict({ ... "key 1": torch.ones(3, 4, 5), ... "key
+2": torch.zeros(3, 4, 5, dtype=torch.bool), ... }, batch_size=[3, 4]) ``` The
+`batch_size` and the first dimensions of each of the tensors must be compliant.
+The tensors can be of any dtype and device. Optionally, one can restrict a
+tensordict to live on a dedicated device, which will send each tensor that is
+written there: ```python >>> tensordict = TensorDict({ ... "key 1": torch.ones
+(3, 4, 5), ... "key 2": torch.zeros(3, 4, 5, dtype=torch.bool), ... },
+batch_size=[3, 4], device="cuda:0") >>> tensordict["key 3"] = torch.randn(3, 4,
+device="cpu") >>> assert tensordict["key 3"].device is torch.device("cuda:0")
+``` ### Tensor-like features TensorDict objects can be indexed exactly like
+tensors. The resulting of indexing a TensorDict is another TensorDict
+containing tensors indexed along the required dimension: ```python >>>
 tensordict = TensorDict({ ... "key 1": torch.ones(3, 4, 5), ... "key 2":
-torch.zeros(3, 4, 5, dtype=torch.bool), ... }, batch_size=[3, 4]) >>> print
-(tensordict.view(-1)) torch.Size([12]) >>> print(tensordict.reshape(-1))
-torch.Size([12]) >>> print(tensordict.unsqueeze(-1)) torch.Size([3, 4, 1]) ```
-One can also send tensordict from device to device, place them in shared
-memory, clone them, update them in-place or not, split them, unbind them,
-expand them etc. If a functionality is missing, it is easy to call it using
-`apply()` or `apply_()`: ```python tensordict_uniform = tensordict.apply(lambda
-tensor: tensor.uniform_()) ``` ### Distributed capabilities Complex data
-structures can be cumbersome to synchronize in distributed settings.
-`tensordict` solves that problem with synchronous and asynchronous helper
-methods such as `recv`, `irecv`, `send` and `isend` that behave like their
-`torch.distributed` counterparts: ```python >>> # on all workers >>> data =
-TensorDict({"a": torch.zeros(()), ("b", "c"): torch.ones(())}, []) >>> # on
-worker 1 >>> data.isend(dst=0) >>> # on worker 0 >>> data.irecv(src=1) ``` When
-nodes share a common scratch space, the [`MemmapTensor` backend](https://
-pytorch-labs.github.io/tensordict/tutorials/tensordict_memory.html) can be used
-to seamlessly send, receive and read a huge amount of data. ### TensorDict for
-functional programming using FuncTorch We also provide an API to use TensorDict
-in conjunction with [FuncTorch](https://pytorch.org/functorch). For instance,
-TensorDict makes it easy to concatenate model weights to do model ensembling:
-```python >>> from torch import nn >>> from tensordict import TensorDict >>>
-from tensordict.nn import make_functional >>> import torch >>> from functorch
-import vmap >>> layer1 = nn.Linear(3, 4) >>> layer2 = nn.Linear(4, 4) >>> model
-= nn.Sequential(layer1, layer2) >>> # we represent the weights hierarchically
->>> weights1 = TensorDict(layer1.state_dict(), []).unflatten_keys(".") >>>
-weights2 = TensorDict(layer2.state_dict(), []).unflatten_keys(".") >>> params =
-make_functional(model) >>> assert (params == TensorDict({"0": weights1, "1":
-weights2}, [])).all() >>> # Let's use our functional module >>> x = torch.randn
-(10, 3) >>> out = model(x, params=params) # params is the last arg (or kwarg)
->>> # an ensemble of models: we stack params along the first dimension... >>>
+torch.zeros(3, 4, 5, dtype=torch.bool), ... }, batch_size=[3, 4]) >>>
+sub_tensordict = tensordict[..., :2] >>> assert sub_tensordict.shape ==
+torch.Size([3, 2]) >>> assert sub_tensordict["key 1"].shape == torch.Size([3,
+2, 5]) ``` Similarly, one can build tensordicts by stacking or concatenating
+single tensordicts: ```python >>> tensordicts = [TensorDict({ ... "key 1":
+torch.ones(3, 4, 5), ... "key 2": torch.zeros(3, 4, 5, dtype=torch.bool), ...
+}, batch_size=[3, 4]) for _ in range(2)] >>> stack_tensordict = torch.stack
+(tensordicts, 1) >>> assert stack_tensordict.shape == torch.Size([3, 2, 4]) >>>
+assert stack_tensordict["key 1"].shape == torch.Size([3, 2, 4, 5]) >>>
+cat_tensordict = torch.cat(tensordicts, 0) >>> assert cat_tensordict.shape ==
+torch.Size([6, 4]) >>> assert cat_tensordict["key 1"].shape == torch.Size([6,
+4, 5]) ``` TensorDict instances can also be reshaped, viewed, squeezed and
+unsqueezed: ```python >>> tensordict = TensorDict({ ... "key 1": torch.ones(3,
+4, 5), ... "key 2": torch.zeros(3, 4, 5, dtype=torch.bool), ... }, batch_size=
+[3, 4]) >>> print(tensordict.view(-1)) torch.Size([12]) >>> print
+(tensordict.reshape(-1)) torch.Size([12]) >>> print(tensordict.unsqueeze(-1))
+torch.Size([3, 4, 1]) ``` One can also send tensordict from device to device,
+place them in shared memory, clone them, update them in-place or not, split
+them, unbind them, expand them etc. If a functionality is missing, it is easy
+to call it using `apply()` or `apply_()`: ```python tensordict_uniform =
+tensordict.apply(lambda tensor: tensor.uniform_()) ``` ### Distributed
+capabilities Complex data structures can be cumbersome to synchronize in
+distributed settings. `tensordict` solves that problem with synchronous and
+asynchronous helper methods such as `recv`, `irecv`, `send` and `isend` that
+behave like their `torch.distributed` counterparts: ```python >>> # on all
+workers >>> data = TensorDict({"a": torch.zeros(()), ("b", "c"): torch.ones(
+())}, []) >>> # on worker 1 >>> data.isend(dst=0) >>> # on worker 0 >>>
+data.irecv(src=1) ``` When nodes share a common scratch space, the
+[`MemmapTensor` backend](https://pytorch-labs.github.io/tensordict/tutorials/
+tensordict_memory.html) can be used to seamlessly send, receive and read a huge
+amount of data. ### TensorDict for functional programming using FuncTorch We
+also provide an API to use TensorDict in conjunction with [FuncTorch](https://
+pytorch.org/functorch). For instance, TensorDict makes it easy to concatenate
+model weights to do model ensembling: ```python >>> from torch import nn >>>
+from tensordict import TensorDict >>> from tensordict.nn import make_functional
+>>> import torch >>> from torch import vmap >>> layer1 = nn.Linear(3, 4) >>>
+layer2 = nn.Linear(4, 4) >>> model = nn.Sequential(layer1, layer2) >>> # we
+represent the weights hierarchically >>> weights1 = TensorDict
+(layer1.state_dict(), []).unflatten_keys(".") >>> weights2 = TensorDict
+(layer2.state_dict(), []).unflatten_keys(".") >>> params = make_functional
+(model) >>> assert (params == TensorDict({"0": weights1, "1": weights2},
+[])).all() >>> # Let's use our functional module >>> x = torch.randn(10, 3) >>>
+out = model(x, params=params) # params is the last arg (or kwarg) >>> # an
+ensemble of models: we stack params along the first dimension... >>>
 params_stack = torch.stack([params, params], 0) >>> # ... and use it as an
 input we'd like to pass through the model >>> y = vmap(model, (None, 0))(x,
 params_stack) >>> print(y.shape) torch.Size([2, 10, 4]) ``` Moreover,
 tensordict modules are compatible with `torch.fx` and `torch.compile`, which
 means that you can get the best of both worlds: a codebase that is both
 readable and future-proof as well as efficient and portable! ### Lazy
 preallocation Pre-allocating tensors can be cumbersome and hard to scale if the
@@ -161,21 +172,22 @@
 dtype=torch.int64), mask=Tensor(torch.Size([10, 10, 1, 64, 64]),
 dtype=torch.bool), batch_size=torch.Size([10, 10]), device=None,
 is_shared=False) ``` As this example shows, one can write a specific data
 structures with dedicated methods while still enjoying the TensorDict artifacts
 such as shape operations (e.g. reshape or permutations), data manipulation
 (indexing, `cat` and `stack`) or calling arbitrary functions through the
 `apply` method (and many more). Tensorclasses support nesting and, in fact, all
-the TensorDict features. ## Installation To install the latest stable version
-of tensordict, simply run ```bash pip install tensordict ``` This will work
-with Python 3.7 and upward as well as PyTorch 1.12 and upward. To enjoy the
-latest features, one can use ```bash pip install tensordict-nightly ``` ##
-Citation If you're using TensorDict, please refer to this BibTeX entry to cite
-this work: ``` @software{TensorDict, author = {Moens, Vincent}, title = {
-{TensorDict: your PyTorch universal data carrier}}, url = {https://github.com/
-pytorch-labs/tensordict}, version = {0.1.0}, year = {2023} } ``` ## Disclaimer
-TensorDict is at the *beta*-stage, meaning that there may be bc-breaking
-changes introduced, but they should come with a warranty. Hopefully these
-should not happen too often, as the current roadmap mostly involves adding new
-features and building compatibility with the broader PyTorch ecosystem. ##
-License TensorDict is licensed under the MIT License. See [LICENSE](LICENSE)
-for details.
+the TensorDict features. ## Installation **With Pip**: To install the latest
+stable version of tensordict, simply run ```bash pip install tensordict ```
+This will work with Python 3.7 and upward as well as PyTorch 1.12 and upward.
+To enjoy the latest features, one can use ```bash pip install tensordict-
+nightly ``` **With Conda**: Install `tensordict` from `conda-forge` channel.
+```sh conda install -c conda-forge tensordict ``` ## Citation If you're using
+TensorDict, please refer to this BibTeX entry to cite this work: ``` @software
+{TensorDict, author = {Moens, Vincent}, title = {{TensorDict: your PyTorch
+universal data carrier}}, url = {https://github.com/pytorch-labs/tensordict},
+version = {0.1.1}, year = {2023} } ``` ## Disclaimer TensorDict is at the
+*beta*-stage, meaning that there may be bc-breaking changes introduced, but
+they should come with a warranty. Hopefully these should not happen too often,
+as the current roadmap mostly involves adding new features and building
+compatibility with the broader PyTorch ecosystem. ## License TensorDict is
+licensed under the MIT License. See [LICENSE](LICENSE) for details.
```

## Comparing `tensordict-0.1.0.dist-info/RECORD` & `tensordict-0.1.1.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,27 @@
-tensordict/__init__.py,sha256=TzlBunqtDVsaGqyrVWa-7zglgfqQ8Qy6WkD5kJsj_fI,859
-tensordict/memmap.py,sha256=RqGslaau2qw6K-vMEf3qCySHFdON7JLc1SL4Y__2_Mg,28442
-tensordict/tensordict.py,sha256=X7rTxOtciTnNCGbqh2XkDnWTmE4NS1F0ElplsiTVSTo,228528
-tensordict/utils.py,sha256=a-XQGPkO5OyXhTEoQa1a2abXdR5aRa4320pa7duOuXw,24542
-tensordict/version.py,sha256=Abe62JSz8zl09Wwxn_-rnzkDBsjLxBoxDMb6F0cNr8c,79
-tensordict/nn/__init__.py,sha256=4vBuSRfTECdRhewPLXqDXZ_bxTzVcYTyNjHSuJFGKME,1034
-tensordict/nn/common.py,sha256=c1RbAFqR6-ShOJAPsL29GXySyQCxo1w5DTBaqBAajB8,18445
-tensordict/nn/functional_modules.py,sha256=EXwoGu4lY8lENcV2IQt87jrnjzoI5W5iqlPXtAThEAE,14639
-tensordict/nn/probabilistic.py,sha256=zH5_PHEb6Mslpe8HOSecdDT6v_dx32OGK4eBy-i2eXs,18684
-tensordict/nn/sequence.py,sha256=G-jcf6slCO-GvCaD19uV0MWJs53fbuUaac3Z3ailh6Q,10925
-tensordict/nn/utils.py,sha256=klUTQV7ixDmcmUB6v2eFr4hbO0StxLZY-c8C4wRpeQI,3198
+tensordict/__init__.py,sha256=dDQidc208swLADInUxPlfvgfERJr2xeVTNC5NRvwN4A,1088
+tensordict/_contextlib.py,sha256=F4b0KH4FSeKsY9dkRuIXgHEn1dL_aNk7lFs1DonDYn4,6000
+tensordict/memmap.py,sha256=sBIRRJVadGiXlT5A8UfxoQqn6EEE1TBUDUaCyz65Yws,29601
+tensordict/persistent.py,sha256=CkF6hVsKAO21Le-7fuUChsLczoUr7Eflj6A6H7Z1XEo,33049
+tensordict/tensorclass.py,sha256=6eGhArep4GwEOeMFrdvv9MyVuy6oc4G58mhI2AVPh8M,30420
+tensordict/tensordict.py,sha256=raNiDj7w5CKompvO7wGDFxaPMfvqGPDR3YnOau0tko4,267125
+tensordict/utils.py,sha256=rZjY_b8mGys_YDWyWIQbZ1xeiJrXvG-u7sUxaSsjqIc,26209
+tensordict/version.py,sha256=jhJ2Sy4GJngPYcrvZZ4zbqaa04WBDg17E9l2N_F3pvk,79
+tensordict/nn/__init__.py,sha256=gjahPjJuC1uGPppYt7yZ8Ifusf2hTnOJHZGf8IutgoU,1314
+tensordict/nn/common.py,sha256=ncXtR3RsA3Ma5xxJILMi-W6or_hAmRwqZYsEaBxD208,35649
+tensordict/nn/functional_modules.py,sha256=jGJOUTaqCKO6Pmp8IuzGLWvej5WIOV26akH_0AMU7FI,19188
+tensordict/nn/probabilistic.py,sha256=ZYa7f2PzWqgwTw3TJAcd125HRpD4p6aPc1HD5o709WM,22301
+tensordict/nn/sequence.py,sha256=l5nuYu0Ja11IO9qWSlijvRZH4XDLbUy8lwkFmyAHrHE,19564
+tensordict/nn/utils.py,sha256=Hb8zIWL_wGs8OSaGjqQJ4DAadLqA9d4GARR7EboKOFU,10621
 tensordict/nn/distributions/__init__.py,sha256=sD3yMuMceDJ8EqtptE4HEaS9Q_3keskCB9npPNFKXUo,499
 tensordict/nn/distributions/continuous.py,sha256=Y31G7ozOnlGUgzdqYZaKeXVjDOVMoSW1hIQWtcbyDO0,7073
 tensordict/nn/distributions/discrete.py,sha256=gUzTKs3yO8GkSY0ghBWVaZdHdmFyMMLWd5LV52CfrXY,2580
 tensordict/nn/distributions/truncated_normal.py,sha256=d1ontYbG_Q-W5gcVnWLadvZ1OBBeZGmBb5EUmr3ekak,6504
 tensordict/nn/distributions/utils.py,sha256=fX6NUeNnWKK6kDdOp8NTM43Lls3vMCF5h-S2teVZw3E,1226
-tensordict/prototype/__init__.py,sha256=tpTW6Z2fzhHNtskx6cwsxAt7Kt4Sios0GboB3tdKfRU,382
+tensordict/prototype/__init__.py,sha256=b9Wmi1tbh2Em_wmKa52IXwxuudd6CUqdLgaob0bSWqQ,381
 tensordict/prototype/fx.py,sha256=Z3X821miRKcrOYwApvBDYt2_hST3IXNVe4v03tVvQKo,7507
-tensordict/prototype/tensorclass.py,sha256=FONMiHwNmNbFjKbtXS8uUH-PenOoAM2nM46HVYBv2sU,32673
-tensordict-0.1.0.dist-info/LICENSE,sha256=xdjS4_xk-IwnLuIFCvTYTl9Y8aXRejqpmke3dGam_nI,1098
-tensordict-0.1.0.dist-info/METADATA,sha256=phtIJ41j_hpiFkYWysJS88-MrZ-IVztSTbQnEWRXllY,14118
-tensordict-0.1.0.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-tensordict-0.1.0.dist-info/top_level.txt,sha256=4EMgKpsnmq04uFLPJXf8tMQb1POT8QqR1pR74y5wycc,11
-tensordict-0.1.0.dist-info/RECORD,,
+tensordict/prototype/tensorclass.py,sha256=pE53rWFqcPmuJOyOkI7cBZL9sMVfPx8bdQR1hNgYPvU,739
+tensordict-0.1.1.dist-info/LICENSE,sha256=xdjS4_xk-IwnLuIFCvTYTl9Y8aXRejqpmke3dGam_nI,1098
+tensordict-0.1.1.dist-info/METADATA,sha256=4DEZg_Nwe0Z27sKTb_Y44Vu9_-dnsR8oTlm1m4Ol70Y,15197
+tensordict-0.1.1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+tensordict-0.1.1.dist-info/top_level.txt,sha256=4EMgKpsnmq04uFLPJXf8tMQb1POT8QqR1pR74y5wycc,11
+tensordict-0.1.1.dist-info/RECORD,,
```

