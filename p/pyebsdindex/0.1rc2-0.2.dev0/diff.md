# Comparing `tmp/pyebsdindex-0.1rc2.tar.gz` & `tmp/pyebsdindex-0.2.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyebsdindex-0.1rc2.tar", last modified: Thu May 19 16:55:34 2022, max compression
+gzip compressed data, was "pyebsdindex-0.2.dev0.tar", last modified: Sat May  6 11:03:22 2023, max compression
```

## Comparing `pyebsdindex-0.1rc2.tar` & `pyebsdindex-0.2.dev0.tar`

### file list

```diff
@@ -1,48 +1,92 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-19 16:55:34.100075 pyebsdindex-0.1rc2/
--rw-r--r--   0 runner    (1001) docker     (121)     1596 2022-05-19 16:55:12.000000 pyebsdindex-0.1rc2/License
--rw-r--r--   0 runner    (1001) docker     (121)     5087 2022-05-19 16:55:34.100075 pyebsdindex-0.1rc2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3809 2022-05-19 16:55:12.000000 pyebsdindex-0.1rc2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-19 16:55:34.096075 pyebsdindex-0.1rc2/pyebsdindex/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-19 16:55:34.096075 pyebsdindex-0.1rc2/pyebsdindex/EBSDImage/
--rw-r--r--   0 runner    (1001) docker     (121)     6896 2022-05-19 16:55:12.000000 pyebsdindex-0.1rc2/pyebsdindex/EBSDImage/IPFcolor.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-19 16:55:12.000000 pyebsdindex-0.1rc2/pyebsdindex/EBSDImage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      302 2022-05-19 16:55:12.000000 pyebsdindex-0.1rc2/pyebsdindex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    19271 2022-05-19 16:55:12.000000 pyebsdindex-0.1rc2/pyebsdindex/band_detect.py
--rw-r--r--   0 runner    (1001) docker     (121)    34349 2022-05-19 16:55:12.000000 pyebsdindex-0.1rc2/pyebsdindex/band_vote.py
--rw-r--r--   0 runner    (1001) docker     (121)     3958 2022-05-19 16:55:12.000000 pyebsdindex-0.1rc2/pyebsdindex/crystal_sym.py
--rw-r--r--   0 runner    (1001) docker     (121)     9348 2022-05-19 16:55:12.000000 pyebsdindex-0.1rc2/pyebsdindex/crystallometry.py
--rw-r--r--   0 runner    (1001) docker     (121)    32148 2022-05-19 16:55:12.000000 pyebsdindex-0.1rc2/pyebsdindex/ebsd_index.py
--rw-r--r--   0 runner    (1001) docker     (121)    29048 2022-05-19 16:55:12.000000 pyebsdindex-0.1rc2/pyebsdindex/ebsd_pattern.py
--rw-r--r--   0 runner    (1001) docker     (121)    21581 2022-05-19 16:55:12.000000 pyebsdindex-0.1rc2/pyebsdindex/nlpar.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-19 16:55:34.096075 pyebsdindex-0.1rc2/pyebsdindex/opencl/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-19 16:55:12.000000 pyebsdindex-0.1rc2/pyebsdindex/opencl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    26665 2022-05-19 16:55:12.000000 pyebsdindex-0.1rc2/pyebsdindex/opencl/band_detect_cl.py
--rw-r--r--   0 runner    (1001) docker     (121)     3105 2022-05-19 16:55:12.000000 pyebsdindex-0.1rc2/pyebsdindex/opencl/openclparam.py
--rw-r--r--   0 runner    (1001) docker     (121)     6326 2022-05-19 16:55:12.000000 pyebsdindex-0.1rc2/pyebsdindex/opencl/radon_fast_cl.py
--rw-r--r--   0 runner    (1001) docker     (121)     9713 2022-05-19 16:55:12.000000 pyebsdindex-0.1rc2/pyebsdindex/pairlib.py
--rw-r--r--   0 runner    (1001) docker     (121)     7803 2022-05-19 16:55:12.000000 pyebsdindex-0.1rc2/pyebsdindex/pcopt.py
--rw-r--r--   0 runner    (1001) docker     (121)    11762 2022-05-19 16:55:12.000000 pyebsdindex-0.1rc2/pyebsdindex/radon_fast.py
--rw-r--r--   0 runner    (1001) docker     (121)    22234 2022-05-19 16:55:12.000000 pyebsdindex-0.1rc2/pyebsdindex/rotations.py
--rw-r--r--   0 runner    (1001) docker     (121)    51648 2022-05-19 16:55:12.000000 pyebsdindex-0.1rc2/pyebsdindex/rotlib.py
--rw-r--r--   0 runner    (1001) docker     (121)    11739 2022-05-19 16:55:12.000000 pyebsdindex-0.1rc2/pyebsdindex/spherical_radon_fast.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-19 16:55:34.100075 pyebsdindex-0.1rc2/pyebsdindex/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-19 16:55:12.000000 pyebsdindex-0.1rc2/pyebsdindex/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2318 2022-05-19 16:55:12.000000 pyebsdindex-0.1rc2/pyebsdindex/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-19 16:55:34.096075 pyebsdindex-0.1rc2/pyebsdindex/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-19 16:55:34.100075 pyebsdindex-0.1rc2/pyebsdindex/tests/data/al_sim_20kv/
--rw-r--r--   0 runner    (1001) docker     (121)    10569 2022-05-19 16:55:12.000000 pyebsdindex-0.1rc2/pyebsdindex/tests/data/al_sim_20kv/al_sim_20kv.png
--rw-r--r--   0 runner    (1001) docker     (121)     2279 2022-05-19 16:55:12.000000 pyebsdindex-0.1rc2/pyebsdindex/tests/numbatest.py
--rw-r--r--   0 runner    (1001) docker     (121)     2214 2022-05-19 16:55:12.000000 pyebsdindex-0.1rc2/pyebsdindex/tests/raytest.py
--rw-r--r--   0 runner    (1001) docker     (121)     6386 2022-05-19 16:55:12.000000 pyebsdindex-0.1rc2/pyebsdindex/tests/rotlibunittest.py
--rw-r--r--   0 runner    (1001) docker     (121)     3125 2022-05-19 16:55:12.000000 pyebsdindex-0.1rc2/pyebsdindex/tests/test_ebsd_index.py
--rw-r--r--   0 runner    (1001) docker     (121)     2589 2022-05-19 16:55:12.000000 pyebsdindex-0.1rc2/pyebsdindex/tests/test_pcopt.py
--rw-r--r--   0 runner    (1001) docker     (121)    10710 2022-05-19 16:55:12.000000 pyebsdindex-0.1rc2/pyebsdindex/tripletlib.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-19 16:55:34.096075 pyebsdindex-0.1rc2/pyebsdindex.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5087 2022-05-19 16:55:33.000000 pyebsdindex-0.1rc2/pyebsdindex.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1109 2022-05-19 16:55:34.000000 pyebsdindex-0.1rc2/pyebsdindex.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-19 16:55:33.000000 pyebsdindex-0.1rc2/pyebsdindex.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      355 2022-05-19 16:55:33.000000 pyebsdindex-0.1rc2/pyebsdindex.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-05-19 16:55:34.000000 pyebsdindex-0.1rc2/pyebsdindex.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-19 16:55:31.000000 pyebsdindex-0.1rc2/pyebsdindex.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       74 2022-05-19 16:55:34.100075 pyebsdindex-0.1rc2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2883 2022-05-19 16:55:12.000000 pyebsdindex-0.1rc2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 11:03:22.504583 pyebsdindex-0.2.dev0/
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    48700 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/IPFCubic.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    49952 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/IPFCubic.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/License
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-05-06 11:03:22.504583 pyebsdindex-0.2.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/RELEASE.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 11:03:22.488583 pyebsdindex-0.2.dev0/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/doc/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 11:03:22.488583 pyebsdindex-0.2.dev0/doc/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 11:03:22.492583 pyebsdindex-0.2.dev0/doc/_static/colormap_banners/
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/doc/_static/colormap_banners/banner0.png
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/doc/_static/colormap_banners/banner1.png
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/doc/_static/colormap_banners/create_colormap_banners.py
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/doc/_static/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 11:03:22.492583 pyebsdindex-0.2.dev0/doc/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 11:03:22.492583 pyebsdindex-0.2.dev0/doc/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/doc/_templates/autosummary/base.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/doc/_templates/custom-attribute-template.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/doc/_templates/custom-class-template.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/doc/_templates/custom-function-template.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/doc/_templates/custom-method-template.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/doc/_templates/custom-module-template.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/doc/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5926 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/doc/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 11:03:22.492583 pyebsdindex-0.2.dev0/doc/dev/
+-rw-r--r--   0 runner    (1001) docker     (123)     4304 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/doc/dev/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/doc/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/doc/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 11:03:22.492583 pyebsdindex-0.2.dev0/doc/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/doc/reference/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 11:03:22.496583 pyebsdindex-0.2.dev0/doc/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)     7282 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/doc/tutorials/NLPAR_demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   634518 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/doc/tutorials/ebsd_index_demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/doc/tutorials/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 11:03:22.496583 pyebsdindex-0.2.dev0/doc/user/
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/doc/user/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/doc/user/installation.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 11:03:22.500583 pyebsdindex-0.2.dev0/pyebsdindex/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 11:03:22.500583 pyebsdindex-0.2.dev0/pyebsdindex/EBSDImage/
+-rw-r--r--   0 runner    (1001) docker     (123)     6896 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/pyebsdindex/EBSDImage/IPFcolor.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/pyebsdindex/EBSDImage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/pyebsdindex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24999 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/pyebsdindex/_ebsd_index_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21731 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/pyebsdindex/_ebsd_index_single.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21899 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/pyebsdindex/band_detect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34349 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/pyebsdindex/band_vote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/pyebsdindex/crystal_sym.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9348 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/pyebsdindex/crystallometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/pyebsdindex/ebsd_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31299 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/pyebsdindex/ebsd_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/pyebsdindex/ebsdfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24576 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/pyebsdindex/nlpar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 11:03:22.500583 pyebsdindex-0.2.dev0/pyebsdindex/opencl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/pyebsdindex/opencl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26661 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/pyebsdindex/opencl/band_detect_cl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21518 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/pyebsdindex/opencl/clkernels.cl
+-rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/pyebsdindex/opencl/openclparam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6326 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/pyebsdindex/opencl/radon_fast_cl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9713 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/pyebsdindex/pairlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8801 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/pyebsdindex/pcopt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11762 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/pyebsdindex/radon_fast.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22234 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/pyebsdindex/rotations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51672 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/pyebsdindex/rotlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11739 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/pyebsdindex/spherical_radon_fast.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 11:03:22.504583 pyebsdindex-0.2.dev0/pyebsdindex/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/pyebsdindex/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/pyebsdindex/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 11:03:22.484583 pyebsdindex-0.2.dev0/pyebsdindex/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 11:03:22.504583 pyebsdindex-0.2.dev0/pyebsdindex/tests/data/al_sim_20kv/
+-rw-r--r--   0 runner    (1001) docker     (123)    10569 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/pyebsdindex/tests/data/al_sim_20kv/al_sim_20kv.png
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/pyebsdindex/tests/data/al_sim_20kv/generate_al_sim_20kv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/pyebsdindex/tests/numbatest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/pyebsdindex/tests/raytest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6386 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/pyebsdindex/tests/rotlibunittest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/pyebsdindex/tests/test_ebsd_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/pyebsdindex/tests/test_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/pyebsdindex/tests/test_pcopt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10790 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/pyebsdindex/tripletlib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 11:03:22.500583 pyebsdindex-0.2.dev0/pyebsdindex.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-05-06 11:03:22.000000 pyebsdindex-0.2.dev0/pyebsdindex.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-05-06 11:03:22.000000 pyebsdindex-0.2.dev0/pyebsdindex.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 11:03:22.000000 pyebsdindex-0.2.dev0/pyebsdindex.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-06 11:03:22.000000 pyebsdindex-0.2.dev0/pyebsdindex.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-06 11:03:22.000000 pyebsdindex-0.2.dev0/pyebsdindex.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 11:03:22.000000 pyebsdindex-0.2.dev0/pyebsdindex.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-06 11:03:22.504583 pyebsdindex-0.2.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/setup.py
```

### Comparing `pyebsdindex-0.1rc2/License` & `pyebsdindex-0.2.dev0/License`

 * *Files identical despite different names*

### Comparing `pyebsdindex-0.1rc2/pyebsdindex/EBSDImage/IPFcolor.py` & `pyebsdindex-0.2.dev0/pyebsdindex/EBSDImage/IPFcolor.py`

 * *Files identical despite different names*

### Comparing `pyebsdindex-0.1rc2/pyebsdindex/band_detect.py` & `pyebsdindex-0.2.dev0/pyebsdindex/band_detect.py`

 * *Files 15% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 from timeit import default_timer as timer
 
 import matplotlib.pyplot as plt
 import numba
 import numpy as np
 from scipy.ndimage import gaussian_filter
 from scipy.ndimage import grey_dilation as scipy_grey_dilation
+import scipy.optimize as opt
 
 from pyebsdindex import radon_fast
 
 
 tempdir = PurePath("/tmp" if platform.system() == "Darwin" else tempfile.gettempdir())
 tempdir = tempdir.joinpath('numba')
 environ["NUMBA_CACHE_DIR"] = str(tempdir)
@@ -221,17 +222,77 @@
       back = pat1 / float(len(stride))
       #pshape = pat1.shape
     # a bit of image processing.
     if back is not None:
       #if sigma is None:
        #sigma = 2.0 * float(pshape[-1]) / 80.0
       #back[0,:,:] = gaussian_filter(back[0,:,:], sigma = sigma )
-      back -= np.mean(back)
+      back = self.backsub_fit(back)
+      #back -= np.mean(back)
     self.backgroundsub = back
 
+  def backsub_fit(self, back):
+    # This function will fit a 2D gaussian on top of a plane to the averaged set of patterns (data) that is provided.
+    # It will automatically use whatever mask is defined for valid data.
+    # If the gaussian fit fails to converge, it will fall back to just using the mean set of patterns for the background
+    # with a warning.
+    def gaussian_surf(x, y, a, x0, y0, sigx, sigy, c, d, e):
+    # equation for 2D gaussian on top of a plane.
+      return a * np.exp(- ((x - x0) ** 2) / (2.0 * sigx ** 2) - ((y - y0) ** 2) / (2.0 * sigy ** 2)) + c + d * x + e * y
+
+    def fit_gauss(M, *args):
+    # helper function
+      x, y = M
+      #arr = np.zeros(x.shape)
+      return gaussian_surf(x, y, *args)
+
+    #back = np.mean(data, axis=0) # start with the mean of all the data
+    # now fit a 2D gaussian sitting on a plane.  See fuction def above.
+    nx = back.shape[-1]
+    ny = back.shape[-2]
+    #plt.imshow(back)
+    x = np.arange(nx, dtype=float)
+    x = (np.broadcast_to(x.reshape(1,nx), (ny, nx))).ravel()
+    y = np.arange(ny, dtype=float)
+    y = (np.broadcast_to(y, (nx, ny)).T).ravel()
+    # make a circular mask - even if not EDAX, this should work OK.
+    cx = (np.arange(nx) - nx*0.5)**2
+    cy = (np.arange(ny) - ny*0.5)**2
+    cmask = np.sqrt(np.broadcast_to(cx.reshape(1,nx), (ny, nx)) + np.broadcast_to(cy, (nx, ny)).T) < (ny*0.49)
+
+    # need to grab only the values that are in the mask.
+    wh = np.nonzero(cmask.ravel())[0]
+    xwh = x[wh]
+    ywh = y[wh]
+    xywh = np.vstack((xwh, ywh))
+    zwh = (back.ravel())[wh]
+    whmx = np.unravel_index(back.argmax(), back.shape)
+    minz = zwh.min()
+    # initialize a guess for the parameters.
+    # [gauss amplitude, max loc x, max loc y, sigx, sigy, const offset, slope x, slope y]
+    p0 = [(zwh.max() - zwh.min())*0.1, whmx[1], whmx[0], nx/2.355, ny/2.355, minz, 0, 0]
+    try:
+      popt, pcov = opt.curve_fit(fit_gauss, xywh, zwh, p0)
+      backfit = (gaussian_surf(x, y, *popt)).reshape(ny, nx)
+      #print(p0, popt)
+    except RuntimeError:
+      print('Warning: no convergence on back subtract ... using mean of the patterns.')
+      print('This may not be ideal for scans with few grains across the width of the scan.')
+      backfit = back
+    backfit -= np.mean(backfit)
+    #f, axarr = plt.subplots(1, 3)
+    #f.set_size_inches(10, 4)
+    #axarr[0].imshow(data[0,:,:].squeeze(), cmap='gray')
+    #axarr[1].imshow(data[0,:,:].squeeze() - backfit, cmap='gray')
+    #axarr[2].imshow(backfit, cmap='gray')
+
+
+    return backfit
+
+
   def find_bands(self, patternsIn, verbose=0, chunksize=-1,  **kwargs):
     tic0 = timer()
     tic = timer()
     ndim = patternsIn.ndim
     if ndim == 2:
       patterns = np.expand_dims(patternsIn, axis=0)
     else:
@@ -297,14 +358,16 @@
       im2show -= mean
       im2show /= stdv
       im2show = im2show.clip(-4, None)
       im2show += 6
       im2show[0:rhoMaskTrim,:] = 0
       im2show[-rhoMaskTrim:,:] = 0
       im2show = np.fliplr(im2show)
+
+      plt.figure()
       plt.imshow(im2show, cmap='gray', extent=[self.radonPlan.theta.min(), self.radonPlan.theta.max(),
                                                self.radonPlan.rho.min(), self.radonPlan.rho.max()],
                  interpolation='none', zorder=1, aspect='auto')
       width = bandData['width'][-1, :]
       width /= width.min()
       width *= 2
       xplt = np.squeeze(
@@ -314,15 +377,14 @@
 
       plt.scatter(y=yplt, x=xplt, c='r', s=width, zorder=2)
 
       for pt in range(self.nBands):
         plt.annotate(str(pt + 1), np.squeeze([xplt[pt], yplt[pt]]), color='yellow')
       plt.xlim(0,180)
       plt.ylim(-self.rhoMax, self.rhoMax)
-      plt.show()
 
 
     return bandData
 
   def radonPad(self,radon,rPad=0,tPad = 0, mirrorTheta = True):
     # function for padding the radon transform
     # theta padding (tPad) will use the symmetry of the radon and will vertical flip the transform and place it on
@@ -490,22 +552,24 @@
         nn /= sumnn
         bandData_avemax[q,i] = sumnn / nnN
         # rnn = np.sum(nn * (np.float32(r) + nnr))
         # cnn = np.sum(nn * (np.float32(c) + nnc))
         dx  = 0.5*(nn[1,2] - nn[1,0])
         dy  = 0.5*(nn[2,1] - nn[0,1])
         dxx = nn[1,2] + nn[1,0] - 2 * nn[1,1]
-        dyy = nn[2, 1] + nn[0, 2] - 2 * nn[1, 1]
+        dyy = nn[2,1] + nn[0,1] - 2 * nn[1,1]
         dxy = 0.25*(nn[2,2] - nn [0,2] - nn[2,0] + nn[0,0])
         #det = 1.0 / (dxx * dyy - dxy * dxy)
         det = (dxx * dyy - dxy * dxy)
         det = det if np.fabs(det) > 1e-12 else 1.0e-12
-        rnn = r - (dxx * dy - dxy * dx) * det
+        det = 1.0/det
         cnn = c - (dyy * dx - dxy * dy) * det
+        rnn = r - (dxx * dy - dxy * dx) * det
         bandData_aveloc[q,i,:] = np.array([rnn,cnn])
         bandData_valid[q,i] = 1
+
     return bandData_max,bandData_avemax,bandData_maxloc,bandData_aveloc, bandData_valid, bandData_width
 
 def getopenclparam(**kwargs): # dummy function to maintain compatability with openCL version
   return None
```

