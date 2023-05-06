# Comparing `tmp/optical_dispersion_relations-0.1.1.tar.gz` & `tmp/optical_dispersion_relations-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/george/Documents/Projects/optical_dispersion_relations/dist/.tmp-z05hi6g7/optical_dispersion_relations-0.1.1.tar", last modified: Tue Nov 29 20:30:00 2022, max compression
+gzip compressed data, was "optical_dispersion_relations-0.2.0.tar", last modified: Sat May  6 20:34:05 2023, max compression
```

## Comparing `optical_dispersion_relations-0.1.1.tar` & `optical_dispersion_relations-0.2.0.tar`

### file list

```diff
@@ -1,24 +1,23 @@
-drwxr-xr-x   0 george     (501) staff       (20)        0 2022-11-29 20:30:00.641524 optical_dispersion_relations-0.1.1/
--rw-r--r--   0 george     (501) staff       (20)     1071 2022-11-29 19:55:02.000000 optical_dispersion_relations-0.1.1/LICENSE.txt
--rw-r--r--   0 george     (501) staff       (20)     1127 2022-11-29 20:30:00.641333 optical_dispersion_relations-0.1.1/PKG-INFO
--rw-r--r--   0 george     (501) staff       (20)      592 2022-11-29 19:55:02.000000 optical_dispersion_relations-0.1.1/README.md
--rw-r--r--   0 george     (501) staff       (20)      549 2022-11-29 20:29:27.000000 optical_dispersion_relations-0.1.1/pyproject.toml
--rw-r--r--   0 george     (501) staff       (20)       38 2022-11-29 20:30:00.641574 optical_dispersion_relations-0.1.1/setup.cfg
-drwxr-xr-x   0 george     (501) staff       (20)        0 2022-11-29 20:30:00.637277 optical_dispersion_relations-0.1.1/src/
-drwxr-xr-x   0 george     (501) staff       (20)        0 2022-11-29 20:30:00.639141 optical_dispersion_relations-0.1.1/src/optical_dispersion_relations/
--rw-r--r--   0 george     (501) staff       (20)        0 2022-11-19 19:16:36.000000 optical_dispersion_relations-0.1.1/src/optical_dispersion_relations/__init__.py
--rw-r--r--   0 george     (501) staff       (20)     4446 2022-11-29 20:29:27.000000 optical_dispersion_relations-0.1.1/src/optical_dispersion_relations/dielectric_waveguides.py
--rw-r--r--   0 george     (501) staff       (20)     3125 2022-11-29 19:55:02.000000 optical_dispersion_relations-0.1.1/src/optical_dispersion_relations/drude_lorentz.py
--rw-r--r--   0 george     (501) staff       (20)     3975 2022-11-29 19:55:02.000000 optical_dispersion_relations-0.1.1/src/optical_dispersion_relations/plasmon.py
--rw-r--r--   0 george     (501) staff       (20)     1109 2022-11-29 19:55:02.000000 optical_dispersion_relations-0.1.1/src/optical_dispersion_relations/utilities.py
-drwxr-xr-x   0 george     (501) staff       (20)        0 2022-11-29 20:30:00.640008 optical_dispersion_relations-0.1.1/src/optical_dispersion_relations.egg-info/
--rw-r--r--   0 george     (501) staff       (20)     1127 2022-11-29 20:30:00.000000 optical_dispersion_relations-0.1.1/src/optical_dispersion_relations.egg-info/PKG-INFO
--rw-r--r--   0 george     (501) staff       (20)      663 2022-11-29 20:30:00.000000 optical_dispersion_relations-0.1.1/src/optical_dispersion_relations.egg-info/SOURCES.txt
--rw-r--r--   0 george     (501) staff       (20)        1 2022-11-29 20:30:00.000000 optical_dispersion_relations-0.1.1/src/optical_dispersion_relations.egg-info/dependency_links.txt
--rw-r--r--   0 george     (501) staff       (20)       14 2022-11-29 20:30:00.000000 optical_dispersion_relations-0.1.1/src/optical_dispersion_relations.egg-info/requires.txt
--rw-r--r--   0 george     (501) staff       (20)       29 2022-11-29 20:30:00.000000 optical_dispersion_relations-0.1.1/src/optical_dispersion_relations.egg-info/top_level.txt
-drwxr-xr-x   0 george     (501) staff       (20)        0 2022-11-29 20:30:00.641045 optical_dispersion_relations-0.1.1/test/
--rw-r--r--   0 george     (501) staff       (20)     2273 2022-11-29 19:55:02.000000 optical_dispersion_relations-0.1.1/test/test_dielectric_waveguide.py
--rw-r--r--   0 george     (501) staff       (20)     3715 2022-11-19 19:16:36.000000 optical_dispersion_relations-0.1.1/test/test_drude_lorentz.py
--rw-r--r--   0 george     (501) staff       (20)     5846 2022-11-19 19:16:36.000000 optical_dispersion_relations-0.1.1/test/test_plasmon.py
--rw-r--r--   0 george     (501) staff       (20)     1768 2022-11-19 19:16:36.000000 optical_dispersion_relations-0.1.1/test/test_utilities.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-06 20:34:05.825769 optical_dispersion_relations-0.2.0/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1071 2023-05-06 20:05:35.000000 optical_dispersion_relations-0.2.0/LICENSE.txt
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2100 2023-05-06 20:34:05.821769 optical_dispersion_relations-0.2.0/PKG-INFO
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1565 2023-05-06 20:05:35.000000 optical_dispersion_relations-0.2.0/README.md
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-06 20:34:05.817769 optical_dispersion_relations-0.2.0/optical_dispersion_relations/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)        0 2023-05-06 20:05:35.000000 optical_dispersion_relations-0.2.0/optical_dispersion_relations/__init__.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4553 2023-05-06 20:05:35.000000 optical_dispersion_relations-0.2.0/optical_dispersion_relations/dielectric_waveguides.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     5636 2023-05-06 20:05:35.000000 optical_dispersion_relations-0.2.0/optical_dispersion_relations/drude_lorentz.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3976 2023-05-06 20:05:35.000000 optical_dispersion_relations-0.2.0/optical_dispersion_relations/plasmon.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1342 2023-05-06 20:05:35.000000 optical_dispersion_relations-0.2.0/optical_dispersion_relations/utilities.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-06 20:34:05.821769 optical_dispersion_relations-0.2.0/optical_dispersion_relations.egg-info/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2100 2023-05-06 20:34:05.000000 optical_dispersion_relations-0.2.0/optical_dispersion_relations.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      623 2023-05-06 20:34:05.000000 optical_dispersion_relations-0.2.0/optical_dispersion_relations.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)        1 2023-05-06 20:34:05.000000 optical_dispersion_relations-0.2.0/optical_dispersion_relations.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)       14 2023-05-06 20:34:05.000000 optical_dispersion_relations-0.2.0/optical_dispersion_relations.egg-info/requires.txt
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)       29 2023-05-06 20:34:05.000000 optical_dispersion_relations-0.2.0/optical_dispersion_relations.egg-info/top_level.txt
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      714 2023-05-06 20:05:35.000000 optical_dispersion_relations-0.2.0/pyproject.toml
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)       38 2023-05-06 20:34:05.825769 optical_dispersion_relations-0.2.0/setup.cfg
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-06 20:34:05.821769 optical_dispersion_relations-0.2.0/test/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2185 2023-05-06 20:05:35.000000 optical_dispersion_relations-0.2.0/test/test_dielectric_waveguide.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     6848 2023-05-06 20:05:35.000000 optical_dispersion_relations-0.2.0/test/test_drude_lorentz.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     5902 2023-05-06 20:05:35.000000 optical_dispersion_relations-0.2.0/test/test_plasmon.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2109 2023-05-06 20:05:35.000000 optical_dispersion_relations-0.2.0/test/test_utilities.py
```

### Comparing `optical_dispersion_relations-0.1.1/LICENSE.txt` & `optical_dispersion_relations-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `optical_dispersion_relations-0.1.1/PKG-INFO` & `optical_dispersion_relations-0.2.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,32 +1,71 @@
 Metadata-Version: 2.1
 Name: optical_dispersion_relations
-Version: 0.1.1
+Version: 0.2.0
 Summary: Optical Dispersion Relations
 Author: George Duffett
 Project-URL: Homepage, https://github.com/g-duff/optical_dispersion_relations
 Project-URL: Bug Tracker, https://github.com/g-duff/optical_dispersion_relations/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-# Optical dispersion relations
+# [Optical Dispersion Relations](https://github.com/g-duff/optical_dispersion_relations)
 
 ## Features
 
 * A collection of exact and approximate optical dispersion relations.
 * Academic Sources eg textbooks and journal articles.
 * Fully tested (see `test/`) so users can calculate with confidence.
 
+## Examples
+
+* Silver permittivity can be calculated with a Single Pole Drude-Lorentz model:
+
+```py
+silver_drude_parameters = {
+	'dielectric_constant': 1,
+	'plasma_frequency': 1.35e16,
+	'damping_constant': 0.0023*1.35e16,
+}
+
+silver_permittivity = drude_lorentz.single_pole(
+	angular_frequency, **silver_drude_parameters)
+```
+
+* Gold permittivity can be calculated with a Double Pole Drude-Lorentz model:
+
+```py
+gold_drude_parameters = {
+	'dielectric_constant': 6,
+	'plasma_frequency': 1,
+	'first_pole': {
+		'peak_strength': 5.37e15**2,
+		'damping_constant': 6.216e13,
+		'peak_position': 0,
+	},
+	'second_pole': {
+		'peak_strength': 2.263e15**2,
+		'damping_constant': 1.332e15,
+		'peak_position': 4.572e15
+	}
+}
+
+gold_permittivity = drude_lorentz.double_pole(
+	angular_frequency, **gold_drude_parameters)
+```
+
+* More examples can be found under `/examples/`.
+
 ## Install
 
-Install with pip eg:
+[Install with pip](https://pypi.org/project/optical-dispersion-relations/) eg:
 
 ```sh
 pip3 install optical_dispersion_relations
 ```
 
 Download the latest release [here](https://github.com/g-duff/optical_dispersion_relations/releases/latest), or previous releases [here](https://github.com/g-duff/optical_dispersion_relations/releases).
```

