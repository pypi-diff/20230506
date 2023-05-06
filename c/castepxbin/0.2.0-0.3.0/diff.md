# Comparing `tmp/castepxbin-0.2.0.tar.gz` & `tmp/castepxbin-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "castepxbin-0.2.0.tar", last modified: Thu Nov  4 20:53:12 2021, max compression
+gzip compressed data, was "castepxbin-0.3.0.tar", last modified: Sat May  6 06:42:48 2023, max compression
```

## Comparing `castepxbin-0.2.0.tar` & `castepxbin-0.3.0.tar`

### file list

```diff
@@ -1,19 +1,35 @@
-drwxr-xr-x   0 bonan     (1000) bonan     (1000)        0 2021-11-04 20:53:12.673551 castepxbin-0.2.0/
--rw-r--r--   0 bonan     (1000) bonan     (1000)     5990 2021-11-04 20:53:12.673551 castepxbin-0.2.0/PKG-INFO
--rw-r--r--   0 bonan     (1000) bonan     (1000)     4593 2021-11-04 20:30:43.000000 castepxbin-0.2.0/README.md
-drwxr-xr-x   0 bonan     (1000) bonan     (1000)        0 2021-11-04 20:53:12.673551 castepxbin-0.2.0/castepxbin/
--rw-r--r--   0 bonan     (1000) bonan     (1000)      145 2021-11-04 20:30:43.000000 castepxbin-0.2.0/castepxbin/__init__.py
--rw-r--r--   0 bonan     (1000) bonan     (1000)    27681 2021-11-04 20:30:43.000000 castepxbin-0.2.0/castepxbin/castep_bin.py
--rw-r--r--   0 bonan     (1000) bonan     (1000)        0 2021-10-20 18:23:25.000000 castepxbin-0.2.0/castepxbin/cst_esp.py
--rw-r--r--   0 bonan     (1000) bonan     (1000)        0 2021-10-20 18:23:28.000000 castepxbin-0.2.0/castepxbin/elf.py
--rw-r--r--   0 bonan     (1000) bonan     (1000)     4976 2021-11-04 20:30:43.000000 castepxbin-0.2.0/castepxbin/ome_bin.py
--rw-r--r--   0 bonan     (1000) bonan     (1000)    10810 2021-11-04 20:30:43.000000 castepxbin-0.2.0/castepxbin/pdos.py
--rw-r--r--   0 bonan     (1000) bonan     (1000)     7312 2021-11-04 20:30:43.000000 castepxbin-0.2.0/castepxbin/test_reader.py
-drwxr-xr-x   0 bonan     (1000) bonan     (1000)        0 2021-11-04 20:53:12.673551 castepxbin-0.2.0/castepxbin.egg-info/
--rw-r--r--   0 bonan     (1000) bonan     (1000)     5990 2021-11-04 20:53:12.000000 castepxbin-0.2.0/castepxbin.egg-info/PKG-INFO
--rw-r--r--   0 bonan     (1000) bonan     (1000)      342 2021-11-04 20:53:12.000000 castepxbin-0.2.0/castepxbin.egg-info/SOURCES.txt
--rw-r--r--   0 bonan     (1000) bonan     (1000)        1 2021-11-04 20:53:12.000000 castepxbin-0.2.0/castepxbin.egg-info/dependency_links.txt
--rw-r--r--   0 bonan     (1000) bonan     (1000)      154 2021-11-04 20:53:12.000000 castepxbin-0.2.0/castepxbin.egg-info/requires.txt
--rw-r--r--   0 bonan     (1000) bonan     (1000)       11 2021-11-04 20:53:12.000000 castepxbin-0.2.0/castepxbin.egg-info/top_level.txt
--rw-r--r--   0 bonan     (1000) bonan     (1000)       38 2021-11-04 20:53:12.673551 castepxbin-0.2.0/setup.cfg
--rw-r--r--   0 bonan     (1000) bonan     (1000)     1281 2021-11-04 20:13:38.000000 castepxbin-0.2.0/setup.py
+-rw-r--r--   0        0        0     1762 2023-05-06 06:42:42.983312 castepxbin-0.3.0/.github/workflows/docs.yml
+-rw-r--r--   0        0        0     1528 2023-05-06 06:42:42.983312 castepxbin-0.3.0/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0      751 2023-05-06 06:42:42.983312 castepxbin-0.3.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     2120 2023-05-06 06:42:42.983312 castepxbin-0.3.0/.gitignore
+-rw-r--r--   0        0        0      964 2023-05-06 06:42:42.983312 castepxbin-0.3.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      212 2023-05-06 06:42:42.983312 castepxbin-0.3.0/.prospector.yaml
+-rw-r--r--   0        0        0    13807 2023-05-06 06:42:42.983312 castepxbin-0.3.0/.pylintrc
+-rw-r--r--   0        0        0     1066 2023-05-06 06:42:42.983312 castepxbin-0.3.0/LICENSE
+-rw-r--r--   0        0        0     4863 2023-05-06 06:42:42.983312 castepxbin-0.3.0/README.md
+-rw-r--r--   0        0        0      145 2023-05-06 06:42:42.983312 castepxbin-0.3.0/castepxbin/__init__.py
+-rw-r--r--   0        0        0    28157 2023-05-06 06:42:42.983312 castepxbin-0.3.0/castepxbin/castep_bin.py
+-rw-r--r--   0        0        0     4976 2023-05-06 06:42:42.983312 castepxbin-0.3.0/castepxbin/ome_bin.py
+-rw-r--r--   0        0        0    11007 2023-05-06 06:42:42.983312 castepxbin-0.3.0/castepxbin/pdos.py
+-rw-r--r--   0        0        0     5676 2023-05-06 06:42:42.983312 castepxbin-0.3.0/castepxbin/wave.py
+-rw-r--r--   0        0        0       13 2023-05-06 06:42:42.983312 castepxbin-0.3.0/docs/.gitignore
+-rw-r--r--   0        0        0      634 2023-05-06 06:42:42.983312 castepxbin-0.3.0/docs/Makefile
+-rw-r--r--   0        0        0     3258 2023-05-06 06:42:42.983312 castepxbin-0.3.0/docs/conf.py
+-rw-r--r--   0        0        0      453 2023-05-06 06:42:42.983312 castepxbin-0.3.0/docs/index.md
+-rw-r--r--   0        0        0      338 2023-05-06 06:42:42.983312 castepxbin-0.3.0/docs/installation.md
+-rw-r--r--   0        0        0      800 2023-05-06 06:42:42.983312 castepxbin-0.3.0/docs/make.bat
+-rw-r--r--   0        0        0     2610 2023-05-06 06:42:42.983312 castepxbin-0.3.0/docs/usage.md
+-rw-r--r--   0        0        0     1165 2023-05-06 06:42:42.983312 castepxbin-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0    16546 2023-05-06 06:42:42.983312 castepxbin-0.3.0/tests/test_data/Si2-out.cell
+-rw-r--r--   0        0        0   193647 2023-05-06 06:42:42.983312 castepxbin-0.3.0/tests/test_data/Si2-sc-skew.castep_bin
+-rw-r--r--   0        0        0    47257 2023-05-06 06:42:42.983312 castepxbin-0.3.0/tests/test_data/Si2.bands
+-rw-r--r--   0        0        0      266 2023-05-06 06:42:42.983312 castepxbin-0.3.0/tests/test_data/Si2.cell
+-rw-r--r--   0        0        0  4410479 2023-05-06 06:42:43.011312 castepxbin-0.3.0/tests/test_data/Si2.check
+-rw-r--r--   0        0        0    76176 2023-05-06 06:42:43.015312 castepxbin-0.3.0/tests/test_data/Si2.cst_ome
+-rw-r--r--   0        0        0    61704 2023-05-06 06:42:43.015312 castepxbin-0.3.0/tests/test_data/Si2.dome_bin
+-rw-r--r--   0        0        0    50904 2023-05-06 06:42:43.015312 castepxbin-0.3.0/tests/test_data/Si2.ome_bin
+-rw-r--r--   0        0        0      149 2023-05-06 06:42:43.015312 castepxbin-0.3.0/tests/test_data/Si2.param
+-rw-r--r--   0        0        0   189032 2023-05-06 06:42:43.015312 castepxbin-0.3.0/tests/test_data/Si2.pdos_bin
+-rw-r--r--   0        0        0   634669 2023-05-06 06:42:43.019312 castepxbin-0.3.0/tests/test_data/SiO2.castep_bin
+-rw-r--r--   0        0        0     8765 2023-05-06 06:42:43.019312 castepxbin-0.3.0/tests/test_reader.py
+-rw-r--r--   0        0        0     6305 1970-01-01 00:00:00.000000 castepxbin-0.3.0/PKG-INFO
```

### Comparing `castepxbin-0.2.0/PKG-INFO` & `castepxbin-0.3.0/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,121 +1,107 @@
-Metadata-Version: 2.1
-Name: castepxbin
-Version: 0.2.0
-Summary: A collection of readers for CASTEP binary outputs
-Home-page: https://github.com/zhubonan/castepxbin
-Author: Bonan Zhu
-Author-email: zhubonan@outlook.com
-License: MIT License
-Description: # castepxbin
-        
-        ## Overview
-        
-        A collection of readers for binary output from [CASTEP](http://www.castep.org).
-        
-        Available readers for:
-        
-        - `castep_bin`: The compact checkpoint file contains all internal data stored by CASTEP (excluding the wavefunction) and may be read for restarting. High precision forces can be read from this file for single point calculations, as the `geom` file not written.
-        - `pdos_bin`: Weights for computing the projected density of states.
-        - `ome_bin`: Optical matrix elements from the *Spectral* task.
-        - `dome_bin`: Diagonal elements (band gradients) of the optical matrix from the *Spectral* task.
-        - `cst_ome`: Legacy format containing optical matrix elements from the *Optics* task.
-        
-        
-        To-dos:
-        
-        - `cst_esp`: Electrostatic potentials?
-        - `elf`: Electron localsation function.
-        - More data from `castep_bin`/`check` files.
-        
-        
-        ## Installation
-        
-        This package can be install using `pip`
-        
-        ```
-        pip install castepxbin
-        ```
-        
-        To install extra dependencies may be needed for testing:
-        
-        ```
-        pip install castepxbin[testing]
-        ```
-        
-        Or directly from the GitHub repo:
-        
-        ```
-        pip install git+https://github.com/zhubonan/castepxbin.git
-        ```
-        
-        The two main dependencies are `numpy` and `scipy`.
-        The optional `pymatgen` dependency is used for naming the orbitals.
-        Please note that the consistency of these labels for the f orbitals has not been checked.
-        
-        ## Usage
-        
-        Simply import the function and pass the file path. For the `castep_bin` reader, the example is shown below:
-        
-        ```python
-        In [1]: from castepxbin import read_castep_bin
-        
-        In [2]: data = read_castep_bin("test_data/SiO2.castep_bin")
-        
-        In [3]: data.keys()
-        Out[3]: dict_keys(['elec_temp', 'electronic_minimizer', 'nelectrons', 'nup', 'ndown', 'spin', 'charge', 'spin_treatment', 'num_ions_orig', 'max_ions_in_species_orig', 'real_lattice_orig', 'recip_lattice_orig', 'num_species_orig', 'num_ions_in_species_orig', 'ionic_positions', 'species_symbol_orig', 'num_ions', 'max_ions_in_species', 'real_lattice', 'recip_lattice', 'num_species', 'num_ions_in_species', 'species_symbol', 'nkpts', 'kpoints', 'kpoint_weights', 'found_ground_state_wavefunction', 'found_ground_state_density', 'total_energy', 'fermi_energy', 'nbands', 'nspins', 'occupancies', 'eigenvalues', 'kpoints_of_eigenvalues', 'ngx_fine', 'ngy_fine', 'ngz_fine', 'spin_density', 'charge_density', 'fermi_energy_second_spin', 'forces'])
-        ```
-        
-        Note that these readers should be considered as "low-level" as they corresponds to unprocessed Fortran data as it is. Further processes are often needed, such reordering the axes (Fortran arrays are column-major) and recasting into different `dtype`s.
-        
-        Once exception is for the optical matrix element reader, where output array are converted into the "C" (row-major) ordering internally.
-        
-        ### Extending the `castep_bin` reader
-        
-        At the moment, not all sections of the `castep_bin` is read (as there are too many!), but more contents can be added easily by including relevant sections in the `castepxbin.castep_bin.CASTEP_BIN_FIELD_SPEC` dictionary. The `read_castep_bin` function can accept such modified version instead of using the default one.
-        
-        For example, suppose the binary field is written as such:
-        
-        ```fortran
-        header = 'MY_SECTION'
-        write(unit) header
-        write(unit) my_int    # An INTEGER(4)
-        write(unit) my_bool    # An LOGICAL type
-        write(unit) my_array    # An array of real numbers with size (3, nspecies, my_int)
-        header = 'END_MY_SECTION'
-        write(unit) header
-        ```
-        
-        The the following specifications can be added to read the section:
-        
-        ```python
-        my_spec = dict(CASTEP_BIN_FIELD_SPEC)
-        my_spec['MY_SECTION'] = (
-                ScalarField('my_int', int),
-                BoolField('my_bool'),
-                ArrayField('my_array', float, shape=(3, 'nspecies', 'my_int'))
-        )
-        ```
-        
-        The value of `my_int` is unknown, but it is read before processing the `my_array` field.
-        This imples that the order of fields in `CASTEP_BIN_FIELD_SPEC` can be important, as certain array sizes are only available from other fields, such as the `nspecies` field above.
-        However, even if `nspecies` is not read previously, it can still be resolved by inspecting the length of the record.
-        This would not be possible if there are two unknown dimension sizes.
-        
-        ## Acknowledgement
-        
-        The data structures of binary `pdos_bin`, `dome_bin`, `ome_bin`, files are inferred from the code snippet
-        in the documentation of the open sourced [OptaDOS](https://github.com/optados-developers/optados) package for computing high quality DOS and other spectral properties using outputs from CASTEP.
-        
-        ## Contributors
-        
-        - Bonan Zhu, University College London
-        - Matthew Evans, UCLouvain/University of Cambridge
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Development Status :: 4 - Beta
-Description-Content-Type: text/markdown
-Provides-Extra: testing
-Provides-Extra: pmg
-Provides-Extra: pre-commit
+# castepxbin
+
+[Documentation](https://zhubonan.github.io/castepxbin/)
+## Overview
+
+A collection of readers for binary output from [CASTEP](http://www.castep.org).
+
+Available readers for:
+
+- `castep_bin`: The compact checkpoint file contains all internal data stored by CASTEP (excluding the wavefunction) and may be read for restarting. High precision forces can be read from this file for single point calculations, as the `geom` file not written.
+- `check`: Same as `castep_bin` but includes wave function data (SCF kpoints).
+- `orbitals`: Same as `check` but includes wave function data for sampled (none-SCF) k-points in spectral/bandstructure/optics tasks.
+- `pdos_bin`: Weights for computing the projected density of states.
+- `ome_bin`: Optical matrix elements from the *Spectral* task.
+- `dome_bin`: Diagonal elements (band gradients) of the optical matrix from the *Spectral* task.
+- `cst_ome`: Legacy format containing optical matrix elements from the *Optics* task.
+
+
+To-dos:
+
+- `cst_esp`: Electrostatic potentials?
+- `elf`: Electron localsation function.
+- More data from `castep_bin`/`check` files.
+
+
+## Installation
+
+This package can be install using `pip`
+
+```
+pip install castepxbin
+```
+
+To install extra dependencies may be needed for testing:
+
+```
+pip install castepxbin[testing]
+```
+
+Or directly from the GitHub repo:
+
+```
+pip install git+https://github.com/zhubonan/castepxbin.git
+```
+
+The two main dependencies are `numpy` and `scipy`.
+The optional `pymatgen` dependency is used for naming the orbitals.
+Please note that the consistency of these labels for the f orbitals has not been checked.
+
+## Usage
+
+Simply import the function and pass the file path. For the `castep_bin` reader, the example is shown below:
+
+```python
+In [1]: from castepxbin import read_castep_bin
+
+In [2]: data = read_castep_bin("test_data/SiO2.castep_bin")
+
+In [3]: data.keys()
+Out[3]: dict_keys(['elec_temp', 'electronic_minimizer', 'nelectrons', 'nup', 'ndown', 'spin', 'charge', 'spin_treatment', 'num_ions_orig', 'max_ions_in_species_orig', 'real_lattice_orig', 'recip_lattice_orig', 'num_species_orig', 'num_ions_in_species_orig', 'ionic_positions', 'species_symbol_orig', 'num_ions', 'max_ions_in_species', 'real_lattice', 'recip_lattice', 'num_species', 'num_ions_in_species', 'species_symbol', 'nkpts', 'kpoints', 'kpoint_weights', 'found_ground_state_wavefunction', 'found_ground_state_density', 'total_energy', 'fermi_energy', 'nbands', 'nspins', 'occupancies', 'eigenvalues', 'kpoints_of_eigenvalues', 'ngx_fine', 'ngy_fine', 'ngz_fine', 'spin_density', 'charge_density', 'fermi_energy_second_spin', 'forces'])
+```
+
+Note that these readers should be considered as "low-level" as they corresponds to unprocessed Fortran data as it is. Further processes are often needed, such reordering the axes (Fortran arrays are column-major) and recasting into different `dtype`s.
+
+Once exception is for the optical matrix element reader, where output array are converted into the "C" (row-major) ordering internally.
+
+### Extending the `castep_bin` reader
+
+At the moment, not all sections of the `castep_bin` is read (as there are too many!), but more contents can be added easily by including relevant sections in the `castepxbin.castep_bin.CASTEP_BIN_FIELD_SPEC` dictionary. The `read_castep_bin` function can accept such modified version instead of using the default one.
+
+For example, suppose the binary field is written as such:
+
+```fortran
+header = 'MY_SECTION'
+write(unit) header
+write(unit) my_int    # An INTEGER(4)
+write(unit) my_bool    # An LOGICAL type
+write(unit) my_array    # An array of real numbers with size (3, nspecies, my_int)
+header = 'END_MY_SECTION'
+write(unit) header
+```
+
+The the following specifications can be added to read the section:
+
+```python
+my_spec = dict(CASTEP_BIN_FIELD_SPEC)
+my_spec['MY_SECTION'] = (
+        ScalarField('my_int', int),
+        BoolField('my_bool'),
+        ArrayField('my_array', float, shape=(3, 'nspecies', 'my_int'))
+)
+```
+
+The value of `my_int` is unknown, but it is read before processing the `my_array` field.
+This imples that the order of fields in `CASTEP_BIN_FIELD_SPEC` can be important, as certain array sizes are only available from other fields, such as the `nspecies` field above.
+However, even if `nspecies` is not read previously, it can still be resolved by inspecting the length of the record.
+This would not be possible if there are two unknown dimension sizes.
+
+## Acknowledgement
+
+The data structures of binary `pdos_bin`, `dome_bin`, `ome_bin`, files are inferred from the code snippet
+in the documentation of the open sourced [OptaDOS](https://github.com/optados-developers/optados) package for computing high quality DOS and other spectral properties using outputs from CASTEP.
+
+## Contributors
+
+- Bonan Zhu, University College London
+- Matthew Evans, UCLouvain/University of Cambridge
```

### Comparing `castepxbin-0.2.0/castepxbin/castep_bin.py` & `castepxbin-0.3.0/castepxbin/castep_bin.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,38 +5,38 @@
 CASTEP run.
 
 Reading this file can be beneficial as it uses the native floating-point
 precision of the CASTEP run itself.
 
 This implementation takes inspiration from similar functions in the
 the [Euphonic](https://github.com/pace-neutrons/Euphonic) package.
-
 """
 
+import io
+
 # pylint: disable=invalid-name,too-few-public-methods
 import re
-
-from typing import Union, Dict, Any, Tuple, Collection, Optional, List
 from pathlib import Path
 from struct import unpack
-import io
+from typing import Any, Collection, Dict, List, Optional, Tuple, Union
 
 import numpy as np
 
-__all__ = ("read_castep_bin", )
+__all__ = ("read_castep_bin",)
 
 TYPE_MAP = {
     int: "i4",
     float: "f8",
     complex: "c16",
 }
 
 
 class FieldType:
     """Abstract representation of the field type"""
+
     def __init__(self, name, dtype, endian="BIG"):
         self.name = name
         ed = ">" if endian.lower() == "big" else "<"
         dtype = TYPE_MAP.get(dtype, dtype)
         self.type_string = f"{ed}{dtype}"
 
     def decode(self, fp, decoded=None, record_data=None):
@@ -44,52 +44,53 @@
         Decode the field with given file object or existing byte array
         """
         _ = decoded
         if record_data is None:
             record_data, marker = _read_record(fp)
         else:
             marker = len(record_data)
-        count = marker // int(
-            re.match(r"[><][a-z?]+(\d+)", self.type_string).group(1))
-        return np.frombuffer(record_data,
-                             np.dtype(self.type_string),
-                             count=count)
+        count = marker // int(re.match(r"[><][a-z?]+(\d+)", self.type_string).group(1))
+        return np.frombuffer(record_data, np.dtype(self.type_string), count=count)
 
 
 class CompositeField:
     """Composition field - multiple entities are stored in a single record"""
+
     def __init__(self, fields: List[FieldType]) -> None:
         super().__init__()
         self.fields = fields
 
 
 class ScalarField(FieldType):
     """Abstract Representation of sclar type"""
+
     def decode(self, fp, decoded=None, record_data=None):
         array = super().decode(fp, decoded, record_data)
         return array.tolist()[0]
 
     @property
     def shape(self):
-        return (1, )
+        return (1,)
 
 
 class SkippedField(FieldType):
     """A field that will be skipped"""
+
     def __init__(self):
-        super().__init__("None", dtype='i4')
+        super().__init__("None", dtype="i4")
 
     def decode(self, fp, decoded=None, record_data=None):
         """Recode - read the field the advance the stream"""
         _read_record(fp)
 
 
 class ArrayField(ScalarField):
     """Abstract Representation of a Array type"""
-    def __init__(self, name, dtype, shape, endian='BIG'):
+
+    def __init__(self, name, dtype, shape, endian="BIG"):
         """Instantiate an array field"""
         super().__init__(name, dtype, endian)
         self._shape = shape
 
     @property
     def shape(self):
         return self._shape
@@ -126,326 +127,428 @@
             record_data, _ = _read_record(fp)
         if decoded is None:
             decoded = {}
         shape, missing_dim = self.resolve_shape(decoded)
         count = np.prod(shape)
         # Fully specified
         if count > 0:
-            array = np.frombuffer(record_data,
-                                  np.dtype(self.type_string),
-                                  count=count)
+            array = np.frombuffer(record_data, np.dtype(self.type_string), count=count)
         else:
             # Not fully specified - in this case we read the full record
-            array = np.frombuffer(record_data,
-                                  np.dtype(self.type_string),
-                                  count=-1)
+            array = np.frombuffer(record_data, np.dtype(self.type_string), count=-1)
             # Work out the missing dimension...
             tot = array.size
-            left = -tot / np.prod(
-                [elem for elem in shape if isinstance(elem, int)])
+            left = -tot / np.prod([elem for elem in shape if isinstance(elem, int)])
             decoded[missing_dim] = int(left)
             # Reconstruct the shape array
             actual_shape = []
             for elem in shape:
                 if elem == -1:
                     actual_shape.append(int(left))
                 else:
                     actual_shape.append(elem)
             shape = actual_shape
 
         # Special case for 1D string array - return a list of strings
-        if 'a' in self.type_string and len(self.shape) == 1:
+        if "a" in self.type_string and len(self.shape) == 1:
             return [tmp.decode().strip() for tmp in array]
-        array = np.reshape(array, shape, order='F')
+        array = np.reshape(array, shape, order="F")
         return array
 
 
 class StrField(ScalarField):
     """Abstract Representation of a Array type"""
+
     def decode(self, fp, decoded=None, record_data=None):
         bdata = super().decode(fp, decoded, record_data)
         return bdata.decode().strip()
 
 
 class BoolField(ScalarField):
     """
     A boolean field
 
     Note that LOGICAL type is typically represented as INTEGER by Fortran.
     Different compilers may have different conventions, but 0 can be consistently
     identified as .FALSE.
     """
-    def __init__(self, name, endian='BIG'):
+
+    def __init__(self, name, endian="BIG"):
         super().__init__(name, "i4", endian)
 
     def decode(self, fp, decoded=None, record_data=None):
         val = super().decode(fp, decoded, record_data)
         return bool(val)  # Anything !=0 is True
 
 
 class StructuredField:
     """A field that require case-by-case parsing"""
-    def __init__(self, endian='BIG'):
+
+    def __init__(self, endian="BIG"):
         self.endian = endian
         self.endian_sym = ">" if endian.lower() == "big" else "<"
 
 
 class EigenValueAndOccCompositeField(StructuredField):
     """Complex field for the eigenvalues and the occupations"""
+
     def decode(self, fp, decoded_data, record_data=None):
         """Decode the occupation and eigenvalues field"""
         _ = record_data
-        nbands = decoded_data['nbands']
-        nspin = decoded_data['nspins']
-        nkpts = decoded_data['nkpts']
+        nbands = decoded_data["nbands"]
+        nspin = decoded_data["nspins"]
+        nkpts = decoded_data["nkpts"]
         kpoints = np.zeros((3, nkpts))
         occ = np.zeros((nbands, nkpts, nspin))
         eigenvalues = np.zeros((nbands, nkpts, nspin))
 
         # Now start reading
         for ik in range(nkpts):
             data, _ = _read_record(fp)
             kpoints[:, ik] = np.frombuffer(data, self.endian_sym + "f8")
             for idx_spin in range(nspin):
                 data, _ = _read_record(fp)
-                occ[:, ik, idx_spin] = np.frombuffer(data,
-                                                     self.endian_sym + "f8")
+                occ[:, ik, idx_spin] = np.frombuffer(data, self.endian_sym + "f8")
                 data, _ = _read_record(fp)
                 eigenvalues[:, ik, idx_spin] = np.frombuffer(
-                    data, self.endian_sym + "f8")
+                    data, self.endian_sym + "f8"
+                )
         decoded_data["occupancies"] = occ
         decoded_data["eigenvalues"] = eigenvalues
         # Kpoints consistent with the order of eigenvalues and occupancies - as distribution of the
         # kpoints may result in a different order compared to those specified in the CELL part
         decoded_data["kpoints_of_eigenvalues"] = kpoints
 
 
 class ChargeDensityField(StructuredField):
     """For reading charge density"""
+
     def decode(self, fp, decoded_data, record_data=None):
         """
         Decode the charge density
         """
         _ = record_data
-        ngx_fine = decoded_data['ngx_fine']
-        ngy_fine = decoded_data['ngy_fine']
-        ngz_fine = decoded_data['ngz_fine']
-        nspin = decoded_data['nspins']
+        ngx_fine = decoded_data["ngx_fine"]
+        ngy_fine = decoded_data["ngy_fine"]
+        ngz_fine = decoded_data["ngz_fine"]
+        nspin = decoded_data["nspins"]
 
         # Check if NCM
-        has_ncm = decoded_data['spin_treatment'] == "VECTOR"
+        has_ncm = decoded_data["spin_treatment"] == "VECTOR"
 
-        charge_density = np.zeros((ngx_fine, ngy_fine, ngz_fine),
-                                  dtype=complex)
+        charge_density = np.zeros((ngx_fine, ngy_fine, ngz_fine), dtype=complex)
         zcol = np.zeros(ngz_fine, dtype=complex)
 
         if nspin == 2 and not has_ncm:
-            spin_density = np.zeros((ngx_fine, ngy_fine, ngz_fine),
-                                    dtype=complex)
+            spin_density = np.zeros((ngx_fine, ngy_fine, ngz_fine), dtype=complex)
 
         if has_ncm:
-            spin_density = np.zeros((ngx_fine, ngy_fine, ngz_fine, 3),
-                                    dtype=complex)
+            spin_density = np.zeros((ngx_fine, ngy_fine, ngz_fine, 3), dtype=complex)
 
         for _ in range(ngx_fine):
             for _ in range(ngy_fine):
                 data, _ = _read_record(fp)
-                nx = np.frombuffer(data,
-                                   self.endian_sym + "i4",
-                                   offset=0,
-                                   count=1)[0]
-                ny = np.frombuffer(data,
-                                   self.endian_sym + "i4",
-                                   offset=4,
-                                   count=1)[0]
-                zcol = np.frombuffer(data,
-                                     self.endian_sym + "c16",
-                                     offset=8,
-                                     count=ngz_fine)
+                nx = np.frombuffer(data, self.endian_sym + "i4", offset=0, count=1)[0]
+                ny = np.frombuffer(data, self.endian_sym + "i4", offset=4, count=1)[0]
+                zcol = np.frombuffer(
+                    data, self.endian_sym + "c16", offset=8, count=ngz_fine
+                )
                 charge_density[nx - 1, ny - 1, :] = zcol
                 # For NSPIN = 2
                 if nspin == 2 and not has_ncm:
-                    spin_col = np.frombuffer(data,
-                                             self.endian_sym + "c16",
-                                             offset=8 + 16 * ngz_fine,
-                                             count=ngz_fine)
+                    spin_col = np.frombuffer(
+                        data,
+                        self.endian_sym + "c16",
+                        offset=8 + 16 * ngz_fine,
+                        count=ngz_fine,
+                    )
                     spin_density[nx - 1, ny - 1, :] = spin_col
                 if has_ncm:
-                    spin_col = np.frombuffer(data,
-                                             self.endian_sym + "c16",
-                                             offset=8 + 16 * ngz_fine,
-                                             count=ngz_fine * 3)
+                    spin_col = np.frombuffer(
+                        data,
+                        self.endian_sym + "c16",
+                        offset=8 + 16 * ngz_fine,
+                        count=ngz_fine * 3,
+                    )
                     spin_density[nx - 1, ny - 1, :, :] = spin_col.reshape(
-                        (ngz_fine, 3), order='C')
+                        (ngz_fine, 3), order="C"
+                    )
 
         if nspin == 2 or has_ncm:
             decoded_data["spin_density"] = spin_density
         decoded_data["charge_density"] = charge_density
 
 
+class WaveFunctionField(StructuredField):
+    """For reading the wave function"""
+
+    STORE_COEFFS = False
+
+    @staticmethod
+    def decode(fp, decoded_data, record_data=None):
+        """
+        Decode the charge density
+        """
+        _ = record_data
+        ngx = decoded_data["ngx"]
+        ngy = decoded_data["ngy"]
+        ngz = decoded_data["ngz"]
+        spinorcomps = decoded_data["wave_spinorcomps"]
+        nbands_max = decoded_data["wave_nbands_max"]
+        nkpts = decoded_data["wave_nkpts"]
+        nspins = decoded_data["wave_nspins"]
+        coeff_size_1 = decoded_data["wave_coeff_size_1"]
+
+        # Main storage space for the coefficients
+        coeffs = np.zeros(
+            (coeff_size_1, spinorcomps, nbands_max, nkpts, nspins),
+            order="F",
+            dtype=complex,
+        )
+
+        nwaves_at_kp = np.zeros(nkpts, dtype=int)
+        kpts = np.zeros((3, nkpts), dtype=float, order="F")
+        pw_grid_coord = np.zeros((3, coeff_size_1, nkpts), dtype=int, order="F")
+
+        record_spec1 = CompositeField(
+            [ArrayField("kpt", dtype=float, shape=(3,)), ScalarField("nwaves", int)]
+        )
+
+        for ispin in range(nspins):
+            for ik in range(nkpts):
+                (  # pylint: disable=unbalanced-tuple-unpacking
+                    kpts[:, ik],
+                    nwaves,
+                ) = _decode_composite(fp, record_spec1)
+                nwaves_at_kp[ik] = nwaves
+                wavecoords_spec = ArrayField("grid", int, (nwaves,))
+                coeff_spec = ArrayField("coeff", complex, (nwaves,))
+                # Read the coordinates of the plane waves with the unit of the reciprocal lattice vectors
+                coords_x = wavecoords_spec.decode(fp)
+                coords_y = wavecoords_spec.decode(fp)
+                coords_z = wavecoords_spec.decode(fp)
+                pw_grid_coord[0, :nwaves, ik] = coords_x
+                pw_grid_coord[1, :nwaves, ik] = coords_y
+                pw_grid_coord[2, :nwaves, ik] = coords_z
+                for iband in range(nbands_max):
+                    for ispinor in range(spinorcomps):
+                        this_coeff = coeff_spec.decode(fp)
+                        coeffs[:nwaves, ispinor, iband, ik, ispin] = this_coeff
+
+        # Collect the data
+        data = {
+            "ngx": ngx,
+            "ngy": ngy,
+            "ngz": ngz,
+            "pw_grid_coords": pw_grid_coord,
+            "coeffs": coeffs,
+            "kpts": kpts,
+            "nwaves_at_kp": nwaves_at_kp,
+            **{
+                key.replace("wave_", ""): value
+                for key, value in decoded_data.items()
+                if key.startswith("wave_")
+            },
+        }
+        # Save the data under the key 'wavefunction'
+        decoded_data["wavefunction"] = data
+
+
 # Defines the location of field relative to the tags
 CASTEP_BIN_FIELD_SPEC = {
     # Parameters
     "BEGIN_ELECTRONIC": (
         SkippedField(),
         SkippedField(),
         SkippedField(),
         SkippedField(),  # nspin
-        SkippedField(),  #nbands - no need to read again
-        ScalarField("elec_temp", float),  #elect
+        SkippedField(),  # nbands - no need to read again
+        ScalarField("elec_temp", float),  # elect
         SkippedField(),
         SkippedField(),
         SkippedField(),
         StrField("electronic_minimizer", "a10"),
         ScalarField("nelectrons", float),
         ScalarField("nup", float),
         ScalarField("ndown", float),
         ScalarField("spin", float),
         ScalarField("charge", float),
         StrField("spin_treatment", "a20"),
     ),
-
     # The "original" cell
-    "CELL%NUM_IONS": (ScalarField("num_ions_orig", int), ),
-    "CELL%MAX_IONS_IN_SPECIES": (ScalarField("max_ions_in_species_orig",
-                                             int), ),
-    "CELL%REAL_LATTICE": (ArrayField("real_lattice_orig", float, (
-        3,
-        3,
-    )), ),
-    "CELL%RECIP_LATTICE": (ArrayField("recip_lattice_orig", float, (
-        3,
-        3,
-    )), ),
-    "CELL%NUM_SPECIES": (ScalarField("num_species_orig", int), ),
-    "CELL%NUM_IONS_IN_SPECIES": (ArrayField("num_ions_in_species_orig", int,
-                                            ("num_species_orig", )), ),
-    "CELL%IONIC_POSITIONS":
-    (ArrayField("ionic_positions", float,
-                (3, "max_ions_in_species_orig", "num_species_orig")), ),
-    "CELL%SPECIES_SYMBOL": (ArrayField("species_symbol_orig", 'a8',
-                                       ("num_species_orig", )), ),
-
+    "CELL%NUM_IONS": (ScalarField("num_ions_orig", int),),
+    "CELL%MAX_IONS_IN_SPECIES": (ScalarField("max_ions_in_species_orig", int),),
+    "CELL%REAL_LATTICE": (
+        ArrayField(
+            "real_lattice_orig",
+            float,
+            (
+                3,
+                3,
+            ),
+        ),
+    ),
+    "CELL%RECIP_LATTICE": (
+        ArrayField(
+            "recip_lattice_orig",
+            float,
+            (
+                3,
+                3,
+            ),
+        ),
+    ),
+    "CELL%NUM_SPECIES": (ScalarField("num_species_orig", int),),
+    "CELL%NUM_IONS_IN_SPECIES": (
+        ArrayField("num_ions_in_species_orig", int, ("num_species_orig",)),
+    ),
+    "CELL%IONIC_POSITIONS": (
+        ArrayField(
+            "ionic_positions",
+            float,
+            (3, "max_ions_in_species_orig", "num_species_orig"),
+        ),
+    ),
+    "CELL%SPECIES_SYMBOL": (
+        ArrayField("species_symbol_orig", "a8", ("num_species_orig",)),
+    ),
     # The "current" cell
-    "CELL%NUM_IONS_01": (ScalarField("num_ions", int), ),
-    "CELL%MAX_IONS_IN_SPECIES_01": (ScalarField("max_ions_in_species", int), ),
-    "CELL%REAL_LATTICE_01": (ArrayField("real_lattice", float, (
-        3,
-        3,
-    )), ),
-    "CELL%RECIP_LATTICE_01": (ArrayField("recip_lattice", float, (
-        3,
-        3,
-    )), ),
-    "CELL%NUM_SPECIES_01": (ScalarField("num_species", int), ),
-    "CELL%NUM_IONS_IN_SPECIES_01": (ArrayField("num_ions_in_species", int,
-                                               ("num_species", )), ),
-    "CELL%IONIC_POSITIONS_01":
-    (ArrayField("ionic_positions", float,
-                (3, "max_ions_in_species", "num_species")), ),
-    "CELL%SPECIES_SYMBOL_01": (ArrayField("species_symbol", 'a8',
-                                          ("num_species", )), ),
-    "NKPTS_01": (ScalarField("nkpts", int), ),
-    "KPOINTS_01":
-    (ArrayField("kpoints", float,
-                shape=(3, "nkpts")), ),  # Kpoints in the original order
-    "KPOINT_WEIGHTS_01":
-    (ArrayField("kpoint_weights", float,
-                shape=("nkpts", )), ),  # Weights in the original order
-
+    "CELL%NUM_IONS_01": (ScalarField("num_ions", int),),
+    "CELL%MAX_IONS_IN_SPECIES_01": (ScalarField("max_ions_in_species", int),),
+    "CELL%REAL_LATTICE_01": (
+        ArrayField(
+            "real_lattice",
+            float,
+            (
+                3,
+                3,
+            ),
+        ),
+    ),
+    "CELL%RECIP_LATTICE_01": (
+        ArrayField(
+            "recip_lattice",
+            float,
+            (
+                3,
+                3,
+            ),
+        ),
+    ),
+    "CELL%NUM_SPECIES_01": (ScalarField("num_species", int),),
+    "CELL%NUM_IONS_IN_SPECIES_01": (
+        ArrayField("num_ions_in_species", int, ("num_species",)),
+    ),
+    "CELL%IONIC_POSITIONS_01": (
+        ArrayField("ionic_positions", float, (3, "max_ions_in_species", "num_species")),
+    ),
+    "CELL%SPECIES_SYMBOL_01": (ArrayField("species_symbol", "a8", ("num_species",)),),
+    "NKPTS_01": (ScalarField("nkpts", int),),
+    "KPOINTS_01": (
+        ArrayField("kpoints", float, shape=(3, "nkpts")),
+    ),  # Kpoints in the original order
+    "KPOINT_WEIGHTS_01": (
+        ArrayField("kpoint_weights", float, shape=("nkpts",)),
+    ),  # Weights in the original order
     # Parameters starts after the end of the global section of the "current" cell
     "END_CELL_GLOBAL_01": (
-        BoolField("found_ground_state_wavefunction"
-                  ),  # Fortran logical saved as integer....
+        BoolField(
+            "found_ground_state_wavefunction"
+        ),  # Fortran logical saved as integer....
         BoolField("found_ground_state_density"),
         ScalarField("total_energy", float),
         ScalarField("fermi_energy", float),
+        CompositeField([ScalarField("nbands", int), ScalarField("nspins", int)]),
+        EigenValueAndOccCompositeField(),  # Read the eigenvalues note that the arrays are reshaped
+        BoolField("found_ground_state_density"),
         CompositeField(
-            [ScalarField("nbands", int),
-             ScalarField("nspins", int)]),
-        EigenValueAndOccCompositeField(
-        ),  # Read the eigenvalues note that the arrays are reshaped
+            [
+                ScalarField("ngx_fine", int),
+                ScalarField("ngy_fine", int),
+                ScalarField("ngz_fine", int),
+            ]
+        ),
+        ChargeDensityField(),
+    ),
+    "E_FERMI": (ScalarField("fermi_energy_second_spin", float),),
+    "FORCES": (ArrayField("forces", float, (3, "max_ions_in_species", "num_species")),),
+    "STRESS": (ArrayField("stress", float, (6,)),),
+    "FORCE_CON": (
+        ArrayField("phonon_supercell_matrix", int, (3, 3)),
+        ArrayField(
+            "phonon_force_constant_matrix",
+            float,
+            (3, "num_ions", 3, "num_ions", "num_cells"),
+        ),
+        ArrayField("phonon_supercell_origins", int, (3, "num_cells")),
+        ScalarField("phonon_force_constant_row", int),
+    ),
+    "BORN_CHGS": (ArrayField("born_charges", float, (3, 3, "num_ions")),),
+}
+
+# Specifications for the check file, the only difference is the additional wavefunction
+# data taht is between the "nspins" and the "EigenValueAndOccCompositeField"
+CASTEP_CHECK_FIELD_SPEC = {
+    **CASTEP_BIN_FIELD_SPEC,
+    "END_CELL_GLOBAL_01": (
+        BoolField(
+            "found_ground_state_wavefunction"
+        ),  # Fortran logical saved as integer....
         BoolField("found_ground_state_density"),
-        CompositeField([
-            ScalarField("ngx_fine", int),
-            ScalarField("ngy_fine", int),
-            ScalarField("ngz_fine", int)
-        ]),
+        ScalarField("total_energy", float),
+        ScalarField("fermi_energy", float),
+        CompositeField([ScalarField("nbands", int), ScalarField("nspins", int)]),
+        # Read the wave function
+        StrField("wave_header", "a4"),
+        CompositeField(
+            [
+                ScalarField("ngx", int),
+                ScalarField("ngy", int),
+                ScalarField("ngz", int),
+            ]
+        ),
+        # Here starts the wavefunction relaxed data
+        CompositeField(
+            [
+                ScalarField("wave_coeff_size_1", int),
+                ScalarField("wave_spinorcomps", int),
+                ScalarField("wave_nbands_max", int),
+                ScalarField("wave_nkpts", int),
+                ScalarField("wave_nspins", int),
+            ]
+        ),
+        WaveFunctionField(),
+        EigenValueAndOccCompositeField(),  # Read the eigenvalues note that the arrays are reshaped
+        BoolField("found_ground_state_density"),
+        CompositeField(
+            [
+                ScalarField("ngx_fine", int),
+                ScalarField("ngy_fine", int),
+                ScalarField("ngz_fine", int),
+            ]
+        ),
         ChargeDensityField(),
     ),
-    "E_FERMI": (ScalarField("fermi_energy_second_spin", float), ),
-    "FORCES": (ArrayField("forces", float,
-                          (3, "max_ions_in_species", "num_species")), ),
-    "FORCE_CON": (ArrayField("phonon_supercell_matrix", int, (3, 3)),
-                  ArrayField("phonon_force_constant_matrix", float,
-                             (3, "num_ions", 3, "num_ions", "num_cells")),
-                  ArrayField("phonon_supercell_origins", int,
-                             (3, "num_cells")),
-                  ScalarField("phonon_force_constant_row", int)),
-    "BORN_CHGS": (ArrayField("born_charges", float, (3, 3, "num_ions")), ),
 }
 
 # Shape of each field
 CASTEP_BIN_FIELD_SHAPES = {
     field.name: field.shape
-    for tag in CASTEP_BIN_FIELD_SPEC for field in CASTEP_BIN_FIELD_SPEC[tag]
+    for value in CASTEP_BIN_FIELD_SPEC.values()
+    for field in value
     if isinstance(field, ArrayField)
 }
 
-# CASTEP_BIN_HEADERS = {
-#     "CELL%NUM_IONS": {
-#         "num_ions": (">i4", (1, ))
-#     },
-#     "CELL%MAX_IONS_IN_SPECIES": {
-#         "max_ions_in_species": (">i4", (1, ))
-#     },
-#     "CELL%REAL_LATTICE": {
-#         "real_lattice": (">f8", (3, 3))
-#     },
-#     "CELL%RECIP_LATTICE": {
-#         "recip_lattice": (">f8", (3, 3))
-#     },
-#     "CELL%NUM_SPECIES": {
-#         "num_species": (">i4", (1, ))
-#     },
-#     "CELL%NUM_IONS_IN_SPECIES": {
-#         "num_ions_in_species": (">i4", ("num_species", ))
-#     },
-#     "CELL%IONIC_POSITIONS": {
-#         "ionic_positions": (">f8", (3, "max_ions_in_species", "num_species"))
-#     },
-#     "CELL%SPECIES_SYMBOL": {
-#         "species_symbol": (">a8", ("num_species", ))
-#     },
-#     "FORCES": {
-#         "forces": (">f8", (3, "max_ions_in_species", "num_species"))
-#     },
-#     "FORCE_CON": {
-#         "phonon_supercell_matrix": (">i4", (3, 3)),
-#         "phonon_force_constant_matrix":
-#         (">f8", (3, "num_ions", 3, "num_ions", "num_cells")),
-#         "phonon_supercell_origins": (">i4", (3, "num_cells")),
-#         "phonon_force_constant_row": (">i4", (1, )),
-#     },
-#     "BORN_CHGS": {
-#         "born_charges": (">f8", (3, 3, "num_ions")),
-#     },
-# }
-
-# CASTEP_BIN_HEADERS_UNPACKED = {
-#     k: v
-#     for header in CASTEP_BIN_HEADERS
-#     for k, v in CASTEP_BIN_HEADERS[header].items()
-# }
-
-
-def read_castep_bin(filename: Union[str, Path] = None,
-                    fileobj=None,
-                    records_to_extract: Optional[Collection[str]] = None
-                    ) -> Dict[str, Any]:
+
+def read_castep_bin(
+    filename: Union[str, Path] = None,
+    fileobj=None,
+    records_to_extract: Optional[Collection[str]] = None,
+    spec=None,
+) -> Dict[str, Any]:
     """
     Read a castep_bin file for a given CASTEP run.
 
     Fortran binary files consist of records, one for each Fortran `write`
     statement used to create the file. Each record is surrounded by
     a *record marker* that encodes the length of the record in bytes.
 
@@ -466,135 +569,68 @@
         <length of string header>
         <string header>
         <length of string header>
         <length of binary data in bytes (record marker)>
         <binary data>
         <length of binary data in bytes (record marker)>
 
-    Args:
-        filename: path of the file to be read
-        fileobj: An file-like object from which the data needs to be read
-        records_to_extract: A collection of CASTEP bin headers. If `None`,
-            extract all headers for which there is a defined shape specification
-            in `CASTEP_BIN_HEADERS`.
-
-    Returns:
-        A dictionary following the CASTEP header hierarchy found within
-        the castep_bin file, containing the decoded data.
+    :param filename: path of the file to be read
+    :param fileobj: An file-like object from which the data needs to be read
+    :param records_to_extract: A collection of CASTEP bin headers. If `None`,
+        all headers for which there is a defined shape specification in `CASTEP_BIN_HEADERS`.
 
+    :returns: A dictionary following the CASTEP header hierarchy found within
+    the castep_bin file, containing the decoded data.
     """
 
-    if filename is not None:
-        f = open(filename, mode='rb')
-    else:
-        f = fileobj
-
-    header_offset_map = _generate_header_offset_map(f)
-    f.seek(0)
-
-    castep_data = {}
+    def _read_handle(f):
+        is_check, header_offset_map = _generate_header_offset_map(f)
+        f.seek(0)
+
+        castep_data = {}
+        if spec is None:
+            _spec = CASTEP_CHECK_FIELD_SPEC if is_check else CASTEP_BIN_FIELD_SPEC
+        for header, field in _spec.items():
+
+            if (
+                records_to_extract
+                and header not in records_to_extract
+                and not header.startswith("CELL%")
+            ):
+                continue
 
-    for header in CASTEP_BIN_FIELD_SPEC:
+            if header not in header_offset_map:
+                if records_to_extract and header in records_to_extract:
+                    raise RuntimeError(
+                        f"Unable to find desired header {header} in file."
+                    )
+                continue
 
-        if records_to_extract and header not in records_to_extract and not header.startswith(
-                "CELL%"):
-            continue
-
-        if header not in header_offset_map:
-            if records_to_extract and header in records_to_extract:
-                raise RuntimeError(
-                    f"Unable to find desired header {header} in file.")
-            continue
-
-        castep_data.update(
-            _decode_records(
-                f,
-                CASTEP_BIN_FIELD_SPEC[header],
-                header_offset_map[header],
-                castep_data,
-            ))
+            castep_data.update(
+                _decode_records(
+                    f,
+                    field,
+                    header_offset_map[header],
+                    castep_data,
+                )
+            )
+        return castep_data
 
     if filename is not None:
-        f.close()
-
-    return castep_data
+        with open(filename, mode="rb") as fhandle:
+            return _read_handle(fhandle)
 
-
-# def _reshape_arrays(castep_data: Dict[str, Any],
-#                     _requires: Optional[dict] = None) -> None:
-#     """Recursively solve for unknown dimensions across arrays, reshaping
-#     them along the way.
-
-#     Procedure will fail if any iteration starts with every un-reshaped field
-#     possessing multiple unknown dimensions.
-
-#     Unknown dimensions that are repeated (e.g., square matrix) will be solved.
-
-#     Args:
-#         castep_data: The dictionary of decoded but un-reshaped data, with keys
-#             from `CASTEP_BIN_FIELD_SHAPES`.
-#         _requires: Cache of remaining unknowns used for recursion.
-
-#     """
-#     if _requires is None:
-#         _requires = {}
-#     resolved_unknowns = {}
-#     for field in castep_data:
-#         if isinstance(castep_data[field], np.ndarray) and len(
-#                 castep_data[field].shape) == 1:
-#             shape = [
-#                 castep_data.get(s) or s for s in CASTEP_BIN_FIELD_SHAPES[field]
-#             ]
-#             _requires[field] = [s for s in shape if isinstance(s, str)]
-
-#             if len(set(_requires[field])) == 1:
-#                 # Attempt to resolve a single missing unknown.
-#                 # This unknown can appear in multiple dimensions of the same field.
-#                 unknown = _requires[field][0]
-#                 n = int(
-#                     np.round(
-#                         (castep_data[field].shape[0] //
-#                          np.prod([s for s in shape if s != unknown]))**1. /
-#                         len(_requires[field])))
-#                 castep_data[field] = np.reshape(
-#                     castep_data[field],
-#                     [n if isinstance(v, str) else v for v in shape],
-#                     order="F")
-#                 resolved_unknowns[unknown] = castep_data[field].shape[
-#                     shape.index(unknown)]
-#                 _requires.pop(field)
-
-#             elif not _requires[field]:
-#                 # Shape should now be fully-specified
-#                 castep_data[field] = np.reshape(castep_data[field],
-#                                                 shape,
-#                                                 order="F")
-#                 _requires.pop(field)
-
-#     castep_data.update(resolved_unknowns)
-#     for field in _requires:
-#         _requires[field] = [
-#             s for s in
-#             [castep_data.get(s) or s for s in CASTEP_BIN_FIELD_SHAPES[field]]
-#             if isinstance(s, str)
-#         ]
-#     # If all remaining fields have more than 1 unknown, give up
-#     if _requires and all(
-#             len(set(_requires[field])) > 1 for field in _requires):  # pylint: disable=bad-continuation
-#         raise RuntimeError(f"Too many unknowns to resolve: {_requires}")
-
-#     while _requires:
-#         _reshape_arrays(castep_data, _requires)
+    return _read_handle(fileobj)
 
 
 def _decode_records(
-        fp: io.BufferedReader,
-        record_specs: Tuple[FieldType],
-        offset: int,
-        decoded_data: dict = None,
+    fp: io.BufferedReader,
+    record_specs: Tuple[FieldType],
+    offset: int,
+    decoded_data: dict = None,
 ) -> Dict[str, Any]:
     """For a given file buffer, header name and byte offset, read
     the expected number of file records and decode them according to
     the type and shape specification provided in `CASTEP_BIN_HEADERS`.
 
     Note:
         The file buffer will not be reset to its initial position.
@@ -630,46 +666,61 @@
             record_data, _ = _read_record(fp)
             for subspec in record_spec.fields:
                 offset = int(subspec.type_string[-1])
                 if isinstance(subspec, ArrayField):
                     offset *= np.prod(subspec.resolve_shape(decoded_data)[0])
                 assert offset > 0
                 decoded_data[subspec.name] = subspec.decode(
-                    fp, decoded_data, record_data=record_data)
+                    fp, decoded_data, record_data=record_data
+                )
                 record_data = record_data[offset:]
         elif isinstance(record_spec, StructuredField):
             record_spec.decode(fp, decoded_data)
 
     return decoded_data
 
 
-def _generate_header_offset_map(fileobj) -> Dict[str, int]:
-    """Scans a castep_bin file for recognisable headers, creating a
+def _decode_composite(fp, record_spec):
+    """Decode a composite field return the decoded data"""
+    record_data, _ = _read_record(fp)
+    decoded = []
+    for subspec in record_spec.fields:
+        offset = int(subspec.type_string[-1])
+        if isinstance(subspec, ArrayField):
+            offset *= np.prod(subspec.shape)
+        assert offset > 0
+        decoded.append(subspec.decode(fp, {}, record_data=record_data))
+        record_data = record_data[offset:]
+    return decoded
+
+
+def _generate_header_offset_map(fileobj) -> Tuple[bool, Dict[str, int]]:
+    """
+    Scans a castep_bin/check file for recognisable headers, creating a
     dictionary of their byte-offsets within the file. The stored
     offset corresponds to the start of the record immediately
     following the CASTEP header.
 
-    Args:
-        filename: The file to read.
-
-    Returns:
-        A dictionary of headers mapped to the offsets of the following
-        record.
+    :param fileobj: A file object from which the data should be read.
 
+    :returns: Tuple of (is_check, offset_map), where the latter is a dictionary of
+    headers mapped to the offsets of the following record.
     """
     header_offset_map: Dict[str, int] = {}
 
     f = fileobj
+    loc = f.tell()
 
     # Check first header is "CASTEP_BIN"
     header, _ = _read_record(f)
     header = header.decode("utf-8").strip("'")
+    is_check = False
     if header != "CASTEP_BIN":
-        raise RuntimeError(
-            f"File handler does not start with 'CASTEP_BIN' header.")
+        is_check = True
+        f.seek(loc)
 
     data = None
     while data != "END":
         data, _ = _read_record(f, seek_only=True)
         try:
             data = data.decode("utf-8").strip("'").strip()
             # Strip any non-alpha fields
@@ -680,34 +731,34 @@
                 if data in header_offset_map:
                     data = _find_header_suffix(data, header_offset_map)
 
                 header_offset_map[data] = f.tell()
         except (AttributeError, UnicodeDecodeError):
             pass
 
-    return header_offset_map
+    return is_check, header_offset_map
 
 
 def _find_header_suffix(name, header_offset_map):
     """Found a suitable suffix the a given header name with number suffix"""
     counter = 1
     for key in header_offset_map.keys():
         match = re.match(f"{name}_(\\d+)", key)
         if match:
             num = int(match.group(1))
             if num >= counter:
                 counter = num + 1
-    return f'{name}_{counter:02d}'
+    return f"{name}_{counter:02d}"
 
 
 def _read_record(
-        f: io.BufferedReader,
-        seek_only: bool = False,
-        record_marker_size: int = 4,
-        read_data_smaller_than=512,
+    f: io.BufferedReader,
+    seek_only: bool = False,
+    record_marker_size: int = 4,
+    read_data_smaller_than=512,
 ) -> Tuple[Optional[bytes], int]:
     """Reads the preceeding record marker for the next record in the
     file, decodes the record data, then reads the suffix record marker,
     eventually returning the decoded record data.
 
     Args:
         f: The open binary file stream in the buffer.
@@ -736,16 +787,17 @@
         raise RuntimeError(
             f"The start ({marker}) and end ({marker_end}) record markers were inconsistent."
         )
 
     return data, marker
 
 
-def _read_marker(f: Union[io.BufferedReader, bytes],
-                 record_marker_size: int = 4) -> int:
+def _read_marker(
+    f: Union[io.BufferedReader, bytes], record_marker_size: int = 4
+) -> int:
     """Read the next *n* bytes from the buffer and try to interpret them
     as a Fortran record marker (typically uint4, but can depend on
     compiler).
 
     Args:
         f: An open file buffer.
         record_marker_size: The number of bytes to read as a record marker.
```

### Comparing `castepxbin-0.2.0/castepxbin/ome_bin.py` & `castepxbin-0.3.0/castepxbin/ome_bin.py`

 * *Files identical despite different names*

### Comparing `castepxbin-0.2.0/castepxbin/pdos.py` & `castepxbin-0.3.0/castepxbin/pdos.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 """
 Reader module for CASTEP pdos_bin
 
 Written based on the example `pdos_bin.f90` file in open-source OptaDos code
 """
 from enum import Enum, unique
+from typing import Any, BinaryIO, Dict, Union
+
 import numpy as np
 from scipy.io import FortranFile
 
-__all__ = ["read_pdos_bin", "compute_pdos"]
+__all__ = ["read_pdos_bin", "compute_pdos", "reorder_pdos_data"]
 
 # pylint: disable=import-outside-toplevel, too-many-locals, too-many-branches
 
 
 @unique
 class SpinEnum(Enum):
     """
     Enum type for Spin.  Only up and down.
     Usage: Spin.up, Spin.down.
     """
+
     up, down = (1, -1)
 
     def __int__(self):
         return self.value
 
     def __float__(self):
         return float(self.value)
@@ -66,162 +69,176 @@
     f_zzz = "Fzzz"
     f_xyz = "Fxyz"
     f_z_xx_yy = "Fz(xx-yy)"
     f_y_zz_xx = "Fy(zz-xx)"
     f_x_yy_zz = "Fx(yy-zz)"
 
     def __int__(self):
+        """Instantiate"""
         return self.value
 
     def __str__(self):
         return str(self.name)
 
     @property
-    def orbital_type(self):
+    def orbital_type(self) -> OrbitalType:
         """
         Returns OrbitalType of an orbital.
         """
         return OrbitalType[self.name[0]]  # pylint: disable=unsubscriptable-object
 
 
-def read_pdos_bin(filename, endian='big'):
+def read_pdos_bin(filename: Union[str, BinaryIO], endian="big") -> Dict[str, Any]:
     """
     Read the pdos_bin file generated by CASTEP Spectral task.
 
     Args:
         filename (str): name of the file to be read
 
     Returns:
         A dictionary of the data that have been read.
         the weights of each orbital in stored in the 'pdos_weights' array
         with dimension (n_orbital, n_max_eign, n_kpoints, n_spin)
     """
-    esymbol = '>' if endian.upper() == 'BIG' else '>'
-    dint = np.dtype(esymbol + 'i4')
-    ddouble = np.dtype(esymbol + 'f8')
-    dch80 = np.dtype(esymbol + 'a80')
-    diarray = lambda x: '{}({},)i4'.format(esymbol, x)
+    esymbol = ">" if endian.upper() == "BIG" else ">"
+    dint = np.dtype(esymbol + "i4")
+    ddouble = np.dtype(esymbol + "f8")
+    dch80 = np.dtype(esymbol + "a80")
+    diarray = lambda x: f"{esymbol}({x},)i4"
 
-    with FortranFile(filename, header_dtype=np.dtype('>u4')) as fhandle:
+    with FortranFile(filename, header_dtype=np.dtype(">u4")) as fhandle:
         fversion = fhandle.read_record(ddouble)[0]
         fheader = fhandle.read_record(dch80)[0].decode()
         num_kpoints = fhandle.read_record(dint)[0]
         num_spins = fhandle.read_record(dint)[0]
         num_popn_orb = fhandle.read_record(dint)[0]
         max_eignenv = fhandle.read_record(dint)[0]
 
         # Now we start to read more data
         species = fhandle.read_record(diarray(num_popn_orb))
         ion = fhandle.read_record(diarray(num_popn_orb))
         am_channel = fhandle.read_record(diarray(num_popn_orb))
 
         # Now we initialize the storage space for the weights
         pdos_weights = np.zeros(
-            (num_popn_orb, max_eignenv, num_kpoints, num_spins), dtype=float)
+            (num_popn_orb, max_eignenv, num_kpoints, num_spins), dtype=float
+        )
 
         kpoint_positions = np.zeros((num_kpoints, 3), dtype=float)
         num_eigenvalues = np.zeros(num_spins, dtype=int)
         # Now we start to read the actual data
         for nk in range(num_kpoints):
-            _, kpoint_positions[nk, :] = fhandle.read_record('>i4', '>(3,)f8')
+            _, kpoint_positions[nk, :] = fhandle.read_record(">i4", ">(3,)f8")
             for ns in range(num_spins):
                 _ = fhandle.read_record(dint)
                 num_eigenvalues[ns] = fhandle.read_record(dint)
                 for nb in range(num_eigenvalues[ns]):
                     pdos_weights[:, nb, nk, ns] = fhandle.read_record(
-                        '>({},)f8'.format(num_popn_orb))
+                        f">({num_popn_orb},)f8"
+                    )
 
     output = {
-        'fversion': fversion,
-        'fheader': fheader,
-        'num_kpoints': num_kpoints,
-        'num_spins': num_spins,
-        'num_popn_orb': num_popn_orb,
-        'max_eigenenv': max_eignenv,
-        'species': species,
-        'ion': ion,
-        'am_channel': am_channel,
-        'pdos_weights': pdos_weights,
-        'kpoints_positions': kpoint_positions,
-        'num_eigenvalues': num_eigenvalues,
+        "fversion": fversion,
+        "fheader": fheader,
+        "num_kpoints": num_kpoints,
+        "num_spins": num_spins,
+        "num_popn_orb": num_popn_orb,
+        "max_eigenenv": max_eignenv,
+        "species": species,
+        "ion": ion,
+        "am_channel": am_channel,
+        "pdos_weights": pdos_weights,
+        "kpoints_positions": kpoint_positions,
+        "num_eigenvalues": num_eigenvalues,
     }
     return output
 
 