### Comparing `pyebsdindex-0.1rc2/pyebsdindex/band_vote.py` & `pyebsdindex-0.2.dev0/pyebsdindex/band_vote.py`

 * *Files identical despite different names*

### Comparing `pyebsdindex-0.1rc2/pyebsdindex/crystal_sym.py` & `pyebsdindex-0.2.dev0/pyebsdindex/crystal_sym.py`

 * *Files identical despite different names*

### Comparing `pyebsdindex-0.1rc2/pyebsdindex/crystallometry.py` & `pyebsdindex-0.2.dev0/pyebsdindex/crystallometry.py`

 * *Files identical despite different names*

### Comparing `pyebsdindex-0.1rc2/pyebsdindex/ebsd_index.py` & `pyebsdindex-0.2.dev0/pyebsdindex/_ebsd_index_parallel.py`

 * *Files 26% similar despite different names*

```diff
@@ -16,787 +16,621 @@
 # This software can be redistributed and/or modified freely provided that any derivative
 # works bear some notice that they are derived from it, and any modified versions bear
 # some notice that they have been modified.
 #
 # Author: David Rowenhorst;
 # The US Naval Research Laboratory Date: 21 Aug 2020
 
-"""Setup and handling of Hough indexing runs of EBSD patterns."""
+"""Setup and handling of Hough indexing runs of EBSD patterns in
+parallel.
+"""
 
 from os import path
 import multiprocessing
-
+import logging
 import sys
 import time
 from timeit import default_timer as timer
 
-import matplotlib.pyplot as plt
 import numpy as np
-import ray
 import h5py
+import ray
 
-from pyebsdindex import (
-    band_vote,
-    ebsd_pattern,
-    rotlib,
-    tripletlib
-)
-from pyebsdindex.EBSDImage import IPFcolor
+from pyebsdindex import ebsd_pattern, _pyopencl_installed
+from pyebsdindex._ebsd_index_single import EBSDIndexer, index_pats
 
-try:
+if _pyopencl_installed:
     from pyebsdindex.opencl import band_detect_cl as band_detect
-except ImportError:
+else:
     from pyebsdindex import band_detect as band_detect
 
 
-# if sys.platform == 'darwin':
-#   if ray.__version__ < '1.1.0':  # this fixes an issue when running locally on a VPN
-#     ray.services.get_node_ip_address = lambda: '127.0.0.1'
-#   else:
-#     ray._private.services.get_node_ip_address = lambda: '127.0.0.1'
-
-RADEG = 180.0 / np.pi
-
-
-def index_pats(patsIn=None,filename=None,filenameout=None,phaselist=['FCC'], \
-               vendor=None,PC=None,sampleTilt=70.0,camElev=5.3, \
-               bandDetectPlan=None,nRho=90,nTheta=180,tSigma=None,rSigma=None,rhoMaskFrac=0.1,nBands=9, \
-               backgroundSub=False,patstart=0,npats=-1, \
-               return_indexer_obj=False,ebsd_indexer_obj=None,clparams=None,verbose=0, chunksize = 528, gpu_id=None):
-
-  pats = None
-  if patsIn is None:
-    pdim = None
-  else:
-    if isinstance(patsIn,ebsd_pattern.EBSDPatterns):
-      pats = patsIn.patterns
-    if type(patsIn) is np.ndarray:
-      pats = patsIn
-    if isinstance(patsIn, h5py.Dataset):
-      shp = patsIn.shape
-      if len(shp) == 3:
-        pats = patsIn
-      if len(shp) == 2:  # just read off disk now.
-        pats = patsIn[()]
-        pats = pats.reshape(1, shp[0], shp[1])
+def index_pats_distributed(
+    patsin=None,
+    filename=None,
+    phaselist=["FCC"],
+    vendor=None,
+    PC=None,
+    sampleTilt=70.0,
+    camElev=5.3,
+    bandDetectPlan=None,
+    nRho=90,
+    nTheta=180,
+    tSigma=None,
+    rSigma=None,
+    rhoMaskFrac=0.1,
+    nBands=9,
+    patstart=0,
+    npats=-1,
+    chunksize=528,
+    ncpu=-1,
+    return_indexer_obj=False,
+    ebsd_indexer_obj=None,
+    keep_log=False,
+    gpu_id=None,
+):
+    """Index EBSD patterns in parallel.
+
+    Parameters
+    ----------
+    patsin : numpy.ndarray, optional
+        EBSD patterns in an array of shape (n points, n pattern
+        rows, n pattern columns). If not given, these are read from
+        ``filename``.
+    filename : str, optional
+        Name of file with EBSD patterns. If not given, ``patsin`` must
+        be passed.
+    phaselist : list of str, optional
+        Options are ``"FCC"`` and ``"BCC"``. Default is ``["FCC"]``.
+    vendor : str, optional
+        Which vendor convention to use for the pattern center (PC) and
+        the returned orientations. The available options are ``"EDAX"``
+        (default), ``"BRUKER"``, ``"OXFORD"``, ``"EMSOFT"``,
+        ``"KIKUCHIPY"``.
+    PC : list, optional
+        Pattern center (PCx, PCy, PCz) in the :attr:`indexer.vendor` or
+        ``vendor`` convention. For EDAX TSL, this is (x*, y*, z*),
+        defined in fractions of pattern width with respect to the lower
+        left corner of the detector. If not passed, this is set to (x*,
+        y*, z*) = (0.471659, 0.675044, 0.630139). If
+        ``vendor="EMSOFT"``, the PC must be four numbers, the final
+        number being the pixel size.
+    sampleTilt : float, optional
+        Sample tilt towards the detector in degrees. Default is 70
+        degrees. Unused if ``ebsd_indexer_obj`` is passed.
+    camElev : float, optional
+        Camera elevation in degrees. Default is 5.3 degrees. Unused
+        if ``ebsd_indexer_obj`` is passed.
+    bandDetectPlan : pyebsdindex.band_detect.BandDetect, optional
+        Collection of parameters using in band detection. Unused if
+        ``ebsd_indexer_obj`` is passed.
+    nRho : int, optional
+        Default is 90 degrees. Unused if ``ebsd_indexer_obj`` is
+        passed.
+    nTheta : int, optional
+        Default is 180 degrees. Unused if ``ebsd_indexer_obj`` is
+        passed.
+    tSigma : float, optional
+        Unused if ``ebsd_indexer_obj`` is passed.
+    rSigma : float, optional
+        Unused if ``ebsd_indexer_obj`` is passed.
+    rhoMaskFrac : float, optional
+        Default is 0.1. Unused if ``ebsd_indexer_obj`` is passed.
+    nBands : int, optional
+        Number of detected bands to use in triplet voting. Default
+        is 9. Unused if ``ebsd_indexer_obj`` is passed.
+    patstart : int, optional
+        Starting index of the patterns to index. Default is ``0``.
+    npats : int, optional
+        Number of patterns to index. Default is ``-1``, which will
+        index up to the final pattern in ``patsin``.
+    chunksize : int, optional
+        Default is 528.
+    ncpu : int, optional
+        Number of CPUs to use. Default value is ``-1``, meaning all
+        available CPUs will be used.
+    return_indexer_obj : bool, optional
+        Whether to return the EBSD indexer. Default is ``False``.
+    ebsd_indexer_obj : EBSDIndexer, optional
+        EBSD indexer. If not given, many of the above parameters must be
+        passed. Otherwise, these parameters are retrieved from this
+        indexer.
+    keep_log : bool, optional
+        Whether to keep the log. Default is ``False``.
+    gpu_id : int, optional
+        ID of GPU to use if :mod:`pyopencl` is installed.
+
+    Returns
+    -------
+    indxData : numpy.ndarray
+        Complex numpy array (or array of structured data), that is
+        [nphases + 1, npoints]. The data is stored for each phase used
+        in indexing and the ``indxData[-1]`` layer uses the best guess
+        on which is the most likely phase, based on the fit, and number
+        of bands matched for each phase. Each data entry contains the
+        orientation expressed as a quaternion (quat) (using the
+        convention of ``vendor`` or :attr:`indexer.vendor`), Pattern
+        Quality (pq), Confidence Metric (cm), Phase ID (phase), Fit
+        (fit) and Number of Bands Matched (nmatch). There are some other
+        metrics reported, but these are mostly for debugging purposes.
+    bandData : numpy.ndarray
+        Band identification data from the Radon transform.
+    indexer : EBSDIndexer
+        EBSD indexer, returned if ``return_indexer_obj=True``.
+
+    Notes
+    -----
+    Requires :mod:`ray[default]`. See the :doc:`installation guide
+    </user/installation>` for details.
+    """
+    pats = None
+    if patsin is None:
+        pdim = None
+    else:
+        if isinstance(patsin, ebsd_pattern.EBSDPatterns):
+            pats = patsin.patterns
+        if type(patsin) is np.ndarray:
+            pats = patsin
+        if isinstance(patsin, h5py.Dataset):
+            shp = patsin.shape
+            if len(shp) == 3:
+                pats = patsin
+            if len(shp) == 2:  # just read off disk now.
+                pats = patsin[()]
+                pats = pats.reshape(1, shp[0], shp[1])
+
+        if pats is None:
+            print("Unrecognized input data type")
+            return
+        pdim = pats.shape[-2:]
+
+    # run a test flight to make sure all parameters are set properly before being sent off to the cluster
+    if ebsd_indexer_obj is None:
+        indexer = EBSDIndexer(
+            filename=filename,
+            phaselist=phaselist,
+            vendor=vendor,
+            PC=PC,
+            sampleTilt=sampleTilt,
+            camElev=camElev,
+            bandDetectPlan=bandDetectPlan,
+            nRho=nRho,
+            nTheta=nTheta,
+            tSigma=tSigma,
+            rSigma=rSigma,
+            rhoMaskFrac=rhoMaskFrac,
+            nBands=nBands,
+            patDim=pdim,
+            gpu_id=gpu_id,
+        )
+    else:
+        indexer = ebsd_indexer_obj
 
-    if pats is None:
-      print('Unrecognized input data type')
-      return
-    pdim = pats.shape[-2:]
-
-
-  if ebsd_indexer_obj == None:
-    indexer = EBSDIndexer(filename=filename,phaselist=phaselist, \
-                          vendor=vendor,PC=PC,sampleTilt=sampleTilt,camElev=camElev, \
-                          bandDetectPlan=bandDetectPlan, \
-                          nRho=nRho,nTheta=nTheta,tSigma=tSigma,rSigma=rSigma,rhoMaskFrac=rhoMaskFrac,nBands=nBands,
-                          patDim=pdim, gpu_id=gpu_id)
-  else:
-    indexer = ebsd_indexer_obj
-
-  if filename is not None:
-    indexer.update_file(filename)
-  if pats is not None:
-    if not np.all(indexer.bandDetectPlan.patDim == np.array(pdim)):
-      indexer.update_file(patDim=pats.shape[-2:])
-
-  if backgroundSub == True:
-    indexer.bandDetectPlan.collect_background(fileobj=indexer.fID,patsIn=pats,nsample=1000)
-
-  dataout,banddata, indxstart,indxend = indexer.index_pats(patsin=pats,patstart=patstart,npats=npats, \
-                                                 clparams=clparams,verbose=verbose, chunksize = chunksize)
-
-  if return_indexer_obj == False:
-    return dataout, banddata
-  else:
-    return dataout,banddata, indexer
-
-def index_pats_distributed(patsIn=None,filename=None,filenameout=None,phaselist=['FCC'], \
-                           vendor=None,PC=None,sampleTilt=70.0,camElev=5.3, \
-                           peakDetectPlan=None,nRho=90,nTheta=180,tSigma=None,rSigma=None,rhoMaskFrac=0.1,nBands=9,
-                           patstart=0,npats=-1,chunksize=528,ncpu=-1,
-                           return_indexer_obj=False,ebsd_indexer_obj=None,keep_log=False, gpu_id=None):
-  pats = None
-  if patsIn is None:
-    pdim = None
-  else:
-    if isinstance(patsIn, ebsd_pattern.EBSDPatterns):
-      pats = patsIn.patterns
-    if type(patsIn) is np.ndarray:
-      pats = patsIn
-    if isinstance(patsIn, h5py.Dataset):
-      shp = patsIn.shape
-      if len(shp) == 3:
-        pats = patsIn
-      if len(shp) == 2:  # just read off disk now.
-        pats = patsIn[()]
-        pats = pats.reshape(1, shp[0], shp[1])
+    if filename is not None:
+        indexer.update_file(filename)
+    else:
+        indexer.update_file(patDim=pats.shape[-2:])
 
+    # Differentiate between getting a file to index or an array.
+    # Need to index one pattern to make sure the indexer object is fully
+    # initiated before placing in shared memory store.
+    mode = "memorymode"
     if pats is None:
-      print('Unrecognized input data type')
-      return
-    pdim = pats.shape[-2:]
-
-
-  # run a test flight to make sure all parameters are set properly before being sent off to the cluster
-  if ebsd_indexer_obj == None:
-    indexer = EBSDIndexer(filename=filename,phaselist=phaselist, \
-                          vendor=vendor,PC=PC,sampleTilt=sampleTilt,camElev=camElev, \
-                          bandDetectPlan=peakDetectPlan, \
-                          nRho=nRho,nTheta=nTheta,tSigma=tSigma,rSigma=rSigma,rhoMaskFrac=rhoMaskFrac,nBands=nBands,
-                          patDim=pdim, gpu_id=gpu_id)
-  else:
-    indexer = ebsd_indexer_obj
-
-  if filename is not None:
-    indexer.update_file(filename)
-  else:
-    indexer.update_file(patDim=pats.shape[-2:])
-
-  # differentiate between getting a file to index or an array
-  # Need to index one pattern to make sure the indexer object is fully initiated before
-  #   placing in shared memory store.
-  mode = 'memorymode'
-  if pats is None:
-    mode = 'filemode'
-    temp,temp2, indexer = index_pats(patstart=0,npats=1,return_indexer_obj=True,ebsd_indexer_obj=indexer)
-
-  if mode == 'filemode':
-    npatsTotal = indexer.fID.nPatterns
-  else:
-    pshape = pats.shape
-    if len(pshape) == 2:
-      npatsTotal = 1
-      pats = pats.reshape([1,pshape[0],pshape[1]])
-    else:
-      npatsTotal = pshape[0]
-    temp,temp2, indexer = index_pats(pats[0,:,:],patstart=0,npats=1,return_indexer_obj=True,ebsd_indexer_obj=indexer)
+        mode = "filemode"
+        temp, temp2, indexer = index_pats(
+            npats=1, return_indexer_obj=True, ebsd_indexer_obj=indexer
+        )
 
-  if patstart < 0:
-    patstart = npatsTotal - patstart
-  if npats <= 0:
-    npats = npatsTotal - patstart
-
-  # now set up the cluster with the indexer
-
-  n_cpu_nodes = int(multiprocessing.cpu_count())  # int(sum([ r['Resources']['CPU'] for r in ray.nodes()]))
-  if ncpu != -1:
-    n_cpu_nodes = ncpu
-
-  ngpu = None
-  if gpu_id is not None:
-    ngpu = np.atleast_1d(gpu_id).shape[0]
-
-  try:
-    clparam = band_detect.getopenclparam()
-    if clparam is None:
-      ngpu = 0
-      ngpupnode = 0
+    if mode == "filemode":
+        npatsTotal = indexer.fID.nPatterns
     else:
-      if ngpu is None:
-        ngpu = len(clparam.gpu)
-      ngpupnode = ngpu / n_cpu_nodes
-  except:
-    ngpu = 0
-    ngpupnode = 0
-
-  ray.shutdown()
-
-  print("num cpu/gpu:", n_cpu_nodes, ngpu)
-  #ray.init(num_cpus=n_cpu_nodes,num_gpus=ngpu,_system_config={"maximum_gcs_destroyed_actor_cached_count": n_cpu_nodes})
-  ray.init(num_cpus=n_cpu_nodes,num_gpus=ngpu, _node_ip_address="0.0.0.0")
-
-  # place indexer obj in shared memory store so all workers can use it.
-  remote_indexer = ray.put(indexer)
-  clparamfunction = band_detect.getopenclparam
-  # set up the jobs
-  njobs = (np.ceil(npats / chunksize)).astype(np.long)
-  # p_indx_start = [i*chunksize+patStart for i in range(njobs)]
-  # p_indx_end = [(i+1)*chunksize+patStart for i in range(njobs)]
-  # p_indx_end[-1] = npats+patStart
-  p_indx_start_end = [[i * chunksize + patstart,(i + 1) * chunksize + patstart,chunksize] for i in range(njobs)]
-  p_indx_start_end[-1][1] = npats + patstart
-  p_indx_start_end[-1][2] = p_indx_start_end[-1][1] - p_indx_start_end[-1][0]
-
-  if njobs < n_cpu_nodes:
-    n_cpu_nodes = njobs
-
-  nPhases = len(indexer.phaseLib)
-  dataout = np.zeros((nPhases + 1,npats),dtype=indexer.dataTemplate)
-  banddataout = np.zeros((npats, indexer.bandDetectPlan.nBands),dtype=indexer.bandDetectPlan.dataType)
-  ndone = 0
-  nsubmit = 0
-  tic0 = timer()
-  npatsdone = 0.0
-
-  if keep_log is True:
-    newline = '\n'
-  else:
-    newline = '\r'
-  if mode == 'filemode':
-    # send out the first batch
-    workers = []
-    jobs = []
-    timers = []
-    jobs_indx = []
-    chunkave = 0.0
-    for i in range(n_cpu_nodes):
-      job_pstart_end = p_indx_start_end.pop(0)
-      workers.append(IndexerRay.options(num_cpus=1,num_gpus=ngpupnode).remote(i, clparamfunction, gpu_id=gpu_id))
-      jobs.append(workers[i].index_chunk_ray.remote(pats=None,indexer=remote_indexer, \
-                                                    patstart=job_pstart_end[0],npats=job_pstart_end[2]))
-      nsubmit += 1
-      timers.append(timer())
-      time.sleep(0.01)
-      jobs_indx.append(job_pstart_end[:])
-
-    while ndone < njobs:
-      # toc = timer()
-      wrker,busy = ray.wait(jobs,num_returns=1,timeout=None)
-
-      # print("waittime: ",timer() - toc)
-      jid = jobs.index(wrker[0])
-      try:
-        wrkdataout,wrkbanddata, indxstr,indxend,rate = ray.get(wrker[0])
-      except:
-        # print('a death has occured')
-        indxstr = jobs_indx[jid][0]
-        indxend = jobs_indx[jid][1]
-        rate = [-1,-1]
-      if rate[0] >= 0:  # job finished as expected
-
-        ticp = timers[jid]
-        dataout[:,indxstr - patstart:indxend - patstart] = wrkdataout
-        banddataout[indxstr - patstart:indxend - patstart, :] = wrkbanddata
-        npatsdone += rate[1]
-        ndone += 1
-
-        ratetemp = n_cpu_nodes * (rate[1]) / (timer() - ticp)
-        chunkave += ratetemp
-        totalave = npatsdone / (timer() - tic0)
-        # print('Completed: ',str(indxstr),' -- ',str(indxend), '  ', npatsdone/(timer()-tic) )
-
-        toc0 = timer() - tic0
-        if keep_log is False:
-          print('                                                                                             ',
-                end='\r')
-          time.sleep(0.00001)
-        print('Completed: ',str(indxstr),' -- ',str(indxend),'  PPS:',"{:.0f}".format(ratetemp) + ';' +
-              "{:.0f}".format(chunkave / ndone) + ';' + "{:.0f}".format(totalave),
-              '  ',"{:.0f}".format((ndone / njobs) * 100) + '%',
-              "{:.0f};".format(toc0) + "{:.0f}".format((njobs - ndone) / ndone * toc0) + ' running;remaining(s)',
-              end=newline)
-
-        if len(p_indx_start_end) > 0:
-          job_pstart_end = p_indx_start_end.pop(0)
-          jobs[jid] = workers[jid].index_chunk_ray.remote(pats=None,indexer=remote_indexer,
-                                                          patstart=job_pstart_end[0],npats=job_pstart_end[2])
-          nsubmit += 1
-          timers[jid] = timer()
-          jobs_indx[jid] = job_pstart_end[:]
-        else:
-          del jobs[jid]
-          del workers[jid]
-          del timers[jid]
-          del jobs_indx[jid]
-
-      else:  # something bad happened.  Put the job back on the queue and kill this worker
-        p_indx_start_end.append([indxstr,indxend,indxend - indxstr])
-        del jobs[jid]
-        del workers[jid]
-        del timers[jid]
-        del jobs_indx[jid]
-        n_cpu_nodes -= 1
-        if len(workers) < 1:  # rare case that we have killed all workers...
-          job_pstart_end = p_indx_start_end.pop(0)
-          workers.append(IndexerRay.options(num_cpus=1,num_gpus=ngpupnode).remote(jid,clparamfunction,gpu_id))
-          jobs.append(workers[0].index_chunk_ray.remote(pats=None,indexer=remote_indexer, \
-                                                        patstart=job_pstart_end[0],npats=job_pstart_end[2]))
-          nsubmit += 1
-          timers.append(timer())
-          time.sleep(0.01)
-          jobs_indx.append(job_pstart_end[:])
-          n_cpu_nodes += 1
-
-  if mode == 'memorymode':
-    workers = []
-    jobs = []
-    timers = []
-    jobs_indx = []
-    chunkave = 0.0
-    for i in range(n_cpu_nodes):
-      job_pstart_end = p_indx_start_end.pop(0)
-      workers.append(IndexerRay.options(num_cpus=1,num_gpus=ngpupnode).remote(i,clparamfunction, gpu_id))
-      jobs.append(workers[i].index_chunk_ray.remote(pats=pats[job_pstart_end[0]:job_pstart_end[1],:,:],
-                                                    indexer=remote_indexer, \
-                                                    patstart=job_pstart_end[0],npats=job_pstart_end[2]))
-      nsubmit += 1
-      timers.append(timer())
-      jobs_indx.append(job_pstart_end)
-      time.sleep(0.01)
-
-    # workers = [index_chunk.remote(pats = None, indexer = remote_indexer, patStart = p_indx_start[i], patEnd = p_indx_end[i]) for i in range(n_cpu_nodes)]
-    # nsubmit += n_cpu_nodes
-
-    while ndone < njobs:
-      toc = timer()
-      wrker,busy = ray.wait(jobs,num_returns=1,timeout=None)
-      jid = jobs.index(wrker[0])
-      # print("waittime: ",timer() - toc)
-      try:
-        wrkdataout, wrkbanddata, indxstr, indxend, rate = ray.get(wrker[0])
-      except:
-        indxstr = jobs_indx[jid][0]
-        indxend = jobs_indx[jid][1]
-        rate = [-1,-1]
-      if rate[0] >= 0:
-        ticp = timers[jid]
-        dataout[:,indxstr - patstart:indxend - patstart] = wrkdataout
-        banddataout[indxstr - patstart:indxend - patstart, :] = wrkbanddata
-        npatsdone += rate[1]
-        ratetemp = n_cpu_nodes * (rate[1]) / (timer() - ticp)
-        chunkave += ratetemp
-        totalave = npatsdone / (timer() - tic0)
-        # print('Completed: ',str(indxstr),' -- ',str(indxend), '  ', npatsdone/(timer()-tic) )
-        ndone += 1
-        toc0 = timer() - tic0
-        if keep_log is False:
-          print('                                                                                             ',
-                end='\r')
-          time.sleep(0.0001)
-        print('Completed: ',str(indxstr),' -- ',str(indxend),'  PPS:',"{:.0f}".format(ratetemp) + ';' +
-              "{:.0f}".format(chunkave / ndone) + ';' + "{:.0f}".format(totalave),
-              '  ',"{:.0f}".format((ndone / njobs) * 100) + '%',
-              "{:.0f};".format(toc0) + "{:.0f}".format((njobs - ndone) / ndone * toc0) + ' running;remaining(s)',
-              end=newline)
-
-        if len(p_indx_start_end) > 0:
-          job_pstart_end = p_indx_start_end.pop(0)
-          jobs[jid] = workers[jid].index_chunk_ray.remote(pats=pats[job_pstart_end[0]:job_pstart_end[1],:,:]
-                                                          ,indexer=remote_indexer,
-                                                          patstart=job_pstart_end[0],npats=job_pstart_end[2])
-          nsubmit += 1
-          timers[jid] = timer()
-          jobs_indx[jid] = job_pstart_end
-        else:
-          del jobs[jid]
-          del workers[jid]
-          del timers[jid]
-          del jobs_indx[jid]
-      else:  # something bad happened.  Put the job back on the queue and kill this worker
-        p_indx_start_end.append([indxstr,indxend,indxend - indxstr])
-        del jobs[jid]
-        del workers[jid]
-        del timers[jid]
-        del jobs_indx[jid]
-        n_cpu_nodes -= 1
-        if len(workers) < 1:  # rare case that we have killed all workers...
-          job_pstart_end = p_indx_start_end.pop(0)
-          workers.append(IndexerRay.options(num_cpus=1,num_gpus=ngpupnode).remote(jid, clparamfunction, gpu_id))
-          jobs.append(workers[0].index_chunk_ray.remote(pats=pats[job_pstart_end[0]:job_pstart_end[1],:,:],
-                                                        indexer=remote_indexer, \
-                                                        patstart=job_pstart_end[0],npats=job_pstart_end[2]))
-          nsubmit += 1
-          timers.append(timer())
-          jobs_indx.append(job_pstart_end)
-          n_cpu_nodes += 1
-
-    del jobs
-    del workers
-    del timers
-    # # send out the first batch
-    # workers = [index_chunk_ray.remote(pats=pats[p_indx_start[i]:p_indx_end[i],:,:],indexer=remote_indexer,patStart=p_indx_start[i],patEnd=p_indx_end[i]) for i
-    #            in range(n_cpu_nodes)]
-    # nsubmit += n_cpu_nodes
-    #
-    # while ndone < njobs:
-    #   wrker,busy = ray.wait(workers,num_returns=1,timeout=None)
-    #   wrkdataout,indxstr,indxend, rate = ray.get(wrker[0])
-    #   dataout[indxstr:indxend] = wrkdataout
-    #   print('Completed: ',str(indxstr),' -- ',str(indxend))
-    #   workers.remove(wrker[0])
-    #   ndone += 1
-    #
-    #   if nsubmit < njobs:
-    #     workers.append(index_chunk_ray.remote(pats=pats[p_indx_start[nsubmit]:p_indx_end[nsubmit],:,:],indexer=remote_indexer,patStart=p_indx_start[nsubmit],
-    #                                       patEnd=p_indx_end[nsubmit]))
-    #     nsubmit += 1
-
-  ray.shutdown()
-  if return_indexer_obj:
-    return dataout,banddataout,indexer
-  else:
-    return dataout,banddataout
-
-@ray.remote(num_cpus=1,num_gpus=1)
-class IndexerRay():
-  def __init__(self,actorid=0, clparammodule=None, gpu_id=None):
-    sys.path.append((path.dirname(path.dirname(__file__))))  # do this to help Ray find the program files
-    # import openclparam # do this to help Ray find the program files
-    # device, context, queue, program, mf
-    # self.dataout = None
-    # self.indxstart = None
-    # self.indxend = None
-    # self.rate = None
-    self.actorID = actorid
-    self.openCLParams = None
-    self.useGPU = False
-    if clparammodule is not None:
-      try:
-        if sys.platform != 'darwin':  # linux with NVIDIA (unsure if it is the os or GPU type) is slow to make a
-          self.openCLParams = clparammodule()
-
-
-        else:  # MacOS handles GPU memory conflicts much better when the context is destroyed between each
-          # run, and has very low overhead for making the context.
-          #pass
-          self.openCLParams = clparammodule()
-          #self.openCLParams.gpu_id = 0
-          #self.openCLParams.gpu_id = 1
-          self.openCLParams.gpu_id = self.actorID % self.openCLParams.ngpu
-        if gpu_id is None:
-          gpu_id = np.arange(self.openCLParams.ngpu)
-        gpu_list = np.atleast_1d(gpu_id)
-        ngpu = gpu_list.shape[0]
-        self.openCLParams.gpu_id = gpu_list[self.actorID % ngpu]
-        self.openCLParams.get_queue()
-        self.useGPU = True
-      except:
-        self.openCLParams = None
+        pshape = pats.shape
+        if len(pshape) == 2:
+            npatsTotal = 1
+            pats = pats.reshape([1, pshape[0], pshape[1]])
+        else:
+            npatsTotal = pshape[0]
+        temp, temp2, indexer = index_pats(
+            pats[0, :, :],
+            npats=1,
+            return_indexer_obj=True,
+            ebsd_indexer_obj=indexer,
+        )
+
+    if patstart < 0:
+        patstart = npatsTotal - patstart
+    if npats <= 0:
+        npats = npatsTotal - patstart
+
+    # Now set up the cluster with the indexer
+    n_cpu_nodes = int(multiprocessing.cpu_count())
+    # int(sum([ r['Resources']['CPU'] for r in ray.nodes()]))
+    if ncpu != -1:
+        n_cpu_nodes = ncpu
+
+    ngpu = None
+    if gpu_id is not None:
+        ngpu = np.atleast_1d(gpu_id).shape[0]
 
-  def index_chunk_ray(self,pats=None,indexer=None,patstart=0,npats=-1):
     try:
-      #print(type(self.openCLParams.ctx))
-      tic = timer()
-      dataout,banddata, indxstart,npatsout = indexer.index_pats(patsin=pats,patstart=patstart,npats=npats,
-                                                      clparams=self.openCLParams, chunksize = -1)
-      rate = np.array([timer() - tic,npatsout])
-      return dataout,banddata, indxstart,indxstart + npatsout,rate
+        clparam = band_detect.getopenclparam()
+        if clparam is None:
+            ngpu = 0
+            ngpupnode = 0
+        else:
+            if ngpu is None:
+                ngpu = len(clparam.gpu)
+            ngpupnode = ngpu / n_cpu_nodes
     except:
-      indxstart = patstart
-      indxend = patstart + npats
-      return None,None, indxstart,indxend,[-1,-1]
-
-
-class EBSDIndexer:
-    """Setup of Hough indexing of EBSD patterns."""
-    def __init__(
-        self,
-        filename=None,
-        phaselist=['FCC'],
-        vendor=None,
-        PC=None,
-        sampleTilt=70.0,
-        camElev=5.3,
-        bandDetectPlan=None,
-        nRho=90,
-        nTheta=180,
-        tSigma=1.0,
-        rSigma=1.2,
-        rhoMaskFrac=0.15,
-        nBands=9,
-        patDim=None,
-        **kwargs
-    ):
-        """Create an EBSD indexer.
-
-        Parameters
-        ----------
-        filename : str, optional
-            Name of file with EBSD patterns.
-        phaselist : list of str, optional
-            Options are "FCC" and "BCC". Default is ["FCC"].
-        vendor : str, optional
-            This string determines the pattern center (PC) convention to
-            use. The available options are "EDAX" (default), "BRUKER",
-            "OXFORD", "EMSOFT", "KIKUCHIPY" (equivalent to "BRUKER").
-        PC : list, optional
-            Pattern center (PC) x*, y*, z* in EDAX TSL's convention,
-            defined in fractions of pattern width with respect to the
-            lower left corner of the detector. If not passed, this is
-            set to (x*, y*, z*) = (0.471659, 0.675044, 0.630139).
-        sampleTilt : float, optional
-            Sample tilt towards the detector in degrees. Default is 70
-            degrees. Unused if `ebsd_indexer_obj` is passed.
-        camElev : float, optional
-            Camera elevation in degrees. Default is 5.3 degrees. Unused
-            if `ebsd_indexer_obj` is passed.
-        bandDetectPlan : pyebsdindex.band_detect.BandDetect, optional
-            Collection of parameters using in band detection. Unused if
-            `ebsd_indexer_obj` is passed.
-        nRho : int, optional
-            Default is 90 degrees. Unused if `ebsd_indexer_obj` is passed.
-        nTheta : int, optional
-            Default is 180 degrees. Unused if `ebsd_indexer_obj` is passed.
-        tSigma : float, optional
-            Unused if `ebsd_indexer_obj` is passed.
-        rSigma : float, optional
-            Unused if `ebsd_indexer_obj` is passed.
-        rhoMaskFrac : float, optional
-            Default is 0.1. Unused if `ebsd_indexer_obj` is passed.
-        nBands : int, optional
-            Number of detected bands to use in triplet voting. Default
-            is 9. Unused if `ebsd_indexer_obj` is passed.
-        patDim : int, optional
-            Number of dimensions of pattern array.
-        kwargs
-            Keyword arguments passed on to `BandDetect`.
-
-        """
-        self.filein = filename
-        if self.filein is not None:
-            self.fID = ebsd_pattern.get_pattern_file_obj(self.filein)
-        else:
-            self.fID = None
-
-        # self.fileout = filenameout
-        # if self.fileout is None:
-        #     self.fileout = str.lower(Path(self.filein).stem)+'.ang'
-
-        self.phaselist = phaselist
-        self.phaseLib = []
-        for ph in self.phaselist:
-            self.phaseLib.append(band_vote.BandVote(tripletlib.triplib(libType=ph)))
-
-        self.vendor = 'EDAX'
-        if vendor is None:
-            if self.fID is not None:
-                self.vendor = self.fID.vendor
-        else:
-            self.vendor = vendor
-
-        if PC is None:
-            self.PC = np.array([0.471659, 0.675044, 0.630139])  # a default value
-        else:
-            self.PC = np.asarray(PC)
-
-        self.PCcorrectMethod = None
-        self.PCcorrectParam = None
-
-        self.sampleTilt = sampleTilt
-        self.camElev = camElev
+        ngpu = 0
+        ngpupnode = 0
 
-        if bandDetectPlan is None:
-            self.bandDetectPlan = band_detect.BandDetect(
-              nRho=nRho, nTheta=nTheta, tSigma=tSigma, rSigma=rSigma, rhoMaskFrac=rhoMaskFrac, nBands=nBands,
-              **kwargs)
-        else:
-            self.bandDetectPlan = bandDetectPlan
+    ray.shutdown()
 
-        if self.fID is not None:
-            self.bandDetectPlan.band_detect_setup(patDim=[self.fID.patternW, self.fID.patternH])
-        else:
-            if patDim is not None:
-                self.bandDetectPlan.band_detect_setup(patDim=patDim)
+    print("num cpu/gpu:", n_cpu_nodes, ngpu)
+    # ray.init(num_cpus=n_cpu_nodes,num_gpus=ngpu,_system_config={"maximum_gcs_destroyed_actor_cached_count": n_cpu_nodes})
+    # Need to append path for installs from source ... otherwise the ray
+    # workers do not know where to find the PyEBSDIndex module.
+    ray.init(
+        num_cpus=n_cpu_nodes,
+        num_gpus=ngpu,
+        _node_ip_address="0.0.0.0",
+        runtime_env={"env_vars": {"PYTHONPATH": path.dirname(path.dirname(__file__))}},
+        logging_level=logging.WARNING,
+    )  # Supress INFO messages from ray.
+
+    # Place indexer obj in shared memory store so all workers can use it
+    remote_indexer = ray.put(indexer)
+    # Get the function that will collect opencl parameters - if opencl
+    # is not installed, this is None, and the program will automatically
+    # fall back to CPU only calculation.
+    clparamfunction = band_detect.getopenclparam
+    # Set up the jobs
+    njobs = (np.ceil(npats / chunksize)).astype(np.compat.long)
+    # p_indx_start = [i*chunksize+patStart for i in range(njobs)]
+    # p_indx_end = [(i+1)*chunksize+patStart for i in range(njobs)]
+    # p_indx_end[-1] = npats+patStart
+    p_indx_start_end = [
+        [i * chunksize + patstart, (i + 1) * chunksize + patstart, chunksize]
+        for i in range(njobs)
+    ]
+    p_indx_start_end[-1][1] = npats + patstart
+    p_indx_start_end[-1][2] = p_indx_start_end[-1][1] - p_indx_start_end[-1][0]
+
+    if njobs < n_cpu_nodes:
+        n_cpu_nodes = njobs
+
+    nPhases = len(indexer.phaseLib)
+    dataout = np.zeros((nPhases + 1, npats), dtype=indexer.dataTemplate)
+    banddataout = np.zeros(
+        (npats, indexer.bandDetectPlan.nBands), dtype=indexer.bandDetectPlan.dataType
+    )
+    ndone = 0
+    nsubmit = 0
+    tic0 = timer()
+    npatsdone = 0.0
 
-        self.dataTemplate = np.dtype([
-            ('quat', np.float64, 4),
-            ('iq', np.float32),
-            ('pq', np.float32),
-            ('cm', np.float32),
-            ('phase', np.int32),
-            ('fit', np.float32),
-            ('nmatch', np.int32),
-            ('matchattempts', np.int32, 2),
-            ('totvotes', np.int32)
-        ])
-
-    def update_file(self, filename=None, patDim=np.array([120, 120], dtype=np.int32)):
-        if filename is None:
-            self.filein = None
-            self.bandDetectPlan.band_detect_setup(patDim=patDim)
-        else:
-            self.filein = filename
-            self.fID = ebsd_pattern.get_pattern_file_obj(self.filein)
-            self.bandDetectPlan.band_detect_setup(patDim=[self.fID.patternW, self.fID.patternH])
-
-    def index_pats(
-        self,
-        patsin=None,
-        patstart=0,
-        npats=-1,
-        clparams=None,
-        PC=[None, None, None],
-        verbose=0,
-        chunksize=528
-    ):
-        """Hough indexing of EBSD patterns.
-
-        Parameters
-        ----------
-        patsin : numpy.ndarray, optional
-            EBSD patterns in an array of shape (n points, n pattern
-            rows, n pattern columns). If not given, these are read from
-            `self.filename`.
-        patstart : int, optional
-            Starting index of the patterns to index. Default is 0.
-        npats : int, optional
-            Number of patterns to index. Default is -1, which will index
-            up to the final pattern in `patsin`.
-        clparams : list, optional
-            OpenCL parameters passed to pyopencl.
-        PC : list, optional
-            Pattern center (PC) (PCx, PCy, PCz) in `self.vendor`'s
-            convention (default is "EDAX"). If not given, this is read
-            from `self.PC`.
-        verbose : int, optional
-            0 - no output, 1 - timings, 2 - timings and the Hough
-            transform of the first pattern with detected bands
-            highlighted.
-        chunksize : int, optional
-            Default is 528.
-
-        Returns
-        -------
-        indxData : numpy.ndarray
-            Complex numpy array (or array of structured data), that is
-            [nphases + 1, npoints]. The data is stored for each phase
-            used in indexing and the `indxData[-1]` layer uses the best
-            guess on which is the most likely phase, based on the fit,
-            and number of bands matched for each phase. Each data entry
-            contains the orientation expressed as a quaternion (quat)
-            (using `self.vendor`'s convention), Pattern Quality (pq),
-            Confidence Metric (cm), Phase ID (phase), Fit (fit) and
-            Number of Bands Matched (nmatch). There are some other
-            metrics reported, but these are mostly for debugging
-            purposes.
-        bandData : numpy.ndarray
-            Band identification data from the Radon transform.
-        patstart : int
-            Starting index of the indexed patterns.
-        npats : int
-            Number of patterns indexed. This and `patstart` are useful
-            for the distributed indexing procedures.
-
-        """
-        tic = timer()
+    if keep_log is True:
+        newline = "\n"
+    else:
+        newline = "\r"
+    if mode == "filemode":
+        # Send out the first batch
+        workers = []
+        jobs = []
+        timers = []
+        jobs_indx = []
+        chunkave = 0.0
+        for i in range(n_cpu_nodes):
+            job_pstart_end = p_indx_start_end.pop(0)
+            workers.append(
+                IndexerRay.options(num_cpus=1, num_gpus=ngpupnode).remote(
+                    i, clparamfunction, gpu_id=gpu_id
+                )
+            )
+            jobs.append(
+                workers[i].index_chunk_ray.remote(
+                    pats=None,
+                    indexer=remote_indexer,
+                    patstart=job_pstart_end[0],
+                    npats=job_pstart_end[2],
+                )
+            )
+            nsubmit += 1
+            timers.append(timer())
+            time.sleep(0.01)
+            jobs_indx.append(job_pstart_end[:])
+
+        while ndone < njobs:
+            # toc = timer()
+            wrker, busy = ray.wait(jobs, num_returns=1, timeout=None)
+
+            # print("waittime: ",timer() - toc)
+            jid = jobs.index(wrker[0])
+            try:
+                wrkdataout, wrkbanddata, indxstr, indxend, rate = ray.get(wrker[0])
+            except:
+                # print('a death has occured')
+                indxstr = jobs_indx[jid][0]
+                indxend = jobs_indx[jid][1]
+                rate = [-1, -1]
+            if rate[0] >= 0:  # Job finished as expected
+
+                ticp = timers[jid]
+                dataout[:, indxstr - patstart : indxend - patstart] = wrkdataout
+                banddataout[indxstr - patstart : indxend - patstart, :] = wrkbanddata
+                npatsdone += rate[1]
+                ndone += 1
+
+                ratetemp = n_cpu_nodes * (rate[1]) / (timer() - ticp)
+                chunkave += ratetemp
+                totalave = npatsdone / (timer() - tic0)
+                # print('Completed: ',str(indxstr),' -- ',str(indxend), '  ', npatsdone/(timer()-tic) )
+
+                toc0 = timer() - tic0
+                if keep_log is False:
+                    print("", end="\r")
+                    time.sleep(0.00001)
+                print(
+                    "Completed: ",
+                    str(indxstr),
+                    " -- ",
+                    str(indxend),
+                    "  PPS:",
+                    "{:.0f}".format(ratetemp)
+                    + ";"
+                    + "{:.0f}".format(chunkave / ndone)
+                    + ";"
+                    + "{:.0f}".format(totalave),
+                    "  ",
+                    "{:.0f}".format((ndone / njobs) * 100) + "%",
+                    "{:.0f};".format(toc0)
+                    + "{:.0f}".format((njobs - ndone) / ndone * toc0)
+                    + " running;remaining(s)",
+                    end=newline,
+                )
 
-        if patsin is None:
-            pats = self.fID.read_data(returnArrayOnly=True, patStartCount=[patstart, npats], convertToFloat=True)
-        else:
-            pshape = patsin.shape
-            if len(pshape) == 2:
-                pats = np.reshape(patsin, (1, pshape[0], pshape[1]))
+                if len(p_indx_start_end) > 0:
+                    job_pstart_end = p_indx_start_end.pop(0)
+                    jobs[jid] = workers[jid].index_chunk_ray.remote(
+                        pats=None,
+                        indexer=remote_indexer,
+                        patstart=job_pstart_end[0],
+                        npats=job_pstart_end[2],
+                    )
+                    nsubmit += 1
+                    timers[jid] = timer()
+                    jobs_indx[jid] = job_pstart_end[:]
+                else:
+                    del jobs[jid]
+                    del workers[jid]
+                    del timers[jid]
+                    del jobs_indx[jid]
             else:
-                pats = patsin  # [patStart:patEnd, :,:]
-            pshape = pats.shape
+                # Something bad happened. Put the job back on the queue
+                # and kill this worker.
+                p_indx_start_end.append([indxstr, indxend, indxend - indxstr])
+                del jobs[jid]
+                del workers[jid]
+                del timers[jid]
+                del jobs_indx[jid]
+                n_cpu_nodes -= 1
+                if len(workers) < 1:  # Rare case that we have killed all workers...
+                    job_pstart_end = p_indx_start_end.pop(0)
+                    workers.append(
+                        IndexerRay.options(num_cpus=1, num_gpus=ngpupnode).remote(
+                            jid, clparamfunction, gpu_id
+                        )
+                    )
+                    jobs.append(
+                        workers[0].index_chunk_ray.remote(
+                            pats=None,
+                            indexer=remote_indexer,
+                            patstart=job_pstart_end[0],
+                            npats=job_pstart_end[2],
+                        )
+                    )
+                    nsubmit += 1
+                    timers.append(timer())
+                    time.sleep(0.01)
+                    jobs_indx.append(job_pstart_end[:])
+                    n_cpu_nodes += 1
+
+    if mode == "memorymode":
+        workers = []
+        jobs = []
+        timers = []
+        jobs_indx = []
+        chunkave = 0.0
+        for i in range(n_cpu_nodes):
+            job_pstart_end = p_indx_start_end.pop(0)
+            workers.append(
+                IndexerRay.options(num_cpus=1, num_gpus=ngpupnode).remote(
+                    i, clparamfunction, gpu_id
+                )
+            )
+            jobs.append(
+                workers[i].index_chunk_ray.remote(
+                    pats=pats[job_pstart_end[0] : job_pstart_end[1], :, :],
+                    indexer=remote_indexer,
+                    patstart=job_pstart_end[0],
+                    npats=job_pstart_end[2],
+                )
+            )
+            nsubmit += 1
+            timers.append(timer())
+            jobs_indx.append(job_pstart_end)
+            time.sleep(0.01)
+
+        # workers = [index_chunk.remote(pats = None, indexer = remote_indexer, patStart = p_indx_start[i], patEnd = p_indx_end[i]) for i in range(n_cpu_nodes)]
+        # nsubmit += n_cpu_nodes
+
+        while ndone < njobs:
+            # toc = timer()
+            wrker, busy = ray.wait(jobs, num_returns=1, timeout=None)
+            jid = jobs.index(wrker[0])
+            # print("waittime: ",timer() - toc)
+            try:
+                wrkdataout, wrkbanddata, indxstr, indxend, rate = ray.get(wrker[0])
+            except:
+                indxstr = jobs_indx[jid][0]
+                indxend = jobs_indx[jid][1]
+                rate = [-1, -1]
+            if rate[0] >= 0:
+                ticp = timers[jid]
+                dataout[:, indxstr - patstart : indxend - patstart] = wrkdataout
+                banddataout[indxstr - patstart : indxend - patstart, :] = wrkbanddata
+                npatsdone += rate[1]
+                ratetemp = n_cpu_nodes * (rate[1]) / (timer() - ticp)
+                chunkave += ratetemp
+                totalave = npatsdone / (timer() - tic0)
+                # print('Completed: ',str(indxstr),' -- ',str(indxend), '  ', npatsdone/(timer()-tic) )
+                ndone += 1
+                toc0 = timer() - tic0
+                if keep_log is False:
+                    print("", end="\r")
+                    time.sleep(0.0001)
+                print(
+                    "Completed: ",
+                    str(indxstr),
+                    " -- ",
+                    str(indxend),
+                    "  PPS:",
+                    "{:.0f}".format(ratetemp)
+                    + ";"
+                    + "{:.0f}".format(chunkave / ndone)
+                    + ";"
+                    + "{:.0f}".format(totalave),
+                    "  ",
+                    "{:.0f}".format((ndone / njobs) * 100) + "%",
+                    "{:.0f};".format(toc0)
+                    + "{:.0f}".format((njobs - ndone) / ndone * toc0)
+                    + " running;remaining(s)",
+                    end=newline,
+                )
 
-            if self.bandDetectPlan.patDim is None:
-                self.bandDetectPlan.band_detect_setup(patDim=pshape[1:3])
+                if len(p_indx_start_end) > 0:
+                    job_pstart_end = p_indx_start_end.pop(0)
+                    jobs[jid] = workers[jid].index_chunk_ray.remote(
+                        pats=pats[job_pstart_end[0] : job_pstart_end[1], :, :],
+                        indexer=remote_indexer,
+                        patstart=job_pstart_end[0],
+                        npats=job_pstart_end[2],
+                    )
+                    nsubmit += 1
+                    timers[jid] = timer()
+                    jobs_indx[jid] = job_pstart_end
+                else:
+                    del jobs[jid]
+                    del workers[jid]
+                    del timers[jid]
+                    del jobs_indx[jid]
             else:
-                if np.all((np.array(pshape[1:3]) - self.bandDetectPlan.patDim) == 0):
-                    self.bandDetectPlan.band_detect_setup(patDim=pshape[1:3])
+                # Something bad happened.  Put the job back on the queue
+                # and kill this worker.
+                p_indx_start_end.append([indxstr, indxend, indxend - indxstr])
+                del jobs[jid]
+                del workers[jid]
+                del timers[jid]
+                del jobs_indx[jid]
+                n_cpu_nodes -= 1
+                if len(workers) < 1:  # Rare case that we have killed all workers...
+                    job_pstart_end = p_indx_start_end.pop(0)
+                    workers.append(
+                        IndexerRay.options(num_cpus=1, num_gpus=ngpupnode).remote(
+                            jid, clparamfunction, gpu_id
+                        )
+                    )
+                    jobs.append(
+                        workers[0].index_chunk_ray.remote(
+                            pats=pats[job_pstart_end[0] : job_pstart_end[1], :, :],
+                            indexer=remote_indexer,
+                            patstart=job_pstart_end[0],
+                            npats=job_pstart_end[2],
+                        )
+                    )
+                    nsubmit += 1
+                    timers.append(timer())
+                    jobs_indx.append(job_pstart_end)
+                    n_cpu_nodes += 1
+
+        del jobs
+        del workers
+        del timers
+        # # send out the first batch
+        # workers = [index_chunk_ray.remote(pats=pats[p_indx_start[i]:p_indx_end[i],:,:],indexer=remote_indexer,patStart=p_indx_start[i],patEnd=p_indx_end[i]) for i
+        #            in range(n_cpu_nodes)]
+        # nsubmit += n_cpu_nodes
+        #
+        # while ndone < njobs:
+        #   wrker,busy = ray.wait(workers,num_returns=1,timeout=None)
+        #   wrkdataout,indxstr,indxend, rate = ray.get(wrker[0])
+        #   dataout[indxstr:indxend] = wrkdataout
+        #   print('Completed: ',str(indxstr),' -- ',str(indxend))
+        #   workers.remove(wrker[0])
+        #   ndone += 1
+        #
+        #   if nsubmit < njobs:
+        #     workers.append(index_chunk_ray.remote(pats=pats[p_indx_start[nsubmit]:p_indx_end[nsubmit],:,:],indexer=remote_indexer,patStart=p_indx_start[nsubmit],
+        #                                       patEnd=p_indx_end[nsubmit]))
+        #     nsubmit += 1
+
+    ray.shutdown()
+    if return_indexer_obj:
+        return dataout, banddataout, indexer
+    else:
+        return dataout, banddataout
 
-        if self.bandDetectPlan.patDim is None:
-            self.bandDetectPlan.band_detect_setup(patterns=pats)
 
-        npoints = pats.shape[0]
-        if npats == -1:
-            npats = npoints
-
-        # print(timer() - tic)
-        tic = timer()
-        bandData = self.bandDetectPlan.find_bands(pats, clparams=clparams, verbose=verbose, chunksize=chunksize)
-        shpBandDat = bandData.shape
-        if PC[0] is None:
-            PC_0 = self.PC
-        else:
-            PC_0 = PC
-        bandNorm = self.bandDetectPlan.radonPlan.radon2pole(bandData, PC=PC_0, vendor=self.vendor)
-        # print('Find Band: ', timer() - tic)
-
-        # return bandNorm,patStart,patEnd
-        tic = timer()
-        # bv = []
-        # for tl in self.phaseLib:
-        #  bv.append(band_vote.BandVote(tl))
-        nPhases = len(self.phaseLib)
-        q = np.zeros((nPhases, npoints, 4))
-        indxData = np.zeros((nPhases + 1, npoints), dtype=self.dataTemplate)
-
-        indxData['phase'] = -1
-        indxData['fit'] = 180.0
-        indxData['totvotes'] = 0
-        earlyexit = max(7, shpBandDat[1])
-        for i in range(npoints):
-            bandNorm1 = bandNorm[i, :, :]
-            bDat1 = bandData[i, :]
-            whgood = np.nonzero(bDat1['max'] > -1.0e6)[0]
-            if whgood.size >= 3:
-                bDat1 = bDat1[whgood]
-                bandNorm1 = bandNorm1[whgood, :]
-                indxData['pq'][0:nPhases, i] = np.sum(bDat1['max'], axis=0)
-
-                for j in range(len(self.phaseLib)):
-                  (
-                    avequat, fit, cm, bandmatch, nMatch, matchAttempts, totvotes
-                  ) = self.phaseLib[j].tripvote(bandNorm1, band_intensity = bDat1['avemax'], goNumba=True, verbose=verbose)
-                  # avequat,fit,cm,bandmatch,nMatch, matchAttempts = self.phaseLib[j].pairVoteOrientation(bandNorm1,goNumba=True)
-                  if nMatch >= 3:
-                      q[j, i, :] = avequat
-                      indxData['fit'][j, i] = fit
-                      indxData['cm'][j, i] = cm
-                      indxData['phase'][j, i] = j
-                      indxData['nmatch'][j, i] = nMatch
-                      indxData['matchattempts'][j, i] = matchAttempts
-                      indxData['totvotes'][j, i] = totvotes
-                  if nMatch >= earlyexit:
-                      break
-
-        qref2detect = self.refframe2detector()
-        q = q.reshape(nPhases * npoints, 4)
-        q = rotlib.quat_multiply(q, qref2detect)
-        q = rotlib.quatnorm(q)
-        q = q.reshape(nPhases, npoints, 4)
-        indxData['quat'][0:nPhases, :, :] = q
-        if nPhases > 1:
-            for j in range(nPhases - 1):
-                indxData[-1, :] = np.where(
-                    (indxData[j, :]['cm'] * indxData[j, :]['nmatch']) > (indxData[j + 1, :]['cm'] * indxData[j + 1, :]['nmatch']),
-                    indxData[j, :],
-                    indxData[j + 1, :]
-                )
-        else:
-          indxData[-1, :] = indxData[0, :]
-
-        if verbose > 0:
-            print('Band Vote Time: ', timer() - tic)
-        return indxData, bandData, patstart, npats
-
-    def refframe2detector(self):
-        ven = str.upper(self.vendor)
-        if ven in ['EDAX', 'EMSOFT', 'KIKUCHIPY']:
-            q0 = np.array([np.sqrt(2.0) * 0.5, 0.0, 0.0, -1.0 * np.sqrt(2.0) * 0.5])
-            tiltang = -1.0 * (90.0 - self.sampleTilt + self.camElev) / RADEG
-            q1 = np.array([np.cos(tiltang * 0.5), np.sin(tiltang * 0.5), 0.0, 0.0])
-            quatref2detect = rotlib.quat_multiply(q1, q0)
-
-        if ven in ['OXFORD', 'BRUKER']:
-            tiltang = -1.0 * (90.0 - self.sampleTilt + self.camElev) / RADEG
-            q1 = np.array([np.cos(tiltang * 0.5), np.sin(tiltang * 0.5), 0.0, 0.0])
-            quatref2detect = q1
-
-        return quatref2detect
-
-    def pcCorrect(self, xy=[[0.0, 0.0]]):  # at somepoint we will put some methods here for correcting the PC
-        # depending on the location within the scan.  Need to correct band_detect.radon2pole to accept a
-        # PC for each point
-        pass
-
-
-def __main__(file=None,ncpu=-1):
-  print('Hello')
-  if file is None:
-    file = '~/Desktop/SLMtest/scan2v3nlparl09sw7.up1'
-
-  dat1,indxer = index_pats(filename=file,
-                           patstart=0,npats=1,return_indexer_obj=True,
-                           nTheta=180,nRho=90,
-                           tSigma=1.0,rSigma=1.2,rhoMaskFrac=0.1,nBands=9, \
-                           phaselist=['FCC'])
-
-  dat = index_pats_distributed(filename=file,patstart=0,npats=-1,
-                               chunksize=1008,ncpu=ncpu,ebsd_indexer_obj=indxer)
-  imshape = (indxer.fID.nRows,indxer.fID.nCols)
-  ipfim = IPFcolor.ipf_color_cubic(dat['quat']).reshape(imshape[0],imshape[1],3);
-  plt.imshow(ipfim)
+@ray.remote(num_cpus=1, num_gpus=1)
+class IndexerRay:
+    def __init__(self, actorid=0, clparammodule=None, gpu_id=None):
+        # sys.path.append(path.dirname(path.dirname(__file__)))  # do this to help Ray find the program files
+        # import openclparam # do this to help Ray find the program files
+        # device, context, queue, program, mf
+        # self.dataout = None
+        # self.indxstart = None
+        # self.indxend = None
+        # self.rate = None
+        self.actorID = actorid
+        self.openCLParams = None
+        self.useGPU = False
+        if clparammodule is not None:
+            try:
+                if (
+                    sys.platform != "darwin"
+                ):  # linux with NVIDIA (unsure if it is the os or GPU type) is slow to make a
+                    self.openCLParams = clparammodule()
+                else:  # MacOS handles GPU memory conflicts much better when the context is destroyed between each
+                    # run, and has very low overhead for making the context.
+                    # pass
+                    self.openCLParams = clparammodule()
+                    # self.openCLParams.gpu_id = 0
+                    # self.openCLParams.gpu_id = 1
+                    self.openCLParams.gpu_id = self.actorID % self.openCLParams.ngpu
+                if gpu_id is None:
+                    gpu_id = np.arange(self.openCLParams.ngpu)
+                gpu_list = np.atleast_1d(gpu_id)
+                ngpu = gpu_list.shape[0]
+                self.openCLParams.gpu_id = gpu_list[self.actorID % ngpu]
+                self.openCLParams.get_queue()
+                self.useGPU = True
+            except:
+                self.openCLParams = None
+
+    def index_chunk_ray(self, pats=None, indexer=None, patstart=0, npats=-1):
+        try:
+            # print(type(self.openCLParams.ctx))
+            tic = timer()
+            dataout, banddata, indxstart, npatsout = indexer.index_pats(
+                patsin=pats,
+                patstart=patstart,
+                npats=npats,
+                clparams=self.openCLParams,
+                chunksize=-1,
+            )
+            rate = np.array([timer() - tic, npatsout])
+            return dataout, banddata, indxstart, indxstart + npatsout, rate
+        except:
+            indxstart = patstart
+            indxend = patstart + npats
+            return None, None, indxstart, indxend, [-1, -1]
```