### Comparing `optical_dispersion_relations-0.1.1/pyproject.toml` & `optical_dispersion_relations-0.2.0/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,19 +1,26 @@
+[build-system]
+requires = ["setuptools>=61.0"]
+build-backend = "setuptools.build_meta"
+
 [project]
 dependencies = ["numpy>=1.23.4"]
 name = "optical_dispersion_relations"
-version = "0.1.1"
+version = "0.2.0"
 authors = [
   { name="George Duffett" },
 ]
 description = "Optical Dispersion Relations"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
+[tool.setuptools.packages.find]
+include = ["optical_dispersion_relations*"]
+
 [project.urls]
 "Homepage" = "https://github.com/g-duff/optical_dispersion_relations"
 "Bug Tracker" = "https://github.com/g-duff/optical_dispersion_relations/issues"
```

### Comparing `optical_dispersion_relations-0.1.1/src/optical_dispersion_relations/dielectric_waveguides.py` & `optical_dispersion_relations-0.2.0/optical_dispersion_relations/dielectric_waveguides.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-'''Dielectric Waveduide dispersions'''
+"""Dielectric Waveduide dispersions"""
 
 import numpy as np
 from numpy.lib import scimath
 
 
-def transcendential_slab_waveguide_TE(
-    waveguide_propagation_constant,
-    free_space_wavenumber,
-    waveguide_thickness,
-    cover_refractive_index,
-    guiding_layer_refractive_index,
-    substrate_refractive_index,
-):
-    # pylint: disable = invalid-name, too-many-arguments
-    '''Transcendential equation for a slab waveguide with TE polarization.
+def transcendential_slab_waveguide_te(
+    waveguide_propagation_constant: float,
+    free_space_wavenumber: float,
+    waveguide_thickness: float,
+    cover_refractive_index: float,
+    guiding_layer_refractive_index: float,
+    substrate_refractive_index: float,
+) -> float:
+    # pylint: disable = too-many-arguments
+    """Transcendential equation for a slab waveguide with TE polarization.
     Find the value of waveguide_propagation_constant for which the function equals zero
     to solve the system.
 
     Parameters
     ----------
     waveguide_propagation_constant: float, unkown - vary to find the system solutions.
     free_space_wavenumber: float
@@ -31,15 +31,15 @@
     residual to be minimized: float
 
     Derivation
     ----------
     Yariv, A. Optical Electronics.
     ISBN-10: 0030474442
     ISBN-13: 9780030474446
-    '''
+    """
 
     cover_wavenumber = cover_refractive_index * free_space_wavenumber
     guiding_layer_wavenumber = guiding_layer_refractive_index * free_space_wavenumber
     substrate_wavenumber = substrate_refractive_index * free_space_wavenumber
 
     cover_parameter = scimath.sqrt(
         waveguide_propagation_constant**2 - cover_wavenumber**2)
@@ -55,24 +55,24 @@
 
     transcendential_function_value = np.tan(
         guiding_layer_parameter*waveguide_thickness)
 
     return np.abs(transcendential_function_value - algebraic_function_value)
 
 
-def transcendential_slab_waveguide_TM(
-    waveguide_propagation_constant,
-    free_space_wavenumber,
-    waveguide_thickness,
-    cover_refractive_index,
-    guiding_layer_refractive_index,
-    substrate_refractive_index,
-):
-    # pylint: disable = invalid-name, too-many-arguments
-    '''Transcendential equation for a slab waveguide with TM polarization.
+def transcendential_slab_waveguide_tm(
+    waveguide_propagation_constant: float,
+    free_space_wavenumber: float,
+    waveguide_thickness: float,
+    cover_refractive_index: float,
+    guiding_layer_refractive_index: float,
+    substrate_refractive_index: float,
+) -> float:
+    # pylint: disable = too-many-arguments
+    """Transcendential equation for a slab waveguide with TM polarization.
     Find the value of waveguide_propagation_constant for which the function equals zero
     to solve the system.
 
     Parameters
     ----------
     waveguide_propagation_constant: float, unkown - vary to find the system solutions.
     free_space_wavenumber: float