-def reorder_pdos_data(input_items,
-                      pymatgen_labels=True,
-                      use_string_as_keys=False):
+def reorder_pdos_data(
+    input_items: Dict[str, Any],
+    pymatgen_labels: bool = True,
+    use_string_as_keys: bool = False,
+) -> dict:
     """
     Arrange the PDOS weights so it is more meaningful
 
     The result can be used to compute PDOS for creating CompleteDos object
-    that can be used for Pymatgen
+    that can be used for pymatgen.
 
-    Args:
-        input_items (dict): A dictionary of the pdos information, use the
+    :param input_items: A dictionary of the pdos information, use the
         output of  `read_pdos` function.
-        pymatgen_labels (bool): Use pymatgen Enum as the keys of the result dictionary.
-
+    :param pymatgen_labels: Use pymatgen Enum as the keys of the result dictionary.
 
-    Returns:
-        A dictionary of {Site_index: {Orbital: {Spin: weight}}}
+    :returns: A dictionary of `{Site_index: {Orbital: {Spin: weight}}}`.
     """
 
     _ = use_string_as_keys
     if pymatgen_labels is True:
         try:
-            from pymatgen.electronic_structure.core import Orbital as POrbital
+            from pymatgen.electronic_structure.core import (
+                Orbital as POrbital,
+            )
             from pymatgen.electronic_structure.core import Spin as PSpin
         except ImportError:
             pymatgen_labels = False
 
     if pymatgen_labels:
         # Note that s-p labels are inferreed from dot castep output
         # f labels - I know the first three is among the first three.
         # There is no way to tell if they are correct, f_1 is not very informative from VASP....
