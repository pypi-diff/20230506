# Comparing `tmp/colliderscope-0.2.2.tar.gz` & `tmp/colliderscope-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "colliderscope-0.2.2.tar", last modified: Thu Mar  9 16:34:28 2023, max compression
+gzip compressed data, was "colliderscope-0.2.3.tar", last modified: Sat May  6 13:00:23 2023, max compression
```

## Comparing `colliderscope-0.2.2.tar` & `colliderscope-0.2.3.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 16:34:28.182549 colliderscope-0.2.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 16:34:28.174549 colliderscope-0.2.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 16:34:28.178549 colliderscope-0.2.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-03-09 16:34:15.000000 colliderscope-0.2.2/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-03-09 16:34:15.000000 colliderscope-0.2.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-03-09 16:34:15.000000 colliderscope-0.2.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-03-09 16:34:15.000000 colliderscope-0.2.2/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-03-09 16:34:15.000000 colliderscope-0.2.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-03-09 16:34:28.178549 colliderscope-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-03-09 16:34:15.000000 colliderscope-0.2.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 16:34:28.178549 colliderscope-0.2.2/colliderscope/
--rw-r--r--   0 runner    (1001) docker     (123)    27680 2023-03-09 16:34:15.000000 colliderscope-0.2.2/colliderscope/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5141 2023-03-09 16:34:15.000000 colliderscope-0.2.2/colliderscope/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-03-09 16:34:28.000000 colliderscope-0.2.2/colliderscope/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-03-09 16:34:15.000000 colliderscope-0.2.2/colliderscope/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6724 2023-03-09 16:34:15.000000 colliderscope-0.2.2/colliderscope/webui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 16:34:28.178549 colliderscope-0.2.2/colliderscope.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-03-09 16:34:28.000000 colliderscope-0.2.2/colliderscope.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-03-09 16:34:28.000000 colliderscope-0.2.2/colliderscope.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-09 16:34:28.000000 colliderscope-0.2.2/colliderscope.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-03-09 16:34:28.000000 colliderscope-0.2.2/colliderscope.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-03-09 16:34:28.000000 colliderscope-0.2.2/colliderscope.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-03-09 16:34:28.000000 colliderscope-0.2.2/colliderscope.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 16:34:28.178549 colliderscope-0.2.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-03-09 16:34:15.000000 colliderscope-0.2.2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-03-09 16:34:15.000000 colliderscope-0.2.2/docs/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-03-09 16:34:15.000000 colliderscope-0.2.2/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 16:34:28.178549 colliderscope-0.2.2/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 16:34:28.178549 colliderscope-0.2.2/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-09 16:34:15.000000 colliderscope-0.2.2/docs/source/_static/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 16:34:28.178549 colliderscope-0.2.2/docs/source/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-09 16:34:15.000000 colliderscope-0.2.2/docs/source/_templates/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-03-09 16:34:15.000000 colliderscope-0.2.2/docs/source/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-03-09 16:34:15.000000 colliderscope-0.2.2/docs/source/cli.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6922 2023-03-09 16:34:15.000000 colliderscope-0.2.2/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-03-09 16:34:15.000000 colliderscope-0.2.2/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-03-09 16:34:15.000000 colliderscope-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-09 16:34:28.182549 colliderscope-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-09 16:34:15.000000 colliderscope-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 13:00:23.239854 colliderscope-0.2.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 13:00:23.235854 colliderscope-0.2.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 13:00:23.235854 colliderscope-0.2.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-06 13:00:13.000000 colliderscope-0.2.3/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-06 13:00:13.000000 colliderscope-0.2.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-05-06 13:00:13.000000 colliderscope-0.2.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-06 13:00:13.000000 colliderscope-0.2.3/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-05-06 13:00:13.000000 colliderscope-0.2.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-05-06 13:00:23.239854 colliderscope-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-05-06 13:00:13.000000 colliderscope-0.2.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 13:00:23.235854 colliderscope-0.2.3/colliderscope/
+-rw-r--r--   0 runner    (1001) docker     (123)    34158 2023-05-06 13:00:13.000000 colliderscope-0.2.3/colliderscope/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5141 2023-05-06 13:00:13.000000 colliderscope-0.2.3/colliderscope/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-06 13:00:23.000000 colliderscope-0.2.3/colliderscope/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-05-06 13:00:13.000000 colliderscope-0.2.3/colliderscope/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6724 2023-05-06 13:00:13.000000 colliderscope-0.2.3/colliderscope/webui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 13:00:23.235854 colliderscope-0.2.3/colliderscope.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-05-06 13:00:23.000000 colliderscope-0.2.3/colliderscope.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-06 13:00:23.000000 colliderscope-0.2.3/colliderscope.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 13:00:23.000000 colliderscope-0.2.3/colliderscope.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-06 13:00:23.000000 colliderscope-0.2.3/colliderscope.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-06 13:00:23.000000 colliderscope-0.2.3/colliderscope.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-06 13:00:23.000000 colliderscope-0.2.3/colliderscope.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 13:00:23.235854 colliderscope-0.2.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-06 13:00:13.000000 colliderscope-0.2.3/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-05-06 13:00:13.000000 colliderscope-0.2.3/docs/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-06 13:00:13.000000 colliderscope-0.2.3/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 13:00:23.239854 colliderscope-0.2.3/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 13:00:23.239854 colliderscope-0.2.3/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 13:00:13.000000 colliderscope-0.2.3/docs/source/_static/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 13:00:23.239854 colliderscope-0.2.3/docs/source/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 13:00:13.000000 colliderscope-0.2.3/docs/source/_templates/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-06 13:00:13.000000 colliderscope-0.2.3/docs/source/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-05-06 13:00:13.000000 colliderscope-0.2.3/docs/source/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6922 2023-05-06 13:00:13.000000 colliderscope-0.2.3/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-06 13:00:13.000000 colliderscope-0.2.3/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-05-06 13:00:13.000000 colliderscope-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 13:00:23.239854 colliderscope-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-06 13:00:13.000000 colliderscope-0.2.3/setup.py
```

### Comparing `colliderscope-0.2.2/.github/workflows/publish-to-pypi.yml` & `colliderscope-0.2.3/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `colliderscope-0.2.2/.gitignore` & `colliderscope-0.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `colliderscope-0.2.2/.pre-commit-config.yaml` & `colliderscope-0.2.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `colliderscope-0.2.2/LICENSE.txt` & `colliderscope-0.2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `colliderscope-0.2.2/PKG-INFO` & `colliderscope-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: colliderscope
-Version: 0.2.2
+Version: 0.2.3
 Summary: Plotting tools for Monte-Carlo particle showers.
 Author: Jacan Chaplais
 Maintainer: Jacan Chaplais
 License: BSD 3-Clause License
         
         Copyright (c) 2021, Jacan Chaplais.
         All rights reserved.