@@ -86,40 +86,41 @@
     residual to be minimized: float
 
     Derivation
     ----------
     Yariv, A. Optical Electronics.
     ISBN-10: 0030474442
     ISBN-13: 9780030474446
-    '''
+    """
 
     cover_wavenumber = cover_refractive_index * free_space_wavenumber
     guiding_layer_wavenumber = guiding_layer_refractive_index * free_space_wavenumber
     substrate_wavenumber = substrate_refractive_index * free_space_wavenumber
 
     cover_parameter = scimath.sqrt(waveguide_propagation_constant**2 - cover_wavenumber**2) \
         * (guiding_layer_refractive_index/cover_refractive_index)**2
-    substrate_parameter = scimath.sqrt(waveguide_propagation_constant**2 - substrate_wavenumber**2) \
-        * (guiding_layer_refractive_index/substrate_refractive_index)**2
+    substrate_parameter = scimath.sqrt(
+        waveguide_propagation_constant**2 - substrate_wavenumber**2
+    ) * (guiding_layer_refractive_index/substrate_refractive_index)**2
 
     guiding_layer_parameter = scimath.sqrt(
         guiding_layer_wavenumber**2 - waveguide_propagation_constant**2)
 
     algebraic_function_value = algebraic_function(cover_parameter,
                                                   guiding_layer_parameter,
                                                   substrate_parameter)
 
     transcendential_function_value = np.tan(
         guiding_layer_parameter*waveguide_thickness)
 
     return np.abs(transcendential_function_value - algebraic_function_value)
 
 
-def algebraic_function(cover_parameter,
-                       guiding_layer_parameter,
-                       substrate_parameter):
+def algebraic_function(cover_parameter: complex,
+                       guiding_layer_parameter: complex,
+                       substrate_parameter) -> complex:
     # pylint: disable = missing-function-docstring
     algebraic_function_value = guiding_layer_parameter \
         * (substrate_parameter + cover_parameter) \
         / (guiding_layer_parameter**2 - substrate_parameter*cover_parameter)
 
     return algebraic_function_value
```

### Comparing `optical_dispersion_relations-0.1.1/src/optical_dispersion_relations/plasmon.py` & `optical_dispersion_relations-0.2.0/optical_dispersion_relations/plasmon.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-'''Plasmonics Dispersion Relations'''
+"""Plasmonics Dispersion Relations"""
+
 import numpy as np
 
 
 def surface_plasmon_polariton(dielectric_permittivity: float,
                               metal_permittivity: complex) -> complex:
-    '''Exact surface plasmon dispersion relation for TM polarization.
+    """Exact surface plasmon dispersion relation for TM polarization.
     Surface plasmons only exist for TM polarization.
 
     Parameters
     ----------
     dielectric_permittivity: float, complex number or numpy array
     metal_permittivity: float, complex number or numpy array
 
@@ -16,26 +17,26 @@
     -------
     effective_refractive_index of surface plasmon polariton: complex number or numpy array
 
     Derivation
     ----------
     Maier SA. Plasmonics: Fundamentals and Applications.
     ISBN: 978-0-387-37825-1
-    '''
+    """
     numerator = dielectric_permittivity*metal_permittivity
     denominator = dielectric_permittivity+metal_permittivity
     effective_refractive_index = np.sqrt(numerator/denominator)
     return effective_refractive_index
 
 
 def metal_insulator_metal_collin_approximation(dielectric_permittivity: float,
                                                metal_permittivity: complex,
                                                wavelength: float,
                                                insulator_thickness: float) -> complex:
-    '''Approximate metal-insulator-metal waveguide dispersion relation for TM polarization.
+    """Approximate metal-insulator-metal waveguide dispersion relation for TM polarization.
 
     Parameters
     ----------
     dielectric_permittivity: float or complex
     metal_permittivity: float or complex
     wavelength, in any unit of distance: float
     insulator_thickness, in the same unit of distance as wavelength: float
@@ -44,28 +45,28 @@
     -------
     effective_refractive_index of the light propagating in the waveguide: complex
 
     Derivation
     ----------
     Waveguiding in nanoscale metallic apertures.
     https://doi.org/10.1364/OE.15.004310
-    '''
+    """
     surface_plasmon_coupling_term = wavelength * \
         np.sqrt(1-dielectric_permittivity/metal_permittivity) / \
         (np.pi*insulator_thickness*np.sqrt(-1*metal_permittivity))
     effective_refractive_index = np.sqrt(dielectric_permittivity) * \
         np.sqrt(1 + surface_plasmon_coupling_term)
     return effective_refractive_index
 
 
 def metal_insulator_metal_sondergaard_narrow_approximation(dielectric_permittivity: float,
                                                            metal_permittivity: complex,
                                                            wavelength: float,
                                                            insulator_thickness: float) -> complex:
-    '''Approximate metal-insulator-metal waveguide dispersion relation for TM polarization.
+    """Approximate metal-insulator-metal waveguide dispersion relation for TM polarization.
 
     Parameters
     ----------
     dielectric_permittivity: float or complex
     metal_permittivity: float or complex
     wavelength: float, in any unit of distance
     insulator_thickness: float, in the same unit of distance as wavelength