-        orbital_mapping = [[POrbital.s],
-                           [POrbital.px, POrbital.py, POrbital.pz],
-                           [
-                               POrbital.dz2, POrbital.dyz, POrbital.dxz,
-                               POrbital.dx2, POrbital.dxy
-                           ],
-                           [
-                               POrbital.f_1, POrbital.f_2, POrbital.f_3,
-                               POrbital.f0, POrbital.f1, POrbital.f2,
-                               POrbital.f3
-                           ]]
+        orbital_mapping = [
+            [POrbital.s],
+            [POrbital.px, POrbital.py, POrbital.pz],
+            [POrbital.dz2, POrbital.dyz, POrbital.dxz, POrbital.dx2, POrbital.dxy],
+            [
+                POrbital.f_1,
+                POrbital.f_2,
+                POrbital.f_3,
+                POrbital.f0,
+                POrbital.f1,
+                POrbital.f2,
+                POrbital.f3,
+            ],
+        ]
         Spin = PSpin
     else:
         # These are the orders inferred from CASTEP output
-        orbital_mapping = [[OrbitalEnum.s],
-                           [OrbitalEnum.px, OrbitalEnum.py, OrbitalEnum.pz],
-                           [
-                               OrbitalEnum.dz2, OrbitalEnum.dyz,
-                               OrbitalEnum.dxz, OrbitalEnum.dx2,
-                               OrbitalEnum.dxy
-                           ],
-                           [
-                               OrbitalEnum.f_xxx, OrbitalEnum.f_yyy,
-                               OrbitalEnum.f_zzz, OrbitalEnum.f_xyz,
-                               OrbitalEnum.f_z_xx_yy, OrbitalEnum.f_y_zz_xx,
-                               OrbitalEnum.f_x_yy_zz
-                           ]]
+        orbital_mapping = [
+            [OrbitalEnum.s],
+            [OrbitalEnum.px, OrbitalEnum.py, OrbitalEnum.pz],
+            [
+                OrbitalEnum.dz2,
+                OrbitalEnum.dyz,
+                OrbitalEnum.dxz,
+                OrbitalEnum.dx2,
+                OrbitalEnum.dxy,
+            ],
+            [
+                OrbitalEnum.f_xxx,
+                OrbitalEnum.f_yyy,
+                OrbitalEnum.f_zzz,
+                OrbitalEnum.f_xyz,
+                OrbitalEnum.f_z_xx_yy,
+                OrbitalEnum.f_y_zz_xx,
+                OrbitalEnum.f_x_yy_zz,
+            ],
+        ]
         Spin = SpinEnum
 
     # We take average of each kpoints from here
     # One might task why not take account the kpoints weight?
     # because it should be taken account of in the TDOS