```

### Comparing `colliderscope-0.2.2/README.rst` & `colliderscope-0.2.3/README.rst`

 * *Files identical despite different names*

### Comparing `colliderscope-0.2.2/colliderscope/__init__.py` & `colliderscope-0.2.3/colliderscope/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,28 +4,30 @@
 
 Visualise your high energy physics (HEP) data with colliderscope!
 """
 import collections as cl
 import collections.abc as cla
 import dataclasses as dc
 import gzip as gz
+import io
 import itertools as it
 import json
 import operator as op
 import textwrap as tw
 import typing as ty
 import warnings
 from pathlib import Path
 
 import colour
 import graphicle as gcl
 import more_itertools as mit
 import numpy as np
 import pandas as pd
 import plotly.express as px
+import plotly.graph_objs as go
 import webcolors
 from pyvis.network import Network
 from scipy.stats import cauchy
 
 from . import base
 from ._version import __version__, __version_tuple__
 
@@ -38,14 +40,15 @@
     "__version__",
     "__version_tuple__",
     "Color",
     "NodePdgs",
     "color_range",
     "shower_dag",
     "eta_phi_scatter",
+    "eta_phi_network",
     "Histogram",
     "breit_wigner_pdf",
     "hist_to_bw_params",
     "histogram_barchart",
 ]
 
 
@@ -538,67 +541,85 @@
         idx = np.digitize(val, self.bin_edges) - 1
         if -1 < idx < self.num_bins:
             self.counts[idx] += 1
         self._total += 1
 
     def to_json(
         self,
-        fname: ty.Union[str, Path],
+        fname: ty.Union[str, Path, io.IOBase],
         encoding: str = "utf-8",
     ) -> None:
         """Serialise and store ``Histogram`` object as a JSON file.
 