@@ -73,15 +74,15 @@
     Returns
     -------
     effective_refractive_index of the light propagating in the wavevuide: complex
 
     Derivation
     ----------
     General properties of slow-plasmon resonant nanostructures: nano-antennas and resonators.
-    https://doi.org/10.1364/OE.15.010869'''
+    https://doi.org/10.1364/OE.15.010869"""
     freespace_wavenumber = 2 * np.pi / wavelength
 
     narrow_gap_limit_propagation_constant = -2 * dielectric_permittivity \
         / (insulator_thickness * metal_permittivity)
 
     narrow_gap_limit_effective_refractive_index = narrow_gap_limit_propagation_constant \
         / freespace_wavenumber
```

### Comparing `optical_dispersion_relations-0.1.1/src/optical_dispersion_relations/utilities.py` & `optical_dispersion_relations-0.2.0/optical_dispersion_relations/utilities.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,53 +1,66 @@
-'''Utilities for calculating optical parameters'''
+"""Utilities for calculating optical parameters"""
 import numpy as np
 
 
 def permittivity_to_extinction_coefficient(
     permittivity: complex
 ) -> float:
-    '''Convert complex permittivity to extinction coefficient
+    """Convert complex permittivity to extinction coefficient
 
     Parameters
     ----------
     permittivity: float
 
     Returns
     -------
     extinction_coefficient: complex
-    '''
+    """
     refractive_index: complex = permittivity_to_refractive_index(
         permittivity)
     extinction_coefficient = refractive_index.imag
     return extinction_coefficient
 
 
 def permittivity_to_refractive_index(
     permittivity: complex
 ) -> complex:
-    '''Convert complex permittivity to complex refractive index
+    """Convert complex permittivity to complex refractive index
 
     Parameters
     ----------
     permittivity: complex
 
     Returns
     -------
     refractive_index: complex