### Comparing `pyebsdindex-0.1rc2/pyebsdindex/ebsd_pattern.py` & `pyebsdindex-0.2.dev0/pyebsdindex/ebsd_pattern.py`

 * *Files 3% similar despite different names*

```diff
@@ -61,25 +61,29 @@
     if hdf5path is None: #automatically chose the first data group
       ebsdfileobj.get_data_paths()
       ebsdfileobj.set_data_path(pathindex=0)
   if (ftype.upper() == 'H5'):
     ebsdfileobj = HDF5PatFile(path) # if the path variable is a list,
     # the second item is set to be the hdf5 path to the patterns.
     try:
-      f = h5py.File(Path(path).expanduser(),'r+')
+      f = h5py.File(Path(pathtemp[0]).expanduser(),'r+')
     except:
-      print("File Not Found:",str(Path(path)))
+      print("File Not Found:",str(Path(pathtemp[0])))
       return -1
 
     if 'Manufacture' in f.keys():
       vendor = str(f['Manufacture'][()][0])
       if vendor.upper() == 'EDAX':
         ebsdfileobj = EDAXOH5(path)
-      if vendor.upper() >= 'Bruker Nano':
+      if vendor.upper() >= 'BRUKER NANO':
         ebsdfileobj = BRUKERH5(path)
+    if 'manufacturer' in f.keys():
+      vendor = str((f['manufacturer'][()][0]).decode('UTF-8'))
+      if vendor >= 'kikuchipy':
+        ebsdfileobj = KIKUCHIPYH5(path)
     if ebsdfileobj.h5patdatpth is None: #automatically chose the first data group
       ebsdfileobj.get_data_paths()
       ebsdfileobj.set_data_path(pathindex=0)
   ebsdfileobj.read_header()
   return ebsdfileobj
 
 def pat_flt2int(patterns,typeout=None,method='clip',scalevalue=0.98,maxScale=None):
@@ -101,14 +105,15 @@
     pats = pats
 
   shp = pats.shape
   npats = shp[0]
   max = pats.max()
   min = pats.min()
   type = pats.dtype
+
   # make a guess if the bitdepth is not set
   if typeout is None:
     typeout = np.uint8
     if max > 258:
      typeout = np.uint16
 
   if (isinstance(typeout(0), np.floating )):
@@ -127,14 +132,15 @@
   if method=='clip':
     patsout[:,:,:] = pats.clip(minval, maxval).astype(dtype=typeout)
   elif method=='fullscale':
     temp = pats.astype(np.float32) - min
     if maxScale is None:
       maxScale = temp.max()
     temp *= scalevalue * maxval / maxScale
+    temp = temp.clip(0, maxval)
     temp = np.around(temp)
     patsout[:,:,:] = temp.astype(typeout)
   elif method=='scale': # here we assume that the min if not < 0 should not be scaled.
     temp = pats.astype(np.float32)
     if min < minval:
       temp += minval  - min
     if maxScale is None:
@@ -427,14 +433,15 @@
     if self.version == 1:
       dat = np.fromfile(f, dtype=np.uint32, count=3)
       self.patternW = dat[0]
       self.patternH = dat[1]
       self.filePos = dat[2]
       self.nPatterns = np.int((Path(self.filepath).expanduser().stat().st_size - 16) /
                               (self.patternW * self.patternH * (self.filedatatype(0).nbytes)))
+
     elif self.version >= 3:
       dat = np.fromfile(f, dtype=np.uint32, count=3)
       self.patternW = dat[0]
       self.patternH = dat[1]
       self.filePos = dat[2]
       self.extraPatterns = np.fromfile(f, dtype=np.uint8, count=1)[0]
       dat = np.fromfile(f, dtype=np.uint32, count=2)
@@ -585,41 +592,43 @@
         self.bitdepth = 8
 
 
 class HDF5PatFile(EBSDPatternFile):
   def __init__(self, path=None):
     filepath = None
     hdf5path = None
+    self.patternh5id = 'Pattern'  # the name used for the pattern dataset array in the h5 file.
     if path is not None:
       ptemp = np.atleast_1d(path)
       filepath = ptemp[0]
       if ptemp.size > 1:
         hdf5path = ptemp[1]
+        self.patternh5id = ''
     EBSDPatternFile.__init__(self, filepath)
     self.filetype = 'HDF5'
     self.vendor = 'PyEBSDIndex'
     # HDF only attributes
     self.h5datagroups = []  # there can be multiple scans in one h5 file.  Potential data groups will be stored here.
     self.h5othergrps = []  # and this is all the other stuff in the h5 that is not an EBSD pattern dataset.
     self.h5patdatpth = None
     self.set_filepath(path)
 
     self.filedatatype = np.uint8
     self.set_data_path(hdf5path) # This will be the h5 path to the patterns
 
-    self.patternh5id = 'Pattern' #the name used for the pattern dataset array in the h5 file.
+
 
   def set_filepath(self, path=None):
     if path is not None:
       ptemp = np.atleast_1d(path)
       self.filepath = Path(ptemp[0]).expanduser().resolve()
       if ptemp.size > 1:
         self.set_data_path(ptemp[1])
 
-  def set_data_path(self, datapath=None):
+  def set_data_path(self, datapath=None, **kwargs):
     if datapath is not None:
       self.h5patdatpth = datapath
 
   def get_data_paths(self, verbose=0):
     '''Based on the H5EBSD spec this will search for viable Pattern Datasets '''
     try:
       f = h5py.File(self.filepath,'r')
@@ -628,17 +637,18 @@
       return -1
     self.h5datagroups = []
     self.h5othergrps = []
     groupsets = list(f.keys())
     for grpset in groupsets:
       if isinstance(f[grpset],h5py.Group):
         if 'EBSD' in f[grpset]:
-          if self.patternh5id in f[grpset + '/EBSD/Data']:
-            if (grpset  not in self.h5datagroups):
-              self.h5datagroups.append(grpset)
+          if 'Data' in f[grpset + '/EBSD/']:
+            if self.patternh5id in f[grpset + '/EBSD/Data']:
+              if (grpset  not in self.h5datagroups):
+                self.h5datagroups.append(grpset)
       else:
         self.h5othergrps.append(grpset)
 
     if len(self.h5datagroups) < 1:
       print("No viable EBSD patterns found:",str(Path(self.filepath)))
       return -2
     else:
@@ -662,14 +672,15 @@
     patterndset = f[self.h5patdatpth]
     readpats = np.array(patterndset[int(patStart):int(patStart+nPatToRead), :, :])
     readpats = readpats.reshape(nPatToRead,self.patternH,self.patternW)
     f.close()
     return readpats
 
   def copy_file(self, newpath, **kwargs):
+    # oh - this is a mess!
     pathtemp = np.atleast_1d(newpath)
     fpath = Path(pathtemp[0]).expanduser().resolve()
     #print(pathtemp)
     hdf5path = None
     if pathtemp.size > 1:
       hdf5path = pathtemp[1]
     if hdf5path is None: # no hdf dataset path is specified -- just copy the whole file.
@@ -739,21 +750,21 @@
       self.filepath = path
 
     try:
       f = h5py.File(Path(self.filepath).expanduser(),'r')
     except:
       print("File Not Found:",str(Path(self.filepath)))
       return -1
-
-    dset = f[self.h5patdatpth]
-    shp = np.array(dset.shape)
-    self.patternW = shp[-1]
-    self.patternH = shp[-2]
-    self.nPatterns = shp[-3]
-    self.filedatatype = dset.dtype.type
+    if self.h5patdatpth is not None:
+      dset = f[self.h5patdatpth]
+      shp = np.array(dset.shape)
+      self.patternW = shp[-1]
+      self.patternH = shp[-2]
+      self.nPatterns = shp[-3]
+      self.filedatatype = dset.dtype.type
 
 class EDAXOH5(HDF5PatFile):
   def __init__(self, path=None):
     HDF5PatFile.__init__(self, path)
     self.vendor = 'EDAX'
     #EDAXOH5 only attributes
     self.filedatatype = None # np.uint8
@@ -802,14 +813,70 @@
       self.hexFlag = np.int32(headerpath['Grid Type'][()][0] == 'HexGrid')
 
       self.xStep = np.float32(headerpath['Step X'][()][0])
       self.yStep = np.float32(headerpath['Step Y'][()][0])
 
     return 0 #note this function uses multiple returns
 
+class KIKUCHIPYH5(HDF5PatFile):
+  def __init__(self, path=None):
+    HDF5PatFile.__init__(self, path)
+    self.vendor = 'kikuchipy'
+    #EDAXOH5 only attributes
+    self.filedatatype = None # np.uint8
+    self.patternh5id = 'patterns'
+    if self.filepath is not None:
+      self.get_data_paths()
+
+  def set_data_path(self, datapath=None, pathindex=0): #overloaded from parent - will default to first group.
+    if datapath is not None:
+      self.h5patdatpth = datapath
+    else:
+      if len(self.h5datagroups) > 0:
+        #self.activegroupid = pathindex
+        self.h5patdatpth = self.h5datagroups[pathindex] + '/EBSD/Data/' + self.patternh5id
+
+
+  def read_header(self, path=None):
+    if path is not None:
+      self.filepath = path
+
+    try:
+      f = h5py.File(Path(self.filepath).expanduser(),'r')
+    except:
+      print("File Not Found:",str(Path(self.filepath)))
+      return -1
+
+    self.version = str((f['version'][()][0]).decode('UTF-8'))
+
+    if self.version  >= '0.3.dev0':
+      ngrp = self.get_data_paths()
+      if ngrp <= 0:
+        f.close()
+        return -2 # no data groups with patterns found.
+      if self.h5patdatpth is None: # default to the first datagroup
+        self.set_data_path(pathindex=0)
+
+      dset = f[self.h5patdatpth]
+      shp = np.array(dset.shape)
+      self.patternW = shp[-1]
+      self.patternH = shp[-2]
+      self.nPatterns = shp[-3]
+      self.filedatatype = dset.dtype.type
+      headerpath = (f[self.h5patdatpth].parent.parent)["Header"]
+      self.nCols = np.int32(headerpath['n_columns'][()][0])
+      self.nRows = np.int32(headerpath['n_rows'][()][0])
+      self.hexFlag = np.int32(headerpath['grid_type'][()][0] == 'hexagonal')
+
+      self.xStep = np.float32(headerpath['step_x'][()][0])
+      self.yStep = np.float32(headerpath['step_y'][()][0])
+
+    return 0 #note this function uses multiple returns
+
+
 class BRUKERH5(HDF5PatFile):
   def __init__(self, path=None):
     HDF5PatFile.__init__(self, path)
     self.vendor = 'BRUKER'
     #EDAXOH5 only attributes
     self.filedatatype = None # np.uint8
     self.patternh5id = 'RawPatterns'
```