+        .. versionchanged:: 0.2.3
+           ``fname`` accepts file-like object.
+
         Parameters
         ----------
-        fname : str or Path
-            Location on disk to save the data. If ``gzip`` compression
-            is desired, use the ``".gz"`` extension.
+        fname : str or Path or file-like
+            Location on disk, or file-object, to save the data. If
+            ``gzip`` compression is desired, use the ``".gz"``
+            extension.
         encoding : str
             Standard used to encode the text into binary formats.
             Default is ``"utf-8"``.
         """
-        fname = Path(fname)
-        if fname.suffix == ".gz":
-            f = gz.open(fname, mode="wt", encoding=encoding)
-        else:
-            f = open(fname, mode="w", encoding=encoding)
         data = dc.asdict(self)
         for key, val in data.items():
             if isinstance(val, np.ndarray):
                 data[key] = val.tolist()
-        with f:
-            json.dump(data, f)
+        if isinstance(fname, io.TextIOBase):
+            json.dump(data, fname)
+        elif isinstance(fname, io.IOBase):
+            with io.StringIO() as f:
+                json.dump(data, f)
+                fname.write(f.getvalue().encode(encoding))
+        else:
+            fname = Path(fname)
+            if fname.suffix == ".gz":
+                f = gz.open(fname, mode="wt", encoding=encoding)
+            else:
+                f = open(fname, mode="w", encoding=encoding)
+            with f:
+                json.dump(data, f)
 
     @classmethod
     def from_json(
         cls,
-        fname: ty.Union[str, Path],
+        fname: ty.Union[str, Path, io.IOBase],
         encoding: str = "utf-8",
     ) -> "Histogram":
         """Instantiate a histogram from JSON file, encoded using the
         ``Histogram.to_json()`` method.
 
+        .. versionchanged:: 0.2.3
+           ``fname`` accepts file-like object.
+
         Parameters
         ----------
         fname : str or Path
             Location on disk from which to load the data.
         encoding : str
             Standard used to encode the text into binary formats.
             Default is ``"utf-8"``.
 
         Returns
         -------
         Histogram
             Instance loaded from JSON stored data.
         """
-        fname = Path(fname)
-        if fname.suffix == ".gz":
-            f = gz.open(fname, mode="rt", encoding=encoding)
+        if isinstance(fname, (str, Path)):
+            fname = Path(fname)
+            if fname.suffix == ".gz":
+                f = gz.open(fname, mode="rt", encoding=encoding)
+            else:
+                f = open(fname, encoding=encoding)
         else:
-            f = open(fname, encoding=encoding)
+            f = fname
+            f.seek(0)
         with f:
             data = json.load(f)
         hist = cls(
             data.pop("num_bins"),
             tuple(data.pop("window")),
             data.pop("align"),
             data.pop("expected"),
@@ -698,104 +719,274 @@
 def _pt_size(pt: base.DoubleVector) -> float:
     log_pt = np.log(pt)
     size = (log_pt - np.min(log_pt)) / (np.max(log_pt) - np.min(log_pt))
     size = size + 0.1
     return size
 
 
-def eta_phi_scatter(
+def _iterable_to_momentum(
     pmu: ty.Iterable[ty.Tuple[float, float, float, float]],
+    count: ty.Optional[int] = None,
+) -> gcl.MomentumArray:
+    if isinstance(pmu, gcl.MomentumArray):
+        return pmu
+    kwargs = dict()
+    if count is not None:
+        kwargs["count"] = count
+    if not isinstance(pmu, cla.Sized):
+        pmu = np.fromiter(pmu, dtype=("<f8", 4), **kwargs)
+    return gcl.MomentumArray(pmu)  # type: ignore
+
+
+def _iterable_to_pdg(
     pdg: ty.Iterable[int],
+    count: ty.Optional[int] = None,
+) -> gcl.PdgArray:
+    if isinstance(pdg, gcl.PdgArray):
+        return pdg
+    kwargs = dict()
+    if count is not None:
+        kwargs["count"] = count
+    if not isinstance(pdg, cla.Sized):
+        pdg = np.fromiter(pdg, dtype="<i4", **kwargs)
+    return gcl.PdgArray(pdg)  # type: ignore
+
+
+def eta_phi_scatter(
+    pmu: ty.Iterable[ty.Tuple[float, float, float, float]],
+    pdg: ty.Optional[ty.Iterable[int]] = None,
     masks: ty.Optional[ty.Mapping[str, ty.Iterable[bool]]] = None,
-    eta_max: ty.Optional[float] = 2.5,
-    pt_min: ty.Optional[float] = 0.5,
+    eta_max: ty.Optional[float] = None,
+    pt_min: ty.Optional[float] = None,
     indices: ty.Optional[ty.Iterable[int]] = None,
+    title: ty.Optional[str] = None,
+    pi_units: bool = True,
 ) -> "PlotlyFigure":
     """Produces a scatter plot of particles over the
     :math:`\\eta-\\phi`, *ie.* pseudorapidity-azimuth, plane.
 
     :group: figs
 
     .. versionadded:: 0.2.0
 