-    '''
+    """
     return np.sqrt(permittivity)
 
 
 def refractive_index_to_permittivity(
     refractive_index: complex
 ) -> complex:
-    '''Convert complex refractive index to complex permittivity
+    """Convert complex refractive index to complex permittivity
 
     Parameters
     ----------
     refractive_index: complex
 
     Returns
     -------
     permittivity: complex
-    '''
+    """
     return refractive_index**2
+
+
+def wavelength_to_wavenumber(wavelength: float) -> float:
+    """Convert wavelength to wavenumber
+
+    Parameters
+    ----------
+    wavelength: float
+
+    Returns
+    -------
+    wavenumber: float"""
+    return 2*np.pi/wavelength
```

### Comparing `optical_dispersion_relations-0.1.1/src/optical_dispersion_relations.egg-info/PKG-INFO` & `optical_dispersion_relations-0.2.0/optical_dispersion_relations.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,32 +1,71 @@
 Metadata-Version: 2.1
 Name: optical-dispersion-relations
-Version: 0.1.1
+Version: 0.2.0
 Summary: Optical Dispersion Relations
 Author: George Duffett
 Project-URL: Homepage, https://github.com/g-duff/optical_dispersion_relations
 Project-URL: Bug Tracker, https://github.com/g-duff/optical_dispersion_relations/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-# Optical dispersion relations
+# [Optical Dispersion Relations](https://github.com/g-duff/optical_dispersion_relations)
 
 ## Features
 
 * A collection of exact and approximate optical dispersion relations.
 * Academic Sources eg textbooks and journal articles.
 * Fully tested (see `test/`) so users can calculate with confidence.
 
+## Examples
+
+* Silver permittivity can be calculated with a Single Pole Drude-Lorentz model:
+
+```py
+silver_drude_parameters = {
+	'dielectric_constant': 1,
+	'plasma_frequency': 1.35e16,
+	'damping_constant': 0.0023*1.35e16,
+}
+
+silver_permittivity = drude_lorentz.single_pole(
+	angular_frequency, **silver_drude_parameters)
+```
+
+* Gold permittivity can be calculated with a Double Pole Drude-Lorentz model:
+
+```py
+gold_drude_parameters = {
+	'dielectric_constant': 6,
+	'plasma_frequency': 1,
+	'first_pole': {
+		'peak_strength': 5.37e15**2,
+		'damping_constant': 6.216e13,
+		'peak_position': 0,
+	},
+	'second_pole': {
+		'peak_strength': 2.263e15**2,
+		'damping_constant': 1.332e15,
+		'peak_position': 4.572e15
+	}
+}
+
+gold_permittivity = drude_lorentz.double_pole(
+	angular_frequency, **gold_drude_parameters)
+```
+
+* More examples can be found under `/examples/`.
+
 ## Install
 
