# Comparing `tmp/aeppl-0.1.3.tar.gz` & `tmp/aeppl-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aeppl-0.1.3.tar", last modified: Sat Mar 11 04:12:39 2023, max compression
+gzip compressed data, was "aeppl-0.1.4.tar", last modified: Sat May  6 06:32:48 2023, max compression
```

## Comparing `aeppl-0.1.3.tar` & `aeppl-0.1.4.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 04:12:39.126389 aeppl-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-03-11 04:12:36.000000 aeppl-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-03-11 04:12:36.000000 aeppl-0.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-03-11 04:12:39.126389 aeppl-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5451 2023-03-11 04:12:36.000000 aeppl-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 04:12:39.126389 aeppl-0.1.3/aeppl/
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-03-11 04:12:36.000000 aeppl-0.1.3/aeppl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-03-11 04:12:39.126389 aeppl-0.1.3/aeppl/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-03-11 04:12:36.000000 aeppl-0.1.3/aeppl/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     8455 2023-03-11 04:12:36.000000 aeppl-0.1.3/aeppl/censoring.py
--rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-03-11 04:12:36.000000 aeppl-0.1.3/aeppl/cumsum.py
--rw-r--r--   0 runner    (1001) docker     (123)     8667 2023-03-11 04:12:36.000000 aeppl-0.1.3/aeppl/dists.py
--rw-r--r--   0 runner    (1001) docker     (123)    11572 2023-03-11 04:12:36.000000 aeppl-0.1.3/aeppl/joint_logprob.py
--rw-r--r--   0 runner    (1001) docker     (123)    21265 2023-03-11 04:12:36.000000 aeppl-0.1.3/aeppl/logprob.py
--rw-r--r--   0 runner    (1001) docker     (123)    15197 2023-03-11 04:12:36.000000 aeppl-0.1.3/aeppl/mixture.py
--rw-r--r--   0 runner    (1001) docker     (123)    24329 2023-03-11 04:12:36.000000 aeppl-0.1.3/aeppl/printing.py
--rw-r--r--   0 runner    (1001) docker     (123)    11398 2023-03-11 04:12:36.000000 aeppl-0.1.3/aeppl/rewriting.py
--rw-r--r--   0 runner    (1001) docker     (123)    21143 2023-03-11 04:12:36.000000 aeppl-0.1.3/aeppl/scan.py
--rw-r--r--   0 runner    (1001) docker     (123)     7038 2023-03-11 04:12:36.000000 aeppl-0.1.3/aeppl/tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)    30620 2023-03-11 04:12:36.000000 aeppl-0.1.3/aeppl/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     7859 2023-03-11 04:12:36.000000 aeppl-0.1.3/aeppl/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 04:12:39.126389 aeppl-0.1.3/aeppl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-03-11 04:12:39.000000 aeppl-0.1.3/aeppl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-03-11 04:12:39.000000 aeppl-0.1.3/aeppl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-11 04:12:39.000000 aeppl-0.1.3/aeppl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-11 04:12:39.000000 aeppl-0.1.3/aeppl.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-03-11 04:12:39.000000 aeppl-0.1.3/aeppl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-11 04:12:39.000000 aeppl-0.1.3/aeppl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-03-11 04:12:39.126389 aeppl-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-03-11 04:12:36.000000 aeppl-0.1.3/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    70144 2023-03-11 04:12:36.000000 aeppl-0.1.3/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 06:32:48.425737 aeppl-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-06 06:32:43.000000 aeppl-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-06 06:32:43.000000 aeppl-0.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-05-06 06:32:48.425737 aeppl-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5534 2023-05-06 06:32:43.000000 aeppl-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 06:32:48.425737 aeppl-0.1.4/aeppl/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-06 06:32:43.000000 aeppl-0.1.4/aeppl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-06 06:32:48.425737 aeppl-0.1.4/aeppl/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-05-06 06:32:43.000000 aeppl-0.1.4/aeppl/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8455 2023-05-06 06:32:43.000000 aeppl-0.1.4/aeppl/censoring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-05-06 06:32:43.000000 aeppl-0.1.4/aeppl/convolutions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-05-06 06:32:43.000000 aeppl-0.1.4/aeppl/cumsum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8667 2023-05-06 06:32:43.000000 aeppl-0.1.4/aeppl/dists.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11349 2023-05-06 06:32:43.000000 aeppl-0.1.4/aeppl/joint_logprob.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21265 2023-05-06 06:32:43.000000 aeppl-0.1.4/aeppl/logprob.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15197 2023-05-06 06:32:43.000000 aeppl-0.1.4/aeppl/mixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24329 2023-05-06 06:32:43.000000 aeppl-0.1.4/aeppl/printing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11894 2023-05-06 06:32:43.000000 aeppl-0.1.4/aeppl/rewriting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21143 2023-05-06 06:32:43.000000 aeppl-0.1.4/aeppl/scan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7038 2023-05-06 06:32:43.000000 aeppl-0.1.4/aeppl/tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30605 2023-05-06 06:32:43.000000 aeppl-0.1.4/aeppl/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7859 2023-05-06 06:32:43.000000 aeppl-0.1.4/aeppl/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 06:32:48.425737 aeppl-0.1.4/aeppl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-05-06 06:32:48.000000 aeppl-0.1.4/aeppl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-05-06 06:32:48.000000 aeppl-0.1.4/aeppl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 06:32:48.000000 aeppl-0.1.4/aeppl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 06:32:48.000000 aeppl-0.1.4/aeppl.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-06 06:32:48.000000 aeppl-0.1.4/aeppl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-06 06:32:48.000000 aeppl-0.1.4/aeppl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-05-06 06:32:48.425737 aeppl-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-05-06 06:32:43.000000 aeppl-0.1.4/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70144 2023-05-06 06:32:43.000000 aeppl-0.1.4/versioneer.py
```

### Comparing `aeppl-0.1.3/LICENSE` & `aeppl-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `aeppl-0.1.3/PKG-INFO` & `aeppl-0.1.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aeppl
-Version: 0.1.3
+Version: 0.1.4
 Summary: PPL tools for Aesara
 Home-page: https://github.com/aesara-devs/aeppl
 Author: aesara-devs
 Author-email: aesara.devs@gmail.com
 License: UNKNOWN
 Description: UNKNOWN
 Keywords: aeppl,math,probability,symbolic,probabilistic programming
```