### Comparing `pyebsdindex-0.1rc2/pyebsdindex/nlpar.py` & `pyebsdindex-0.2.dev0/pyebsdindex/nlpar.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,44 +1,50 @@
-'''This software was developed by employees of the US Naval Research Laboratory (NRL), an
-agency of the Federal Government. Pursuant to title 17 section 105 of the United States
-Code, works of NRL employees are not subject to copyright protection, and this software
-is in the public domain. PyEBSDIndex is an experimental system. NRL assumes no
-responsibility whatsoever for its use by other parties, and makes no guarantees,
-expressed or implied, about its quality, reliability, or any other characteristic. We
-would appreciate acknowledgment if the software is used. To the extent that NRL may hold
-copyright in countries other than the United States, you are hereby granted the
-non-exclusive irrevocable and unconditional right to print, publish, prepare derivative
-works and distribute this software, in any medium, or authorize others to do so on your
-behalf, on a royalty-free basis throughout the world. You may improve, modify, and
-create derivative works of the software or any portion of the software, and you may copy
-and distribute such modifications or works. Modified works should carry a notice stating
-that you changed the software and should note the date and nature of any such change.
-Please explicitly acknowledge the US Naval Research Laboratory as the original source.
-This software can be redistributed and/or modified freely provided that any derivative
-works bear some notice that they are derived from it, and any modified versions bear
-some notice that they have been modified.
-
-Author: David Rowenhorst;
-The US Naval Research Laboratory Date: 21 Aug 2020'''
+# This software was developed by employees of the US Naval Research Laboratory (NRL), an
+# agency of the Federal Government. Pursuant to title 17 section 105 of the United States
+# Code, works of NRL employees are not subject to copyright protection, and this software
+# is in the public domain. PyEBSDIndex is an experimental system. NRL assumes no
+# responsibility whatsoever for its use by other parties, and makes no guarantees,
+# expressed or implied, about its quality, reliability, or any other characteristic. We
+# would appreciate acknowledgment if the software is used. To the extent that NRL may hold
+# copyright in countries other than the United States, you are hereby granted the
+# non-exclusive irrevocable and unconditional right to print, publish, prepare derivative
+# works and distribute this software, in any medium, or authorize others to do so on your
+# behalf, on a royalty-free basis throughout the world. You may improve, modify, and
+# create derivative works of the software or any portion of the software, and you may copy
+# and distribute such modifications or works. Modified works should carry a notice stating
+# that you changed the software and should note the date and nature of any such change.
+# Please explicitly acknowledge the US Naval Research Laboratory as the original source.
+# This software can be redistributed and/or modified freely provided that any derivative
+# works bear some notice that they are derived from it, and any modified versions bear
+# some notice that they have been modified.
+#
+# Author: David Rowenhorst;
+# The US Naval Research Laboratory Date: 21 Aug 2020
 