-    weights = input_items['pdos_weights']
+    weights = input_items["pdos_weights"]
     # Specie index for all orbitals
-    species = input_items['species']
+    species = input_items["species"]
     # Index of each ion for all orbitals
-    ion = input_items['ion']
-    num_spins = input_items['num_spins']
+    ion = input_items["ion"]
+    num_spins = input_items["num_spins"]
     # Angular momentum channel all orbitals
-    am_channel = input_items['am_channel']
+    am_channel = input_items["am_channel"]
 
     unique_speices = np.unique(species)
     unique_speices.sort()
     site_index = 0
     output_data = {}
     # Initialise storage space
     for specie in unique_speices:  # pylint: disable=too-many-nested-blocks
@@ -252,56 +269,63 @@
                     else:
                         orb_dict[Spin.up] = weights[iloc, :, :, 0]
 
                     # Now we have the orb_dict populated
                     # Combined the weights if this orbital has been seen...
                     if this_orb in site_dict:
                         site_dict[this_orb] = _merge_weights(
-                            site_dict[this_orb], orb_dict)
+                            site_dict[this_orb], orb_dict
+                        )
                     else:
                         site_dict[this_orb] = orb_dict
             # Now we populated site_dict add it to output_data
             output_data[site_index] = site_dict
             site_index += 1
 
     return output_data
 
 