### Comparing `aeppl-0.1.3/README.md` & `aeppl-0.1.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 <div align="center">
 
+<img src="./docs/source/_static/aeppl_logo.png" alt="AePPL Logo" width=400></img>
+
 # AePPL
 
 [![Pypi][pypi-badge]][pypi]
 [![Downloads][downloads-badge]][releases]
 [![Contributors][contributors-badge]][contributors]
  </br>
 [![Gitter][gitter-badge]][gitter]
```

### Comparing `aeppl-0.1.3/aeppl/abstract.py` & `aeppl-0.1.4/aeppl/abstract.py`

 * *Files identical despite different names*

### Comparing `aeppl-0.1.3/aeppl/censoring.py` & `aeppl-0.1.4/aeppl/censoring.py`

 * *Files identical despite different names*

### Comparing `aeppl-0.1.3/aeppl/cumsum.py` & `aeppl-0.1.4/aeppl/cumsum.py`

 * *Files identical despite different names*

### Comparing `aeppl-0.1.3/aeppl/dists.py` & `aeppl-0.1.4/aeppl/dists.py`

 * *Files identical despite different names*

### Comparing `aeppl-0.1.3/aeppl/joint_logprob.py` & `aeppl-0.1.4/aeppl/joint_logprob.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,43 +137,37 @@
         original_rv_values[rv] = vv
 
     # Value variables are not cloned when constructing the conditional log-probability
     # graphs. We can thus use them to recover the original random variables to index the
     # maps to the logprob graphs and value variables before returning them.
     rv_values = {**original_rv_values, **realized}
 