+"""Non-local pattern averaging and re-indexing (NLPAR)."""
 
 from pathlib import Path
 from timeit import default_timer as timer
 
 import numba
 import numpy as np
 import scipy.optimize as opt
 
 from pyebsdindex import ebsd_pattern
 
 #from os import environ
 #environ["NUMBA_CACHE_DIR"] = str(tempdir)
 
 
-class NLPAR():
+__all__ = [
+    "NLPAR",
+]
+
+
+class NLPAR:
   def __init__(self, filename=None,  lam=0.7, searchradius=3,dthresh=0.0, nrows = None, ncols = None):
     self.lam = lam
     self.searchradius = searchradius
     self.dthresh = dthresh
     self.filepath = None
     self.hdfdatapath = None
     self.filepathout = None
@@ -86,25 +92,29 @@
     #print(fpath, hdf5path)
     if fpath is not None: # the user has set an output file path.
       self.filepathout = Path(fpath).expanduser().resolve()
       self.hdfdatapathout =  hdf5path
       if patternfile.filetype != 'HDF5': #check that the input and output are not the same.
         pathok = self.filepathout.exists()
         if pathok:
-          pathok = self.filepathout.samefile(patternfile.filepath)
-        if pathok:
-          raise ValueError('Error: File input and output are exactly the same.')
-          return
+          pathok = not self.filepathout.samefile(patternfile.filepath)
+          if not pathok:
+            raise ValueError('Error: File input and output are exactly the same.')
+            return
 
         patternfile.copy_file([self.filepathout,self.hdfdatapathout] )
         return  # fpath and (maybe) hdf5 path were set manually.
       else: # this is a hdf5 file