-def compute_pdos(pdos_bin, eigenvalues, kpoints_weights, bins):
+def compute_pdos(
+    pdos_bin: str,
+    eigenvalues: Dict[SpinEnum, np.ndarray],
+    kpoints_weights: np.ndarray,
+    bins: np.ndarray,
+) -> Dict[str, Any]:
     """
     Compute the PDOS from eigenvalue and kpoint weights
 
-    Args:
-        pdos_bin (str): Path to the binary pdos_bin file
-        eigenvealues (str): Eigenvalue as {Spin: array_)}.
-        kpoints_weights (np.ndarray): Weights of each kpoints.
-        bins: The bins for computing the density of states.
+    :param pdos_bin: Path to the binary pdos_bin file
+    :param eigenvalues: Eigenvalue as {Spin: array_)}.
+    :param kpoints_weights: Weights of each kpoints.
+    :param bins: The bins for computing the density of states.
+
+    :returns: A dictionary containing the calculated un-broadened PDOS in the bins.
     """
 
     # Walk through the ordred_weights dictionary and compute PDOS for each weight
     ordered_weights = reorder_pdos_data(read_pdos_bin(pdos_bin))
     pdos_data = {}
     for site, porbs_dict in ordered_weights.items():
         porbs_outdict = {}
         for orb, pspin_dict in porbs_dict.items():
             pdos_orbit = {
                 spin: np.histogram(
                     eigenvalue_set,
                     bins=bins,
-                    weights=kpoints_weights * pspin_dict[
-                        spin]  # weight (nk, ); pspin_dict[spin] (nk, nb)
+                    weights=kpoints_weights
+                    * pspin_dict[spin],  # weight (nk, ); pspin_dict[spin] (nk, nb)
                 )[0]
                 for spin, eigenvalue_set in eigenvalues.items()
             }
             porbs_outdict[orb] = pdos_orbit
         pdos_data[site] = porbs_outdict
     return pdos_data
 
 