-    fgraph, _, memo = construct_ir_fgraph(rv_values, ir_rewriter=ir_rewriter)
-
-    if extra_rewrites is not None:
-        extra_rewrites.add_requirements(fgraph, rv_values, memo)
-        extra_rewrites.apply(fgraph)
+    fgraph, new_rv_values = construct_ir_fgraph(
+        rv_values, ir_rewriter=ir_rewriter, extra_rewrites=extra_rewrites
+    )
 
     # We assign log-densities on a per-node basis, and not per-output/variable.
     realized_vars = set()
     new_to_old_rvs = {}
     nodes_to_vals: Dict["Apply", List[Tuple["Variable", "Variable"]]] = {}
 
-    for bnd_var, (old_mvar, old_val) in zip(fgraph.outputs, rv_values.items()):
+    for bnd_var, (old_mvar, val) in zip(fgraph.outputs, new_rv_values.items()):
         mnode = bnd_var.owner
         assert mnode and isinstance(mnode.op, ValuedVariable)
 
         rv_var, val_var = mnode.inputs
         rv_node = rv_var.owner
 
         if rv_node is None:
             raise DensityNotFound(f"Couldn't derive a log-probability for {rv_var}")
 
         if old_mvar in realized:
             realized_vars.add(rv_var)
 
-        # Do this just in case a value variable was changed.  (Some transforms
-        # do this.)
-        new_val = memo[old_val]
-
-        nodes_to_vals.setdefault(rv_node, []).append((val_var, new_val))
+        nodes_to_vals.setdefault(rv_node, []).append((val_var, val))
 
         new_to_old_rvs[rv_var] = old_mvar
 
     value_vars: Tuple["Variable", ...] = ()
     logprob_vars = {}
 
     for rv_node, rv_val_pairs in nodes_to_vals.items():
```

### Comparing `aeppl-0.1.3/aeppl/logprob.py` & `aeppl-0.1.4/aeppl/logprob.py`

 * *Files identical despite different names*

### Comparing `aeppl-0.1.3/aeppl/mixture.py` & `aeppl-0.1.4/aeppl/mixture.py`

 * *Files identical despite different names*

### Comparing `aeppl-0.1.3/aeppl/printing.py` & `aeppl-0.1.4/aeppl/printing.py`

 * *Files identical despite different names*

### Comparing `aeppl-0.1.3/aeppl/rewriting.py` & `aeppl-0.1.4/aeppl/rewriting.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,20 @@
-from typing import Dict, Optional, Tuple
+from typing import Dict, Optional, Tuple, Union
 
 import aesara.tensor as at
 from aesara.compile.mode import optdb
 from aesara.graph.basic import Apply, Variable
 from aesara.graph.features import Feature
 from aesara.graph.fg import FunctionGraph