-        #if self.filepathout.exists():
-        #  print([self.filepathout,self.hdfdatapathout])
-        patternfile.copy_file([self.filepathout, self.hdfdatapathout])
+        if self.hdfdatapathout is None:
+          patternfile.copy_file(self.filepathout)
+          self.hdfdatapathout = patternfile.h5patdatpth
+          return
+        else:
+          patternfile.copy_file([self.filepathout, self.hdfdatapathout])
+          return
 
     if patternfile is not None: # the user has set no path.
       hdf5path = None
       if patternfile.filetype == 'UP':
         p = Path(patternfile.filepath)
         appnd = "_NLPAR_l{:1.2f}".format(self.lam) + "sr{:d}".format(self.searchradius)
         newfilepath = str(p.parent / Path(p.stem + appnd + p.suffix))
@@ -124,30 +134,30 @@
         patternfile.copy_file([newfilepath])
         hdf5path = patternfile.h5patdatpth
 
       self.filepathout = newfilepath
       self.hdfdatapathout = hdf5path
       return
 
-  def getinfileobj(self, inout=True):
+  def getinfileobj(self):
     if self.filepath is not None:
       fID = ebsd_pattern.get_pattern_file_obj([self.filepath, self.hdfdatapath])
-      if self.nrows is None:
+      if fID.nRows is not None:
         self.nrows = fID.nRows
       else:
         fID.nRows = self.nrows
-      if self.ncols is None:
+      if fID.nCols is not None:
         self.ncols = fID.nCols
       else:
         fID.nCols = self.ncols
       return fID
     else:
       return None
 
-  def getoutfileobj(self, inout=True):
+  def getoutfileobj(self):
     if self.filepathout is not None:
       return ebsd_pattern.get_pattern_file_obj([self.filepathout, self.hdfdatapathout])
     else:
       return None
 
   def opt_lambda(self,chunksize=0,saturation_protect=True,automask=True, backsub = False,
                  target_weights=[0.5, 0.34, 0.25], dthresh=0.0, autoupdate=True):
@@ -214,70 +224,72 @@
       rowstartread = np.int64(j)
       rowend = min(j + chunksize + nn,nrows)
       rowcountread = np.int64(rowend - rowstartread)
       data = patternfile.read_data(patStartCount=[[0,rowstartread],[ncols,rowcountread]],
                                         convertToFloat=True,returnArrayOnly=True)
 
       shp = data.shape
-      data = data.reshape(shp[0],phw)
+
       if backsub is True:
-        back = np.mean(data, axis=0)
-        back -= np.mean(back)
-        data -= back
+        data = self.backsub(data)
+        #back = np.mean(data, axis=0)
+        #back -= np.mean(back)
+        #data -= back
+      data = data.reshape(shp[0], phw)
 
       rowstartcount = np.asarray([0,rowcountread],dtype=np.int64)
       sigchunk, (d2,n2, dij) = self.sigma_numba(data,nn,rowcountread,ncols,rowstartcount,colstartcount,indices,saturation_protect)
       tmp = (sigma[j:j + rowstartcount[1],:] < sigchunk).choose( sigchunk, sigma[j:j + rowstartcount[1],:])
       sigma[j:j + rowstartcount[1],:] = tmp
 
 
       d2norm(d2, n2, dij, sigchunk)
       lamopt_values_chnk = []
       for tw in target_weights:
         lam = 1.0
         lambopt1 = opt.minimize(loptfunc,lam,args=(d2,tw,dthresh),method='Nelder-Mead',
-                                bounds = [[0.0, 10.0]],options={'fatol': 0.0001})
+                                bounds = [[0.001, 10.0]],options={'fatol': 0.0001})
         lamopt_values_chnk.append(lambopt1['x'])
 
 
       lamopt_values.append(lamopt_values_chnk)
     lamopt_values = np.asarray(lamopt_values)
     print("Range of lambda values: ", np.mean(lamopt_values, axis = 0).flatten())
     print("Optimal Choice: ", np.median(np.mean(lamopt_values, axis = 0)))
     if autoupdate == True:
       self.lam = np.median(np.mean(lamopt_values, axis = 0))
     if self.sigma is None:
       self.sigma = sigma
 
-  def calcnlpar(self,chunksize=0,searchradius=None,lam = None,dthresh = None,saturation_protect=True,automask=True,
-                filepath=None,filepathout=None,reset_sigma=True,backsub = False):
+  def calcnlpar(self, chunksize=0, searchradius=None, lam = None, dthresh = None, saturation_protect=True, automask=True,
+                filename=None, fileout=None, reset_sigma=True, backsub = False, rescale = False):
 
     if lam is not None:
       self.lam = lam
 
     if dthresh is not None:
       self.dthresh = dthresh
 
     if searchradius is not None:
       self.searchradius = searchradius
 
     lam = np.float32(self.lam)
     dthresh = np.float32(self.dthresh)
     sr = np.int64(self.searchradius)
 
-    if filepath is not None:
-      self.setfile(filepath=filepath)
+    if filename is not None:
+      self.setfile(filepath=filename)
 
     if reset_sigma:
       self.sigma = None
 
     patternfile = self.getinfileobj()
 
     #if filepathout is not None:
-    self.setoutfile(patternfile, filepath=filepathout)
+    self.setoutfile(patternfile, filepath=fileout)
 
     patternfileout = self.getoutfileobj()
 
 
     nrows = np.int64(self.nrows)#np.int64(patternfile.nRows)
     ncols = np.int64(self.ncols)#np.int64(patternfile.nCols)
     if patternfileout.nCols is None:
@@ -318,33 +330,41 @@
     shpsigma = np.asarray(self.sigma).shape
     if (shpsigma[0] != nrows) and (shpsigma[1] != ncols):
       self.sigma = np.zeros((nrows,ncols),dtype=np.float32) + 1e24
       calcsigma = True
 
 
     sigma = np.asarray(self.sigma)
+    scalemethod = 'clip'
+    if rescale == True:
+      if np.issubdtype(patternfileout.filedatatype, np.integer):
+        mxval = np.iinfo(patternfileout.filedatatype).max
+        scalemethod = 'fullscale'
+      else: # not int, so no rescale.
+        rescale = False
 
     nthreadpos = numba.get_num_threads()
     #numba.set_num_threads(36)
     colstartcount = np.asarray([0,ncols],dtype=np.int64)
     print(lam, sr, dthresh)
+
     for j in range(0,nrows,chunksize):
       rowstartread = np.int64(max(0, j-sr))
       rowend = min(j + chunksize+sr,nrows)
       rowcountread = np.int64(rowend-rowstartread)
       data = patternfile.read_data(patStartCount = [[0,rowstartread], [ncols,rowcountread]],
                                         convertToFloat=True,returnArrayOnly=True)
 
       shpdata = data.shape
-      data = data.reshape(shpdata[0], phw)
 
       if backsub is True:
-        back = np.mean(data,axis=0)
-        back -= np.mean(back)
-        data -= back
+        data = self.backsub(data)
+
+
+      data = data.reshape(shpdata[0], phw)
 
       rowstartcount = np.asarray([0,rowcountread],dtype=np.int64)
       if calcsigma is True:
         sigchunk, tmp = self.sigma_numba(data,1,rowcountread,ncols,rowstartcount,colstartcount,indices,saturation_protect)
         del tmp
         tmp = (sigma[rowstartread:rowend,:] < sigchunk).choose(sigchunk,sigma[rowstartread:rowend,:])
         sigma[rowstartread:rowend,:] = tmp
@@ -355,14 +375,20 @@
       dataout = self.nlpar_nb(data,lam, sr, dthresh, sigchunk,
                               rowcountread,ncols,indices,saturation_protect)
 
       dataout = dataout.reshape(rowcountread, ncols, phw)
       dataout = dataout[j-rowstartread:, :, : ]
       shpout = dataout.shape
       dataout = dataout.reshape(shpout[0]*shpout[1], pheight, pwidth)
+      if rescale == True:
+        for i in range(dataout.shape[0]):
+          temp = dataout[i,:,:]
+          temp -= temp.min()
+          temp *= float(mxval)/temp.max()
+          dataout[i,:,:] = temp
 
       patternfileout.write_data(newpatterns=dataout,patStartCount = [[0,j], [ncols, shpout[0]]],
                                      flt2int='clip',scalevalue=1.0 )
       #self.patternfileout.write_data(newpatterns=dataout,patStartCount=[j*ncols,shpout[0]*shpout[1]],
       #                               flt2int='clip',scalevalue=1.0 )
       #return dataout
       #sigma[j:j+rowstartcount[1],:] += \
@@ -421,14 +447,71 @@
       sigchunk, temp = self.sigma_numba(data,nn, rowcountread,ncols,rowstartcount,colstartcount,indices,saturation_protect)
       dave += (timer() - dtic)
       sigma[j:j+rowstartcount[1],:] += \
         sigchunk[rowstartcount[0]:rowstartcount[0]+rowstartcount[1],:]
 
     return sigma
 
