# Comparing `tmp/kartograf-0.0.3.tar.gz` & `tmp/kartograf-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kartograf-0.0.3.tar", last modified: Fri Feb 24 19:24:23 2023, max compression
+gzip compressed data, was "kartograf-0.0.6.tar", last modified: Fri May  5 21:47:16 2023, max compression
```

## Comparing `kartograf-0.0.3.tar` & `kartograf-0.0.6.tar`

### file list

```diff
@@ -1,27 +1,25 @@
-drwxrwxr-x   0 mmh       (1000) mmh       (1000)        0 2023-02-24 19:24:23.931560 kartograf-0.0.3/
--rw-rw-r--   0 mmh       (1000) mmh       (1000)     1073 2023-02-22 20:28:15.000000 kartograf-0.0.3/LICENSE
--rw-rw-r--   0 mmh       (1000) mmh       (1000)     1356 2023-02-24 19:24:23.931560 kartograf-0.0.3/PKG-INFO
--rw-rw-r--   0 mmh       (1000) mmh       (1000)      711 2023-02-22 20:28:15.000000 kartograf-0.0.3/README.md
--rw-rw-r--   0 mmh       (1000) mmh       (1000)     1273 2023-02-24 19:20:23.000000 kartograf-0.0.3/pyproject.toml
--rw-rw-r--   0 mmh       (1000) mmh       (1000)       38 2023-02-24 19:24:23.931560 kartograf-0.0.3/setup.cfg
-drwxrwxr-x   0 mmh       (1000) mmh       (1000)        0 2023-02-24 19:24:23.931560 kartograf-0.0.3/src/
-drwxrwxr-x   0 mmh       (1000) mmh       (1000)        0 2023-02-24 19:24:23.931560 kartograf-0.0.3/src/kartograf/
--rw-rw-r--   0 mmh       (1000) mmh       (1000)      166 2023-02-24 19:20:23.000000 kartograf-0.0.3/src/kartograf/__init__.py
--rw-rw-r--   0 mmh       (1000) mmh       (1000)       22 2023-02-24 19:24:23.000000 kartograf-0.0.3/src/kartograf/_version.py
-drwxrwxr-x   0 mmh       (1000) mmh       (1000)        0 2023-02-24 19:24:23.931560 kartograf-0.0.3/src/kartograf/atom_mapping/
--rw-rw-r--   0 mmh       (1000) mmh       (1000)       48 2023-02-22 20:28:15.000000 kartograf-0.0.3/src/kartograf/atom_mapping/__init__.py
--rw-rw-r--   0 mmh       (1000) mmh       (1000)     1358 2023-02-22 20:28:15.000000 kartograf-0.0.3/src/kartograf/atom_mapping/geom_align.py
--rw-rw-r--   0 mmh       (1000) mmh       (1000)    20626 2023-02-22 20:28:15.000000 kartograf-0.0.3/src/kartograf/atom_mapping/geom_mapper.py
--rw-rw-r--   0 mmh       (1000) mmh       (1000)     4655 2023-02-22 20:28:15.000000 kartograf-0.0.3/src/kartograf/atom_mapping/geom_scorer.py
-drwxrwxr-x   0 mmh       (1000) mmh       (1000)        0 2023-02-24 19:24:23.931560 kartograf-0.0.3/src/kartograf/networks/
--rw-rw-r--   0 mmh       (1000) mmh       (1000)      114 2023-02-22 20:28:15.000000 kartograf-0.0.3/src/kartograf/networks/__init__.py
--rw-rw-r--   0 mmh       (1000) mmh       (1000)     2205 2023-02-22 20:28:15.000000 kartograf-0.0.3/src/kartograf/networks/mst_networker.py
--rw-rw-r--   0 mmh       (1000) mmh       (1000)     2507 2023-02-22 20:28:15.000000 kartograf-0.0.3/src/kartograf/networks/radial_networker.py
-drwxrwxr-x   0 mmh       (1000) mmh       (1000)        0 2023-02-24 19:24:23.931560 kartograf-0.0.3/src/kartograf/tests/
--rw-rw-r--   0 mmh       (1000) mmh       (1000)     1159 2023-02-22 20:28:15.000000 kartograf-0.0.3/src/kartograf/tests/test_geom_mapper.py
-drwxrwxr-x   0 mmh       (1000) mmh       (1000)        0 2023-02-24 19:24:23.931560 kartograf-0.0.3/src/kartograf.egg-info/
--rw-rw-r--   0 mmh       (1000) mmh       (1000)     1356 2023-02-24 19:24:23.000000 kartograf-0.0.3/src/kartograf.egg-info/PKG-INFO
--rw-rw-r--   0 mmh       (1000) mmh       (1000)      590 2023-02-24 19:24:23.000000 kartograf-0.0.3/src/kartograf.egg-info/SOURCES.txt
--rw-rw-r--   0 mmh       (1000) mmh       (1000)        1 2023-02-24 19:24:23.000000 kartograf-0.0.3/src/kartograf.egg-info/dependency_links.txt
--rw-rw-r--   0 mmh       (1000) mmh       (1000)       27 2023-02-24 19:24:23.000000 kartograf-0.0.3/src/kartograf.egg-info/requires.txt
--rw-rw-r--   0 mmh       (1000) mmh       (1000)       10 2023-02-24 19:24:23.000000 kartograf-0.0.3/src/kartograf.egg-info/top_level.txt
+drwxr-xr-x   0 bries     (1000) bries     (1000)        0 2023-05-05 21:47:16.739968 kartograf-0.0.6/
+-rw-r--r--   0 bries     (1000) bries     (1000)     1073 2023-02-03 06:44:21.000000 kartograf-0.0.6/LICENSE
+-rw-r--r--   0 bries     (1000) bries     (1000)     3268 2023-05-05 21:47:16.739968 kartograf-0.0.6/PKG-INFO
+-rw-r--r--   0 bries     (1000) bries     (1000)     2648 2023-05-05 20:51:44.000000 kartograf-0.0.6/README.md
+-rw-r--r--   0 bries     (1000) bries     (1000)     1366 2023-05-05 16:51:56.000000 kartograf-0.0.6/pyproject.toml
+-rw-r--r--   0 bries     (1000) bries     (1000)       38 2023-05-05 21:47:16.739968 kartograf-0.0.6/setup.cfg
+drwxr-xr-x   0 bries     (1000) bries     (1000)        0 2023-05-05 21:47:16.739968 kartograf-0.0.6/src/
+drwxr-xr-x   0 bries     (1000) bries     (1000)        0 2023-05-05 21:47:16.739968 kartograf-0.0.6/src/kartograf/
+-rw-r--r--   0 bries     (1000) bries     (1000)      239 2023-05-05 16:51:56.000000 kartograf-0.0.6/src/kartograf/__init__.py
+-rw-r--r--   0 bries     (1000) bries     (1000)       22 2023-05-05 21:47:16.000000 kartograf-0.0.6/src/kartograf/_version.py
+-rw-r--r--   0 bries     (1000) bries     (1000)     2348 2023-05-05 16:51:56.000000 kartograf-0.0.6/src/kartograf/atom_align.py
+-rw-r--r--   0 bries     (1000) bries     (1000)    21050 2023-05-05 21:44:58.000000 kartograf-0.0.6/src/kartograf/atom_mapper.py
+-rw-r--r--   0 bries     (1000) bries     (1000)    13007 2023-05-05 16:51:56.000000 kartograf-0.0.6/src/kartograf/atom_mapping_scorer.py
+drwxr-xr-x   0 bries     (1000) bries     (1000)        0 2023-05-05 21:47:16.739968 kartograf-0.0.6/src/kartograf/tests/
+-rw-r--r--   0 bries     (1000) bries     (1000)        0 2023-04-06 16:28:36.000000 kartograf-0.0.6/src/kartograf/tests/__init__.py
+-rw-r--r--   0 bries     (1000) bries     (1000)     2605 2023-05-05 16:51:56.000000 kartograf-0.0.6/src/kartograf/tests/conf.py
+-rw-r--r--   0 bries     (1000) bries     (1000)      652 2023-05-05 16:51:56.000000 kartograf-0.0.6/src/kartograf/tests/test_atom_align.py
+-rw-r--r--   0 bries     (1000) bries     (1000)     3842 2023-04-07 22:20:12.000000 kartograf-0.0.6/src/kartograf/tests/test_atom_mapper.py
+-rw-r--r--   0 bries     (1000) bries     (1000)     3105 2023-05-05 16:51:56.000000 kartograf-0.0.6/src/kartograf/tests/test_atom_mapping_scorer.py
+drwxr-xr-x   0 bries     (1000) bries     (1000)        0 2023-05-05 21:47:16.739968 kartograf-0.0.6/src/kartograf.egg-info/
+-rw-r--r--   0 bries     (1000) bries     (1000)     3268 2023-05-05 21:47:16.000000 kartograf-0.0.6/src/kartograf.egg-info/PKG-INFO
+-rw-r--r--   0 bries     (1000) bries     (1000)      549 2023-05-05 21:47:16.000000 kartograf-0.0.6/src/kartograf.egg-info/SOURCES.txt
+-rw-r--r--   0 bries     (1000) bries     (1000)        1 2023-05-05 21:47:16.000000 kartograf-0.0.6/src/kartograf.egg-info/dependency_links.txt
+-rw-r--r--   0 bries     (1000) bries     (1000)       23 2023-05-05 21:47:16.000000 kartograf-0.0.6/src/kartograf.egg-info/requires.txt
+-rw-r--r--   0 bries     (1000) bries     (1000)       10 2023-05-05 21:47:16.000000 kartograf-0.0.6/src/kartograf.egg-info/top_level.txt
```

### Comparing `kartograf-0.0.3/LICENSE` & `kartograf-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `kartograf-0.0.3/pyproject.toml` & `kartograf-0.0.6/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,50 +1,50 @@
-[build-system]
-requires=[
-	"setuptools>=61.0",
-	"versioningit",
-]
-build-backend = "setuptools.build_meta"
-
-[project]
-name = "kartograf"
-dynamic = ["version"]
-authors=[
-    {name="Benjamin Ries", email="benjamin-ries@outlook.com"},
-    {name="David Swenson", email="dwhswenson@gmail.com"},
-    {name="Irfan Alibay", email="irfan.alibay@gmail.com"},
-    {name="Mike Henry", email="mike.henry@choderalab.org"},
-    {name="Richard J Gowers", email="richardjgowers@gmail.com"},
-]
-dependencies = [
-  'rdkit',
-  'scipy',
-  'numpy',
-  'networkx',
-]
-description="Kartograf is an package for a setting up free energy calculation."
-readme="README.md"
-requires-python = ">=3.9"
-classifiers = [
-    "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
-]
-
-[project.urls]
-"Homepage" = "https://github.com/OpenFreeEnergy/kartograf"
-
-[tool.versioningit]
-default-version = "1+unknown"
-
-[tool.versioningit.format]
-distance = "{base_version}+{distance}.{vcs}{rev}"
-dirty = "{base_version}+{distance}.{vcs}{rev}.dirty"
-distance-dirty = "{base_version}+{distance}.{vcs}{rev}.dirty"
-
-[tool.versioningit.vcs]
-method = "git" 
-match = ["*"]
-default-tag = "0.0.0"
-
-[tool.versioningit.write]
-file = "src/kartograf/_version.py"
+[build-system]
+requires=[
+	"setuptools>=61.0",
+	"versioningit",
+]
+build-backend = "setuptools.build_meta"
+
+[project]
+name = "kartograf"
+dynamic = ["version"]
+authors=[
+    {name="Benjamin Ries", email="benjamin-ries@outlook.com"},
+    {name="David Swenson", email="dwhswenson@gmail.com"},
+    {name="Irfan Alibay", email="irfan.alibay@gmail.com"},
+    {name="Mike Henry", email="mike.henry@choderalab.org"},
+    {name="Richard J Gowers", email="richardjgowers@gmail.com"},
+]
+dependencies = [
+  'rdkit',
+  'scipy',
+  'numpy',
+  'gufe',
+]
+description="Kartograf is a package for mapping geometrically atoms of two molecules. (like you need it with hybrid topology)"
+readme="README.md"
+requires-python = ">=3.9"
+classifiers = [
+    "Programming Language :: Python :: 3",
+    "License :: OSI Approved :: MIT License",
+    "Operating System :: OS Independent",
+]
+
+[project.urls]
+"Homepage" = "https://github.com/OpenFreeEnergy/kartograf"
+
+[tool.versioningit]
+default-version = "1+unknown"
+
+[tool.versioningit.format]
+distance = "{base_version}+{distance}.{vcs}{rev}"
+dirty = "{base_version}+{distance}.{vcs}{rev}.dirty"
+distance-dirty = "{base_version}+{distance}.{vcs}{rev}.dirty"
+
+[tool.versioningit.vcs]
+method = "git" 
+match = ["*"]
+default-tag = "0.0.0"
+
+[tool.versioningit.write]
+file = "src/kartograf/_version.py"
```

