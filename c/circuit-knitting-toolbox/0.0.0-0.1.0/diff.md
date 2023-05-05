# Comparing `tmp/circuit_knitting_toolbox-0.0.0.tar.gz` & `tmp/circuit-knitting-toolbox-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "circuit_knitting_toolbox-0.0.0.tar", last modified: Fri Nov  4 20:06:37 2022, max compression
+gzip compressed data, was "circuit-knitting-toolbox-0.1.0.tar", last modified: Fri May  5 23:57:12 2023, max compression
```

## Comparing `circuit_knitting_toolbox-0.0.0.tar` & `circuit-knitting-toolbox-0.1.0.tar`

### file list

```diff
@@ -1,84 +1,90 @@
--rw-r--r--   0        0        0       21 2022-11-04 20:06:31.909524 circuit_knitting_toolbox-0.0.0/.dockerignore
--rw-r--r--   0        0        0     3711 2022-11-04 20:06:31.909524 circuit_knitting_toolbox-0.0.0/.github/workflows/README.md
--rw-r--r--   0        0        0     2092 2022-11-04 20:06:31.909524 circuit_knitting_toolbox-0.0.0/.github/workflows/citation.yml
--rw-r--r--   0        0        0     1088 2022-11-04 20:06:31.909524 circuit_knitting_toolbox-0.0.0/.github/workflows/coverage.yml
--rw-r--r--   0        0        0      884 2022-11-04 20:06:31.909524 circuit_knitting_toolbox-0.0.0/.github/workflows/docs.yml
--rw-r--r--   0        0        0      569 2022-11-04 20:06:31.909524 circuit_knitting_toolbox-0.0.0/.github/workflows/lint.yml
--rw-r--r--   0        0        0      997 2022-11-04 20:06:31.909524 circuit_knitting_toolbox-0.0.0/.github/workflows/release.yml
--rw-r--r--   0        0        0     1175 2022-11-04 20:06:31.909524 circuit_knitting_toolbox-0.0.0/.github/workflows/test_development_versions.yml
--rw-r--r--   0        0        0     1142 2022-11-04 20:06:31.909524 circuit_knitting_toolbox-0.0.0/.github/workflows/test_latest_versions.yml
--rw-r--r--   0        0        0     1218 2022-11-04 20:06:31.909524 circuit_knitting_toolbox-0.0.0/.github/workflows/test_minimum_versions.yml
--rw-r--r--   0        0        0      580 2022-11-04 20:06:31.909524 circuit_knitting_toolbox-0.0.0/.gitignore
--rw-r--r--   0        0        0       79 2022-11-04 20:06:31.909524 circuit_knitting_toolbox-0.0.0/.mypy.ini
--rw-r--r--   0        0        0     6153 2022-11-04 20:06:31.909524 circuit_knitting_toolbox-0.0.0/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0      637 2022-11-04 20:06:31.909524 circuit_knitting_toolbox-0.0.0/Dockerfile
--rw-r--r--   0        0        0     3366 2022-11-04 20:06:31.909524 circuit_knitting_toolbox-0.0.0/INSTALL.rst
--rw-r--r--   0        0        0    11416 2022-11-04 20:06:31.909524 circuit_knitting_toolbox-0.0.0/LICENSE.txt
--rw-r--r--   0        0        0     4278 2022-11-04 20:06:31.909524 circuit_knitting_toolbox-0.0.0/README.md
--rw-r--r--   0        0        0      688 2022-11-04 20:06:31.909524 circuit_knitting_toolbox-0.0.0/circuit_knitting_toolbox/__init__.py
--rw-r--r--   0        0        0      671 2022-11-04 20:06:31.909524 circuit_knitting_toolbox-0.0.0/circuit_knitting_toolbox/circuit_cutting/__init__.py
--rw-r--r--   0        0        0     1020 2022-11-04 20:06:31.909524 circuit_knitting_toolbox-0.0.0/circuit_knitting_toolbox/circuit_cutting/wire_cutting/__init__.py
--rw-r--r--   0        0        0    21919 2022-11-04 20:06:31.909524 circuit_knitting_toolbox-0.0.0/circuit_knitting_toolbox/circuit_cutting/wire_cutting/mip_model.py
--rw-r--r--   0        0        0    36770 2022-11-04 20:06:31.909524 circuit_knitting_toolbox-0.0.0/circuit_knitting_toolbox/circuit_cutting/wire_cutting/wire_cutting.py
--rw-r--r--   0        0        0    14328 2022-11-04 20:06:31.909524 circuit_knitting_toolbox-0.0.0/circuit_knitting_toolbox/circuit_cutting/wire_cutting/wire_cutting_evaluation.py
--rw-r--r--   0        0        0    18195 2022-11-04 20:06:31.909524 circuit_knitting_toolbox-0.0.0/circuit_knitting_toolbox/circuit_cutting/wire_cutting/wire_cutting_post_processing.py
--rw-r--r--   0        0        0     5889 2022-11-04 20:06:31.913524 circuit_knitting_toolbox-0.0.0/circuit_knitting_toolbox/circuit_cutting/wire_cutting/wire_cutting_verification.py
--rw-r--r--   0        0        0     1617 2022-11-04 20:06:31.913524 circuit_knitting_toolbox-0.0.0/circuit_knitting_toolbox/entanglement_forging/__init__.py
--rw-r--r--   0        0        0    18282 2022-11-04 20:06:31.913524 circuit_knitting_toolbox-0.0.0/circuit_knitting_toolbox/entanglement_forging/cholesky_decomposition.py
--rw-r--r--   0        0        0     6779 2022-11-04 20:06:31.913524 circuit_knitting_toolbox-0.0.0/circuit_knitting_toolbox/entanglement_forging/entanglement_forging_ansatz.py
--rw-r--r--   0        0        0    16945 2022-11-04 20:06:31.913524 circuit_knitting_toolbox-0.0.0/circuit_knitting_toolbox/entanglement_forging/entanglement_forging_ground_state_solver.py
--rw-r--r--   0        0        0    30984 2022-11-04 20:06:31.913524 circuit_knitting_toolbox-0.0.0/circuit_knitting_toolbox/entanglement_forging/entanglement_forging_knitter.py
--rw-r--r--   0        0        0     3302 2022-11-04 20:06:31.913524 circuit_knitting_toolbox-0.0.0/circuit_knitting_toolbox/entanglement_forging/entanglement_forging_operator.py
--rw-r--r--   0        0        0      817 2022-11-04 20:06:31.913524 circuit_knitting_toolbox-0.0.0/circuit_knitting_toolbox/utils/__init__.py
--rw-r--r--   0        0        0     3875 2022-11-04 20:06:31.913524 circuit_knitting_toolbox-0.0.0/circuit_knitting_toolbox/utils/conversion.py
--rw-r--r--   0        0        0     3545 2022-11-04 20:06:31.913524 circuit_knitting_toolbox-0.0.0/circuit_knitting_toolbox/utils/integral_driver.py
--rw-r--r--   0        0        0     7993 2022-11-04 20:06:31.913524 circuit_knitting_toolbox-0.0.0/circuit_knitting_toolbox/utils/metrics.py
--rw-r--r--   0        0        0     1345 2022-11-04 20:06:31.913524 circuit_knitting_toolbox-0.0.0/circuit_knitting_toolbox/utils/orbital_reduction.py
--rw-r--r--   0        0        0      339 2022-11-04 20:06:31.913524 circuit_knitting_toolbox-0.0.0/docker-compose.yml
--rw-r--r--   0        0        0     4062 2022-11-04 20:06:31.913524 circuit_knitting_toolbox-0.0.0/docs/_static/gallery.css
--rw-r--r--   0        0        0     5285 2022-11-04 20:06:31.913524 circuit_knitting_toolbox-0.0.0/docs/_static/no_image.png
--rw-r--r--   0        0        0      194 2022-11-04 20:06:31.913524 circuit_knitting_toolbox-0.0.0/docs/apidocs/circuit_cutting.rst
--rw-r--r--   0        0        0      219 2022-11-04 20:06:31.913524 circuit_knitting_toolbox-0.0.0/docs/apidocs/entanglement_forging.rst
--rw-r--r--   0        0        0      271 2022-11-04 20:06:31.913524 circuit_knitting_toolbox-0.0.0/docs/apidocs/index.rst
--rw-r--r--   0        0        0      156 2022-11-04 20:06:31.913524 circuit_knitting_toolbox-0.0.0/docs/apidocs/utils.rst
--rw-r--r--   0        0        0     2053 2022-11-04 20:06:31.913524 circuit_knitting_toolbox-0.0.0/docs/conf.py
--rw-r--r--   0        0        0      347 2022-11-04 20:06:31.913524 circuit_knitting_toolbox-0.0.0/docs/explanation/circuit_cutting/index.rst
--rw-r--r--   0        0        0    19307 2022-11-04 20:06:31.913524 circuit_knitting_toolbox-0.0.0/docs/explanation/entanglement_forging/figs/Fig_5_c.png
--rw-r--r--   0        0        0   200296 2022-11-04 20:06:31.913524 circuit_knitting_toolbox-0.0.0/docs/explanation/entanglement_forging/figs/forging_info_graphic.png
--rw-r--r--   0        0        0    16573 2022-11-04 20:06:31.913524 circuit_knitting_toolbox-0.0.0/docs/explanation/entanglement_forging/index.rst
--rw-r--r--   0        0        0      211 2022-11-04 20:06:31.913524 circuit_knitting_toolbox-0.0.0/docs/explanation/index.rst
--rw-r--r--   0        0        0      102 2022-11-04 20:06:31.913524 circuit_knitting_toolbox-0.0.0/docs/how-tos/circuit_cutting/index.rst
--rw-r--r--   0        0        0    13858 2022-11-04 20:06:31.913524 circuit_knitting_toolbox-0.0.0/docs/how-tos/entanglement_forging/freeze-orbitals.ipynb
--rw-r--r--   0        0        0      288 2022-11-04 20:06:31.913524 circuit_knitting_toolbox-0.0.0/docs/how-tos/entanglement_forging/index.rst
--rw-r--r--   0        0        0     1354 2022-11-04 20:06:31.913524 circuit_knitting_toolbox-0.0.0/docs/how-tos/entanglement_forging/specify-problem.rst
--rw-r--r--   0        0        0    19853 2022-11-04 20:06:31.913524 circuit_knitting_toolbox-0.0.0/docs/how-tos/entanglement_forging/use-asymmetric-bitstrings.ipynb
--rw-r--r--   0        0        0      194 2022-11-04 20:06:31.913524 circuit_knitting_toolbox-0.0.0/docs/how-tos/index.rst
--rw-r--r--   0        0        0     2561 2022-11-04 20:06:31.913524 circuit_knitting_toolbox-0.0.0/docs/index.rst
--rw-r--r--   0        0        0       28 2022-11-04 20:06:31.913524 circuit_knitting_toolbox-0.0.0/docs/install.rst
--rw-r--r--   0        0        0      550 2022-11-04 20:06:31.917524 circuit_knitting_toolbox-0.0.0/docs/tutorials/circuit_cutting/README.rst
--rw-r--r--   0        0        0   120601 2022-11-04 20:06:31.917524 circuit_knitting_toolbox-0.0.0/docs/tutorials/circuit_cutting/img/how-to-manual-cut.png
--rw-r--r--   0        0        0      146 2022-11-04 20:06:31.917524 circuit_knitting_toolbox-0.0.0/docs/tutorials/circuit_cutting/index.rst
--rw-r--r--   0        0        0   164415 2022-11-04 20:06:31.917524 circuit_knitting_toolbox-0.0.0/docs/tutorials/circuit_cutting/tutorial_1_automatic_cut_finding.ipynb
--rw-r--r--   0        0        0   262634 2022-11-04 20:06:31.921524 circuit_knitting_toolbox-0.0.0/docs/tutorials/circuit_cutting/tutorial_2_manual_cutting.ipynb
--rw-r--r--   0        0        0   173267 2022-11-04 20:06:31.921524 circuit_knitting_toolbox-0.0.0/docs/tutorials/circuit_cutting/tutorial_3_cutting_with_quantum_serverless.ipynb
--rw-r--r--   0        0        0     1686 2022-11-04 20:06:31.921524 circuit_knitting_toolbox-0.0.0/docs/tutorials/entanglement_forging/data/reactant_2mo.npz
--rw-r--r--   0        0        0      215 2022-11-04 20:06:31.921524 circuit_knitting_toolbox-0.0.0/docs/tutorials/entanglement_forging/index.rst
--rw-r--r--   0        0        0    83401 2022-11-04 20:06:31.921524 circuit_knitting_toolbox-0.0.0/docs/tutorials/entanglement_forging/tutorial_1_getting_started.ipynb
--rw-r--r--   0        0        0   104233 2022-11-04 20:06:31.921524 circuit_knitting_toolbox-0.0.0/docs/tutorials/entanglement_forging/tutorial_2_forging_with_quantum_serverless.ipynb
--rw-r--r--   0        0        0      174 2022-11-04 20:06:31.921524 circuit_knitting_toolbox-0.0.0/docs/tutorials/index.rst
--rw-r--r--   0        0        0     1690 2022-11-04 20:06:31.921524 circuit_knitting_toolbox-0.0.0/pyproject.toml
--rw-r--r--   0        0        0      475 2022-11-04 20:06:31.921524 circuit_knitting_toolbox-0.0.0/test/__init__.py
--rw-r--r--   0        0        0      475 2022-11-04 20:06:31.921524 circuit_knitting_toolbox-0.0.0/test/circuit_cutting/__init__.py
--rw-r--r--   0        0        0     2475 2022-11-04 20:06:31.921524 circuit_knitting_toolbox-0.0.0/test/circuit_cutting/test_circuit_cutting.py
--rw-r--r--   0        0        0      475 2022-11-04 20:06:31.921524 circuit_knitting_toolbox-0.0.0/test/entanglement_forging/__init__.py
--rw-r--r--   0        0        0      416 2022-11-04 20:06:31.921524 circuit_knitting_toolbox-0.0.0/test/entanglement_forging/test_data/CH3_one_body.npy
--rw-r--r--   0        0        0    10496 2022-11-04 20:06:31.921524 circuit_knitting_toolbox-0.0.0/test/entanglement_forging/test_data/CH3_two_body.npy
--rw-r--r--   0        0        0      640 2022-11-04 20:06:31.921524 circuit_knitting_toolbox-0.0.0/test/entanglement_forging/test_data/CN_one_body.npy
--rw-r--r--   0        0        0    32896 2022-11-04 20:06:31.921524 circuit_knitting_toolbox-0.0.0/test/entanglement_forging/test_data/CN_two_body.npy
--rw-r--r--   0        0        0      640 2022-11-04 20:06:31.921524 circuit_knitting_toolbox-0.0.0/test/entanglement_forging/test_data/O2_one_body.npy
--rw-r--r--   0        0        0    32896 2022-11-04 20:06:31.921524 circuit_knitting_toolbox-0.0.0/test/entanglement_forging/test_data/O2_two_body.npy
--rw-r--r--   0        0        0     2393 2022-11-04 20:06:31.921524 circuit_knitting_toolbox-0.0.0/test/entanglement_forging/test_entanglement_forging_ground_state_solver.py
--rw-r--r--   0        0        0    13478 2022-11-04 20:06:31.921524 circuit_knitting_toolbox-0.0.0/test/entanglement_forging/test_entanglement_forging_knitter.py
--rwxr-xr-x   0        0        0     2825 2022-11-04 20:06:31.921524 circuit_knitting_toolbox-0.0.0/tools/extremal_dependency_versions.py
--rw-r--r--   0        0        0     1720 2022-11-04 20:06:31.921524 circuit_knitting_toolbox-0.0.0/tox.ini
--rw-r--r--   0        0        0     6321 1970-01-01 00:00:00.000000 circuit_knitting_toolbox-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0       21 2023-05-05 23:57:07.625493 circuit-knitting-toolbox-0.1.0/.dockerignore
+-rw-r--r--   0        0        0      118 2023-05-05 23:57:07.625493 circuit-knitting-toolbox-0.1.0/.github/dependabot.yml
+-rw-r--r--   0        0        0     3711 2023-05-05 23:57:07.625493 circuit-knitting-toolbox-0.1.0/.github/workflows/README.md
+-rw-r--r--   0        0        0     2092 2023-05-05 23:57:07.625493 circuit-knitting-toolbox-0.1.0/.github/workflows/citation.yml
+-rw-r--r--   0        0        0     1112 2023-05-05 23:57:07.625493 circuit-knitting-toolbox-0.1.0/.github/workflows/coverage.yml
+-rw-r--r--   0        0        0      562 2023-05-05 23:57:07.625493 circuit-knitting-toolbox-0.1.0/.github/workflows/docker.yml
+-rw-r--r--   0        0        0      923 2023-05-05 23:57:07.625493 circuit-knitting-toolbox-0.1.0/.github/workflows/docs.yml
+-rw-r--r--   0        0        0      608 2023-05-05 23:57:07.625493 circuit-knitting-toolbox-0.1.0/.github/workflows/lint.yml
+-rw-r--r--   0        0        0      997 2023-05-05 23:57:07.625493 circuit-knitting-toolbox-0.1.0/.github/workflows/release.yml
+-rw-r--r--   0        0        0     1175 2023-05-05 23:57:07.625493 circuit-knitting-toolbox-0.1.0/.github/workflows/test_development_versions.yml
+-rw-r--r--   0        0        0     1495 2023-05-05 23:57:07.625493 circuit-knitting-toolbox-0.1.0/.github/workflows/test_latest_versions.yml
+-rw-r--r--   0        0        0     1218 2023-05-05 23:57:07.625493 circuit-knitting-toolbox-0.1.0/.github/workflows/test_minimum_versions.yml
+-rw-r--r--   0        0        0      580 2023-05-05 23:57:07.625493 circuit-knitting-toolbox-0.1.0/.gitignore
+-rw-r--r--   0        0        0       79 2023-05-05 23:57:07.625493 circuit-knitting-toolbox-0.1.0/.mypy.ini
+-rw-r--r--   0        0        0      199 2023-05-05 23:57:07.625493 circuit-knitting-toolbox-0.1.0/.ruff.toml
+-rw-r--r--   0        0        0      664 2023-05-05 23:57:07.625493 circuit-knitting-toolbox-0.1.0/CITATION.bib
+-rw-r--r--   0        0        0     6153 2023-05-05 23:57:07.625493 circuit-knitting-toolbox-0.1.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0      619 2023-05-05 23:57:07.625493 circuit-knitting-toolbox-0.1.0/Dockerfile
+-rw-r--r--   0        0        0     3707 2023-05-05 23:57:07.625493 circuit-knitting-toolbox-0.1.0/INSTALL.rst
+-rw-r--r--   0        0        0    11416 2023-05-05 23:57:07.625493 circuit-knitting-toolbox-0.1.0/LICENSE.txt
+-rw-r--r--   0        0        0     4687 2023-05-05 23:57:07.625493 circuit-knitting-toolbox-0.1.0/README.md
+-rw-r--r--   0        0        0      927 2023-05-05 23:57:07.625493 circuit-knitting-toolbox-0.1.0/circuit_knitting_toolbox/__init__.py
+-rw-r--r--   0        0        0      923 2023-05-05 23:57:07.625493 circuit-knitting-toolbox-0.1.0/circuit_knitting_toolbox/circuit_cutting/__init__.py
+-rw-r--r--   0        0        0     1020 2023-05-05 23:57:07.625493 circuit-knitting-toolbox-0.1.0/circuit_knitting_toolbox/circuit_cutting/wire_cutting/__init__.py
+-rw-r--r--   0        0        0    22382 2023-05-05 23:57:07.625493 circuit-knitting-toolbox-0.1.0/circuit_knitting_toolbox/circuit_cutting/wire_cutting/mip_model.py
+-rw-r--r--   0        0        0    37295 2023-05-05 23:57:07.625493 circuit-knitting-toolbox-0.1.0/circuit_knitting_toolbox/circuit_cutting/wire_cutting/wire_cutting.py
+-rw-r--r--   0        0        0    14798 2023-05-05 23:57:07.625493 circuit-knitting-toolbox-0.1.0/circuit_knitting_toolbox/circuit_cutting/wire_cutting/wire_cutting_evaluation.py
+-rw-r--r--   0        0        0    18166 2023-05-05 23:57:07.625493 circuit-knitting-toolbox-0.1.0/circuit_knitting_toolbox/circuit_cutting/wire_cutting/wire_cutting_post_processing.py
+-rw-r--r--   0        0        0     5902 2023-05-05 23:57:07.625493 circuit-knitting-toolbox-0.1.0/circuit_knitting_toolbox/circuit_cutting/wire_cutting/wire_cutting_verification.py
+-rw-r--r--   0        0        0     1617 2023-05-05 23:57:07.625493 circuit-knitting-toolbox-0.1.0/circuit_knitting_toolbox/entanglement_forging/__init__.py
+-rw-r--r--   0        0        0    15773 2023-05-05 23:57:07.625493 circuit-knitting-toolbox-0.1.0/circuit_knitting_toolbox/entanglement_forging/cholesky_decomposition.py
+-rw-r--r--   0        0        0     6793 2023-05-05 23:57:07.625493 circuit-knitting-toolbox-0.1.0/circuit_knitting_toolbox/entanglement_forging/entanglement_forging_ansatz.py
+-rw-r--r--   0        0        0    15253 2023-05-05 23:57:07.625493 circuit-knitting-toolbox-0.1.0/circuit_knitting_toolbox/entanglement_forging/entanglement_forging_ground_state_solver.py
+-rw-r--r--   0        0        0    29419 2023-05-05 23:57:07.625493 circuit-knitting-toolbox-0.1.0/circuit_knitting_toolbox/entanglement_forging/entanglement_forging_knitter.py
+-rw-r--r--   0        0        0     3137 2023-05-05 23:57:07.625493 circuit-knitting-toolbox-0.1.0/circuit_knitting_toolbox/entanglement_forging/entanglement_forging_operator.py
+-rw-r--r--   0        0        0      717 2023-05-05 23:57:07.625493 circuit-knitting-toolbox-0.1.0/circuit_knitting_toolbox/utils/__init__.py
+-rw-r--r--   0        0        0     3875 2023-05-05 23:57:07.625493 circuit-knitting-toolbox-0.1.0/circuit_knitting_toolbox/utils/conversion.py
+-rw-r--r--   0        0        0     7993 2023-05-05 23:57:07.625493 circuit-knitting-toolbox-0.1.0/circuit_knitting_toolbox/utils/metrics.py
+-rw-r--r--   0        0        0     1347 2023-05-05 23:57:07.625493 circuit-knitting-toolbox-0.1.0/circuit_knitting_toolbox/utils/orbital_reduction.py
+-rw-r--r--   0        0        0      365 2023-05-05 23:57:07.625493 circuit-knitting-toolbox-0.1.0/docker-compose.yml
+-rw-r--r--   0        0        0     4062 2023-05-05 23:57:07.625493 circuit-knitting-toolbox-0.1.0/docs/_static/gallery.css
+-rw-r--r--   0        0        0     5285 2023-05-05 23:57:07.625493 circuit-knitting-toolbox-0.1.0/docs/_static/no_image.png
+-rw-r--r--   0        0        0      194 2023-05-05 23:57:07.629493 circuit-knitting-toolbox-0.1.0/docs/apidocs/circuit_cutting.rst
+-rw-r--r--   0        0        0      219 2023-05-05 23:57:07.629493 circuit-knitting-toolbox-0.1.0/docs/apidocs/entanglement_forging.rst
+-rw-r--r--   0        0        0      271 2023-05-05 23:57:07.629493 circuit-knitting-toolbox-0.1.0/docs/apidocs/index.rst
+-rw-r--r--   0        0        0      156 2023-05-05 23:57:07.629493 circuit-knitting-toolbox-0.1.0/docs/apidocs/utils.rst
+-rw-r--r--   0        0        0      347 2023-05-05 23:57:07.629493 circuit-knitting-toolbox-0.1.0/docs/circuit_cutting/explanation/index.rst
+-rw-r--r--   0        0        0      102 2023-05-05 23:57:07.629493 circuit-knitting-toolbox-0.1.0/docs/circuit_cutting/how-tos/index.rst
+-rw-r--r--   0        0        0      550 2023-05-05 23:57:07.629493 circuit-knitting-toolbox-0.1.0/docs/circuit_cutting/tutorials/README.rst
+-rw-r--r--   0        0        0      146 2023-05-05 23:57:07.629493 circuit-knitting-toolbox-0.1.0/docs/circuit_cutting/tutorials/index.rst
+-rw-r--r--   0        0        0   164415 2023-05-05 23:57:07.629493 circuit-knitting-toolbox-0.1.0/docs/circuit_cutting/tutorials/tutorial_1_automatic_cut_finding.ipynb
+-rw-r--r--   0        0        0   262634 2023-05-05 23:57:07.629493 circuit-knitting-toolbox-0.1.0/docs/circuit_cutting/tutorials/tutorial_2_manual_cutting.ipynb
+-rw-r--r--   0        0        0   171432 2023-05-05 23:57:07.629493 circuit-knitting-toolbox-0.1.0/docs/circuit_cutting/tutorials/tutorial_3_cutting_with_quantum_serverless.ipynb
+-rw-r--r--   0        0        0     2041 2023-05-05 23:57:07.629493 circuit-knitting-toolbox-0.1.0/docs/conf.py
+-rw-r--r--   0        0        0    19307 2023-05-05 23:57:07.629493 circuit-knitting-toolbox-0.1.0/docs/entanglement_forging/explanation/figs/Fig_5_c.png
+-rw-r--r--   0        0        0   200296 2023-05-05 23:57:07.633493 circuit-knitting-toolbox-0.1.0/docs/entanglement_forging/explanation/figs/forging_info_graphic.png
+-rw-r--r--   0        0        0    12930 2023-05-05 23:57:07.633493 circuit-knitting-toolbox-0.1.0/docs/entanglement_forging/explanation/index.rst
+-rw-r--r--   0        0        0    11722 2023-05-05 23:57:07.633493 circuit-knitting-toolbox-0.1.0/docs/entanglement_forging/how-tos/freeze-orbitals.ipynb
+-rw-r--r--   0        0        0      310 2023-05-05 23:57:07.633493 circuit-knitting-toolbox-0.1.0/docs/entanglement_forging/how-tos/index.rst
+-rw-r--r--   0        0        0     1354 2023-05-05 23:57:07.633493 circuit-knitting-toolbox-0.1.0/docs/entanglement_forging/how-tos/specify-problem.rst
+-rw-r--r--   0        0        0    18145 2023-05-05 23:57:07.633493 circuit-knitting-toolbox-0.1.0/docs/entanglement_forging/how-tos/use-asymmetric-bitstrings.ipynb
+-rw-r--r--   0        0        0     1686 2023-05-05 23:57:07.633493 circuit-knitting-toolbox-0.1.0/docs/entanglement_forging/tutorials/data/reactant_2mo.npz
+-rw-r--r--   0        0        0      239 2023-05-05 23:57:07.633493 circuit-knitting-toolbox-0.1.0/docs/entanglement_forging/tutorials/index.rst
+-rw-r--r--   0        0        0    81343 2023-05-05 23:57:07.633493 circuit-knitting-toolbox-0.1.0/docs/entanglement_forging/tutorials/tutorial_1_getting_started.ipynb
+-rw-r--r--   0        0        0   100607 2023-05-05 23:57:07.633493 circuit-knitting-toolbox-0.1.0/docs/entanglement_forging/tutorials/tutorial_2_forging_with_quantum_serverless.ipynb
+-rw-r--r--   0        0        0     2927 2023-05-05 23:57:07.633493 circuit-knitting-toolbox-0.1.0/docs/index.rst
+-rw-r--r--   0        0        0       28 2023-05-05 23:57:07.633493 circuit-knitting-toolbox-0.1.0/docs/install.rst
+-rw-r--r--   0        0        0       53 2023-05-05 23:57:07.633493 circuit-knitting-toolbox-0.1.0/docs/release-notes.rst
+-rw-r--r--   0        0        0     2611 2023-05-05 23:57:07.633493 circuit-knitting-toolbox-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0       40 2023-05-05 23:57:07.633493 circuit-knitting-toolbox-0.1.0/releasenotes/config.yaml
+-rw-r--r--   0        0        0      401 2023-05-05 23:57:07.633493 circuit-knitting-toolbox-0.1.0/releasenotes/notes/0.1/dep-versions-383f4a21044cf599.yaml
+-rw-r--r--   0        0        0      177 2023-05-05 23:57:07.633493 circuit-knitting-toolbox-0.1.0/releasenotes/notes/0.1/deprecate-py37-5ef642682641aeb8.yaml
+-rw-r--r--   0        0        0     1060 2023-05-05 23:57:07.633493 circuit-knitting-toolbox-0.1.0/releasenotes/notes/0.1/migrate-to-qiskit-nature-0.5.0-96e90cd48f36d731.yaml
+-rw-r--r--   0        0        0      140 2023-05-05 23:57:07.633493 circuit-knitting-toolbox-0.1.0/releasenotes/notes/0.1/optional-cplex-f578dabd9d1a83f8.yaml
+-rw-r--r--   0        0        0       38 2023-05-05 23:57:07.633493 circuit-knitting-toolbox-0.1.0/setup.py
+-rw-r--r--   0        0        0      475 2023-05-05 23:57:07.633493 circuit-knitting-toolbox-0.1.0/test/__init__.py
+-rw-r--r--   0        0        0      475 2023-05-05 23:57:07.633493 circuit-knitting-toolbox-0.1.0/test/circuit_cutting/__init__.py
+-rw-r--r--   0        0        0     2630 2023-05-05 23:57:07.633493 circuit-knitting-toolbox-0.1.0/test/circuit_cutting/test_circuit_cutting.py
+-rw-r--r--   0        0        0      475 2023-05-05 23:57:07.633493 circuit-knitting-toolbox-0.1.0/test/entanglement_forging/__init__.py
+-rw-r--r--   0        0        0      416 2023-05-05 23:57:07.633493 circuit-knitting-toolbox-0.1.0/test/entanglement_forging/test_data/CH3_one_body.npy
+-rw-r--r--   0        0        0    10496 2023-05-05 23:57:07.633493 circuit-knitting-toolbox-0.1.0/test/entanglement_forging/test_data/CH3_two_body.npy
+-rw-r--r--   0        0        0      640 2023-05-05 23:57:07.633493 circuit-knitting-toolbox-0.1.0/test/entanglement_forging/test_data/CN_one_body.npy
+-rw-r--r--   0        0        0    32896 2023-05-05 23:57:07.633493 circuit-knitting-toolbox-0.1.0/test/entanglement_forging/test_data/CN_two_body.npy
+-rw-r--r--   0        0        0      640 2023-05-05 23:57:07.633493 circuit-knitting-toolbox-0.1.0/test/entanglement_forging/test_data/O2_one_body.npy
+-rw-r--r--   0        0        0    32896 2023-05-05 23:57:07.633493 circuit-knitting-toolbox-0.1.0/test/entanglement_forging/test_data/O2_two_body.npy
+-rw-r--r--   0        0        0     2575 2023-05-05 23:57:07.633493 circuit-knitting-toolbox-0.1.0/test/entanglement_forging/test_entanglement_forging_ground_state_solver.py
+-rw-r--r--   0        0        0    13312 2023-05-05 23:57:07.637493 circuit-knitting-toolbox-0.1.0/test/entanglement_forging/test_entanglement_forging_knitter.py
+-rwxr-xr-x   0        0        0     2818 2023-05-05 23:57:07.637493 circuit-knitting-toolbox-0.1.0/tools/extremal_dependency_versions.py
+-rw-r--r--   0        0        0     1904 2023-05-05 23:57:07.637493 circuit-knitting-toolbox-0.1.0/tox.ini
+-rw-r--r--   0        0        0     7801 1970-01-01 00:00:00.000000 circuit-knitting-toolbox-0.1.0/PKG-INFO
```

### Comparing `circuit_knitting_toolbox-0.0.0/.github/workflows/README.md` & `circuit-knitting-toolbox-0.1.0/.github/workflows/README.md`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.0.0/.github/workflows/citation.yml` & `circuit-knitting-toolbox-0.1.0/.github/workflows/citation.yml`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     paths: ['CITATION.bib', '.github/workflows/citation.yml']
 
 jobs:
   build-preview:
     runs-on: ubuntu-latest
     timeout-minutes: 30
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v3
       - name: Check for non-ASCII characters
         run: |
           # Fail immediately if there are any non-ASCII characters in
           # the BibTeX source.  We prefer "escaped codes" rather than
           # UTF-8 characters in order to ensure the bibliography will
           # display correctly even in documents that do not contain
           # \usepackage[utf8]{inputenc}.
@@ -59,11 +59,11 @@
         run: |
           if [ -f "CITATION.bib" ]; then
           pdflatex preview
           pdflatex preview
           fi
       - name: Upload PDF
         if: always()
-        uses: actions/upload-artifact@v2
+        uses: actions/upload-artifact@v3
         with:
           name: preview.pdf
           path: preview.pdf
```

### Comparing `circuit_knitting_toolbox-0.0.0/.github/workflows/coverage.yml` & `circuit-knitting-toolbox-0.1.0/.github/workflows/coverage.yml`

 * *Files 5% similar despite different names*

```diff
@@ -17,26 +17,27 @@
     timeout-minutes: 30
     strategy:
       max-parallel: 4
       matrix:
         os: [ubuntu-latest]
         python-version: ["3.10"]
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v3
       - name: Set up Python ${{ matrix.python-version }}
-        uses: actions/setup-python@v2
+        uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
       - name: Install tox
         run: |
           python -m pip install --upgrade pip
-          pip install tox coveragepy-lcov
+          pip install tox coveragepy-lcov 'coverage<7'
       - name: Run coverage
         run: |
           tox -e coverage
       - name: Convert to lcov
         run: coveragepy-lcov --output_file_path coveralls.info
       - name: Upload report to Coveralls
-        uses: coverallsapp/github-action@master
+        uses: coverallsapp/github-action@v2
         with:
           github-token: ${{ secrets.GITHUB_TOKEN }}
-          path-to-lcov: coveralls.info
+          file: coveralls.info
+          format: lcov
```

### Comparing `circuit_knitting_toolbox-0.0.0/.github/workflows/lint.yml` & `circuit-knitting-toolbox-0.1.0/.github/workflows/lint.yml`

 * *Files 24% similar despite different names*

```diff
@@ -11,17 +11,19 @@
       - 'stable/**'
 
 jobs:
   lint:
     runs-on: ubuntu-latest
     timeout-minutes: 30
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v3
+        with:
+          fetch-depth: 0
       - name: Set up Python 3.9
-        uses: actions/setup-python@v2
+        uses: actions/setup-python@v4
         with:
           python-version: '3.9'
       - name: Install tox
         run: |
           python -m pip install --upgrade pip
           pip install tox
       - name: Run styles check
```

### Comparing `circuit_knitting_toolbox-0.0.0/.github/workflows/release.yml` & `circuit-knitting-toolbox-0.1.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.0.0/.github/workflows/test_development_versions.yml` & `circuit-knitting-toolbox-0.1.0/.github/workflows/test_development_versions.yml`

 * *Files 2% similar despite different names*

```diff
@@ -17,17 +17,17 @@
     runs-on: ubuntu-latest
     timeout-minutes: 30
     strategy:
       max-parallel: 4
       matrix:
         python-version: [3.9]
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v3
       - name: Set up Python ${{ matrix.python-version }}
-        uses: actions/setup-python@v1
+        uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
       - name: Install dependencies (development versions)
         shell: bash
         run: |
           python -m pip install --upgrade pip tox
           python -m pip install toml fire
```

### Comparing `circuit_knitting_toolbox-0.0.0/.github/workflows/test_latest_versions.yml` & `circuit-knitting-toolbox-0.1.0/.github/workflows/test_minimum_versions.yml`

 * *Files 17% similar despite different names*

```diff
@@ -1,43 +1,40 @@
-name: Latest version tests
+name: Minimum version tests
 
 on:
   push:
     branches:
       - main
       - 'stable/**'
   pull_request:
     branches:
       - main
       - 'stable/**'
-  schedule:
-    - cron: '0 1 * * *'
 
 jobs:
   tests:
-    runs-on: ${{ matrix.os }}
+    runs-on: ubuntu-latest
     timeout-minutes: 30
     strategy:
       max-parallel: 4
       matrix:
-        os: [ubuntu-latest]
-        python-version: ["3.7", "3.10"]
-        include:
-          - os: macos-latest
-            python-version: "3.7"
+        python-version: [3.7]
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v3
       - name: Set up Python ${{ matrix.python-version }}
-        uses: actions/setup-python@v1
+        uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
-      - name: Install dependencies
+      - name: Install dependencies (minimum versions)
+        shell: bash
         run: |
           python -m pip install --upgrade pip
-          pip install tox
+          python -m pip install toml fire
+          pip install "tox==$(./tools/extremal_dependency_versions.py get_tox_minversion)"
+          python tools/extremal_dependency_versions.py pin_dependencies min --inplace
       - name: Modify tox.ini for more thorough check
         shell: bash
         run: |
           sed -i.bak -E '/#.*CI:[[:space:]]*skip-next-line/I{N;d;}' tox.ini
           cat tox.ini
       - name: Test using tox environment
         shell: bash
```

### Comparing `circuit_knitting_toolbox-0.0.0/.gitignore` & `circuit-knitting-toolbox-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.0.0/CODE_OF_CONDUCT.md` & `circuit-knitting-toolbox-0.1.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.0.0/Dockerfile` & `circuit-knitting-toolbox-0.1.0/Dockerfile`

 * *Files 25% similar despite different names*

```diff
@@ -15,9 +15,8 @@
 USER ${NB_UID}
 
 # Consolidate the docs into the home directory
 RUN mkdir docs && \
     cp -a .src/circuit-knitting-toolbox/docs docs/circuit-knitting-toolbox
 
 # Pip install everything
-RUN pip install ipywidgets pylatexenc matplotlib \
-        -e .src/circuit-knitting-toolbox
+RUN pip install -e '.src/circuit-knitting-toolbox[notebook-dependencies]'
```

### Comparing `circuit_knitting_toolbox-0.0.0/INSTALL.rst` & `circuit-knitting-toolbox-0.1.0/INSTALL.rst`

 * *Files 8% similar despite different names*

```diff
@@ -5,17 +5,26 @@
 There are two options: installing locally or using within a Docker
 container.
 
 - If you are using Linux or macOS with an Intel chip (i.e., not the
   new M1 or M2 chips), everything should work natively, so we
   recommend the first option.
 - All users on ARM chips, as well as all Windows users, will have to
-  use the toolbox within Docker (the second option) for everything to
+  use the toolbox within Docker (the second option) for all features to
   work as designed.
 
+Specifically, the following features are unavailable on the
+aforementioned platforms:
+
+- The automatic wire cut search in the circuit cutting module
+  depends on cplex, which is only available on Intel chips and is not
+  yet available for Python 3.11.
+- The entanglement forging notebooks require pyscf, which does not
+  support Windows.
+
 Option 1: Local installation
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 -  **OPTIONAL** If a user wishes to use the circuit cutting tool to
    automatically find optimized wire cuts for a circuit too large for
    the free version of CPLEX, they should acquire a license and install
    the `full
```

### Comparing `circuit_knitting_toolbox-0.0.0/LICENSE.txt` & `circuit-knitting-toolbox-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.0.0/README.md` & `circuit-knitting-toolbox-0.1.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 <!-- SHIELDS -->
 <div align="left">
 
-  [![Stability](https://img.shields.io/badge/Stability-alpha-f4d03f.svg)](https://github.com/Qiskit-Extensions/quantum-serverless/releases)
+  [![Stability](https://img.shields.io/badge/Stability-alpha-f4d03f.svg)](https://github.com/Qiskit-Extensions/circuit-knitting-toolbox/releases)
   ![Platform](https://img.shields.io/badge/Platform-Linux%20%7C%20macOS-informational)
-  [![Python](https://img.shields.io/badge/Python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10-informational)](https://www.python.org/)
-  [![Qiskit](https://img.shields.io/badge/Qiskit-%E2%89%A5%200.39.0-6133BD)](https://github.com/Qiskit/qiskit)
-  [![Qiskit Nature](https://img.shields.io/badge/Qiskit%20Nature-%E2%89%A5%200.4.4-6133BD)](https://github.com/Qiskit/qiskit-nature)
+  [![Python](https://img.shields.io/badge/Python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-informational)](https://www.python.org/)
+  [![Qiskit](https://img.shields.io/badge/Qiskit-%E2%89%A5%200.42.1-6133BD)](https://github.com/Qiskit/qiskit)
+  [![Qiskit Nature](https://img.shields.io/badge/Qiskit%20Nature-%E2%89%A5%200.5.2-6133BD)](https://github.com/Qiskit/qiskit-nature)
 <br />
-  [![License](https://img.shields.io/github/license/qiskit-community/prototype-entanglement-forging?label=License)](LICENSE.txt)
+  [![License](https://img.shields.io/github/license/Qiskit-Extensions/circuit-knitting-toolbox?label=License)](LICENSE.txt)
+  [![Code style: Black](https://img.shields.io/badge/Code%20style-Black-000.svg)](https://github.com/psf/black)
   [![Tests](https://github.com/Qiskit-Extensions/circuit-knitting-toolbox/actions/workflows/test_latest_versions.yml/badge.svg)](https://github.com/Qiskit-Extensions/circuit-knitting-toolbox/actions/workflows/test_latest_versions.yml)
+  [![Coverage](https://coveralls.io/repos/github/Qiskit-Extensions/circuit-knitting-toolbox/badge.svg?branch=main)](https://coveralls.io/github/Qiskit-Extensions/circuit-knitting-toolbox?branch=main)
 
 # Circuit Knitting Toolbox
 
 ### Table of Contents
 
 * [About](#about)
 * [Documentation](#documentation)
@@ -40,15 +42,15 @@
 
 The documentation, including installation instructions, is available at https://qiskit-extensions.github.io/circuit-knitting-toolbox/.
 
 ----------------------------------------------------------------------------------------------------
 
 ### Deprecation Policy
 
-This project is meant to evolve rapidly and, as such, does not follow [Qiskit's deprecation policy](https://qiskit.org/documentation/contributing_to_qiskit.html#deprecation-policy).  We may occasionally make breaking changes in order to improve the user experience.  When possible, we will keep old interfaces and mark them as deprecated, as long as they can co-exist with the new ones.  Each substantial improvement, breaking change, or deprecation will be documented in the release notes.
+This project is meant to evolve rapidly and, as such, does not follow [Qiskit's deprecation policy](https://qiskit.org/documentation/contributing_to_qiskit.html#deprecation-policy).  We may occasionally make breaking changes in order to improve the user experience.  When possible, we will keep old interfaces and mark them as deprecated, as long as they can co-exist with the new ones.  Each substantial improvement, breaking change, or deprecation will be documented in the [release notes](https://qiskit-extensions.github.io/circuit-knitting-toolbox/release-notes.html).
 
 ----------------------------------------------------------------------------------------------------
 
 ### References
 
 [1] Andrew Eddins, Mario Motta, Tanvi P. Gujarati, Sergey Bravyi, Antonio Mezzacapo, Charles Hadfield, Sarah Sheldon, [Doubling the size of quantum simulators by entanglement forging](https://journals.aps.org/prxquantum/abstract/10.1103/PRXQuantum.3.010309). PRX Quantum 3, 010309 (2022).
```

### Comparing `circuit_knitting_toolbox-0.0.0/circuit_knitting_toolbox/__init__.py` & `circuit-knitting-toolbox-0.1.0/circuit_knitting_toolbox/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,11 +7,19 @@
 # of this source tree or at http://www.apache.org/licenses/LICENSE-2.0.
 # Any modifications or derivative works of this code must retain this
 # copyright notice, and modified files need to carry a notice indicating
 # that they have been altered from the originals.
 
 """Main Circuit Knitting Toolbox public functionality."""
 
-from qiskit_nature.settings import settings
+import sys
+import warnings
 
-# This will suppress a warning about an upcoming change in Qiskit Nature
-settings.dict_aux_operators = True
+
+if sys.version_info < (3, 8):  # pragma: no cover
+    warnings.warn(
+        "Using the Circuit Knitting Toolbox with Python 3.7 is deprecated."
+        "Support for Python 3.7 will be removed in the near future, as soon as "
+        "https://github.com/Qiskit-Extensions/circuit-knitting-toolbox/pull/80 "
+        "is merged.",
+        DeprecationWarning,
+    )
```

### Comparing `circuit_knitting_toolbox-0.0.0/circuit_knitting_toolbox/circuit_cutting/__init__.py` & `circuit-knitting-toolbox-0.1.0/circuit_knitting_toolbox/utils/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -6,15 +6,23 @@
 # obtain a copy of this license in the LICENSE.txt file in the root directory
 # of this source tree or at http://www.apache.org/licenses/LICENSE-2.0.
 # Any modifications or derivative works of this code must retain this
 # copyright notice, and modified files need to carry a notice indicating
 # that they have been altered from the originals.
 
 """
-Circuit Cutting (:mod:`circuit_knitting_toolbox.circuit_cutting`).
-
-.. currentmodule:: circuit_knitting_toolbox.circuit_cutting
+Utility functions.
 
 .. autosummary::
    :toctree: ../stubs/
    :nosignatures:
+
+   conversion
+   metrics
+   orbital_reduction.reduce_bitstrings
 """
+
+from .orbital_reduction import reduce_bitstrings
+
+__all__ = [
+    "reduce_bitstrings",
+]
```

### Comparing `circuit_knitting_toolbox-0.0.0/circuit_knitting_toolbox/circuit_cutting/wire_cutting/__init__.py` & `circuit-knitting-toolbox-0.1.0/circuit_knitting_toolbox/circuit_cutting/wire_cutting/__init__.py`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.0.0/circuit_knitting_toolbox/circuit_cutting/wire_cutting/mip_model.py` & `circuit-knitting-toolbox-0.1.0/circuit_knitting_toolbox/circuit_cutting/wire_cutting/mip_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,20 +6,30 @@
 # obtain a copy of this license in the LICENSE.txt file in the root directory
 # of this source tree or at http://www.apache.org/licenses/LICENSE-2.0.
 # Any modifications or derivative works of this code must retain this
 # copyright notice, and modified files need to carry a notice indicating
 # that they have been altered from the originals.
 
 """File containing the tools to find and manage the cuts."""
-from typing import Sequence, Dict, Tuple, Any, List
 
-from docplex.mp.model import Model
-from docplex.mp.utils import DOcplexException
+from __future__ import annotations
+
+from typing import Sequence, Any
+
 import numpy as np
 
+try:
+    from docplex.mp.model import Model
+    from docplex.mp.utils import DOcplexException
+except ModuleNotFoundError as ex:
+    raise ModuleNotFoundError(
+        "DOcplex is not installed.  For automatic cut finding to work, both "
+        "DOcplex and cplex must be available."
+    ) from ex
+
 
 class MIPModel(object):
     """
     Class to contain the model that manages the cut MIP.
 
     This class represents circuit cutting as a Mixed Integer Programming (MIP) problem
     that can then be solved (provably) optimally using a MIP solver. This is integrated
@@ -47,17 +57,17 @@
             to each node
         - model (docplex model): the model interface for CPLEX
     """
 
     def __init__(
         self,
         n_vertices: int,
-        edges: Sequence[Tuple[int]],
-        vertex_ids: Dict[str, int],
-        id_vertices: Dict[int, str],
+        edges: Sequence[tuple[int]],
+        vertex_ids: dict[str, int],
+        id_vertices: dict[int, str],
         num_subcircuit: int,
         max_subcircuit_width: int,
         max_subcircuit_cuts: int,
         max_subcircuit_size: int,
         num_qubits: int,
         max_cuts: int,
     ):
@@ -91,15 +101,15 @@
         self.num_subcircuit = num_subcircuit
         self.max_subcircuit_width = max_subcircuit_width
         self.max_subcircuit_cuts = max_subcircuit_cuts
         self.max_subcircuit_size = max_subcircuit_size
         self.num_qubits = num_qubits
         self.max_cuts = max_cuts
 
-        self.subcircuit_counter: Dict[int, Dict[str, Any]] = {}
+        self.subcircuit_counter: dict[int, dict[str, Any]] = {}
 
         """
         Count the number of input qubits directly connected to each node
         """
         self.vertex_weight = {}
         for node in self.vertex_ids:
             qargs = node.split(" ")
@@ -406,15 +416,15 @@
                 # self.model.setPWLObj(self.subcircuit_counter[subcircuit]['build_cost_exponent'], ptx, ptf)
 
         # self.model.setObjective(self.num_cuts,gp.GRB.MINIMIZE)
         self.model.set_objective("min", self.num_cuts)
 
     def pwl_exp(
         self, lb: int, ub: int, base: int, coefficient: int, integer_only: bool
-    ) -> Tuple[List[int], List[int]]:
+    ) -> tuple[list[int], list[int]]:
         """
         Approximate a nonlinear exponential function via a piecewise linear function.
 
         Args:
             - lb (int): lower bound
             - ub (int): upper bound
             - base (int): the base of the input exponential
@@ -433,15 +443,15 @@
         # print('x_range : {}, integer_only : {}'.format(x_range,integer_only))
         for x in x_range:
             y = coefficient * base**x
             ptx.append(x)
             ptf.append(y)
         return ptx, ptf
 
-    def check_graph(self, n_vertices: int, edges: Sequence[Tuple[int]]) -> None:
+    def check_graph(self, n_vertices: int, edges: Sequence[tuple[int]]) -> None:
         """
         Ensure circuit DAG is viable.
 
         This means that there are no oversized edges, that all edges are from viable nodes,
         and that the graph is otherwise a valid graph.
 
         Args:
@@ -486,31 +496,37 @@
         # print('model has %d variables, %d linear constraints,%d quadratic constraints, %d general constraints'
         # % (self.model.NumVars,self.model.NumConstrs, self.model.NumQConstrs, self.model.NumGenConstrs))
         print(
             "Exporting as a LP file to let you check the model that will be solved : ",
             min_postprocessing_cost,
             str(type(min_postprocessing_cost)),
         )
-        self.model.export_as_lp(path="./docplex_cutter.lp")
+        try:
+            self.model.export_as_lp(path="./docplex_cutter.lp")
+        except RuntimeError:
+            print(
+                "The LP file export has failed.  This is known to happen sometimes "
+                "when cplex is not installed.  Now attempting to continue anyway."
+            )
         try:
             self.model.set_time_limit(300)
             if min_postprocessing_cost != float("inf"):
                 self.model.parameters.mip.tolerances.uppercutoff(
                     min_postprocessing_cost
                 )
             self.model.solve(log_output=True)
 
         except DOcplexException as e:
             print("Caught: " + e.message)
+            raise e
 
         if self.model._has_solution:
             my_solve_details = self.model.solve_details
-            self.objective = None
             self.subcircuits = []
-            self.optimal = self.model.get_solve_status() == "optimal"
+            self.optimal = my_solve_details.status == "optimal"
             self.runtime = my_solve_details.time
             self.node_count = my_solve_details.nb_nodes_processed
             self.mip_gap = my_solve_details.mip_relative_gap
             self.objective = self.model.objective_value
 
             for i in range(self.num_subcircuit):
                 subcircuit = []
```

### Comparing `circuit_knitting_toolbox-0.0.0/circuit_knitting_toolbox/circuit_cutting/wire_cutting/wire_cutting.py` & `circuit-knitting-toolbox-0.1.0/circuit_knitting_toolbox/circuit_cutting/wire_cutting/wire_cutting.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,47 @@
+# This code is a Qiskit project.
+
+# (C) Copyright IBM 2022.
+
+# This code is licensed under the Apache License, Version 2.0. You may
+# obtain a copy of this license in the LICENSE.txt file in the root directory
+# of this source tree or at http://www.apache.org/licenses/LICENSE-2.0.
+# Any modifications or derivative works of this code must retain this
+# copyright notice, and modified files need to carry a notice indicating
+# that they have been altered from the originals.
+
 """Functions for conducting the wire cutting on quantum circuits."""
-import typing
-from typing import Optional, Sequence, Any, Dict, Tuple, List, Union, cast
 
-from nptyping import NDArray
+from __future__ import annotations
+
+from typing import Sequence, Any, Dict, cast, no_type_check
 
+import numpy as np
 from qiskit import QuantumCircuit, QuantumRegister
 from qiskit.circuit import Qubit
 from qiskit.dagcircuit import DAGCircuit, DAGOpNode
 from qiskit.converters import circuit_to_dag, dag_to_circuit
 from qiskit_ibm_runtime import Options, QiskitRuntimeService
 
 from .wire_cutting_evaluation import run_subcircuit_instances
 from .wire_cutting_post_processing import generate_summation_terms, build
 from .wire_cutting_verification import generate_reconstructed_output
-from .mip_model import MIPModel
 
 
 def cut_circuit_wires(
     circuit: QuantumCircuit,
     method: str,
-    subcircuit_vertices: Optional[Sequence[Sequence[int]]] = None,
-    max_subcircuit_width: Optional[int] = None,
-    max_subcircuit_cuts: Optional[int] = None,
-    max_subcircuit_size: Optional[int] = None,
-    max_cuts: Optional[int] = None,
-    num_subcircuits: Optional[Sequence[int]] = None,
+    subcircuit_vertices: Sequence[Sequence[int]] | None = None,
+    max_subcircuit_width: int | None = None,
+    max_subcircuit_cuts: int | None = None,
+    max_subcircuit_size: int | None = None,
+    max_cuts: int | None = None,
+    num_subcircuits: Sequence[int] | None = None,
     verbose: bool = True,
-) -> Dict[str, Any]:
+) -> dict[str, Any]:
     """
     Decompose the circuit into a collection of subcircuits.
 
     Args:
         - method (str): whether to have the cuts be 'automatically' found, in a
             provably optimal way, or whether to 'manually' specify the cuts
         - subcircuit_vertices (Sequence[Sequence[int]]): the vertices to be used in
@@ -39,16 +50,16 @@
         - max_subcircuit_width (int): max number of qubits in each subcircuit
         - max_cuts (int): max total number of cuts allowed
         - num_subcircuits (Sequence[int]): list of number of subcircuits to try
         - max_subcircuit_cuts (int, optional): max number of cuts for a subcircuit
         - max_subcircuit_size (int, optional): max number of gates in a subcircuit
         - verbose (bool, optional): flag for printing output of cutting
     Returns:
-        - (Dict[str, Any]): A dictionary containing information on the cuts,
-            including the subcircuits themselves (key: 'subcircuits')
+        (dict[str, Any]): A dictionary containing information on the cuts,
+        including the subcircuits themselves (key: 'subcircuits')
     Raises:
         - ValueError: if the input method does not match the other provided arguments
     """
     cuts = {}
     if method == "automatic":
         if max_subcircuit_width is None:
             raise ValueError(
@@ -76,30 +87,30 @@
             'The method argument for the decompose method should be either "automatic" or "manual".'
         )
 
     return cuts
 
 
 def evaluate_subcircuits(
-    cuts: Dict[str, Any],
-    service: Optional[QiskitRuntimeService] = None,
-    backend_names: Optional[Union[str, Sequence[str]]] = None,
-    options: Optional[Union[Options, Sequence[Options]]] = None,
-) -> Dict[int, Dict[int, NDArray]]:
+    cuts: dict[str, Any],
+    service: QiskitRuntimeService | None = None,
+    backend_names: str | Sequence[str] | None = None,
+    options: Options | Sequence[Options] | None = None,
+) -> dict[int, dict[int, np.ndarray]]:
     """
     Evaluate the subcircuits.
 
     Args:
-        - cuts (Dict): the results of cutting
-        - service (QiskitRuntimeService): A service for connecting to Qiskit Runtime Service
-        - options (Union[Options, Sequence[Options]]): Options to use on each backend
-        - backend_names (Union[str, Sequence[str]]): The name(s) of the backend(s) to be used
+        - cuts (dict): the results of cutting
+        - service (QiskitRuntimeService | None): A service for connecting to Qiskit Runtime Service
+        - options (Options | Sequence[Options] | None): Options to use on each backend
+        - backend_names (str | Sequence[str] | None): The name(s) of the backend(s) to be used
     Returns:
-        - (Dict): the dictionary containing the results from running
-            each of the subcircuits
+        (dict): the dictionary containing the results from running
+        each of the subcircuits
     """
     # Put backend_names and options in lists to ensure it is unambiguous how to sync them
     backends_list: Sequence[str] = []
     options_list: Sequence[Options] = []
     if backend_names is None or isinstance(backend_names, str):
         if isinstance(options, Options):
             options_list = [options]
@@ -133,28 +144,28 @@
     )
 
     return subcircuit_instance_probabilities
 
 
 def reconstruct_full_distribution(
     circuit: QuantumCircuit,
-    subcircuit_instance_probabilities: Dict[int, Dict[int, NDArray]],
-    cuts: Dict[str, Any],
+    subcircuit_instance_probabilities: dict[int, dict[int, np.ndarray]],
+    cuts: dict[str, Any],
     num_threads: int = 1,
-) -> NDArray:
+) -> np.ndarray:
     """
     Reconstruct the full probabilities from the subcircuit evaluations.
 
     Args:
         - circuit (QuantumCircuit): the original full circuit
         - subcircuit_instance_probabilities (dict): the probability vectors from each
             of the subcircuit instances, as output by the _run_subcircuits function
         - num_threads (int): the number of threads to use to parallelize the recomposing
     Returns:
-        - (NDArray): the reconstructed probability vector
+        - (np.ndarray): the reconstructed probability vector
     """
     summation_terms, subcircuit_entries, _ = _generate_metadata(cuts)
 
     subcircuit_entry_probabilities = _attribute_shots(
         subcircuit_entries, subcircuit_instance_probabilities
     )
 
@@ -173,25 +184,25 @@
         cuts["complete_path_map"],
     )
 
     return reconstructed_probability
 
 
 def _generate_metadata(
-    cuts: Dict[str, Any]
-) -> Tuple[
-    List[Dict[int, int]],
-    Dict[int, Dict[Tuple[str, str], Tuple[int, Sequence[Tuple[int, int]]]]],
-    Dict[int, Dict[Tuple[Tuple[str, ...], Tuple[Any, ...]], int]],
+    cuts: dict[str, Any]
+) -> tuple[
+    list[dict[int, int]],
+    dict[int, dict[tuple[str, str], tuple[int, Sequence[tuple[int, int]]]]],
+    dict[int, dict[tuple[tuple[str, ...], tuple[Any, ...]], int]],
 ]:
     """
     Generate metadata used to execute subcircuits and reconstruct probabilities of original circuit.
 
     Args:
-        - cuts (Dict[str, Any]): results from the cutting step
+        - cuts (dict[str, Any]): results from the cutting step
     Returns:
         - (tuple): information about the 4^(num cuts) summation terms used to reconstruct original
             probabilities, a dictionary with information on each of the subcircuits, and a dictionary
             containing indexes for each of the subcircuits
     """
     (
         summation_terms,
@@ -202,81 +213,77 @@
         complete_path_map=cuts["complete_path_map"],
         num_cuts=cuts["num_cuts"],
     )
     return summation_terms, subcircuit_entries, subcircuit_instances
 
 
 def _run_subcircuits(
-    cuts: Dict[str, Any],
-    subcircuit_instances: Dict[int, Dict[Tuple[Tuple[str, ...], Tuple[Any, ...]], int]],
-    service: Optional[QiskitRuntimeService] = None,
-    backend_names: Optional[Sequence[str]] = None,
-    options: Optional[Sequence[Options]] = None,
-) -> Dict[int, Dict[int, NDArray]]:
+    cuts: dict[str, Any],
+    subcircuit_instances: dict[int, dict[tuple[tuple[str, ...], tuple[Any, ...]], int]],
+    service: QiskitRuntimeService | None = None,
+    backend_names: Sequence[str] | None = None,
+    options: Sequence[Options] | None = None,
+) -> dict[int, dict[int, np.ndarray]]:
     """
     Execute all the subcircuit instances.
 
     task['subcircuit_instance_probs'][subcircuit_idx][subcircuit_instance_idx] = measured prob
 
     Args:
-        - cuts (Dict[str, Any]): results from the cutting step
-        - subcircuit_instances (Dict): the dictionary containing the index information for each
+        - cuts (dict[str, Any]): results from the cutting step
+        - subcircuit_instances (dict): the dictionary containing the index information for each
             of the subcircuit instances
-        - service (QiskitRuntimeService): the arguments for the runtime service
-        - backend_names (Sequence[str]): the backend(s) used to run the subcircuits
-        - options (Options): options for the runtime execution of subcircuits
+        - service (QiskitRuntimeService | None): the arguments for the runtime service
+        - backend_names (Sequence[str] | None): the backend(s) used to run the subcircuits
+        - options (Options | None): options for the runtime execution of subcircuits
     Returns:
-        - (Dict): the resulting probabilities from each of the subcircuit instances
+        - (dict): the resulting probabilities from each of the subcircuit instances
     """
     subcircuit_instance_probs = run_subcircuit_instances(
         subcircuits=cuts["subcircuits"],
         subcircuit_instances=subcircuit_instances,
         service=service,
         backend_names=backend_names,
         options=options,
     )
 
     return subcircuit_instance_probs
 
 
 def _attribute_shots(
-    subcircuit_entries: Dict[
-        int, Dict[Tuple[str, str], Tuple[int, Sequence[Tuple[int, int]]]]
+    subcircuit_entries: dict[
+        int, dict[tuple[str, str], tuple[int, Sequence[tuple[int, int]]]]
     ],
-    subcircuit_instance_probs: Dict[int, Dict[int, NDArray]],
-) -> Dict[int, Dict[int, NDArray]]:
+    subcircuit_instance_probs: dict[int, dict[int, np.ndarray]],
+) -> dict[int, dict[int, np.ndarray]]:
     """
     Attribute the shots into respective subcircuit entries.
 
     task['subcircuit_entry_probs'][subcircuit_idx][subcircuit_entry_idx] = prob
 
     Args:
-        - subcircuit_entries (Dict): dictionary containing information about each of the
+        - subcircuit_entries (dict): dictionary containing information about each of the
             subcircuit instances
-        - subcircuit_instance_probs (Dict): the probability vectors from each of the subcircuit
+        - subcircuit_instance_probs (dict): the probability vectors from each of the subcircuit
             instances, as output by the _run_subcircuits function
     Returns:
-        - (Dict): a dictionary containing the probability results to each of the appropriate subcircuits
+        - (dict): a dictionary containing the probability results to each of the appropriate subcircuits
     Raises:
         - ValueError: if each of the kronecker terms are not of size two or if there are no subcircuit
             probs provided
     """
-    subcircuit_entry_probs: Dict[int, Dict[int, NDArray]] = {}
+    subcircuit_entry_probs: dict[int, dict[int, np.ndarray]] = {}
     for subcircuit_idx in subcircuit_entries:
         subcircuit_entry_probs[subcircuit_idx] = {}
         for label in subcircuit_entries[subcircuit_idx]:
             subcircuit_entry_idx, kronecker_term = subcircuit_entries[subcircuit_idx][
                 label
             ]
-            subcircuit_entry_prob: Optional[NDArray] = None
-            for term in kronecker_term:
-                if len(term) == 2:
-                    coefficient, subcircuit_instance_idx = cast(Tuple[int, int], term)
-                else:
-                    raise ValueError("Ill-formed Kronecker term: {term}")
+            subcircuit_entry_prob: np.ndarray | None = None
+            for coefficient, subcircuit_instance_idx in kronecker_term:
                 if subcircuit_entry_prob is None:
                     subcircuit_entry_prob = (
                         coefficient
                         * subcircuit_instance_probs[subcircuit_idx][
                             subcircuit_instance_idx
                         ]
                     )
@@ -295,24 +302,24 @@
             subcircuit_entry_probs[subcircuit_idx][
                 subcircuit_entry_idx
             ] = subcircuit_entry_prob
 
     return subcircuit_entry_probs
 
 
-@typing.no_type_check
+@no_type_check
 def find_wire_cuts(
     circuit: QuantumCircuit,
     max_subcircuit_width: int,
-    max_cuts: Optional[int],
-    num_subcircuits: Optional[Sequence[int]],
-    max_subcircuit_cuts: Optional[int],
-    max_subcircuit_size: Optional[int],
+    max_cuts: int | None,
+    num_subcircuits: Sequence[int] | None,
+    max_subcircuit_cuts: int | None,
+    max_subcircuit_size: int | None,
     verbose: bool,
-) -> Dict[str, Any]:
+) -> dict[str, Any]:
     """
     Find optimal cuts for the wires.
 
     Will print if the model cannot find a solution at all, and will print whether
     the found solution is optimal or not.
 
     Args:
@@ -352,14 +359,16 @@
             max_subcircuit_width=max_subcircuit_width,
             max_subcircuit_cuts=max_subcircuit_cuts,
             max_subcircuit_size=max_subcircuit_size,
             num_qubits=num_qubits,
             max_cuts=max_cuts,
         )
 
+        from .mip_model import MIPModel
+
         mip_model = MIPModel(**kwargs)
         feasible = mip_model.solve(min_postprocessing_cost=min_cost)
         if not feasible:
             if verbose:
                 print("%d subcircuits : NO SOLUTIONS" % (num_subcircuit))
             continue
         else:
@@ -383,14 +392,16 @@
                     "num_cuts": len(positions),
                     "counter": counter,
                     "classical_cost": classical_cost,
                 }
     if verbose and len(cut_solution) > 0:
         print("-" * 20)
         classical_cost: float = float(cut_solution["classical_cost"])
+        # We can remove typing.Dict from this cast statement when py38 is deprecated.
+        # https://bugs.python.org/issue45117
         counter = cast(Dict[int, Dict[str, int]], cut_solution["counter"])
         subcircuits: Sequence[Any] = cut_solution["subcircuits"]
         num_cuts: int = cut_solution["num_cuts"]
         _print_cutter_result(
             num_subcircuit=len(subcircuits),
             num_cuts=num_cuts,
             subcircuits=subcircuits,
@@ -411,15 +422,15 @@
             print("NOT OPTIMAL, MIP gap =", best_mip_model.mip_gap, flush=True)
         print("-" * 20, flush=True)
     return cut_solution
 
 
 def cut_circuit_wire(
     circuit: QuantumCircuit, subcircuit_vertices: Sequence[Sequence[int]], verbose: bool
-) -> Dict[str, Any]:
+) -> dict[str, Any]:
     """
     Perform the provided cuts.
 
     Used when cut locations are chosen manually.
 
     Args:
         - circuit (QuantumCircuit): original quantum circuit to be cut into subcircuits
@@ -475,15 +486,15 @@
     return cut_solution
 
 
 def _print_cutter_result(
     num_subcircuit: int,
     num_cuts: int,
     subcircuits: Sequence[QuantumCircuit],
-    counter: Dict[int, Dict[str, int]],
+    counter: dict[int, dict[str, int]],
     classical_cost: float,
 ) -> None:
     """
     Pretty print the results.
 
     Args:
         - num_subciruit (int): the number of subcircuits
@@ -509,16 +520,16 @@
             )
         )
         print(subcircuits[subcircuit_idx])
     print("Estimated cost = %.3e" % classical_cost, flush=True)
 
 
 def _cuts_parser(
-    cuts: Sequence[Tuple[str]], circ: QuantumCircuit
-) -> List[Tuple[Qubit, int]]:
+    cuts: Sequence[tuple[str]], circ: QuantumCircuit
+) -> list[tuple[Qubit, int]]:
     """
     Convert cuts to wires.
 
     Args:
         - cuts (list): the cuts found by the model (or provided by the user)
         - circ (QuantumCircuit): the quantum circuit the cuts are from
     Returns:
@@ -558,15 +569,17 @@
         for x in dest.split(" "):
             if x.split("]")[0] + "]" == qubit_cut[0]:
                 dest_idx = int(x.split("]")[1])
         multi_Q_gate_idx = max(source_idx, dest_idx)
 
         wire = None
         for qubit in circ.qubits:
-            if qubit.register.name == qubit_cut[0].split("[")[0] and qubit.index == int(
+            if circ.find_bit(qubit).registers[0][0].name == qubit_cut[0].split("[")[
+                0
+            ] and circ.find_bit(qubit).index == int(
                 qubit_cut[0].split("[")[1].split("]")[0]
             ):
                 wire = qubit
         tmp = 0
         all_Q_gate_idx = None
         for gate_idx, gate in enumerate(
             list(dag.nodes_on_wire(wire=wire, only_ops=True))
@@ -579,16 +592,16 @@
             raise ValueError("Something unexpected happened while parsing cuts.")
         positions.append((wire, all_Q_gate_idx))
     positions = sorted(positions, reverse=True, key=lambda cut: cut[1])
     return positions
 
 
 def _subcircuits_parser(
-    subcircuit_gates: List[List[str]], circuit: QuantumCircuit
-) -> Tuple[Sequence[QuantumCircuit], Dict[Qubit, List[Dict[str, Union[int, Qubit]]]]]:
+    subcircuit_gates: list[list[str]], circuit: QuantumCircuit
+) -> tuple[Sequence[QuantumCircuit], dict[Qubit, list[dict[str, int | Qubit]]]]:
     """
     Convert the subcircuit gates into quantum circuits and path out the DAGs to enable conversion.
 
     Args:
         - subcircuit_gates (list): the gates in the subcircuits
         - circuit (QuantumCircuit): the original circuit
     Returns:
@@ -622,47 +635,47 @@
     qubit_2qGate_depths = {x: 0 for x in circuit.qubits}
     gate_depth_encodings = {}
     # print('Before translation :',subcircuit_gates,flush=True)
     for op_node in dag.topological_op_nodes():
         gate_depth_encoding = ""
         for qarg in op_node.qargs:
             gate_depth_encoding += "%s[%d]%d " % (
-                qarg.register.name,
-                qarg.index,
+                circuit.find_bit(qarg).registers[0][0].name,
+                circuit.find_bit(qarg).index,
                 qubit_allGate_depths[qarg],
             )
         gate_depth_encoding = gate_depth_encoding[:-1]
         gate_depth_encodings[op_node] = gate_depth_encoding
         for qarg in op_node.qargs:
             qubit_allGate_depths[qarg] += 1
         if len(op_node.qargs) == 2:
             MIP_gate_depth_encoding = ""
             for qarg in op_node.qargs:
                 MIP_gate_depth_encoding += "%s[%d]%d " % (
-                    qarg.register.name,
-                    qarg.index,
+                    circuit.find_bit(qarg).registers[0][0].name,
+                    circuit.find_bit(qarg).index,
                     qubit_2qGate_depths[qarg],
                 )
                 qubit_2qGate_depths[qarg] += 1
             MIP_gate_depth_encoding = MIP_gate_depth_encoding[:-1]
             # print('gate_depth_encoding = %s, MIP_gate_depth_encoding = %s'%(gate_depth_encoding,MIP_gate_depth_encoding))
             for subcircuit_idx in range(len(subcircuit_gates)):
                 for gate_idx in range(len(subcircuit_gates[subcircuit_idx])):
                     if (
                         subcircuit_gates[subcircuit_idx][gate_idx]
                         == MIP_gate_depth_encoding
                     ):
                         subcircuit_gates[subcircuit_idx][gate_idx] = gate_depth_encoding
                         break
     # print('After translation :',subcircuit_gates,flush=True)
-    subcircuit_op_nodes: Dict[int, List[DAGOpNode]] = {
+    subcircuit_op_nodes: dict[int, list[DAGOpNode]] = {
         x: [] for x in range(len(subcircuit_gates))
     }
     subcircuit_sizes = [0 for x in range(len(subcircuit_gates))]
-    complete_path_map: Dict[Qubit, List[Dict[str, Union[int, Qubit]]]] = {}
+    complete_path_map: dict[Qubit, list[dict[str, int | Qubit]]] = {}
     for circuit_qubit in dag.qubits:
         complete_path_map[circuit_qubit] = []
         qubit_ops = dag.nodes_on_wire(wire=circuit_qubit, only_ops=True)
         for qubit_op_idx, qubit_op in enumerate(qubit_ops):
             gate_depth_encoding = gate_depth_encodings[qubit_op]
             nearest_subcircuit_idx = -1
             min_distance = float("inf")
@@ -713,16 +726,16 @@
         subcircuit_sizes=subcircuit_sizes,
         dag=dag,
     )
     return subcircuits, complete_path_map
 
 
 def _generate_subcircuits(
-    subcircuit_op_nodes: Dict[int, List[DAGOpNode]],
-    complete_path_map: Dict[Qubit, List[Dict[str, Union[int, Qubit]]]],
+    subcircuit_op_nodes: dict[int, list[DAGOpNode]],
+    complete_path_map: dict[Qubit, list[dict[str, int | Qubit]]],
     subcircuit_sizes: Sequence[int],
     dag: DAGCircuit,
 ) -> Sequence[QuantumCircuit]:
     """
     Generate the subcircuits from given nodes and paths.
 
     Called in the subcircuit_parser function to convert the found paths and nodes
@@ -767,18 +780,16 @@
             instruction=op_node.op, qargs=subcircuit_qargs, cargs=None
         )
     return subcircuits
 
 
 def _get_counter(
     subcircuits: Sequence[QuantumCircuit],
-    O_rho_pairs: List[
-        Tuple[Dict[str, Union[int, Qubit]], Dict[str, Union[int, Qubit]]]
-    ],
-) -> Dict[int, Dict[str, int]]:
+    O_rho_pairs: list[tuple[dict[str, int | Qubit], dict[str, int | Qubit]]],
+) -> dict[int, dict[str, int]]:
     """
     Create information regarding each of the subcircuit parameters (qubits, width, etc.).
 
     Args:
         - subcircuits (list): the list of subcircuits
         - O_rho_pairs (list): the pairs for each qubit path as generated in the _get_pairs
             function
@@ -792,26 +803,25 @@
             "rho": 0,
             "O": 0,
             "d": subcircuit.num_qubits,
             "depth": subcircuit.depth(),
             "size": subcircuit.size(),
         }
     for pair in O_rho_pairs:
-        Sequence[Tuple[Dict[str, Union[int, Qubit]]]]
         if len(pair) != 2:
             raise ValueError(f"O_rho_pairs must be length 2: {pair}")
         O_qubit = pair[0]
         rho_qubit = pair[-1]
         counter[O_qubit["subcircuit_idx"]]["effective"] -= 1
         counter[O_qubit["subcircuit_idx"]]["O"] += 1
         counter[rho_qubit["subcircuit_idx"]]["rho"] += 1
     return counter
 
 
-def _cost_estimate(counter: Dict[int, Dict[str, int]]) -> float:
+def _cost_estimate(counter: dict[int, dict[str, int]]) -> float:
     """
     Estimate the cost of processing the subcircuits.
 
     Args:
         - counter (dict): dictionary containing information for each of the
             subcircuits
     Returns:
@@ -831,16 +841,16 @@
         accumulated_kron_len *= 2**effective
         classical_cost += accumulated_kron_len
     classical_cost *= 4**num_cuts
     return classical_cost
 
 
 def _get_pairs(
-    complete_path_map: Dict[Qubit, List[Dict[str, Union[int, Qubit]]]]
-) -> List[Tuple[Dict[str, Union[int, Qubit]], Dict[str, Union[int, Qubit]]]]:
+    complete_path_map: dict[Qubit, list[dict[str, int | Qubit]]]
+) -> list[tuple[dict[str, int | Qubit], dict[str, int | Qubit]]]:
     """
     Get all pairs through each path.
 
     Iterates through the path for each of the qubits and keeps track of the
     each pair of neigbors.
 
     Args:
@@ -876,15 +886,15 @@
         if len(vertex.qargs) == 2 and vertex.op.name != "barrier":
             stripped_dag.apply_operation_back(op=vertex.op, qargs=vertex.qargs)
     return dag_to_circuit(stripped_dag)
 
 
 def _read_circuit(
     circuit: QuantumCircuit,
-) -> Tuple[int, List[Tuple[int, int]], Dict[str, int], Dict[int, str]]:
+) -> tuple[int, list[tuple[int, int]], dict[str, int], dict[int, str]]:
     """
     Read the input circuit to a graph based representation for the MIP model.
 
     Args:
         - circuit (QuantumCircuit): a stripped circuit to be converted into a
             DAG like representation
     Returns:
@@ -903,19 +913,19 @@
     for qubit in dag.qubits:
         qubit_gate_counter[qubit] = 0
     for vertex in dag.topological_op_nodes():
         if len(vertex.qargs) != 2:
             raise Exception("vertex does not have 2 qargs!")
         arg0, arg1 = vertex.qargs
         vertex_name = "%s[%d]%d %s[%d]%d" % (
-            arg0.register.name,
-            arg0.index,
+            circuit.find_bit(arg0).registers[0][0].name,
+            circuit.find_bit(arg0).index,
             qubit_gate_counter[arg0],
-            arg1.register.name,
-            arg1.index,
+            circuit.find_bit(arg1).registers[0][0].name,
+            circuit.find_bit(arg1).index,
             qubit_gate_counter[arg1],
         )
         qubit_gate_counter[arg0] += 1
         qubit_gate_counter[arg1] += 1
         # print(vertex.op.label,vertex_name,curr_node_id)
         if vertex_name not in node_name_ids and id(vertex) not in vertex_ids:
             node_name_ids[vertex_name] = curr_node_id
```

### Comparing `circuit_knitting_toolbox-0.0.0/circuit_knitting_toolbox/circuit_cutting/wire_cutting/wire_cutting_evaluation.py` & `circuit-knitting-toolbox-0.1.0/circuit_knitting_toolbox/circuit_cutting/wire_cutting/wire_cutting_evaluation.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,65 +6,68 @@
 # obtain a copy of this license in the LICENSE.txt file in the root directory
 # of this source tree or at http://www.apache.org/licenses/LICENSE-2.0.
 # Any modifications or derivative works of this code must retain this
 # copyright notice, and modified files need to carry a notice indicating
 # that they have been altered from the originals.
 
 """Contains functions for executing subcircuits."""
-import itertools, copy
-from typing import Dict, Tuple, Sequence, Optional, List, Any, Union
+
+from __future__ import annotations
+
+import itertools
+import copy
+from typing import Sequence, Any
 from multiprocessing.pool import ThreadPool
 
 import numpy as np
-from nptyping import NDArray
 
 from qiskit import QuantumCircuit
 from qiskit.converters import circuit_to_dag, dag_to_circuit
 from qiskit.circuit.library.standard_gates import HGate, SGate, SdgGate, XGate
-from qiskit.primitives import Sampler as TestSampler
+from qiskit.primitives import BaseSampler, Sampler as TestSampler
 from qiskit_ibm_runtime import QiskitRuntimeService, Sampler, Session, Options
 
 
 def run_subcircuit_instances(
     subcircuits: Sequence[QuantumCircuit],
-    subcircuit_instances: Dict[int, Dict[Tuple[Tuple[str, ...], Tuple[Any, ...]], int]],
-    service: Optional[QiskitRuntimeService] = None,
-    backend_names: Optional[Sequence[str]] = None,
-    options: Optional[Sequence[Options]] = None,
-) -> Dict[int, Dict[int, NDArray]]:
+    subcircuit_instances: dict[int, dict[tuple[tuple[str, ...], tuple[Any, ...]], int]],
+    service: QiskitRuntimeService | None = None,
+    backend_names: Sequence[str] | None = None,
+    options: Sequence[Options] | None = None,
+) -> dict[int, dict[int, np.ndarray]]:
     """
     Execute all provided subcircuits.
 
     Using the backend(s) provided, this executes all the subcircuits to generate the
     resultant probability vectors.
     subcircuit_instance_probs[subcircuit_idx][subcircuit_instance_idx] = measured probability
 
     Args:
         - subcircuits (Sequence[QuantumCircuit]): the list of subcircuits to execute
-        - subcircuit_instances (Dict): dictionary containing information about each of the
+        - subcircuit_instances (dict): dictionary containing information about each of the
             subcircuit instances
-        - service (QiskitRuntimeService): the runtime service
-        - backend_names (Sequence[str]): the backend(s) used to execute the subcircuits
-        - options (Sequence[Options]): options for the runtime execution of subcircuits
+        - service (QiskitRuntimeService | None): the runtime service
+        - backend_names (Sequence[str] | None): the backend(s) used to execute the subcircuits
+        - options (Sequence[Options] | None): options for the runtime execution of subcircuits
 
     Returns:
-        - (Dict): the probability vectors from each of the subcircuit instances
+        - (dict): the probability vectors from each of the subcircuit instances
     """
     if backend_names and options:
         if len(backend_names) != len(options):
             raise AttributeError(
                 f"The list of backend names is length ({len(backend_names)}), but the list of options is length ({len(options)}). It is ambiguous how these options should be applied."
             )
     if service:
         if backend_names:
-            backend_names_repeated: List[Union[str, None]] = [
+            backend_names_repeated: list[str | None] = [
                 backend_names[i % len(backend_names)] for i, _ in enumerate(subcircuits)
             ]
             if options is None:
-                options_repeated: List[Union[Options, None]] = [None] * len(
+                options_repeated: list[Options | None] = [None] * len(
                     backend_names_repeated
                 )
             else:
                 options_repeated = [
                     options[i % len(options)] for i, _ in enumerate(subcircuits)
                 ]
         else:
@@ -73,15 +76,15 @@
                 options_repeated = [options[0]] * len(subcircuits)
             else:
                 options_repeated = [None] * len(subcircuits)
     else:
         backend_names_repeated = [None] * len(subcircuits)
         options_repeated = [None] * len(subcircuits)
 
-    subcircuit_instance_probs: Dict[int, Dict[int, NDArray]] = {}
+    subcircuit_instance_probs: dict[int, dict[int, np.ndarray]] = {}
     with ThreadPool() as pool:
         args = [
             [
                 subcircuit_instances[subcircuit_idx],
                 subcircuit,
                 service,
                 backend_names_repeated[subcircuit_idx],
@@ -93,15 +96,15 @@
 
         for i, partition_batch in enumerate(subcircuit_instance_probs_list):
             subcircuit_instance_probs[i] = partition_batch
 
     return subcircuit_instance_probs
 
 
-def mutate_measurement_basis(meas: Tuple[str, ...]) -> List[Tuple[Any, ...]]:
+def mutate_measurement_basis(meas: tuple[str, ...]) -> list[tuple[Any, ...]]:
     """
     Change of basis for all identity measurements.
 
     For every identity measurement, it is split into an I and Z measurement.
     I and Z measurement basis correspond to the same logical circuit.
 
     Args:
@@ -121,15 +124,15 @@
                 mutated_meas.append(["I", "Z"])
         mutated_meas_out = list(itertools.product(*mutated_meas))
 
         return mutated_meas_out
 
 
 def modify_subcircuit_instance(
-    subcircuit: QuantumCircuit, init: Tuple[str, ...], meas: Tuple[str, ...]
+    subcircuit: QuantumCircuit, init: tuple[str, ...], meas: tuple[str, ...]
 ) -> QuantumCircuit:
     """
     Modify the initialization and measurement bases for a given subcircuit.
 
     Args:
         - subcircuit (QuantumCircuit): the subcircuit to be modified
         - init (tuple): the current initializations
@@ -200,80 +203,97 @@
         else:
             raise Exception("Illegal measurement basis:", x)
     subcircuit_instance_circuit = dag_to_circuit(subcircuit_instance_dag)
 
     return subcircuit_instance_circuit
 
 
-def run_subcircuits(
+def run_subcircuits_using_sampler(
     subcircuits: Sequence[QuantumCircuit],
-    service: Optional[QiskitRuntimeService] = None,
-    backend_name: Optional[str] = None,
-    options: Optional[Options] = None,
-) -> List[NDArray]:
+    sampler: BaseSampler,
+) -> list[np.ndarray]:
     """
     Execute the subcircuit(s).
 
     Args:
         - subcircuit (QuantumCircuit): the subcircuits to be executed
-        - service (QiskitRuntimeService): the runtime service
-        - backend_name (str): the backend used to execute the subcircuits
-        - options (Options): options for the runtime execution of subcircuits
+        - sampler (BaseSampler): the Sampler to use for executions
 
     Returns:
-        - (NDArray): the probability distributions
+        - (np.ndarray): the probability distributions
     """
     for subcircuit in subcircuits:
         if subcircuit.num_clbits == 0:
             subcircuit.measure_all()
 
-    if service is not None:
-        session = Session(service=service, backend=backend_name)
-        sampler = Sampler(session=session, options=options)
-    else:
-        sampler = TestSampler(options=options)
-
     quasi_dists = sampler.run(circuits=subcircuits).result().quasi_dists
 
     all_probabilities_out = []
     for i, qd in enumerate(quasi_dists):
         probabilities = qd.nearest_probability_distribution()
         probabilities_out = np.zeros(2 ** subcircuits[i].num_qubits, dtype=float)
 
         for state in probabilities:
             probabilities_out[state] = probabilities[state]
         all_probabilities_out.append(probabilities_out)
 
     return all_probabilities_out
 
 
-def measure_prob(unmeasured_prob: NDArray, meas: Tuple[Any, ...]) -> NDArray:
+def run_subcircuits(
+    subcircuits: Sequence[QuantumCircuit],
+    service: QiskitRuntimeService | None = None,
+    backend_name: str | None = None,
+    options: Options | None = None,
+) -> list[np.ndarray]:
+    """
+    Execute the subcircuit(s).
+
+    Args:
+        - subcircuit (QuantumCircuit): the subcircuits to be executed
+        - service (QiskitRuntimeService | None): the runtime service
+        - backend_name (str | None): the backend used to execute the subcircuits
+        - options (Options | None): options for the runtime execution of subcircuits
+
+    Returns:
+        - (np.ndarray): the probability distributions
+    """
+    if service is not None:
+        session = Session(service=service, backend=backend_name)
+        sampler = Sampler(session=session, options=options)
+    else:
+        sampler = TestSampler(options=options)
+
+    return run_subcircuits_using_sampler(subcircuits, sampler)
+
+
+def measure_prob(unmeasured_prob: np.ndarray, meas: tuple[Any, ...]) -> np.ndarray:
     """
     Compute the effective probability distribution from the subcircuit distribution.
 
     Args:
         - unmeasured_prob (Sequence[float]): the outputs of the subcircuit execution
         - meas (tuple): the measurement bases
 
     Returns:
-        - (NDArray): the updated measured probability distribution
+        - (np.ndarray): the updated measured probability distribution
     """
     if meas.count("comp") == len(meas):
         return np.array(unmeasured_prob)
     else:
         measured_prob = np.zeros(int(2 ** meas.count("comp")))
         for full_state, p in enumerate(unmeasured_prob):
             sigma, effective_state = measure_state(full_state=full_state, meas=meas)
             # TODO: Add states merging here. Change effective_state to merged_bin
             measured_prob[effective_state] += sigma * p
 
         return measured_prob
 
 
-def measure_state(full_state: int, meas: Tuple[Any, ...]) -> Tuple[int, int]:
+def measure_state(full_state: int, meas: tuple[Any, ...]) -> tuple[int, int]:
     """
     Compute the corresponding effective_state for the given full_state.
 
     Measured in basis `meas`. Returns sigma (int), effective_state (int) where sigma = +-1
 
     Args:
         - full_state (int): the current state (in decimal form)
@@ -293,25 +313,25 @@
             bin_effective_state += meas_bit
     effective_state = int(bin_effective_state, 2) if bin_effective_state != "" else 0
 
     return sigma, effective_state
 
 
 def _run_subcircuit_batch(
-    subcircuit_instance: Dict[Tuple[Tuple[str, ...], Tuple[Any, ...]], int],
+    subcircuit_instance: dict[tuple[tuple[str, ...], tuple[Any, ...]], int],
     subcircuit: QuantumCircuit,
-    service: Optional[QiskitRuntimeService] = None,
-    backend_name: Optional[str] = None,
-    options: Optional[Options] = None,
+    service: QiskitRuntimeService | None = None,
+    backend_name: str | None = None,
+    options: Options | None = None,
 ):
     """
     Execute a circuit using qiskit runtime.
 
     Args:
-        - subcircuit_instances (Dict): dictionary containing information about each of the
+        - subcircuit_instances (dict): dictionary containing information about each of the
             subcircuit instances
         - subcircuit (QuantumCircuit): the subcircuit to execute
         - service (QiskitRuntimeService): the runtime service
         - backend_name (str): the backends used to execute the subcircuit
         - options (Options): options for the runtime execution of subcircuit
 
     Returns:
```

### Comparing `circuit_knitting_toolbox-0.0.0/circuit_knitting_toolbox/circuit_cutting/wire_cutting/wire_cutting_post_processing.py` & `circuit-knitting-toolbox-0.1.0/circuit_knitting_toolbox/circuit_cutting/wire_cutting/wire_cutting_post_processing.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,28 +6,29 @@
 # obtain a copy of this license in the LICENSE.txt file in the root directory
 # of this source tree or at http://www.apache.org/licenses/LICENSE-2.0.
 # Any modifications or derivative works of this code must retain this
 # copyright notice, and modified files need to carry a notice indicating
 # that they have been altered from the originals.
 
 """File containing all cutting post processing functionality."""
+
+from __future__ import annotations
+
 import itertools
 import multiprocessing as mp
-from typing import Dict, Sequence, Union, Tuple, List, Optional, Any
-
+from typing import Sequence, Any
 
 import numpy as np
-from nptyping import NDArray
 from qiskit import QuantumCircuit
 from qiskit.circuit import Qubit
 
 
 def get_cut_qubit_pairs(
-    complete_path_map: Dict[Qubit, Sequence[Dict[str, Union[int, Qubit]]]]
-) -> List[Tuple[Dict[str, Union[int, Any]], Dict[str, Union[int, Any]]]]:
+    complete_path_map: dict[Qubit, Sequence[dict[str, int | Qubit]]]
+) -> list[tuple[dict[str, Any], dict[str, Any]]]:
     """
     Get O-rho cut qubit pairs.
 
     Iterates through the path for each of the qubits and keeps track of the
     each pair of neigbors.
 
     Args:
@@ -67,17 +68,17 @@
         label.append(basis[digit])
         label_idx = label_idx // 4
     return label
 
 
 def attribute_label(
     label: Sequence[str],
-    O_rho_pairs: List[Tuple[Dict[str, Union[int, Any]], Dict[str, Union[int, Any]]]],
+    O_rho_pairs: list[tuple[dict[str, Any], dict[str, Any]]],
     num_subcircuits: int,
-) -> Dict[int, Dict[str, str]]:
+) -> dict[int, dict[str, str]]:
     """
     Get the label attributed to each subcircuit.
 
     subcircuit_label[subcircuit_idx]['init'] = str of init for the cut qubits.
     subcircuit_label[subcircuit_idx]['meas'] = str of meas for the cut qubits.
 
     Args:
@@ -96,26 +97,26 @@
     }
     for c, pair in zip(label, O_rho_pairs):
         if len(pair) != 2:
             raise ValueError(
                 "O_rho_pairs should only contain sequences of length 2: {pair}"
             )
         O_qubit = pair[0]
-        rho_qubit: Dict[str, Union[int, Qubit]] = pair[-1]
+        rho_qubit: dict[str, int | Qubit] = pair[-1]
         subcircuit_label[O_qubit["subcircuit_idx"]]["meas"] += c
         subcircuit_label[rho_qubit["subcircuit_idx"]]["init"] += c
     return subcircuit_label
 
 
 def fill_label(
     subcircuit_idx: int,
     subcircuit: QuantumCircuit,
-    subcircuit_label: Dict[str, str],
-    O_rho_pairs: List[Tuple[Dict[str, Union[int, Any]], Dict[str, Union[int, Any]]]],
-) -> Tuple[List[str], List[str]]:
+    subcircuit_label: dict[str, str],
+    O_rho_pairs: list[tuple[dict[str, Any], dict[str, Any]]],
+) -> tuple[list[str], list[str]]:
     """
     Given a subcircuit, its label and O-rho cut qubit pairs fill the full init, meas strings.
 
     Args:
         - subcircuit_idx (int): the subcircuit index
         - subcircuit (QuantumCircuit): the subcircuit
         - subcircuit_label (dict): the dictionary containing the applied labels for the bases
@@ -129,29 +130,29 @@
     subcircuit_meas_label_counter = 0
     init = ["zero" for q in range(subcircuit.num_qubits)]
     meas = ["comp" for q in range(subcircuit.num_qubits)]
     for pair in O_rho_pairs:
         if len(pair) != 2:
             raise ValueError(f"O_rho_pairs should be length 2: {O_rho_pairs}")
         O_qubit = pair[0]
-        rho_qubit: Dict[str, Union[int, Qubit]] = pair[-1]
+        rho_qubit: dict[str, int | Qubit] = pair[-1]
         if O_qubit["subcircuit_idx"] == subcircuit_idx:
             qubit_idx = subcircuit.qubits.index(O_qubit["subcircuit_qubit"])
             meas[qubit_idx] = subcircuit_label["meas"][subcircuit_meas_label_counter]
             subcircuit_meas_label_counter += 1
         if rho_qubit["subcircuit_idx"] == subcircuit_idx:
             qubit_idx = subcircuit.qubits.index(rho_qubit["subcircuit_qubit"])
             init[qubit_idx] = subcircuit_label["init"][subcircuit_init_label_counter]
             subcircuit_init_label_counter += 1
     return init, meas
 
 
 def get_init_meas(
     init_label: Sequence[str], meas_label: Sequence[str]
-) -> List[Tuple[Tuple[str, ...], Tuple[str, ...]]]:
+) -> list[tuple[tuple[str, ...], tuple[str, ...]]]:
     """
     Generate the initial measurements.
 
     Args:
         - init_label (list): the list of initial bases
         - meas (list): the list of measurement bases
 
@@ -182,15 +183,15 @@
     subcircuit_init_meas = []
     for init in init_combinations:
         for meas in meas_combinations:
             subcircuit_init_meas.append((tuple(init), tuple(meas)))
     return subcircuit_init_meas
 
 
-def convert_to_physical_init(init: List[str]) -> Tuple[int, Tuple[str, ...]]:
+def convert_to_physical_init(init: list[str]) -> tuple[int, tuple[str, ...]]:
     """
     Convert the initial measurements to the physical representations.
 
     Args:
         - init (list): the initial measurements, e.g. ["zero", "2plus"]
 
     Returns:
@@ -220,53 +221,56 @@
         else:
             raise Exception("Illegal initilization symbol :", x)
     return coefficient, tuple(init)
 
 
 def generate_summation_terms(
     subcircuits: Sequence[QuantumCircuit],
-    complete_path_map: Dict[Qubit, Sequence[Dict[str, Union[int, Qubit]]]],
+    complete_path_map: dict[Qubit, Sequence[dict[str, int | Qubit]]],
     num_cuts: int,
-) -> Tuple[
-    List[Dict[int, int]],
-    Dict[int, Dict[Tuple[str, str], Tuple[int, Sequence[Tuple[int, int]]]]],
-    Dict[int, Dict[Tuple[Tuple[str, ...], Tuple[Any, ...]], int]],
+) -> tuple[
+    list[dict[int, int]],
+    dict[int, dict[tuple[str, str], tuple[int, Sequence[tuple[int, int]]]]],
+    dict[int, dict[tuple[tuple[str, ...], tuple[Any, ...]], int]],
 ]:
     """
     Generate all summation terms for the final reconstructions.
 
     Final CutQC reconstruction result = Sum(summation_terms).
 
-    summation_terms (list) : [summation_term_0, summation_term_1, ...] --> 4^#cuts elements.
+    summation_terms (list): [summation_term_0, summation_term_1, ...] --> 4^#cuts elements.
 
-    summation_term[subcircuit_idx] = subcircuit_entry_idx.
-    E.g. summation_term = {0:0,1:13,2:7} = Kron(subcircuit_0_entry_0, subcircuit_1_entry_13, subcircuit_2_entry_7).
+    | summation_term[subcircuit_idx] = subcircuit_entry_idx.
+    | E.g. summation_term = {0:0,1:13,2:7} = Kron(subcircuit_0_entry_0, subcircuit_1_entry_13, subcircuit_2_entry_7).
 
-    subcircuit_entries[subcircuit_idx][init_label,meas_label] = subcircuit_entry_idx, kronecker_term.
-    kronecker_term (list): (coefficient, subcircuit_instance_idx).
-    Add coefficient*subcircuit_instance to subcircuit_entry.
+    | subcircuit_entries[subcircuit_idx][init_label,meas_label] = subcircuit_entry_idx, kronecker_term.
+    | kronecker_term (list): (coefficient, subcircuit_instance_idx).
+    | Add coefficient*subcircuit_instance to subcircuit_entry.
 
     subcircuit_instances[subcircuit_idx][init,meas] = subcircuit_instance_idx.
 
     Args:
         - subcircuits (list): the list of subcircuits
         - complete_path_map (dict): the paths of all the qubits through the circuit DAGs
         - num_cuts (int): the number of cuts
 
     Returns:
+        a tuple
+        containing:
+
         - (dict): dictionary containing information on the summation terms
         - (dict): dictionary containing the subcircuits entry information
         - (dict): dictionary containing subcircuit instances
     """
     summation_terms = []
-    subcircuit_entries: Dict[
-        int, Dict[Tuple[str, str], Tuple[int, Sequence[Tuple[int, int]]]]
+    subcircuit_entries: dict[
+        int, dict[tuple[str, str], tuple[int, Sequence[tuple[int, int]]]]
     ] = {subcircuit_idx: {} for subcircuit_idx in range(len(subcircuits))}
-    subcircuit_instances: Dict[
-        int, Dict[Tuple[Tuple[str, ...], Tuple[Any, ...]], int]
+    subcircuit_instances: dict[
+        int, dict[tuple[tuple[str, ...], tuple[Any, ...]], int]
     ] = {subcircuit_idx: {} for subcircuit_idx in range(len(subcircuits))}
     O_rho_pairs = get_cut_qubit_pairs(complete_path_map=complete_path_map)
     for summation_term_idx in range(4**num_cuts):
         label = get_label(label_idx=summation_term_idx, num_cuts=num_cuts)
         # print('%d/%d summation term:'%(summation_term_idx+1,4**num_cuts),label)
         summation_term = {}
         subcircuit_labels = attribute_label(
@@ -301,16 +305,16 @@
                 )
                 kronecker_term = []
                 for init_meas in subcircuit_init_meas:
                     if len(init_meas) != 2:
                         raise ValueError(
                             f"init_meas variable should be a length-2 tuple: {init_meas}"
                         )
-                    init: Tuple[str, ...] = init_meas[0]
-                    meas: Tuple[str, ...] = init_meas[-1]
+                    init: tuple[str, ...] = init_meas[0]
+                    meas: tuple[str, ...] = init_meas[-1]
                     coefficient, init = convert_to_physical_init(
                         init=list(init_meas[0])
                     )
                     if (init, meas) in subcircuit_instances[subcircuit_idx]:
                         subcircuit_instance_idx = subcircuit_instances[subcircuit_idx][
                             (init, meas)
                         ]
@@ -332,32 +336,32 @@
         summation_terms.append(summation_term)
         # print('summation_term =',summation_term,'\n')
     return summation_terms, subcircuit_entries, subcircuit_instances
 
 
 def naive_compute(
     subcircuit_order: Sequence[int],
-    summation_terms: Sequence[Dict[int, int]],
-    subcircuit_entry_probs: Dict[int, Dict[int, NDArray]],
-) -> Tuple[Optional[NDArray], Dict[str, int]]:
+    summation_terms: Sequence[dict[int, int]],
+    subcircuit_entry_probs: dict[int, dict[int, np.ndarray]],
+) -> tuple[np.ndarray | None, dict[str, int]]:
     """
     Reconstruct the full probability distribution from the subcircuits.
 
     This function is called within the build function, meant to be used
     in a multipooling manner.
 
     Args:
         - subcircuit_order (list): the order of the subcircuit inputs
         - summation_terms (list): the summation terms, as generated
             from generate_summation_terms
         - subcircuit_entry_probs (dict): the input probabilities from each of
             the subcircuit executions
 
     Returns:
-        - (NDArray): the reconstructed probability distribution
+        - (np.ndarray): the reconstructed probability distribution
         - (dict): the approximate computational overhead of the function
     """
     reconstructed_prob = None
     overhead = {"additions": 0, "multiplications": 0}
     for summation_term in summation_terms:
         summation_term_prob = None
         for subcircuit_idx in subcircuit_order:
@@ -377,33 +381,36 @@
         else:
             reconstructed_prob += summation_term_prob
             overhead["additions"] += len(reconstructed_prob)
     return reconstructed_prob, overhead
 
 
 def build(
-    summation_terms: Sequence[Dict[int, int]],
-    subcircuit_entry_probs: Dict[int, Dict[int, NDArray]],
+    summation_terms: Sequence[dict[int, int]],
+    subcircuit_entry_probs: dict[int, dict[int, np.ndarray]],
     num_cuts: int,
     num_threads: int,
-) -> Tuple[NDArray, List[int], Dict[str, int]]:
+) -> tuple[np.ndarray, list[int], dict[str, int]]:
     """
     Reconstruct the full probability distribution from the subcircuits.
 
     Args:
         - summation_terms (list): the summation terms used to generate the full
             vector, as generated in generate_summation_terms
         - subcircuit_entry_probs (dict): the probabilities vectors from the
             subcircuit executions
         - num_cuts (int): the number of cuts
         - num_threads (int): the number of threads to use for multithreading
 
     Returns:
-        - (NDArray): the reconstructed probability distribution of the full
-            circuit
+        a tuple
+        containing:
+
+        - (np.ndarray): the reconstructed probability distribution of the full
+          circuit
         - (list): the ordering of the distribution
         - (dict): the computational post-processing overhead
     """
     smart_order = sorted(
         list(subcircuit_entry_probs.keys()),
         key=lambda subcircuit_idx: len(subcircuit_entry_probs[subcircuit_idx][0]),
     )
@@ -434,16 +441,16 @@
     if reconstructed_prob is None:
         raise ValueError("Something went wrong during the build.")
 
     return reconstructed_prob, smart_order, overhead
 
 
 def _find_process_jobs(
-    jobs: Sequence[Dict[int, int]], rank: int, num_workers: int
-) -> Sequence[Dict[int, int]]:
+    jobs: Sequence[dict[int, int]], rank: int, num_workers: int
+) -> Sequence[dict[int, int]]:
     """
     Split up the total jobs into subjobs to be multithreaded.
 
     Args:
         - jobs (list): all summation terms to be used
         - rank (int): the input thread
         - num_workers (int): 5 * the number of threads
```

### Comparing `circuit_knitting_toolbox-0.0.0/circuit_knitting_toolbox/circuit_cutting/wire_cutting/wire_cutting_verification.py` & `circuit-knitting-toolbox-0.1.0/circuit_knitting_toolbox/circuit_cutting/wire_cutting/wire_cutting_verification.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,19 +7,21 @@
 # of this source tree or at http://www.apache.org/licenses/LICENSE-2.0.
 # Any modifications or derivative works of this code must retain this
 # copyright notice, and modified files need to carry a notice indicating
 # that they have been altered from the originals.
 
 """File that contains the function to verify the results of the cut circuits."""
 
-import psutil, copy
-from typing import Tuple, Sequence, Dict, Union, List
+from __future__ import annotations
+
+import copy
+import psutil
+from typing import Sequence
 
 import numpy as np
-from nptyping import NDArray
 from qiskit import QuantumCircuit
 from qiskit.circuit import Qubit
 from qiskit.quantum_info import Statevector
 from qiskit_aer import Aer
 
 from circuit_knitting_toolbox.utils.conversion import quasi_to_real
 from circuit_knitting_toolbox.utils.metrics import (
@@ -29,32 +31,35 @@
     cross_entropy,
     HOP,
 )
 
 
 def verify(
     full_circuit: QuantumCircuit,
-    reconstructed_output: NDArray,
-) -> Tuple[Dict[str, Dict[str, float]], Sequence[float]]:
+    reconstructed_output: np.ndarray,
+) -> tuple[dict[str, dict[str, float]], Sequence[float]]:
     """
     Compare the reconstructed probabilities to the ground truth.
 
     Executes the original circuit, then measures the distributional differences between this exact
     result (ground truth) and the reconstructed result from the subcircuits.
     Provides a variety of metrics to evaluate the differences in the distributions.
 
     Args:
         - full_circuit (QuantumCircuit): the original quantum circuit that was cut
-        - reconstructed_output (NDArray): the reconstructed probability distribution from the
+        - reconstructed_output (np.ndarray): the reconstructed probability distribution from the
             execution of the subcircuits
 
     Returns:
-        - (dict): a dictionary containing a variety of distributional difference metrics for the
-            ground truth and reconstructed distributions
-        - (Sequence[float]): the true probability distribution of the full circuit
+        a tuple
+        containing:
+
+        - a dictionary containing a variety of distributional difference
+          metrics for the ground truth and reconstructed distributions; and,
+        - the true probability distribution of the full circuit
     """
     ground_truth = _evaluate_circuit(circuit=full_circuit)
     metrics = {}
     for quasi_conversion_mode in ["nearest", "naive"]:
         real_probability = quasi_to_real(
             quasiprobability=reconstructed_output, mode=quasi_conversion_mode
         )
@@ -73,34 +78,34 @@
         }
     return metrics, ground_truth
 
 
 def generate_reconstructed_output(
     full_circuit: QuantumCircuit,
     subcircuits: Sequence[QuantumCircuit],
-    unordered: NDArray,
+    unordered: np.ndarray,
     smart_order: Sequence[int],
-    complete_path_map: Dict[Qubit, Sequence[Dict[str, Union[int, Qubit]]]],
-) -> NDArray:
+    complete_path_map: dict[Qubit, Sequence[dict[str, int | Qubit]]],
+) -> np.ndarray:
     """
     Reorder the probability distribution.
 
     Args:
         - full_circuit (QuantumCircuit): the original uncut circuit
         - subcircuits (list): the cut subcircuits
-        - unordered (NDArray): the unordered results of the subcircuits
+        - unordered (np.ndarray): the unordered results of the subcircuits
         - smart_order (list): the correct ordering of the subcircuits
         - complete_path_map (dict): the path map of the cuts, as defined from the
             cutting function
 
     Returns:
-        - (NDArray): the reordered and reconstructed probability distribution over the
+        - (np.ndarray): the reordered and reconstructed probability distribution over the
             full circuit
     """
-    subcircuit_out_qubits: Dict[int, List[Qubit]] = {
+    subcircuit_out_qubits: dict[int, list[Qubit]] = {
         subcircuit_idx: [] for subcircuit_idx in smart_order
     }
     for input_qubit in complete_path_map:
         path = complete_path_map[input_qubit]
         output_qubit = path[-1]
         subcircuit_out_qubits[output_qubit["subcircuit_idx"]].append(
             (output_qubit["subcircuit_qubit"], full_circuit.qubits.index(input_qubit))
@@ -112,15 +117,15 @@
             key=lambda x: subcircuits[subcircuit_idx].qubits.index(x[0]),
             reverse=True,
         )
         subcircuit_out_qubits[subcircuit_idx] = [
             x[1] for x in subcircuit_out_qubits[subcircuit_idx]
         ]
 
-    unordered_qubit: List[int] = []
+    unordered_qubit: list[int] = []
     for subcircuit_idx in smart_order:
         unordered_qubit += subcircuit_out_qubits[subcircuit_idx]
 
     reconstructed_output = np.zeros(len(unordered))
 
     for unordered_state, unordered_p in enumerate(unordered):
         bin_unordered_state = bin(unordered_state)[2:].zfill(full_circuit.num_qubits)
```

### Comparing `circuit_knitting_toolbox-0.0.0/circuit_knitting_toolbox/entanglement_forging/__init__.py` & `circuit-knitting-toolbox-0.1.0/circuit_knitting_toolbox/entanglement_forging/__init__.py`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.0.0/circuit_knitting_toolbox/entanglement_forging/cholesky_decomposition.py` & `circuit-knitting-toolbox-0.1.0/circuit_knitting_toolbox/entanglement_forging/cholesky_decomposition.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,172 +7,127 @@
 # of this source tree or at http://www.apache.org/licenses/LICENSE-2.0.
 # Any modifications or derivative works of this code must retain this
 # copyright notice, and modified files need to carry a notice indicating
 # that they have been altered from the originals.
 
 """File containing the EntanglementForgingGroundStateSolver class and associated functions."""
 
+from __future__ import annotations
+
 import copy
-from typing import Dict, Iterable, List, Optional, Sequence, Tuple
+from typing import Sequence
 
 import numpy as np
-from nptyping import Float, Int, NDArray, Shape
 from qiskit.opflow import ListOp, PauliSumOp
 from qiskit.quantum_info import Pauli
-from qiskit_nature.converters.second_quantization import QubitConverter
-from qiskit_nature.drivers.second_quantization import ElectronicStructureDriver
-from qiskit_nature.mappers.second_quantization import JordanWignerMapper
-from qiskit_nature.problems.second_quantization import ElectronicStructureProblem
-from qiskit_nature.properties.second_quantization.electronic.bases import (
-    ElectronicBasis,
+from qiskit_nature.second_q.problems import ElectronicStructureProblem
+from qiskit_nature.second_q.mappers import QubitConverter, JordanWignerMapper
+from qiskit_nature.second_q.operators import (
+    FermionicOp,
+    PolynomialTensor,
 )
-from qiskit_nature.properties.second_quantization.electronic.integrals import (
-    IntegralProperty,
-    OneBodyElectronicIntegrals,
-    TwoBodyElectronicIntegrals,
+from qiskit_nature.second_q.operators.tensor_ordering import (
+    to_chemist_ordering,
+    to_physicist_ordering,
 )
 
 from .entanglement_forging_ansatz import EntanglementForgingAnsatz
 from .entanglement_forging_operator import EntanglementForgingOperator
-from .entanglement_forging_ansatz import EntanglementForgingAnsatz
-
-
-SingleBodyIntegrals = NDArray[Shape["N, N"], Float]
-Matrix = NDArray[Shape["N, N"], Float]
-TwoBodyIntegrals = NDArray[Shape["N, N, N, N"], Float]
 
 
 def get_cholesky_op(
-    l_op: NDArray, g: int, converter: QubitConverter, opname: str
+    l_op: np.ndarray, g: int, converter: QubitConverter, opname: str
 ) -> PauliSumOp:
     """
     Convert a two-body term into a cholesky operator.
 
     Args:
         - l_op: Two body integrals
         - g: integral index
         - converter: Qubit converter to be used
         - opname: Prefix for output cholesky operator name
 
     Returns:
         - cholesky_operator: The converted operator
     """
-    # This will suppress a warning about an upcoming change in Qiskit Nature
-    from qiskit_nature.settings import settings
-
-    settings.dict_aux_operators = True
-
-    cholesky_int = OneBodyElectronicIntegrals(
-        basis=ElectronicBasis.SO, matrices=l_op[:, :, g]
-    )
-    cholesky_property = IntegralProperty("cholesky_op", [cholesky_int])
-    if isinstance(cholesky_property.second_q_ops(), dict):
-        cholesky_op = converter.convert(cholesky_property.second_q_ops()["cholesky_op"])
-    else:
-        cholesky_op = converter.convert(cholesky_property.second_q_ops()[0])
+    pt = PolynomialTensor({"+-": l_op[:, :, g]})
+    fer_op = FermionicOp.from_polynomial_tensor(pt)
+    cholesky_op = converter.convert(fer_op)
     cholesky_op._name = opname + "_chol" + str(g)
+
     return cholesky_op
 
 
 def cholesky_decomposition(
     problem: ElectronicStructureProblem,
-    orbitals_to_reduce: Optional[Sequence[int]] = None,
-) -> Tuple[ListOp, float]:
+    mo_coeff: np.ndarray | None = None,
+    orbitals_to_reduce: Sequence[int] | None = None,
+) -> tuple[ListOp, float]:
     """
     Construct the decomposed Hamiltonian from an input ``ElectronicStructureProblem``.
 
     Args:
         - problem (ElectronicStructureProblem): An ``ElectronicStructureProblem`` from which the decomposed Hamiltonian will be
             calculated.
-        - orbitals_to_reduce (Optional[Sequence[int]]): A list of orbital indices to remove from the problem before decomposition.
+        - mo_coeff (np.ndarray | None): The coefficients for mapping to the MO basis. If ``None``, the input integrals will be
+            assumed to be in the MO basis.
+        - orbitals_to_reduce (Sequence[int] | None): A list of orbital indices to remove from the problem before decomposition.
 
     Returns:
         - Tuple containing
             - cholesky_operator (ListOp): A list of operators representing the decomposed Hamiltonian.
               shape: [single-body hamiltonian, cholesky_0, ..., cholesky_N]
             - freeze_shift (float): An energy shift resulting from the decomposition. This shift should be re-applied after
               calculating properties of the decomposed operator (i.e. ground state energy).
-    """
-    # Store the ElectronicStructureProblem
-    problem.second_q_ops()
 
-    if problem.grouped_property_transformed is None:
-        raise AttributeError(
-            "There was a problem retrieving the grouped properties from the ElectronicStructureProblem."
-        )
-    if problem.driver is None:
-        raise AttributeError("The ElectronicStructureProblem has no driver.")
-
-    if not isinstance(problem.driver, ElectronicStructureDriver):
-        raise AttributeError(
-            "The ElectronicStructureProblem's driver should be an instance of ElectronicStructureDriver."
-        )
-
-    electronic_basis_transform = problem.grouped_property_transformed.get_property(
-        "ElectronicBasisTransform"
-    )
-    if electronic_basis_transform is None:
-        raise AttributeError(
-            "There was a problem retrieving the ElectronicBasisTransform property from the ElectronicStructureProblem."
-        )
-
-    electronic_energy = problem.grouped_property_transformed.get_property(
-        "ElectronicEnergy"
-    )
-    if electronic_energy is None:
-        raise AttributeError(
-            "There was a problem retrieving the ElectronicEnergy property from the ElectronicStructureProblem."
-        )
-
-    particle_number = problem.grouped_property_transformed.get_property(
-        "ParticleNumber"
+    Raises:
+        - ValueError:
+            The input ElectronicStructureProblem contains no particle number information.
+    """
+    hcore = np.array(problem.hamiltonian.electronic_integrals.one_body.alpha["+-"])
+    eri = to_chemist_ordering(
+        problem.hamiltonian.electronic_integrals.two_body.alpha["++--"]
     )
-    if particle_number is None:
-        raise AttributeError(
-            "There was a problem retrieving the ParticleNumber property from the ElectronicStructureProblem."
+    num_alpha = problem.num_alpha
+    if num_alpha is None:
+        raise ValueError(
+            "The input ElectronicStructureProblem contains no particle number information."
         )
 
-    # Get data for generating the cholesky decomposition
-    mo_coeff: Matrix = electronic_basis_transform.coeff_alpha
-    hcore: SingleBodyIntegrals = electronic_energy.get_electronic_integral(
-        ElectronicBasis.AO, 1
-    )._matrices[0]
-    eri: TwoBodyIntegrals = electronic_energy.get_electronic_integral(
-        ElectronicBasis.AO, 2
-    )._matrices[0]
-    num_alpha = particle_number.num_alpha
+    # If no mo coeffs are passed, we assume the integrals are with respect to MO basis
+    if mo_coeff is None:
+        mo_coeff = np.eye(eri.shape[0], eri.shape[0])
 
     # Store the reduced orbitals as virtual and occupied lists
     if orbitals_to_reduce is None:
         orbitals_to_reduce = []
-    orbitals_to_reduce_dict: Dict[
-        str, NDArray[Shape["*"], Int]
-    ] = _get_orbitals_to_reduce(orbitals_to_reduce, num_alpha)
+    orbitals_to_reduce_dict: dict[str, np.ndarray] = _get_orbitals_to_reduce(
+        orbitals_to_reduce, num_alpha
+    )
 
     # Hold fields used to calculate the final energy shift
     # Freeze shift will be calculated during decomposition
-    freeze_shift = 0.0
-    nuclear_repulsion_energy = electronic_energy.nuclear_repulsion_energy
+    nuclear_repulsion_energy = problem.nuclear_repulsion_energy
+    if nuclear_repulsion_energy is None:
+        nuclear_repulsion_energy = 0.0
 
     h_1_op, h_chol_ops, freeze_shift, _, _ = _get_fermionic_ops_with_cholesky(
         mo_coeff,
         hcore,
         eri,
         opname="H",
         halve_transformed_h2=True,
         occupied_orbitals_to_reduce=orbitals_to_reduce_dict["occupied"],
         virtual_orbitals_to_reduce=orbitals_to_reduce_dict["virtual"],
     )
 
     op_list = [h_1_op] + h_chol_ops
     operator = ListOp(op_list)
 
-    energy_shift = freeze_shift + nuclear_repulsion_energy
-
-    return operator, energy_shift
+    return operator, nuclear_repulsion_energy + freeze_shift
 
 
 def convert_cholesky_operator(
     operator: ListOp,
     ansatz: EntanglementForgingAnsatz,
 ) -> EntanglementForgingOperator:
     """
@@ -279,66 +234,66 @@
         w_ab=w_ab,
     )
 
     return forged_operator
 
 
 def _get_fermionic_ops_with_cholesky(
-    mo_coeff: Matrix,
-    h1: SingleBodyIntegrals,
-    h2: TwoBodyIntegrals,
+    mo_coeff: np.ndarray,
+    h1: np.ndarray,
+    h2: np.ndarray,
     opname: str,
     halve_transformed_h2: bool = False,
-    occupied_orbitals_to_reduce: Optional[NDArray[Shape["*"], Int]] = None,
-    virtual_orbitals_to_reduce: Optional[NDArray[Shape["*"], Int]] = None,
+    occupied_orbitals_to_reduce: np.ndarray | None = None,
+    virtual_orbitals_to_reduce: np.ndarray | None = None,
     epsilon_cholesky: float = 1e-10,
-) -> Tuple[PauliSumOp, List[PauliSumOp], float, SingleBodyIntegrals, TwoBodyIntegrals,]:
+) -> tuple[PauliSumOp, list[PauliSumOp], float, np.ndarray, np.ndarray,]:
     r"""
     Decompose the Hamiltonian operators into a form appropriate for entanglement forging.
 
     Args:
-        - mo_coeff (NDArray[Shape["N, N"], Float]): 2D array representing coefficients for converting from AO to MO basis.
-        - h1 (NDArray[Shape["N, N"], Float]): 2D array representing operator
+        - mo_coeff (np.ndarray): 2D array representing coefficients for converting from AO to MO basis.
+        - h1 (np.ndarray): 2D array representing operator
             coefficients of one-body integrals in the AO basis.
-        - h2 (NDArray[Shape["N, N, N, N"], Float]): 4D array representing operator coefficients
+        - h2 (np.ndarray): 4D array representing operator coefficients
             of two-body integrals in the AO basis.
-        - halve_transformed_h2 (Optional[bool]): Should be set to True for Hamiltonian
+        - halve_transformed_h2 (bool | None): Should be set to True for Hamiltonian
             operator to agree with Qiskit conventions.
-        - occupied_orbitals_to_reduce (Optional[NDArray[Shape["*"], Int]]): Optional; A list of occupied orbitals that will be removed.
-        - virtual_orbitals_to_reduce (Optional[NDArray[Shape["*"], Int]]):Optional; A list of virtual orbitals that will be removed.
-        - epsilon_cholesky (Optional[float]): The threshold for the decomposition (typically a number close to 0).
+        - occupied_orbitals_to_reduce (np.ndarray | None): A list of occupied orbitals that will be removed.
+        - virtual_orbitals_to_reduce (np.ndarray | None): A list of virtual orbitals that will be removed.
+        - epsilon_cholesky (float | None): The threshold for the decomposition (typically a number close to 0).
 
     Returns:
         - qubit_op (PauliSumOp): H_1 in the Cholesky decomposition.
-        - cholesky_ops (List[PauliSumOp]): L_\\gamma in the Cholesky decomposition
+        - cholesky_ops (list[PauliSumOp]): L_\\gamma in the Cholesky decomposition
         - freeze_shift (float): Energy shift due to freezing.
-        - h1 (NDArray[Shape["N, N"], Float]): 2D array representing operator coefficients of one-body
+        - h1 (np.ndarray): 2D array representing operator coefficients of one-body
             integrals in the MO basis.
-        - h2 (NDArray[Shape["N, N, N, N"], Float]): 4D array representing operator coefficients of
+        - h2 (np.ndarray): 4D array representing operator coefficients of
             two-body integrals in the MO basis.
     """
     if virtual_orbitals_to_reduce is None:
         virtual_orbitals_to_reduce = np.array([])
     if occupied_orbitals_to_reduce is None:
         occupied_orbitals_to_reduce = np.array([])
 
     coeff_mo = copy.copy(mo_coeff)
 
     h1 = np.einsum("pi,pr->ir", coeff_mo, h1)
     h1 = np.einsum("rj,ir->ij", coeff_mo, h1)  # h_{pq} in MO basis
 
     # Do the cholesky decomposition
     if h2 is not None:
-        num_gammas, l_op = _get_modified_cholesky(h2, epsilon_cholesky)
+        _, l_op = _get_modified_cholesky(h2, epsilon_cholesky)
 
         # Obtain L_{pr,g} in the MO basis
         l_op = np.einsum("prg,pi,rj->ijg", l_op, coeff_mo, coeff_mo)
     else:
         size = len(h1)
-        num_gammas, l_op = 0, np.zeros(shape=(size, size, 0))
+        l_op = np.zeros(shape=(size, size, 0))
 
     if len(occupied_orbitals_to_reduce) > 0:
         orbitals_not_to_reduce_array = np.array(
             sorted(set(range(len(h1))) - set(occupied_orbitals_to_reduce))
         )
 
         h1_frozenpart = h1[
@@ -384,38 +339,30 @@
     else:
         pass
 
     h2 = np.einsum("prg,qsg->prqs", l_op, l_op)
 
     if halve_transformed_h2:
         h2 /= 2  # type: ignore
-    h1_int = OneBodyElectronicIntegrals(basis=ElectronicBasis.SO, matrices=h1)
-    h2_int = TwoBodyElectronicIntegrals(basis=ElectronicBasis.SO, matrices=h2)
-    int_property = IntegralProperty("fer_op", [h1_int, h2_int])
-
-    if isinstance(int_property.second_q_ops(), dict):
-        fer_op = int_property.second_q_ops()["fer_op"]
-    else:
-        fer_op = int_property.second_q_ops()[0]
 
     converter = QubitConverter(JordanWignerMapper())
+    pt = PolynomialTensor({"+-": h1, "++--": to_physicist_ordering(h2)})
+    fer_op = FermionicOp.from_polynomial_tensor(pt)
     qubit_op = converter.convert(fer_op)
 
     qubit_op._name = opname + "_onebodyop"
 
     cholesky_ops = [
         get_cholesky_op(l_op, g, converter, opname) for g in range(l_op.shape[2])
     ]
 
     return qubit_op, cholesky_ops, freeze_shift, h1, h2
 
 
-def _get_modified_cholesky(
-    two_body_overlap_integrals: NDArray[Shape["*, *, *"], Float], eps: float
-):
+def _get_modified_cholesky(two_body_overlap_integrals: np.ndarray, eps: float):
     """Perform modified Cholesky decomposition on the two-body integrals given an epsilon value."""
     n_basis_states = two_body_overlap_integrals.shape[0]  # number of basis states
     # Max (chmax) and current (n_gammas) number of Cholesky vectors
     ch_max, n_gammas = 10 * n_basis_states, 0
 
     w_op = two_body_overlap_integrals.reshape(n_basis_states**2, n_basis_states**2)
     l_op = np.zeros((n_basis_states**2, ch_max))
@@ -435,17 +382,17 @@
 
     l_op = l_op[:, :n_gammas].reshape((n_basis_states, n_basis_states, n_gammas))
 
     return n_gammas, l_op
 
 
 def _get_orbitals_to_reduce(
-    orbitals_to_reduce: Iterable[int],
+    orbitals_to_reduce: Sequence[int],
     num_alpha: int,
-) -> Dict[str, NDArray[Shape["*"], Int]]:
+) -> dict[str, np.ndarray]:
     orb_to_reduce_dict = {
         "occupied": np.asarray(orbitals_to_reduce),
         "virtual": np.asarray(orbitals_to_reduce),
         "all": np.asarray(orbitals_to_reduce),
     }
 
     # Populate the occupied list within the dict
```

### Comparing `circuit_knitting_toolbox-0.0.0/circuit_knitting_toolbox/entanglement_forging/entanglement_forging_ansatz.py` & `circuit-knitting-toolbox-0.1.0/circuit_knitting_toolbox/entanglement_forging/entanglement_forging_ansatz.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,22 +7,19 @@
 # of this source tree or at http://www.apache.org/licenses/LICENSE-2.0.
 # Any modifications or derivative works of this code must retain this
 # copyright notice, and modified files need to carry a notice indicating
 # that they have been altered from the originals.
 
 """File containing the entanglement forging ansatz class."""
 
-from typing import List, Tuple, Optional
+from __future__ import annotations
 
 from qiskit import QuantumCircuit
 
 
-Bitstring = Tuple[int]
-
-
 class EntanglementForgingAnsatz:
     """Class to hold features of the ansatz for Entanglement Forging.
 
     Entanglement Forging is based on a Schmidt decomposition of a 2N-qubit
     wavefunction into two N-qubit subsystems. These subsystems are described by a
     unitary operator U acting on a set of computational basis states. The unitary
     can be represented by a parametrized quantum circuit whose parameters are
@@ -34,44 +31,44 @@
     should be of length N. This class functions as a container for information about
     the circuit and bitstrings, and is required for the EntanglementForgingGroundStateSolver.
 
     Attributes:
         - circuit_u (QuantumCircuit): the parameterized circuit that is optimized to
             find the minimum energy of the original problem. It represents the
             unitary U for both N-qubit subsystems in the Schmidt decomposition.
-        - bitstrings_u (List[Tuple[Int]]): the input bitstrings for each N-qubit
+        - bitstrings_u (list[tuple[Int]]): the input bitstrings for each N-qubit
             subsystem. The bitstrings represent the computational basis states
             contributing to the Schmidt decomposition. List must contain less than
             or equal to 2^N elements and each bitstring must have length N. These
             bitstrings are used for each subsystem unless bitstrings_v is provided.
-        - bitstrings_v (List[Tuple[Int]], optional): specifies the bitstrings to be
+        - bitstrings_v (list[tuple[Int]], optional): specifies the bitstrings to be
             used for the second subsystem in the Schmidt decomposition. Must be the
             same shape as bitstrings_u. If not provided, then bitstrings_u is used
             for both subsystems.
     """
 
     def __init__(
         self,
         circuit_u: QuantumCircuit,
-        bitstrings_u: List[Bitstring],
-        bitstrings_v: Optional[List[Bitstring]] = None,
+        bitstrings_u: list[tuple[int, ...]],
+        bitstrings_v: list[tuple[int, ...]] | None = None,
     ):
         """
         Assign the necessary member variables and check for shaping errors.
 
         Args:
             - circuit_u (QuantumCircuit): the parameterized circuit that is optimized to
                 find the minimum energy of the original problem. It represents the
                 unitary U for both N-qubit subsystems in the Schmidt decomposition.
-            - bitstrings_u (List[Tuple[Int]]): the input bitstrings for each N-qubit
+            - bitstrings_u (list[tuple[Int]]): the input bitstrings for each N-qubit
                 subsystem. The bitstrings represent the computational basis states
                 contributing to the Schmidt decomposition. List must contain less than
                 or equal to 2^N elements and each bitstring must have length N. These
                 bitstrings are used for each subsystem unless bitstrings_v is provided.
-            - bitstrings_v (List[Tuple[Int]], optional): specifies the bitstrings to be
+            - bitstrings_v (list[tuple[Int]], optional): specifies the bitstrings to be
                 used for the second subsystem in the Schmidt decomposition. Must be the
                 same shape as bitstrings_u. If not provided, then bitstrings_u is used
                 for both subsystems.
 
         Returns:
             - None
 
@@ -93,44 +90,44 @@
 
             if len(bitstrings_u) != len(bitstrings_v):
                 raise ValueError(
                     "There must be the same number of V bitstrings as U bitstrings."
                 )
 
         self._circuit_u: QuantumCircuit = circuit_u
-        self._bitstrings_u: List[Bitstring] = bitstrings_u
-        self._bitstrings_v: List[Bitstring] = bitstrings_v or bitstrings_u
+        self._bitstrings_u: list[tuple[int, ...]] = bitstrings_u
+        self._bitstrings_v: list[tuple[int, ...]] = bitstrings_v or bitstrings_u
 
     @property
     def circuit_u(self) -> QuantumCircuit:
         """
         Property function for the circuit.
 
         Returns:
             - (QuantumCircuit): the _circuit_u member variable
         """
         return self._circuit_u
 
     @property
-    def bitstrings_u(self) -> List[Bitstring]:
+    def bitstrings_u(self) -> list[tuple[int, ...]]:
         """
         Property function for the first bitstrings.
 
         Returns:
-            - (List[Bitstring]): the _bitstrings_u member variable
+            - (list[tuple[int, ...]]): the _bitstrings_u member variable
         """
         return self._bitstrings_u
 
     @property
-    def bitstrings_v(self) -> List[Bitstring]:
+    def bitstrings_v(self) -> list[tuple[int, ...]]:
         """
         Property function for the second bitstrings.
 
         Returns:
-            - (List[Bitstring]): the _bitstrings_v member variable
+            - (list[tuple[int, ...]]): the _bitstrings_v member variable
         """
         return self._bitstrings_v
 
     @property
     def bitstrings_are_symmetric(self) -> bool:
         """
         Property function for the symmetry of bitstrings.
```

### Comparing `circuit_knitting_toolbox-0.0.0/circuit_knitting_toolbox/entanglement_forging/entanglement_forging_ground_state_solver.py` & `circuit-knitting-toolbox-0.1.0/circuit_knitting_toolbox/entanglement_forging/entanglement_forging_ground_state_solver.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,83 +7,69 @@
 # of this source tree or at http://www.apache.org/licenses/LICENSE-2.0.
 # Any modifications or derivative works of this code must retain this
 # copyright notice, and modified files need to carry a notice indicating
 # that they have been altered from the originals.
 
 """File containing the entanglement forging ground state solver class and associated support methods."""
 
+from __future__ import annotations
+
 from dataclasses import dataclass, field
 from time import time
 from typing import (
     Callable,
-    Dict,
     Iterable,
-    List,
-    Optional,
     Sequence,
-    TypeVar,
     Union,
-    Tuple,
 )
 
 import scipy
 import numpy as np
-from nptyping import NDArray
 
-from qiskit import QuantumCircuit
-from qiskit.circuit import Instruction
+from qiskit.algorithms.minimum_eigensolvers import MinimumEigensolverResult
 from qiskit.algorithms.optimizers import SPSA, Optimizer, OptimizerResult
-from qiskit.opflow import PauliSumOp, OperatorBase
-from qiskit.quantum_info import Statevector
-from qiskit.result import Result
-from qiskit_nature import ListOrDictType
-from qiskit_nature.algorithms import GroundStateSolver
-from qiskit_nature.operators.second_quantization import SecondQuantizedOp
-from qiskit_nature.problems.second_quantization import (
-    BaseProblem,
+from qiskit.opflow import ListOp
+from qiskit_nature.second_q.problems import (
     ElectronicStructureProblem,
+    EigenstateResult,
+    ElectronicBasis,
 )
-from qiskit_nature.results import EigenstateResult
 from qiskit_ibm_runtime import QiskitRuntimeService, Options
 
 from .entanglement_forging_ansatz import EntanglementForgingAnsatz
 from .entanglement_forging_knitter import EntanglementForgingKnitter
 from .entanglement_forging_operator import EntanglementForgingOperator
 from .cholesky_decomposition import cholesky_decomposition, convert_cholesky_operator
-from .entanglement_forging_ansatz import EntanglementForgingAnsatz
 
-RESULT = Union[scipy.optimize.OptimizeResult, OptimizerResult]
-OBJECTIVE = Callable[[NDArray], float]
+
+OBJECTIVE = Callable[[np.ndarray], float]
 MINIMIZER = Callable[
     [
         OBJECTIVE,  # the objective function to minimize
-        NDArray,  # the initial point for the optimization
+        np.ndarray,  # the initial point for the optimization
     ],
-    RESULT,  # a result object (either SciPy's or Qiskit's)
+    Union[scipy.optimize.OptimizeResult, OptimizerResult],
 ]
-_T = TypeVar("_T")  # Pylint does not allow single character class names.
-
-ListOrDict = Union[List[Optional[_T]], Dict[str, _T]]
 
 
 @dataclass
 class EntanglementForgingEvaluation:
     """Entanglement Forging Evaluation."""
 
     parameters: Sequence[float]
     eigenvalue: float
-    eigenstate: NDArray
+    eigenstate: np.ndarray
 
 
 @dataclass
 class EntanglementForgingHistory:
     """Entanglement Forging History."""
 
-    evaluations: List[EntanglementForgingEvaluation] = field(default_factory=list)
-    optimal_evaluation: Optional[EntanglementForgingEvaluation] = None
+    evaluations: list[EntanglementForgingEvaluation] = field(default_factory=list)
+    optimal_evaluation: EntanglementForgingEvaluation | None = None
 
     def store_evaluation(self, evaluation: EntanglementForgingEvaluation):
         """Store an evaluation iteration and update optimal values, as necessary."""
         self.evaluations.append(evaluation)
         if (
             self.optimal_evaluation is None
             or evaluation.eigenvalue < self.optimal_evaluation.eigenvalue
@@ -94,76 +80,27 @@
 class EntanglementForgingResult(EigenstateResult):
     """Entanglement Forging Result."""
 
     def __init__(self) -> None:
         """Initialize `EigenstateResult` parent class and set class fields."""
         super().__init__()
         self._energy_shift: float = 0.0
-        self._history: List[EntanglementForgingEvaluation] = []
-
-    @property
-    def groundenergy(self) -> Optional[float]:
-        """Return ground energy."""
-        return self._groundenergy
-
-    @groundenergy.setter
-    def groundenergy(self, energy: Optional[float]) -> None:
-        """Set ground energy."""
-        self._groundenergy = energy
+        self._history: list[EntanglementForgingEvaluation] = []
 
     @property
-    def history(self) -> List[EntanglementForgingEvaluation]:
+    def history(self) -> list[EntanglementForgingEvaluation]:
         """Return optimizer history."""
         return self._history
 
     @history.setter
-    def history(self, history: List[EntanglementForgingEvaluation]) -> None:
+    def history(self, history: list[EntanglementForgingEvaluation]) -> None:
         """Set optimizer history."""
         self._history = history
 
     @property
-    def groundstate(
-        self,
-    ) -> Optional[
-        Union[
-            str,
-            dict,
-            Result,
-            list,
-            np.ndarray,
-            Statevector,
-            QuantumCircuit,
-            Instruction,
-            OperatorBase,
-        ]
-    ]:
-        """Return ground state."""
-        return self._groundstate
-
-    @groundstate.setter
-    def groundstate(
-        self,
-        groundstate: Optional[
-            Union[
-                str,
-                dict,
-                Result,
-                list,
-                np.ndarray,
-                Statevector,
-                QuantumCircuit,
-                Instruction,
-                OperatorBase,
-            ]
-        ],
-    ) -> None:
-        """Set ground state."""
-        self._groundstate = groundstate
-
-    @property
     def energy_shift(self) -> float:
         """Return the energy shift."""
         return self._energy_shift
 
     @energy_shift.setter
     def energy_shift(self, value: float) -> None:
         """Set the energy shift."""
@@ -176,311 +113,301 @@
 
     @elapsed_time.setter
     def elapsed_time(self, value: float):
         """Set the elapsed time."""
         self._elapsed_time = value
 
 
-class EntanglementForgingGroundStateSolver(GroundStateSolver):
+class EntanglementForgingGroundStateSolver:
     """A class which estimates the ground state energy of a molecule."""
 
     def __init__(
         self,
-        ansatz: Optional[EntanglementForgingAnsatz] = None,
-        service: Optional[QiskitRuntimeService] = None,
-        optimizer: Optional[Union[Optimizer, MINIMIZER]] = None,
-        initial_point: Optional[NDArray] = None,
-        orbitals_to_reduce: Optional[Sequence[int]] = None,
-        backend_names: Optional[Union[str, List[str]]] = None,
-        options: Optional[Union[Options, List[Options]]] = None,
+        ansatz: EntanglementForgingAnsatz | None = None,
+        service: QiskitRuntimeService | None = None,
+        optimizer: Optimizer | MINIMIZER | None = None,
+        initial_point: np.ndarray | None = None,
+        orbitals_to_reduce: Sequence[int] | None = None,
+        backend_names: str | list[str] | None = None,
+        options: Options | list[Options] | None = None,
+        mo_coeff: np.ndarray | None = None,
     ):
         """
         Assign the necessary class variables and initialize any defaults.
 
         Args:
-            - ansatz: Class which holes the ansatz circuit and bitstrings
+            - ansatz: Class which holds the ansatz circuit and bitstrings
             - service: The service used to spawn Qiskit primitives
             - optimizer: Optimizer to use to optimize the ansatz circuit parameters
             - initial_point: Initial values for ansatz parameters
             - orbitals_to_reduce: List of orbital indices to remove from the problem before
                 decomposition.
             - backend_names: Backend name or list of backend names to use during parallel computation
             - options: Options or list of options to be applied to the backends
+            - mo_coeff: Coefficients for converting an input problem to MO basis
 
         Returns:
             - None
         """
-        # These fields will be used when solve is called
-        self._knitter: Optional[EntanglementForgingKnitter] = None
+        # Set class fields
+        self._knitter: EntanglementForgingKnitter | None = None
         self._history: EntanglementForgingHistory = EntanglementForgingHistory()
         self._energy_shift = 0.0
-
-        # Set class fields
-        self._ansatz: Optional[EntanglementForgingAnsatz] = ansatz
-        self._service: Optional[QiskitRuntimeService] = service
-        self._initial_point: Optional[NDArray] = initial_point
+        self._ansatz: EntanglementForgingAnsatz | None = ansatz
+        self._service: QiskitRuntimeService | None = service
+        self._initial_point: np.ndarray | None = initial_point
         self._orbitals_to_reduce = orbitals_to_reduce
         self.backend_names = backend_names  # type: ignore
         self.options = options
-
-        self._optimizer: Union[Optimizer, MINIMIZER] = optimizer or SPSA()
+        self._mo_coeff = mo_coeff
+        self._optimizer: Optimizer | MINIMIZER = optimizer or SPSA()
 
     @property
-    def ansatz(self) -> Optional[EntanglementForgingAnsatz]:
+    def ansatz(self) -> EntanglementForgingAnsatz | None:
         """Return ansatz."""
         return self._ansatz
 
     @ansatz.setter
-    def ansatz(self, ansatz: Optional[EntanglementForgingAnsatz]) -> None:
+    def ansatz(self, ansatz: EntanglementForgingAnsatz | None) -> None:
         """Set the ansatz."""
         self._ansatz = ansatz
 
     @property
-    def service(self) -> Optional[QiskitRuntimeService]:
+    def service(self) -> QiskitRuntimeService | None:
         """Return service."""
         return self._service
 
     @service.setter
-    def service(self, service: Optional[QiskitRuntimeService]) -> None:
+    def service(self, service: QiskitRuntimeService | None) -> None:
         """Set the service."""
         self._service = service
 
     @property
-    def orbitals_to_reduce(self) -> Optional[Sequence[int]]:
+    def orbitals_to_reduce(self) -> Sequence[int] | None:
         """Return the orbitals to reduce."""
         return self._orbitals_to_reduce
 
     @orbitals_to_reduce.setter
-    def orbitals_to_reduce(self, orbitals_to_reduce: Optional[Sequence[int]]) -> None:
+    def orbitals_to_reduce(self, orbitals_to_reduce: Sequence[int] | None) -> None:
         """Set the orbitals to reduce."""
         self._orbitals_to_reduce = orbitals_to_reduce
 
     @property
     def optimizer(self) -> Optimizer:
         """Return the optimizer."""
         return self._optimizer
 
     @optimizer.setter
     def optimizer(self, optimizer: Optimizer) -> None:
         """Set the optimizer."""
         self._optimizer = optimizer
 
     @property
-    def initial_point(self) -> Optional[NDArray]:
+    def initial_point(self) -> np.ndarray | None:
         """Return the initial point."""
         return self._initial_point
 
     @initial_point.setter
-    def initial_point(self, initial_point: Optional[NDArray]) -> None:
+    def initial_point(self, initial_point: np.ndarray | None) -> None:
         """Set the initial point."""
         self._initial_point = initial_point
 
     @property
-    def backend_names(self) -> Optional[List[str]]:
+    def backend_names(self) -> list[str] | None:
         """Return the backend names."""
         return self._backend_names
 
     @backend_names.setter
-    def backend_names(self, backend_names: Union[str, List[str]]) -> None:
+    def backend_names(self, backend_names: str | list[str]) -> None:
         """Set the backend names."""
         if isinstance(backend_names, str):
             self._backend_names = [backend_names]
         else:
             self._backend_names = backend_names
 
     @property
-    def options(self) -> Optional[List[Options]]:
+    def options(self) -> list[Options] | None:
         """Return the options."""
         return self._options
 
     @options.setter
-    def options(self, options: Union[Options, List[Options]]) -> None:
+    def options(self, options: Options | list[Options]) -> None:
         """Set the options."""
         if isinstance(options, Options):
             self._options = [options]
         else:
             self._options = options
 
+    @property
+    def mo_coeff(self) -> np.ndarray | None:
+        """Return the coefficients for converting integrals to the MO basis."""
+        return self._mo_coeff
+
+    @mo_coeff.setter
+    def mo_coeff(self, mo_coeff: np.ndarray | None) -> None:
+        """Set the coefficients for converting integrals to the MO basis."""
+        self._mo_coeff = mo_coeff
+
     def solve(
         self,
-        problem: BaseProblem,
-        aux_operators: Optional[
-            ListOrDictType[Union[SecondQuantizedOp, PauliSumOp]]
-        ] = None,
-    ) -> EigenstateResult:
+        problem: ElectronicStructureProblem,
+    ) -> EntanglementForgingResult:
         """Compute Ground State properties.
 
         Args:
-            - problem: a class encoding a problem to be solved.
-            - aux_operators: Additional auxiliary operators to evaluate.
+            - problem: a class encoding a problem to be solved
 
         Returns:
-            - An interpreted :class:`~.EigenstateResult`. For more information see also
-            :meth:`~.BaseProblem.interpret`.
+            - A result object
+
+        Raises:
+            - ValueError:
+                The ``backend_names`` and ``options`` lists are of incompatible lengths
+            - AttributeError:
+                Ansatz must be set before calling `solve` method
         """
-        if not isinstance(problem, ElectronicStructureProblem):
-            raise AttributeError(
-                "EntanglementForgingGroundStateSolver only accepts ElectronicStructureProblem as input to its solve method."
-            )
         if self._backend_names and self._options:
             if len(self._backend_names) != len(self._options):
                 if len(self._options) == 1:
                     self._options = [self._options[0]] * len(self._backend_names)
                 else:
                     raise AttributeError(
-                        f"The list of backend names is length ({len(self._backend_names)}), but the list of options is length ({len(self._options)}). It is ambiguous how to combine the options with the backends."
+                        f"The list of backend names is length ({len(self._backend_names)}), but the list of options is "
+                        f"length ({len(self._options)}). It is ambiguous how to combine the options with the backends."
                     )
         if self._ansatz is None:
             raise AttributeError("Ansatz must be set before calling solve.")
         if self._initial_point is None:
             self._initial_point = np.array(
                 [0.0 for i in range(len(self._ansatz.circuit_u.parameters))]
             )
 
+        # Get the decomposed hamiltonian
         hamiltonian_terms = self.get_qubit_operators(problem)
         ef_operator = convert_cholesky_operator(hamiltonian_terms, self._ansatz)
 
-        if self._service:
+        # Set the knitter class field
+        if self._service is not None:
             backend_names = self._backend_names or ["ibmq_qasm_simulator"]
             self._knitter = EntanglementForgingKnitter(
                 self._ansatz,
                 service=self._service,
                 backend_names=backend_names,
                 options=self._options,
             )
         else:
             self._knitter = EntanglementForgingKnitter(
                 self._ansatz, options=self._options
             )
         self._history = EntanglementForgingHistory()
         self._eval_count = 0
-
         evaluate_eigenvalue = self.get_eigenvalue_evaluation(ef_operator)
 
+        # Minimize the minimum eigenvalue with respect to the ansatz parameters
         start_time = time()
-
         if callable(self._optimizer):
-            optimizer_result = self.optimizer(
-                fun=evaluate_eigenvalue, x0=self._initial_point
-            )
+            self.optimizer(fun=evaluate_eigenvalue, x0=self._initial_point)
         else:
-            optimizer_result = self.optimizer.minimize(
-                fun=evaluate_eigenvalue, x0=self._initial_point
-            )
-
+            self.optimizer.minimize(fun=evaluate_eigenvalue, x0=self._initial_point)
         elapsed_time = time() - start_time
 
+        # Find the minimum eigenvalue found during optimization
         optimal_evaluation = self._history.optimal_evaluation
         if optimal_evaluation is None:
             raise RuntimeError("Unable to retrieve optimal evaluation.")
 
-        result = EntanglementForgingResult()
-        result.eigenenergies = np.array(
-            [e.eigenvalue for e in self._history.evaluations]
+        # Create the EntanglementForgingResult from the results from the
+        # results of eigenvalue minimization and other meta information
+        min_eigsolver_result = MinimumEigensolverResult()
+        min_eigsolver_result.eigenvalue = optimal_evaluation.eigenvalue
+        min_eigsolver_result.eigenstate = optimal_evaluation.eigenstate
+        result = EntanglementForgingResult.from_minimum_eigensolver_result(
+            min_eigsolver_result
         )
-        result.eigenstates = np.array([e.eigenstate for e in self._history.evaluations])  # type: ignore
-        if self._history.optimal_evaluation is None:
-            raise ValueError(
-                "Something unexpected happened, and the solver was not able to find an optimal parametrization."
-            )
-        result.groundenergy = self._history.optimal_evaluation.eigenvalue
-        result.groundstate = self._history.optimal_evaluation.eigenstate
         result.energy_shift = self._energy_shift
         result.history = self._history.evaluations
         result.elapsed_time = elapsed_time
 
         # Close any runtime sessions
         self._knitter.close_sessions()
 
         return result
 
     def get_eigenvalue_evaluation(
         self, operator: EntanglementForgingOperator
-    ) -> Callable[[Sequence[float]], Union[float, Iterable[float]]]:
+    ) -> Callable[[Sequence[float]], float | Iterable[float]]:
         """Produce a callable function which provides an estimation of the minimum eigenvalue of the input operator.
 
         Args:
           - operator (EntanglementForgingOperator): The decomposed Hamiltonian in entanglement forging format
         Returns:
           - callable (Callable):  Callable function which provides an estimation of the mihnimum eigenvalue
               of the input operator given some ansatz circuit parameters.
         """
 
         def evaluate_eigenvalue(parameters: Sequence[float]) -> float:
             if self._knitter is None:
-                raise AttributeError(
-                    "Knitter must be set before evaluating eigenvalue."
-                )
+                raise RuntimeError("Knitter must be set before evaluating eigenvalue.")
 
             eigenvalue, schmidt_coeffs, _ = self._knitter(
                 ansatz_parameters=parameters, forged_operator=operator
             )
             self._history.store_evaluation(
                 EntanglementForgingEvaluation(parameters, eigenvalue, schmidt_coeffs)
             )
 
             return eigenvalue
 
         return evaluate_eigenvalue
 
     def get_qubit_operators(
         self,
-        problem: BaseProblem,
-        aux_operators: Optional[
-            ListOrDictType[Union[SecondQuantizedOp, PauliSumOp]]
-        ] = None,
-    ) -> Tuple[PauliSumOp, Optional[ListOrDictType[PauliSumOp]]]:
+        problem: ElectronicStructureProblem,
+    ) -> ListOp:
         """Construct decomposed qubit operators from an ``ElectronicStructureProblem``.
 
         Args:
-          - problem (BaseProblem): A class encoding a problem to be solved.
-          - aux_operators (ListOrDictType[Union[SecondQuantizedOp, PauliSumOp]]): Additional auxiliary operators to evaluate.
+          - problem (ElectronicStructureProblem): A class encoding a problem to be solved.
 
         Returns:
           - hamiltonian_ops: qubit operator representing the decomposed Hamiltonian.
+
+        Raises:
+            - ValueError:
+                The input problem is not in MO basis, and ``mo_coeff`` is set to ``None``
+            - ValueError:
+                The ``mo_coeff`` and input problem integrals are of incompatible shapes
+            - ValueError:
+                The input integrals are ``None``
         """
-        if not isinstance(problem, ElectronicStructureProblem):
-            raise AttributeError(
-                "EntanglementForgingGroundStateSolver only supports ElectronicStructureProblem."
-            )
-        decomposed_operator = cholesky_decomposition(problem, self._orbitals_to_reduce)
-        hamiltonian_ops = decomposed_operator[0]
-        self._energy_shift = decomposed_operator[1]
+        self._validate_problem_and_coeffs(problem, self.mo_coeff)
 
+        hamiltonian_ops, self._energy_shift = cholesky_decomposition(
+            problem, self.mo_coeff, self._orbitals_to_reduce  # type: ignore
+        )
         return hamiltonian_ops
 
-    def returns_groundstate(self) -> bool:
-        """Whether this class returns only the ground state energy or also the ground state itself.
-
-        Returns:
-            - True, if this class also returns the ground state in the results object.
-            False otherwise.
-        """
-        return True
-
-    @property
-    def qubit_converter(self):
-        """Not implemented."""
+    @staticmethod
+    def _validate_problem_and_coeffs(
+        problem: ElectronicStructureProblem, mo_coeff: np.ndarray | None
+    ):
+        """Ensure the input problem can be translated to the MO basis."""
+        if (problem.basis != ElectronicBasis.MO) and (mo_coeff is None):
+            raise ValueError(
+                f"Cannot transform integrals to MO basis. The input problem is in the ({problem.basis}) basis, "
+                "and the mo_coeff class field is None."
+            )
 
-    @property
-    def solver(self):
-        """Not implemented."""
+        h1 = np.array(problem.hamiltonian.electronic_integrals.one_body.alpha["+-"])
+        if h1.shape == ():
+            raise ValueError("The input integrals are empty.")
 
-    def evaluate_operators(
-        self,
-        state: Union[
-            str,
-            dict,
-            Result,
-            list,
-            np.ndarray,
-            Statevector,
-            QuantumCircuit,
-            Instruction,
-            OperatorBase,
-        ],
-        operators: Union[PauliSumOp, OperatorBase, list, dict],
-    ) -> Union[float, List[float], Dict[str, List[float]]]:
-        """Not necessary to implement."""
-        raise NotImplementedError(
-            "This class method is not used by EntanglementForgingGroundStateSolver."
-        )
+        # First two lines of this conditional are already implied by passing above checks, but alas, mypy :)
+        if (
+            problem.basis != ElectronicBasis.MO
+            and mo_coeff is not None
+            and mo_coeff.shape != h1.shape
+        ):
+            raise ValueError(
+                f"The mo_coeff class field has shape ({mo_coeff.shape}), but the input one body integral "
+                f"has shape ({h1.shape})."
+            )
```

### Comparing `circuit_knitting_toolbox-0.0.0/circuit_knitting_toolbox/entanglement_forging/entanglement_forging_knitter.py` & `circuit-knitting-toolbox-0.1.0/circuit_knitting_toolbox/entanglement_forging/entanglement_forging_knitter.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,79 +6,67 @@
 # obtain a copy of this license in the LICENSE.txt file in the root directory
 # of this source tree or at http://www.apache.org/licenses/LICENSE-2.0.
 # Any modifications or derivative works of this code must retain this
 # copyright notice, and modified files need to carry a notice indicating
 # that they have been altered from the originals.
 
 """File containing the knitter class and associated functions."""
+
+from __future__ import annotations
+
 import time
 import logging
-from typing import List, Optional, Sequence, Tuple, Union, Any, Dict
+from typing import Sequence, Any
 from concurrent.futures import ThreadPoolExecutor
 
 import numpy as np
-from nptyping import Float, Int, NDArray, Shape
 
 from qiskit import QuantumCircuit
 from qiskit.quantum_info import Pauli
 from qiskit.primitives import Estimator as TestEstimator
 from qiskit_ibm_runtime import QiskitRuntimeService, Session, Options, Estimator
 
-from .entanglement_forging_ansatz import Bitstring, EntanglementForgingAnsatz
+from .entanglement_forging_ansatz import EntanglementForgingAnsatz
 from .entanglement_forging_operator import EntanglementForgingOperator
 
 logger = logging.getLogger(__name__)
 
 
 class EntanglementForgingKnitter:
     """Container for Knitter class functions and attributes.
 
     A class which performs entanglement forging and returns the
     ground state energy and Schmidt coefficients found for given
     ansatz parameters and Schmidt coefficients.
     """
 
-    # Attributes:
-    #     - _ansatz (EntanglementForgingAnsatz): the ansatz containing the
-    #         information for the circuit structure and bitstrings to be used
-    #     - _backend_names (List[str]): the names of the backends to use
-    #     - _service (QiskitRuntimeService): the service used to access backends
-    #     - _tensor_circuits_u (List[QuantumCircuit]): the set of circuits used for the first
-    #         operator that have the same Schmidt values
-    #     - _superposition_circuits_u (List[QuantumCircuit]): the set of circuits used for
-    #         the first operator that have different Schmidt values
-    #     - _tensor_circuits_v (List[QuantumCircuit]): the set of circuits used for the second
-    #         operator that have the same Schmidt values
-    #     - _superposition_circuits_v (List[QuantumCircuit]): the set of circuits used for
-    #         the second operator that have different Schmidt values
-
     def __init__(
         self,
         ansatz: EntanglementForgingAnsatz,
-        service: Optional[QiskitRuntimeService] = None,
-        backend_names: Optional[Union[str, List[str]]] = None,
-        options: Optional[Union[Options, List[Options]]] = None,
+        service: QiskitRuntimeService | None = None,
+        backend_names: str | list[str] | None = None,
+        options: Options | list[Options] | None = None,
     ):
         """
         Assign the necessary member variables.
 
         Args:
             - ansatz (EntanglementForgingAnsatz): The container for the circuit structure and bitstrings
                 to be used (and generate the stateprep circuits)
             - service (QiskitRuntimeService): The service used to spawn Qiskit primitives and runtime jobs
-            - backend_names (List[str]): Names of the backends to use for calculating expectation values
-            - options (List[Options]): Options to use with the backends
+            - backend_names (list[str]): Names of the backends to use for calculating expectation values
+            - options (list[Options]): Options to use with the backends
 
         Returns:
             - None
         """
         # Call backend_names setter to update the session_ids hidden class field
-        self._session_ids: Optional[List[Union[str, None]]] = None
-        self._backend_names: Optional[List[str]] = None
-        self._options: Optional[List[Options]] = None
+        self._session_ids: list[str | None] | None = None
+        self._backend_names: list[str] | None = None
+        self._options: list[Options] | None = None
         # Call constructors
         self.backend_names = backend_names  # type: ignore
         self.options = options
 
         # The service hidden class field is a json representing the QiskitRuntimeService object
         self._service = service.active_account() if service is not None else service
 
@@ -121,79 +109,79 @@
 
         Returns:
             - (EntanglementForgingAnsatz): the ansatz member variable
         """
         return self._ansatz
 
     @property
-    def backend_names(self) -> Optional[List[str]]:
+    def backend_names(self) -> list[str] | None:
         """
         List of backend names to be used.
 
         Returns:
-            - (List[str]): the backend_names member variable
+            - (list[str]): the backend_names member variable
         """
         return self._backend_names
 
     @backend_names.setter
-    def backend_names(self, backend_names: Optional[Union[str, List[str]]]) -> None:
+    def backend_names(self, backend_names: str | list[str] | None) -> None:
         """
         Change the backend_names class field.
 
         Args:
-            - backend_names (List[str]): the list of backends to use
+            - backend_names (list[str]): the list of backends to use
 
         Returns:
             - None
         """
         if isinstance(backend_names, str):
             self._backend_names = [backend_names]
         else:
             self._backend_names = backend_names
         if backend_names:
             self._session_ids = [None] * len(backend_names)
 
     @property
-    def options(self) -> Optional[List[Options]]:
+    def options(self) -> list[Options] | None:
         """
         List of options to be used.
 
         Returns:
-            - (List[Options]): the options member variable
+            - (list[Options]): the options member variable
         """
         return self._options
 
     @options.setter
-    def options(self, options: Optional[Union[Options, List[Options]]]) -> None:
+    def options(self, options: Options | list[Options] | None) -> None:
         """
         Change the options class field.
 
         Args:
-            - options (List[Options]): the list of options to use
+            - options (list[Options]): the list of options to use
 
         Returns:
             - None
         """
         if isinstance(options, Options):
             self._options = [options]
         else:
             self._options = options
 
     @property
-    def service(self) -> Optional[QiskitRuntimeService]:
+    def service(self) -> QiskitRuntimeService | None:
         """
         Property function for service class field.
 
         Returns:
             - (QiskitRuntimeService): the service member variable
         """
         return QiskitRuntimeService(**self._service)
 
     @service.setter
-    def service(self, service: Optional[QiskitRuntimeService]) -> None:
+    def service(self, service: QiskitRuntimeService | None) -> None:
         """
         Change the service class field.
 
         Args:
             - service (QiskitRuntimeService): the service used to spawn Qiskit primitives
 
         Returns:
@@ -201,17 +189,15 @@
         """
         self._service = service.active_account() if service is not None else service
 
     def __call__(
         self,
         ansatz_parameters: Sequence[float],
         forged_operator: EntanglementForgingOperator,
-    ) -> Tuple[
-        float, NDArray[Shape["*"], Float], NDArray[Shape["*, *"], Float]
-    ]:  # noqa: D301, D202
+    ) -> tuple[float, np.ndarray, np.ndarray]:
         r"""Calculate the energy.
 
         Computes ⟨H⟩ - the energy value and the Schmidt matrix, $h_{n, m}$, given
         some ansatz parameter values.
 
         $h_{n, n} = \sum_{a, b} w_{a, b} \left [ \lambda_n^2 \langle b_n | U^t P_a U | b_n \rangle
             \langle b_n | V^t P_b V | b_n \rangle \right ]$
@@ -229,15 +215,15 @@
             - self
             - ansatz_parameters (Sequence[float]): the parameters to be used by the ansatz circuit,
                 must be the same length as the circuit's parameters
             - forged_operator (EntanglementForgingOperator): the operator to forge the expectation
                 value from
 
         Returns:
-            - (Tuple[float, NDArray[Shape["*"], Float], NDArray[Shape["*, *"], Float]]): a tuple
+            - (tuple[float, np.ndarray, np.ndarray]): a tuple
                 containing the energy (i.e. forged expectation value), the Schmidt coefficients,
                 and the full Schmidt decomposition matrix
         """
         if self._backend_names and self._options:
             if len(self._backend_names) != len(self._options):
                 if len(self._options) == 1:
                     self._options = [self._options[0]] * len(self._backend_names)
@@ -284,15 +270,15 @@
         )
 
         # Get the RuntimeService as a hashable dictionary
         service_args = None
         if self._service:
             service_args = self._service
 
-        session_ids: Optional[List[Union[str, None]]] = None
+        session_ids: list[str | None] | None = None
         if self._session_ids is None:
             session_ids = [None] * num_partitions
         else:
             session_ids = self._session_ids
 
         partitioned_expval_futures = []
         with ThreadPoolExecutor() as executor:
@@ -353,32 +339,31 @@
         energy = evals[0]
 
         return energy, schmidt_coeffs, h_schmidt
 
     def _compute_h_schmidt(
         self,
         forged_operator: EntanglementForgingOperator,
-        tensor_expvals: NDArray[Shape["*, *"], Float],
-        superpos_expvals: NDArray[Shape["*, *"], Float],
-    ) -> NDArray[Shape["*, *"], Float]:  # noqa: D202
+        tensor_expvals: np.ndarray,
+        superpos_expvals: np.ndarray,
+    ) -> np.ndarray:
         """
         Compute the Schmidt decomposition of the Hamiltonian.
 
         Args:
             - forged_operator (EntanglementForgingOperator): the operator that the
                 forged expectation values are computed with
-            - tensor_expvals (NDArray[Shape["*, *"], Float]): the expectation values
+            - tensor_expvals (np.ndarray): the expectation values
                 for the tensor circuits (i.e. same Schmidt coefficients)
-            - superpos_expvals (NDArray[Shape["*, *"], Float]): the expectation values
+            - superpos_expvals (np.ndarray): the expectation values
                 for the superposition circuits (i.e. different Schmidt coefficients)
 
         Returns:
-           - (NDArray[Shape["*, *"], Float]): the Schmidt matrix
+           - (np.ndarray): the Schmidt matrix
         """
-
         # Calculate the diagonal entries of the Schmidt matrix by
         # summing the expectation values associated with the tensor terms
         # h𝑛𝑛 = Σ_ab 𝑤𝑎𝑏•[ 𝜆𝑛^2•⟨b𝑛|U^t•P𝑎•U|b𝑛⟩⟨b𝑛|V^t•P𝑏•V|b𝑛⟩ ]
         if self._ansatz.bitstrings_are_symmetric:
             h_schmidt_diagonal = np.einsum(
                 "ij, xi, xj->x",
                 forged_operator.w_ij,  # type: ignore
@@ -463,17 +448,17 @@
                 session._session_id = session_id
                 session.close()
 
         return
 
 
 def _construct_stateprep_circuits(
-    bitstrings: List[Bitstring],
-    subsystem_id: Optional[str] = None,
-) -> Tuple[List[QuantumCircuit], List[QuantumCircuit]]:  # noqa: D301
+    bitstrings: list[tuple[int, ...]],
+    subsystem_id: str | None = None,
+) -> tuple[list[QuantumCircuit], list[QuantumCircuit]]:
     r"""Prepare all circuits.
 
     Function to make the state preparation circuits. This constructs a set
     of circuits $ | b_n \rangle $ and $ | \phi^{p}_{n, m} \rangle $.
 
     The circuits $ | b_n \rangle $ are computational basis states specified by
     bitstrings $ b_n $, while the circuits $ | \phi^{p}_{n, m} \rangle $ are
@@ -519,19 +504,19 @@
          ┌───┐┌───┐
     q_0: ┤ H ├┤ Z ├──■──
          ├───┤└───┘┌─┴─┐
     q_1: ┤ X ├─────┤ X ├
          └───┘     └───┘
 
     Args:
-        - bitstrings (List[Bitstring]): the input list of bitstrings used to generate the state preparation circuits
-        - subsystem_id (Optional[str]): the subsystem the bitstring reflects ("u" or "v")
+        - bitstrings (list[tuple[int, ...]]): the input list of bitstrings used to generate the state preparation circuits
+        - subsystem_id (str | None): the subsystem the bitstring reflects ("u" or "v")
 
     Returns:
-        - (Tuple[List[QuantumCircuit], List[QuantumCircuit]]): A tuple containing the tensor (i.e., non-superposition
+        - (tuple[list[QuantumCircuit], list[QuantumCircuit]]): A tuple containing the tensor (i.e., non-superposition
             or bitstring) circuits in the first index (length = len(bitstrings)) and the super-position circuits
             as the second element
     """
     # If empty, just return
     if not bitstrings:
         return [], []
 
@@ -589,24 +574,24 @@
                 ]
                 superpos_prep_circuits += [psi_xplus, psi_xmin]
 
     return tensor_prep_circuits, superpos_prep_circuits
 
 
 def _prepare_bitstring(
-    bitstring: Union[NDArray[Shape["*"], Int], Bitstring],
-    name: Optional[str] = None,
+    bitstring: np.ndarray | tuple[int, ...],
+    name: str | None = None,
 ) -> QuantumCircuit:
     """Prepare the bitstring circuits.
 
     Generate a computational basis state from the input bitstring by applying an X gate to
     every qubit that has a 1 in the bitstring.
 
     Args:
-        - bitstring (Union[NDArray[Shape["*"], Int], Bitstring]): the container for the
+        - bitstring (np.ndarray | tuple[int, ...]): the container for the
             bitstring information. Must contain 0s and 1s and the 1s are used to determine
             where to put the X gates
         - name (str, optional): the name of the circuit
 
     Returns:
         - (QuantumCircuit): the prepared circuit
     """
@@ -632,70 +617,67 @@
         - (generator): the generator containing the paritions
     """
     k, m = divmod(len(a), n)
     return (a[i * k + min(i, m) : (i + 1) * k + min(i + 1, m)] for i in range(n))
 
 
 def _estimate_expvals(
-    tensor_ansatze: List[QuantumCircuit],
-    tensor_paulis: List[Pauli],
-    superposition_ansatze: List[QuantumCircuit],
-    superposition_paulis: List[Pauli],
-    service_args: Optional[Dict[str, Any]] = None,
-    backend_name: Optional[str] = None,
-    options: Optional[Options] = None,
-    session_id: Optional[str] = None,
-) -> Tuple[List[NDArray], List[NDArray], Optional[str]]:
+    tensor_ansatze: list[QuantumCircuit],
+    tensor_paulis: list[Pauli],
+    superposition_ansatze: list[QuantumCircuit],
+    superposition_paulis: list[Pauli],
+    service_args: dict[str, Any] | None = None,
+    backend_name: str | None = None,
+    options: Options | None = None,
+    session_id: str | None = None,
+) -> tuple[list[np.ndarray], list[np.ndarray], str | None]:
     """Run quantum circuits to generate the expectation values.
 
     Function to estimate the exepctation value of some observables on the
     tensor and superposition circuits used for reconstructing the full
     expectation value from the Schmidt decomposed circuit. The ray decorator
     indicates that this is an actor function (that runs its own python
     process).
 
     Args:
-        - tensor_ansatze (List[QuantumCircuit]): the circuits that have the same
+        - tensor_ansatze (list[QuantumCircuit]): the circuits that have the same
             Schmidt coefficient
-        - tensor_paulis (List[Pauli]): the pauli operators to measure and calculate
+        - tensor_paulis (list[Pauli]): the pauli operators to measure and calculate
             the expectation values from for the circuits with the same Schmidt coefficient
-        - superposition_ansatze (List[QuantumCircuit]): the circuits with different
+        - superposition_ansatze (list[QuantumCircuit]): the circuits with different
             Schmidt coefficients
-        - superposition_paulis (List[Pauli]): the pauli operators to measure and calculate
+        - superposition_paulis (list[Pauli]): the pauli operators to measure and calculate
             the expectation values from for the circuits with different Schmidt
             coefficients
-        - service_args (Dict[str, Any]): The service account used to spawn Qiskit primitives
+        - service_args (dict[str, Any]): The service account used to spawn Qiskit primitives
         - backend_name (str): The backend to use to evaluate the grouped experiments
         - options (Options): The options to use with the backend
         - session_id (str): The session id to use when calling primitive programs
 
     Returns:
-        - (Tuple[List[NDArray], List[NDArray], Optional[str]]): the expectation values for the
+        - (tuple[list[np.ndarray], list[np.ndarray], str | None]): the expectation values for the
             tensor circuits and superposition circuits
     """
-    all_circuits = tensor_ansatze + superposition_ansatze
-    all_observables = tensor_paulis + superposition_paulis
-
-    ansatz_t: List[QuantumCircuit] = []
-    observables_t: List[Pauli] = []
+    ansatz_t: list[QuantumCircuit] = []
+    observables_t: list[Pauli] = []
     for i, circuit in enumerate(tensor_ansatze):
         ansatz_t += [circuit] * len(tensor_paulis)
         observables_t += tensor_paulis
 
-    ansatz_s: List[QuantumCircuit] = []
-    observables_s: List[Pauli] = []
+    ansatz_s: list[QuantumCircuit] = []
+    observables_s: list[Pauli] = []
     for i, circuit in enumerate(superposition_ansatze):
         ansatz_s += [circuit] * len(superposition_paulis)
         observables_s += superposition_paulis
 
     all_ansatze_for_estimator = ansatz_t + ansatz_s
     all_observables_for_estimator = observables_t + observables_s
 
     # ID for this job. If it is the first job for the knitter, it will become the session ID
-    job_id: Optional[str] = None
+    job_id: str | None = None
     if service_args is not None:
         # Set the backend. Default to runtime qasm simulator
         if backend_name is None:
             raise ValueError(
                 "If passing a QiskitRuntimeService, a list of backend names must be specified."
             )
         service = QiskitRuntimeService(**service_args)
@@ -724,18 +706,15 @@
             raise RuntimeError("A None result was returned from Qiskit Runtime.")
 
         results = job.result().values
 
         job_id = job.job_id
 
     else:
-        estimator = TestEstimator(
-            circuits=all_circuits,
-            observables=all_observables,
-        )
+        estimator = TestEstimator()
         results = (
             estimator.run(
                 circuits=all_ansatze_for_estimator,
                 observables=all_observables_for_estimator,
             )
             .result()
             .values
```

### Comparing `circuit_knitting_toolbox-0.0.0/circuit_knitting_toolbox/entanglement_forging/entanglement_forging_operator.py` & `circuit-knitting-toolbox-0.1.0/circuit_knitting_toolbox/entanglement_forging/entanglement_forging_operator.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,17 +10,16 @@
 # that they have been altered from the originals.
 
 """File containing the entanglement forging operator."""
 
 from dataclasses import dataclass
 from typing import Sequence
 
-from nptyping import Float, NDArray, Shape
-from qiskit.quantum_info import Pauli
 import numpy as np
+from qiskit.quantum_info import Pauli
 
 
 @dataclass
 class EntanglementForgingOperator:  # noqa: D301
     r"""Operator class for Entanglement Forging.
 
     A class that contains the :math:`2N` qubit Pauli operator :math:`\hat{O} = \sum_{i, j} w_{i, j} \hat{T}_{i, j} \otimes \sum_{a, b} \hat{S}_{a, b}`
@@ -28,35 +27,35 @@
     energy for the :class:`EntanglementForgingVQE`.
 
     Attributes:
         - tensor_paulis (Sequence[PauliOp]): The operators acting on the subsystems that have the same
             Schmidt coefficients
         - superposition_paulis (Sequence[PauliOp]): The operators acting on subsystems that have different
             Schmidt coefficients
-        - w_ij (NDArray[Shape["\*, \*"], Float]): The weight matrix associated with the tensor paulis
-        - w_ab (NDArray[Shape["\*, \*"], Float]): The weight matrix associated with the superposition paulis
+        - w_ij (np.ndarray): The weight matrix associated with the tensor paulis
+        - w_ab (np.ndarray): The weight matrix associated with the superposition paulis
     """
 
     def __init__(
         self,
         tensor_paulis: Sequence[Pauli],
         superposition_paulis: Sequence[Pauli],
-        w_ij: NDArray[Shape["*, *"], Float],
-        w_ab: NDArray[Shape["*, *"], Float],
+        w_ij: np.ndarray,
+        w_ab: np.ndarray,
     ):
         r"""
         Assign the necessary member variables.
 
         Args:
             - tensor_paulis (Sequence[PauliOp]): The operators acting on the subsystems that have the same
                 Schmidt coefficients
             - superposition_paulis (Sequence[PauliOp]): The operators acting on subsystems that have different
                 Schmidt coefficients
-            - w_ij (NDArray[Shape["\*, \*"], Float]): The weight matrix associated with the tensor paulis
-            - w_ab (NDArray[Shape["\*, \*"], Float]): The weight matrix associated with the superposition paulis
+            - w_ij (np.ndarray): The weight matrix associated with the tensor paulis
+            - w_ab (np.ndarray): The weight matrix associated with the superposition paulis
 
         Returns:
             - None
         """
         self.tensor_paulis = tensor_paulis
         self.superposition_paulis = superposition_paulis
         self.w_ij = w_ij
```

### Comparing `circuit_knitting_toolbox-0.0.0/circuit_knitting_toolbox/utils/conversion.py` & `circuit-knitting-toolbox-0.1.0/circuit_knitting_toolbox/utils/conversion.py`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.0.0/circuit_knitting_toolbox/utils/metrics.py` & `circuit-knitting-toolbox-0.1.0/circuit_knitting_toolbox/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.0.0/circuit_knitting_toolbox/utils/orbital_reduction.py` & `circuit-knitting-toolbox-0.1.0/circuit_knitting_toolbox/utils/orbital_reduction.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,8 +34,8 @@
     Returns:
         - (List[Tuple]): the list of reduced bitstrings
 
     """
     reduced_bitstrings_list = np.delete(
         bitstrings, orbitals_to_reduce, axis=-1
     ).tolist()
-    return [tuple(l) for l in reduced_bitstrings_list]
+    return [tuple(bs) for bs in reduced_bitstrings_list]
```

### Comparing `circuit_knitting_toolbox-0.0.0/docs/_static/gallery.css` & `circuit-knitting-toolbox-0.1.0/docs/_static/gallery.css`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.0.0/docs/_static/no_image.png` & `circuit-knitting-toolbox-0.1.0/docs/_static/no_image.png`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.0.0/docs/conf.py` & `circuit-knitting-toolbox-0.1.0/docs/conf.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,36 +19,36 @@
 # General options:
 from pathlib import Path
 import sys
 
 from importlib_metadata import version as metadata_version
 
 project = "Circuit Knitting Toolbox"
-copyright = "2022"  # pylint: disable=redefined-builtin
+copyright = "2023"  # pylint: disable=redefined-builtin
 author = "IBM Quantum"
 
 _rootdir = Path(__file__).parent.parent
 sys.path.insert(0, str(_rootdir))
 
 # The full version, including alpha/beta/rc tags
 release = metadata_version("circuit_knitting_toolbox")
 # The short X.Y version
-version = version = ".".join(release.split(".")[:2])
+version = ".".join(release.split(".")[:2])
 
 extensions = [
     "sphinx.ext.napoleon",
     "sphinx.ext.autodoc",
     "sphinx.ext.autosummary",
     "sphinx.ext.mathjax",
     "sphinx.ext.viewcode",
     "sphinx.ext.extlinks",
     # "sphinx.ext.autosectionlabel",
     "jupyter_sphinx",
     "sphinx_autodoc_typehints",
-    # "reno.sphinxext",
+    "reno.sphinxext",
     "nbsphinx",
     "sphinx_copybutton",
 ]
 templates_path = ["_templates"]
 numfig = True
 numfig_format = {"table": "Table %s"}
 language = "en"
```

### Comparing `circuit_knitting_toolbox-0.0.0/docs/explanation/entanglement_forging/figs/Fig_5_c.png` & `circuit-knitting-toolbox-0.1.0/docs/entanglement_forging/explanation/figs/Fig_5_c.png`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.0.0/docs/explanation/entanglement_forging/figs/forging_info_graphic.png` & `circuit-knitting-toolbox-0.1.0/docs/entanglement_forging/explanation/figs/forging_info_graphic.png`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.0.0/docs/explanation/entanglement_forging/index.rst` & `circuit-knitting-toolbox-0.1.0/docs/entanglement_forging/explanation/index.rst`

 * *Files 24% similar despite different names*

```diff
@@ -134,20 +134,14 @@
 when picking orbitals to freeze. One good rule of thumb is to freeze the
 core orbital (for the case of water, this is the core oxygen 1s
 orbital). Furthermore, in the case of water, it turns out that orbital 3
 (corresponding to the out-of-plane oxygen 2p orbitals) has different
 symmetry to the other orbitals, so excitations to orbital 3 are
 suppressed. For water, we thus freeze orbitals 0 and 3.
 
-The core orbitals can be found with the following code:
-
-::
-
-    qmolecule = driver.run()
-    print(f"Core orbitals: {qmolecule.core_orbitals}")
 
 Example: Water molecule
 ^^^^^^^^^^^^^^^^^^^^^^^
 
 The total number of orbitals (core + valence) = 7 orbitals
 
 Frozen orbital approximation = 2 orbitals
@@ -162,15 +156,15 @@
     >>> from circuit_knitting_toolbox.utils import reduce_bitstrings
     >>> orbitals_to_reduce = [0,3]
     >>> bitstrings = [(1,1,1,1,1,0,0), (1,0,1,1,1,0,1), (1,0,1,1,1,1,0)]
     >>> reduced_bitstrings = reduce_bitstrings(bitstrings, orbitals_to_reduce)
     >>> print(f'Bitstrings after orbital reduction: {reduced_bitstrings}')
     Bitstrings after orbital reduction: [[1, 1, 1, 0, 0], [0, 1, 1, 0, 1], [0, 1, 1, 1, 0]]
 
-A complete example is provided in the `guide on freezing orbitals <../../how-tos/entanglement_forging/12-freeze-orbitals.ipynb>`_.
+A complete example is provided in the `guide on freezing orbitals <../how-tos/freeze-orbitals.ipynb>`_.
 
 .. _Picking the bitstrings:
 
 Picking the bitstrings
 ~~~~~~~~~~~~~~~~~~~~~~
 
 General Considerations
@@ -201,34 +195,14 @@
 
 Further reduction in computational resources can be achieved by
 :ref:`freezing some orbitals <Freezing orbitals>`
 that do not participate in electronic excitations (i.e. core orbitals or
 those that lie out of symmetry) by removing the bits that correspond to
 them.
 
-Fixing the Hartree-Fock bitstring
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
-
-In some cases, it is possible to increase the accuracy of simulations
-and speed up the execution by setting ``fix_first_bitstring=True`` in
-``EntanglementForgedConfig``. This bypasses the computation of the first
-bitstring and replaces the result with HF energy.
-
-This setting requires an ansatz that leaves the Hartree-Fock (HF) state
-unchanged under ``var_form``. As a rule of thumb, this can be achieved
-by restricting entanglement between the qubits representing occupied
-orbitals (bits = 1) in the HF state and the qubits representing
-unoccupied orbitals (bits = 0) in the HF state.
-
-For example, this figure from [1] shows the A, B, and C qubits entangled
-with the hop gates, D & E qubits entangled with hop gates, while the
-partition between (A,B,C) and (D,E) are only entangled with a CZ gate.
-
-.. figure:: figs/Fig_5_c.png
-
 .. _Ansatz design:
 
 Designing the ansatz used in Entanglement Forging
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 Because entanglement forging leverages a near-term, heuristic algorithm
 (namely, VQE), a judicious choice for the VQE ansatz can improve
@@ -236,60 +210,14 @@
 unitaries :math:`U` and :math:`V` in the Schmidt decomposition with parameters. An
 open question is how to choose the best unitaries for a given problem.
 
 For a chemistry simulation problem, the number of qubits in the circuit
 must equal the number of orbitals (minus the number of frozen orbitals,
 if applicable).
 
-Picking the backend
-~~~~~~~~~~~~~~~~~~~
-
-``backend`` is an option in the
-``EntanglementForgedConfig``
-class. Users can choose between Statevector simulation, QASM simulation,
-or real quantum hardware.
-
-Statevector simulation is useful when we want to:
-
-1. get the exact values of energies (e.g. for chemistry problems)
-   without any error bars (assuming there are no other sources of
-   randomness)
-2. test the performance of an algorithm in the absence of shot noise
-   (for VQE, there could be a difference between the trajectory of the
-   parameters in the presence and absence of shot noise; in this case
-   the statevector simulator can concretely provide an answer
-   regarding the expressivity of a given ansatz without any
-   uncertainty coming from shot noise)
-
-QASM simulation is useful when:
-
-1. the system sizes are larger because the statevector simulator
-   scales exponentially in system size and will not be useful beyond
-   small systems
-2. simulating circuits with noise to mimic a real noisy quantum
-   computer
-
-When running the entanglement forging module either on the QASM
-simulator or on real quantum hardware, several additional options are
-available: ``shots``, ``bootstrap_trials``, ``copysample_job_size``,
-``meas_error_mit``, ``meas_error_shots``,
-``meas_error_refresh_period_minutes``, ``zero_noise_extrap``. These
-options can be specified in the ``EntanglementForgedConfig``
-class. Users can use the QASM simulator to test out these options before
-running them on real quantum hardware.
-
-Notes:
-
-- In the limit of infinite shots, the mean value of the QASM simulator
-  will be equal to the value of the statevector simulator.
-- The QASM simulator also has a method that `mimics the statevector
-  simulator
-  <https://qiskit.org/documentation/tutorials/simulators/1_aer_provider.html>`__
-  without shot noise as an alternative to statevector simulator.
-
 ⚠️ Current limitations
 ----------------------
 
 Ansatz & bitstrings
 ~~~~~~~~~~~~~~~~~~~
 
 -  It is currently an open problem how to pick the best circuit
@@ -302,34 +230,14 @@
 
    -  For molecular calculations, one can usually force the ansatz to be
       real. On the other hand, in crystalline solids (away from the
       gamma point and without inversion symmetry), the Hamiltonian is
       defined by the complex numbers.
    -  There are plans in the future to implement complex ansatze.
 
-Orbitals
-~~~~~~~~
-
--  The current implementation of Forged VQE also requires that the
-   number of alpha particles equals the number of beta particles. The
-   relevant parameters can be found with the following code:
-
-::
-
-    qmolecule = driver.run()
-    print(f"Number of spatial orbitals: {qmolecule.num_molecular_orbitals}")
-    print(f"Number of alpha particles: {qmolecule.num_alpha}")
-    print(f"Number of beta particles: {qmolecule.num_beta}")
-
-Converter
-~~~~~~~~~
-
--  The current implementation only supports the ``JordanWignerMapper``
-   converter.
-
 Results
 ~~~~~~~
 
 -  In the current implementation, only the energy of the final state is
    available. It would be useful to have a feature to output the 1- and
    2-body density matrices of the final state after the optimization.
 
@@ -350,25 +258,20 @@
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 Results on hardware will not be as good as on the QASM simulator.
 Getting good results will require using a quantum backend with good
 properties (qubit fidelity, gate fidelity etc.), as well as a lot of
 fine-tuning of parameters.
 
-Unsupported Qiskit VQE features
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-
-This module is based on Qiskit’s Variational Quantum Eigensolver (VQE)
-algorithm, however, some of the features available in VQE are not
-currently supported by this module. Here is a list of known features
-that are not supported:
-
--  Using ``QuantumInstance`` instead of ``backend``.
+Pauli grouping
+~~~~~~~~~~~~~~
 
-This list is not exhaustive.
+There is currently no Pauli grouping for the expectation value experiments
+calculated at each iteration, so expectation values are calculated on the
+full Pauli basis. This can result in long training times for larger systems.
 
 References
 ----------
 
 This module is based on the theory and experiment described in the
 following paper:
```

### Comparing `circuit_knitting_toolbox-0.0.0/docs/how-tos/entanglement_forging/freeze-orbitals.ipynb` & `circuit-knitting-toolbox-0.1.0/docs/entanglement_forging/how-tos/freeze-orbitals.ipynb`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9731026785714285%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(2, 'In this guide, we apply Entanglement Forging to compute "*

 * *            'the energy of a $\\\\mathrm{H}_2\\\\mathrm{O}$ molecule. We reduce the number of '*

 * *            'orbitals in the problem, in turn reducing the number of qubits needed in each '*

 * *            'circuit, following the logic given in the [explanatory '*

 * *            "material](../explanation/index.rst).')], delete: [2]}}, 2: {'source': {insert: [(6, "*

 * *            "'from qiskit_nature.second_q.drivers imp […]*

```diff
@@ -2,15 +2,15 @@
     "cells": [
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# How to freeze orbitals (with the H\u2082O molecule as an example)\n",
                 "\n",
-                "In this guide, we apply Entanglement Forging to compute the energy of a $\\mathrm{H}_2\\mathrm{O}$ molecule. We reduce the number of orbitals in the problem, in turn reducing the number of qubits needed in each circuit, following the logic given in the [explanatory material](../../explanation/entanglement_forging/index.rst)."
+                "In this guide, we apply Entanglement Forging to compute the energy of a $\\mathrm{H}_2\\mathrm{O}$ molecule. We reduce the number of orbitals in the problem, in turn reducing the number of qubits needed in each circuit, following the logic given in the [explanatory material](../explanation/index.rst)."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Import the relevant modules\n",
@@ -32,20 +32,17 @@
             "source": [
                 "from matplotlib import pyplot as plt\n",
                 "import numpy as np\n",
                 "\n",
                 "from qiskit.circuit import QuantumCircuit, Parameter\n",
                 "from qiskit.circuit.library import TwoLocal\n",
                 "from qiskit.algorithms.optimizers import COBYLA\n",
-                "from qiskit_nature.drivers import Molecule\n",
-                "from qiskit_nature.drivers.second_quantization import PySCFDriver\n",
-                "from qiskit_nature.problems.second_quantization import ElectronicStructureProblem\n",
-                "from qiskit_nature.mappers.second_quantization import JordanWignerMapper\n",
-                "from qiskit_nature.converters.second_quantization import QubitConverter\n",
-                "from qiskit_nature.algorithms.ground_state_solvers import (\n",
+                "from qiskit_nature.second_q.drivers import PySCFDriver\n",
+                "from qiskit_nature.second_q.problems import ElectronicStructureProblem, ElectronicBasis\n",
+                "from qiskit_nature.second_q.algorithms import (\n",
                 "    GroundStateEigensolver,\n",
                 "    NumPyMinimumEigensolverFactory,\n",
                 ")\n",
                 "\n",
                 "from circuit_knitting_toolbox.entanglement_forging import (\n",
                 "    EntanglementForgingAnsatz,\n",
                 "    EntanglementForgingGroundStateSolver,\n",
@@ -77,91 +74,38 @@
                 "radius_2 = 0.958  # position for the second H atom\n",
                 "thetas_in_deg = 104.478  # bond angles.\n",
                 "\n",
                 "H1_x = radius_1\n",
                 "H2_x = radius_2 * np.cos(np.pi / 180 * thetas_in_deg)\n",
                 "H2_y = radius_2 * np.sin(np.pi / 180 * thetas_in_deg)\n",
                 "\n",
-                "molecule = Molecule(\n",
-                "    geometry=[\n",
-                "        [\"O\", [0.0, 0.0, 0.0]],\n",
-                "        [\"H\", [H1_x, 0.0, 0.0]],\n",
-                "        [\"H\", [H2_x, H2_y, 0.0]],\n",
-                "    ],\n",
-                "    charge=0,\n",
-                "    multiplicity=1,\n",
+                "driver = PySCFDriver(\n",
+                "    f\"O 0.0 0.0 0.0; H {H1_x} 0.0 0.0; H {H2_x} {H2_y} 0.0\", basis=\"sto6g\"\n",
                 ")\n",
-                "driver = PySCFDriver.from_molecule(molecule=molecule, basis=\"sto6g\")\n",
-                "problem = ElectronicStructureProblem(driver)\n",
-                "converter = QubitConverter(JordanWignerMapper())"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "### Compute the classical result\n",
-                "\n",
-                "For comparison, we also use `numpy` to compute the classical result. "
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 3,
-            "metadata": {
-                "ExecuteTime": {
-                    "end_time": "2021-04-27T13:41:08.499392Z",
-                    "start_time": "2021-04-27T13:41:08.080069Z"
-                }
-            },
-            "outputs": [
-                {
-                    "name": "stderr",
-                    "output_type": "stream",
-                    "text": [
-                        "/Users/caleb/opt/anaconda3/envs/ckt/lib/python3.7/site-packages/qiskit_nature/problems/second_quantization/electronic/electronic_structure_problem.py:93: ListAuxOpsDeprecationWarning: List-based `aux_operators` are deprecated as of version 0.3.0 and support for them will be removed no sooner than 3 months after the release. Instead, use dict-based `aux_operators`. You can switch to the dict-based interface immediately, by setting `qiskit_nature.settings.dict_aux_operators` to `True`.\n",
-                        "  second_quantized_ops = self._grouped_property_transformed.second_q_ops()\n"
-                    ]
-                },
-                {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "Classical energy =  -75.72890671869246\n"
-                    ]
-                }
-            ],
-            "source": [
-                "solver = GroundStateEigensolver(\n",
-                "    converter, NumPyMinimumEigensolverFactory(use_default_filter_criterion=False)\n",
-                ")\n",
-                "\n",
-                "result = solver.solve(problem)\n",
-                "classical_energy = result.total_energies[0]\n",
-                "\n",
-                "print(\"Classical energy = \", classical_energy)"
+                "driver.run()\n",
+                "problem = driver.to_problem(basis=ElectronicBasis.AO)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Prepare the bitstrings and the ansatz"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "The ansatz for Entanglement Forging consists of a set of input bitstrings and a parameterized circuit. (See the \"explanatory material\" section of the documentation for additional background on the method.) For this demo, we will use the same bitstrings and ansatz for both the U and V subsystems. "
+                "The ansatz for Entanglement Forging consists of a set of input bitstrings and a parameterized circuit. (See the [explanatory material](../explanation/index.rst) section of the documentation for additional background on the method.) For this demo, we will use the same bitstrings and ansatz for both the U and V subsystems. "
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 4,
+            "execution_count": 3,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<pre style=\"word-wrap: normal;white-space: pre;background: #fff0;line-height: 1.1;font-family: &quot;Courier New&quot;,Courier,monospace\">     \u250c\u2500\u2500\u2500\u2510\u250c\u2500\u2500\u2500\u2510     \u250c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2510     \u250c\u2500\u2500\u2500\u2510\n",
                             "q_0: \u2524 H \u251c\u2524 X \u251c\u2500\u2500\u25a0\u2500\u2500\u2524 Ry(-1.0*\u03b8) \u251c\u2500\u2500\u25a0\u2500\u2500\u2524 H \u251c\n",
@@ -173,15 +117,15 @@
                             "     \u250c\u2500\u2500\u2500\u2510\u250c\u2500\u2500\u2500\u2510     \u250c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2510     \u250c\u2500\u2500\u2500\u2510\n",
                             "q_0: \u2524 H \u251c\u2524 X \u251c\u2500\u2500\u25a0\u2500\u2500\u2524 Ry(-1.0*\u03b8) \u251c\u2500\u2500\u25a0\u2500\u2500\u2524 H \u251c\n",
                             "     \u2514\u2500\u2500\u2500\u2518\u2514\u2500\u252c\u2500\u2518\u250c\u2500\u2534\u2500\u2510\u251c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2524\u250c\u2500\u2534\u2500\u2510\u2514\u2500\u2500\u2500\u2518\n",
                             "q_1: \u2500\u2500\u2500\u2500\u2500\u2500\u2500\u25a0\u2500\u2500\u2524 X \u251c\u2524 Ry(-1.0*\u03b8) \u251c\u2524 X \u251c\u2500\u2500\u2500\u2500\u2500\n",
                             "               \u2514\u2500\u2500\u2500\u2518\u2514\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518\u2514\u2500\u2500\u2500\u2518     "
                         ]
                     },
-                    "execution_count": 4,
+                    "execution_count": 3,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "theta = Parameter(\"\u03b8\")\n",
                 "\n",
@@ -195,15 +139,15 @@
                 "hop_gate.h(0)\n",
                 "\n",
                 "hop_gate.draw()"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 5,
+            "execution_count": 4,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<pre style=\"word-wrap: normal;white-space: pre;background: #fff0;line-height: 1.1;font-family: &quot;Courier New&quot;,Courier,monospace\">     \u250c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2510                \u250c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2510\n",
                             "q_0: \u25240              \u251c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u25240              \u251c\n",
@@ -227,15 +171,15 @@
                             "     \u250c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2510\u2502  Hop gate(0) \u2502\u251c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2524\n",
                             "q_3: \u25240              \u251c\u2524              \u251c\u25240              \u251c\n",
                             "     \u2502  Hop gate(\u03b82) \u2502\u2502              \u2502\u2502  Hop gate(\u03b84) \u2502\n",
                             "q_4: \u25241              \u251c\u25241             \u251c\u25241              \u251c\n",
                             "     \u2514\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518\u2514\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518\u2514\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518"
                         ]
                     },
-                    "execution_count": 5,
+                    "execution_count": 4,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "theta_1, theta_2, theta_3, theta_4 = (\n",
                 "    Parameter(\"\u03b81\"),\n",
@@ -261,26 +205,26 @@
                 "ansatz.circuit_u.draw()"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "From here, the problem can be solved following the same steps as in the [tutorials](../../tutorials/entanglement_forging/index.rst)."
+                "From here, the problem can be solved following the same steps as in the [tutorials](../tutorials/index.rst)."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 10,
+            "execution_count": 5,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
-                            "<h3>Version Information</h3><table><tr><th>Qiskit Software</th><th>Version</th></tr><tr><td><code>qiskit-terra</code></td><td>0.22.0</td></tr><tr><td><code>qiskit-aer</code></td><td>0.11.0</td></tr><tr><td><code>qiskit-ignis</code></td><td>0.7.1</td></tr><tr><td><code>qiskit-ibmq-provider</code></td><td>0.19.2</td></tr><tr><td><code>qiskit-nature</code></td><td>0.4.5</td></tr><tr><th>System information</th></tr><tr><td>Python version</td><td>3.9.7</td></tr><tr><td>Python compiler</td><td>GCC 7.5.0</td></tr><tr><td>Python build</td><td>default, Sep 16 2021 13:09:58</td></tr><tr><td>OS</td><td>Linux</td></tr><tr><td>CPUs</td><td>6</td></tr><tr><td>Memory (Gb)</td><td>30.943462371826172</td></tr><tr><td colspan='2'>Wed Oct 26 13:40:28 2022 EDT</td></tr></table>"
+                            "<h3>Version Information</h3><table><tr><th>Qiskit Software</th><th>Version</th></tr><tr><td><code>qiskit-terra</code></td><td>0.23.3</td></tr><tr><td><code>qiskit-aer</code></td><td>0.12.0</td></tr><tr><td><code>qiskit-ibmq-provider</code></td><td>0.20.2</td></tr><tr><td><code>qiskit-nature</code></td><td>0.5.2</td></tr><tr><th>System information</th></tr><tr><td>Python version</td><td>3.8.16</td></tr><tr><td>Python compiler</td><td>Clang 14.0.6 </td></tr><tr><td>Python build</td><td>default, Mar  1 2023 21:19:10</td></tr><tr><td>OS</td><td>Darwin</td></tr><tr><td>CPUs</td><td>8</td></tr><tr><td>Memory (Gb)</td><td>32.0</td></tr><tr><td colspan='2'>Tue Apr 11 19:14:09 2023 CDT</td></tr></table>"
                         ],
                         "text/plain": [
                             "<IPython.core.display.HTML object>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
@@ -322,15 +266,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.7.13"
+            "version": "3.8.16"
         },
         "vscode": {
             "interpreter": {
                 "hash": "987cdf5eeb33585dc719bb9ff4378c2f5c2124692c306f8bea7b3d839af38946"
             }
         }
     },
```

### Comparing `circuit_knitting_toolbox-0.0.0/docs/how-tos/entanglement_forging/specify-problem.rst` & `circuit-knitting-toolbox-0.1.0/docs/entanglement_forging/how-tos/specify-problem.rst`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.0.0/docs/how-tos/entanglement_forging/use-asymmetric-bitstrings.ipynb` & `circuit-knitting-toolbox-0.1.0/docs/entanglement_forging/how-tos/use-asymmetric-bitstrings.ipynb`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9910755621693121%*

 * *Differences: {"'cells'": "{2: {'source': {insert: [(4, 'from qiskit_nature.second_q.drivers import "*

 * *            "PySCFDriver\\n'), (5, 'from qiskit_nature.second_q.hamiltonians import "*

 * *            "ElectronicEnergy\\n'), (6, 'from qiskit_nature.second_q.problems import "*

 * *            "ElectronicStructureProblem, ElectronicBasis\\n'), (7, 'from "*

 * *            "qiskit_nature.second_q.transformers import ActiveSpaceTransformer\\n'), (12, ')')], "*

 * *            "delete: [21, 20, 15, 14, 13, 12, 11, 10, 9, 8, 7, 6, 5, 4]}}, 4: […]*

```diff
@@ -28,32 +28,23 @@
             },
             "outputs": [],
             "source": [
                 "from matplotlib import pyplot as plt\n",
                 "import numpy as np\n",
                 "\n",
                 "from qiskit.circuit import QuantumCircuit, Parameter\n",
-                "from qiskit.algorithms.optimizers import COBYLA\n",
-                "from qiskit_nature.drivers import Molecule\n",
-                "from qiskit_nature.drivers.second_quantization import PySCFDriver\n",
-                "from qiskit_nature.problems.second_quantization import ElectronicStructureProblem\n",
-                "from qiskit_nature.mappers.second_quantization import JordanWignerMapper\n",
-                "from qiskit_nature.converters.second_quantization import QubitConverter\n",
-                "from qiskit_nature.properties.second_quantization.electronic.bases import (\n",
-                "    ElectronicBasis,\n",
-                ")\n",
-                "from qiskit_nature.transformers.second_quantization.electronic.active_space_transformer import (\n",
-                "    ActiveSpaceTransformer,\n",
-                ")\n",
+                "from qiskit_nature.second_q.drivers import PySCFDriver\n",
+                "from qiskit_nature.second_q.hamiltonians import ElectronicEnergy\n",
+                "from qiskit_nature.second_q.problems import ElectronicStructureProblem, ElectronicBasis\n",
+                "from qiskit_nature.second_q.transformers import ActiveSpaceTransformer\n",
                 "\n",
                 "from circuit_knitting_toolbox.entanglement_forging import (\n",
                 "    EntanglementForgingAnsatz,\n",
                 "    EntanglementForgingGroundStateSolver,\n",
-                ")\n",
-                "from circuit_knitting_toolbox.utils import IntegralDriver"
+                ")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Define the $\\mathrm{CH}_3$ molecule, define the active space transform, and instantiate an `ElectronicStructureProblem`"
@@ -67,106 +58,85 @@
                     "end_time": "2021-04-27T13:41:07.934705Z",
                     "start_time": "2021-04-27T13:41:07.880717Z"
                 }
             },
             "outputs": [],
             "source": [
                 "# Define a molecular system of interest - Methyl radical\n",
-                "molecule = Molecule(\n",
-                "    geometry=[\n",
-                "        [\"C\", [0.0, 0.0, 0.00]],\n",
-                "        [\"H\", [1.0790, 0.0, 0.00]],\n",
-                "        [\"H\", [-0.5395, -0.9344, 0.00]],\n",
-                "        [\"H\", [-0.5395, 0.9344, 0.00]],\n",
-                "    ],\n",
-                "    charge=0,\n",
-                "    multiplicity=2,\n",
+                "driver = PySCFDriver(\n",
+                "    atom=f\"C 0.0 0.0 0.0; H 1.0790 0.0 0.0; H -0.5395 -0.9344 0.0; H -0.5395 0.9344 0.0\",\n",
+                "    spin=1,\n",
                 ")\n",
-                "\n",
-                "driver = PySCFDriver.from_molecule(molecule=molecule, basis=\"sto-3g\")\n",
-                "converter = QubitConverter(JordanWignerMapper())\n",
+                "problem = driver.run()\n",
                 "\n",
                 "# Construct an active space composed of 6 molecular orbitals\n",
-                "transformer = ActiveSpaceTransformer(num_electrons=(3, 2), num_molecular_orbitals=6)\n",
-                "problem_reduced = ElectronicStructureProblem(driver, [transformer])"
+                "transformer = ActiveSpaceTransformer(num_electrons=(3, 2), num_spatial_orbitals=6)\n",
+                "problem_reduced = transformer.transform(problem)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Retrieve the one and two-body integrals and the nuclear repulsion energy. These will be used to decompose the operator into a bipartite system."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 3,
             "metadata": {},
-            "outputs": [
-                {
-                    "name": "stderr",
-                    "output_type": "stream",
-                    "text": [
-                        "/Users/caleb/opt/anaconda3/envs/ckt/lib/python3.7/site-packages/qiskit_nature/problems/second_quantization/electronic/electronic_structure_problem.py:93: ListAuxOpsDeprecationWarning: List-based `aux_operators` are deprecated as of version 0.3.0 and support for them will be removed no sooner than 3 months after the release. Instead, use dict-based `aux_operators`. You can switch to the dict-based interface immediately, by setting `qiskit_nature.settings.dict_aux_operators` to `True`.\n",
-                        "  second_quantized_ops = self._grouped_property_transformed.second_q_ops()\n"
-                    ]
-                }
-            ],
+            "outputs": [],
             "source": [
-                "H_fermionic = problem_reduced.second_q_ops()\n",
-                "electronic_energy_object = problem_reduced.grouped_property_transformed.get_property(\n",
-                "    \"ElectronicEnergy\"\n",
-                ")\n",
-                "nuclear_repulsion_energy = electronic_energy_object.nuclear_repulsion_energy\n",
+                "nuclear_repulsion_energy = problem_reduced.nuclear_repulsion_energy\n",
                 "\n",
                 "# These are the integrals in the molecular orbital basis retrieved from the 6 orbital active space.\n",
-                "one_body_integrals_alpha = electronic_energy_object.get_electronic_integral(\n",
-                "    ElectronicBasis.MO, 1\n",
-                ")._matrices[0]\n",
-                "one_body_integrals_beta = electronic_energy_object.get_electronic_integral(\n",
-                "    ElectronicBasis.MO, 1\n",
-                ")._matrices[1]\n",
-                "\n",
-                "two_body_integrals_alpha_alpha = electronic_energy_object.get_electronic_integral(\n",
-                "    ElectronicBasis.MO, 2\n",
-                ")._matrices[0]\n",
-                "two_body_integrals_beta_alpha = electronic_energy_object.get_electronic_integral(\n",
-                "    ElectronicBasis.MO, 2\n",
-                ")._matrices[1]\n",
-                "two_body_integrals_beta_beta = electronic_energy_object.get_electronic_integral(\n",
-                "    ElectronicBasis.MO, 2\n",
-                ")._matrices[2]\n",
-                "two_body_integrals_alpha_beta = electronic_energy_object.get_electronic_integral(\n",
-                "    ElectronicBasis.MO, 2\n",
-                ")._matrices[3]"
+                "one_body_integrals_alpha = (\n",
+                "    problem_reduced.hamiltonian.electronic_integrals.one_body.alpha[\"+-\"]\n",
+                ")\n",
+                "one_body_integrals_beta = (\n",
+                "    problem_reduced.hamiltonian.electronic_integrals.one_body.beta[\"+-\"]\n",
+                ")\n",
+                "two_body_integrals_alpha_alpha = (\n",
+                "    problem_reduced.hamiltonian.electronic_integrals.two_body.alpha[\"++--\"]\n",
+                ")\n",
+                "two_body_integrals_beta_beta = (\n",
+                "    problem_reduced.hamiltonian.electronic_integrals.two_body.beta[\"++--\"]\n",
+                ")\n",
+                "two_body_integrals_alpha_beta = (\n",
+                "    problem_reduced.hamiltonian.electronic_integrals.two_body.alpha_beta[\"++--\"]\n",
+                ")\n",
+                "two_body_integrals_beta_alpha = (\n",
+                "    problem_reduced.hamiltonian.electronic_integrals.two_body.beta_alpha[\"++--\"]\n",
+                ")\n",
+                "two_body_integrals_beta_beta = (\n",
+                "    problem_reduced.hamiltonian.electronic_integrals.two_body.beta[\"++--\"]\n",
+                ")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "### Use the `IntegralDriver` and `ElectronicStructureProblem` objects to specify the entanglement-forged operator"
+                "### Set up the reduced `ElectronicStructureProblem` "
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 4,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# Create an ElectronicStructureProblem from our IntegralDriver and performing second quantization transformation\n",
-                "driver = IntegralDriver(\n",
-                "    hcore=one_body_integrals_alpha,\n",
-                "    mo_coeff=np.eye(6, 6),\n",
-                "    eri=two_body_integrals_alpha_alpha,\n",
-                "    num_alpha=3,\n",
-                "    num_beta=2,\n",
-                "    nuclear_repulsion_energy=nuclear_repulsion_energy,\n",
+                "hamiltonian = ElectronicEnergy.from_raw_integrals(\n",
+                "    one_body_integrals_alpha, two_body_integrals_alpha_alpha\n",
                 ")\n",
-                "problem = ElectronicStructureProblem(driver)"
+                "hamiltonian.nuclear_repulsion_energy = nuclear_repulsion_energy\n",
+                "problem = ElectronicStructureProblem(hamiltonian)\n",
+                "problem.num_particles = (3, 2)\n",
+                "problem.basis = ElectronicBasis.MO"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Prepare the bitstrings and the ansatz. \n",
@@ -284,26 +254,26 @@
                 "ansatz.circuit_u.draw(\"text\", justify=\"right\", fold=-1)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "From here, the problem can be solved following the same steps as in the [tutorials](../../tutorials/entanglement_forging/index.rst)."
+                "From here, the problem can be solved following the same steps as in the [tutorials](../tutorials/index.rst)."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 11,
+            "execution_count": 6,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
-                            "<h3>Version Information</h3><table><tr><th>Qiskit Software</th><th>Version</th></tr><tr><td><code>qiskit-terra</code></td><td>0.22.0</td></tr><tr><td><code>qiskit-aer</code></td><td>0.11.0</td></tr><tr><td><code>qiskit-ignis</code></td><td>0.7.1</td></tr><tr><td><code>qiskit-ibmq-provider</code></td><td>0.19.2</td></tr><tr><td><code>qiskit-nature</code></td><td>0.4.5</td></tr><tr><th>System information</th></tr><tr><td>Python version</td><td>3.9.7</td></tr><tr><td>Python compiler</td><td>GCC 7.5.0</td></tr><tr><td>Python build</td><td>default, Sep 16 2021 13:09:58</td></tr><tr><td>OS</td><td>Linux</td></tr><tr><td>CPUs</td><td>6</td></tr><tr><td>Memory (Gb)</td><td>30.943462371826172</td></tr><tr><td colspan='2'>Wed Oct 26 13:39:30 2022 EDT</td></tr></table>"
+                            "<h3>Version Information</h3><table><tr><th>Qiskit Software</th><th>Version</th></tr><tr><td><code>qiskit-terra</code></td><td>0.23.3</td></tr><tr><td><code>qiskit-aer</code></td><td>0.12.0</td></tr><tr><td><code>qiskit-ibmq-provider</code></td><td>0.20.2</td></tr><tr><td><code>qiskit-nature</code></td><td>0.5.2</td></tr><tr><th>System information</th></tr><tr><td>Python version</td><td>3.8.16</td></tr><tr><td>Python compiler</td><td>Clang 14.0.6 </td></tr><tr><td>Python build</td><td>default, Mar  1 2023 21:19:10</td></tr><tr><td>OS</td><td>Darwin</td></tr><tr><td>CPUs</td><td>8</td></tr><tr><td>Memory (Gb)</td><td>32.0</td></tr><tr><td colspan='2'>Fri Apr 14 14:14:57 2023 CDT</td></tr></table>"
                         ],
                         "text/plain": [
                             "<IPython.core.display.HTML object>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
@@ -345,15 +315,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.7"
+            "version": "3.8.16"
         },
         "nbsphinx": {
             "execute": "never"
         },
         "vscode": {
             "interpreter": {
                 "hash": "987cdf5eeb33585dc719bb9ff4378c2f5c2124692c306f8bea7b3d839af38946"
```

### Comparing `circuit_knitting_toolbox-0.0.0/docs/index.rst` & `circuit-knitting-toolbox-0.1.0/docs/index.rst`

 * *Files 19% similar despite different names*

```diff
@@ -4,34 +4,38 @@
 
 Circuit Knitting is the process of decomposing a quantum circuit into smaller circuits, executing those smaller circuits on a quantum processor(s), and then knitting their results into a reconstruction of the original circuit's outcome. Circuit knitting includes techniques such as entanglement forging, circuit cutting, and classical embedding. The Circuit Knitting Toolbox (CKT) is a collection of such tools.
 
 Each tool in the CKT partitions a user's problem into quantum and classical components to enable efficient use of resources constrained by scaling limits, i.e. size of quantum processors and classical compute capability. It is designed to work seamlessly with the `Quantum Serverless <https://qiskit-extensions.github.io/quantum-serverless/>`_ framework, which enables users to run parallelized and hybrid (quantum + classical) workloads without worrying about allocating and managing underlying infrastructure.
 
 The toolbox currently contains the following tools:
 
-- Entanglement Forging
 - Circuit Cutting
+- Entanglement Forging
 
 The source code to the toolbox is available `on GitHub <https://github.com/Qiskit-Extensions/circuit-knitting-toolbox>`_.
 
 .. note::
 
-   The `Quantum Serverless <https://qiskit-extensions.github.io/quantum-serverless/>`_ framework is documented separately, as it lives in its own repository.  Check out `Tutorial 2: Forging with Quantum Serverless <./tutorials/entanglement_forging/tutorial_2_forging_with_quantum_serverless.ipynb>`_  and `Tutorial 3: Circuit Cutting with Quantum Serverless <./tutorials/circuit_cutting/tutorial_3_cutting_with_quantum_serverless.ipynb>`_ for examples on how to integrate Quantum Serverless into circuit knitting workflows.
+   The `Quantum Serverless <https://qiskit-extensions.github.io/quantum-serverless/>`_ framework is documented separately, as it lives in its own repository.  Check out `Tutorial 2: Forging with Quantum Serverless <./entanglement_forging/tutorials/tutorial_2_forging_with_quantum_serverless.ipynb>`_  and `Tutorial 3: Circuit Cutting with Quantum Serverless <./circuit_cutting/tutorials/tutorial_3_cutting_with_quantum_serverless.ipynb>`_ for examples on how to integrate Quantum Serverless into circuit knitting workflows.
 
-This project is meant to evolve rapidly and, as such, does not follow `Qiskit's deprecation policy <https://qiskit.org/documentation/contributing_to_qiskit.html#deprecation-policy>`_.  We may occasionally make breaking changes in order to improve the user experience.  When possible, we will keep old interfaces and mark them as deprecated, as long as they can co-exist with the new ones.  Each substantial improvement, breaking change, or deprecation will be documented in the release notes.
+This project is meant to evolve rapidly and, as such, does not follow `Qiskit's deprecation policy <https://qiskit.org/documentation/contributing_to_qiskit.html#deprecation-policy>`_.  We may occasionally make breaking changes in order to improve the user experience.  When possible, we will keep old interfaces and mark them as deprecated, as long as they can co-exist with the new ones.  Each substantial improvement, breaking change, or deprecation will be documented in the :ref:`release notes`.
 
 Contents
 --------
 
 .. toctree::
-  :maxdepth: 3
+  :maxdepth: 2
 
   Installation Instructions <install>
-  Tutorials <tutorials/index>
-  Explanatory Material <explanation/index>
-  How-To Guides <how-tos/index>
+  Circuit Cutting Tutorials <circuit_cutting/tutorials/index>
+  Circuit Cutting Explanatory Material <circuit_cutting/explanation/index>
+  Circuit Cutting How-To Guides <circuit_cutting/how-tos/index>
+  Entanglement Forging Tutorials <entanglement_forging/tutorials/index>
+  Entanglement Forging Explanatory Material <entanglement_forging/explanation/index>
+  Entanglement Forging How-To Guides <entanglement_forging/how-tos/index>
   API References <apidocs/index>
+  Release Notes <release-notes>
 
 .. Hiding - Indices and tables
    :ref:`genindex`
    :ref:`modindex`
    :ref:`search`
```

### Comparing `circuit_knitting_toolbox-0.0.0/docs/tutorials/circuit_cutting/README.rst` & `circuit-knitting-toolbox-0.1.0/docs/circuit_cutting/tutorials/README.rst`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.0.0/docs/tutorials/circuit_cutting/tutorial_1_automatic_cut_finding.ipynb` & `circuit-knitting-toolbox-0.1.0/docs/circuit_cutting/tutorials/tutorial_1_automatic_cut_finding.ipynb`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.0.0/docs/tutorials/circuit_cutting/tutorial_2_manual_cutting.ipynb` & `circuit-knitting-toolbox-0.1.0/docs/circuit_cutting/tutorials/tutorial_2_manual_cutting.ipynb`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.0.0/docs/tutorials/circuit_cutting/tutorial_3_cutting_with_quantum_serverless.ipynb` & `circuit-knitting-toolbox-0.1.0/docs/circuit_cutting/tutorials/tutorial_3_cutting_with_quantum_serverless.ipynb`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9965514894635291%*

 * *Differences: {"'cells'": "{2: {'outputs': {0: {'data': {'image/png': "*

 * *            "'iVBORw0KGgoAAAANSUhEUgAAAyUAAAGOCAYAAACJ0KybAAAAOXRFWHRTb2Z0d2FyZQBNYXRwbG90bGliIHZlcnNpb24zLjcuMSwgaHR0cHM6Ly9tYXRwbG90bGliLm9yZy/bCgiHAAAACXBIWXMAAA9hAAAPYQGoP6dpAAB6FElEQVR4nO3dd3wUdf7H8dfupkKAECDUhCIt9EAUUYEY8FCxAAqKopzneYjlxEOQU7Gc5+9ExFNPRdCzoWBBFOSQLooQCCVID6GHXgNJSN3d3x8DwUAq7Ga2vJ+PRx6S2dnvfLJ+vzPz2W8Zi9PpdCIiIiIiImISq9kBiIiIiIiIf1NSIiIiIiIiplJSIiIiIiIiplJSIiIiIiIiplJSIiIiIiIiplJSIiIiIiIiplJSIiIiIiIiplJSIiIiIiIiplJSIiIiIiIiplJS […]*

```diff
@@ -36,25 +36,27 @@
             "cell_type": "code",
             "execution_count": 1,
             "id": "eb859bde",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
-                        "image/png": "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iHg3JSUVEBCsccPiO1SfxZeoPouIeDcN3xIREREREVMpKREREREREVMpKREREREREVMpKREREREREVMpKREREREREVMpKREREREREVMpKREREREREVMpKREREREREVMpKREREREREVMpKREREREREVMpKREREREREVMpKREREREREVMFmB2ANynIhcxj5hw7rDYEBJtzbBFPoTYo3szM+uuL1CZFfIuSkgrIPAarp5lz7LjBEN7QnGOLeAq1QfFmZtZfX6Q2KeJbNHxLRERERERMpaRERERERERMpeFbIpXM6YQjGbDvODgcxrYFG6FBTYiuBdVCzI1PfFOBHQ6kQ9rv6t3PW6FRhPETrKuBiIiYSJchFxs5MZ4texKx2QKxWm1E12nNAze+QueWvc0OTUxWYIcVO+DXbXDoVNHX/veb8V8LENMAerSG1vUrPUSfoDZY1Kls+GUrrNwBmblFX/tujfHfoACIawI9W0PdGpUeophEbUVEPImGb7nBAze+wg+vZDL9haN0aNaTlz4bQFbOabPDEhPtPQ6v/wjTV12ckPyeE9h8AN5fDJ8shcycSgvRp6gNGj1ySTvhXz/Aos0XJyS/l1cAy7fDa/+D+RvB7qi8OMVcaisi4imUlLhRYEAQN8QN5UxuBvuOppgdjpgkeQ+8Oa/0ZKQ46/bChLlwLMM9cfkDf22DDid8uxqmJkJOfvnfZ3fCnN/gw5+NREX8h7+2FRHxHEpK3Cg3P5u5Sf8l0BZEZM3GZocjJthyAKYsM24SL8XJLHh3EWSox+SS+Gsb/N86Y5jgpdpyAD5bZvS2iH/w17YiIp5DSYkbfDJvLP3GhnPrs1X5MelDnh3yFTXDIhnzQR8271kBQH5BHo++dSVH0/eZHK24S1au8U11aQnJq4OMn9KczILpSbpBrAh/boOph43hWqUpT73buM8Y0iW+zZ/bioh4Fq9JSvLy8hg7dixRUVGEhoaSkJBAUlISFouFmTNnmh1eEX/s8zLfv5zOV88fomWjODbtXgbA4/3f5f1ZT2J32Pl6yWv06nwvdcIbmRytuMv/1pXdwxFgNX7K8luaMdfEbDn5sHa38S38xn3G5H1P5K9t0OGAr1aWvV95693Mtb49r8nhMHqFft0Gq3YaXyT4G39tKyLiebxi9S2n08nAgQNJSkrixRdfpHnz5kydOpX+/fsDEBsb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IiLiXjpXi4iYS3NKKiCstpGFm3VsEREpns7P4ivMrMveTm3RuykpqYCAYHULioh4Ip2fxVeoLou/0vAtERERERExlZISERERERExlZISERERERExlZISERERERExlZISERERERExlZISERERERExlZISERERERExlZISERERERExlZISERERERExlZISERERERExlZISERERERExlZISERERERExVYDZAXiTglzIPGbOscNqQ0CwOccWERHvouuViLnUBitOSUkFZB6D1dPMOXbcYAhvaM6xRUTEu+h6JWIutcGK0/AtERERERExlZISERERERExlZISERE/kW+HvcfB6TR+dh6B3HyzoxLxPDn5sOPw+baSdhwK7GZHJeLbNKdERMSH2R2wcR8sS4Xth8HhPP/a2wvAAjSKgGtaQOcmEKyrgvipnHxYvQsSt8P+k0VfmzAXbFZoXheuawFtGhq/i4jr6PLjYiMnxrNlTyI2WyBWq43oOq154MZX6Nyyt9mhiYifSTsBUxPhYHrJ+zjP7vfVSpi7Hu7qatxwie/T9eq8DWnwdRJk5JS8j90BKQeNn6gIuKcb1A+vtBDFB6kNFqU83w0euPEVfnglk+kvHKVDs5689NkAsnJOmx2WiPiRFTvg33NLT0gudCobJi+BH5KNISvi+/z9euVwwozV8N9fSk9ILpR2Al6fA2t2uS828Q/+3gZ/T0mJGwUGBHFD3FDO5Gaw72iK2eGIiJ9I2glfrig6VKsiFm2GOb+5NibxbP56vfp+DfxyiX+u3QlTlsO6Pa6NSfyTv7bB31NS4ka5+dnMTfovgbYgIms2NjscEfEDR04bw1BK8+og46c0CzbB1oOui0s8mz9er9anlZ2QlKetTF0BxzNdF5f4J39sgxfymqQkLy+PsWPHEhUVRWhoKAkJCSQlJWGxWJg5c6bZ4RXxybyx9Bsbzq3PVuXHpA95dshX1AyLZMwHfdi8ZwUA+QV5PPrWlRxN32dytCLiK5xOo4ekrFWCAqzGT1m+XAF5Ba6JzVOdzobdx+DQKf8csuav16ucfPimjOQdytdW8grKV5a3O5ZhtBUlYK7lr22wOF6RlDidTgYOHMiHH37Ic889x+zZs2natCn9+/cHIDY21uQIi/pjn5f5/uV0vnr+EC0bxbFp9zIAHu//Lu/PehK7w87XS16jV+d7qRPe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\n",
+                        "image/png": "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iHg3JSUVEBCsccPiO1SfxZeoPouIeDcN3xIREREREVMpKREREREREVMpKREREREREVMpKREREREREVMpKREREREREVMpKREREREREVMpKREREREREVMpKREREREREVMpKREREREREVMpKREREREREVMpKREREREREVMpKREREREREVMFmB2ANynIhcxj5hw7rDYEBJtzbBFPoTYo3szM+uuL1CZFfIuSkgrIPAarp5lz7LjBEN7QnGOLeAq1QfFmZtZfX6Q2KeJbNHxLRERERERMpaRERERERERMpeFbIpXM6YQjGbDvODgcxrYFG6FBTYiuBdVCzI1PfFOBHQ6kQ9rv6t3PW6FRhPETrKuBiIiYSJchFxs5MZ4texKx2QKxWm1E12nNAze+QueWvc0OTUxWYIcVO+DXbXDoVNHX/veb8V8LENMAerSG1vUrPUSfoDZY1Kls+GUrrNwBmblFX/tujfHfoACIawI9W0PdGpUeophEbUVEPImGb7nBAze+wg+vZDL9haN0aNaTlz4bQFbOabPDEhPtPQ6v/wjTV12ckPyeE9h8AN5fDJ8shcycSgvRp6gNGj1ySTvhXz/Aos0XJyS/l1cAy7fDa/+D+RvB7qi8OMVcaisi4imUlLhRYEAQN8QN5UxuBvuOppgdjpgkeQ+8Oa/0ZKQ46/bChLlwLMM9cfkDf22DDid8uxqmJkJOfvnfZ3fCnN/gw5+NREX8h7+2FRHxHEpK3Cg3P5u5Sf8l0BZEZM3GZocjJthyAKYsM24SL8XJLHh3EWSox+SS+Gsb/N86Y5jgpdpyAD5bZvS2iH/w17YiIp5DSYkbfDJvLP3GhnPrs1X5MelDnh3yFTXDIhnzQR8271kBQH5BHo++dSVH0/eZHK24S1au8U11aQnJq4OMn9KczILpSbpBrAh/boOph43hWqUpT73buM8Y0iW+zZ/bioh4Fq9JSvLy8hg7dixRUVGEhoaSkJBAUlISFouFmTNnmh1eEX/s8zLfv5zOV88fomWjODbtXgbA4/3f5f1ZT2J32Pl6yWv06nwvdcIbmRytuMv/1pXdwxFgNX7K8luaMdfEbDn5sHa38S38xn3G5H1P5K9t0OGAr1aWvV95693Mtb49r8nhMHqFft0Gq3YaXyT4G39tKyLiebxi9S2n08nAgQNJSkrixRdfpHnz5kydOpX+/fsDEBsb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IiLiXjpXi4iYS3NKKiCstpGFm3VsEREpns7P4ivMrMveTm3RuykpqYCAYHULioh4Ip2fxVeoLou/0vAtERERERExlZISERERERExlZISERERERExlZISERERERExlZISERERERExlZISERERERExlZISERERERExlZISERERERExlZISERERERExlZISERERERExlZISERERERExlZISERERERExVYDZAXiTglzIPGbOscNqQ0CwOccWERHvouuViLnUBitOSUkFZB6D1dPMOXbcYAhvaM6xRUTEu+h6JWIutcGK0/AtERERERExlZISERERERExlZISERE/kW+HvcfB6TR+dh6B3HyzoxLxPDn5sOPw+baSdhwK7GZHJeLbNKdERMSH2R2wcR8sS4Xth8HhPP/a2wvAAjSKgGtaQOcmEKyrgvipnHxYvQsSt8P+k0VfmzAXbFZoXheuawFtGhq/i4jr6PLjYiMnxrNlTyI2WyBWq43oOq154MZX6Nyyt9mhiYifSTsBUxPhYHrJ+zjP7vfVSpi7Hu7qatxwie/T9eq8DWnwdRJk5JS8j90BKQeNn6gIuKcb1A+vtBDFB6kNFqU83w0euPEVfnglk+kvHKVDs5689NkAsnJOmx2WiPiRFTvg33NLT0gudCobJi+BH5KNISvi+/z9euVwwozV8N9fSk9ILpR2Al6fA2t2uS828Q/+3gZ/T0mJGwUGBHFD3FDO5Gaw72iK2eGIiJ9I2glfrig6VKsiFm2GOb+5NibxbP56vfp+DfxyiX+u3QlTlsO6Pa6NSfyTv7bB31NS4ka5+dnMTfovgbYgIms2NjscEfEDR04bw1BK8+og46c0CzbB1oOui0s8mz9er9anlZ2QlKetTF0BxzNdF5f4J39sgxfymqQkLy+PsWPHEhUVRWhoKAkJCSQlJWGxWJg5c6bZ4RXxybyx9Bsbzq3PVuXHpA95dshX1AyLZMwHfdi8ZwUA+QV5PPrWlRxN32dytCLiK5xOo4ekrFWCAqzGT1m+XAF5Ba6JzVOdzobdx+DQKf8csuav16ucfPimjOQdytdW8grKV5a3O5ZhtBUlYK7lr22wOF6RlDidTgYOHMiHH37Ic889x+zZs2natCn9+/cHIDY21uQIi/pjn5f5/uV0vnr+EC0bxbFp9zIAHu//Lu/PehK7w87XS16jV+d7qRPe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",
                         "text/plain": [
                             "<Figure size 1020.64x491.633 with 1 Axes>"
                         ]
                     },
                     "execution_count": 1,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
+                "from __future__ import annotations\n",
+                "\n",
                 "import numpy as np\n",
                 "from qiskit.circuit.library import EfficientSU2\n",
                 "\n",
                 "num_qubits = 8\n",
                 "circuit = EfficientSU2(\n",
                 "    num_qubits=num_qubits,\n",
                 "    reps=2,\n",
@@ -72,15 +74,15 @@
         {
             "cell_type": "markdown",
             "id": "c6382121",
             "metadata": {},
             "source": [
                 "## Set up Quantum Serverless\n",
                 "\n",
-                "We can use Quantum Serverless to allocate the steps of wire cutting to various compute resources. For this tutorial, we will use our local CPU cores as our cluster. See the [Quantum Serverless](https://github.com/Qiskit-Extensions/quantum-serverless) documentation (and below) for more informatin about how to use other clusters."
+                "We can use Quantum Serverless to allocate the steps of wire cutting to various compute resources. For this tutorial, we will use our local CPU cores as our cluster. See the [Quantum Serverless](https://github.com/Qiskit-Extensions/quantum-serverless) documentation (and below) for more information about how to use other clusters."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 2,
             "id": "175b4f9e",
             "metadata": {},
@@ -118,32 +120,31 @@
         {
             "cell_type": "code",
             "execution_count": 3,
             "id": "8c11457a",
             "metadata": {},
             "outputs": [],
             "source": [
-                "from typing import Optional, Sequence, Any, Dict\n",
-                "from nptyping import NDArray\n",
+                "from typing import Sequence, Any\n",
                 "from qiskit import QuantumCircuit\n",
                 "from circuit_knitting_toolbox.circuit_cutting.wire_cutting import cut_circuit_wires\n",
-                "from quantum_serverless import run_qiskit_remote, get\n",
+                "from quantum_serverless import distribute_task, get\n",
                 "\n",
                 "# Create a wrapper function to be sent to remote cluster\n",
-                "@run_qiskit_remote()\n",
+                "@distribute_task()\n",
                 "def cut_circuit_wires_remote(\n",
                 "    circuit: QuantumCircuit,\n",
                 "    method: str,\n",
-                "    subcircuit_vertices: Optional[Sequence[Sequence[int]]] = None,\n",
-                "    max_subcircuit_width: Optional[int] = None,\n",
-                "    max_subcircuit_cuts: Optional[int] = None,\n",
-                "    max_subcircuit_size: Optional[int] = None,\n",
-                "    max_cuts: Optional[int] = None,\n",
-                "    num_subcircuits: Optional[Sequence[int]] = None,\n",
-                ") -> Dict[str, Any]:\n",
+                "    subcircuit_vertices: Sequence[Sequence[int]] | None = None,\n",
+                "    max_subcircuit_width: int | None = None,\n",
+                "    max_subcircuit_cuts: int | None = None,\n",
+                "    max_subcircuit_size: int | None = None,\n",
+                "    max_cuts: int | None = None,\n",
+                "    num_subcircuits: Sequence[int] | None = None,\n",
+                ") -> dict[str, Any]:\n",
                 "    return cut_circuit_wires(\n",
                 "        circuit=circuit,\n",
                 "        method=method,\n",
                 "        subcircuit_vertices=subcircuit_vertices,\n",
                 "        max_subcircuit_width=max_subcircuit_width,\n",
                 "        max_subcircuit_cuts=max_subcircuit_cuts,\n",
                 "        max_subcircuit_size=max_subcircuit_size,\n",
@@ -172,62 +173,54 @@
             "id": "ecad9a4a",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "\u001b[2m\u001b[36m(cut_circuit_wires_remote pid=85257)\u001b[0m Exporting as a LP file to let you check the model that will be solved :  inf <class 'float'>\n",
-                        "\u001b[2m\u001b[36m(cut_circuit_wires_remote pid=85257)\u001b[0m Version identifier: 22.1.0.0 | 2022-03-27 | 54982fbec\n",
-                        "\u001b[2m\u001b[36m(cut_circuit_wires_remote pid=85257)\u001b[0m CPXPARAM_Read_DataCheck                          1\n",
-                        "\u001b[2m\u001b[36m(cut_circuit_wires_remote pid=85257)\u001b[0m CPXPARAM_TimeLimit                               300\n",
-                        "\u001b[2m\u001b[36m(cut_circuit_wires_remote pid=85257)\u001b[0m Warning:  Non-integral bounds for integer variables rounded.\n",
-                        "\u001b[2m\u001b[36m(cut_circuit_wires_remote pid=85257)\u001b[0m Tried aggregator 3 times.\n",
-                        "\u001b[2m\u001b[36m(cut_circuit_wires_remote pid=85257)\u001b[0m MIP Presolve eliminated 37 rows and 8 columns.\n",
-                        "\u001b[2m\u001b[36m(cut_circuit_wires_remote pid=85257)\u001b[0m MIP Presolve modified 7 coefficients.\n",
-                        "\u001b[2m\u001b[36m(cut_circuit_wires_remote pid=85257)\u001b[0m Aggregator did 103 substitutions.\n",
-                        "\u001b[2m\u001b[36m(cut_circuit_wires_remote pid=85257)\u001b[0m Reduced MIP has 366 rows, 127 columns, and 1072 nonzeros.\n",
-                        "\u001b[2m\u001b[36m(cut_circuit_wires_remote pid=85257)\u001b[0m Reduced MIP has 121 binaries, 6 generals, 0 SOSs, and 0 indicators.\n",
-                        "\u001b[2m\u001b[36m(cut_circuit_wires_remote pid=85257)\u001b[0m Presolve time = 0.00 sec. (2.10 ticks)\n",
-                        "\u001b[2m\u001b[36m(cut_circuit_wires_remote pid=85257)\u001b[0m Found incumbent of value 2.000000 after 0.01 sec. (3.52 ticks)\n",
-                        "\u001b[2m\u001b[36m(cut_circuit_wires_remote pid=85257)\u001b[0m Probing fixed 18 vars, tightened 0 bounds.\n",
-                        "\u001b[2m\u001b[36m(cut_circuit_wires_remote pid=85257)\u001b[0m Probing changed sense of 36 constraints.\n",
-                        "\u001b[2m\u001b[36m(cut_circuit_wires_remote pid=85257)\u001b[0m Probing time = 0.00 sec. (1.05 ticks)\n",
-                        "\u001b[2m\u001b[36m(cut_circuit_wires_remote pid=85257)\u001b[0m Cover probing fixed 4 vars, tightened 14 bounds.\n",
-                        "\u001b[2m\u001b[36m(cut_circuit_wires_remote pid=85257)\u001b[0m Tried aggregator 2 times.\n",
-                        "\u001b[2m\u001b[36m(cut_circuit_wires_remote pid=85257)\u001b[0m MIP Presolve eliminated 347 rows and 108 columns.\n",
-                        "\u001b[2m\u001b[36m(cut_circuit_wires_remote pid=85257)\u001b[0m MIP Presolve modified 102 coefficients.\n",
-                        "\u001b[2m\u001b[36m(cut_circuit_wires_remote pid=85257)\u001b[0m Aggregator did 19 substitutions.\n",
-                        "\u001b[2m\u001b[36m(cut_circuit_wires_remote pid=85257)\u001b[0m All rows and columns eliminated.\n",
-                        "\u001b[2m\u001b[36m(cut_circuit_wires_remote pid=85257)\u001b[0m Presolve time = 0.00 sec. (0.90 ticks)\n",
-                        "\u001b[2m\u001b[36m(cut_circuit_wires_remote pid=85257)\u001b[0m \n",
-                        "\u001b[2m\u001b[36m(cut_circuit_wires_remote pid=85257)\u001b[0m Root node processing (before b&c):\n",
-                        "\u001b[2m\u001b[36m(cut_circuit_wires_remote pid=85257)\u001b[0m   Real time             =    0.01 sec. (5.60 ticks)\n",
-                        "\u001b[2m\u001b[36m(cut_circuit_wires_remote pid=85257)\u001b[0m Parallel b&c, 16 threads:\n",
-                        "\u001b[2m\u001b[36m(cut_circuit_wires_remote pid=85257)\u001b[0m   Real time             =    0.00 sec. (0.00 ticks)\n",
-                        "\u001b[2m\u001b[36m(cut_circuit_wires_remote pid=85257)\u001b[0m   Sync time (average)   =    0.00 sec.\n",
-                        "\u001b[2m\u001b[36m(cut_circuit_wires_remote pid=85257)\u001b[0m   Wait time (average)   =    0.00 sec.\n",
-                        "\u001b[2m\u001b[36m(cut_circuit_wires_remote pid=85257)\u001b[0m                           ------------\n",
-                        "\u001b[2m\u001b[36m(cut_circuit_wires_remote pid=85257)\u001b[0m Total (root+branch&cut) =    0.01 sec. (5.60 ticks)\n",
-                        "\u001b[2m\u001b[36m(cut_circuit_wires_remote pid=85257)\u001b[0m --------------------\n",
-                        "\u001b[2m\u001b[36m(cut_circuit_wires_remote pid=85257)\u001b[0m subcircuit 0\n",
-                        "\u001b[2m\u001b[36m(cut_circuit_wires_remote pid=85257)\u001b[0m \u03c1 qubits = 0, O qubits = 2, width = 5, effective = 3, depth = 8, size = 19\n"
-                    ]
-                },
-                {
-                    "name": "stderr",
-                    "output_type": "stream",
-                    "text": [
-                        "/Users/caleb/opt/anaconda3/envs/ckt/lib/python3.9/site-packages/ray/_private/worker.py:976: UserWarning: len(ctx) is deprecated. Use len(ctx.address_info) instead.\n",
-                        "  warnings.warn(\"len(ctx) is deprecated. Use len(ctx.address_info) instead.\")\n"
+                        "\u001b[2m\u001b[36m(cut_circuit_wires_remote pid=47814)\u001b[0m Exporting as a LP file to let you check the model that will be solved :  inf <class 'float'>\n",
+                        "\u001b[2m\u001b[36m(cut_circuit_wires_remote pid=47814)\u001b[0m Version identifier: 22.1.1.0 | 2023-02-11 | 22d6266e5\n",
+                        "\u001b[2m\u001b[36m(cut_circuit_wires_remote pid=47814)\u001b[0m CPXPARAM_Read_DataCheck                          1\n",
+                        "\u001b[2m\u001b[36m(cut_circuit_wires_remote pid=47814)\u001b[0m CPXPARAM_TimeLimit                               300\n",
+                        "\u001b[2m\u001b[36m(cut_circuit_wires_remote pid=47814)\u001b[0m Warning:  Non-integral bounds for integer variables rounded.\n",
+                        "\u001b[2m\u001b[36m(cut_circuit_wires_remote pid=47814)\u001b[0m Tried aggregator 3 times.\n",
+                        "\u001b[2m\u001b[36m(cut_circuit_wires_remote pid=47814)\u001b[0m MIP Presolve eliminated 37 rows and 8 columns.\n",
+                        "\u001b[2m\u001b[36m(cut_circuit_wires_remote pid=47814)\u001b[0m MIP Presolve modified 7 coefficients.\n",
+                        "\u001b[2m\u001b[36m(cut_circuit_wires_remote pid=47814)\u001b[0m Aggregator did 103 substitutions.\n",
+                        "\u001b[2m\u001b[36m(cut_circuit_wires_remote pid=47814)\u001b[0m Reduced MIP has 366 rows, 127 columns, and 1072 nonzeros.\n",
+                        "\u001b[2m\u001b[36m(cut_circuit_wires_remote pid=47814)\u001b[0m Reduced MIP has 121 binaries, 6 generals, 0 SOSs, and 0 indicators.\n",
+                        "\u001b[2m\u001b[36m(cut_circuit_wires_remote pid=47814)\u001b[0m Presolve time = 0.00 sec. (2.10 ticks)\n",
+                        "\u001b[2m\u001b[36m(cut_circuit_wires_remote pid=47814)\u001b[0m Found incumbent of value 2.000000 after 0.01 sec. (3.52 ticks)\n",
+                        "\u001b[2m\u001b[36m(cut_circuit_wires_remote pid=47814)\u001b[0m Probing fixed 18 vars, tightened 0 bounds.\n",
+                        "\u001b[2m\u001b[36m(cut_circuit_wires_remote pid=47814)\u001b[0m Probing changed sense of 36 constraints.\n",
+                        "\u001b[2m\u001b[36m(cut_circuit_wires_remote pid=47814)\u001b[0m Probing time = 0.00 sec. (1.05 ticks)\n",
+                        "\u001b[2m\u001b[36m(cut_circuit_wires_remote pid=47814)\u001b[0m Cover probing fixed 4 vars, tightened 14 bounds.\n",
+                        "\u001b[2m\u001b[36m(cut_circuit_wires_remote pid=47814)\u001b[0m Tried aggregator 2 times.\n",
+                        "\u001b[2m\u001b[36m(cut_circuit_wires_remote pid=47814)\u001b[0m MIP Presolve eliminated 347 rows and 108 columns.\n",
+                        "\u001b[2m\u001b[36m(cut_circuit_wires_remote pid=47814)\u001b[0m MIP Presolve modified 102 coefficients.\n",
+                        "\u001b[2m\u001b[36m(cut_circuit_wires_remote pid=47814)\u001b[0m Aggregator did 19 substitutions.\n",
+                        "\u001b[2m\u001b[36m(cut_circuit_wires_remote pid=47814)\u001b[0m All rows and columns eliminated.\n",
+                        "\u001b[2m\u001b[36m(cut_circuit_wires_remote pid=47814)\u001b[0m Presolve time = 0.00 sec. (0.90 ticks)\n",
+                        "\u001b[2m\u001b[36m(cut_circuit_wires_remote pid=47814)\u001b[0m \n",
+                        "\u001b[2m\u001b[36m(cut_circuit_wires_remote pid=47814)\u001b[0m Root node processing (before b&c):\n",
+                        "\u001b[2m\u001b[36m(cut_circuit_wires_remote pid=47814)\u001b[0m   Real time             =    0.01 sec. (5.60 ticks)\n",
+                        "\u001b[2m\u001b[36m(cut_circuit_wires_remote pid=47814)\u001b[0m Parallel b&c, 12 threads:\n",
+                        "\u001b[2m\u001b[36m(cut_circuit_wires_remote pid=47814)\u001b[0m   Real time             =    0.00 sec. (0.00 ticks)\n",
+                        "\u001b[2m\u001b[36m(cut_circuit_wires_remote pid=47814)\u001b[0m   Sync time (average)   =    0.00 sec.\n",
+                        "\u001b[2m\u001b[36m(cut_circuit_wires_remote pid=47814)\u001b[0m   Wait time (average)   =    0.00 sec.\n",
+                        "\u001b[2m\u001b[36m(cut_circuit_wires_remote pid=47814)\u001b[0m                           ------------\n",
+                        "\u001b[2m\u001b[36m(cut_circuit_wires_remote pid=47814)\u001b[0m Total (root+branch&cut) =    0.01 sec. (5.60 ticks)\n",
+                        "\u001b[2m\u001b[36m(cut_circuit_wires_remote pid=47814)\u001b[0m --------------------\n",
+                        "\u001b[2m\u001b[36m(cut_circuit_wires_remote pid=47814)\u001b[0m subcircuit 0\n",
+                        "\u001b[2m\u001b[36m(cut_circuit_wires_remote pid=47814)\u001b[0m \u03c1 qubits = 0, O qubits = 2, width = 5, effective = 3, depth = 8, size = 19\n"
                     ]
                 }
             ],
             "source": [
-                "with serverless:\n",
+                "with serverless.context():\n",
                 "    cuts_future = cut_circuit_wires_remote(\n",
                 "        circuit=circuit,\n",
                 "        method=\"automatic\",\n",
                 "        max_subcircuit_width=5,\n",
                 "        max_cuts=2,\n",
                 "        num_subcircuits=[2],\n",
                 "    )\n",
@@ -246,15 +239,15 @@
             "cell_type": "code",
             "execution_count": 5,
             "id": "13dc6132",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
-                        "image/png": "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\n",
+                        "image/png": "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",
                         "text/plain": [
                             "<Figure size 523.664x270.9 with 1 Axes>"
                         ]
                     },
                     "execution_count": 5,
                     "metadata": {},
                     "output_type": "execute_result"
@@ -269,15 +262,15 @@
             "cell_type": "code",
             "execution_count": 6,
             "id": "c5eebeaa",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
-                        "image/png": "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\n",
+                        "image/png": "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",
                         "text/plain": [
                             "<Figure size 623.998x270.9 with 1 Axes>"
                         ]
                     },
                     "execution_count": 6,
                     "metadata": {},
                     "output_type": "execute_result"
@@ -307,21 +300,21 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "from qiskit_ibm_runtime import Options\n",
                 "from circuit_knitting_toolbox.circuit_cutting.wire_cutting import evaluate_subcircuits\n",
                 "\n",
                 "# Create a wrapper function to be sent to remote cluster\n",
-                "@run_qiskit_remote()\n",
+                "@distribute_task()\n",
                 "def evaluate_subcircuits_remote(\n",
-                "    cuts: Dict[str, Any],\n",
-                "    service_args: Optional[Dict[str, Any]] = None,\n",
-                "    backend_names: Optional[Sequence[str]] = None,\n",
-                "    options_dict: Optional[Dict] = None,\n",
-                ") -> Dict[int, Dict[int, NDArray]]:\n",
+                "    cuts: dict[str, Any],\n",
+                "    service_args: dict[str, Any] | None = None,\n",
+                "    backend_names: Sequence[str] | None = None,\n",
+                "    options_dict: dict | None = None,\n",
+                ") -> dict[int, dict[int, np.ndarray]]:\n",
                 "    service = None if service_args is None else QiskitRuntimeService(**service_args)\n",
                 "    options = None if options_dict is None else Options(**options_dict)\n",
                 "\n",
                 "    return evaluate_subcircuits(\n",
                 "        cuts, service=service, backend_names=backend_names, options=options\n",
                 "    )"
             ]
@@ -399,15 +392,15 @@
             "execution_count": 10,
             "id": "2ae5160c",
             "metadata": {},
             "outputs": [],
             "source": [
                 "from dataclasses import asdict\n",
                 "\n",
-                "with serverless:\n",
+                "with serverless.context():\n",
                 "    # QiskitRuntimeService is not serializable, so we must convert it to a dictionary before passing to remote function\n",
                 "    service_args = None if service is None else service.active_account()\n",
                 "\n",
                 "    # The Options class is not serializable, so we must convert it to a dictionary before passing to remote function\n",
                 "    options_dict = asdict(options)\n",
                 "\n",
                 "    subcircuit_probabilities_future = evaluate_subcircuits_remote(\n",
@@ -441,21 +434,21 @@
             "outputs": [],
             "source": [
                 "from circuit_knitting_toolbox.circuit_cutting.wire_cutting import (\n",
                 "    reconstruct_full_distribution,\n",
                 ")\n",
                 "\n",
                 "\n",
-                "@run_qiskit_remote()\n",
+                "@distribute_task()\n",
                 "def reconstruct_full_distribution_remote(\n",
                 "    circuit: QuantumCircuit,\n",
-                "    subcircuit_instance_probabilities: Dict[int, Dict[int, NDArray]],\n",
-                "    cuts: Dict[str, Any],\n",
+                "    subcircuit_instance_probabilities: dict[int, dict[int, np.ndarray]],\n",
+                "    cuts: dict[str, Any],\n",
                 "    num_threads: int = 1,\n",
-                ") -> NDArray:\n",
+                ") -> np.ndarray:\n",
                 "    return reconstruct_full_distribution(\n",
                 "        circuit, subcircuit_instance_probabilities, cuts\n",
                 "    )"
             ]
         },
         {
             "cell_type": "markdown",
@@ -474,15 +467,15 @@
             "execution_count": 12,
             "id": "5aceecc0",
             "metadata": {},
             "outputs": [],
             "source": [
                 "%%capture\n",
                 "\n",
-                "with serverless:\n",
+                "with serverless.context():\n",
                 "    reconstructed_probabilities_future = reconstruct_full_distribution_remote(\n",
                 "        circuit, subcircuit_instance_probabilities, cuts\n",
                 "    )\n",
                 "    reconstructed_probabilities = get(reconstructed_probabilities_future)"
             ]
         },
         {
@@ -522,24 +515,24 @@
             "execution_count": 14,
             "id": "673d3cb3",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "{'nearest': {'chi2': 0.014781577189785336,\n",
-                            "  'Mean Squared Error': 3.607494186206942e-07,\n",
-                            "  'Mean Absolute Percentage Error': 78992.90552703604,\n",
-                            "  'Cross Entropy': 3.6842346725058057,\n",
-                            "  'HOP': 0.9934651038602943},\n",
-                            " 'naive': {'chi2': 0.014293570101341663,\n",
-                            "  'Mean Squared Error': 3.7810267377915685e-07,\n",
-                            "  'Mean Absolute Percentage Error': 80793.04233599117,\n",
-                            "  'Cross Entropy': 3.6693264359537037,\n",
-                            "  'HOP': 0.9915340741625416}}"
+                            "{'nearest': {'chi2': 0,\n",
+                            "  'Mean Squared Error': 1.5404638469060036e-34,\n",
+                            "  'Mean Absolute Percentage Error': 7.541771945010017e-10,\n",
+                            "  'Cross Entropy': 3.56455111606822,\n",
+                            "  'HOP': 0.9945381353717202},\n",
+                            " 'naive': {'chi2': 0,\n",
+                            "  'Mean Squared Error': 2.6551806564992906e-34,\n",
+                            "  'Mean Absolute Percentage Error': 7.541785864061976e-10,\n",
+                            "  'Cross Entropy': 3.5645511160682206,\n",
+                            "  'HOP': 0.99453813537172}}"
                         ]
                     },
                     "execution_count": 14,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -563,15 +556,15 @@
             "id": "c8cc97e9",
             "metadata": {
                 "scrolled": false
             },
             "outputs": [
                 {
                     "data": {
-                        "image/png": "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+qlbt24aPny4PDw8ZGtrq4kTJyoyMvKfDhf3gYN3AQAAAAAAUCTc3X7k7NmzZu0JCQlm2+3ctXPnTqWlpWncuHEyGAwyGAyKjIxUbGysDAaDtmzZIkl6+eWXdfPmTZ07d06//vqr4uPjdePGjUzb7ERHR+vRRx9V8eLFdfr0aTk6Oppd79Wrl6ZMmaKxY8eqXr16Onz4sNatW2c6jPf8+fNmB+bmRkxMjPr06aMaNWpo8ODB6tOnj7777jvT9eLFi2vTpk1q166datSooWHDhql79+764Ycf8jQPHi4ZGRnq16+fXF1d9c477+i7777TsmXLzPosWbJElSpV0rJly9SnTx8FBASoTZs2pn3976pcubKio6N19erVHOdk657Cw0p+AAAAAAAAFAnOzs5ycnLSmjVrNHHiREl3DsmNiopS27ZtM/UPCAjIVLh88803devWLc2bN0+NGjUyu+br6ytJ2rhxo1JSUvTiiy+arl28eFGPPvqobG1tderUKdOq+78bOHBgltvzSNK2bdtyzC+rA0kHDx6swYMHZ3uPj4+Ptm/fnuO4wN9NmzZNu3fv1qpVq9SpUydt27ZNb7zxhp566im5u7tL+t8e/n89PHfv3r2KiIgwfa9IUvfu3TV79myNHz8+x4N3nZycst0CCwWLIj8AAAAAAACKjKCgIP33v/9VcHCwunbtquHDh8toNGrKlCmS7qwq9vDwUEREhEqWLKlnn33W7P7hw4dLkll7SEiIfH19Va9ePW3YsEEfffSRypYtq1GjRkm6U+CvUaOG0tPTtXLlSkVHRys6OlrSnb31ixcv/k+kDuTajz/+qN9++y1Te7NmzXTr1i29++676tevn+ng54ULF6pevXp68803tXjxYklS586dtWzZMj377LPq1KmTzp49qzlz5qhmzZqmA6slqVWrVurTp4/++9//6vTp02rfvr0yMjK0c+dOtWrVyvSml7+/vzZt2qRp06apbNmyqlixoumQaBQsivwAAAAAAAAoMmbOnKno6GgtWLBAX3zxhZycnDR37lzTPvYJCQl53hbk3Llz+u9//6v09HTZ2tqqadOm+vHHH03XlyxZopSUFEnS008/bXbvzp071bx58/vMCkXF3KGFHUH+GDt2bJbtX3zxhT777DO5u7trxowZpvaqVatq4sSJGjJkiBYvXqyePXuqX79+io2N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V69u0bzZocgPAAAAAAAAAFakUaNGatCggaQ728o0b95cL774ok6ePGk6+PXtt99WQEBAlvdXqVKlwGLLbnX93W1wJGno0KHq0qWLVqxYofXr1+vdd9/VxIkTtWXLFtWvXz9X85QoUSJTW3ar8NPT03M1Zm5lZGSobdu2+ve//53l9WrVquXrfPdCkR8AAAAAAAAArJStra0mTpyoVq1aadasWXrllVck3dlSp02bNjneW7lyZR07dizHPhUqVNDRo0eVkZFhtpr/t99+M123ROXKlTVs2DANGzZMp0+fVr169TR16lR9/fXXknK3bc7flSpVSteuXcvU/vdPG1SuXFkZGRn69ddfVa9evWzHyy6GypUrKzk5+Z7Pb4UKFbR582YlJyebreY/efJkjvflFUV+AAAAAAAAFAnBMwo7gqyNLOwAgHto2bKlGjVqpBkzZmjo0KFq2bKlPvvsMw0aNEje3t5mfa9cuWLaZqZ79+567733tHz58kz78huNRhkMBnXs2FEbNmzQokWLTPvyp6Wl6eOPP5azs7NatGiRp1hv3LghGxsbOTg4mNoqV64sFxcX3bp1y9Tm5OSUZcE+J5UrV1ZiYqKOHj2qOnXqSJJiYmK0fPlys37dunXTiBEj9N5772V58O7d4n52MfTs2VOhoaFav359pk9LXLt2Tc7OzrKzs1PHjh31+eef69NPPzUdvJuenq6PP/44T3ndC0V+AAAAAAAAALByw4cPV48ePbRw4ULNnj1bzZs3V+3atRUcHKxKlSopLi5OERERunjxoo4cOWK6Z8mSJerRo4deeeUV+fv76+rVq1q1apXmzJmjunXr6rXXXtNnn32mfv366cCBA/Lz89OSJUv0008/acaMGXJxcclTnKdOndLTTz+tnj17qmbNmrKzs9Py5csVFxen3r17m/r5+/vr008/1X/+8x9VqVJFHh4eat26dY5j9+7dWyNGjNCzzz6rwYMH68aNG/r0009VrVo1HTx40NSvSpUqGj16tCZMmKAnn3xSzz33nOzt7bVv3z6VLVtWEydOzDGG4cOHa9WqVercubP69esnf39/paSk6JdfftGSJUsUFRUld3d3denSRU888YRGjhypqKgo1axZU8uWLVNiYmKenrN7ocgPAAAAAAAA4KHwIB9U/Nxzz6ly5cqaMmWKgoODtX//fo0fP14LFy5U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N9C6dessv6dkyZI4cuRIhmOnT5/OtOTP84QQmZb0eZZ5c6vHjx+/zK9ARET/Y//LDQPz5cuHDRs2vPDvtLOzw6xZszBr1qyXqpWIiIiIiOhVw+V6iCiTwYMH49y5cwgICMC2bdtQs2ZNCCEsjZaKFStmWFt50qRJuHv3Ljp16oQdO3agRYsWSEpKwpdffgkAuHv3Lnx8fLB48WIcPnwYq1atQuXKlZGeno4xY8YAAJYsWYJevXrh999/x+HDhzF79my0bdsWBoMBgwYNyvt/BCIiIiIiIiIiIhvAO/mJKJPvv/8ed+7cwbJly7B48WI4OTlh0aJFlqUW7t+/D0VRLOcPGzYMYWFhmDdvHrZt2wYHBwdMmzYN3bp1A/B048YbN25g2LBhUFUVOp0ORYsWxfLly9GlSxcAgJubGwIDA7F+/XoIIWAwGFC5cmWsWLECBQoUyPt/BCIiIiIiIiIiIhvAJj8RZemPP/7I9rH4+PhMx+bMmYM5c+Zkeb6bmxvu3LmT49/Xo0cP9OjR46VqJCKif094lWlal5AtriNMRERERET0X1yuh4iIiIiIiIiIiIjIRrHJT0RERERERERERERko7hcDxFlEPCd1hVkb9H7WldARERERERERERkXXgnPxERERERERERERGRjWKTn4iIiIiIiIiIiIjIRrHJT0RERERERERERERko9jkJyIiIiIiIiIiIiKyUWzyExERERERERERERHZKDb5iYiIiIiIiIiIiIhsFJv8REREREREREREREQ2ik1+IiIiIiIiIiIiIiIbxSY/EREREREREREREZGNYpOfiIiIiIiIiIiIiMhGsclPRERERERERERERGSj2OQnIiIiIiIiIiIiIrJRbPITEREREREREREREdkoNvmJiIiIiIiIiIiIiGwUm/xERERERERERERERDaKTX4iIiIiIiIiIiIiIhvFJj8RERERERERERERkY1ik5+IiIiIiIiIiIiIyEaxyU9EREREREREREREZKPY5CciIiIiIiIiIiIislFs8hMRERERERERERER2Sg2+YmIiIiIiIiIiIiIbJTVNvlDQkLQvn17uLm5wcnJCY0bN8batWtf6mcYjUZ89tlnqFSpEvLly4eSJUti6NChuHv3brbfs3r1ajRs2BBOTk4oWLAgOnbsiNOnT//TX4eIiIiIiIiIiIiI6H/O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\n",
+                        "image/png": "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LSMjQ1FRUXdd6udex0xOTlabNm3k6OioVatW5bp3AAAAACAR8gMAAAC4DwYMGKADBw4oNDRUq1evVs2aNWUymTR16lRJUmBgoEXYnZKSosjISEVGRspkMuns2bOKjIy0CMnvNubZs2dVrVo1paWlafny5YqLi9P+/fu1f/9+3bp1K9d6w8LCNG/ePEVEROjw4cN69dVXlZqaqn79+kmSQkJCNHr0aHP/W7duae/evdq7d69u3bqlc+fOae/evTp+/Hiex8wM+FNTU7VgwQIlJycrISFBCQkJSk9Pv8e/AQAAADysCPkBAIWmR48esre3l8FgkJubmxYuXJhr/7CwMDk5OclgMMjZ2VkTJkywOH7w4EFVqlRJRqNRBoNBXl5eWdZV7t27t4oVKyaDwSCDwaBTp07lqdY5c+YoICBAzs7OatCggX799ddc+y9dulTVqlWTs7OzatasqbVr11ocP3/+vPr27avSpUvLxcVFbdu2VUxMjEWfzz77TM2bN5eHh4cMBoOuXLmSp1oBwBbNnDlTL7zwghYuXKhOnTrpzJkzmjdvnmrUqCHpzjI7Fy9eNPffu3evevXqpV69eikjI0O7du1Sr1691K1btzyP+c033yg1NVU3btzQs88+q1q1apm/7vZ9vmfPnpo6darGjRun2rVra+/evVq3bp1549zTp08rPj7e3D8uLk516tRRnTp1FB8fr6lTp6pOnTp65ZVX8jzm7t279csvv+jAgQOqVKmS/Pz8zF9nzpy5x78BAAAAPKwMJpPJVNRFPKySk5Pl6emppKQkeXh4FHU5AHBfDR06VB999JH69eunLl26aOTIkTp69KgOHDigJ554Ikv/Tz/9VIMHD1b79u316quvavLkydq2bZuWL1+url27KiMjQ56enrKzs9NHH30kb29vhYWFKSYmRnFxcfL29pYkde3aVdevX5ckrV+/XrGxsSpfvnyutUZGRiokJERz585VgwYNNGPGDC1dulRHjx41j/tX27dvV9OmTTVp0iR17NhRX331lSZPnqzdu3erRo0aMplMaty4sRwcHDRt2jR5eHho+vTpWrdunX7//Xe5urpKkmbMmKEbN25IkkaPHq0///wzT8tIAAAAALYodEZRV5B3oz4JL+oS8izwaHhRl1CoyNeAuyPkL0R8EwLwKHNzc1PFihW1f/9+SXfWSXZyclLr1q21bt26LP39/f118+ZNiw0J3dzc5O/vr99//13r169X27ZttXLlSnXu3Nk8pqOjo/r06aOIiAiL8WbMmKE333wzTyF/gwYNVK9ePc2ePVvSnTWSy5UrpyFDhmjUqFFZ+vfs2VOpqalavXq1ua1hw4aqXbu25s6dq2PHjqlq1ao6ePCg+Q2NjIwM+fr6auLEiRZ3dUrS5s2b1aJFC0J+AAAAPNQI+QsHIT8AlusBABS4lJQUpaamqkOHDuY2e3t7BQQEaN++fdmeExcXp8aNG1u0BQUF6eTJk+YxJcnd3d1iTDs7O/38889W13rr1i399ttvatWqlbnNzs5OrVq1UnR0dLbnREdHW/SXpODgYHP/mzdvSpLFZol2dnZycnLStm3brK4VAAAAAADg7wj5AQAF7tixY5KkChUqWLSXLFlSV69ezfac9PR0lS1b1qLNz8/PHJi3a9dORqNRL7/8sk6ePKmUlBS1a9dO6enp97SWfWJiotLT083rIWfy8fFRQkJCtuckJCTk2r9atWry9/c3L8Fz69YtTZ48WWfPnrVYvxkAAAAAAOBeEfIDAGyCi4uLFi1apMTERFWsWFHu7u7auXOnSpUqJYPBUNTlWXBwcNDy5ct17NgxlShRQi4uLtq0aZPatWsnOzt+9AIAAAAAgIJD0gAAKHBVqlSRJPNSO5kuXbpksdzOXxmNRp09e9aiLT4+Xk5OTubHvXv31vXr13Xq1Cn9/vvvSkxM1LVr1+Tr62t1rV5eXjIajRZ7AUjS+fPncxzX19f3rv2DgoK0d+9eXblyRfHx8Vq3bp0uXbqkihUrWl0rAAAAAADA39kXdQEAgIePm5ubXF1dtWbNGk2aNEnSnU1yY2Nj1bp162zPKV26tLZv327Rtnv37ixL/kh3NumVpI0bNyo1NVUvvfSS1bU6OjoqKChIUVFR6tKli6Q7m+RGRUXp9ddfz/acRo0aKSoqSsOGDTO3bdy4UY0aNcrS19PTU5IUExOjXbt26b333rO6VgCwJba0uaLEBosAAACwXdzJDwAoFAMGDNCBAwcUGhqq1atXq2bNmjKZTJo6daokKTAw0CIUHzNmjC5cuKBOnTpp7dq1at68uVJSUvT++++b+4SFhWnGjBnavHmz3n77bbVr106lS5fW6NGjzX3279+vyMhI7dmzR5L03XffKTIyUidOnMix1rCwMM2bN08RERE6fPiwXn31VaWmpqpfv36SpJCQEItrDB06VOvWrdO0adN05MgRhYeHa9euXRZvCixdulSbN2/WH3/8oW+//VatW7dWly5d1KZNG3OfhIQE7d27V8ePH5ckHThwQHv37tXly5etes4BAAAAAMCjh5AfAFAoZs6cqRdeeEELFy5Up06ddObMGc2bN081atSQdGfpnosXL5r7Dxo0SG+++abWr1+vDh06aMeOHQoPD1fXrl3NfU6dOqW33npLLVq00AcffKBGjRrp6NGjFtd944031KtXL33xxReSpCFDhqhXr17mTxRkp2fPnpo6darGjRun2rVra+/evVq3bp15c93Tp09bbJjbuHFjffXVV/rss89Uq1YtffPNN1q5cqV5btKdpYb69OmjatWq6Y033lCfPn303//+1+K6c+fOVZ06dRQaGipJatq0qerUqaNVq1bl67kGAMCW9OjRQ/b29jIYDHJzc9PChQtz7R8WFiYnJycZDAY5OztrwoQJFscTEhL05JNPymg0ymAwyMnJKcun/Hr37q1ixYrJYDDIYDDo1KlTea53zpw5CggIkLOzsxo0aKBff/011/5Lly5VtWrV5OzsrJo1a2rt2rUWx1NSUvT666+rbNmyeuyxx1S9enXNnTvXos9nn32m5s2by8PDQwaDQVeuXMlzvQAA4NFjMJlMpqIu4mGVnJwsT09PJSUlycPDo6jLAQAAAO4bluspPLa8XM/QoUP10UcfqV+/furSpYtGjhypo0eP6sCBA3riiSey9P/00081ePBgtW/fXq+++qomT56sbdu2afny5eYbAR5//HEdP35cU6ZMUd26dTV37lx9+eWXevvtt82fCOzatauuX78uSVq/fr1iY2NVvnz5u9YbGRmpkJAQzZ07Vw0aNNCMGTO0dOlSHT16VN7e3ln6b9++XU2bNtWkSZPUsWNHffXVV5o8ebJ2795tvhlg4MCB+vHHHzV//nwFBARow4YNeu2117R8+XI999xzkqQZM2boxo0bkqTRo0frzz//VLFixfL/hAMPGFv62cDPhQcH+Rpwd4T8hYhvQgAAAHhU2VKQIxHm3C9ubm6qWLGi9u/fL+nOnj1OTk5q3bq11q1bl6W/v7+/bt68abHhvZubm/z9/fX7779LkpydnfX0008rKirK3MfFxUVPPfWUtm3bZjHejBkz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IiIiIpJFqckvIiIiIiIiIiIiIpJFqckvIiIiIiIiIiIiIpJFqckvIiIiIiIiIiIiIpJFqckvIiIiIiIiIiIiIpJFZdomf1hYGA899BD+/v7kyZOHRo0asWDBgn/1O5KSknjrrbeoXLkyuXLlokSJEgwcOJDz58/f8WfmzZtHgwYNyJMnDwUKFKBDhw788ssv/+vbERERERERERERERFJc5myyb9x40YaN27Mli1b6NmzJ4MHDyY6OppevXrxySef/KPfYbfb6dy5M2PHjqVw4cI8//zz3H///UyfPp3777+fCxcu3PIz7777Lv369eP8+fMMHjyYHj16EBISQlBQEFu3bk3rtykiIiIiIiIiIiIi8j/xdHcBf5WSksKAAQOwWq2EhIRQp04dAMaMGUODBg0YNWoUDz/8MGXLlr3r75k9ezarV6+md+/ezJs3D4vFAsCUKVMYMmQIo0ePZurUqa71jx49yrhx46hSpQq7du0if/78AAwdOpRGjRoxYMAADhw4gNWaKcdFRERERERERERERCQHynQd6w0bNnDs2DH69OnjavAD5M+fn1GjRnHjxg1mz579t79n2rRpAIwfP97V4AcYNGgQFSpUYN68eSQkJLhenzlzJikpKbz++uuuBj9AnTp16N27N4cOHWLLli1p8A5FRERERERERERERNJGpruSf9OmTQC0bdv2lmUPPvggAJs3b77r70hMTGTnzp1UrVr1liv+LRYLbdq0YerUqezevZumTZv+o3931qxZbN68mWbNmt3x301KSiIpKcn1fVxcHAAxMTEkJycDYLVa8fDwwGazYbfbXes6X09JScEY43rdw8MDq9V6x9edv9fJ09PxkaakpPyj1728vLDb7dhstlT/jTw9Pe/4+s2130j0uuN/j8zmqi3p71fKRC5duuT6+n/9nCB9s6ccpB9nDrLCNiIr5QCyVhacOUivbTmk3TZCOUg/ly5dyjLHETcSM90h5l1ltRxk9PEe/P+2ETcSM931RHeVlXIQExOT4cd78P/bRtxI/B/fbAbLSjmIjY3NFOeE8M+yl5X2DVkpB1euXMkU54Twz7KXlY4Vs1oOMsM5YXpl7+rVqwCp1hGR1DLdXvbo0aMAVK5c+ZZlxYoVw8/Pz7XOnRw7dgy73X7b33Hz7z569KiryX/06FH8/PwoVqzYXde/m/Hjx/Pmm2/e8nr58uXv+nOSMb5xdwH/VuH33V1BtqQciFOWyoJykG6UAwHlQByyVA4KKQfpJUvloIBykF6yVA7yKwfpRTnIfK5evZpq9g0R+VOma/I7r36/0x9tvnz5XOv8L7/j5vWcX99zzz3/eP3bee2113jxxRdd39vtdmJiYihUqFCqKYMk4125coXSpUtz6tQp1+cpOY9yIE7KgoByIA7KgYByIA7KgYByIA7KQebivJq/RIkS7i5FJNPKdE3+rMzHxwcfH59Ur/n7+7unGLmtfPnyaQctyoG4KAsCyoE4KAcCyoE4KAcCyoE4KAeZh67gF7m7TDdRpvOP9k5XzV+5cuVv/7D/ye+4eT3n1/9mfRERERERERERERERd8t0Tf67zX8fHR3NtWvX7jjXvlOFChWwWq13nEP/dvP+V65cmWvXrhEdHf2P1hcRERERERERERERcbdM1+Rv3rw5AGvWrLll2erVq1Otcye5c+emQYMGhIeHExkZmWqZMYa1a9eSJ08eAgMD0/TflczLx8eHsWPH3jKdkuQsyoE4KQsCyoE4KAcCyoE4KAcCyoE4KAciktVYjDHG3UXcLCUlhapVqxIVFcWOHTuoU6cO4Jh6p0GDBpw4cYLw8HDKlSsHwNmzZ4mLi6N48eKpptOZOXMmTz31FL1792bevHmuB99OmTKFIUOGMHDgQKZOnepa/8iRIwQEBFChQgV27drl+l2//vorjRo1okKFChw4cACrNdONi4iIiIiIiIiIiIhIDpXpmvwAGzdu5MEHHyRXrlw88sgj5M2blx9//JHIyEg+/vhjXnrpJde6TzzxBLNnz2bmzJk88cQTrtftdjsPPfQQq1evplGjRjRv3pw//viDRYsWUa5cOXbu3EmRIkVS/bvvvvsuo0ePpmzZsnTv3p2rV68yf/58bty4wfr162ncuHFG/ScQEREREREREREREflbmfKy9JYtW7JlyxYaN27M999/z+TJkylatCjz589P1eC/G6vVyk8//cS4ceO4cOECn376KVu3bqV///5s3779lgY/wOuvv87cuXMpUqQIkydPZsGCBTRt2pRt27apwS8iIiIiIiIiIiIimU6mvJJfRERERERERERERET+Xqa8kl9ERERERERERERERP6emvwiIiIiIiIiIiIiIlmUmvwiIiIiIiIiIiIiIlmUmvwiIiIiIiIiIiJ/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MpUjR44QFxfH/fffT58+fVi7di3bt29n+fLllClThhYtWtC6dWvq1q1LyZIl8ff358CBA0ybNo0WLVrogD2bUA4ElANxUA4ElANxUA4ElAP508SJEzlz5gy//vrrHQd7bp6qKT4+ng8//FCDPSIiki2pyS+ZypEjR0hMTKRt27YMGzaMDh06EB4ezvbt29mwYQM//vgj8+bNo3r16jzwwAMEBwezfv16rly5woABA9xdvqQR5UBAORAH5UBAORAH5UBAORAHDfaIiIikpul6JFNZuHAhPXv2ZP78+fTs2dP1enJyMpGRkezbt4/Q0FA2bdrEoUOH8PLywhiDj48PMTExbqxc0pJyIKAciINyIKAciINyIKAciMPy5cvp2rUro0ePZuzYsURGRqYa7Pnll19ITEy8ZbDn448/ZtmyZbRv397db0FERCRNqckvmYoxhsOHD5MrVy7Kly+f6mFZTvHx8Rw5coTw8HBmzpzJ2rVrGT58OF988YWbqpa0phwIKAfioBwIKAfioBwIKAfioMEeERGR1NTklyzjdgfwzz77LBMnTmTPnj3UrVvXTZVJRlIOBJQDcVAOBJQDcVAOBJSDnESDPSIiIqmpyS9Zjt1ux2q1cuLECTp37szly5c5efKku8uSDKYcCCgH4qAcCCgH4qAcCCgHOZ0Ge0REJCfS02Yky3E+JCkqKork5GSGDh3q5orEHZQDAeVAHJQDAeVAHJQDAeUgp3M2+O12OwAnTpxg8+bNlCpVSg1+ERHJtnQlv2RZxhhOnz5NwYIFyZMnj7vLETdRDgSUA3FQDgSUA3FQDgSUA3HYunUrAwYM4LHHHuPVV191dzkiIiLpQk1+EREREREREcmWNNgjIiI5gZr8IiIiIiIiIiIiIiJZlObkFxERERERERERERHJotTkFxERERERERERERHJotTkFxERERERERERERHJotTkFxERERERERERERHJotTkFxERERERERERERHJotTkFxERERERERERERHJotTkFxERERERERERERHJotTkFxERERERERERERHJov4PWX7hfOxe09gAAAAASUVORK5CYII=",
                         "text/plain": [
                             "<Figure size 1600x600 with 1 Axes>"
                         ]
                     },
                     "execution_count": 15,
                     "metadata": {},
                     "output_type": "execute_result"
@@ -615,15 +608,15 @@
             "execution_count": 16,
             "id": "5e6e41aa",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
-                            "<h3>Version Information</h3><table><tr><th>Qiskit Software</th><th>Version</th></tr><tr><td><code>qiskit-terra</code></td><td>0.22.1</td></tr><tr><td><code>qiskit-aer</code></td><td>0.11.1</td></tr><tr><td><code>qiskit-ibmq-provider</code></td><td>0.19.2</td></tr><tr><td><code>qiskit</code></td><td>0.39.1</td></tr><tr><td><code>qiskit-nature</code></td><td>0.4.5</td></tr><tr><th>System information</th></tr><tr><td>Python version</td><td>3.9.13</td></tr><tr><td>Python compiler</td><td>Clang 12.0.0 </td></tr><tr><td>Python build</td><td>main, Aug 25 2022 18:29:29</td></tr><tr><td>OS</td><td>Darwin</td></tr><tr><td>CPUs</td><td>8</td></tr><tr><td>Memory (Gb)</td><td>32.0</td></tr><tr><td colspan='2'>Thu Nov 03 18:23:57 2022 CDT</td></tr></table>"
+                            "<h3>Version Information</h3><table><tr><th>Qiskit Software</th><th>Version</th></tr><tr><td><code>qiskit-terra</code></td><td>0.23.3</td></tr><tr><td><code>qiskit-aer</code></td><td>0.12.0</td></tr><tr><td><code>qiskit-ibmq-provider</code></td><td>0.20.2</td></tr><tr><td><code>qiskit-nature</code></td><td>0.5.2</td></tr><tr><th>System information</th></tr><tr><td>Python version</td><td>3.9.16</td></tr><tr><td>Python compiler</td><td>GCC 12.2.1 20221121 (Red Hat 12.2.1-4)</td></tr><tr><td>Python build</td><td>main, Dec  7 2022 00:00:00</td></tr><tr><td>OS</td><td>Linux</td></tr><tr><td>CPUs</td><td>6</td></tr><tr><td>Memory (Gb)</td><td>30.821285247802734</td></tr><tr><td colspan='2'>Mon May 01 14:50:37 2023 EDT</td></tr></table>"
                         ],
                         "text/plain": [
                             "<IPython.core.display.HTML object>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
@@ -665,13 +658,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.13"
+            "version": "3.8.16"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `circuit_knitting_toolbox-0.0.0/docs/tutorials/entanglement_forging/data/reactant_2mo.npz` & `circuit-knitting-toolbox-0.1.0/docs/entanglement_forging/tutorials/data/reactant_2mo.npz`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.0.0/docs/tutorials/entanglement_forging/tutorial_1_getting_started.ipynb` & `circuit-knitting-toolbox-0.1.0/docs/entanglement_forging/tutorials/tutorial_1_getting_started.ipynb`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.995422150867923%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(4, 'In the `Circuit Knitting Toolbox`, entanglement forging "*

 * *            'is implemented to estimate the ground state energy of a molecule. Entanglement '*

 * *            'forging is most easily run using the `EntanglementForgingGroundStateSolver` '*

 * *            'interface, which wraps most of the algorithm within a single function call, `solve`. '*

 * *            'Steps 1-4 describe the workflow within `solve`. See the [explanatory '*

 * *            "material](../explanation/inde […]*

```diff
@@ -5,15 +5,15 @@
             "id": "52acc23d",
             "metadata": {},
             "source": [
                 "# Tutorial 1: Entanglement Forging for estimating the ground state energy of the H<sub>2</sub> molecule\n",
                 "\n",
                 "**Entanglement forging** is a method which allows us to represent expectation values of a 2n-qubit wavefunction as sums of multiple expectation values of n-qubit states, embedded in a classical optimization, thus doubling the size of the system that can be exactly simulated with a fixed number of qubits.\n",
                 "\n",
-                "In the `Circuit Knitting Toolbox`, entanglement forging is implemented to estimate the ground state energy of a molecule. Entanglement forging is most easily run using the `EntanglementForgingGroundStateSolver` interface, which wraps most of the algorithm within a single function call, `solve`. Steps 1-4 describe the workflow within `solve`. See the [explanatory material](https://github.com/Qiskit-Extensions/circuit-knitting-toolbox/blob/main/docs/explanation/entanglement_forging/index.rst) for more detailed information:\n",
+                "In the `Circuit Knitting Toolbox`, entanglement forging is implemented to estimate the ground state energy of a molecule. Entanglement forging is most easily run using the `EntanglementForgingGroundStateSolver` interface, which wraps most of the algorithm within a single function call, `solve`. Steps 1-4 describe the workflow within `solve`. See the [explanatory material](../explanation/index.rst) for more detailed information:\n",
                 "\n",
                 "1. **Decompose**:\n",
                 "    * Decompose the 2n-qubit ansatz (wavefunction) into many parameterized, n-qubit ansatze\n",
                 "    * Decompose the 2n-qubit observable (Hamiltonian) into many n-qubit observables\n",
                 "\n",
                 "\n",
                 "2. **Evaluate**:\n",
@@ -30,48 +30,45 @@
         {
             "cell_type": "markdown",
             "id": "faf77d79",
             "metadata": {},
             "source": [
                 "### Instantiate the `ElectronicStructureProblem`\n",
                 "\n",
-                "First, we set up the $\\mathrm{H}_2$ molecule, specify the driver and converter, and instantiate an  `ElectronicStructureProblem`, just like is done in the [Qiskit Nature VQE tutorial](https://github.com/Qiskit/qiskit-nature/blob/stable/0.4/docs/tutorials/03_ground_state_solvers.ipynb)."
+                "First, we set up the $\\mathrm{H}_2$ molecule, specify the driver and converter, and instantiate an  `ElectronicStructureProblem`. We also get the coefficients for translating to MO basis, since entanglement forging needs to transform the inputs.\n",
+                "\n",
+                "If the input `ElectronicStructureProblem` is already defined in the MO basis, the coefficients don't need to be calculated or accounted for."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 1,
             "id": "7d74f57e",
             "metadata": {},
             "outputs": [],
             "source": [
-                "from qiskit_nature.drivers import Molecule\n",
-                "from qiskit_nature.drivers.second_quantization import PySCFDriver\n",
-                "from qiskit_nature.problems.second_quantization import ElectronicStructureProblem\n",
-                "\n",
-                "molecule = Molecule(\n",
-                "    geometry=[\n",
-                "        (\"H\", [0.0, 0.0, 0.0]),\n",
-                "        (\"H\", [0.0, 0.0, 0.735]),\n",
-                "    ],\n",
-                "    charge=0,\n",
-                "    multiplicity=1,\n",
-                ")\n",
-                "driver = PySCFDriver.from_molecule(molecule=molecule, basis=\"sto3g\")\n",
-                "problem = ElectronicStructureProblem(driver)"
+                "from qiskit_nature.second_q.drivers import PySCFDriver\n",
+                "from qiskit_nature.second_q.formats import get_ao_to_mo_from_qcschema\n",
+                "from qiskit_nature.second_q.problems import ElectronicStructureProblem, ElectronicBasis\n",
+                "\n",
+                "driver = PySCFDriver(\"H 0.0 0.0 0.0; H 0.0 0.0 0.735\")\n",
+                "driver.run()\n",
+                "problem = driver.to_problem(basis=ElectronicBasis.AO)\n",
+                "qcschema = driver.to_qcschema()\n",
+                "mo_coeff = get_ao_to_mo_from_qcschema(qcschema).coefficients.alpha[\"+-\"]"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "453dde4f",
             "metadata": {},
             "source": [
                 "### Configure the entanglement forging specific inputs\n",
                 "\n",
-                "The ansatz for Entanglement Forging consists of a set of input bitstrings and a parameterized circuit.  (See the [explanatory material](https://github.com/Qiskit-Extensions/circuit-knitting-toolbox/blob/main/docs/explanation/entanglement_forging/index.rst) section of the documentation for additional background on the method.) For this demo, we will use the same bitstrings and ansatz for both the U and V subsystems, and we will use the [TwoLocal](https://qiskit.org/documentation/stubs/qiskit.circuit.library.TwoLocal.html) circuit from Qiskit."
+                "The ansatz for Entanglement Forging consists of a set of input bitstrings and a parameterized circuit.  (See the [explanatory material](../explanation/index.rst) section of the documentation for additional background on the method.) For this demo, we will use the same bitstrings and ansatz for both the U and V subsystems, and we will use the [TwoLocal](https://qiskit.org/documentation/stubs/qiskit.circuit.library.TwoLocal.html) circuit from Qiskit."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 2,
             "id": "f25814e9",
             "metadata": {},
@@ -150,15 +147,16 @@
                 "Next, we set up the `EntanglementForgingGroundStateSolver`. It is passed the ansatz, a classical optimizer ([COBYLA](https://qiskit.org/documentation/stubs/qiskit.algorithms.optimizers.COBYLA.html?highlight=cobyla#qiskit.algorithms.optimizers.COBYLA), in this case), and an initial point.\n",
                 "\n",
                 " * The `ansatz` field is required.\n",
                 " * If no optimizer is passed, [SPSA](https://qiskit.org/documentation/stubs/qiskit.algorithms.optimizers.SPSA.html) with default settings will be used.\n",
                 " * If a Qiskit Runtime Service is not passed, then a local simulator will be used with the [Qiskit Primitives](https://qiskit.org/documentation/apidoc/primitives.html), and the `backend_names` argument will be ignored.\n",
                 " * If multiple backend names are passed, the expectation value calculations at each iteration will be divided evenly among them and calculated in parallel.\n",
                 " * If a single options argument is passed, it will be used for all backends. If a list of options is passed, they will be synchronized with the backends 1:1\n",
-                " * If the `initial_point` field is not set, it will be initialized to all 0's."
+                " * If the `initial_point` field is not set, it will be initialized to all 0's.\n",
+                " * If `mo_coeff` is not passed, the input problem will be assumed to be in the MO basis"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 4,
             "id": "0cb73a4f",
             "metadata": {},
@@ -175,14 +173,15 @@
                 "solver = EntanglementForgingGroundStateSolver(\n",
                 "    ansatz=ansatz,\n",
                 "    optimizer=optimizer,\n",
                 "    service=service,\n",
                 "    backend_names=backend_names,\n",
                 "    options=options,\n",
                 "    initial_point=[0.0, np.pi / 2],\n",
+                "    mo_coeff=mo_coeff,\n",
                 ")"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "0a2b14a5",
             "metadata": {},
@@ -225,15 +224,15 @@
                     "output_type": "stream",
                     "text": [
                         "Energy:\n"
                     ]
                 },
                 {
                     "data": {
-                        "image/png": "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wzRNs3x1HgAAgNLQ8wIAADyF8AIAADyF8AIAADyF8AIAADyF8AIAADyF8AIAADyF8AIAADyF8AIAADyF8AKgJkyfPl133nlnpYcBoAwILwAKtnr1an3wgx+UJC1btkw33HBD2a7d0dGhtra2Y+5/8skndfXVV5dtHAAqJ1DpAQCAJMViMYVCoaKf397e7uBoAFQzKi8AirZ69Wpt27ZNd911lwzDkGEY2rNnjyTpj3/8oy666CI1NTVpwoQJuuKKK3To0CH7ucuWLdP111+vG264QePGjdOFF14oSbrjjju0YMECNTY2aurUqfrkJz+pvr4+SdLWrVv1sY99TN3d3fb1br75ZknHTht1dXVp1apVampqUktLiz784Q/rwIED9vdvvvlmnX322frOd76j6dOnq7W1VR/5yEfU29trP+YHP/iBFixYoPr6ep1yyilasWKF+vv7XXo1AeSL8AKgaHfddZeWLFmiT3ziE9q/f7/279+vqVOn6ujRo3rPe96jxYsX66mnntJDDz2kAwcO6MMf/vCQ52/cuFGhUEi//e1vde+990qSfD6fvva1r+m5557Txo0b9eijj+rv/u7vJElLly7VnXfeqZaWFvt6n/vc544ZVyqV0qpVq3TkyBFt27ZNjzzyiF555RVddtllQx63a9cu/ehHP9JPf/pT/fSnP9W2bdt06623SpL279+vj370o7rqqqu0Y8cObd26VZdccok4yxaoPKaNABSttbVVoVBIDQ0Nmjhxon3/v/3bv2nx4sX68pe/bN/3zW9+U1OnTtWLL76oOXPmSJJOP/103X777UN+Zm7/zPTp0/XP//zPuuaaa/Tv//7vCoVCam1tlWEYQ6433ObNm/Xss89q9+7dmjp1qiTp29/+ts4880w9+eSTOvfccyWlQ05HR4eam5slSVdccYU2b96s9evXa//+/UokErrkkks0bdo0SdKCBQtKeLUAOIXKCwDH/eEPf9CWLVvU1NRk3+bNmycpXe2wnHPOOcc895e//KWWL1+uU089Vc3Nzbriiit0+PBhRSKRvK+/Y8cOTZ061Q4ukjR//ny1tbVpx44d9n3Tp0+3g4skTZo0SQcPHpQkLVq0SMuXL9eCBQt06aWX6j/+4z/05ptv5v8iAHAN4QWA4/r6+vSBD3xAnZ2dQ24vvfSSzj//fPtxjY2NQ563Z88evf/979fChQv1wx/+UNu3b9c999wjKd3Q67RgMDjka8MwlEqlJEl+v1+PPPKIfv7zn2v+/Pm6++67NXfuXO3evdvxcQAoDOEFQElCoZCSyeSQ+97ylrfoueee0/Tp0zV79uwht+GBJdf27duVSqX01a9+VW9/+9s1Z84c7du377jXG+6MM87Q3r17tXfvXvu+559/XkePHtX8+fPz/rMZhqF3vOMduuWWW/T0008rFApp06ZNeT8fgDsILwBKMn36dD3xxBPas2ePDh06pFQqpeuuu05HjhzRRz/6UT355JPatWuXHn74YX3sYx8bM3jMnj1b8Xhcd999t1555RV95zvfsRt5c6/X19enzZs369ChQyNOJ61YsUILFizQ5Zdfrt///vf63e9+p7/6q7/Su971Lr31rW/N68/1xBNP6Mtf/rKeeuopdXV16YEHHtAbb7yhM844o7AXCIDjCC8ASvK5z31Ofr9f8+fPV3t7u7q6ujR58mT99re/VTKZ1AUXXKAFCxbohhtuUFtbm3y+0f/aWbRoke644w7ddtttOuuss/Td735XGzZsGPKYpUuX6pprrtFll12m9vb2Yxp+pXTF5MEHH9RJJ52k888/XytWrNDMmTN1//335/3namlp0a9+9Su9973v1Zw5c/SP//iP+upXv6qLLroo/xcHgCsMk3V/AADAQ6i8AAAATyG8AAAATyG8AAAATyG8AAAATyG8AAAATyG8AAAATyG8AAAATyG8AAAATyG8AAAATyG8AAAATyG8AAAAT/m/mCzqSLipGX4AAAAASUVORK5CYII=\n",
+                        "image/png": "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AAAQ1s6dO9XS0jLkNZYJEnHqiOM4euuttzR+/HhZllXVn93T06P29nZt2rRJzc3NVf3ZKMaz3nt41nsPz3rv4VnvPdV61sYY7dy5U5MnT1YiMXRXy6irvCQSCU2ZMqWmv6O5uZn/Z9hLeNZ7D8967+FZ7z08672nGs96uIqLi4ZdAABQVwgvAACgrhBeQshkMvqnf/onZTKZkb6VUY9nvffwrPcenvXew7Pee0biWY+6hl0AADC6UXkBAAB1hfACAADqCuEFAADUFcILAACoK4SXEG6//XZNnTpVY8aM0UknnaSnnnpqpG+pri1dulQnnniixo8frwMPPFCf/OQntWHDhqJr9uzZo6uuukoHHHCAxo0bp0996lPasmXLCN3x6HHzzTfLsiwtWrTIe41nXT1vvvmm/u7v/k4HHHCAGhsbNWvWLD399NPe940xuuGGG3TQQQepsbFR8+bN0yuvvDKCd1y/bNvWN7/5TR122GFqbGzU4Ycfrm9/+9tF83F43tH89re/1cc//nFNnjxZlmXpgQceKPp+kOe6fft2LViwQM3NzWptbdXnP/959fb2xr85g0Duvfdek06nzZ133mleeOEF84UvfMG0traaLVu2jPSt1a2zzjrL3HXXXeb55583nZ2d5pxzzjGHHHKI6e3t9a654oorTHt7u1mxYoV5+umnzYc+9CEzZ86cEbzr+vfUU0+ZqVOnmmOPPdZ8+ctf9l7nWVfH9u3bzaGHHmoWLlxo1qxZY15//XXzyCOPmFdffdW75uabbzYtLS3mgQceMM8++6z5xCc+YQ477DCze/fuEbzz+rRkyRJzwAEHmIcffths3LjR3HfffWbcuHHm1ltv9a7heUfzv//7v+Yb3/iGuf/++40ks3z58qLvB3mu8+fPN8cdd5x58sknzeOPP26mT59uLrrootj3RngJ6IMf/KC56qqrvK9t2zaTJ082S5cuHcG7Gl22bt1qJJnVq1cbY4zZsWOHaWhoMPfdd593zfr1640k84c//GGkbrOu7dy50xxxxBHm0UcfNaeffroXXnjW1fMP//AP5tRTT634fcdxzKRJk8z3vvc977UdO3aYTCZj/uu//mtv3OKocu6555rLLrus6LULLrjALFiwwBjD866W0vAS5Lm++OKLRpJZu3atd82vfvUrY1mWefPNN2PdD8tGAfT392vdunWaN2+e91oikdC8efP0hz/8YQTvbHTp7u6WJO2///6SpHXr1mlgYKDouc+YMUOHHHIIzz2iq666Sueee27RM5V41tX00EMP6YQTTtCFF16oAw88ULNnz9aPfvQj7/sbN27U22+/XfSsW1padNJJJ/GsI5gzZ45WrFihl19+WZL07LPP6oknntDZZ58tieddK0Ge6x/+8Ae1trbqhBNO8K6ZN2+eEomE1qxZE+v3j7rBjLWwbds22batiRMnFr0+ceJEvfTSSyN0V6OL4zhatGiRTjnlFB1zzDGSpLffflvpdFqtra1F106cOFFvv/32CNxlfbv33nv1xz/+UWvXrh30PZ519bz++uv693//d33lK1/R17/+da1du1Zf+tKXlE6ndckll3jPs9x/T3jW4S1evFg9PT2aMWOGksmkbNvWkiVLtGDBAknieddIkOf69ttv68ADDyz6fiqV0v777x/72RNesE+46qqr9Pzzz+uJJ54Y6VsZlTZt2qQvf/nLevTRRzVmzJiRvp1RzXEcnXDCCbrpppskSbNnz9bzzz+vO+64Q5dccskI393o89///d+655579J//+Z963/vep87OTi1atEiTJ0/meY9iLBsFMGHCBCWTyUE7L7Zs2aJJkyaN0F2NHldffbUefvhhrVy5UlOmTPFenzRpkvr7+7Vjx46i63nu4a1bt05bt27VBz7wAaVSKaVSKa1evVo//OEPlUqlNHHiRJ51lRx00EGaOXNm0WtHH320urq6JMl7nvz3pDquu+46LV68WJ/97Gc1a9YsXXzxxbrmmmu0dOlSSTzvWgnyXCdNmqStW7cWfT+bzWr79u2xnz3hJYB0Oq3jjz9eK1as8F5zHEcrVqzQySefPIJ3Vt+MMbr66qu1fPlyPfbYYzrssMOKvn/88ceroaGh6Llv2LBBXV1dPPeQzjjjDP3pT39SZ2en93HCCSdowYIF3p951tVxyimnDNry//LLL+vQQw+VJB122GGaNGlS0bPu6enRmjVreNYR7Nq1S4lE8T9lyWRSjuNI4nnXSpDnevLJJ2vHjh1at26dd81jjz0mx3F00kknxbuBWO2+7yH33nuvyWQypqOjw7z44ovm8ssvN62trebtt98e6VurW1deeaVpaWkxq1atMps3b/Y+du3a5V1zxRVXmEMOOcQ89thj5umnnzYnn3yyOfnkk0fwrkcP/24jY3jW1fLUU0+ZVCpllixZYl555RVzzz33mKamJvPTn/7Uu+bmm282ra2t5sEHHzTPPfecOe+889i6G9Ell1xiDj74YG+r9P33328mTJhgvva1r3nX8Lyj2blzp3nmmWfMM888YySZW265xTzzzDPmz3/+szEm2HOdP3++mT17tlmzZo154oknzBFHHMFW6b3ttttuM4cccohJp9Pmgx/8oHnyySdH+pbqmqSyH3fddZd3ze7du80Xv/hFs99++5mmpiZz/vnnm82bN4/cTY8ipeGFZ109v/jFL8wxxxxjMpmMmTFjhvmP//iPou87jmO++c1vmokTJ5pMJmPOOOMMs2HDhhG62/rW09NjvvzlL5tDDjnEjBkzxkybNs184xvfMH19fd41PO9oVq5cWfa/0ZdccokxJthzfeedd8xFF11kxo0bZ5qbm82ll15qdu7cGfveLGN8xxACAADs4+h5AQAAdYXwAgAA6grhBQAA1BXCCwAAqCuEFwAAUFcILwAAoK4QXgAAQF0hvAAAgLpCeAEwKkydOlU/+MEPRvo2AOwFhBcAoS1cuFCf/OQnJUlz587VokWL9trv7ujoUGtr66DX165dq8svv3yv3QeAkZMa6RsAAEnq7+9XOp2O/P62trYq3g2AfRmVFwCRLVy4UKtXr9att94qy7JkWZbeeOMNSdLzzz+vs88+W+PGjdPEiRN18cUXa9u2bd57586dq6uvvlqLFi3ShAkTdNZZZ0mSbrnlFs2aNUtjx45Ve3u7vvjFL6q3t1eStGrVKl166aXq7u72ft+3vvUtSYOXjbq6unTeeedp3Lhxam5u1qc//Wlt2bLF+/63vvUtvf/979dPfvITTZ06VS0tLfrsZz+rnTt3etf8z//8j2bNmqXGxkYdcMABmjdvnt59990aPU0AQRFeAER266236uSTT9YXvvAFbd68WZs3b1Z7e7t27Nihj370o5o9e7aefvpp/frXv9aWLVv06U9/uuj9y5YtUzqd1u9+9zvdcccdkqREIqEf/vCHeuGFF7Rs2TI99thj+trXviZJmjNnjn7wgx+oubnZ+31f/epXB92X4zg677zztH37dq1evVqPPvqoXn/9dX3mM58puu61117TAw88oIcfflgPP/ywVq9erZtvvlmStHnzZl100UW67LLLtH79eq1atUoXXHCBmGULjDyWjQBE1tLSonQ6raamJk2aNMl7/V//9V81e/Zs3XTTTd5rd955p9rb2/Xyyy/ryCOPlCQdccQR+u53v1v0M/39M1OnTtU///M/64orrtC//du/KZ1Oq6WlRZZlFf2+UitWrNCf/vQnbdy4Ue3t7ZKku+++W+973/u0du1anXjiiZJyIaejo0Pjx4+XJF188cVasWKFlixZos2bNyubzeqCCy7QoYceKkmaNWtWjKcFoFqovACoumeffVYrV67UuHHjvI8ZM2ZIylU7XMcff/yg9/7mN7/RGWecoYMPPljjx4/XxRdfrHfeeUe7du0K/PvXr1+v9vZ2L7hI0syZM9Xa2qr169d7r02dOtULLpJ00EEHaevWrZKk4447TmeccYZmzZqlCy+8UD/60Y/0t7/9LfhDAFAzhBcAVdfb26uPf/zj6uzsLPp45ZVXdNppp3nXjR07tuh9b7zxhj72sY/p2GOP1c9//nOtW7dOt99+u6RcQ2+1NTQ0FH1tWZYcx5EkJZNJPfroo/rVr36lmTNn6rbbbtNRRx2ljRs3Vv0+AIRDeAEQSzqdlm3bRa994AMf0AsvvKCpU6dq+vTpRR+lgcVv3bp1chxH3//+9/WhD31IRx55pN56661hf1+po48+Wps2bdKmTZu811588UXt2LFDM2fODPx3syxLp5xyim688UY988wzSqfTWr58eeD3A6gNwguAWKZOnao1a9bojTfe0LZt2+Q4jq666ipt375dF110kdauXavXXntNjzzyiC699NIhg8f06dM1MDCg2267Ta+//rp+8pOfeI28/t/X29urFStWaNu2bWWXk+bNm6dZs2ZpwYIF+uMf/6innnpKn/vc53T66afrhBNOCPT3WrNmjW666SY9/fTT6urq0v3336+//vWvOvroo8M9IABVR3gBEMtXv/pVJZNJzZw5U21tberq6tLkyZP1u9/9TrZt68wzz9SsWbO0aNEitba2KpGo/J+d4447Trfccou+853v6JhjjtE999yjpUuXFl0zZ84cXXHFFfrMZz6jtra2QQ2/Uq5i8uCDD2q//fbTaaedpnnz5mnatGn62c9+Fvjv1dzcrN/+9rc655xzdOSRR+of//Ef9f3vf19nn3128IcDoCYsw74/AABQR6i8AACAukJ4AQAAdYXwAgAA6grhBQAA1BXCCwAAqCuEFwAAUFcILwAAoK4QXgAAQF0hvAAAgLpCeAEAAHWF8AIAAOrK/w8s3VAWlU6OFgAAAABJRU5ErkJggg==",
                         "text/plain": [
                             "<Figure size 640x480 with 1 Axes>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 },
@@ -242,15 +241,15 @@
                     "output_type": "stream",
                     "text": [
                         "Schmidt Coefficients:\n"
                     ]
                 },
                 {
                     "data": {
-                        "image/png": "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AABgO8ZxAQAAcYfgAgAAHIPgAgAAHIPgAgAAHIPgAgAAHIPgAgAAHIPgAgAAHCNuggsD0AEAEP8YgA4AANiOAegAAEDcIbgAAADHILgAAADHILgAAADHILgAAADHILgAAADHILgAAADHILgAAADHILgAAADHiJvgwpD/AADEP4b8BwAAtmPIfwAAEHcILgAAwDEILgAAwDEILgAAwDEILgAAwDEILgAAwDEILgAAwDEILgAAwDEILgAAwDEILgAAwDHiJrgwVxEAAPGPuYoAAIDtmKsIAADEHYILAABwDIILAABwDIILAABwDIILAABwDIILAABwDIILAABwDIILAABwDIILAABwDIILAABwDIILAABwDIILAABwDIILAABwDIILAABwjLgJLl6vV4WFhSouLra7KAAAIEJclmVZdhcinOrr65Wdna26ujplZWXZXRwAABCCUD+/46bGBQAAxD+CCwAAcAyCCwAAcAyCCwAAcAyCCwAAcAyCCwAAcAyCCwAAcAyCCwAAcAyCCwAAcAyCCwAAcAyCCwAAcAyCCwAAcAyCCwAAcAyCCwAAcAyCCwAAcAyCCwAAcAyCCwAAcIy4CS5er1eFhYUqLi62uygAACBCXJZlWXYXIpzq6+uVnZ2turo6ZWVl2V0cAAAQglA/v+OmxgUAAMQ/ggsAAHAMggsAAHAMggsAAHAMggsAAHAMggsAAHAMggsAAHAMggsAAHAMggsAAHAMggsAAHAMggsAAHAMggsAAHAMggsAAHAMggsAAHAMggsAAHAMggsAAHAMggsAAHAMggsAAHAMggsAAHAMggsAAHAMggsAAHAMggsAAHAMggsAAHAMggsAAHAMggsAAHAMggsAAHCMuAkuXq9XhYWFKi4utrsoAAAgQlyWZVl2FyKc6uvrlZ2drbq6OmVlZdldHAAAEIJQP7/jpsYFAADEP4ILAABwDIILAABwDIILAABwDIILAABwDIILAABwDIILAABwDIILAABwDIILAABwDIILAABwDIILAABwDIILAABwDIILAABwDIILAABwDIILAABwDIILAABwDIILAABwDIILAABwDIILAABwDIILAABwDIILAABwDIILAABwDIILAABwDIILAABwDIILAABwDIILAABwDIILAABwDIILAABwDIILAABwDIILAABwDIILAABwDIILAABw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nyjnzUDHpT8lJSWSFPfnjMfj0fTp0zVv3jytXbtWRUVFevjhhxPyXCG4DMLj8WjevHmqrKwMbvP7/aqsrFRpaamNJYs9jY2NOnjwoMaPH293UWLG1KlTNW7cuB7nT319vV5//XXOn3589NFHOnnyZNyfQ5Zl6Y477tDTTz+tl19+WVOnTu3x+Lx585SSktLjvNm3b58OHToU1+fNYMelP1VVVZIU9+dMb36/X62trYl5rtjdOtgJfv3rX1upqanWxo0brb1791q33nqrlZOTY9XU1NhdNFt961vfsrZs2WJVV1dbr776qlVWVmbl5uZax44ds7toUdXQ0GC9+eab1ptvvmlJstatW2e9+eab1t/+9jfLsizrgQcesHJycqxnnnnGeuutt6zrrrvOmjp1qnXmzBmbSx55Zzs2DQ0N1l133WVt377dqq6utl566SXr0ksvtS644AKrpaXF7qJH1Ne//nUrOzvb2rJli3X06NHgrbm5Ofic2267zZo0aZL18ssvW7t27bJKS0ut0tJSG0sdeYMdlwMHDlj/9m//Zu3atcuqrq62nnnmGWvatGnWlVdeaXPJI2vNmjXW1q1brerqauutt96y1qxZY7lcLuuFF16wLCvxzhWCS4geeeQRa9KkSZbH47EWLFhgvfbaa3YXyXbLly+3xo8fb3k8HmvChAnW8uXLrQMHDthdrKh75ZVXLEl9bitWrLAsy3SJ/td//VcrLy/PSk1NtRYvXmzt27fP3kJHydmOTXNzs3XNNddYY8aMsVJSUqzJkydbq1atSogvBP0dE0nWz3/+8+Bzzpw5Y91+++3WqFGjrPT0dOuGG26wjh49al+ho2Cw43Lo0CHryiuvtEaPHm2lpqZa06dPt7797W9bdXV19hY8wm655RZr8uTJlsfjscaMGWMtXrw4GFosK/HOFZdlWVb06ncAAACGjzYuAADAMQguAADAMQguAADAMQguAADAMQguAADAMQguAADAMQguAADAMQguAADAMQguABxvypQpWr9+vd3FABAFBBcAQ3LzzTfr+uuvlyQtXLhQd955Z9T2vXHjRuXk5PTZvnPnTt16661RKwcA+yTbXQAAaGtrk8fjGfbPjxkzJoylARDLqHEBMCw333yztm7dqocfflgul0sul0sffvihJOmdd95ReXm5Ro4cqby8PN100006ceJE8GcXLlyoO+64Q3feeadyc3O1ZMkSSdK6des0e/ZsZWRkqKCgQLfffrsaGxslSVu2bNHKlStVV1cX3N99990nqe+lokOHDum6667TyJEjlZWVpRtvvFG1tbXBx++77z7NnTtXv/zlLzVlyhRlZ2fri1/8ohoaGoLPeeqppzR79mylpaXpvPPOU1lZmZqamiJ0NAGEiuACYFgefvhhlZaWatWqVTp69KiOHj2qgoICnT59WldffbUuueQS7dq1S88//7xqa2t144039vj5X/ziF/J4PHr11Ve1YcMGSZLb7daPf/xj7dmzR7/4xS/08ssv6zvf+Y4k6fLLL9f69euVlZUV3N9dd93Vp1x+v1/XXXedTp06pa1bt+rFF1/UBx98oOXLl/d43sGDB7V582Y9++yzevbZZ7V161Y98MADkqSjR4/qS1/6km655Ra9++672rJli5YtWybmpAXsx6UiAMOSnZ0tj8ej9PR0jRs3Lrj9Jz/5iS655BL98Ic/DG577LHHVFBQoPfff18zZsyQJF1wwQV68MEHe7xm9/YyU6ZM0fe//33ddttt+s///E95PB5lZ2fL5XL12F9vlZWVevvtt1VdXa2CggJJ0uOPP66LL75YO3fuVHFxsSQTcDZu3KjMzExJ0k033aTKykr94Ac/0NGjR9XR0aFly5Zp8uTJkqTZs2efw9ECEC7UuAAIq7/+9a965ZVXNHLkyODtwgsvlGRqOQLmzZvX52dfeuklLV68WBMmTFBmZqZuuukmnTx5Us3NzSHv/91331VBQUEwtEhSYWGhcnJy9O677wa3TZkyJRhaJGn8+PE6duyYJKmoqEiLFy/W7Nmz9YUvfEE/+9nP9Mknn4R+EABEDMEFQFg1NjZq6dKlqqqq6nHbv3+/rrzyyuDzMjIyevzchx9+qM9+9rOaM2eOfvvb32r37t3yer2STOPdcEtJSelx3+Vyye/3S5KSkpL04osv6g9/+IMKCwv1yCOPaObMmaqurg57OQAMDcEFwLB5PB75fL4e2y699FLt2bNHU6ZM0fTp03vceoeV7nbv3i2/36+HHnpIl112mWbMmKEjR44Mur/eLrroIh0+fFiHDx8Obtu7d69Onz6twsLCkH83l8ulK664Qvfff7/efPNNeTwePf300yH/PIDIILgAGLYpU6bo9ddf14cffqgTJ07I7/eroqJCp06d0pe+9CXt3LlTBw8e1B//+EetXLnyrKFj+vTpam9v1yOPPKIPPvhAv/zlL4ONdrvvr7GxUZWVlTpx4kS/l5DKyso0e/ZsfeUrX9Ebb7yhHTt26Ktf/aquuuoqzZ8/P6Tf6/XXX9cPf/hD7dq1S4cOHdLvfvc7HT9+XBdddNHQDhCAsCO4ABi2u+66S0lJSSosLNSYMWN06NAh5efn69VXX5XP59M111yj2bNn684771ROTo7c7oHfcoqKirRu3Tr9+7//u2bNmqVf/epXWrt2bY/nXH755brtttu0fPlyjRkzpk/jXsnUlDzzzDMaNWqUrrzySpWVlWnatGnatGlTyL9XVlaWtm3bps985jOaMWOG/uVf/kUPPfSQysvLQz84ACLCZdG/DwAAOAQ1LgAAwDEILgAAwDEILgAAwDEILgAAwDEILgAAwDEILgAAwDEILgAAwDEILgAAwDEILgAAwDEILgAAwDEILgAAwDH+fyVs4xtonlBJAAAAAElFTkSuQmCC\n",
+                        "image/png": "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AIBjEFwAAIBjEFwAAIBjEFwAAIBjEFwAAIBjEFwAAIBjpExwYQI6AABSHxPQAQCApGMCOgAAkHIILgAAwDEILgAAwDEILgAAwDEILgAAwDEILgAAwDEILgAAwDEILgAAwDEILgAAwDFSJrgw5T8AAKmPKf8BAEDSMeU/AABIOQQXAADgGAQXAADgGAQXAADgGAQXAADgGAQXAADgGAQXAADgGAQXAADgGAQXAADgGAQXAADgGCkTXLhXEQAAqY97FQEAgKTjXkUAACDlEFwAAIBjEFwAAIBjEFwAAIBjEFwAAIBjEFwAAIBjEFwAAIBjEFwAAIBjEFwAAIBjEFwAAIBjEFwAAIBjEFwAAIBjEFwAAIBjpExwqaysVElJiUpLS5PdFAAAECcuY4xJdiPsFOttsQEAwNAR6+93ylRcAABA6iO4AAAAxyC4AAAAxyC4AAAAxyC4AAAAxyC4AAAAxyC4AAAAxyC4AAAAxyC4AAAAxyC4AAAAxyC4AAAAxyC4AAAAxyC4AAAAxyC4AAAAxyC4AAAAxyC4AAAAxyC4AAAAxyC4AAAAx0iZ4FJZWamSkhKVlpYmuykAACBOXMYYk+xG2KmpqUk5OTlqbGxUdnZ2spsDAABiEOvvd8pUXAAAQOojuAAAAMcguAAAAMcguAAAAMcguAAAAMcguAAAAMcguAAAAMcguAAAAMcguAAAAMcguAAAAMcguAAAAMcguAAAAMcguAAAAMcguAAAAMcguAAAAMcguAAAAMcguAAAAMcguAAAAMcguAAAAMcguAAAAMcguAAAAMcguAAAAMcguAAAAMcguAAAAMcguAAAAMcguAAAAMdImeBSWVmpkpISlZaWJrspAAAgTlzGGJPsRtipqalJOTk5amxsVHZ2drKbAwAAYhDr73fKVFwAAEDqI7gAAADHILgAAADHILgAAADHILgAAADHILgAAADHILgAAADHILgAAADHILgAAADHILgAAADHILgAAADHILgAAADHILgAAADHILgAAADHILgAAADHILgAAADHILgAAADHILgAAADHILgAAADHILgAAADHILgAAADHILgAAADHILgAAADHILgAAADHILgAAADHILgAAADHILgAAADHILgAAADHILgAAADHILgAAADHILgAAADHILgAAADHILgAAADHILgAAADHILgAAADHILgAAADH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",
                         "text/plain": [
                             "<Figure size 640x480 with 1 Axes>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 },
@@ -259,15 +258,15 @@
                     "output_type": "stream",
                     "text": [
                         "Parameters:\n"
                     ]
                 },
                 {
                     "data": {
-                        "image/png": "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fiD61fwcfHD/DMSEhardFCIiIp/rU83Lgw8+iDvvvLPHY7Kzs/vVkJQUqZegsrISqampnv2VlZWYPHlyt88zGo0wGrn0PRER0WDRp/CSmJiIxMRERRqSlZWFlJQUbNu2zRNWLBYL9u3b16cZS0RERBTcFKt5KS0tRVFREUpLS+F0OlFUVISioiI0NjZ6jsnJycHGjRsBSLUaK1euxO9+9zt89NFHOHz4MJYsWYK0tDQsWrRIqWYSERGRxig2VXrNmjV47bXXPPenTJkCANixYwdmz54NADh58iTMZrPnmIceeghWqxX33nsv6uvrce2112LLli0ICwtTqplERESkMYIoiqLajfAli8UCk8kEs9mMmJgYtZtDREREvdCX7++AmSpNRERE1BsML0RERKQpDC9ERESkKQwvREREpCkML0RERKQpDC9ERESkKQwvREREpCkML0RERKQpDC9ERESkKYpdHkAt8oLBFotF5ZYQERFRb8nf271Z+D/owktDQwMAICMjQ+WWEBERUV81NDTAZDL1eEzQXdvI5XKhrKwM0dHREATBp+e2WCzIyMjA+fPned2kdvi+dI/vTdf4vnSP703X+L50L1jeG1EU0dDQgLS0NOh0PVe1BF3Pi06nw9ChQxV9jZiYGE1/QJTC96V7fG+6xvele3xvusb3pXvB8N5crsdFxoJdIiIi0hSGFyIiItIUhpc+MBqNeOSRR2A0GtVuSkDh+9I9vjdd4/vSPb43XeP70r3B+N4EXcEuERERBTf2vBAREZGmMLwQERGRpjC8EBERkaYwvBAREZGmMLz00rp165CZmYmwsDBMnz4d+/fvV7tJqnv00UchCILXlpOTo3azVLF7927cdNNNSEtLgyAI2LRpk9fjoihizZo1SE1NRXh4OPLz83Hq1Cl1GutHl3tf7rzzzk6fofnz56vTWD8qKCjAVVddhejoaCQlJWHRokU4efKk1zEtLS1Yvnw5hgwZgqioKPzwhz9EZWWlSi32j968L7Nnz+70mbnvvvtUarH/vPjii5g4caJnIbq8vDx88sknnscH2+eF4aUX3n33XaxatQqPPPIIDh48iEmTJmHevHm4dOmS2k1T3RVXXIHy8nLP9sUXX6jdJFVYrVZMmjQJ69at6/LxJ598Es899xzWr1+Pffv2ITIyEvPmzUNLS4ufW+pfl3tfAGD+/Ple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\n",
+                        "image/png": "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a16IiIiUwPASCW1X15X5a17Y80JERBRJioaXkpISTJ06FYmJicjIyMDChQtRVlZ2wef985//REFBAYxGIwoLC7FhwwYlm9l7nQ4bseeFiIhICYqGl23btmHJkiX44osvsGnTJrhcLlx99dVobu76F/rnn3+OW2+9FT/60Y/w1VdfYeHChVi4cCH27dunZFN7x9nJVGn2vBARESlC0b2NNm7cGPTxqlWrkJGRgT179uCKK67o9DnPPfcc5s2bhwceeAAA8Nhjj2HTpk148cUXsXLlSiWb23P+nheu80JERKS0Pq15aWxsBACkpKR0ec327dtRXFwc9NjcuXOxffv2Tq93OBywWq1BR59ru8KujD0vREREiuiz8OL1erFs2TLMnDkT48aN6/K6qqoqZGZmBj2WmZmJqqqqTq8vKSmBxWLxH7m5uRFtd0g6LdhlzwsREZES+iy8LFmyBPv27cObb74Z0c+7YsUKNDY2+o+KioqIfv6QdLpIHdd5ISIiUoKiNS+ypUuXYt26dfj4448xePDgbq/NyspCdXV10GPV1dXIysrq9HqDwQCDwRCxtvZItyvssueFiIgokhTteZEkCUuXLsWaNWuwefNm5OfnX/A5RUVFKC0tDXps06ZNKCoqUqqZvdftVGn2vBAREUWSoj0vS5YswerVq/HOO+8gMTHRX7disVgQFxcHALjjjjswaNAglJSUAADuu+8+zJo1C08//TQWLFiAN998E7t378Yrr7yiZFN7p9uCXfa8EBERRZKiPS8vv/wyGhsbMXv2bGRnZ/uPt956y39NeXk5Kisr/R/PmDEDq1evxiuvvIIJEybgX//6F9auXdttkW/UObjOCxERUV9RtOdFkqQLXrN169YOj91444248cYbFWiRQjobNpL3OWLPCxERUURxb6PecjsAr0u831XPSwghjoiIiELD8NJbbXtWOgsvkhdw2/u2TURERAMYw0tvyTUtWiOgaTMKp2szhMS1XoiIiCKG4aW3OltdFwDU6kCAYdEuERFRxDC89FZnxboyTpcmIiKKOIaX3vKvrpvY8RzDCxERUcQxvPSWs4thI6DNKrtNfdceIiKiAY7hpbe6GzYycH8jIiKiSGN46S15dd22WwPIOGxEREQUcQwvveXveWF4ISIi6gsML73VbXjhztJERESRxvDSW6EU7HKROiIioohheOkt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xx3IycnBwoULlWomERERxRjFpko//PDD+Otf/+r/eNKkSQCALVu2YPbs2QCAsrIyNDY2+q958MEH0dzcjHvuuQcNDQ24/PLLsXHjRhiNXCOFiIiIBJUkSVK0GxFJVqsVFosFjY2NMJvN0W4OERERhSCc39/9Zqo0ERERUSgYXoiIiCimMLwQERFRTGF4ISIiopjC8EJEREQxheGFiIiIYgrDCxEREcUUhhciIiKKKQwvREREFFMU2x4gWuQFg61Wa5RbQkRERKGSf2+HsvD/gAsvTU1NAIDc3Nwot4SIiIjC1dTUBIvF0u01A25vI6/Xi7NnzyIxMREqlSqin9tqtSI3NxcVFRXcN0lhvNd9h/e67/Be9x3e674TqXstSRKampqQk5MDtbr7qpYB1/OiVqsxePBgRV/DbDbzP0Mf4b3uO7zXfYf3uu/wXvedSNzrC/W4yFiwS0RERDGF4YWIiIhiCsNLGAwGA37961/DYDBEuykDHu913+G97ju8132H97rvRONeD7iCXSIiIhrY2PNCREREMYXhhYiIiGIKwwsRERHFFIYXIiIiiikMLyF66aWXkJeXB6PRiOnTp2Pnzp3RblLMKykpwdSpU5GYmIiMjAwsXLgQZWVlQdfY7XYsWbIEqampSEhIwPe//31UV1dHqcUDx5NPPgmVSoVly5b5H+O9jpwzZ87gBz/4AVJTUxEXF4fCwkLs3r3bf16SJDz88MPIzs5GXFwciouLceTIkSi2ODZ5PB786le/Qn5+PuLi4jB8+HA89thjQXvj8F733Mcff4zrrrsOOTk5UKlUWLt2bdD5UO5tfX09brvtNpjNZiQlJeFHP/oRbDZb7xsn0QW9+eabkl6vl1599VVp//790uLFi6WkpCSpuro62k2LaXPnzpVee+01ad++fdLevXula665RhoyZIhks9n819x7771Sbm6uVFpaKu3evVu67LLLpBkzZkSx1bFv586dUl5enjR+/Hjpvvvu8z/Oex0Z9fX10tChQ6U777xT2rFjh3T8+HHpgw8+kI4ePeq/5sknn5QsFou0du1a6euvv5auv/56KT8/X2ptbY1iy2PP448/LqWmpkrr1q2TTpw4If3zn/+UEhISpOeee85/De91z23YsEH6xS9+Ib399tsSAGnNmjVB50O5t/PmzZMmTJggffHFF9Inn3wijRgxQrr1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",
                         "text/plain": [
                             "<Figure size 640x480 with 1 Axes>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 }
@@ -297,15 +296,15 @@
             "execution_count": 7,
             "id": "807204bb",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
-                            "<h3>Version Information</h3><table><tr><th>Qiskit Software</th><th>Version</th></tr><tr><td><code>qiskit-terra</code></td><td>0.22.1</td></tr><tr><td><code>qiskit-aer</code></td><td>0.11.1</td></tr><tr><td><code>qiskit-ibmq-provider</code></td><td>0.19.2</td></tr><tr><td><code>qiskit</code></td><td>0.39.1</td></tr><tr><td><code>qiskit-nature</code></td><td>0.4.5</td></tr><tr><th>System information</th></tr><tr><td>Python version</td><td>3.9.13</td></tr><tr><td>Python compiler</td><td>Clang 12.0.0 </td></tr><tr><td>Python build</td><td>main, Aug 25 2022 18:29:29</td></tr><tr><td>OS</td><td>Darwin</td></tr><tr><td>CPUs</td><td>8</td></tr><tr><td>Memory (Gb)</td><td>32.0</td></tr><tr><td colspan='2'>Thu Nov 03 18:09:29 2022 CDT</td></tr></table>"
+                            "<h3>Version Information</h3><table><tr><th>Qiskit Software</th><th>Version</th></tr><tr><td><code>qiskit-terra</code></td><td>0.23.3</td></tr><tr><td><code>qiskit-aer</code></td><td>0.12.0</td></tr><tr><td><code>qiskit-ibmq-provider</code></td><td>0.20.2</td></tr><tr><td><code>qiskit-nature</code></td><td>0.5.2</td></tr><tr><th>System information</th></tr><tr><td>Python version</td><td>3.8.16</td></tr><tr><td>Python compiler</td><td>Clang 14.0.6 </td></tr><tr><td>Python build</td><td>default, Mar  1 2023 21:19:10</td></tr><tr><td>OS</td><td>Darwin</td></tr><tr><td>CPUs</td><td>8</td></tr><tr><td>Memory (Gb)</td><td>32.0</td></tr><tr><td colspan='2'>Tue Apr 11 19:11:37 2023 CDT</td></tr></table>"
                         ],
                         "text/plain": [
                             "<IPython.core.display.HTML object>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
@@ -348,13 +347,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.13"
+            "version": "3.8.16"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `circuit_knitting_toolbox-0.0.0/docs/tutorials/entanglement_forging/tutorial_2_forging_with_quantum_serverless.ipynb` & `circuit-knitting-toolbox-0.1.0/docs/entanglement_forging/tutorials/tutorial_2_forging_with_quantum_serverless.ipynb`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9886336352449634%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(4, 'See [Tutorial 1](tutorial_1_getting_started.ipynb) for "*

 * *            'a high-level breakdown of the entanglement forging algorithm, or check out the '*

 * *            '[explanatory material](../explanation/index.rst) for a more detailed '*

 * *            'explanation.\\n\'), (5, \'\\n\'), (6, \'<span style="color:red"><i>Quantum Serverless '*

 * *            'does not support Qiskit Nature 0.6.0 yet. In order to use entanglement forging with '*

 * *            'quantum serverless, u […]*

```diff
@@ -5,15 +5,17 @@
             "id": "52acc23d",
             "metadata": {},
             "source": [
                 "# Tutorial 2: Entanglement Forging with Quantum Serverless\n",
                 "\n",
                 "**Entanglement forging** is a method which allows us to represent expectation values of a 2n-qubit wavefunction as sums of multiple expectation values of n-qubit states, embedded in a classical optimization, thus doubling the size of the system that can be exactly simulated with a fixed number of qubits.\n",
                 "\n",
-                "See [Tutorial 1](https://github.com/Qiskit-Extensions/circuit-knitting-toolbox/blob/main/docs/tutorials/entanglement_forging/tutorial_1_getting_started.ipynb) for a high-level breakdown of the entanglement forging algorithm, or check out the [explanatory material](https://github.com/Qiskit-Extensions/circuit-knitting-toolbox/blob/main/docs/explanation/entanglement_forging/index.rst) for a more detailed explanation."
+                "See [Tutorial 1](tutorial_1_getting_started.ipynb) for a high-level breakdown of the entanglement forging algorithm, or check out the [explanatory material](../explanation/index.rst) for a more detailed explanation.\n",
+                "\n",
+                "<span style=\"color:red\"><i>Quantum Serverless does not support Qiskit Nature 0.6.0 yet. In order to use entanglement forging with quantum serverless, users should use 0.5.2 < Qiskit Nature < 0.6.0. There is an [associated issue in the quantum-serverless repo](https://github.com/Qiskit-Extensions/quantum-serverless/issues/413) to address this.</i></span>"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "69a8216f",
             "metadata": {},
             "source": [
@@ -39,42 +41,41 @@
         {
             "cell_type": "code",
             "execution_count": 1,
             "id": "4173c15e",
             "metadata": {},
             "outputs": [],
             "source": [
+                "from __future__ import annotations\n",
+                "\n",
                 "from pathlib import Path\n",
                 "import numpy as np\n",
-                "from qiskit_nature.problems.second_quantization import ElectronicStructureProblem\n",
-                "from circuit_knitting_toolbox.utils import IntegralDriver\n",
+                "from qiskit_nature.second_q.problems import ElectronicStructureProblem\n",
+                "from qiskit_nature.second_q.hamiltonians import ElectronicEnergy\n",
                 "\n",
                 "system_data = np.load(Path(\"data\") / \"reactant_2mo.npz\")\n",
                 "num_molecular_orbitals = 2\n",
                 "\n",
-                "driver = IntegralDriver(\n",
-                "    hcore=system_data[\"h1\"],\n",
-                "    mo_coeff=system_data[\"HF_mo_coeff\"],\n",
-                "    eri=system_data[\"Gamma_eri\"],\n",
-                "    num_alpha=system_data[\"na\"],\n",
-                "    num_beta=system_data[\"nb\"],\n",
-                "    nuclear_repulsion_energy=system_data[\"h0\"],\n",
+                "hamiltonian = ElectronicEnergy.from_raw_integrals(\n",
+                "    system_data[\"h1\"], system_data[\"Gamma_eri\"]\n",
                 ")\n",
-                "\n",
-                "problem = ElectronicStructureProblem(driver)"
+                "hamiltonian.nuclear_repulsion_energy = system_data[\"h0\"]\n",
+                "problem = ElectronicStructureProblem(hamiltonian)\n",
+                "problem.num_particles = (system_data[\"na\"], system_data[\"nb\"])\n",
+                "mo_coeff = system_data[\"HF_mo_coeff\"]"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "453dde4f",
             "metadata": {},
             "source": [
                 "### Configure the entanglement forging specific inputs\n",
                 "\n",
-                "The ansatz for Entanglement Forging consists of a set of input bitstrings and a parameterized circuit.  (See the [explanatory material](https://github.com/Qiskit-Extensions/circuit-knitting-toolbox/blob/main/docs/explanation/entanglement_forging/index.rst) for additional background on the method). For this demo, we will use the same bitstrings and ansatz for both the U and V subsystems, and we will use the [TwoLocal](https://qiskit.org/documentation/stubs/qiskit.circuit.library.TwoLocal.html) circuit from Qiskit, along with [hop gates](https://doi.org/10.1103/PRXQuantum.3.010309)."
+                "The ansatz for Entanglement Forging consists of a set of input bitstrings and a parameterized circuit.  (See the [explanatory material](../explanation/index.rst) for additional background on the method). For this demo, we will use the same bitstrings and ansatz for both the U and V subsystems, and we will use the [TwoLocal](https://qiskit.org/documentation/stubs/qiskit.circuit.library.TwoLocal.html) circuit from Qiskit, along with [hop gates](https://doi.org/10.1103/PRXQuantum.3.010309)."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 2,
             "id": "f25814e9",
             "metadata": {},
@@ -113,15 +114,15 @@
             "cell_type": "code",
             "execution_count": 3,
             "id": "67d53b1a",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
-                        "image/png": "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\n",
+                        "image/png": "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",
                         "text/plain": [
                             "<Figure size 287.294x200.667 with 1 Axes>"
                         ]
                     },
                     "execution_count": 3,
                     "metadata": {},
                     "output_type": "execute_result"
@@ -178,15 +179,15 @@
         {
             "cell_type": "markdown",
             "id": "5b77cbc9",
             "metadata": {},
             "source": [
                 "### Set up Quantum Serverless\n",
                 "\n",
-                "We can use Quantum Serverless to send the entanglement forging routine to a remote compute resource. For this tutorial, we will use our local CPU cores as the compute cluster. See the [Quantum Serverless](https://github.com/Qiskit-Extensions/quantum-serverless) documentation (and below) for more informatin about how to use other clusters."
+                "We can use Quantum Serverless to send the entanglement forging routine to a remote compute resource. For this tutorial, we will use our local CPU cores as the compute cluster. See the [Quantum Serverless](https://github.com/Qiskit-Extensions/quantum-serverless) documentation (and below) for more information about how to use other clusters."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 5,
             "id": "ec28c8e4",
             "metadata": {},
@@ -224,67 +225,70 @@
         {
             "cell_type": "code",
             "execution_count": 6,
             "id": "a940a226",
             "metadata": {},
             "outputs": [],
             "source": [
-                "from typing import Optional, Sequence, Tuple, Dict, Union\n",
+                "from typing import Sequence\n",
                 "from qiskit.algorithms.optimizers import Optimizer\n",
                 "from qiskit.result import Result\n",
-                "from quantum_serverless import run_qiskit_remote\n",
+                "from quantum_serverless import distribute_task\n",
                 "from circuit_knitting_toolbox.entanglement_forging import (\n",
                 "    EntanglementForgingGroundStateSolver,\n",
                 ")\n",
                 "\n",
                 "\n",
-                "@run_qiskit_remote()\n",
+                "@distribute_task()\n",
                 "def solve_remote(\n",
                 "    problem: ElectronicStructureProblem,\n",
-                "    ansatz_circuit: EntanglementForgingAnsatz,\n",
+                "    ansatz: EntanglementForgingAnsatz,\n",
                 "    optimizer: Optimizer,\n",
-                "    service_args: Optional[Dict] = None,\n",
-                "    backend_names: Optional[Union[str, Sequence[str]]] = None,\n",
-                "    options_dicts: Optional[Union[Dict, Sequence[Dict]]] = None,\n",
-                "    initial_point: Optional[Sequence[float]] = None,\n",
-                "    orbitals_to_reduce: Optional[Sequence[int]] = None,\n",
+                "    service_args: dict | None = None,\n",
+                "    backend_names: str | Sequence[str] | None = None,\n",
+                "    options_dicts: dict | Sequence[dict] | None = None,\n",
+                "    initial_point: Sequence[float] | None = None,\n",
+                "    orbitals_to_reduce: Sequence[int] | None = None,\n",
+                "    mo_coeff: np.ndarray | None = None,\n",
                 ") -> Result:\n",
                 "    \"\"\"\n",
                 "    Wrapper function for running entanglement forging VQE on a remote resource.\n",
                 "\n",
                 "        Args:\n",
                 "            - problem: A class encoding the problem to be solved\n",
                 "            - ansatz: The ansatz\n",
                 "            - optimizer: Optimizer to use to optimize the ansatz circuit parameters\n",
                 "            - service_args: The arguments for instantiating a QiskitRuntimeService\n",
                 "            - backend_names: List of backend names to use during parallel computation\n",
                 "            - options_dicts: Options to use with backends\n",
                 "            - initial_point: Initial values for ansatz parameters\n",
                 "            - orbitals_to_reduce: List of orbital indices to remove from the problem before\n",
                 "                decomposition.\n",
+                "            - mo_coeff: Coefficients for converting an input problem to MO basis\n",
                 "        Returns:\n",
                 "            - An interpreted EigenstateResult\n",
                 "    \"\"\"\n",
                 "    service = QiskitRuntimeService(**service_args) if service_args else None\n",
                 "\n",
                 "    # Convert options dictionaries into Options objects\n",
                 "    options = None\n",
                 "    if options_dicts:\n",
-                "        if isinstance(options_dicts, Dict):\n",
+                "        if isinstance(options_dicts, dict):\n",
                 "            options_dicts = [options_dicts]\n",
                 "        options = [Options(**o) for o in options_dicts]\n",
                 "\n",
                 "    solver = EntanglementForgingGroundStateSolver(\n",
                 "        ansatz=ansatz,\n",
                 "        service=service,\n",
                 "        optimizer=optimizer,\n",
                 "        backend_names=backend_names,\n",
                 "        options=options,\n",
                 "        initial_point=initial_point,\n",
                 "        orbitals_to_reduce=orbitals_to_reduce,\n",
+                "        mo_coeff=mo_coeff,\n",
                 "    )\n",
                 "    result = solver.solve(problem)\n",
                 "\n",
                 "    return result"
             ]
         },
         {
@@ -318,52 +322,63 @@
                 "\n",
                 "# QiskitRuntimeService is not serializable, so we must convert it to a dictionary before passing to remote function\n",
                 "service_args = None if service is None else service.active_account()\n",
                 "\n",
                 "# The Options class is not serializable, so we must convert it to a dictionary before passing to remote function\n",
                 "options_dicts = [asdict(o) for o in options]\n",
                 "\n",
-                "with serverless:\n",
+                "with serverless.context():\n",
                 "    forging_result_future = solve_remote(\n",
                 "        problem,\n",
                 "        ansatz,\n",
                 "        optimizer,\n",
                 "        service_args=service_args,\n",
                 "        backend_names=backend_names,\n",
                 "        options_dicts=options_dicts,\n",
+                "        mo_coeff=mo_coeff,\n",
                 "    )\n",
                 "    results = get(forging_result_future)"
             ]
         },
         {
+            "cell_type": "code",
+            "execution_count": 8,
+            "id": "829fdae1",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "problem.basis"
+            ]
+        },
+        {
             "cell_type": "markdown",
             "id": "9601ac33",
             "metadata": {},
             "source": [
                 "### Visualize the results\n",
                 "\n",
                 "Visualize the convergence of the estimated ground state energy and the Schmidt coefficients as the ansatz parameters are optimized."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 8,
+            "execution_count": 9,
             "id": "97ae8342",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Energy:\n"
                     ]
                 },
                 {
                     "data": {
-                        "image/png": "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v+gX6+8x1t8fEPvvUan3J0kSWlpakJOTA52u966WmBt50el0GDZsmKKvkZqaGpP/Qcpi/f0Bsf8e+f6iX6y/x1h/f0Dsv0cl3t/FRlxkbNglIiKiqMLwQkRERFGF4aUPTCYTHn30UZhMJrVLUUSsvz8g9t8j31/0i/X3GOvvD4j996iF9xdzDbtEREQU2zjyQkRERFGF4YWIiIiiCsMLERERRRWGFyIiIooqDC998MILLyAvLw+JiYmYMmUKtm7dqnZJYVFeXo5JkyYhJSUFgwcPxq233oqqqiq1y1LME088AUEQMH/+fLVLCasTJ07ge9/7HjIyMpCUlITi4mJs375d7bLCwufzYcmSJRg5ciSSkpJwySWX4Ne//nVIZ6Bo1ccff4ybbroJOTk5EAQBb731VrevS5KEpUuXYsiQIUhKSsKMGTNw4MABdYrth97eX0dHBx555BEUFxfDYrEgJycH99xzD06ePKlewX10sb+/rh544AEIgoCVK1dGrL5wCOU97tu3DzfffDOsVissFgsmTZqE6upqxWtjeAnRG2+8gZ/85Cd49NFHsXPnTowfPx4zZ85EfX292qUN2KZNm/Dggw9i8+bNWLduHTo6OnD99dejtbVV7dLCbtu2bfjd736Hyy67TO1SwurMmTO4+uqrkZCQgPfeew9ff/01nnrqKQwaNEjt0sJixYoVePHFF/H8889j3759WLFiBZ588kk899xzapfWb62trRg/fjxeeOGFHr/+5JNP4tlnn8WqVauwZcsWWCwWzJw5E+3t7RGutH96e39tbW3YuXMnlixZgp07d+LNN99EVVUVbr75ZhUq7Z+L/f3J1qxZg82bNyMnJydClYXPxd7joUOHcM0116CoqAgbN27Erl27sGTJEiQmJipfnEQhmTx5svTggw8G7/t8PiknJ0cqLy9XsSpl1NfXSwCkTZs2qV1KWLW0tEijR4+W1q1bJ1177bXSQw89pHZJYfPII49I11xzjdplKObGG2+U7r///m6PzZ49W7r77rtVqii8AEhr1qwJ3hdFUcrOzpZ+85vfBB9ramqSTCaT9Je//EWFCgfm3PfXk61bt0oApGPHjkWmqDC60Ps7fvy4NHToUGnPnj3SiBEjpN/+9rcRry1cenqPd9xxh/S9731PlXo48hICj8eDHTt2YMaMGcHHdDodZsyYgS+++ELF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\n",
+                        "image/png": "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4EAMq+25adOmqbS0VC+88IIeeugh7d27V5/61KdUW1vb4fGJev8k6emnn5bH49GiRYs6PSbR7t+ZQvchknvUm9/jeNHQ0KA777xTN998c5eb3UX6c26nuXPn6rHHHtPGjRt1zz33aMuWLbrqqqsUCAQ6PD6R758krVmzRtnZ2d12qcTrPezob0N1dbVcLtdZgbq7v42hY3p6TqSSbldpdO/222/XO++8020f6/Tp0zV9+vTw8xkzZmjChAn61a9+pe9///tWlxmxq666Kvzv8847T9OmTdPIkSP1xBNP9Oj/CSWSRx55RFdddZUKCws7PSbR7l9/1tTUpAULFsg0TT300ENdHptIP+c33XRT+N+TJ0/Weeedp3POOUebN2/WrFmzbKzMGo8++qhuueWWbgfGx+s97OnfhnhAy0urwYMHy+l0njWCuqamRvn5+R2ek5+fH9Hx8eDrX/+6nnvuOW3atEnDhw+P6NzU1FSVlJTogw8+sKi66MrNzdW4ceM6rTcR758k7d+/Xxs2bNC//uu/RnReot2/0H2I5B715vfYbqHgsn//fq1fv77LVpeOdPdzHk/GjBmjwYMHd1prIt6/kJdfflnl5eUR/15K8XEPO/vbkJ+fL7/fL4/H0+747v42ho7p6TmRIry0crlcmjp1qjZu3Bh+LRgMauPGje3+3+vppk+f3u54SVq/fn2nx9vJNE19/etf17p16/TSSy9p9OjREb9HIBDQ22+/rYKCAgsqjL66ujp9+OGHndabSPfvdL/97W81ZMgQXXPNNRGdl2j3b/To0crPz293j3w+n15//fVO71Fvfo/tFAou77//vjZs2KBBgwZF/B7d/ZzHkwMHDujYsWOd1ppo9+90jzzyiKZOnaopU6ZEfK6d97C7vw1Tp05Vampqu3tSXl6uioqKTu9Jb353e1M4Wv3xj38009LSzNLSUnPXrl3mV7/6VTM3N9esrq42TdM0Fy5caC5dujR8/KuvvmqmpKSY//3f/23u3r3bXLFihZmammq+/fbbdl1CpxYvXmy63W5z8+bNZlVVVfhRX18fPubM61u5cqX54osvmh9++KG5Y8cO86abbjLT09PNd999145L6NaSJUvMzZs3m3v37jVfffVVc/bs2ebgwYPNw4cPm6aZ2PcvJBAImCNGjDDvvPPOs76WiPevtrbWfPPNN80333zTlGTed9995ptvvhmebfOjH/3IzM3NNZ955hnzrbfeMufNm2eOHj3aPHXqVPg9Lr/8cvOBBx4IP+/u9zhers/v95vXXnutOXz4cLOsrKzd72VjY2On19fdz3m8XF9tba357W9/23zttdfMvXv3mhs2bDAvuOAC89xzzzUbGho6vb54un+m2f3PqGmaptfrNTMzM82HHnqow/eI53vYk78Nt912mzlixAjzpZdeMrdv325Onz7dnD59erv3GT9+vPnUU0+Fn/fkd7cvCC9neOCBB8wRI0aYLpfLvPjii82tW7eGv3bZZZeZX/jCF9od/8QTT5jjxo0zXS6XOWnSJPP555+PccU9I6nDx29/+9vwMWde3x133BH+XgwdOtS8+uqrzZ07d8a++B668cYbzYKCAtPlcpnDhg0zb7zxRvODDz4Ifz2R71/Iiy++aEoyy8vLz/paIt6/TZs2dfhzGbqOYDBo3nXXXebQoUPNtLQ0c9asWWdd+8iRI80VK1a0e62r3+NY6ur69u7d2+nv5aZNm8Lvceb1dfdzHktdXV99fb155ZVXmnl5eWZqaqo5cuRI8ytf+cpZISSe759pdv8zapqm+atf/crMyMgwPR5Ph+8Rz/ewJ38bTp06ZX7ta18zBw4caGZmZprXX3+9WVVVddb7nH5OT353+8Jo/VAAAICEwJgXAACQUAgvAAAgoRBeAABAQiG8AACAhEJ4AQAACYXwAgAAEgrhBQAAJBTCCwAASCiEFwBJYdSoUbr//vvtLgNADBBeAERs0aJFuu666yRJM2fO1B133BGzzy4tLVVubu5Zr2/btk1f/epXY1YHAPuk2F0AAEiS3++Xy+Xq9fl5eXlRrAZAPKPlBUCvLVq0SFu2bNHPfvYzGYYhwzC0b98+SdI777yjq666SgMGDNDQoUO1cOFCHT16NHzuzJkz9fWvf1133HGHBg8erDlz5kiS7rvvPk2ePFlZWVkqKirS1772NdXV1UmSNm/erC9+8Yvyer3hz7v77rslnd1tVFFRoXnz5mnAgAHKycnRggULVFNTE/763XffrfPPP1+/+93vNGrUKLndbt10002qra0NH/OnP/1JkydPVkZGhgYNGqTZs2fr5MmTFn03AfQU4QVAr/3sZz/T9OnT9ZWvfEVVVVWqqqpSUVGRPB6PLr/8cpWUlGj79u164YUXVFNTowULFrQ7f82aNXK5XHr11Vf18MMPS5IcDod+/vOf691339WaNWv00ksv6bvf/a4kacaMGbr//vuVk5MT/rxvf/vbZ9UVDAY1b948HT9+XFu2bNH69ev10Ucf6cYbb2x33Icffqinn35azz33nJ577jlt2bJFP/rRjyRJVVVVuvnmm/WlL31Ju3fv1ubNm3XDDTeIvWwB+9FtBKDX3G63XC6XMjMzlZ+fH379wQcfVElJiX74wx+GX3v00UdVVFSk9957T+PGjZMknXvuubr33nvbvefp42dGjRqlH/zgB7rtttv0y1/+Ui6XS263W4ZhtPu8M23cuFFvv/229u7dq6KiIknSY489pkmTJmnbtm266KKLJLWEnNLSUmVnZ0uSFi5cqI0bN2rVqlWqqqpSc3OzbrjhBo0cOVKSNHny5D58twBECy0vAKLun//8pzZt2qQBAwaEH8XFxZJaWjtCpk6deta5GzZs0KxZszRs2DBlZ2dr4cKFOnbsmOrr63v8+bt371ZRUVE4uEjSxIkTlZubq927d4dfGzVqVDi4SFJBQYEOHz4sSZoyZYpmzZqlyZMna/78+fr1r3+tEydO9PybAMAyhBcAUVdXV6fPfvazKisra/d4//33demll4aPy8rKanfevn379JnPfEbnnXee/vznP2vHjh36xS9+IallQG+0paamtntuGIaCwaAkyel0av369frrX/+qiRMn6oEHHtD48eO1d+/eqNcBIDKEFwB94nK5FAgE2r12wQUX6N1339WoUaM0duzYdo8zA8vpduzYoWAwqJ/85Cf6xCc+oXHjxunQoUPdft6ZJkyYoMrKSlVWVoZf27VrlzwejyZOnNjjazMMQ5/85Ce1cuVKvfnmm3K5XFq3bl2PzwdgDcILgD4ZNWqUXn/9de3bt09Hjx5VMBjU7bffruPHj+vmm2/Wtm3b9OGHH+rFF1/UF7/4xS6Dx9ixY9XU1KQHHnhAH330kX73u9+FB/Ke/nl1dXXauHGjjh492mF30uzZszV58mTdcsst2rlzp9544w3deuutuuyyy3ThhRf26Lpef/11/fCHP9T27dtVUVGhp556SkeOHNGECRMi+wYBiDrCC4A++fa3vy2n06mJEycqLy9PFRUVKiws1KuvvqpAIKArr7xSkydP1h133KHc3Fw5HJ3/Z2fKlCm67777dM899+jjH/+4/vCHP2j16tXtjpkxY4Zuu+023XjjjcrLyztrwK/U0mLyzDPPaODAgbr00ks1e/ZsjRkzRmvXru3xdeXk5Ojvf/+7rr76ao0bN07f+9739JOf/ERXXXVVz785ACxhmMz7AwAACYSWFwAAkFAILwAAIKEQXgAAQEIhvAAAgIRCeAEAAAmF8AIAABIK4QUAACQUwgsAAEgohBcAAJBQCC8AACChEF4AAEBC+X8wJWxDTgAiDAAAAABJRU5ErkJggg==",
                         "text/plain": [
                             "<Figure size 640x480 with 1 Axes>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 },
@@ -372,15 +387,15 @@
                     "output_type": "stream",
                     "text": [
                         "Schmidt Coefficients:\n"
                     ]
                 },
                 {
                     "data": {
-                        "image/png": "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1NnZqcWLF6u6ulrnnHOONm7c6PeQXHHbbbdp+fLlqq+v15w5c/Te975XL774ot/D8sztt9+uSCSitWvX+j0UV73xxhu69tpr1dLSopqaGi1ZskTPPvus38NyRSqV0s0336zjjjtONTU1estb3qK/+Zu/mfY8kyB78sknddlll6mtrU2RSEQPPvjguNsty9LnPvc5zZ8/XzU1NVq5cqVefvllfwZbgKle3+joqD796U9ryZIlSiQSamtr04c//GHt3r3bvwEXYLq/w1wf+9jHFIlEdPfdd5dsfMWayet74YUXdPnll6uxsVGJRELLly/Xzp07PR8bwWUG7r//fq1bt0633HKLtmzZoqVLl+rSSy/Vvn37/B5a0TZs2KCOjg49/fTTevTRRzU6Oqp3vetd6u/v93tortu0aZP+4R/+QWeccYbfQ3HVgQMHdP7556uyslI/+clPtG3bNt15551qamrye2iuuOOOO/T1r39dX/va1/TCCy/ojjvu0Je//GXdc889fg+tYP39/Vq6dKk6OzsnvP3LX/6yvvrVr+ree+/VM888o0QioUsvvVRDQ0MlHmlhpnp9AwMD2rJli26++WZt2bJFP/zhD/Xiiy/q8ssv92GkhZvu79B44IEH9PTTT6utra1EI3PHdK/v1Vdf1dvf/nadcsopeuKJJ/Sb3/xGN998s6qrq70fnIVprVixwuro6HC+TqVSVltbm3Xbbbf5OCpv7Nu3z5Jkbdiwwe+huKq3t9c68cQTrUcffdS68MILrRtvvNHvIbnm05/+tPX2t7/d72F45t3vfrd1ww03jLvuyiuvtK655hqfRuQuSdYDDzzgfJ1Op6158+ZZf/u3f+tcd/DgQauqqsr6wQ9+4MMIi3P465vIxo0bLUnWjh07SjMol032Gn//+99bCxYssJ5//nnr2GOPtf7u7/6u5GNzw0Sv7+qrr7auvfZaX8bDjMs0RkZGtHnzZq1cudK5LhqNauXKlXrqqad8HJk3Dh06JElqbm72eSTu6ujo0Lvf/e5xf4/l4j//8z+1bNkyfeADH9CcOXN01lln6Zvf/Kbfw3LNeeedp/Xr1+ull16SJP3617/WL37xC61atcrnkXlj+/bt2rNnz7if1cbGRp1zzjll+TtHsn/vRCIRzZo1y++huCadTmv16tW66aabdNppp/k9HFel02k9/PDDOumkk3TppZdqzpw5Ouecc6ZcLnMTwWUayWRSqVRKc+fOHXf93LlztWfPHp9G5Y10Oq21a9fq/PPP1+mnn+73cFzzr//6r9qyZYtuu+02v4fiiddee01f//rXdeKJJ+qnP/2p/vRP/1Qf//jH9e1vf9vvobniM5/5jD74wQ/qlFNOUWVlpc466yytXbtW11xzjd9D84T5vXI0/M6RpKGhIX3605/Whz70obI6lPCOO+5QRUWFPv7xj/s9FNft27dPfX19uv322/WHf/iH+tnPfqb3ve99uvLKK7VhwwbPn7/sTodG4To6OvT888/rF7/4hd9Dcc2uXbt044036tFHHy3N2qsP0um0li1bpltvvVWSdNZZZ+n555/Xvffeq+uuu87n0RXv3/7t3/S9731P3//+93Xaaadp69atWrt2rdra2sri9R3NRkdHddVVV8myLH3961/3eziu2bx5s77yla9oy5YtikQifg/Hdel0WpJ0xRVX6BOf+IQk6cwzz9T//M//6N5779WFF17o6fMz4zKN1tZWxWIx7d27d9z1e/fu1bx583walfvWrFmjhx56SI8//riOOeYYv4fjms2bN2vfvn1661vfqoqKClVUVGjDhg366le/qoqKCqVSKb+HWLT58+ervb193HWnnnpqSar7S+Gmm25yZl2WLFmi1atX6xOf+ETZzqCZ3yvl/jvHhJYdO3bo0UcfLavZlv/+7//Wvn37tGjRIuf3zo4dO/Tnf/7nWrx4sd/DK1pra6sqKip8+71DcJlGPB7X2WefrfXr1zvXpdNprV+/Xueee66PI3OHZVlas2aNHnjgAf385z/Xcccd5/eQXHXJJZfoueee09atW52PZcuW6ZprrtHWrVsVi8X8HmLRzj///CO2sL/00ks69thjfRqRuwYGBhSNjv9VFYvFnP/rKzfHHXec5s2bN+53Tk9Pj5555pmy+J0jZUPLyy+/rMcee0wtLS1+D8lVq1ev1m9+85txv3fa2tp000036ac//anfwytaPB7X8uXLffu9w1LRDKxbt07XXXedli1bphUrVujuu+9Wf3+/rr/+er+HVrSOjg59//vf149+9CPV19c7a+iNjY2qqanxeXTFq6+vP6JeJ5FIqKWlpWzqeD7xiU/ovPPO06233qqrrrpKGzdu1De+8Q194xvf8Htorrjsssv0pS99SYsWLdJpp52mX/3qV7rrrrt0ww03+D20gvX19emVV15xvt6+fbu2bt2q5uZmLVq0SGvXrtUXv/hFnXjiiTruuON08803q62tTe9973v9G3Qepnp98+fP1/vf/35t2bJFDz30kFKplPN7p7m5WfF43K9h52W6v8PDw1hlZaXmzZunk08+udRDLch0r++mm27S1VdfrQsuuEAXX3yxHnnkEf34xz/WE0884f3gfNnLFEL33HOPtWjRIisej1srVqywnn76ab+H5ApJE3788z//s99D80y5bYe2LMv68Y9/bJ1++ulWVVWVdcopp1jf+MY3/B6Sa3p6eqwbb7zRWrRokVVdXW0df/zx1l/+5V9aw8PDfg+tYI8//viE/+6uu+46y7LsLdE333yzNXfuXKuqqsq65JJLrBdffNHfQedhqte3ffv2SX/vPP74434Pfcam+zs8XNi2Q8/k9f3TP/2TdcIJJ1jV1dXW0qVLrQcffLAkY4tYVojbTwIAgKMKNS4AACA0CC4AACA0CC4AACA0CC4AACA0CC4AACA0CC4AACA0CC4AACA0CC4AACA0CC4AQm/x4sW6++67/R4GgBIguADIy0c+8hHnzJyLLrpIa9euLdlz33fffZo1a9YR12/atEl/8id/UrJxAPAPhywC8N3IyEhRh+vNnj3bxdEACDJmXAAU5CMf+Yg2bNigr3zlK4pEIopEInr99dclSc8//7xWrVqluro6zZ07V6tXr1YymXS+96KLLtKaNWu0du1atba26tJLL5Uk3XXXXVqyZIkSiYQWLlyoP/uzP1NfX58k6YknntD111+vQ4cOOc/3+c9/XtKRS0U7d+7UFVdcobq6OjU0NOiqq67S3r17nds///nP68wzz9R3v/tdLV68WI2NjfrgBz+o3t5e5z7//u//riVLlqimpkYtLS1auXKl+vv7PfrTBDBTBBcABfnKV76ic889Vx/96Ef15ptv6s0339TChQt18OBBvfOd79RZZ52lZ599Vo888oj27t2rq666atz3f/vb31Y8Htcvf/lL3XvvvZKkaDSqr371q/rtb3+rb3/72/r5z3+uT33qU5Kk8847T3fffbcaGhqc5/vkJz95xLjS6bSuuOIKdXd3a8OGDXr00Uf12muv6eqrrx53v1dffVUPPvigHnroIT300EPasGGDbr/9dknSm2++qQ996EO64YYb9MILL+iJJ57QlVdeKc6kBfzHUhGAgjQ2Nioej6u2tlbz5s1zrv/a176ms846S7feeqtz3be+9S0tXLhQL730kk466SRJ0oknnqgvf/nL4x4zt15m8eLF+uIXv6iPfexj+vu//3vF43E1NjYqEomMe77DrV+/Xs8995y2b9+uhQsXSpK+853v6LTTTtOmTZu0fPlySXbAue+++1RfXy9JWr16tdavX68vfelLevPNNzU2NqYrr7xSxx57rCRpyZIlRfxpAXALMy4AXPXrX/9ajz/+uOrq6pyPU045RZI9y2GcffbZR3zvY489pksuuUQLFixQfX29Vq9era6uLg0MDMz4+V944QUtXLjQCS2S1N7erlmzZumFF15wrlu8eLETWiRp/vz52rdvnyRp6dKluuSSS7RkyRJ94AMf0De/+U0dOHBg5n8IADxDcAHgqr6+Pl122WXaunXruI+XX35ZF1xwgXO/RCIx7vtef/11vec979EZZ5yh//iP/9DmzZvV2dkpyS7edVtlZeW4ryORiNLptCQpFovp0Ucf1U9+8hO1t7frnnvu0cknn6zt27e7Pg4A+SG4AChYPB5XKpUad91b3/pW/fa3v9XixYt1wgknjPs4PKzk2rx5s9LptO6880697W1v00knnaTdu3dP+3yHO/XUU7Vr1y7t2rXLuW7btm06ePCg2tvbZ/zaIpGIzj//fH3hC1/Qr371K8XjcT3wwAMz/n4A3iC4ACjY4sWL9cwzz+j1119XMplUOp1WR0eHuru79aEPfUibNm3Sq6++qp/+9Ke6/vrrpwwdJ5xwgkZHR3XPPffotdde03e/+12naDf3+fr6+rR+/Xolk8kJl5BWrlypJUuW6JprrtGWLVu0ceNGffjDH9aFF16oZcuWzeh1PfPMM7r11lv17LPPaufOnfrhD3+o/fv369RTT83vDwiA6wguAAr2yU9+UrFYTO3t7Zo9e7Z27typtrY2/fKXv1QqldK73vUuLVmyRGvXrtWsWbMUjU7+K2fp0qW66667dMcdd+j000/X9773Pd12223j7nPeeefpYx/7mK6++mrNnj37iOJeyZ4p+dGPfqSmpiZdcMEFWrlypY4//njdf//9M35dDQ0NevLJJ/VHf/RHOumkk/RXf/VXuvPOO7Vq1aqZ/+EA8ETEYn8fAAAICWZcAABAaBBcAABAaBBcAABAaBBcAABAaBBcAABAaBBcAABAaBBcAABAaBBcAABAaBBcAABAaBBcAABAaBBcAABAaPx/6MI6ArM2Tv4AAAAASUVORK5CYII=\n",
+                        "image/png": "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DhzQjBkzRn3OjBkzcjreL9asWaOHHnpITz75pE444YScnltZWamzzjpLr776apFa556mpibNmzdvzLYG9fpJ0htvvKHHH39cf/d3f5fT84J0/ezrkMs1yufv2Gt2aHnjjTf02GOPjdvbMpqJfs/95qSTTtKUKVPGbG8Qr6Ek/e53v9POnTtz/puU/HENx/pcmDFjhgYGBhSLxYYdP9Fno31Mts/JFcFFUiQS0aJFi7Rx40bnvmQyqY0bNw77P9ZMy5YtG3a8JD322GNjHu810zS1Zs0aPfDAA3riiSd04okn5nyORCKhF198Uccff3wRWuiurq4uvfbaa2O2NWjXL9OPfvQjTZs2TR/5yEdyel6Qrt+JJ56oGTNmDLtGHR0devbZZ8e8Rvn8HXvJDi27du3S448/rsmTJ+d8jol+z/3mrbfe0jvvvDNme4N2DW0//OEPtWjRIi1cuDDn53p5DSf6XFi0aJEqKyuHXY+dO3fqzTffHPN65PO3m0/DYZrmz3/+c7OqqsrcsGGDuX37dvPTn/602dTUZO7fv980TdO85pprzK985SvO8c8884xZUVFh/tu//Zu5Y8cOc926dWZlZaX54osvevUWxvW5z33OjEaj5lNPPWXu27fP+erp6XGOOfY93nLLLeajjz5qvvbaa+bWrVvNq666yqyurjZffvllL97CuP7xH//RfOqpp8zdu3ebzzzzjLl8+XJzypQp5sGDB03TDP71syUSCXP27Nnml7/85RGPBe36dXZ2ms8//7z5/PPPm5LM2267zXz++eedWTXf+MY3zKamJvOXv/yl+ec//9lctWqVeeKJJ5q9vb3OOT70oQ+Zd955p/PzRH/Hfnl/AwMD5qWXXmqecMIJ5gsvvDDsb7K/v3/M9zfR73mpjfceOzs7zS9+8Yvm5s2bzd27d5uPP/64+b73vc88+eSTzb6+PuccQb2Gtng8btbW1pp33XXXqOfw8zXM5nPhs5/9rDl79mzziSeeMJ977jlz2bJl5rJly4adZ/78+eb999/v/JzN324hCC4Z7rzzTnP27NlmJBIxlyxZYv7xj390HvvgBz9oXnvttcOO/8UvfmHOmzfPjEQi5mmnnWY+/PDDJW5x9iSN+vWjH/3IOebY93jjjTc6/x7Tp083P/zhD5vbtm0rfeOzsHr1avP44483I5GIOWvWLHP16tXmq6++6jwe9Otne/TRR01J5s6dO0c8FrTr9+STT476O2m/h2QyaX71q181p0+fblZVVZkXXnjhiPc9Z84cc926dcPuG+/vuJTGe3+7d+8e82/yySefdM5x7Pub6Pe81MZ7jz09PeZFF11kTp061aysrDTnzJlj3nDDDSMCSFCvoe373/++WVNTY8ZisVHP4edrmM3nQm9vr/n5z3/enDRpkllbW2tefvnl5r59+0acJ/M52fztFsJIvSgAAIDvUeMCAAACg+ACAAACg+ACAAACg+ACAAACg+ACAAACg+ACAAACg+ACAAACg+ACAAACg+ACIPDmzp2r22+/3etmACgBgguAnFx33XW67LLLJEnnn3++brzxxpK99oYNG9TU1DTi/vb2dn36058uWTsAeKfC6wYAwMDAgCKRSN7Pnzp1qoutAeBn9LgAyMt1112nTZs26bvf/a4Mw5BhGHr99dclSS+99JJWrlyp+vp6TZ8+Xddcc40OHz7sPPf888/XmjVrdOONN2rKlClasWKFJOm2227TggULVFdXp+bmZn3+859XV1eXJOmpp57S9ddfr3g87rzezTffLGnkUNGbb76pVatWqb6+Xo2Njbryyit14MAB5/Gbb75ZZ555pn7yk59o7ty5ikajuuqqq9TZ2ekc81//9V9asGCBampqNHnyZC1fvlzd3d1F+tcEkC2CC4C8fPe739WyZct0ww03aN++fdq3b5+am5sVi8X0oQ99SGeddZaee+45PfLIIzpw4ICuvPLKYc+/5557FIlE9Mwzz+juu++WJIVCId1xxx16+eWXdc899+iJJ57Ql770JUnSOeeco9tvv12NjY3O633xi18c0a5kMqlVq1bpyJEj2rRpkx577DH99a9/1erVq4cd99prr+nBBx/UQw89pIceekibNm3SN77xDUnSvn37dPXVV+uTn/ykduzYoaeeekpXXHGF2JMW8B5DRQDyEo1GFYlEVFtbqxkzZjj3//u//7vOOussff3rX3fuW79+vZqbm/WXv/xF8+bNkySdfPLJ+ta3vjXsnJn1MnPnztW//Mu/6LOf/ay+973vKRKJKBqNyjCMYa93rI0bN+rFF1/U7t271dzcLEn68Y9/rNNOO03t7e1avHixJCvgbNiwQQ0NDZKka665Rhs3btS//uu/at++fRoaGtIVV1yhOXPmSJIWLFhQwL8WALfQ4wLAVX/605/05JNPqr6+3vk65ZRTJFm9HLZFixaNeO7jjz+uCy+8ULNmzVJDQ4OuueYavfPOO+rp6cn69Xfs2KHm5mYntEhSS0uLmpqatGPHDue+uXPnOqFFko4//ngdPHhQkrRw4UJdeOGFWrBggT72sY/pBz/4gY4ePZr9PwKAoiG4AHBVV1eXLrnkEr3wwgvDvnbt2qXzzjvPOa6urm7Y815//XX9zd/8jc444wz993//t7Zu3aq2tjZJVvGu2yorK4f9bBiGksmkJCkcDuuxxx7Tb37zG7W0tOjOO+/U/PnztXv3btfbASA3BBcAeYtEIkokEsPue9/73qeXX35Zc+fO1Xvf+95hX8eGlUxbt25VMpnUd77zHb3//e/XvHnztHfv3glf71innnqq9uzZoz179jj3bd++XbFYTC0tLVm/N8MwdO655+qWW27R888/r0gkogceeCDr5wMoDoILgLzNnTtXzz77rF5//XUdPnxYyWRSra2tOnLkiK6++mq1t7frtdde06OPPqrrr79+3NDx3ve+V4ODg7rzzjv117/+VT/5yU+cot3M1+vq6tLGjRt1+PDhUYeQli9frgULFujjH/+4tm3bpi1btugTn/iEPvjBD+rss8/O6n09++yz+vrXv67nnntOb775pu6//34dOnRIp556am7/QABcR3ABkLcvfvGLCofDamlp0dSpU/Xmm29q5syZeuaZZ5RIJHTRRRdpwYIFuvHGG9XU1KRQaOz/5CxcuFC33XabvvnNb+r000/Xf/7nf+rWW28ddsw555yjz372s1q9erWmTp06orhXsnpKfvnLX2rSpEk677zztHz5cp100km69957s35fjY2Nevrpp/XhD39Y8+bN0z/90z/pO9/5jlauXJn9Pw6AojBM5vcBAICAoMcFAAAEBsEFAAAEBsEFAAAEBsEFAAAEBsEFAAAEBsEFAAAEBsEFAAAEBsEFAAAEBsEFAAAEBsEFAAAEBsEFAAAExv8P7e7cVeJMOB0AAAAASUVORK5CYII=",
                         "text/plain": [
                             "<Figure size 640x480 with 1 Axes>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 },
@@ -389,15 +404,15 @@
                     "output_type": "stream",
                     "text": [
                         "Parameters:\n"
                     ]
                 },
                 {
                     "data": {
-                        "image/png": "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\n",
+                        "image/png": "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",
                         "text/plain": [
                             "<Figure size 640x480 with 1 Axes>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 }
@@ -420,22 +435,22 @@
                 "plt.plot([evaluation.parameters for evaluation in results.history])\n",
                 "plt.xlabel(\"Iterations\")\n",
                 "plt.show()"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 9,
+            "execution_count": 10,
             "id": "807204bb",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
-                            "<h3>Version Information</h3><table><tr><th>Qiskit Software</th><th>Version</th></tr><tr><td><code>qiskit-terra</code></td><td>0.22.1</td></tr><tr><td><code>qiskit-aer</code></td><td>0.11.1</td></tr><tr><td><code>qiskit-ibmq-provider</code></td><td>0.19.2</td></tr><tr><td><code>qiskit</code></td><td>0.39.1</td></tr><tr><td><code>qiskit-nature</code></td><td>0.4.5</td></tr><tr><th>System information</th></tr><tr><td>Python version</td><td>3.9.13</td></tr><tr><td>Python compiler</td><td>Clang 12.0.0 </td></tr><tr><td>Python build</td><td>main, Aug 25 2022 18:29:29</td></tr><tr><td>OS</td><td>Darwin</td></tr><tr><td>CPUs</td><td>8</td></tr><tr><td>Memory (Gb)</td><td>32.0</td></tr><tr><td colspan='2'>Thu Nov 03 18:12:06 2022 CDT</td></tr></table>"
+                            "<h3>Version Information</h3><table><tr><th>Qiskit Software</th><th>Version</th></tr><tr><td><code>qiskit-terra</code></td><td>0.23.3</td></tr><tr><td><code>qiskit-aer</code></td><td>0.12.0</td></tr><tr><td><code>qiskit-ibmq-provider</code></td><td>0.20.2</td></tr><tr><td><code>qiskit-nature</code></td><td>0.5.2</td></tr><tr><th>System information</th></tr><tr><td>Python version</td><td>3.8.16</td></tr><tr><td>Python compiler</td><td>Clang 14.0.6 </td></tr><tr><td>Python build</td><td>default, Mar  1 2023 21:19:10</td></tr><tr><td>OS</td><td>Darwin</td></tr><tr><td>CPUs</td><td>8</td></tr><tr><td>Memory (Gb)</td><td>32.0</td></tr><tr><td colspan='2'>Fri May 05 13:47:24 2023 CDT</td></tr></table>"
                         ],
                         "text/plain": [
                             "<IPython.core.display.HTML object>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
@@ -478,13 +493,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.13"
+            "version": "3.8.16"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `circuit_knitting_toolbox-0.0.0/test/circuit_cutting/test_circuit_cutting.py` & `circuit-knitting-toolbox-0.1.0/test/circuit_cutting/test_circuit_cutting.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,25 +8,28 @@
 # Any modifications or derivative works of this code must retain this
 # copyright notice, and modified files need to carry a notice indicating
 # that they have been altered from the originals.
 
 """Tests for circuit_cutting package."""
 
 import unittest
+import importlib.util
 
 import numpy as np
 from qiskit import QuantumCircuit
 
 from circuit_knitting_toolbox.circuit_cutting.wire_cutting import (
     cut_circuit_wires,
     evaluate_subcircuits,
     reconstruct_full_distribution,
     verify,
 )
 
+cplex_available = importlib.util.find_spec("cplex") is not None
+
 
 class TestCircuitCutting(unittest.TestCase):
     def setUp(self):
         qc = QuantumCircuit(5)
         for i in range(5):
             qc.h(i)
         qc.cx(0, 1)
@@ -42,14 +45,15 @@
         qc.cx(2, 3)
         qc.ry(np.pi / 2, 4)
         for i in range(5):
             qc.h(i)
 
         self.circuit = qc
 
+    @unittest.skipIf(not cplex_available, "cplex is not installed")
     def test_circuit_cutting_automatic(self):
         qc = self.circuit
         cuts = cut_circuit_wires(
             circuit=qc,
             method="automatic",
             max_subcircuit_width=3,
             max_subcircuit_cuts=10,
```

### Comparing `circuit_knitting_toolbox-0.0.0/test/entanglement_forging/test_data/CH3_two_body.npy` & `circuit-knitting-toolbox-0.1.0/test/entanglement_forging/test_data/CH3_two_body.npy`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.0.0/test/entanglement_forging/test_data/CN_one_body.npy` & `circuit-knitting-toolbox-0.1.0/test/entanglement_forging/test_data/CN_one_body.npy`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.0.0/test/entanglement_forging/test_data/CN_two_body.npy` & `circuit-knitting-toolbox-0.1.0/test/entanglement_forging/test_data/CN_two_body.npy`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.0.0/test/entanglement_forging/test_data/O2_one_body.npy` & `circuit-knitting-toolbox-0.1.0/test/entanglement_forging/test_data/O2_one_body.npy`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.0.0/test/entanglement_forging/test_data/O2_two_body.npy` & `circuit-knitting-toolbox-0.1.0/test/entanglement_forging/test_data/O2_two_body.npy`

 * *Files identical despite different names*

### Comparing `circuit_knitting_toolbox-0.0.0/test/entanglement_forging/test_entanglement_forging_ground_state_solver.py` & `circuit-knitting-toolbox-0.1.0/test/entanglement_forging/test_entanglement_forging_ground_state_solver.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,56 +9,62 @@
 # copyright notice, and modified files need to carry a notice indicating
 # that they have been altered from the originals.
 
 """Tests for EntanglementForgingVQE module."""
 
 import unittest
 import numpy as np
+
 from qiskit.algorithms.optimizers import SPSA
 from qiskit.circuit.library import TwoLocal
-from qiskit_nature.drivers import Molecule
-from qiskit_nature.drivers.second_quantization import PySCFDriver
-from qiskit_nature.problems.second_quantization import ElectronicStructureProblem
+from qiskit_nature.units import DistanceUnit
+from qiskit_nature.second_q.drivers import PySCFDriver
+from qiskit_nature.second_q.problems import (
+    ElectronicBasis,
+)
+from qiskit_nature.second_q.formats import get_ao_to_mo_from_qcschema
 
 from circuit_knitting_toolbox.entanglement_forging import (
     EntanglementForgingAnsatz,
     EntanglementForgingGroundStateSolver,
 )
 
 
 class TestEntanglementForgingGroundStateSolver(unittest.TestCase):
     def setUp(self):
         # Hard-code some ansatz params/lambdas
         self.optimizer = SPSA(maxiter=0)
 
     def test_entanglement_forging_vqe_hydrogen(self):
         """Test of applying Entanglement Forged Solver to to compute the energy of a H2 molecule."""
-
-        # Specify molecule
-        molecule = Molecule(
-            geometry=[("H", [0.0, 0.0, 0.0]), ("H", [0.0, 0.0, 0.735])],
+        # Set up the ElectronicStructureProblem
+        driver = PySCFDriver(
+            atom="H .0 .0 .0; H .0 .0 0.735",
+            unit=DistanceUnit.ANGSTROM,
             charge=0,
-            multiplicity=1,
+            spin=0,
+            basis="sto3g",
         )
-
-        # Set up the ElectronicStructureProblem
-        driver = PySCFDriver.from_molecule(molecule)
-        problem = ElectronicStructureProblem(driver)
+        driver.run()
+        problem = driver.to_problem(basis=ElectronicBasis.AO)
+        qcschema = driver.to_qcschema()
+        mo_coeff = get_ao_to_mo_from_qcschema(qcschema).coefficients.alpha["+-"]
 
         # Specify the ansatz and bitstrings
         ansatz = EntanglementForgingAnsatz(
             circuit_u=TwoLocal(2, [], "cry", [[0, 1], [1, 0]], reps=1),
             bitstrings_u=[(1, 0), (0, 1)],
         )
 
         # Set up the entanglement forging vqe object
         solver = EntanglementForgingGroundStateSolver(
             ansatz=ansatz,
             optimizer=self.optimizer,
             initial_point=[0.0, np.pi / 2],
+            mo_coeff=mo_coeff,
         )
 
         # Solve for the ground state energy
         results = solver.solve(problem)
         ground_state_energy = results.groundenergy + results.energy_shift
 
         # Ensure ground state energy output is within tolerance
```

### Comparing `circuit_knitting_toolbox-0.0.0/test/entanglement_forging/test_entanglement_forging_knitter.py` & `circuit-knitting-toolbox-0.1.0/test/entanglement_forging/test_entanglement_forging_knitter.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,28 +12,25 @@
 """Tests for EntanglementForgingKnitter module."""
 
 import os
 import unittest
 import numpy as np
 from qiskit.circuit import Parameter, QuantumCircuit
 from qiskit.circuit.library import TwoLocal
-from qiskit_nature import settings
-from qiskit_nature.drivers import Molecule
-from qiskit_nature.drivers.second_quantization import PySCFDriver
-from qiskit_nature.problems.second_quantization import ElectronicStructureProblem
-
-settings.dict_aux_operators = True
+from qiskit_nature.second_q.drivers import PySCFDriver
+from qiskit_nature.second_q.problems import ElectronicStructureProblem, ElectronicBasis
+from qiskit_nature.second_q.hamiltonians import ElectronicEnergy
+from qiskit_nature.second_q.formats import get_ao_to_mo_from_qcschema
 
 from circuit_knitting_toolbox.entanglement_forging import (
     EntanglementForgingAnsatz,
     EntanglementForgingKnitter,
     cholesky_decomposition,
     convert_cholesky_operator,
 )
-from circuit_knitting_toolbox.utils import IntegralDriver
 
 
 class TestEntanglementForgingKnitter(unittest.TestCase):
     def setUp(self):
         self.energy_shift_h2 = 0.7199689944489797
 
         self.energy_shift_h2o = -61.37433060587931
@@ -74,38 +71,35 @@
         return ansatz
 
     def test_entanglement_forging_H2(self):
         """
         Test to apply Entanglement Forging to compute the energy of a H2 molecule,
         given the optimial ansatz parameters.
         """
-
-        # Specify molecule
-        molecule = Molecule(
-            geometry=[("H", [0.0, 0.0, 0.0]), ("H", [0.0, 0.0, 0.735])],
-            charge=0,
-            multiplicity=1,
-        )
-
         # Set up the ELectrionicStructureProblem
-        driver = PySCFDriver.from_molecule(molecule)
-        problem = ElectronicStructureProblem(driver)
+        driver = PySCFDriver("H 0.0 0.0 0.0; H 0.0 0.0 0.735")
+        driver.run()
+        problem = driver.to_problem(basis=ElectronicBasis.AO)
+        qcschema = driver.to_qcschema()
 
         # Specify the ansatz and bitstrings
         ansatz = EntanglementForgingAnsatz(
             circuit_u=TwoLocal(2, [], "cry", [[0, 1], [1, 0]], reps=1),
             bitstrings_u=[(1, 0), (0, 1), (1, 0)],
             bitstrings_v=[(1, 0), (0, 1), (0, 1)],
         )
 
         # Set up the forging knitter object
         forging_knitter = EntanglementForgingKnitter(ansatz)
 
         # Specify the decomposition method and get the forged operator
-        hamiltonian_terms, energy_shift = cholesky_decomposition(problem)
+        mo_coeff = get_ao_to_mo_from_qcschema(qcschema).coefficients.alpha["+-"]
+        hamiltonian_terms, energy_shift = cholesky_decomposition(
+            problem, mo_coeff=mo_coeff
+        )
         forged_hamiltonian = convert_cholesky_operator(hamiltonian_terms, ansatz)
 
         # Hard-coded optimal ansatz parameters
         ansatz_params = [0, 1.57079633]
 
         energy, _, _ = forging_knitter(ansatz_params, forged_hamiltonian)
 
@@ -122,25 +116,19 @@
         radius_2 = 0.958  # position for the second H atom
         thetas_in_deg = 104.478  # bond angles.
 
         h1_x = radius_1
         h2_x = radius_2 * np.cos(np.pi / 180 * thetas_in_deg)
         h2_y = radius_2 * np.sin(np.pi / 180 * thetas_in_deg)
 
-        molecule = Molecule(
-            geometry=[
-                ("O", [0.0, 0.0, 0.0]),
-                ("H", [h1_x, 0.0, 0.0]),
-                ("H", [h2_x, h2_y, 0.0]),
-            ],
-            charge=0,
-            multiplicity=1,
-        )
-        driver = PySCFDriver.from_molecule(molecule, basis="sto6g")
-        problem = ElectronicStructureProblem(driver)
+        molecule = f"O 0.0 0.0 0.0; H {h1_x} 0.0 0.0; H {h2_x} {h2_y} 0.0"
+        driver = PySCFDriver(molecule, basis="sto6g")
+        driver.run()
+        problem = driver.to_problem(basis=ElectronicBasis.AO)
+        qcschema = driver.to_qcschema()
 
         # solution
         orbitals_to_reduce = [0, 3]
         bitstrings = [
             (1, 1, 1, 1, 1, 0, 0),
             (1, 0, 1, 1, 1, 0, 1),
             (1, 0, 1, 1, 1, 1, 0),
@@ -175,16 +163,17 @@
         circuit.append(hop_gate.to_gate({theta: theta_4}), [3, 4])
 
         ansatz = EntanglementForgingAnsatz(
             circuit_u=circuit, bitstrings_u=reduced_bitstrings
         )
 
         # Specify the decomposition method and get the forged operator
+        mo_coeff = get_ao_to_mo_from_qcschema(qcschema).coefficients.alpha["+-"]
         hamiltonian_terms, energy_shift = cholesky_decomposition(
-            problem, orbitals_to_reduce=orbitals_to_reduce
+            problem, mo_coeff=mo_coeff, orbitals_to_reduce=orbitals_to_reduce
         )
         forged_hamiltonian = convert_cholesky_operator(hamiltonian_terms, ansatz)
 
         # Set up the forging knitter object
         forging_knitter = EntanglementForgingKnitter(ansatz)
 
         ansatz_params = [0.0, 0.0, 0.0, 0.0]
@@ -207,55 +196,46 @@
                 [
                     [[0.44744572, 0.3009177], [0.3009177, 0.44744572]],
                     [[0.57187698, 0.44744572], [0.44744572, 0.77460594]],
                 ],
             ]
         )
 
-        driver = IntegralDriver(
-            hcore=hcore,
-            mo_coeff=mo_coeff,
-            eri=eri,
-            num_alpha=1,
-            num_beta=1,
-            nuclear_repulsion_energy=0.7199689944489797,
-        )
-
-        problem = ElectronicStructureProblem(driver)
+        hamiltonian = ElectronicEnergy.from_raw_integrals(hcore, eri)
+        hamiltonian.nuclear_repulsion_energy = 0.7199689944489797
+        problem = ElectronicStructureProblem(hamiltonian)
+        problem.num_particles = (1, 1)
+        problem.basis = ElectronicBasis.AO
 
         ansatz = EntanglementForgingAnsatz(
             bitstrings_u=[(1, 0), (0, 1)],
             circuit_u=TwoLocal(2, [], "cry", [[0, 1], [1, 0]], reps=1),
         )
 
         # Specify the decomposition method and get the forged operator
-        hamiltonian_terms, energy_shift = cholesky_decomposition(problem)
+        hamiltonian_terms, energy_shift = cholesky_decomposition(
+            problem, mo_coeff=mo_coeff
+        )
         forged_hamiltonian = convert_cholesky_operator(hamiltonian_terms, ansatz)
 
         # Set up the forging knitter object
         forging_knitter = EntanglementForgingKnitter(ansatz)
         ansatz_params = [0.0, np.pi / 2]
 
         energy, _, _ = forging_knitter(ansatz_params, forged_hamiltonian)
 
         # Ensure ground state energy output is within tolerance
         self.assertAlmostEqual(energy + energy_shift, -1.1219365445030705)
 
     def test_asymmetric_bitstrings_O2(self):
         """Test for entanglement forging driver."""
-        driver = IntegralDriver(
-            hcore=self.hcore_o2,
-            mo_coeff=np.eye(8, 8),
-            eri=self.eri_o2,
-            num_alpha=6,
-            num_beta=6,
-            nuclear_repulsion_energy=self.energy_shift_o2,
-        )
-
-        problem = ElectronicStructureProblem(driver)
+        hamiltonian = ElectronicEnergy.from_raw_integrals(self.hcore_o2, self.eri_o2)
+        hamiltonian.nuclear_repulsion_energy = self.energy_shift_o2
+        problem = ElectronicStructureProblem(hamiltonian)
+        problem.num_particles = (6, 6)
 
         ansatz = EntanglementForgingAnsatz(
             circuit_u=self.create_mock_ansatz_circuit(8),
             bitstrings_u=[
                 (1, 1, 1, 1, 1, 1, 0, 0),
                 (1, 1, 1, 1, 1, 0, 1, 0),
                 (1, 1, 1, 1, 0, 1, 1, 0),
@@ -280,24 +260,18 @@
         energy, _, _ = forging_knitter(ansatz_params, forged_hamiltonian)
 
         # Ensure ground state energy output is within tolerance
         self.assertAlmostEqual(energy + energy_shift, -147.63645235088566)
 
     def test_asymmetric_bitstrings_CH3(self):
         """Test for entanglement forging driver."""
-        driver = IntegralDriver(
-            hcore=self.hcore_ch3,
-            mo_coeff=np.eye(6, 6),
-            eri=self.eri_ch3,
-            num_alpha=3,
-            num_beta=2,
-            nuclear_repulsion_energy=self.energy_shift_ch3,
-        )
-
-        problem = ElectronicStructureProblem(driver)
+        hamiltonian = ElectronicEnergy.from_raw_integrals(self.hcore_ch3, self.eri_ch3)
+        hamiltonian.nuclear_repulsion_energy = self.energy_shift_ch3
+        problem = ElectronicStructureProblem(hamiltonian)
+        problem.num_particles = (3, 2)
 
         ansatz = EntanglementForgingAnsatz(
             circuit_u=self.create_mock_ansatz_circuit(6),
             bitstrings_u=[
                 (1, 1, 1, 0, 0, 0),
                 (0, 1, 1, 0, 0, 1),
                 (1, 0, 1, 0, 1, 0),
@@ -324,24 +298,18 @@
         energy, _, _ = forging_knitter(ansatz_params, forged_hamiltonian)
 
         # Ensure ground state energy output is within tolerance
         self.assertAlmostEqual(energy + energy_shift, -39.09031477502881)
 
     def test_asymmetric_bitstrings_CN(self):
         """Test for asymmetric bitstrings with hybrid cross terms."""
-        driver = IntegralDriver(
-            hcore=self.hcore_cn,
-            mo_coeff=np.eye(8, 8),
-            eri=self.eri_cn,
-            num_alpha=5,
-            num_beta=4,
-            nuclear_repulsion_energy=self.energy_shift_cn,
-        )
-
-        problem = ElectronicStructureProblem(driver)
+        hamiltonian = ElectronicEnergy.from_raw_integrals(self.hcore_cn, self.eri_cn)
+        hamiltonian.nuclear_repulsion_energy = self.energy_shift_cn
+        problem = ElectronicStructureProblem(hamiltonian)
+        problem.num_particles = (5, 4)
 
         ansatz = EntanglementForgingAnsatz(
             circuit_u=self.create_mock_ansatz_circuit(8),
             bitstrings_u=[
                 (1, 1, 1, 1, 1, 0, 0, 0),
                 (1, 1, 1, 0, 1, 0, 1, 0),
                 (1, 1, 0, 1, 1, 1, 0, 0),
```

### Comparing `circuit_knitting_toolbox-0.0.0/tools/extremal_dependency_versions.py` & `circuit-knitting-toolbox-0.1.0/tools/extremal_dependency_versions.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import fire
 
 
 def mapfunc_dev(dep):
     """Load the development version(s) of certain Qiskit-related packages"""
     # https://peps.python.org/pep-0440/#direct-references
     return re.sub(
-        r"^(qiskit-(?:terra|nature|ibm-runtime)).*$",
+        r"^(qiskit-(?:terra|ibm-runtime)).*$",
         r"\1 @ git+https://github.com/Qiskit/\1.git",
         dep,
     )
 
 
 def mapfunc_min(dep):
     """Set each dependency to its minimum version"""
```

### Comparing `circuit_knitting_toolbox-0.0.0/PKG-INFO` & `circuit-knitting-toolbox-0.1.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,62 +1,82 @@
 Metadata-Version: 2.1
-Name: circuit_knitting_toolbox
-Version: 0.0.0
+Name: circuit-knitting-toolbox
+Version: 0.1.0
 Summary: A software prototype for a circuit knitting toolbox which connects user applications with runtime primitives
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Physics
-Requires-Dist: qiskit-aer>=0.11.0
-Requires-Dist: qiskit-terra>=0.22.0
-Requires-Dist: qiskit-nature>=0.4.4
-Requires-Dist: qiskit-ibm-runtime>=0.7.0
-Requires-Dist: qiskit-ibmq-provider>=0.19.2
-Requires-Dist: nptyping>=2.1.1
-Requires-Dist: docplex>=2.23.222
-Requires-Dist: cplex>=22.1.0.0; platform_machine != 'arm64'
-Requires-Dist: black[jupyter]==22.10.0 ; extra == "dev"
-Requires-Dist: mypy==0.982 ; extra == "dev"
-Requires-Dist: pytest>=6.2.5 ; extra == "dev"
-Requires-Dist: pydocstyle ; extra == "dev"
-Requires-Dist: pytest-randomly>=1.2.0 ; extra == "dev"
+Requires-Dist: qiskit-aer>=0.12.0
+Requires-Dist: qiskit-terra>=0.23.3
+Requires-Dist: qiskit-nature>=0.5.2
+Requires-Dist: qiskit-ibm-runtime>=0.9.2
+Requires-Dist: docplex>=2.23.222 ; extra == "cplex" and ( python_version < '3.11' and platform_machine != 'arm64')
+Requires-Dist: cplex>=22.1.0.0 ; extra == "cplex" and ( python_version < '3.11' and platform_machine != 'arm64')
+Requires-Dist: circuit-knitting-toolbox[test,lint] ; extra == "dev"
 Requires-Dist: nbmake ; extra == "dev"
-Requires-Dist: quantum-serverless>=0.0.1 ; extra == "notebook-dependencies"
-Requires-Dist: pyscf>=2.0.1 ; extra == "notebook-dependencies" and ( sys_platform != 'win32')
+Requires-Dist: Sphinx>=3.0.0 ; extra == "docs"
+Requires-Dist: sphinx-autodoc-typehints>=1.12.0 ; extra == "docs"
+Requires-Dist: jupyter-sphinx>=0.3.2 ; extra == "docs"
+Requires-Dist: nbsphinx>=0.8.8 ; extra == "docs"
+Requires-Dist: sphinx-copybutton>=0.5.0 ; extra == "docs"
+Requires-Dist: reno>=3.4.0 ; extra == "docs"
+Requires-Dist: circuit-knitting-toolbox[style] ; extra == "lint"
+Requires-Dist: pydocstyle==6.1.1 ; extra == "lint"
+Requires-Dist: mypy==0.982 ; extra == "lint"
+Requires-Dist: reno>=3.4.0 ; extra == "lint"
+Requires-Dist: toml ; extra == "lint"
+Requires-Dist: circuit-knitting-toolbox[cplex,pyscf] ; extra == "notebook-dependencies"
+Requires-Dist: quantum-serverless>=0.0.7 ; extra == "notebook-dependencies"
 Requires-Dist: matplotlib ; extra == "notebook-dependencies"
 Requires-Dist: ipywidgets ; extra == "notebook-dependencies"
 Requires-Dist: pylatexenc ; extra == "notebook-dependencies"
-Requires-Dist: pyscf>=2.0.1 ; extra == "test" and ( sys_platform != 'win32')
+Requires-Dist: qiskit-nature<0.6.0 ; extra == "notebook-dependencies"
+Requires-Dist: pyscf>=2.0.1 ; extra == "pyscf" and ( sys_platform != 'win32')
+Requires-Dist: autoflake==1.7.6 ; extra == "style"
+Requires-Dist: black[jupyter]==22.10.0 ; extra == "style"
+Requires-Dist: ruff>=0.0.246 ; extra == "style"
+Requires-Dist: circuit-knitting-toolbox[pyscf] ; extra == "test"
 Requires-Dist: pytest>=6.2.5 ; extra == "test"
 Requires-Dist: pytest-randomly>=1.2.0 ; extra == "test"
+Project-URL: Documentation, https://qiskit-extensions.github.io/circuit-knitting-toolbox/
+Project-URL: Repository, https://github.com/Qiskit-Extensions/circuit-knitting-toolbox
+Provides-Extra: cplex
 Provides-Extra: dev
+Provides-Extra: docs
+Provides-Extra: lint
 Provides-Extra: notebook-dependencies
+Provides-Extra: pyscf
+Provides-Extra: style
 Provides-Extra: test
 
 <!-- SHIELDS -->
 <div align="left">
 
-  [![Stability](https://img.shields.io/badge/Stability-alpha-f4d03f.svg)](https://github.com/Qiskit-Extensions/quantum-serverless/releases)
+  [![Stability](https://img.shields.io/badge/Stability-alpha-f4d03f.svg)](https://github.com/Qiskit-Extensions/circuit-knitting-toolbox/releases)
   ![Platform](https://img.shields.io/badge/Platform-Linux%20%7C%20macOS-informational)
-  [![Python](https://img.shields.io/badge/Python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10-informational)](https://www.python.org/)
-  [![Qiskit](https://img.shields.io/badge/Qiskit-%E2%89%A5%200.39.0-6133BD)](https://github.com/Qiskit/qiskit)
-  [![Qiskit Nature](https://img.shields.io/badge/Qiskit%20Nature-%E2%89%A5%200.4.4-6133BD)](https://github.com/Qiskit/qiskit-nature)
+  [![Python](https://img.shields.io/badge/Python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-informational)](https://www.python.org/)
+  [![Qiskit](https://img.shields.io/badge/Qiskit-%E2%89%A5%200.42.1-6133BD)](https://github.com/Qiskit/qiskit)
+  [![Qiskit Nature](https://img.shields.io/badge/Qiskit%20Nature-%E2%89%A5%200.5.2-6133BD)](https://github.com/Qiskit/qiskit-nature)
 <br />
-  [![License](https://img.shields.io/github/license/qiskit-community/prototype-entanglement-forging?label=License)](LICENSE.txt)
+  [![License](https://img.shields.io/github/license/Qiskit-Extensions/circuit-knitting-toolbox?label=License)](LICENSE.txt)
+  [![Code style: Black](https://img.shields.io/badge/Code%20style-Black-000.svg)](https://github.com/psf/black)
   [![Tests](https://github.com/Qiskit-Extensions/circuit-knitting-toolbox/actions/workflows/test_latest_versions.yml/badge.svg)](https://github.com/Qiskit-Extensions/circuit-knitting-toolbox/actions/workflows/test_latest_versions.yml)
+  [![Coverage](https://coveralls.io/repos/github/Qiskit-Extensions/circuit-knitting-toolbox/badge.svg?branch=main)](https://coveralls.io/github/Qiskit-Extensions/circuit-knitting-toolbox?branch=main)
 
 # Circuit Knitting Toolbox
 
 ### Table of Contents
 
 * [About](#about)
 * [Documentation](#documentation)
@@ -84,15 +104,15 @@
 
 The documentation, including installation instructions, is available at https://qiskit-extensions.github.io/circuit-knitting-toolbox/.
 
 ----------------------------------------------------------------------------------------------------
 
 ### Deprecation Policy
 
-This project is meant to evolve rapidly and, as such, does not follow [Qiskit's deprecation policy](https://qiskit.org/documentation/contributing_to_qiskit.html#deprecation-policy).  We may occasionally make breaking changes in order to improve the user experience.  When possible, we will keep old interfaces and mark them as deprecated, as long as they can co-exist with the new ones.  Each substantial improvement, breaking change, or deprecation will be documented in the release notes.
+This project is meant to evolve rapidly and, as such, does not follow [Qiskit's deprecation policy](https://qiskit.org/documentation/contributing_to_qiskit.html#deprecation-policy).  We may occasionally make breaking changes in order to improve the user experience.  When possible, we will keep old interfaces and mark them as deprecated, as long as they can co-exist with the new ones.  Each substantial improvement, breaking change, or deprecation will be documented in the [release notes](https://qiskit-extensions.github.io/circuit-knitting-toolbox/release-notes.html).
 
 ----------------------------------------------------------------------------------------------------
 
 ### References
 
 [1] Andrew Eddins, Mario Motta, Tanvi P. Gujarati, Sergey Bravyi, Antonio Mezzacapo, Charles Hadfield, Sarah Sheldon, [Doubling the size of quantum simulators by entanglement forging](https://journals.aps.org/prxquantum/abstract/10.1103/PRXQuantum.3.010309). PRX Quantum 3, 010309 (2022).
```