-Install with pip eg:
+[Install with pip](https://pypi.org/project/optical-dispersion-relations/) eg:
 
 ```sh
 pip3 install optical_dispersion_relations
 ```
 
 Download the latest release [here](https://github.com/g-duff/optical_dispersion_relations/releases/latest), or previous releases [here](https://github.com/g-duff/optical_dispersion_relations/releases).
```

### Comparing `optical_dispersion_relations-0.1.1/src/optical_dispersion_relations.egg-info/SOURCES.txt` & `optical_dispersion_relations-0.2.0/optical_dispersion_relations.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 LICENSE.txt
 README.md
 pyproject.toml
-src/optical_dispersion_relations/__init__.py
-src/optical_dispersion_relations/dielectric_waveguides.py
-src/optical_dispersion_relations/drude_lorentz.py
-src/optical_dispersion_relations/plasmon.py
-src/optical_dispersion_relations/utilities.py
-src/optical_dispersion_relations.egg-info/PKG-INFO
-src/optical_dispersion_relations.egg-info/SOURCES.txt
-src/optical_dispersion_relations.egg-info/dependency_links.txt
-src/optical_dispersion_relations.egg-info/requires.txt
-src/optical_dispersion_relations.egg-info/top_level.txt
+optical_dispersion_relations/__init__.py
+optical_dispersion_relations/dielectric_waveguides.py
+optical_dispersion_relations/drude_lorentz.py
+optical_dispersion_relations/plasmon.py
+optical_dispersion_relations/utilities.py
+optical_dispersion_relations.egg-info/PKG-INFO
+optical_dispersion_relations.egg-info/SOURCES.txt
+optical_dispersion_relations.egg-info/dependency_links.txt
+optical_dispersion_relations.egg-info/requires.txt
+optical_dispersion_relations.egg-info/top_level.txt
 test/test_dielectric_waveguide.py
 test/test_drude_lorentz.py
 test/test_plasmon.py
 test/test_utilities.py
```

### Comparing `optical_dispersion_relations-0.1.1/test/test_dielectric_waveguide.py` & `optical_dispersion_relations-0.2.0/test/test_dielectric_waveguide.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,65 +1,61 @@
 # pylint: disable = import-error, missing-class-docstring, missing-function-docstring, missing-module-docstring
 import unittest
 import numpy as np
-from src.optical_dispersion_relations import dielectric_waveguides
+from optical_dispersion_relations import dielectric_waveguides
 
 
 class TranscendentialSlabWaveguide(unittest.TestCase):
-    '''Benchmarks from Online Mode Solver: 1-D mode solver for dielectric multilayer slab waveguides
+    """Benchmarks from Online Mode Solver: 1-D mode solver for dielectric multilayer slab waveguides
     https://www.siio.eu/oms.html
-    '''
-
-    def test_TE_constants_benchmark(self):
-        # pylint: disable = invalid-name
+    """
 
+    def test_te_constants_benchmark(self):
         # Given
         free_space_wavelength = 1.550
         waveguide_effective_refractive_index = 1.876691009
 
         free_space_wavenumber = 2*np.pi/free_space_wavelength
         waveguide_propagation_constant = free_space_wavenumber * \
             waveguide_effective_refractive_index
 
         waveguide_thickness = 0.5
         cover_refractive_index = 1.0
         guiding_layer_refractive_index = 2.1
         substrate_refractive_index = 1.5
 
         # When
-        residual = dielectric_waveguides.transcendential_slab_waveguide_TE(
+        residual = dielectric_waveguides.transcendential_slab_waveguide_te(
             waveguide_propagation_constant,
             free_space_wavenumber,
             waveguide_thickness,
             cover_refractive_index,
             guiding_layer_refractive_index,
             substrate_refractive_index,
         )
 
         # Then
         self.assertAlmostEqual(residual, 0)
 
-    def test_TM_constants_benchmark(self):
-        # pylint: disable = invalid-name
-
+    def test_tm_constants_benchmark(self):
         # Given
         free_space_wavelength = 1.550
         waveguide_effective_refractive_index = 1.744774075
 
         free_space_wavenumber = 2*np.pi/free_space_wavelength
         waveguide_propagation_constant = free_space_wavenumber * \
             waveguide_effective_refractive_index
 
         waveguide_thickness = 0.5
         cover_refractive_index = 1.0
         guiding_layer_refractive_index = 2.1
         substrate_refractive_index = 1.5
 
         # When
-        residual = dielectric_waveguides.transcendential_slab_waveguide_TM(
+        residual = dielectric_waveguides.transcendential_slab_waveguide_tm(
             waveguide_propagation_constant,
             free_space_wavenumber,
             waveguide_thickness,
             cover_refractive_index,
             guiding_layer_refractive_index,
             substrate_refractive_index,
         )
```

### Comparing `optical_dispersion_relations-0.1.1/test/test_plasmon.py` & `optical_dispersion_relations-0.2.0/test/test_plasmon.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,19 @@
-# pylint: disable = import-error, missing-class-docstring, missing-function-docstring, missing-module-docstring
+#  pylint: disable = import-error, missing-class-docstring, missing-function-docstring, missing-module-docstring
 import unittest
 import numpy as np
-from src.optical_dispersion_relations import plasmon
+from optical_dispersion_relations import plasmon
 
 
 class SurfacePlasmonPolariton(unittest.TestCase):
 
     def test_constants_from_textbook(self):
-        '''Test against fig 2.3 in Maier SA. Plasmonics: fundamentals and applications.
-        ISBN: 978-0-387-37825-1'''
+        """Test against fig 2.3 in Maier SA. Plasmonics: fundamentals and applications.
+        ISBN: 978-0-387-37825-1
+        """
         # Given
         dielectric_permittivity = 1
         metal_permittivity = np.array([-99. + 0.j,
                                        -24. + 0.j,
                                        -10.11111111 + 0.j,
                                        -5.25 + 0.j,
                                        -3. + 0.j,
@@ -41,16 +42,17 @@
 
         # Then
         self.assertTrue(np.allclose(
             expected_refractive_index, actual_refractive_index))
 
 
 class MetalInsulatorMetalCollinApproximation(unittest.TestCase):
-    '''Test against fig 2 in Waveguiding in nanoscale metallic apertures.
-    https://doi.org/10.1364/OE.15.004310'''
+    """Test against fig 2 in Waveguiding in nanoscale metallic apertures.
+    https://doi.org/10.1364/OE.15.004310
+    """
 
     def test_thick_insulator(self):
         # Given
         dielectric_permittivity = 1
         metal_permittivity = -50
         insulator_thickness = 10
         wavelength = 1
@@ -90,17 +92,18 @@
         # Then
         self.assertAlmostEqual(expected_effective_refractive_index,
                                actual_effective_refractive_index,
                                places=3)
 
 
 class MetalInsulatorMetalSondergaardNarrowApproximation(unittest.TestCase):
-    '''Test against fig 4 in
+    """Test against fig 4 in
     General properties of slow-plasmon resonant nanostructures: nano-antennas and resonators.
-    https://doi.org/10.1364/OE.15.010869'''
+    https://doi.org/10.1364/OE.15.010869
+    """
 
     def test_insulator_constants(self):
         # Given
         dielectric_permittivity = 1
         metal_permittivity = -23.6+1.69j
         wavelength = 775
         insulator_thickness = np.array([100, 200, 300, 400, 500])
@@ -110,19 +113,19 @@
                                                         1.08308215+0.00300229j,
                                                         1.062867+0.00228691j,
                                                         1.05056857+0.00184725j])
 
         # When
         actual_effective_refractive_index = \
             plasmon.metal_insulator_metal_sondergaard_narrow_approximation(
-            dielectric_permittivity=dielectric_permittivity,
-            metal_permittivity=metal_permittivity,
-            wavelength=wavelength,
-            insulator_thickness=insulator_thickness,
-        )
+                dielectric_permittivity=dielectric_permittivity,
+                metal_permittivity=metal_permittivity,
+                wavelength=wavelength,
+                insulator_thickness=insulator_thickness,
+            )
 
         # Then
         self.assertTrue(np.allclose(
             expected_effective_refractive_index, actual_effective_refractive_index))
 
     def test_thick_insulator(self):
         # Given
@@ -132,17 +135,17 @@
         wavelength = 1
 
         expected_effective_refractive_index = 1
 
         # When
         actual_effective_refractive_index = \
             plasmon.metal_insulator_metal_sondergaard_narrow_approximation(
-            dielectric_permittivity=dielectric_permittivity,
-            metal_permittivity=metal_permittivity,
-            wavelength=wavelength,
-            insulator_thickness=insulator_thickness,
-        )
+                dielectric_permittivity=dielectric_permittivity,
+                metal_permittivity=metal_permittivity,
+                wavelength=wavelength,
+                insulator_thickness=insulator_thickness,
+            )
 
         # Then
         self.assertAlmostEqual(expected_effective_refractive_index,
                                actual_effective_refractive_index,
                                places=2)
```

### Comparing `optical_dispersion_relations-0.1.1/test/test_utilities.py` & `optical_dispersion_relations-0.2.0/test/test_utilities.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # pylint: disable = import-error, missing-class-docstring, missing-function-docstring, missing-module-docstring
 import unittest
-from src.optical_dispersion_relations import utilities
+from optical_dispersion_relations import utilities
 
 
 class Utilities(unittest.TestCase):
 
     def test_permittivity_to_extinction_coefficient(self):
         # Given
         complex_permittivity = 3.75 + 2.0j
@@ -45,7 +45,19 @@
             refractive_index)
 
         # Then
         self.assertAlmostEqual(expected_permittivity_real,
                                actual_permittivity.real)
         self.assertAlmostEqual(
             expected_permittivity_imaginary, actual_permittivity.imag)
+
+    def test_wavelength_to_wavenumber(self):
+        # Given
+        wavelength = 628.318
+        expected_wavenumber = 0.01
+
+        # When
+        actual_wavenumber = utilities.wavelength_to_wavenumber(wavelength)
+
+        # Then
+        self.assertAlmostEqual(expected_wavenumber,
+                               actual_wavenumber, places=6)
```