### Comparing `kartograf-0.0.3/src/kartograf/atom_mapping/geom_align.py` & `kartograf-0.0.6/src/kartograf/atom_align.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,61 +1,94 @@
-from copy import deepcopy
-
-from rdkit import Chem
-from rdkit.Chem import rdFMCS
-from rdkit.Chem import AllChem
-
-from gufe import SmallMoleculeComponent
-
-import logging
-
-log = logging.getLogger(__name__)
-
-
-def align_mol_sceletons(
-    mol: SmallMoleculeComponent,
-    ref_mol: SmallMoleculeComponent,
-) -> SmallMoleculeComponent:
-    """
-        Aligns very simply molecule to the reference molecule, based on the shared MCS.
-
-    Parameters
-    ----------
-    mol : SmallMoleculeComponent
-        molecule to be aligned to molA (will be moved)
-    ref_mol : SmallMoleculeComponent
-        molecule with the reference_positions.
-
-    Returns
-    -------
-    SmallMoleculeComponent
-        return an aligned copy of molB
-    """
-    mol = deepcopy(mol)
-
-    mol1b = ref_mol._rdkit
-    mol2b = mol._rdkit
-
-    p = rdFMCS.MCSParameters()
-    p.AtomTyper = rdFMCS.AtomCompare.CompareAny
-
-    res = rdFMCS.FindMCS([mol1b, mol2b], p)
-
-    # convert match to mapping'
-    q = Chem.MolFromSmarts(res.smartsString)
-    logging.debug(q)
-
-    m1_idx = mol1b.GetSubstructMatch(q)
-    m2_idx = mol2b.GetSubstructMatch(q)
-    logging.debug(m1_idx, m2_idx)
-
-    idx_mappings = list(zip(m2_idx, m1_idx))
-
-    rms = AllChem.AlignMol(
-        prbMol=mol2b,
-        refMol=mol1b,
-        atomMap=idx_mappings,
-    )
-    logging.debug(rms)
-
-    mol._rdkit = mol2b
-    return mol
+from copy import deepcopy
+
+from rdkit import Chem
+from rdkit.Chem import AllChem
+from rdkit.Chem import rdFMCS
+from rdkit.Chem import rdMolAlign
+
+from gufe import SmallMoleculeComponent
+
+import logging
+
+log = logging.getLogger(__name__)
+
+
+def align_mol_sceletons(
+    mol: SmallMoleculeComponent,
+    ref_mol: SmallMoleculeComponent,
+) -> SmallMoleculeComponent:
+    """
+        WORK IN PROGRESS!
+        This i a Wrapper for rdkit - MCS align
+        Aligns very simply molecule to the reference molecule, based on the shared MCS.
+
+    Parameters
+    ----------
+    mol : SmallMoleculeComponent
+        molecule to be aligned to molA (will be moved)
+    ref_mol : SmallMoleculeComponent
+        molecule with the reference_positions.
+
+    Returns
+    -------
+    SmallMoleculeComponent
+        return an aligned copy of molB
+    """
+    mol = deepcopy(mol)
+
+    mol1b = ref_mol._rdkit
+    mol2b = mol._rdkit
+
+    # MCS
+    p = rdFMCS.MCSParameters()
+    p.AtomTyper = rdFMCS.AtomCompare.CompareAny
+
+    res = rdFMCS.FindMCS([mol1b, mol2b], p)
+
+    # convert match to mapping
+    q = Chem.MolFromSmarts(res.smartsString)
+    logging.debug(q)
+
+    m1_idx = mol1b.GetSubstructMatch(q)
+    m2_idx = mol2b.GetSubstructMatch(q)
+    logging.debug(m1_idx, m2_idx)
+
+    idx_mappings = list(zip(m2_idx, m1_idx))
+
+    rms = AllChem.AlignMol(
+        prbMol=mol2b,
+        refMol=mol1b,
+        atomMap=idx_mappings,
+    )
+    logging.debug(rms)
+
+    mol._rdkit = mol2b
+    return mol
+
+def align_mol_shape(mol:SmallMoleculeComponent, ref_mol:SmallMoleculeComponent)->Chem.Mol:
+    """
+        WORK IN PROGRESS!
+        This i a Wrapper for rdkit / OPEN3DAlign
+        Aligns shape based two SmallMoleculeComponents.
+
+    Parameters
+    ----------
+    mol : SmallMoleculeComponent
+        molecule to be aligned to molA (will be moved)
+    ref_mol : SmallMoleculeComponent
+        molecule with the reference_positions.
+
+    Returns
+    -------
+    SmallMoleculeComponent
+        return an aligned copy of molB
+    """
+    mol = deepcopy(mol)
+
+    mol1b = ref_mol._rdkit
+    mol2b = mol._rdkit
+    pyO3A = rdMolAlign.GetO3A(prbMol=mol2b, refMol=mol1b,)
+    score = pyO3A.Align()
+    logging.debug("alignment score: "+str(score))
+
+    mol._rdkit = mol2b
+    return mol
```

### Comparing `kartograf-0.0.3/src/kartograf/atom_mapping/geom_mapper.py` & `kartograf-0.0.6/src/kartograf/atom_mapper.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,602 +1,592 @@
-# This code is part of OpenFE and is licensed under the MIT license.
-# For details, see https://github.com/OpenFreeEnergy/kartograf
-
-import copy
-import numpy as np
-import networkx as nx
-from enum import Enum
-
-from collections import OrderedDict
-from collections.abc import Iterator
-
-from rdkit import Chem
-
-from scipy.sparse import csr_matrix
-from scipy.optimize import linear_sum_assignment
-from scipy.sparse.csgraph import connected_components
-
-from typing import Callable, Dict, Iterable, List, Optional, Set, Tuple, Union
-
-from gufe import SmallMoleculeComponent
-from gufe import LigandAtomMapping
-from gufe import AtomMapping, AtomMapper
-
-import logging
-
-log = logging.getLogger(__name__)
-
-
-# Enums:
-class mapping_algorithm(Enum):
-    linear_sum_assignment = "LSA"
-    minimal_spanning_tree = "MST"
-
-
-# Helper:
-vector_eucledean_dist = calculate_edge_weight = lambda x, y: np.sqrt(
-    np.sum(np.square(y - x), axis=1)
-)
-
-
-# Implementation of Mapper:
-class geometric_atom_mapper(AtomMapper):
-    atom_max_distance: float
-    atom_ring_matches_ring: bool
-    atom_map_hydrogens: bool
-    mapping_algorithm: mapping_algorithm
-
-    def __init__(
-        self,
-        *,
-        atom_ring_matches_ring: Optional[bool] = False,
-        atom_max_distance: Optional[float] = 0.95,
-        atom_map_hydrogens: Optional[bool] = True,
-        _mapping_algorithm: Optional[mapping_algorithm] = mapping_algorithm.linear_sum_assignment,
-    ):
-        """
-        This mapper is a homebrew, that utilises rdkit in order
-        to generate a mapping.
-
-        Parameters
-        ----------
-        atom_ring_matches_ring : bool, optional
-            default False
-        atom_max_distance : float, optional
-            geometric criteria for two atoms, how far their distance
-            can be maximal (in Angstrom). Default 0.95
-        mapping_algorithm : str, optional
-            default="LSA"
-
-        """
-        self.atom_max_distance = atom_max_distance
-        self.atom_ring_matches_ring = atom_ring_matches_ring
-        self.atom_map_hydrogens = atom_map_hydrogens
-
-        if _mapping_algorithm == _mapping_algorithm.linear_sum_assignment:
-            self.mapping_algorithm = self._linearSumAlgorithm_map
-        elif _mapping_algorithm == _mapping_algorithm.minimal_spanning_tree:
-            self.mapping_algorithm = self._minimalSpanningTree_map
-        else:
-            raise ValueError(
-                "Mapping algorithm not implemented or unknown (options: MST or LSA). got key: "
-                + str(_mapping_algorithm)
-            )
-
-    def _from_dict():
-        pass
-
-    def _to_dict():
-        pass
-
-    def _defaults():
-        pass
-
-    """
-       Privat - Set Operations
-    """
-
-    @staticmethod
-    def _get_connected_atom_subsets(mol: Chem.Mol, to_be_searched: List[int]) -> List[Set[int]]:
-        # Get bonded atoms sets
-        bonded_atom_sets = []
-        for aid in to_be_searched:
-            a = mol.GetAtomWithIdx(int(aid))
-            bond_atoms = [b.GetOtherAtomIdx(aid) for b in a.GetBonds()]
-            connected_atoms = set([aid] + bond_atoms)
-
-            # filter to not connect non mapped atoms
-            filtered_connected_atoms = set(filter(lambda x: x in to_be_searched, connected_atoms))
-
-            # NO mapped atom connected?
-            if len(filtered_connected_atoms) == 1:
-                continue
-            else:
-                bonded_atom_sets.append(filtered_connected_atoms)
-        bonded_atom_sets = list(sorted(bonded_atom_sets))
-
-        log.debug("Bonded atom Sets: " + str(bonded_atom_sets))
-
-        # add new set or merge with existing set
-        atom_mappings = {i: a for i, a in enumerate(to_be_searched)}
-        r_atom_mappings = {a: i for i, a in enumerate(to_be_searched)}
-        max_n = len(to_be_searched)
-
-        connection_matrix = np.zeros(shape=(max_n, max_n))
-        for set_i in bonded_atom_sets:
-            for ai in set_i:
-                for aj in set_i:
-                    connection_matrix[r_atom_mappings[ai]][r_atom_mappings[aj]] = 1
-
-        log.debug("Adjacency Matrix: " + str(connection_matrix))
-
-        # get connected components
-        matrix = csr_matrix(connection_matrix)
-        n_components, labels = connected_components(csgraph=matrix, directed=False)
-
-        log.debug("Connected Components: " + str(n_components) + "\t" + str(labels))
-
-        # Translate back
-        merged_connnected_atom_sets = []
-        labels_sizes = [
-            label
-            for label, _ in sorted(
-                np.vstack(np.unique(labels, return_counts=True)).T, key=lambda x: x[1], reverse=True
-            )
-        ]
-        for selected_label in labels_sizes:
-            connected_atoms_ids = list(
-                sorted(
-                    [atom_mappings[i] for i, label in enumerate(labels) if label == selected_label]
-                )
-            )
-            merged_connnected_atom_sets.append(connected_atoms_ids)
-
-        log.debug("Merged Sets:" + str(merged_connnected_atom_sets))
-
-        return merged_connnected_atom_sets
-
-    @staticmethod
-    def _get_maximal_mapping_set_overlap(
-        sets_a: set, sets_b: set, mapping: Dict[int, int]
-    ) -> Tuple[Tuple[int, int], dict]:
-        # Calculate overlaps
-
-        log.debug("Input: " + str(sets_a) + " " + str(sets_b) + " " + str(mapping))
-
-        max_set_combi = {}
-        for ida, set_a in enumerate(sets_a):
-            mapped_set_a = {mapping[a] for a in set_a}
-            for idb, set_b in enumerate(sets_b):
-                set_intersection_size = len(mapped_set_a.intersection(set_b))
-                if set_intersection_size:
-                    max_set_combi[(ida, idb)] = {
-                        "overlap_count": set_intersection_size,
-                        "set_a_size": len(set_a),
-                        "set_b_size": len(set_b),
-                    }
-
-        # sort overlap by size
-        overlap_sorted_sets = OrderedDict(
-            sorted(max_set_combi.items(), key=lambda x: x[1]["overlap_count"], reverse=False)
-        )
-
-        log.debug("Set overlap properties" + str(overlap_sorted_sets))
-
-        max_overlap_set_a_id, max_overlap_set_b_id = overlap_sorted_sets.popitem()
-        return max_overlap_set_a_id, max_overlap_set_b_id
-
-    @staticmethod
-    def _filter_mapping_for_set_overlap(
-        set_a: Set[int], set_b: Set[int], mapping: Dict[int, int]
-    ) -> Dict[int, int]:
-        filtered_mapping = {}
-        for atom_a, atom_b in mapping.items():
-            if atom_a in set_a and atom_b in set_b:
-                filtered_mapping[atom_a] = atom_b
-        return filtered_mapping
-
-    @classmethod
-    def _filter_mapping_for_max_overlapping_connected_atom_set(
-        cls, moleculeA: Chem.Mol, moleculeB: Chem.Mol, atom_mapping: Dict[int, int]
-    ) -> Dict[int, int]:
-        # get connected sets from mappings
-        sets_a = cls._get_connected_atom_subsets(moleculeA, atom_mapping.keys())
-        sets_b = cls._get_connected_atom_subsets(moleculeB, atom_mapping.values())
-
-        log.debug("Found connected sets: " + "\t".join(map(str, [sets_a, sets_b, atom_mapping])))
-
-        # get maximally overlapping largest sets
-        ((max_set_a_id, max_set_b_id), max_set) = cls._get_maximal_mapping_set_overlap(
-            sets_a, sets_b, atom_mapping
-        )
-
-        # filter mapping for atoms in maximally overlapping sets
-        atom_mapping = cls._filter_mapping_for_set_overlap(
-            sets_a[max_set_a_id], sets_b[max_set_b_id], atom_mapping
-        )
-
-        log.debug(
-            "Found connected set overlaps: "
-            + "\t".join(map(str, [max_set_a_id, max_set_b_id, max_set, atom_mapping]))
-        )
-
-        return atom_mapping
-
-    """
-        Utils
-    """
-
-    @staticmethod
-    def _get_full_distance_matrix(
-        atomA_pos: np.array,
-        atomB_pos: np.array,
-        metric: Callable[
-            [Union[float, Iterable], Union[float, Iterable]], Union[float, Iterable]
-        ] = vector_eucledean_dist,
-    ) -> np.array:
-        distance_matrix = []
-        for atomPosA in atomA_pos:
-            atomPos_distances = metric(atomPosA, atomB_pos)
-            distance_matrix.append(atomPos_distances)
-        distance_matrix = np.array(distance_matrix)
-        return distance_matrix
-
-    @staticmethod
-    def _mask_atoms(
-        mol, mol_pos, map_hydrogens: bool = False, masked_atoms=[]
-    ) -> Tuple[Dict, List]:
-        pos = []
-        masked_atomMapping = {}
-        for atom in mol.GetAtoms():
-            atom_id = atom.GetIdx()
-            if (map_hydrogens or atom.GetSymbol() != "H") and atom_id not in masked_atoms:
-                masked_atomMapping[len(masked_atomMapping)] = atom_id
-                pos.append(mol_pos[atom_id])
-        pos = np.array(pos)
-
-        return masked_atomMapping, pos
-
-    def _minimalSpanningTree_map(
-        self, distance_matrix: np.array, max_dist: float
-    ) -> Dict[int, int]:
-        """
-        This function is a numpy graph based implementation to build up an Atom Mapping purely on 3D criteria.
-
-
-        """
-        # distance matrix:  - full graph
-        log.debug("Got Distance Matrix: \n" + str(distance_matrix))
-        edges = []
-        for i, distance_row in enumerate(distance_matrix):
-            for j, dist in enumerate(distance_row):
-                edges.append([float(dist), int(i), int(j)])
-
-        edges = np.array(edges)
-        log.debug("Edges: \n" + str(edges))
-
-        # priority queue based on edge weight
-        sorted_edges = edges[edges[:, 0].argsort()]
-        log.debug("Sorted Edges: \n" + str(sorted_edges))
-
-        # MST like algorithm
-        mapping = {}
-        for w, x, y in sorted_edges:
-            if w >= max_dist:  # filter for max dist
-                break
-            else:
-                if x not in mapping.keys() and y not in mapping.values():
-                    mapping[int(x)] = int(y)
-
-        return mapping
-
-    @staticmethod
-    def _linearSumAlgorithm_map(distance_matrix: np.array, max_dist: float) -> Dict[int, int]:
-        row_ind, col_ind = linear_sum_assignment(distance_matrix)
-        raw_mapping = list(zip(map(int, row_ind), map(int, col_ind)))
-        # filter for mask value
-        mapping = dict(filter(lambda x: distance_matrix[x] < max_dist, raw_mapping))
-
-        return mapping
-
-    def calculate_mapping(
-        self,
-        molA: Chem.Mol,
-        molB: Chem.Mol,
-        max_d: float = 0.95,
-        masked_atoms_molA=[],
-        masked_atoms_molB=[],
-        pre_mapped_atoms={},
-        map_hydrogens: bool = True
-        ) -> AtomMapping:
-        """
-            find a mapping between two molecules based on 3D coordinates.
-
-        Parameters
-        ----------
-        molA : Chem.Mol
-            rdkit Molecule A
-        molB : Chem.Mol
-            rdkit Molecule B
-        max_d : float, optional
-            maximal allowed distance for atoms to be mapped, by default 0.95
-        masked_atoms_molA : list, optional
-            remove categorical atoms by index of MolA from the mapping, by default []
-        masked_atoms_molB : list, optional
-            remove categorical atoms by index of MolB from the mapping, by default []
-        pre_mapped_atoms : dict, optional
-            pre_mapped atoms, that need to be part of the mapping, by default {}
-        map_hydrogens : bool, optional
-            if True map hydrogens as well, will hapen after heavy atom mapping, by default True
-
-        Returns
-        -------
-        AtomMapping
-            _description_
-        """        
-
-        molA_pos = molA.GetConformer().GetPositions()
-        molB_pos = molB.GetConformer().GetPositions()
-        masked_atoms_molA = copy.deepcopy(masked_atoms_molA)
-        masked_atoms_molB = copy.deepcopy(masked_atoms_molB)
-        pre_mapped_atoms = copy.deepcopy(pre_mapped_atoms)
-
-        if len(pre_mapped_atoms) > 0:
-            masked_atoms_molA.extend(pre_mapped_atoms.keys())
-            masked_atoms_molB.extend(pre_mapped_atoms.values())
-
-        log.debug("Positions lengths: " + str(len(molA_pos)) + " " + str(len(molB_pos)))
-        log.debug("Positions: \n" + "\n\t".join(map(str, [molA_pos, molB_pos])))
-        log.debug("masked_atoms_molA: " + str(masked_atoms_molA))
-        log.debug("masked_atoms_molB: " + str(masked_atoms_molB))
-        log.debug("pre_mapped_atoms: " + str(pre_mapped_atoms))
-        log.debug("map_hydrogens: " + str(map_hydrogens))
-
-        log.info("Masking Atoms")
-
-        molA_masked_atomMapping, molA_pos = self._mask_atoms(
-            mol=molA,
-            mol_pos=molA_pos,
-            masked_atoms=masked_atoms_molA,
-            map_hydrogens=map_hydrogens,
-        )
-        molB_masked_atomMapping, molB_pos = self._mask_atoms(
-            mol=molB,
-            mol_pos=molB_pos,
-            masked_atoms=masked_atoms_molB,
-            map_hydrogens=map_hydrogens,
-        )
-
-        log.debug(
-            "Remove Masked Atoms: \n"
-            + "\n\t".join(map(str, [molA_masked_atomMapping, molB_masked_atomMapping]))
-            + "\n"
-            + "\n\t".join(map(str, [molA_pos, molB_pos]))
-        )
-        log.debug(
-            "filtered Masked Positions lengths: "
-            + "\t".join(map(str, [len(molA_pos), len(molB_pos)]))
-        )
-
-        if len(molA_pos) == 0 or len(molB_pos) == 0:  # TODO: check if this is correct
-            log.warning("no mappable Atoms were found!")
-            return pre_mapped_atoms
-
-        # Calculate mapping
-        log.info("Build Distance Matrix")
-        # distance matrix:  - full graph
-        distance_matrix = self._get_full_distance_matrix(molA_pos, molB_pos)
-        log.debug("Distance Matrix: \n" + str(distance_matrix))
-
-        # Mask distance matrix with max_d
-        # np.inf is considererd as not possible in lsa implementation - therefore use a high value
-        self.mask_dist_val = max_d * 10**6
-        masked_dmatrix = np.array(
-            np.ma.where(distance_matrix < max_d, distance_matrix, self.mask_dist_val)
-        )
-        log.debug("masked Distance Matrix: " + str(max_d) + "\n\t" + str(masked_dmatrix))
-
-        # solve atom mappings
-        log.info("Calculate Mapping")
-        mapping = self.mapping_algorithm(
-            distance_matrix=masked_dmatrix, max_dist=self.mask_dist_val
-        )
-        log.debug("Raw Mapping: " + str(mapping))
-
-        if len(mapping) == 0:  # TODO: check if this is correct
-            log.warning("no mapping could be found!")
-            return pre_mapped_atoms
-
-        # reverse any prior masking:
-        mapping = {
-            molA_masked_atomMapping[k]: molB_masked_atomMapping[v] for k, v in mapping.items()
-        }
-
-        if len(pre_mapped_atoms) > 0:
-            mapping.update(pre_mapped_atoms)
-        log.debug("reverse Masking Mapping: " + str(mapping))
-
-        # Reduce mapping to maximally overlapping two connected sets
-        log.info("Find Maximal overlapping connected sets of mapped atoms")
-        mapping = self._filter_mapping_for_max_overlapping_connected_atom_set(
-            moleculeA=molA, moleculeB=molB, atom_mapping=mapping
-        )
-        log.debug("Set overlap Mapping: " + str(mapping))
-
-        return mapping
-
-    """
-        Mapping functions
-    """
-
-    def get_mapping(
-        self,
-        molA: Chem.Mol,
-        molB: Chem.Mol,
-        masked_atoms_molA=[],
-        masked_atoms_molB=[],
-        pre_mapped_atoms={},
-    ) -> Dict[int, int]:
-        """
-        The function effectivly maps the two molecules on to each other and
-        applies the given settings by the obj.
-
-        Parameters
-        ----------
-        molA, molB : rdkit.Chem.Mol
-            two rdkit molecules that should be mapped onto each other
-        masked_atoms_molA : list, optional
-            remove categorical atoms by index of MolA from the mapping, by default []
-        masked_atoms_molB : list, optional
-            remove categorical atoms by index of MolB from the mapping, by default []
-        pre_mapped_atoms : dict, optional
-            pre_mapped atoms, that need to be part of the mapping, by default {}
-
-        """
-        molA = Chem.Mol(molA)
-        molB = Chem.Mol(molB)
-        masked_atoms_molA = copy.deepcopy(masked_atoms_molA)
-        masked_atoms_molB = copy.deepcopy(masked_atoms_molB)
-        pre_mapped_atoms = copy.deepcopy(pre_mapped_atoms)
-
-        log.info("#################################")
-        log.info("Map Heavy Atoms ")
-        log.info("#################################")
-
-        mapping = self.calculate_mapping(
-            molA,
-            molB,
-            max_d=self.atom_max_distance,
-            masked_atoms_molA=masked_atoms_molA,
-            masked_atoms_molB=masked_atoms_molB,
-            pre_mapped_atoms=pre_mapped_atoms,
-            map_hydrogens=False,
-        )
-
-        if self.atom_map_hydrogens:
-            log.info("#################################")
-            log.info("Map Hydrogen Atoms: ")
-            log.info("#################################")
-
-            pre_mapped_atoms.update(mapping)
-
-            mapping = self.calculate_mapping(
-                molA,
-                molB,
-                max_d=self.atom_max_distance,
-                masked_atoms_molA=masked_atoms_molA,
-                masked_atoms_molB=masked_atoms_molB,
-                pre_mapped_atoms=pre_mapped_atoms,
-                map_hydrogens=self.atom_map_hydrogens,
-            )
-
-        return mapping
-
-    def suggest_mappings(
-        self, A: SmallMoleculeComponent, B: SmallMoleculeComponent
-    ) -> Iterator[AtomMapping]:
-        yield LigandAtomMapping(A, B, self.get_mapping(molA=A.to_rdkit(), molB=B.to_rdkit()))
-
-
-############# Old IMPLEMENTATION IDEA for pure 3D mapping - To Be deleted
-# Working with graphs:
-def _build_graph(molA: Chem.Mol, molB: Chem.Mol, max_d: float = 0.95) -> nx.Graph:
-    """
-    This function builds a full graph, with the exception of filtering for max_d
-
-    Parameters
-    ----------
-    molA : Chem.Mol
-        _description_
-    molB :  Chem.Mol
-        _description_
-    max_d : float, optional
-        _description_, by default 0.95
-
-    Returns
-    -------
-    nx.Graph
-        constructed graph
-    """
-
-    aA = molA.GetConformer().GetPositions()
-    aB = molB.GetConformer().GetPositions()
-
-    G = nx.Graph()
-
-    mol1_length = mol2_start = len(aA)
-    mol2_length = len(aB)
-
-    for n in range(mol1_length + mol2_length):
-        G.add_node(n)
-
-    edges = []
-    for n1, atomPosA in enumerate(aA):
-        for n2, atomPosB in enumerate(aB, start=mol2_start):
-            dist = vector_eucledean_dist(atomPosA, atomPosB)
-            color = "red" if (dist > max_d) else "green"
-            e = (n1, n2, {"dist": vector_eucledean_dist(atomPosA, atomPosB), "color": color})
-            if dist > max_d:
-                continue
-            else:
-                edges.append((e[0], e[1], vector_eucledean_dist(atomPosA, atomPosB)))
-    G.add_weighted_edges_from(edges)
-
-    return G
-
-
-# modified MST
-def _get_mst_chain_graph(graph):
-    """
-    This function uses a graph and returns its edges in order of an MST according to Kruskal algorithm, but filters the edges such no branching occurs in the tree (actually not really a tree anymore I guess...).
-    The 'no-branching' translate to no atom can be mapped twice in the final result.
-
-    Parameters
-    ----------
-    graph : nx.Graph
-        _description_
-
-    Returns
-    -------
-    dict[int, int]
-        resulting atom mapping
-    """
-    gMap = {}
-    min_edges = nx.minimum_spanning_edges(
-        nx.MultiGraph(graph), weight="weight", algorithm="kruskal"
-    )
-    for n1, n2, w, attr in min_edges:
-        if n1 in gMap.keys() or n1 in gMap.values() or n2 in gMap.keys() or n2 in gMap.values():
-            continue
-        else:
-            gMap[n1] = n2
-
-    return gMap
-
-
-def get_geom_Mapping(
-    molA: SmallMoleculeComponent, molB: SmallMoleculeComponent, max_d: float = 0.95
-):
-    """
-    This function is a networkx graph based implementation to build up an Atom Mapping purely on 3D criteria.
-
-    Parameters
-    ----------
-    molA : SmallMoleculeComponent
-        _description_
-    molB : SmallMoleculeComponent
-        _description_
-    max_d : float, optional
-        _description_, by default 0.95
-
-    Returns
-    -------
-    AtomMapping
-        resulting 3d Atom mapping
-    """
-    mol1_length = molA._rdkit.GetNumAtoms()
-    G = _build_graph(molA=molA._rdkit, molB=molB._rdkit, max_d=max_d)
-    gMap = _get_mst_chain_graph(G)
-    map_dict = {
-        k % mol1_length: v % mol1_length for k, v in gMap.items()
-    }  # cleanup step due to graph build up.
-    return AtomMapping(molA, molB, map_dict)
+# This code is part of OpenFE and is licensed under the MIT license.
+# For details, see https://github.com/OpenFreeEnergy/kartograf
+
+import copy
+import numpy as np
+from enum import Enum
+
+from collections import OrderedDict
+from collections.abc import Iterator
+
+from rdkit import Chem
+
+from scipy.sparse import csr_matrix
+from scipy.optimize import linear_sum_assignment
+from scipy.sparse.csgraph import connected_components
+
+from typing import Callable, Dict, Iterable, List, Optional, Set, Tuple, Union
+
+from gufe import SmallMoleculeComponent
+from gufe import LigandAtomMapping
+from gufe import AtomMapping, AtomMapper
+
+import logging
+
+log = logging.getLogger(__name__)
+
+
+# Enums:
+class mapping_algorithm(Enum):
+    linear_sum_assignment = "LSA"
+    minimal_spanning_tree = "MST"
+
+
+# Helper:
+vector_eucledean_dist = calculate_edge_weight = lambda x, y: np.sqrt(
+    np.sum(np.square(y - x), axis=1)
+)
+
+# filter functions:
+def filter_atoms_h_only_h_mapped(
+    molA: Chem.Mol, molB: Chem.Mol, mapping: Dict[int, int]
+) -> Dict[int, int]:
+
+    filtered_mapping = {}
+    for atomA_idx, atomB_idx in mapping.items():
+        atomA = molA.GetAtomWithIdx(atomA_idx)
+        atomB = molB.GetAtomWithIdx(atomB_idx)
+
+        if (atomA.GetAtomicNum() == atomB.GetAtomicNum() == 1) or (
+            atomA.GetAtomicNum() == atomB.GetAtomicNum() != 1
+        ):
+            filtered_mapping[atomA_idx] = atomB_idx
+            log.debug(
+                "keep mapping for atomIDs ("
+                + str(atomA_idx)
+                + ", "
+                + str(atomB_idx)
+                + "): ",
+                atomA.GetAtomicNum(),
+                atomB.GetAtomicNum(),
+            )
+
+        else:
+            log.debug(
+                "no mapping for atomIDs ("
+                + str(atomA_idx)
+                + ", "
+                + str(atomB_idx)
+                + "): ",
+                atomA.GetAtomicNum(),
+                atomB.GetAtomicNum(),
+            )
+
+    return filtered_mapping
+
+
+# Implementation of Mapper:
+class KartografAtomMapper(AtomMapper):
+    atom_max_distance: float
+    atom_ring_matches_ring: bool
+    atom_map_hydrogens: bool
+    mapping_algorithm: mapping_algorithm
+
+    _filter_funcs: Iterable[
+        Callable[Tuple[Chem.Mol, Chem.Mol, Dict[int, int]], Dict[int, int]]
+    ]
+
+    def __init__(
+        self,
+        *,
+        atom_ring_matches_ring: Optional[bool] = False,
+        atom_max_distance: Optional[float] = 0.95,
+        atom_map_hydrogens: Optional[bool] = True,
+        map_hydrogens_on_hydrogens_only: Optional[bool] = False,
+        _additional_mapping_filter_functions: Optional[
+            Iterable[
+                Callable[Tuple[Chem.Mol, Chem.Mol, Dict[int, int]], Dict[int, int]]
+            ]
+        ] = None,
+        _mapping_algorithm: Optional[
+            mapping_algorithm
+        ] = mapping_algorithm.linear_sum_assignment,
+    ):
+        """
+        This mapper is a homebrew, that utilises rdkit in order
+        to generate an atom-mapping based on the coordinates of two molecules.
+
+        Parameters
+        ----------
+        atom_ring_matches_ring : bool, optional
+            default False
+        atom_max_distance : float, optional
+            geometric criteria for two atoms, how far their distance
+            can be maximal (in Angstrom). Default 0.95
+        map_hydrogens_on_hydrogens_only : bool, optional
+            map hydrogens only on hydrogens. Default False
+        mapping_algorithm : str, optional
+            default="LSA"
+
+        """
+        self.atom_max_distance = atom_max_distance
+        self.atom_ring_matches_ring = atom_ring_matches_ring
+        self.atom_map_hydrogens = atom_map_hydrogens
+
+        self._filter_funcs = []
+        if map_hydrogens_on_hydrogens_only:
+            self._filter_funcs.append(filter_atoms_h_only_h_mapped)
+        if _additional_mapping_filter_functions is not None:
+            self._filter_funcs.extend(_additional_mapping_filter_functions)
+
+        if _mapping_algorithm == _mapping_algorithm.linear_sum_assignment:
+            self.mapping_algorithm = self._linearSumAlgorithm_map
+        elif _mapping_algorithm == _mapping_algorithm.minimal_spanning_tree:
+            self.mapping_algorithm = self._minimalSpanningTree_map
+        else:
+            raise ValueError(
+                "Mapping algorithm not implemented or unknown (options: MST or LSA). got key: "
+                + str(_mapping_algorithm)
+            )
+
+    # TODO: Needs to be implemented
+    def _from_dict():
+        pass
+
+    def _to_dict():
+        pass
+
+    def _defaults():
+        pass
+
+    """
+       Privat - Set Operations
+    """
+
+    @staticmethod
+    def _get_connected_atom_subsets(
+        mol: Chem.Mol, to_be_searched: List[int]
+    ) -> List[Set[int]]:
+        # Get bonded atoms sets
+        bonded_atom_sets = []
+        for aid in to_be_searched:
+            a = mol.GetAtomWithIdx(int(aid))
+            bond_atoms = [b.GetOtherAtomIdx(aid) for b in a.GetBonds()]
+            connected_atoms = set([aid] + bond_atoms)
+
+            # filter to not connect non mapped atoms
+            filtered_connected_atoms = set(
+                filter(lambda x: x in to_be_searched, connected_atoms)
+            )
+
+            # NO mapped atom connected?
+            if len(filtered_connected_atoms) == 1:
+                continue
+            else:
+                bonded_atom_sets.append(filtered_connected_atoms)
+        bonded_atom_sets = list(sorted(bonded_atom_sets))
+
+        log.debug("Bonded atom Sets: " + str(bonded_atom_sets))
+
+        # add new set or merge with existing set
+        atom_mappings = {i: a for i, a in enumerate(to_be_searched)}
+        r_atom_mappings = {a: i for i, a in enumerate(to_be_searched)}
+        max_n = len(to_be_searched)
+
+        connection_matrix = np.zeros(shape=(max_n, max_n))
+        for set_i in bonded_atom_sets:
+            for ai in set_i:
+                for aj in set_i:
+                    connection_matrix[r_atom_mappings[ai]][r_atom_mappings[aj]] = 1
+
+        log.debug("Adjacency Matrix: " + str(connection_matrix))
+
+        # get connected components
+        matrix = csr_matrix(connection_matrix)
+        n_components, labels = connected_components(csgraph=matrix, directed=False)
+
+        log.debug("Connected Components: " + str(n_components) + "\t" + str(labels))
+
+        # Translate back
+        merged_connnected_atom_sets = []
+        labels_sizes = [
+            label
+            for label, _ in sorted(
+                np.vstack(np.unique(labels, return_counts=True)).T,
+                key=lambda x: x[1],
+                reverse=True,
+            )
+        ]
+        for selected_label in labels_sizes:
+            connected_atoms_ids = list(
+                sorted(
+                    [
+                        atom_mappings[i]
+                        for i, label in enumerate(labels)
+                        if label == selected_label
+                    ]
+                )
+            )
+            merged_connnected_atom_sets.append(connected_atoms_ids)
+
+        log.debug("Merged Sets:" + str(merged_connnected_atom_sets))
+
+        return merged_connnected_atom_sets
+
+    @staticmethod
+    def _get_maximal_mapping_set_overlap(
+        sets_a: set, sets_b: set, mapping: Dict[int, int]
+    ) -> Tuple[Tuple[int, int], dict]:
+        # Calculate overlaps
+
+        log.debug("Input: " + str(sets_a) + " " + str(sets_b) + " " + str(mapping))
+
+        max_set_combi = {}
+        for ida, set_a in enumerate(sets_a):
+            mapped_set_a = {mapping[a] for a in set_a}
+            for idb, set_b in enumerate(sets_b):
+                set_intersection_size = len(mapped_set_a.intersection(set_b))
+                if set_intersection_size:
+                    max_set_combi[(ida, idb)] = {
+                        "overlap_count": set_intersection_size,
+                        "set_a_size": len(set_a),
+                        "set_b_size": len(set_b),
+                    }
+
+        # sort overlap by size
+        overlap_sorted_sets = OrderedDict(
+            sorted(
+                max_set_combi.items(),
+                key=lambda x: x[1]["overlap_count"],
+                reverse=False,
+            )
+        )
+
+        log.debug("Set overlap properties" + str(overlap_sorted_sets))
+
+        max_overlap_set_a_id, max_overlap_set_b_id = overlap_sorted_sets.popitem()
+        return max_overlap_set_a_id, max_overlap_set_b_id
+
+    @staticmethod
+    def _filter_mapping_for_set_overlap(
+        set_a: Set[int], set_b: Set[int], mapping: Dict[int, int]
+    ) -> Dict[int, int]:
+        filtered_mapping = {}
+        for atom_a, atom_b in mapping.items():
+            if atom_a in set_a and atom_b in set_b:
+                filtered_mapping[atom_a] = atom_b
+        return filtered_mapping
+
+    @classmethod
+    def _filter_mapping_for_max_overlapping_connected_atom_set(
+        cls, moleculeA: Chem.Mol, moleculeB: Chem.Mol, atom_mapping: Dict[int, int]
+    ) -> Dict[int, int]:
+        # get connected sets from mappings
+        sets_a = cls._get_connected_atom_subsets(moleculeA, atom_mapping.keys())
+        sets_b = cls._get_connected_atom_subsets(moleculeB, atom_mapping.values())
+
+        log.debug(
+            "Found connected sets: "
+            + "\t".join(map(str, [sets_a, sets_b, atom_mapping]))
+        )
+
+        # get maximally overlapping largest sets
+        ((max_set_a_id, max_set_b_id), max_set) = cls._get_maximal_mapping_set_overlap(
+            sets_a, sets_b, atom_mapping
+        )
+
+        # filter mapping for atoms in maximally overlapping sets
+        atom_mapping = cls._filter_mapping_for_set_overlap(
+            sets_a[max_set_a_id], sets_b[max_set_b_id], atom_mapping
+        )
+
+        log.debug(
+            "Found connected set overlaps: "
+            + "\t".join(map(str, [max_set_a_id, max_set_b_id, max_set, atom_mapping]))
+        )
+
+        return atom_mapping
+
+    """
+        Utils
+    """
+
+    @staticmethod
+    def _get_full_distance_matrix(
+        atomA_pos: np.array,
+        atomB_pos: np.array,
+        metric: Callable[
+            [Union[float, Iterable], Union[float, Iterable]], Union[float, Iterable]
+        ] = vector_eucledean_dist,
+    ) -> np.array:
+        distance_matrix = []
+        for atomPosA in atomA_pos:
+            atomPos_distances = metric(atomPosA, atomB_pos)
+            distance_matrix.append(atomPos_distances)
+        distance_matrix = np.array(distance_matrix)
+        return distance_matrix
+
+    @staticmethod
+    def _mask_atoms(
+        mol, mol_pos, map_hydrogens: bool = False, masked_atoms=[]
+    ) -> Tuple[Dict, List]:
+        pos = []
+        masked_atomMapping = {}
+        for atom in mol.GetAtoms():
+            atom_id = atom.GetIdx()
+            if (
+                map_hydrogens or atom.GetSymbol() != "H"
+            ) and atom_id not in masked_atoms:
+                masked_atomMapping[len(masked_atomMapping)] = atom_id
+                pos.append(mol_pos[atom_id])
+        pos = np.array(pos)
+
+        return masked_atomMapping, pos
+
+    def _minimalSpanningTree_map(
+        self, distance_matrix: np.array, max_dist: float
+    ) -> Dict[int, int]:
+        """
+        This function is a numpy graph based implementation to build up an Atom Mapping purely on 3D criteria.
+
+
+        """
+        # distance matrix:  - full graph
+        log.debug("Got Distance Matrix: \n" + str(distance_matrix))
+        edges = []
+        for i, distance_row in enumerate(distance_matrix):
+            for j, dist in enumerate(distance_row):
+                edges.append([float(dist), int(i), int(j)])
+
+        edges = np.array(edges)
+        log.debug("Edges: \n" + str(edges))
+
+        # priority queue based on edge weight
+        sorted_edges = edges[edges[:, 0].argsort()]
+        log.debug("Sorted Edges: \n" + str(sorted_edges))
+
+        # MST like algorithm
+        mapping = {}
+        for w, x, y in sorted_edges:
+            if w >= max_dist:  # filter for max dist
+                break
+            else:
+                if x not in mapping.keys() and y not in mapping.values():
+                    mapping[int(x)] = int(y)
+
+        return mapping
+
+    @staticmethod
+    def _linearSumAlgorithm_map(
+        distance_matrix: np.array, max_dist: float
+    ) -> Dict[int, int]:
+        row_ind, col_ind = linear_sum_assignment(distance_matrix)
+        raw_mapping = list(zip(map(int, row_ind), map(int, col_ind)))
+        # filter for mask value
+        mapping = dict(filter(lambda x: distance_matrix[x] < max_dist, raw_mapping))
+
+        return mapping
+
+    def _additional_filter_rules(
+        self, molA: Chem.Mol, molB: Chem.Mol, mapping: Dict[int, int]
+    ) -> Dict[int, int]:
+        filtered_mapping = copy.deepcopy(mapping)
+        for filter_rule in self._filter_funcs:
+            filtered_mapping = filter_rule(molA, molB, filtered_mapping)
+        return filtered_mapping
+
+    def calculate_mapping(
+        self,
+        molA: Chem.Mol,
+        molB: Chem.Mol,
+        max_d: float = 0.95,
+        masked_atoms_molA=[],
+        masked_atoms_molB=[],
+        pre_mapped_atoms={},
+        map_hydrogens: bool = True,
+    ) -> AtomMapping:
+        """
+            find a mapping between two molecules based on 3D coordinates.
+
+        Parameters
+        ----------
+        molA : Chem.Mol
+            rdkit Molecule A
+        molB : Chem.Mol
+            rdkit Molecule B
+        max_d : float, optional
+            maximal allowed distance for atoms to be mapped, by default 0.95
+        masked_atoms_molA : list, optional
+            remove categorical atoms by index of MolA from the mapping, by default []
+        masked_atoms_molB : list, optional
+            remove categorical atoms by index of MolB from the mapping, by default []
+        pre_mapped_atoms : dict, optional
+            pre_mapped atoms, that need to be part of the mapping, by default {}
+        map_hydrogens : bool, optional
+            if True map hydrogens as well, will hapen after heavy atom mapping, by default True
+
+        Returns
+        -------
+        AtomMapping
+            _description_
+        """
+
+        molA_pos = molA.GetConformer().GetPositions()
+        molB_pos = molB.GetConformer().GetPositions()
+        masked_atoms_molA = copy.deepcopy(masked_atoms_molA)
+        masked_atoms_molB = copy.deepcopy(masked_atoms_molB)
+        pre_mapped_atoms = copy.deepcopy(pre_mapped_atoms)
+
+        if len(pre_mapped_atoms) > 0:
+            masked_atoms_molA.extend(pre_mapped_atoms.keys())
+            masked_atoms_molB.extend(pre_mapped_atoms.values())
+
+        log.debug("Positions lengths: " + str(len(molA_pos)) + " " + str(len(molB_pos)))
+        log.debug("Positions: \n" + "\n\t".join(map(str, [molA_pos, molB_pos])))
+        log.debug("masked_atoms_molA: " + str(masked_atoms_molA))
+        log.debug("masked_atoms_molB: " + str(masked_atoms_molB))
+        log.debug("pre_mapped_atoms: " + str(pre_mapped_atoms))
+        log.debug("map_hydrogens: " + str(map_hydrogens))
+
+        log.info("Masking Atoms")
+
+        molA_masked_atomMapping, molA_pos = self._mask_atoms(
+            mol=molA,
+            mol_pos=molA_pos,
+            masked_atoms=masked_atoms_molA,
+            map_hydrogens=map_hydrogens,
+        )
+        molB_masked_atomMapping, molB_pos = self._mask_atoms(
+            mol=molB,
+            mol_pos=molB_pos,
+            masked_atoms=masked_atoms_molB,
+            map_hydrogens=map_hydrogens,
+        )
+
+        log.debug(
+            "Remove Masked Atoms: \n"
+            + "\n\t".join(map(str, [molA_masked_atomMapping, molB_masked_atomMapping]))
+            + "\n"
+            + "\n\t".join(map(str, [molA_pos, molB_pos]))
+        )
+        log.debug(
+            "filtered Masked Positions lengths: "
+            + "\t".join(map(str, [len(molA_pos), len(molB_pos)]))
+        )
+
+        if len(molA_pos) == 0 or len(molB_pos) == 0:  # TODO: check if this is correct
+            if(len(pre_mapped_atoms)==0): log.warning("no mappable Atoms were found!")
+            return pre_mapped_atoms
+
+        # Calculate mapping
+        log.info("Build Distance Matrix")
+        # distance matrix:  - full graph
+        distance_matrix = self._get_full_distance_matrix(molA_pos, molB_pos)
+        log.debug("Distance Matrix: \n" + str(distance_matrix))
+
+        # Mask distance matrix with max_d
+        # np.inf is considererd as not possible in lsa implementation - therefore use a high value
+        self.mask_dist_val = max_d * 10**6
+        masked_dmatrix = np.array(
+            np.ma.where(distance_matrix < max_d, distance_matrix, self.mask_dist_val)
+        )
+        log.debug(
+            "masked Distance Matrix: " + str(max_d) + "\n\t" + str(masked_dmatrix)
+        )
+
+        # solve atom mappings
+        log.info("Calculate Mapping")
+        mapping = self.mapping_algorithm(
+            distance_matrix=masked_dmatrix, max_dist=self.mask_dist_val
+        )
+        log.debug("Raw Mapping: " + str(mapping))
+
+        if len(mapping) == 0:  # TODO: check if this is correct
+            if(len(pre_mapped_atoms)==0): log.warning("no mapping could be found!")
+            return pre_mapped_atoms
+
+        # reverse any prior masking:
+        mapping = {
+            molA_masked_atomMapping[k]: molB_masked_atomMapping[v]
+            for k, v in mapping.items()
+        }
+
+        # filter mapping for rules:
+        if self._filter_funcs is not None:
+            mapping = self._additional_filter_rules(molA, molB, mapping)
+
+        if len(pre_mapped_atoms) > 0:
+            mapping.update(pre_mapped_atoms)
+        log.debug("reverse Masking Mapping: " + str(mapping))
+
+        # Reduce mapping to maximally overlapping two connected sets
+        log.info("Find Maximal overlapping connected sets of mapped atoms")
+        mapping = self._filter_mapping_for_max_overlapping_connected_atom_set(
+            moleculeA=molA, moleculeB=molB, atom_mapping=mapping
+        )
+        log.debug("Set overlap Mapping: " + str(mapping))
+
+        return mapping
+
+    """
+        Mapping functions
+    """
+
+    def get_mapping(
+        self,
+        molA: Chem.Mol,
+        molB: Chem.Mol,
+        masked_atoms_molA=[],
+        masked_atoms_molB=[],
+        pre_mapped_atoms={},
+    ) -> Dict[int, int]:
+        """
+        The function effectivly maps the two molecules on to each other and
+        applies the given settings by the obj.
+
+        Parameters
+        ----------
+        molA, molB : rdkit.Chem.Mol
+            two rdkit molecules that should be mapped onto each other
+        masked_atoms_molA : list, optional
+            remove categorical atoms by index of MolA from the mapping, by default []
+        masked_atoms_molB : list, optional
+            remove categorical atoms by index of MolB from the mapping, by default []
+        pre_mapped_atoms : dict, optional
+            pre_mapped atoms, that need to be part of the mapping, by default {}
+
+        """
+        molA = Chem.Mol(molA)
+        molB = Chem.Mol(molB)
+        masked_atoms_molA = copy.deepcopy(masked_atoms_molA)
+        masked_atoms_molB = copy.deepcopy(masked_atoms_molB)
+        pre_mapped_atoms = copy.deepcopy(pre_mapped_atoms)
+
+        log.info("#################################")
+        log.info("Map Heavy Atoms ")
+        log.info("#################################")
+
+        mapping = self.calculate_mapping(
+            molA,
+            molB,
+            max_d=self.atom_max_distance,
+            masked_atoms_molA=masked_atoms_molA,
+            masked_atoms_molB=masked_atoms_molB,
+            pre_mapped_atoms=pre_mapped_atoms,
+            map_hydrogens=False,
+        )
+
+        if self.atom_map_hydrogens:
+            log.info("#################################")
+            log.info("Map Hydrogen Atoms: ")
+            log.info("#################################")
+
+            pre_mapped_atoms.update(mapping)
+
+            mapping = self.calculate_mapping(
+                molA,
+                molB,
+                max_d=self.atom_max_distance,
+                masked_atoms_molA=masked_atoms_molA,
+                masked_atoms_molB=masked_atoms_molB,
+                pre_mapped_atoms=pre_mapped_atoms,
+                map_hydrogens=self.atom_map_hydrogens,
+            )
+
+        return mapping
+
+    def suggest_mappings(
+        self, A: SmallMoleculeComponent, B: SmallMoleculeComponent
+    ) -> Iterator[AtomMapping]:
+        yield LigandAtomMapping(
+            A, B, self.get_mapping(molA=A.to_rdkit(), molB=B.to_rdkit())
+        )
```

### Comparing `kartograf-0.0.3/src/kartograf.egg-info/SOURCES.txt` & `kartograf-0.0.6/src/kartograf.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 LICENSE
 README.md
 pyproject.toml
 src/kartograf/__init__.py
 src/kartograf/_version.py
+src/kartograf/atom_align.py
+src/kartograf/atom_mapper.py
+src/kartograf/atom_mapping_scorer.py
 src/kartograf.egg-info/PKG-INFO
 src/kartograf.egg-info/SOURCES.txt
 src/kartograf.egg-info/dependency_links.txt
 src/kartograf.egg-info/requires.txt
 src/kartograf.egg-info/top_level.txt
-src/kartograf/atom_mapping/__init__.py
-src/kartograf/atom_mapping/geom_align.py
-src/kartograf/atom_mapping/geom_mapper.py
-src/kartograf/atom_mapping/geom_scorer.py
-src/kartograf/networks/__init__.py
-src/kartograf/networks/mst_networker.py
-src/kartograf/networks/radial_networker.py
-src/kartograf/tests/test_geom_mapper.py
+src/kartograf/tests/__init__.py
+src/kartograf/tests/conf.py
+src/kartograf/tests/test_atom_align.py
+src/kartograf/tests/test_atom_mapper.py
+src/kartograf/tests/test_atom_mapping_scorer.py
```