-from aesara.graph.rewriting.basic import GraphRewriter, in2out, node_rewriter
+from aesara.graph.rewriting.basic import (
+    GraphRewriter,
+    NodeRewriter,
+    in2out,
+    node_rewriter,
+)
 from aesara.graph.rewriting.db import EquilibriumDB, RewriteDatabaseQuery, SequenceDB
 from aesara.tensor.elemwise import DimShuffle, Elemwise
 from aesara.tensor.extra_ops import BroadcastTo
 from aesara.tensor.random.rewriting import local_subtensor_rv_lift
 from aesara.tensor.rewriting.basic import register_canonicalize, register_useless
 from aesara.tensor.rewriting.shape import ShapeFeature
 from aesara.tensor.subtensor import (
@@ -176,17 +181,18 @@
     "incsubtensor_lift", incsubtensor_rv_replace, "basic"
 )
 
 logprob_rewrites_db.register("post-canonicalize", optdb.query("+canonicalize"), "basic")
 
 
 def construct_ir_fgraph(
-    rv_values: Dict[Variable, Variable],
+    rvs_to_values: Dict[Variable, Variable],
     ir_rewriter: Optional[GraphRewriter] = None,
-) -> Tuple[FunctionGraph, Dict[Variable, Variable], Dict[Variable, Variable]]:
+    extra_rewrites: Optional[Union[GraphRewriter, NodeRewriter]] = None,
+) -> Tuple[FunctionGraph, Dict[Variable, Variable]]:
     r"""Construct a `FunctionGraph` in measurable IR form for the keys in `rv_values`.
 
     A custom IR rewriter can be specified. By default,
     ``logprob_rewrites_db.query(RewriteDatabaseQuery(include=["basic"]))`` is used.
 
     Our measurable IR takes the form of an Aesara graph that is more-or-less
     equivalent to a given Aesara graph (i.e. the keys of `rv_values`) but
@@ -211,17 +217,16 @@
     this IR, and the resulting graphs will not be computationally sound,
     because they wouldn't produce independent samples when the original graph
     would.  See https://github.com/aesara-devs/aeppl/pull/78.
 
     Returns
     -------
     A `FunctionGraph` of the measurable IR, a copy of `rv_values` containing
-    the new, cloned versions of the original variables in `rv_values`, and
-    a ``dict`` mapping all the original variables to their cloned values in
-    the `FunctionGraph`.
+    the new, cloned versions of the original variables in `rv_values`.
+
     """
 
     # We're going to create a `FunctionGraph` that effectively represents the
     # joint log-probability of all the random variables assigned values in
     # `rv_values`.
     # The `FunctionGraph`'s outputs will be `ValuedVariable`s.  This serves to
     # associate a random variable with its value and facilitate
@@ -229,58 +234,70 @@
     # The `FunctionGraph` will be transformed by rewrites so that
     # log-probabilities can be assigned to/derived for its outputs.
 
     # We clone the random variables that we'll use as `FunctionGraph` outputs
     # so that they're distinct nodes in the graph.  This allows us to replace
     # all instances of the original random variables with their value
     # variables, while leaving the output clones untouched.
-    rv_value_clones = {}
+    rv_clone_to_value_clone = {}
+    rv_to_value_clone = {}
+    value_clone_to_value = {}
     measured_outputs = {}
-    memo = {}
-    for rv, val in rv_values.items():
+    memo: Dict[Variable, Variable] = {}
+    for rv, val in rvs_to_values.items():
         rv_node_clone = rv.owner.clone()
         rv_clone = rv_node_clone.outputs[rv.owner.outputs.index(rv)]
-        rv_value_clones[rv_clone] = val
-        measured_outputs[rv] = valued_variable(rv_clone, val)
-        # Prevent value variables from being cloned
-        memo[val] = val
+        val_clone = val.clone()
+        val_clone.name = "val_clone"
+        rv_clone_to_value_clone[rv_clone] = val_clone
+        rv_to_value_clone[rv] = val_clone
+        value_clone_to_value[val_clone] = val
+        measured_outputs[rv] = valued_variable(rv_clone, val_clone)
 
     # We add `ShapeFeature` because it will get rid of references to the old
     # `RandomVariable`s that have been lifted; otherwise, it will be difficult
     # to give good warnings when an unaccounted for `RandomVariable` is
     # encountered
     fgraph = FunctionGraph(
         outputs=tuple(measured_outputs.values()),
         features=[ShapeFeature(), MeasurableConversionTracker()],
         clone=True,
         memo=memo,
         copy_orphans=False,
         copy_inputs=False,
     )
 