+  def backsub(self, data):
+    # This function will fit a 2D gaussian on top of a plane to the averaged set of patterns (data) that is provided.
+    # It will automatically use whatever mask is defined for valid data.
+    # If the gaussian fit fails to converge, it will fall back to just using the mean set of patterns for the background
+    # with a warning.
+
+
+    def gaussian_surf(x, y, a, x0, y0, sigx, sigy, c, d, e):
+    # equation for 2D gaussian on top of a plane.
+      return a * np.exp(- ((x - x0) ** 2) / (2.0 * sigx ** 2) - ((y - y0) ** 2) / (2.0 * sigy ** 2)) + c + d * x + e * y
+
+    def fit_gauss(M, *args):
+    # helper function
+      x, y = M
+      #arr = np.zeros(x.shape)
+      return gaussian_surf(x, y, *args)
+
+    back = np.mean(data, axis=0) # start with the mean of all the data
+    # now fit a 2D gaussian sitting on a plane.  See fuction def above.
+    nx = data.shape[-1]
+    ny = data.shape[-2]
+    x = np.arange(nx, dtype=float)
+    x = (np.broadcast_to(x.reshape(1,nx), (ny, nx)))
+    y = np.arange(ny, dtype=float)
+    y = (np.broadcast_to(y, (nx, ny)).T)
+    x = x.ravel()
+    y = y.ravel()
+
+    # need to grab only the values that are in the mask.
+    wh = np.nonzero(self.mask.ravel())[0]
+    xwh = x[wh]
+    ywh = y[wh]
+    xywh = np.vstack((xwh, ywh))
+    zwh = (back.ravel())[wh]
+    whmx = np.unravel_index(back.argmax(), back.shape)
+    minz = zwh.min()
+    # initialize a guess for the parameters.
+    # [gauss amplitude, max loc x, max loc y, sigx, sigy, const offset, slope x, slope y]
+    p0 = [(zwh.max() - zwh.min()), whmx[1], whmx[0], nx/2.355, ny/2.355, minz, 0, 0]
+    try:
+      popt, pcov = opt.curve_fit(fit_gauss, xywh, zwh, p0)
+      backfit = (gaussian_surf(x, y, *popt)).reshape(ny, nx)
+      #print(p0, popt)
+    except RuntimeError:
+      print('Warning: no convergence on back subtract ... using mean of the patterns.')
+      print('This may not be ideal for scans with few grains across the width of the scan.')
+      backfit = back
+    backfit -= np.mean(backfit)
+    #f, axarr = plt.subplots(1, 3)
+    #f.set_size_inches(10, 4)
+    #axarr[0].imshow(data[0,:,:].squeeze(), cmap='gray')
+    #axarr[1].imshow(data[0,:,:].squeeze() - backfit, cmap='gray')
+    #axarr[2].imshow(backfit, cmap='gray')
+
+    data -= backfit
+    return data
+
   @staticmethod
   def automask( h,w ):
     r = (min(h,w)*0.98*0.5)
     x = np.arange(w, dtype=np.float32)
     x = np.minimum(x , (w-x))
     x = x.reshape(1,w)
     y = np.arange(h, dtype=np.float32)
@@ -563,15 +646,15 @@
                 else:
                   d2 = np.float32(1e6)*n2
                 weights[counter] = d2
                 pairdict[pairid] = numba.float32(d2)
             counter += 1
         #print('________________')
         # end of window scanning
-        sum = np.float(0.0)
+        sum = np.float32(0.0)
         for i_nn in range(winsz):
 
           weights[i_nn] = np.maximum(weights[i_nn]-dthresh, numba.float32(0.0))
           weights[i_nn] = np.exp(-1.0 * weights[i_nn] * lam2)
           sum += weights[i_nn]
 
         for i_nn in range(winsz):
```

### Comparing `pyebsdindex-0.1rc2/pyebsdindex/opencl/band_detect_cl.py` & `pyebsdindex-0.2.dev0/pyebsdindex/opencl/band_detect_cl.py`

 * *Files 0% similar despite different names*

```diff
@@ -164,29 +164,29 @@
         im2show -= mean
         im2show /= stdv
         im2show = im2show.clip(-4, None)
         im2show += 6
         im2show[0:rhoMaskTrim,:] = 0
         im2show[-rhoMaskTrim:,:] = 0
         im2show = np.fliplr(im2show)
-        plt.imshow(im2show, cmap='gray', extent = [0, 180, -self.rhoMax, self.rhoMax],
-                   interpolation='none', zorder = 1, aspect='auto')
+        plt.figure()
+        plt.imshow(im2show, cmap='gray', extent=[0, 180, -self.rhoMax, self.rhoMax],
+                   interpolation='none', zorder=1, aspect='auto')
         width = bandData['width'][-1, :]
         width /= width.min()
         width *= 2
         xplt = np.squeeze(180.0 - np.interp(bandData['aveloc'][-1,:,1], np.arange(self.radonPlan.nTheta), self.radonPlan.theta))
         yplt = np.squeeze( -1.0 * np.interp(bandData['aveloc'][-1,:,0], np.arange(self.radonPlan.nRho), self.radonPlan.rho))
 
-        plt.scatter(y=yplt, x=xplt, c='r', s=width, zorder = 2)
+        plt.scatter(y=yplt, x=xplt, c='r', s=width, zorder=2)
 
         for pt in range(self.nBands):
           plt.annotate(str(pt + 1),np.squeeze([xplt[pt],yplt[pt]]), color='yellow')
         plt.xlim(0,180)
         plt.ylim(-self.rhoMax, self.rhoMax)
-        plt.show()
 
 
     except Exception as e: # something went wrong - try the CPU
       print(e)
       bandData = band_detect.BandDetect.find_bands(self, patternsIn, verbose=verbose, chunksize=-1, **kwargs)
 
     return bandData
```

### Comparing `pyebsdindex-0.1rc2/pyebsdindex/opencl/openclparam.py` & `pyebsdindex-0.2.dev0/pyebsdindex/opencl/openclparam.py`

 * *Files identical despite different names*

### Comparing `pyebsdindex-0.1rc2/pyebsdindex/opencl/radon_fast_cl.py` & `pyebsdindex-0.2.dev0/pyebsdindex/opencl/radon_fast_cl.py`

 * *Files identical despite different names*

### Comparing `pyebsdindex-0.1rc2/pyebsdindex/pairlib.py` & `pyebsdindex-0.2.dev0/pyebsdindex/pairlib.py`

 * *Files identical despite different names*

### Comparing `pyebsdindex-0.1rc2/pyebsdindex/pcopt.py` & `pyebsdindex-0.2.dev0/pyebsdindex/pcopt.py`

 * *Files 17% similar despite different names*

```diff
@@ -23,19 +23,26 @@
 """Optimization of the pattern center (PC) of EBSD patterns."""
 
 import numpy as np
 import pyswarms as pso
 import scipy.optimize as opt
 
 
+__all__ = [
+    "optimize",
+    "optimize_pso",
+]
+
 RADEG = 180.0 / np.pi
 
 
-def optfunction(PC_i, indexer, banddat):
-    band_norm = indexer.bandDetectPlan.radonPlan.radon2pole(banddat, PC=PC_i, vendor=indexer.vendor)
+def _optfunction(PC_i, indexer, banddat):
+    band_norm = indexer.bandDetectPlan.radonPlan.radon2pole(
+        banddat, PC=PC_i, vendor=indexer.vendor
+    )
     n_points = banddat.shape[0]
     n_averages = 0
     average_fit = 0
     phase = indexer.phaseLib[0]
 
     for i in range(n_points):
         band_norm1 = band_norm[i, :, :]
@@ -53,165 +60,190 @@
     else:
         average_fit /= n_averages
     return average_fit
 
 
 def optimize(pats, indexer, PC0=None, batch=False):
     """Optimize pattern center (PC) (PCx, PCy, PCz) in the convention
-    of the `indexer.vendor` (default is EDAX) with Nelder-Mead.
+    of the :attr:`indexer.vendor` with Nelder-Mead.
 
     Parameters
     ----------
     pats : numpy.ndarray
-        EBSD patterns.
+        EBSD pattern(s), of shape
+        ``(n detector rows, n detector columns)``,
+        or ``(n patterns, n detector rows, n detector columns)``.
     indexer : pyebsdindex.ebsd_index.EBSDIndexer
         EBSD indexer instance storing all relevant parameters for band
         detection.
     PC0 : list, optional
-        Initial guess of PC. If not given, `indexer.PC` is used.
+        Initial guess of PC. If not given, :attr:`indexer.PC` is used.
+        If :attr:`indexer.vendor` is ``"EMSOFT"``, the PC must be four
+        numbers, the final number being the pixel size.
     batch : bool, optional
-        Default is False which indicates the fit for a set of patterns
-        should be optimized using the cumulative fit for all the
-        patterns, and one PC will be returned.
-        If set to True, then a optimization is run for each individual
-        pattern, and an array of PC values will be returned.
+        Default is ``False`` which indicates the fit for a set of
+        patterns should be optimized using the cumulative fit for all
+        the patterns, and one PC will be returned. If ``True``, then an
+        optimization is run for each individual pattern, and an array of
+        PC values is returned.
 
     Returns
     -------
-    PCoutRet : numpy.ndarray
+    numpy.ndarray
         Optimized PC.
 
     Notes
     -----
     SciPy's Nelder-Mead minimization function is used with a tolerance
-    `fatol` of 0.00001 between each iteration.
-
+    ``fatol=0.00001`` between each iteration, ending the optimization
+    when the improvement is below this value.
     """
     banddat = indexer.bandDetectPlan.find_bands(pats)
-    npoints = banddat.shape[0]
+    npoints, nbands = banddat.shape[:2]
 
     if PC0 is None:
         PC0 = indexer.PC
     emsoftflag = False
-    if indexer.vendor == 'EMSOFT': # convert to EDAX for optimization
+    if indexer.vendor == "EMSOFT":  # Convert to EDAX for optimization
         emsoftflag = True
-        indexer.vendor = 'EDAX'
+        indexer.vendor = "EDAX"
         delta = indexer.PC
-        PC0in = PC0
         PCtemp = PC0[0:3]
         PCtemp[0] *= -1.0
         PCtemp[0] += 0.5 * indexer.bandDetectPlan.patDim[1]
         PCtemp[1] += 0.5 * indexer.bandDetectPlan.patDim[0]
         PCtemp /= indexer.bandDetectPlan.patDim[1]
         PCtemp[2] /= delta[3]
         PC0 = PCtemp
 
     if not batch:
-        PCopt = opt.minimize(optfunction, PC0, args=(indexer, banddat), method='Nelder-Mead', options={'fatol': 0.00001})
+        PCopt = opt.minimize(
+            _optfunction,
+            PC0,
+            args=(indexer, banddat),
+            method="Nelder-Mead",
+            options={"fatol": 0.00001}
+        )
         PCoutRet = PCopt['x']
     else:
         PCoutRet = np.zeros((npoints, 3))
         for i in range(npoints):
-            PCopt = opt.minimize(optfunction, PC0, args=(indexer, banddat[i, :, :]), method='Nelder-Mead')
+            PCopt = opt.minimize(
+                _optfunction,
+                PC0,
+                args=(indexer, banddat[i, :].reshape(1, nbands)),
+                method="Nelder-Mead"
+            )
             PCoutRet[i, :] = PCopt['x']
 
-    if emsoftflag == True: # return original state for indexer
-        indexer.vendor = 'EMSOFT'
+    if emsoftflag:  # Return original state for indexer
+        indexer.vendor = "EMSOFT"
         indexer.PC = delta
-        PC0 = PC0in
         if PCoutRet.ndim == 2:
             newout = np.zeros((npoints, 4))
             PCoutRet[:, 0] -= 0.5
-            PCoutRet[:, 0:3] *= indexer.bandDetectPlan.patDim[1]
+            PCoutRet[:, :3] *= indexer.bandDetectPlan.patDim[1]
             PCoutRet[:, 1] -= 0.5 * indexer.bandDetectPlan.patDim[0]
             PCoutRet[:, 0] *= -1.0
             PCoutRet[:, 2] *= delta[3]
-            newout[:, 0:3] = PCoutRet
+            newout[:, :3] = PCoutRet
             newout[:, 3] = delta[3]
             PCoutRet = newout
         else:
-            newout = np.zeros((4))
+            newout = np.zeros(4)
             PCoutRet[0] -= 0.5
-            PCoutRet[0:3] *= indexer.bandDetectPlan.patDim[1]
+            PCoutRet[:3] *= indexer.bandDetectPlan.patDim[1]
             PCoutRet[1] -= 0.5 * indexer.bandDetectPlan.patDim[0]
             PCoutRet[0] *= -1.0
             PCoutRet[2] *= delta[3]
-            newout[0:3] = PCoutRet
+            newout[:3] = PCoutRet
             newout[3] = delta[3]
             PCoutRet = newout
 
     return PCoutRet
 
 
 def optimize_pso(pats, indexer, PC0=None, batch=False):
     """Optimize pattern center (PC) (PCx, PCy, PCz) in the convention
-    of the `indexer.vendor` (default is EDAX) with particle swarms.
+    of the :attr:`indexer.vendor` with particle swarms.
 
     Parameters
     ----------
     pats : numpy.ndarray
-        EBSD patterns.
+        EBSD pattern(s), of shape
+        ``(n detector rows, n detector columns)``,
+        or ``(n patterns, n detector rows, n detector columns)``.
     indexer : pyebsdindex.ebsd_index.EBSDIndexer
         EBSD indexer instance storing all relevant parameters for band
         detection.
     PC0 : list, optional
-        Initial guess of PC. If not given, `indexer.PC` is used.
+        Initial guess of PC. If not given, :attr:`indexer.PC` is used.
+        If :attr:`indexer.vendor` is ``"EMSOFT"``, the PC must be four
+        numbers, the final number being the pixel size.
     batch : bool, optional
-        Default is False.
+        Default is ``False`` which indicates the fit for a set of
+        patterns should be optimized using the cumulative fit for all
+        the patterns, and one PC will be returned. If ``True``, then an
+        optimization is run for each individual pattern, and an array of
+        PC values is returned.
 
     Returns
     -------
-    PCoutRet : numpy.ndarray
+    numpy.ndarray
         Optimized PC.
 
     Notes
     -----
-    `pyswarms` particle swarm algorithm is used with 50 particles,
+    :mod:`pyswarms` particle swarm algorithm is used with 50 particles,
     bounds of +/- 0.05 on the PC values, and parameters c1 = 2.05, c2 =
     2.05 and w = 0.8.
-
     """
     banddat = indexer.bandDetectPlan.find_bands(pats)
     npoints = banddat.shape[0]
 
     if PC0 is None:
         PC0 = indexer.PC
     else:
         PC0 = np.asarray(PC0)
 
-    pso_options = {'c1': 2.05, 'c2': 2.05, 'w': 0.8}
-    bounds = (PC0 - 0.05, PC0 + 0.05)
-    optimizer = pso.single.GlobalBestPSO(n_particles=50, dimensions=3, options=pso_options, bounds=bounds)
+    optimizer = pso.single.GlobalBestPSO(
+        n_particles=50,
+        dimensions=3,
+        options={"c1": 2.05, "c2": 2.05, "w": 0.8},
+        bounds=(PC0 - 0.05, PC0 + 0.05),
+    )
 
     if not batch:
-        cost, PCopt = optimizer.optimize(optfunction, 1000, indexer=indexer, banddat=banddat)
-        PCoutRet = PCopt
+        cost, PCoutRet = optimizer.optimize(
+            _optfunction, 1000, indexer=indexer, banddat=banddat
+        )
         print(cost)
     else:
         PCoutRet = np.zeros((npoints, 3))
         for i in range(npoints):
-            cost, PCopt = optimizer.optimize(optfunction, 100, indexer=indexer, banddat=banddat[i, :, :])
-            PCoutRet[i, :] = PCopt
+            cost, PCoutRet[i, :] = optimizer.optimize(
+                _optfunction, 100, indexer=indexer, banddat=banddat[i, :, :]
+            )
     return PCoutRet
 
 
-def file_opt(fobj, indexer, stride=200, groupsz = 3):
+def _file_opt(fobj, indexer, stride=200, groupsz = 3):
     nCols = fobj.nCols
     nRows = fobj.nRows
-    #stride = 20
     pcopt = np.zeros((int(nRows / stride), int(nCols / stride), 3), dtype=np.float32)
 
     for i in range(int(nRows / stride)):
         ii = i * stride
         print(ii)
         for j in range(int(nCols / stride)):
             jj = j * stride
 
             pats = fobj.read_data(
-                returnArrayOnly=True, convertToFloat=True, patStartCount=[ii*nCols + jj, groupsz]
+                returnArrayOnly=True,
+                convertToFloat=True,
+                patStartCount=[ii*nCols + jj, groupsz]
             )
 
             pc = optimize(pats, indexer)
-            #print(pc, pc.shape)
             pcopt[i, j, :] = pc
 
     return pcopt
```

### Comparing `pyebsdindex-0.1rc2/pyebsdindex/radon_fast.py` & `pyebsdindex-0.2.dev0/pyebsdindex/radon_fast.py`

 * *Files identical despite different names*

### Comparing `pyebsdindex-0.1rc2/pyebsdindex/rotations.py` & `pyebsdindex-0.2.dev0/pyebsdindex/rotations.py`

 * *Files identical despite different names*

### Comparing `pyebsdindex-0.1rc2/pyebsdindex/rotlib.py` & `pyebsdindex-0.2.dev0/pyebsdindex/rotlib.py`

 * *Files 2% similar despite different names*

```diff
@@ -840,20 +840,20 @@
 
 
 @numba.jit(nopython=True,fastmath=nbFastmath,cache=nbcache, parallel=nbParallel)
 def ho2cuL(hoIn,p=P):
   pf = numba.float32(p > 0) * 2.0 - 1.0
   ho,m,n,intype = prepIn(hoIn)
   cu = np.zeros((n,3),dtype=intype)
-  LPR1 = np.float(1.33067003949147)  # (3pi/4)**(1/3)
-  LPpref = np.float(1.38197659788534)  # sqrt(6/pi)
-  LPbeta = np.float(0.962874509979126)  # pi**(5/6)/6**(1/6)/2
-  LPr2 = np.float(1.4142135623731)  # sqrt(2)
-  LPpi12 = np.float(0.261799387799149)  # pi/12
-  LPsc = np.float(0.897772786961286)  # a/ap == (pi**(5/6)/6**(1/6)) / pi**(2/3)
+  LPR1 = np.float64(1.33067003949147)  # (3pi/4)**(1/3)
+  LPpref = np.float64(1.38197659788534)  # sqrt(6/pi)
+  LPbeta = np.float64(0.962874509979126)  # pi**(5/6)/6**(1/6)/2
+  LPr2 = np.float64(1.4142135623731)  # sqrt(2)
+  LPpi12 = np.float64(0.261799387799149)  # pi/12
+  LPsc = np.float64(0.897772786961286)  # a/ap == (pi**(5/6)/6**(1/6)) / pi**(2/3)
   eps_loc = 1e-7
 
 
 
   for i in numba.prange(n):
     #cu[i,:] = lambert3DBallToCube(ho[i,:])
     # I have inlined all the function of lambert3DCubeToBall