+    .. versionchanged:: 0.2.3
+       Added ``pi_units`` and ``title`` parameters. Set defaults for
+       ``eta_max`` and ``pt_min`` as ``None``. Made ``pdg`` an optional
+       parameter.
+
     Parameters
     ----------
     pmu : iterable[tuple[float, float, float, float]]
         Four momenta of particles in basis :math:`(p_x, p_y, p_z, E)`.
-    pdg : iterable[int]
-        PDG particle identification codes.
+    pdg : iterable[int], optional
+        PDG particle identification codes. Default is ``None``.
     masks : mapping[str, iterable[bool]], optional
         Groups particles using key-value pairs, where the values are
         boolean masks identifying members of a group, and the keys are
         used in the plot legend. Default is ``None``.
     eta_max : float, optional
         Maximum cut-off for the pseudorapidity, :math:`\\eta`. Default
-        is ``2.5``.
+        is ``None``.
     pt_min : float, optional
         Minimum cut-off for the transverse momentum, :math:`p_T`.
-        Default is ``0.5``.
+        Default is ``None``.
     indices : iterable[int], optional
         Adds custom data indices to points on scatter plot. Mostly
         useful for keeping track of particles in ``Dash`` callbacks.
         Default is ``None``.
+    title : str, optional
+        Main heading for the figure. Default is ``None``.
+    pi_units : bool
+        If ``True``, will rescale the :math:`\\phi`-axis to range
+        :math:`[-1, 1]`, by putting it in units of :math:`\\pi`. Default
+        is ``True``.
 
     Returns
     -------
     PlotlyFigure
         Interactive scatter plot over the :math:`\\eta-\\phi` plane.
     """
-    if not isinstance(pdg, cla.Sized):
-        pdg = np.fromiter(pdg, dtype="<i4")
-    NUM_PCLS = len(pdg)
-    if not isinstance(pmu, cla.Sized):
-        pmu = np.fromiter(pmu, dtype=("<f8", 4), count=NUM_PCLS)
-    pmu_ = gcl.MomentumArray(pmu)  # type: ignore
-    pdg_ = gcl.PdgArray(pdg)  # type: ignore
+    pmu_ = _iterable_to_momentum(pmu)
+    NUM_PCLS = len(pmu_)
     vis_mask = gcl.MaskGroup(agg_op="and")  # type: ignore
     if eta_max is not None:
         vis_mask["eta"] = np.abs(pmu_.eta) < eta_max
     if pt_min is not None:
         vis_mask["pt"] = pmu_.pt > pt_min
     if len(vis_mask) == 0:
         vis_mask["none"] = np.ones(NUM_PCLS, dtype="<?")
     NUM_VISIBLE = np.sum(vis_mask.data, dtype="<i4")
     vis_pmu = pmu_[vis_mask]
-    vis_pdg = pdg_[vis_mask]
-    df = pd.DataFrame(
-        {
-            "pt": vis_pmu.pt,
-            "eta": vis_pmu.eta,
-            "phi": vis_pmu.phi / np.pi,
-            "name": vis_pdg.name,
-            "size": _pt_size(vis_pmu.pt),
-            "group": np.full(NUM_VISIBLE, "background", dtype=object),
-        }
-    )
+    vis_phi = vis_pmu.phi
+    eta_unit = phi_unit = "(\\text{rad})"
+    if pi_units:
+        vis_phi = vis_phi.copy() / np.pi
+        phi_unit = "(\\pi \\text{ rad})"
+    data_dict = {
+        "pt": vis_pmu.pt,
+        "eta": vis_pmu.eta,
+        "phi": vis_phi,
+        "size": _pt_size(vis_pmu.pt),
+        "group": np.full(NUM_VISIBLE, "background", dtype=object),
+    }
+    if pdg is not None:
+        pdg_ = _iterable_to_pdg(pdg, count=NUM_PCLS)
+        vis_pdg = pdg_[vis_mask]
+        data_dict["name"] = vis_pdg.name
+    df = pd.DataFrame(data_dict)
     if masks is not None:
         for name, mask_ in masks.items():
             group_mask = np.fromiter(mask_, dtype="<?", count=NUM_PCLS)
             vis_group_mask = group_mask[vis_mask]
             df.loc[(vis_group_mask, "group")] = name
     custom_data = []
     if indices is not None:
         indices = np.fromiter(indices, dtype="<i4", count=NUM_PCLS)
         df["indices"] = indices[vis_mask]
         custom_data.append("indices")
     fig = px.scatter(
         df,
         x="eta",
         y="phi",
+        title=title,
         color="group",
         symbol="group",
         size="size",
-        hover_data=["size", "pt", "name"],
+        hover_data=["size", "pt"] + ([] if pdg is None else ["name"]),
         custom_data=custom_data,
     )
-    fig.update_yaxes(title_text=r"$\phi\;\; (\pi \text{ rad})$")
-    fig.update_xaxes(title_text=r"$\eta$")
+    fig.update_yaxes(title_text=f"$\\phi\\;\\; {phi_unit}$")
+    fig.update_xaxes(title_text=f"$\\eta\\;\\; {eta_unit}$")
+    return fig
+
+
+def _edge_pos(
+    pcl_pos: base.DoubleVector, adj: base.BoolVector
+) -> ty.List[ty.Optional[float]]:
+    edges = []
+    for ux, row in zip(pcl_pos, adj):
+        for vx in pcl_pos[row]:
+            edges += [ux, vx, None]
+    return edges
+
+
+def eta_phi_network(
+    pmu: ty.Iterable[ty.Tuple[float, float, float, float]],
+    radius: float,
+    title: ty.Optional[str] = None,
+    color: ty.Optional[ty.Iterable[float]] = None,
+    colorbar_title: ty.Optional[str] = None,
+    marker_symbols: ty.Optional[ty.Iterable[ty.Union[str, int]]] = None,
+    pi_units: bool = True,
+) -> "PlotlyFigure":
+    """Produces a Plotly figure which calculates interparticle distance,
+    and connects particles in a network visualisation when they are
+    within ``radius`` of each other.
+
+    :group: figs
+
+    .. versionadded:: 0.2.3
+
+    Parameters
+    ----------
+    pmu : iterable[tuple[float, float, float, float]]
+        Representing the four-momenta of the particles, in the order
+        :math:`x, y, z, E`. Numpy arrays with four columns, or
+        graphicle ``MomentumArrays`` may be passed.
+    radius : float
+        Interparticle angular distance on the :math:`\\eta-\\phi` plane
+        below which nodes in the network will be considered adjacent.
+    title : str, optional
+        Main heading for the figure. Default is ``None``.
+    color : iterable[float], optional
+        If passed, will add a colorbar to the figure, and the values
+        provided here will be used to define the color of each node.
+        Default is ``None``.
+    colorbar_title : str, optional
+        String label used to annotate the colorbar. Default is ``None``.
+    marker_symbols : iterable[int | str], optional
+        Symbols defining the shape of markers. Must be of same length
+        as ``pmu``. For symbol names / codes, see:
+        https://plotly.com/python/marker-style/#custom-marker-symbols.
+        Default is ``None``.
+    pi_units : bool
+        If ``True``, will rescale the :math:`\\phi`-axis to range
+        :math:`[-1, 1]`, by putting it in units of :math:`\\pi`. Default
+        is ``True``.
+
+    Returns
+    -------
+    PlotlyFigure
+        Plotly figure of particles on the :math:`\\eta-\\phi` plane,
+        with edges connecting adjacent particles, defined by ``radius``.
+    """
+    pmu = _iterable_to_momentum(pmu)
+    NUM_PCLS = len(pmu)
+    layout_opts = dict()
+    if title is not None:
+        layout_opts["title"] = title
+    marker_opts: ty.Dict[str, ty.Any] = dict(size=10, line_width=1)
+    if color is not None:
+        if not isinstance(color, cla.Sized):
+            color = np.fromiter(color, dtype="<f8", count=NUM_PCLS)
+        marker_opts["color"] = color
+        marker_opts["colorbar"] = dict(
+            thickness=15,
+            xanchor="left",
+            titleside="right",
+        )
+        if colorbar_title is not None:
+            marker_opts["colorbar"]["title"] = colorbar_title
+        if marker_symbols is not None:
+            marker_opts["symbol"] = marker_symbols
+    adj_matrix = pmu.delta_R(pmu) < radius
+    eta = pmu.eta
+    phi = pmu.phi
+    eta_unit = phi_unit = "(\\text{rad})"
+    if pi_units:
+        phi = phi.copy() / np.pi
+        phi_unit = "(\\pi \\text{ rad})"
+    eta_edge = _edge_pos(eta, adj_matrix)
+    phi_edge = _edge_pos(phi, adj_matrix)
+    edge_trace = go.Scatter(
+        x=eta_edge,
+        y=phi_edge,
+        line=dict(width=0.5, color="#686a72"),
+        hoverinfo="none",
+        mode="lines",
+        showlegend=False,
+    )
+    node_trace = go.Scatter(
+        x=eta.tolist(),
+        y=phi.tolist(),
+        mode="markers",
+        showlegend=False,
+        marker=marker_opts,
+    )
+    fig = go.Figure(
+        data=[edge_trace, node_trace],
+        layout=go.Layout(
+            titlefont_size=16,
+            hovermode="closest",
+            margin=dict(b=80, l=80, r=80, t=80, pad=0),
+            xaxis=dict(
+                showgrid=True,
+                zeroline=False,
+                showticklabels=True,
+            ),
+            yaxis=dict(
+                showgrid=True,
+                zeroline=False,
+                showticklabels=True,
+            ),
+            **layout_opts,
+        ),
+    )
+    fig.update_yaxes(title_text=f"$\\phi\\;\\; {phi_unit}$")
+    fig.update_xaxes(title_text=f"$\\eta\\;\\; {eta_unit}$")
     return fig
 
 
 def histogram_barchart(
     hist: Histogram,
     hist_label: str,
     title: str = "",
```

### Comparing `colliderscope-0.2.2/colliderscope/__main__.py` & `colliderscope-0.2.3/colliderscope/__main__.py`

 * *Files identical despite different names*

### Comparing `colliderscope-0.2.2/colliderscope/base.py` & `colliderscope-0.2.3/colliderscope/base.py`

 * *Files identical despite different names*

### Comparing `colliderscope-0.2.2/colliderscope/webui.py` & `colliderscope-0.2.3/colliderscope/webui.py`

 * *Files identical despite different names*

### Comparing `colliderscope-0.2.2/colliderscope.egg-info/PKG-INFO` & `colliderscope-0.2.3/colliderscope.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: colliderscope
-Version: 0.2.2
+Version: 0.2.3
 Summary: Plotting tools for Monte-Carlo particle showers.
 Author: Jacan Chaplais
 Maintainer: Jacan Chaplais
 License: BSD 3-Clause License
         
         Copyright (c) 2021, Jacan Chaplais.
         All rights reserved.
```

### Comparing `colliderscope-0.2.2/colliderscope.egg-info/SOURCES.txt` & `colliderscope-0.2.3/colliderscope.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `colliderscope-0.2.2/docs/Makefile` & `colliderscope-0.2.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `colliderscope-0.2.2/docs/make.bat` & `colliderscope-0.2.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `colliderscope-0.2.2/docs/source/api.rst` & `colliderscope-0.2.3/docs/source/api.rst`

 * *Files identical despite different names*

### Comparing `colliderscope-0.2.2/docs/source/cli.rst` & `colliderscope-0.2.3/docs/source/cli.rst`

 * *Files identical despite different names*

### Comparing `colliderscope-0.2.2/docs/source/conf.py` & `colliderscope-0.2.3/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `colliderscope-0.2.2/pyproject.toml` & `colliderscope-0.2.3/pyproject.toml`

 * *Files identical despite different names*