-def _merge_weights(spin_d1, spin_d2):
+def _merge_weights(spin_d1: dict, spin_d2: dict) -> dict:
     """Sum the weights stored in two dictionaries with keys being the spins"""
     if len(spin_d1) != len(spin_d2):
         raise RuntimeError("Critical - mismatch spin-dict length")
     out = {}
     for spin in spin_d1:
         out[spin] = spin_d1[spin] + spin_d2[spin]
     return out
```

### Comparing `castepxbin-0.2.0/castepxbin/test_reader.py` & `castepxbin-0.3.0/tests/test_reader.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,128 +1,193 @@
 """
 Test the reader
 """
 import os
-import pytest
+
 import numpy as np
+import pytest
 import scipy.constants
 
-from .pdos import read_pdos_bin, reorder_pdos_data, OrbitalEnum, SpinEnum
-from .ome_bin import read_dome_bin, read_ome_bin, read_cst_ome
-from .castep_bin import read_castep_bin
+from castepxbin.castep_bin import read_castep_bin
+from castepxbin.ome_bin import read_cst_ome, read_dome_bin, read_ome_bin
+from castepxbin.pdos import (
+    OrbitalEnum,
+    SpinEnum,
+    read_pdos_bin,
+    reorder_pdos_data,
+)
+from castepxbin.wave import coeff_to_recip, coords_to_indices
 
 
 @pytest.fixture
 def pdos_bin():