@@ -1340,20 +1340,20 @@
     xyzba[1] = sXYZ[2]
     xyzba[2] = sXYZ[0]
   return xyzba
 
 
 @numba.jit(['f8[:](f8[:])','f8[:](f4[:])'], nopython=True,fastmath=nbFastmath, cache=nbcache)
 def lambert3DBallToCube(xyz):
-  LPR1 = np.float(1.33067003949147) # (3pi/4)**(1/3)
-  LPpref = np.float(1.38197659788534) # sqrt(6/pi)
-  LPbeta = np.float(0.962874509979126) # pi**(5/6)/6**(1/6)/2
-  LPr2 = np.float(1.4142135623731) # sqrt(2)
-  LPpi12 = np.float(0.261799387799149) # pi/12
-  LPsc = np.float(0.897772786961286) # a/ap == (pi**(5/6)/6**(1/6)) / pi**(2/3)
+  LPR1 = np.float64(1.33067003949147) # (3pi/4)**(1/3)
+  LPpref = np.float64(1.38197659788534) # sqrt(6/pi)
+  LPbeta = np.float64(0.962874509979126) # pi**(5/6)/6**(1/6)/2
+  LPr2 = np.float64(1.4142135623731) # sqrt(2)
+  LPpi12 = np.float64(0.261799387799149) # pi/12
+  LPsc = np.float64(0.897772786961286) # a/ap == (pi**(5/6)/6**(1/6)) / pi**(2/3)
   eps_loc = 1e-7
 
   xyzcu = np.zeros(3, dtype = np.float64)
   xyz3 = np.zeros(3,dtype=np.float64)
   xyz2 = np.zeros(3,dtype=np.float64)
   xyz1 = np.zeros(3,dtype=np.float64)
   rs = 0.0
```

### Comparing `pyebsdindex-0.1rc2/pyebsdindex/spherical_radon_fast.py` & `pyebsdindex-0.2.dev0/pyebsdindex/spherical_radon_fast.py`

 * *Files identical despite different names*

### Comparing `pyebsdindex-0.1rc2/pyebsdindex/tests/conftest.py` & `pyebsdindex-0.2.dev0/pyebsdindex/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pyebsdindex-0.1rc2/pyebsdindex/tests/data/al_sim_20kv/al_sim_20kv.png` & `pyebsdindex-0.2.dev0/pyebsdindex/tests/data/al_sim_20kv/al_sim_20kv.png`

 * *Files identical despite different names*

### Comparing `pyebsdindex-0.1rc2/pyebsdindex/tests/numbatest.py` & `pyebsdindex-0.2.dev0/pyebsdindex/tests/numbatest.py`

 * *Files identical despite different names*

### Comparing `pyebsdindex-0.1rc2/pyebsdindex/tests/raytest.py` & `pyebsdindex-0.2.dev0/pyebsdindex/tests/raytest.py`

 * *Files identical despite different names*

### Comparing `pyebsdindex-0.1rc2/pyebsdindex/tests/rotlibunittest.py` & `pyebsdindex-0.2.dev0/pyebsdindex/tests/rotlibunittest.py`

 * *Files identical despite different names*

### Comparing `pyebsdindex-0.1rc2/pyebsdindex/tests/test_ebsd_index.py` & `pyebsdindex-0.2.dev0/pyebsdindex/ebsd_index.py`

 * *Files 19% similar despite different names*

```diff
@@ -16,51 +16,22 @@
 # This software can be redistributed and/or modified freely provided that any derivative
 # works bear some notice that they are derived from it, and any modified versions bear
 # some notice that they have been modified.
 #
 # Author: David Rowenhorst;
 # The US Naval Research Laboratory Date: 21 Aug 2020
 
-import numpy as np
+"""Setup and handling of Hough indexing runs of EBSD patterns."""
 
-from pyebsdindex.ebsd_index import EBSDIndexer
-from pyebsdindex.rotlib import qu2eu
+from pyebsdindex import _ray_installed
+from pyebsdindex._ebsd_index_single import EBSDIndexer, index_pats
 
+if _ray_installed:
+    from pyebsdindex._ebsd_index_parallel import index_pats_distributed, IndexerRay
 
-class TestEBSDIndexer:
-    def test_init(self):
-        """Test creation of an indexer instance and its default values.
-        """
-        indexer = EBSDIndexer()
-        assert indexer.phaselist == ["FCC"]
-        assert indexer.sampleTilt == 70
-        assert indexer.camElev == 5.3
-        assert indexer.vendor == "EDAX"
 
-    def test_index_pats(self, pattern_al_sim_20kv):
-        """Test Hough indexing and setting/passing projection center
-        values.
-        """
-        pc = (0.4, 0.6, 0.5)
-        indexer_kwargs = dict(
-            phaselist=["FCC"],
-            vendor="EDAX",
-            sampleTilt=70,
-            camElev=5.3,
-            patDim=pattern_al_sim_20kv.shape
-        )
-
-        # Set PC upon initialization of indexer
-        indexer = EBSDIndexer(PC=pc, **indexer_kwargs)
-        data = indexer.index_pats(patsin=pattern_al_sim_20kv)[0]
-        assert np.allclose(data[0]["quat"], data[1]["quat"])
-
-        # Pass PC upon indexing
-        indexer2 = EBSDIndexer(**indexer_kwargs)
-        data2 = indexer2.index_pats(patsin=pattern_al_sim_20kv, PC=pc)[0]
-
-        # Results are the same in both examples
-        assert np.allclose(data2[0]["quat"], data[0]["quat"])
-
-        # Expected rotation (should be identity, (0, 0, 0)!)
-        euler = np.rad2deg(qu2eu(data[0]["quat"]))
-        assert np.isclose(euler, ((0, 0, 0), (0, 18, 72), (0, 90, 90)), atol=2).any()
+__all__ = [
+    "EBSDIndexer",
+    "IndexerRay",
+    "index_pats",
+    "index_pats_distributed",
+]
```

### Comparing `pyebsdindex-0.1rc2/pyebsdindex/tests/test_pcopt.py` & `pyebsdindex-0.2.dev0/pyebsdindex/tests/test_pcopt.py`

 * *Files 18% similar despite different names*

```diff
@@ -24,30 +24,16 @@
 
 from pyebsdindex import ebsd_index, pcopt
 
 
 class TestPCOptimization:
     def test_pc_optimize(self, pattern_al_sim_20kv):
         pc0 = (0.4, 0.6, 0.5)
-        indexer = ebsd_index.EBSDIndexer(
-            phaselist=["FCC"],
-            vendor="EDAX",
-            PC=None,
-            sampleTilt=70,
-            camElev=5.3,
-            patDim=pattern_al_sim_20kv.shape,
-        )
+        indexer = ebsd_index.EBSDIndexer(patDim=pattern_al_sim_20kv.shape)
         new_pc = pcopt.optimize(pattern_al_sim_20kv, indexer, PC0=pc0)
         assert np.allclose(new_pc, pc0, atol=0.05)
 
     def test_pc_optimize_pso(self, pattern_al_sim_20kv):
         pc0 = (0.4, 0.6, 0.5)
-        indexer = ebsd_index.EBSDIndexer(
-            phaselist=["FCC"],
-            vendor="EDAX",
-            PC=None,
-            sampleTilt=70,
-            camElev=5.3,
-            patDim=pattern_al_sim_20kv.shape,
-        )
+        indexer = ebsd_index.EBSDIndexer(patDim=pattern_al_sim_20kv.shape)
         new_pc = pcopt.optimize_pso(pattern_al_sim_20kv, indexer, PC0=pc0)
         assert np.allclose(new_pc, pc0, atol=0.05)
```

### Comparing `pyebsdindex-0.1rc2/pyebsdindex/tripletlib.py` & `pyebsdindex-0.2.dev0/pyebsdindex/tripletlib.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,61 +35,66 @@
     self.angles = None
     self.polePairs = None
     self.angleFamilyID = None
     self.tripAngles = None
     self.tripID = None
     self.completelib = None
     self.symmetry_pg = None
+    self.symmetry_pgID = None
     self.symmetry_sg = None
+    self.laue_code = None
     self.qsymops = None
     self.phaseName = None
     self.latticeParameter = np.array([1.0, 1.0, 1.0, 90.0, 90.0, 90.0])
 
     if libType is None:
       return
 
     if phaseName is None:
       self.phaseName = libType
     else:
       self.phaseName = phaseName
 
     if str(libType).upper() == 'FCC':
       self.build_fcc()
-      self.symmetry_pg = "Cubic m3m"
-      self.qsymops = crystal_sym.cubicsym_q()
       if phaseName is None:
         self.phaseName = 'FCC'
 
       if laticeParameter is None:
         self.latticeParameter = np.array([1.0,1.0,1.0,90.0,90.0,90.0])
       else:
         self.latticeParameter = laticeParameter
 
     if str(libType).upper() == 'BCC':
+
       self.build_bcc()
 
       if phaseName is None:
         self.phaseName = 'BCC'
       if laticeParameter is None:
         self.latticeParameter = np.array([1.0,1.0,1.0,90.0,90.0,90.0])
       else:
         self.latticeParameter = laticeParameter
 
   def build_fcc(self):
     if self.phaseName is None:
       self.phaseName = 'FCC'
     self.symmetry_pg = "Cubic m3m"
+    self.symmetry_pgID = 131
+    self.laue_code = 43
     self.qsymops = crystal_sym.cubicsym_q()
     poles = np.array([[0,0,2], [1,1,1], [0,2,2], [1,1,3]])
     self.build_trip_lib(poles,crystal_sym.cubicsym_q())
 
   def build_bcc(self):
     if self.phaseName is None:
       self.phaseName = 'BCC'
     self.symmetry_pg = "Cubic m3m"
+    self.symmetry_pgID = 131
+    self.laue_code = 43
     self.qsymops = crystal_sym.cubicsym_q()
     poles = np.array([[0,1,1],[0,0,2],[1,1,2],[0,1,3]])
     self.build_trip_lib(poles,crystal_sym.cubicsym_q())
 
   def build_trip_lib(self,poles,symmetry):
     nsym = symmetry.shape[0]
     npoles = poles.shape[0]
```

### Comparing `pyebsdindex-0.1rc2/pyebsdindex.egg-info/SOURCES.txt` & `pyebsdindex-0.2.dev0/pyebsdindex.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -1,18 +1,50 @@
+.readthedocs.yaml
+CHANGELOG.rst
+CONTRIBUTING.rst
+IPFCubic.pdf
+IPFCubic.png
 License
+MANIFEST.in
 README.md
+RELEASE.rst
 setup.cfg
 setup.py
+doc/Makefile
+doc/changelog.rst
+doc/conf.py
+doc/index.rst
+doc/make.bat
+doc/_static/custom.css
+doc/_static/colormap_banners/banner0.png
+doc/_static/colormap_banners/banner1.png
+doc/_static/colormap_banners/create_colormap_banners.py
+doc/_templates/custom-attribute-template.rst
+doc/_templates/custom-class-template.rst
+doc/_templates/custom-function-template.rst
+doc/_templates/custom-method-template.rst
+doc/_templates/custom-module-template.rst
+doc/_templates/autosummary/base.rst
+doc/dev/index.rst
+doc/reference/index.rst
+doc/tutorials/NLPAR_demo.ipynb
+doc/tutorials/ebsd_index_demo.ipynb
+doc/tutorials/index.rst
+doc/user/index.rst
+doc/user/installation.rst
 pyebsdindex/__init__.py
+pyebsdindex/_ebsd_index_parallel.py
+pyebsdindex/_ebsd_index_single.py
 pyebsdindex/band_detect.py
 pyebsdindex/band_vote.py
 pyebsdindex/crystal_sym.py
 pyebsdindex/crystallometry.py
 pyebsdindex/ebsd_index.py
 pyebsdindex/ebsd_pattern.py
+pyebsdindex/ebsdfile.py
 pyebsdindex/nlpar.py
 pyebsdindex/pairlib.py
 pyebsdindex/pcopt.py
 pyebsdindex/radon_fast.py
 pyebsdindex/rotations.py
 pyebsdindex/rotlib.py
 pyebsdindex/spherical_radon_fast.py
@@ -23,17 +55,20 @@
 pyebsdindex.egg-info/requires.txt
 pyebsdindex.egg-info/top_level.txt
 pyebsdindex.egg-info/zip-safe
 pyebsdindex/EBSDImage/IPFcolor.py
 pyebsdindex/EBSDImage/__init__.py
 pyebsdindex/opencl/__init__.py
 pyebsdindex/opencl/band_detect_cl.py
+pyebsdindex/opencl/clkernels.cl
 pyebsdindex/opencl/openclparam.py
 pyebsdindex/opencl/radon_fast_cl.py
 pyebsdindex/tests/__init__.py
 pyebsdindex/tests/conftest.py
 pyebsdindex/tests/numbatest.py
 pyebsdindex/tests/raytest.py
 pyebsdindex/tests/rotlibunittest.py
 pyebsdindex/tests/test_ebsd_index.py
+pyebsdindex/tests/test_package.py
 pyebsdindex/tests/test_pcopt.py
-pyebsdindex/tests/data/al_sim_20kv/al_sim_20kv.png
+pyebsdindex/tests/data/al_sim_20kv/al_sim_20kv.png
+pyebsdindex/tests/data/al_sim_20kv/generate_al_sim_20kv.py
```

### Comparing `pyebsdindex-0.1rc2/setup.py` & `pyebsdindex-0.2.dev0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,55 +7,77 @@
 
 
 # Projects with optional features for building the documentation and running
 # tests. From setuptools:
 # https://setuptools.readthedocs.io/en/latest/setuptools.html#declaring-extras-optional-features-with-their-own-dependencies
 extra_feature_requirements = {
     "doc": [
-        "furo",
-        "nbsphinx >= 0.7",
-        "sphinx >= 3.0.2",
-        "sphinx-copybutton >= 0.2.5",
-        "sphinx-gallery >= 0.6",
+        "nbsphinx                       >= 0.7",
+        "numpydoc",
+        "pydata-sphinx-theme",
+        "sphinx                         >= 3.0.2",
+        "sphinx-codeautolink[ipython]",
+        "sphinx-copybutton              >= 0.2.5",
+        "sphinx-design",
+        "sphinx-gallery",
     ],
-    "tests": ["coverage >= 5.0", "pytest >= 5.4", "pytest-cov >= 2.8.1"],
-    "gpu": ["pyopencl"],
+    "tests": [
+        "coverage                       >= 5.0",
+        "pytest                         >= 5.4",
+        "pytest-cov                     >= 2.8.1"
+    ],
+    "gpu": [
+        "pyopencl",
+    ],
+    "parallel": [
+        "ray[default]                   >= 1.13",
+    ]
 }
-# Create a development project, including both the docs and tests projects
+# Create a development installation "dev" including "doc" and "tests"
+# projects
 extra_feature_requirements["dev"] = list(
     chain(*list(extra_feature_requirements.values()))
 )
+# Create a user installation "all" including "gpu" and "parallel"
+runtime_extras_require = {}
+for x, packages in extra_feature_requirements.items():
+    if x not in ["doc", "tests"]:
+        runtime_extras_require[x] = packages
+extra_feature_requirements["all"] = list(chain(*list(runtime_extras_require.values())))
 
 
 setup(
     # Package description
     name=__name__,
     version=__version__,
     license="Custom",
-    python_requires=">=3.8",
+    python_requires=">=3.7",
     description=__description__,
     long_description=open("README.md", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     classifiers=[
         "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
         "Development Status :: 4 - Beta",
         "Intended Audience :: Science/Research",
         "License :: Other/Proprietary License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Topic :: Scientific/Engineering",
         "Topic :: Scientific/Engineering :: Physics",
     ],
     keywords=[
         "EBSD",
         "electron backscatter diffraction",
         "HI",
         "Hough indexing",
+        "NLPAR",
     ],
     zip_safe=True,
     # Contact
     author=__credits__,
     download_url="https://pypi.python.org/pypi/pyebsdindex",
     maintainer=__author__,
     maintainer_email=__author_email__,
@@ -69,23 +91,14 @@
     extras_require=extra_feature_requirements,
     install_requires=[
         "h5py",
         "matplotlib",
         "numpy",
         "numba",
         "pyswarms",
-        # See https://github.com/ray-project/ray/issues/24169
-        "ray[default] < 1.12.0",
         "scipy",
     ],
-    # Files to include when distributing package
+    # Files to include when distributing package (see also MANIFEST.in)
     packages=find_packages(),
     package_dir={"pyebsdindex": "pyebsdindex"},
     include_package_data=True,
-    package_data={
-        "pyebsdindex": [
-            "*.py",
-            "*.cl",
-            "tests/data/al_sim_20kv/al_sim_20kv.png",
-        ],
-    },
 )
```