-    # Update `rv_values` so that it uses the new cloned variables
-    rv_value_clones = {memo[k]: v for k, v in rv_value_clones.items()}
-
     # Replace valued non-output variables with their values
     fgraph.replace_all(
         [(memo[rv], val) for rv, val in measured_outputs.items() if rv in memo],
         reason="valued-non-outputs-replace",
         import_missing=True,
     )
 
     if ir_rewriter is None:
         ir_rewriter = logprob_rewrites_db.query(RewriteDatabaseQuery(include=["basic"]))
 
     ir_rewriter.rewrite(fgraph)
 
+    if extra_rewrites is not None:
+        # Expect `value_clone_to_value` to be updated in-place
+        extra_rewrites.add_requirements(fgraph, rv_to_value_clone, value_clone_to_value)
+        extra_rewrites.apply(fgraph)
+
     # Undo un-valued measurable IR rewrites
     new_to_old = tuple((v, k) for k, v in fgraph.measurable_conversions.items())
-    fgraph.replace_all(new_to_old, reason="undo-unvalued-measurables")
+    # and add the original value variables back in
+    new_to_old += tuple(value_clone_to_value.items())
+    fgraph.replace_all(
+        new_to_old, reason="undo-unvalued-measurables", import_missing=True
+    )
+
+    new_rvs_to_values = dict(zip(rvs_to_values.keys(), value_clone_to_value.values()))
 
-    return fgraph, rv_value_clones, memo
+    return fgraph, new_rvs_to_values
 
 
 @register_useless
 @node_rewriter([ValuedVariable])
 def remove_ValuedVariable(fgraph, node):
     return [node.inputs[1]]
```

### Comparing `aeppl-0.1.3/aeppl/scan.py` & `aeppl-0.1.4/aeppl/scan.py`

 * *Files identical despite different names*

### Comparing `aeppl-0.1.3/aeppl/tensor.py` & `aeppl-0.1.4/aeppl/tensor.py`

 * *Files identical despite different names*

### Comparing `aeppl-0.1.3/aeppl/transforms.py` & `aeppl-0.1.4/aeppl/transforms.py`

 * *Files 1% similar despite different names*

```diff
@@ -157,22 +157,18 @@
     "backward"-transform of a new value variable in the "forward"-transformed
     space.
     3. Signify that the original value variable is to be replaced by the new
     one.
     4. Replace the old `ValuedVariable` with a new one containing a
     `TransformedVariable` value.
 
-    Step 3. is currently accomplished by updating the `memo` dictionary
-    associated with the `FunctionGraph`.  Our main entry-point,
+    Step 3. is currently accomplished by updating the `rvs_to_values`
+    dictionary associated with the `FunctionGraph`.  Our main entry-point,
     `conditional_logprob`, checks this dictionary for value variable changes.
 
-    TODO: This approach is less than ideal, because it puts awkward demands on
-    users/callers of this rewrite to check with `memo`; let's see if we can do
-    something better.
-
     The new value variable mentioned in Step 2. may be of a different `Type`
     (e.g. extra/fewer dimensions) than the original value variable; this is why
     we must replace the corresponding original value variables before we
     construct log-probability graphs.  This is due to the fact that we
     generally cannot replace variables with new ones that have different
     `Type`\s.
 
@@ -231,16 +227,16 @@
     # with "inversely/un-" transformed versions of themselves.
     untrans_value_var = transformed_variable(
         transform.backward(trans_value_var, *trans_node.inputs), trans_value_var
     )
 
     # This effectively lets the caller know that a value variable has been
     # replaced (i.e. they should filter all their old value variables through
-    # the memo/replacements map).
-    fgraph.memo[value_var] = trans_value_var
+    # the replacements map).
+    fgraph.value_clone_to_value[value_var] = trans_value_var
 
     trans_var = trans_node.outputs[rv_var_out_idx]
     new_var = valued_variable(trans_var, untrans_value_var)
 
     return {value_var: untrans_value_var, node.outputs[0]: new_var}
 
 