-    return os.path.join(os.path.split(__file__)[0], 'test_data/Si2.pdos_bin')
+    return os.path.join(os.path.split(__file__)[0], "test_data/Si2.pdos_bin")
 
 
 @pytest.fixture
 def ome_bin():
-    return os.path.join(os.path.split(__file__)[0], 'test_data/Si2.ome_bin')
+    return os.path.join(os.path.split(__file__)[0], "test_data/Si2.ome_bin")
 
 
 @pytest.fixture
 def cst_ome():
-    return os.path.join(os.path.split(__file__)[0], 'test_data/Si2.cst_ome')
+    return os.path.join(os.path.split(__file__)[0], "test_data/Si2.cst_ome")
 
 
 @pytest.fixture
 def dome_bin():
-    return os.path.join(os.path.split(__file__)[0], 'test_data/Si2.dome_bin')
+    return os.path.join(os.path.split(__file__)[0], "test_data/Si2.dome_bin")
 
 
 @pytest.fixture
 def bands_file():
-    return os.path.join(os.path.split(__file__)[0], 'test_data/Si2.bands')
+    return os.path.join(os.path.split(__file__)[0], "test_data/Si2.bands")
 
 
 @pytest.fixture
 def castep_bin_Si():
     """.castep_bin test file taken from Euphonic:
     https://github.com/pace-neutrons/Euphonic/blob/v0.6.2/tests_and_analysis/test/data/castep_files/Si2-sc-skew/Si2-sc-skew.castep_bin
     """
-    return os.path.join(
-        os.path.split(__file__)[0], 'test_data/Si2-sc-skew.castep_bin')
+    return os.path.join(os.path.split(__file__)[0], "test_data/Si2-sc-skew.castep_bin")
+
+
+@pytest.fixture
+def castep_check_Si():
+    """.check test file taken from Euphonic:
+    https://github.com/pace-neutrons/Euphonic/blob/v0.6.2/tests_and_analysis/test/data/castep_files/Si2-sc-skew/Si2-sc-skew.castep_bin
+    """
+    return os.path.join(os.path.split(__file__)[0], "test_data/Si2.check")
 
 
 @pytest.fixture
 def castep_bin_SiO2():
-    """Binary output from a singlepoint with `calculate_stress: true`. """
-    return os.path.join(
-        os.path.split(__file__)[0], 'test_data/SiO2.castep_bin')
+    """Binary output from a singlepoint with `calculate_stress: true`."""
+    return os.path.join(os.path.split(__file__)[0], "test_data/SiO2.castep_bin")
 
 
 def test_pdos_reader(pdos_bin):
     """Test the reader for pdos_bin"""
     output = read_pdos_bin(pdos_bin)
-    assert output['pdos_weights'].shape == (8, 23, 110, 1)
+    assert output["pdos_weights"].shape == (8, 23, 110, 1)
 
 
 def test_pdos_reorder(pdos_bin):
     """Test reordering of the PDOS"""
     try:
-        from pymatgen.electronic_structure.core import Orbital as POrbital
+        from pymatgen.electronic_structure.core import (
+            Orbital as POrbital,
+        )
         from pymatgen.electronic_structure.core import Spin as PSpin
     except ImportError:
         pass
     else:
         raw_output = read_pdos_bin(pdos_bin)
         reordered = reorder_pdos_data(raw_output)
         assert reordered[0][POrbital.s][PSpin.up].shape == (23, 110)
 
     raw_output = read_pdos_bin(pdos_bin)
     reordered = reorder_pdos_data(raw_output, pymatgen_labels=False)
     assert reordered[0][OrbitalEnum.s][SpinEnum.up].shape == (23, 110)
 
 
+def test_castep_check_reader(castep_check_Si):
+
+    data = read_castep_bin(castep_check_Si)
+    assert "wavefunction" in data
+    wfc = data["wavefunction"]
+    assert "ngx" in wfc
+    assert "pw_grid_coords" in wfc
+    assert "coeffs" in wfc
+    assert "kpts" in wfc
+    assert "nwaves_at_kp" in wfc
+    mesh_size = np.array([wfc["ngx"], wfc["ngy"], wfc["ngz"]])
+    idx = coords_to_indices(wfc["pw_grid_coords"], mesh_size)
+    assert idx.min() == 0
+    assert idx.max() == mesh_size.max() - 1
+    grid = coeff_to_recip(
+        wfc["coeffs"], wfc["nwaves_at_kp"], wfc["pw_grid_coords"], *mesh_size
+    )
+
+    from castepxbin.wave import WaveFunction
+
+    wf = WaveFunction.from_dict(data)
+    mesh = wf.get_reciprocal_grid()
+    assert all(mesh.shape[:3] == wf.mesh_size)
+
+    assert wf.get_plane_wave_coeffs().size > 0
+    assert (
+        wf.get_plane_wave_coeffs(
+            ik=wf.nkpts - 1, ib=wf.nbands - 1, ispin=wf.nspins - 1
+        ).size
+        > 0
+    )
+    assert wf.get_gvectors().size > 0
+    assert wf.get_gvectors(ik=wf.nkpts - 1).size > 0
+    assert wf.get_gmesh_index().size > 0
+    assert wf.get_gmesh_index(ik=wf.nkpts - 1).size > 0
+    assert isinstance(wf.get_kpoints_cart(), np.ndarray)
+
+
 def test_castep_bin_reader(castep_bin_Si, castep_bin_SiO2):
     if not os.path.isfile(castep_bin_Si):
         pytest.skip(".castep_bin test data is missing")
     data = read_castep_bin(castep_bin_Si)
-    expected_fields = ("num_ions", "num_cells", "num_species",
-                       "max_ions_in_species", "forces",
-                       "phonon_supercell_matrix",
-                       "phonon_force_constant_matrix",
-                       "phonon_supercell_origins", "phonon_force_constant_row")
+    expected_fields = (
+        "num_ions",
+        "num_cells",
+        "num_species",
+        "max_ions_in_species",
+        "forces",
+        "phonon_supercell_matrix",
+        "phonon_force_constant_matrix",
+        "phonon_supercell_origins",
+        "phonon_force_constant_row",
+    )
     assert all(field in data for field in expected_fields)
-    assert data["forces"].shape == (3, data["max_ions_in_species"],
-                                    data["num_species"])
-    assert data["phonon_force_constant_matrix"].shape == (3, data["num_ions"],
-                                                          3, data["num_ions"],
-                                                          data["num_cells"])
+    assert data["forces"].shape == (3, data["max_ions_in_species"], data["num_species"])
+    assert data["phonon_force_constant_matrix"].shape == (
+        3,
+        data["num_ions"],
+        3,
+        data["num_ions"],
+        data["num_cells"],
+    )
 
     # Check that the same parsing works even if cell info is missing (e.g., test recursive dimension solving)
-    data = read_castep_bin(castep_bin_Si,
-                           records_to_extract=("FORCES",
-                                               "CELL%MAX_IONS_IN_SPECIES_01"))
+    data = read_castep_bin(
+        castep_bin_Si, records_to_extract=("FORCES", "CELL%MAX_IONS_IN_SPECIES_01")
+    )
 
     expected_fields = (
         "num_species",
         "max_ions_in_species",
         "forces",
     )
     assert all(field in data for field in expected_fields)
-    assert data["forces"].shape == (3, data["max_ions_in_species"],
-                                    data["num_species"])
+    assert data["forces"].shape == (3, data["max_ions_in_species"], data["num_species"])
     # Check that indivdual blocks can resolve self-consistently
     # (the value of num_ions or num_cells are not read) from the castep_bin
     data = read_castep_bin(castep_bin_Si, records_to_extract=("FORCE_CON"))
 
     expected_fields = (
         "num_ions",
         "num_cells",
         "phonon_supercell_matrix",
         "phonon_force_constant_matrix",
         "phonon_supercell_origins",
     )
     assert all(field in data for field in expected_fields)
-    assert data["phonon_force_constant_matrix"].shape == (3, data["num_ions"],
-                                                          3, data["num_ions"],
-                                                          data["num_cells"])
+    assert data["phonon_force_constant_matrix"].shape == (
+        3,
+        data["num_ions"],
+        3,
+        data["num_ions"],
+        data["num_cells"],
+    )
 
     # Check forces are consistent with castep file with multiple species
     data = read_castep_bin(castep_bin_SiO2)
     assert "forces" in data
     assert data.get("found_ground_state_density") is True
     assert data.get("found_ground_state_wavefunction") is True
     assert data.get("total_energy") == pytest.approx(-77.0824329248417)
@@ -130,44 +195,68 @@
     assert data.get("nspins") == 2
     assert data.get("nkpts") == 14
     assert data.get("kpoints").shape == (3, 14)
     assert data.get("kpoints_of_eigenvalues").shape == (3, 14)
     assert data.get("eigenvalues").shape == (20, 14, 2)
     assert data.get("occupancies")[0, 0, 0] == 1.0
 
-    ev_per_ang_to_hartree_per_bohr = 1e10 * scipy.constants.physical_constants[
-        "Bohr radius"][0] / scipy.constants.physical_constants[
-            "Hartree energy in eV"][0]
-    expected_forces = np.array([
-        [0.00017, -0.40797, 0.00006], [0.40772, 0.00029, 0.00006],
-        [0.00017, 0.40765, -0.00018], [-0.40773, -0.00042, 0.00003],
-        [-0.00052, 0.00009, -0.00007], [0.00018, 0.00038, 0.00010]
-    ]) * ev_per_ang_to_hartree_per_bohr
+    ev_per_ang_to_hartree_per_bohr = (
+        1e10
+        * scipy.constants.physical_constants["Bohr radius"][0]
+        / scipy.constants.physical_constants["Hartree energy in eV"][0]
+    )
+    expected_forces = (
+        np.array(
+            [
+                [0.00017, -0.40797, 0.00006],
+                [0.40772, 0.00029, 0.00006],
+                [0.00017, 0.40765, -0.00018],
+                [-0.40773, -0.00042, 0.00003],
+                [-0.00052, 0.00009, -0.00007],
+                [0.00018, 0.00038, 0.00010],
+            ]
+        )
+        * ev_per_ang_to_hartree_per_bohr
+    )
 
     # Compare the arrays per species
-    np.testing.assert_array_almost_equal(expected_forces[0:4],
-                                         data["forces"][:, :, 0].T)
-    np.testing.assert_array_almost_equal(expected_forces[4:],
-                                         data["forces"][:, :, 1].T[:2, :])
+    np.testing.assert_array_almost_equal(
+        expected_forces[0:4], data["forces"][:, :, 0].T
+    )
+    np.testing.assert_array_almost_equal(
+        expected_forces[4:], data["forces"][:, :, 1].T[:2, :]
+    )
 
     # Test reading all fields
     fobj = open(castep_bin_SiO2, "rb")
     data = read_castep_bin(fileobj=fobj, records_to_extract=None)
-    expected_fields = ("num_ions", "real_lattice", "recip_lattice",
-                       "num_ions_in_species", "ionic_positions",
-                       "species_symbol", "num_species", "spin_density",
-                       "charge_density", "ngz_fine", "spin_treatment")
+    expected_fields = (
+        "num_ions",
+        "real_lattice",
+        "recip_lattice",
+        "num_ions_in_species",
+        "ionic_positions",
+        "species_symbol",
+        "num_species",
+        "spin_density",
+        "charge_density",
+        "ngz_fine",
+        "spin_treatment",
+    )
 
     for field in expected_fields:
         assert field in data
-    assert data['num_species'] == 2
-    assert data['ionic_positions'].shape == (3, data['max_ions_in_species'],
-                                             data['num_species'])
-    assert data['species_symbol'] == ['O', 'Si']
-    assert data['spin_treatment'] == 'SCALAR'
+    assert data["num_species"] == 2
+    assert data["ionic_positions"].shape == (
+        3,
+        data["max_ions_in_species"],
+        data["num_species"],
+    )
+    assert data["species_symbol"] == ["O", "Si"]
+    assert data["spin_treatment"] == "SCALAR"
     fobj.close()
 
 
 def test_ome_bin(ome_bin):
     """Test reading ome_bin file"""
     v, header, om = read_ome_bin(ome_bin, 23, 2, 1)
     assert "CASTEP" in header
```