@@ -248,37 +244,36 @@
     r"""A `Feature` that maintains a map between value variables and their transforms as
     well as between value variables and their transformed counterparts.
 
     This is exclusively/primarily used by `TransformValuesRewrite`.
 
     """
 
-    def __init__(self, values_to_transforms, memo):
+    def __init__(self, values_to_transforms, value_clone_to_value):
         """
         Parameters
         ==========
         values_to_transforms
             Mapping between value variables and their transformations. Each
             value variable can be assigned one of `RVTransform`,
             `DEFAULT_TRANSFORM`, or ``None``. Random variables with no
             transform specified remain unchanged.
-        memo
-            Mapping from variables to their clones.  This is updated
-            in-place whenever a value variable is transformed.
-
+        value_clone_to_value
+            Mapping between random variable value clones and their original
+            value variables.
         """
         self.values_to_transforms = values_to_transforms
-        self.memo = memo
+        self.value_clone_to_value = value_clone_to_value
 
     def on_attach(self, fgraph):
         if hasattr(fgraph, "values_to_transforms"):
             raise AlreadyThere()
 
         fgraph.values_to_transforms = self.values_to_transforms
-        fgraph.memo = self.memo
+        fgraph.value_clone_to_value = self.value_clone_to_value
 
 
 class TransformValuesRewrite(GraphRewriter):
     r"""Transforms measurable variables.
 
     This transformation can be used to replace all occurrences of a measurable
     variable and its values within a model graph with a transformed version of
@@ -318,30 +313,33 @@
         Parameters
         ==========
         rvs_to_transforms
             Mapping between measurable variables and their transformations. Each
             measurable variable can be assigned an `RVTransform` instance,
             `DEFAULT_TRANSFORM`, or ``None``. Measurable variables with no
             transform specified remain unchanged.
+        rvs_to_values
 
         """
 
         self.rvs_to_transforms = rvs_to_transforms
 
     def add_requirements(
         self,
         fgraph,
-        rv_to_values: Dict[TensorVariable, TensorVariable],
-        memo: Dict[TensorVariable, TensorVariable],
+        rvs_to_values: Dict[TensorVariable, TensorVariable],
+        value_clone_to_value: Dict[TensorVariable, TensorVariable],
     ):
         values_to_transforms = {
-            rv_to_values[rv]: transform
+            rvs_to_values[rv]: transform
             for rv, transform in self.rvs_to_transforms.items()
         }
-        values_transforms_feature = TransformValuesMapping(values_to_transforms, memo)
+        values_transforms_feature = TransformValuesMapping(
+            values_to_transforms, value_clone_to_value
+        )
         fgraph.attach_feature(values_transforms_feature)
 
     def apply(self, fgraph: FunctionGraph):
         return self.default_transform_rewrite.rewrite(fgraph)
 
 
 class MeasurableElemwiseTransform(MeasurableElemwise):
```

### Comparing `aeppl-0.1.3/aeppl/utils.py` & `aeppl-0.1.4/aeppl/utils.py`

 * *Files identical despite different names*

### Comparing `aeppl-0.1.3/aeppl.egg-info/PKG-INFO` & `aeppl-0.1.4/aeppl.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aeppl
-Version: 0.1.3
+Version: 0.1.4
 Summary: PPL tools for Aesara
 Home-page: https://github.com/aesara-devs/aeppl
 Author: aesara-devs
 Author-email: aesara.devs@gmail.com
 License: UNKNOWN
 Description: UNKNOWN
 Keywords: aeppl,math,probability,symbolic,probabilistic programming
```

### Comparing `aeppl-0.1.3/setup.cfg` & `aeppl-0.1.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `aeppl-0.1.3/setup.py` & `aeppl-0.1.4/setup.py`

 * *Files identical despite different names*

### Comparing `aeppl-0.1.3/versioneer.py` & `aeppl-0.1.4/versioneer.py`

 * *Files identical despite different names*

