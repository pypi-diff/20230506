# Comparing `tmp/jaxip-0.5.5.tar.gz` & `tmp/jaxip-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaxip-0.5.5.tar", last modified: Mon May  1 12:41:19 2023, max compression
+gzip compressed data, was "jaxip-0.5.6.tar", last modified: Sat May  6 13:11:24 2023, max compression
```

## Comparing `jaxip-0.5.5.tar` & `jaxip-0.5.6.tar`

### file list

```diff
@@ -1,136 +1,139 @@
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-01 12:41:19.052954 jaxip-0.5.5/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      166 2022-12-07 19:09:20.000000 jaxip-0.5.5/AUTHORS.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     3491 2023-04-26 21:18:43.000000 jaxip-0.5.5/CONTRIBUTING.rst
--rw-r--r--   0 hossein   (1000) hossein   (1000)      569 2023-03-02 17:04:49.000000 jaxip-0.5.5/HISTORY.rst
--rw-r--r--   0 hossein   (1000) hossein   (1000)     1523 2023-01-05 20:40:22.000000 jaxip-0.5.5/LICENSE
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      262 2022-12-07 20:18:56.000000 jaxip-0.5.5/MANIFEST.in
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     8962 2023-05-01 12:41:19.056954 jaxip-0.5.5/PKG-INFO
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     8374 2023-05-01 12:41:07.000000 jaxip-0.5.5/README.rst
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-01 12:41:19.032954 jaxip-0.5.5/docs/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      606 2023-02-01 19:45:48.000000 jaxip-0.5.5/docs/Makefile
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-01 12:41:19.024954 jaxip-0.5.5/docs/_build/
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-01 12:41:19.024954 jaxip-0.5.5/docs/_build/doctrees/
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-01 12:41:19.032954 jaxip-0.5.5/docs/_build/doctrees/nbsphinx/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)    11011 2023-05-01 12:30:58.000000 jaxip-0.5.5/docs/_build/doctrees/nbsphinx/notebooks_tutorials_38_0.png
--rw-rw-r--   0 hossein   (1000) hossein   (1000)    12610 2023-05-01 12:30:58.000000 jaxip-0.5.5/docs/_build/doctrees/nbsphinx/notebooks_tutorials_45_0.png
--rw-rw-r--   0 hossein   (1000) hossein   (1000)    12610 2023-05-01 12:30:58.000000 jaxip-0.5.5/docs/_build/doctrees/nbsphinx/notebooks_tutorials_51_0.png
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-01 12:41:19.024954 jaxip-0.5.5/docs/_build/html/
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-01 12:41:19.032954 jaxip-0.5.5/docs/_build/html/_images/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)    11011 2023-05-01 12:30:58.000000 jaxip-0.5.5/docs/_build/html/_images/notebooks_tutorials_38_0.png
--rw-rw-r--   0 hossein   (1000) hossein   (1000)    12610 2023-05-01 12:30:58.000000 jaxip-0.5.5/docs/_build/html/_images/notebooks_tutorials_45_0.png
--rw-rw-r--   0 hossein   (1000) hossein   (1000)    12610 2023-05-01 12:30:58.000000 jaxip-0.5.5/docs/_build/html/_images/notebooks_tutorials_51_0.png
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-01 12:41:19.032954 jaxip-0.5.5/docs/_build/html/_static/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      286 2023-04-26 21:14:06.000000 jaxip-0.5.5/docs/_build/html/_static/file.png
--rw-rw-r--   0 hossein   (1000) hossein   (1000)       90 2023-04-26 21:14:06.000000 jaxip-0.5.5/docs/_build/html/_static/minus.png
--rw-rw-r--   0 hossein   (1000) hossein   (1000)       90 2023-04-26 21:14:06.000000 jaxip-0.5.5/docs/_build/html/_static/plus.png
--rw-rw-r--   0 hossein   (1000) hossein   (1000)       28 2022-12-28 08:07:09.000000 jaxip-0.5.5/docs/authors.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     6406 2023-05-01 12:41:07.000000 jaxip-0.5.5/docs/conf.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)       33 2022-12-07 19:09:20.000000 jaxip-0.5.5/docs/contributing.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)       85 2023-05-01 12:41:07.000000 jaxip-0.5.5/docs/examples.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)       28 2022-12-07 19:09:20.000000 jaxip-0.5.5/docs/history.rst
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-01 12:41:19.032954 jaxip-0.5.5/docs/images/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)    44314 2023-03-28 20:24:39.000000 jaxip-0.5.5/docs/images/flowchart.drawio.png
--rw-rw-r--   0 hossein   (1000) hossein   (1000)    96759 2023-02-06 19:53:40.000000 jaxip-0.5.5/docs/images/water.png
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      305 2023-05-01 12:41:07.000000 jaxip-0.5.5/docs/index.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1864 2023-04-26 21:18:43.000000 jaxip-0.5.5/docs/installation.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      760 2023-05-01 12:13:59.000000 jaxip-0.5.5/docs/jaxip.atoms.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      653 2023-05-01 12:13:59.000000 jaxip-0.5.5/docs/jaxip.datasets.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1095 2023-05-01 12:13:59.000000 jaxip-0.5.5/docs/jaxip.descriptors.acsf.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      595 2023-05-01 12:13:59.000000 jaxip-0.5.5/docs/jaxip.descriptors.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      635 2023-05-01 12:13:59.000000 jaxip-0.5.5/docs/jaxip.models.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1129 2023-05-01 12:41:07.000000 jaxip-0.5.5/docs/jaxip.potentials.nnp.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      616 2023-05-01 12:41:07.000000 jaxip-0.5.5/docs/jaxip.potentials.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      935 2023-05-01 12:30:49.000000 jaxip-0.5.5/docs/jaxip.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      915 2023-05-01 12:14:00.000000 jaxip-0.5.5/docs/jaxip.utils.rst
--rw-r--r--   0 hossein   (1000) hossein   (1000)      803 2023-01-05 20:40:22.000000 jaxip-0.5.5/docs/make.bat
--rw-rw-r--   0 hossein   (1000) hossein   (1000)       52 2023-05-01 12:30:49.000000 jaxip-0.5.5/docs/modules.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)       27 2022-12-20 21:49:36.000000 jaxip-0.5.5/docs/readme.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1158 2023-04-26 21:18:43.000000 jaxip-0.5.5/docs/usage.rst
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-01 12:41:19.036954 jaxip-0.5.5/jaxip/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      568 2023-04-26 21:18:43.000000 jaxip-0.5.5/jaxip/__init__.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      248 2023-05-01 12:41:07.000000 jaxip-0.5.5/jaxip/_version.py
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-01 12:41:19.036954 jaxip-0.5.5/jaxip/atoms/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      174 2023-05-01 12:41:07.000000 jaxip-0.5.5/jaxip/atoms/__init__.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      355 2023-05-01 12:41:07.000000 jaxip-0.5.5/jaxip/atoms/_box.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      779 2023-05-01 12:41:07.000000 jaxip-0.5.5/jaxip/atoms/_neighbor.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1342 2023-05-01 12:41:07.000000 jaxip-0.5.5/jaxip/atoms/_structure.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     3593 2023-05-01 12:41:07.000000 jaxip-0.5.5/jaxip/atoms/box.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     5034 2023-05-01 06:50:37.000000 jaxip-0.5.5/jaxip/atoms/element.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     2865 2023-05-01 12:41:07.000000 jaxip-0.5.5/jaxip/atoms/neighbor.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)    16157 2023-05-01 12:41:07.000000 jaxip-0.5.5/jaxip/atoms/structure.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     2589 2023-02-08 21:09:37.000000 jaxip-0.5.5/jaxip/base.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1131 2023-05-01 12:41:07.000000 jaxip-0.5.5/jaxip/config.py
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-01 12:41:19.036954 jaxip-0.5.5/jaxip/datasets/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      154 2023-05-01 12:41:07.000000 jaxip-0.5.5/jaxip/datasets/__init__.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      551 2023-05-01 12:41:07.000000 jaxip-0.5.5/jaxip/datasets/base.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     6282 2023-05-01 12:41:07.000000 jaxip-0.5.5/jaxip/datasets/runner.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1021 2023-05-01 12:41:07.000000 jaxip-0.5.5/jaxip/datasets/transformer.py
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-01 12:41:19.040954 jaxip-0.5.5/jaxip/descriptors/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      130 2023-05-01 12:41:07.000000 jaxip-0.5.5/jaxip/descriptors/__init__.py
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-01 12:41:19.040954 jaxip-0.5.5/jaxip/descriptors/acsf/
--rw-r--r--   0 hossein   (1000) hossein   (1000)      400 2023-01-05 20:40:22.000000 jaxip-0.5.5/jaxip/descriptors/acsf/__init__.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     5259 2023-05-01 12:41:07.000000 jaxip-0.5.5/jaxip/descriptors/acsf/_acsf.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     7581 2023-05-01 12:41:07.000000 jaxip-0.5.5/jaxip/descriptors/acsf/acsf.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     2226 2023-03-23 20:22:06.000000 jaxip-0.5.5/jaxip/descriptors/acsf/angular.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     2474 2023-03-23 20:22:06.000000 jaxip-0.5.5/jaxip/descriptors/acsf/cutoff.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1352 2023-03-23 20:22:06.000000 jaxip-0.5.5/jaxip/descriptors/acsf/radial.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1011 2023-05-01 12:41:07.000000 jaxip-0.5.5/jaxip/descriptors/acsf/symmetry.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      765 2023-05-01 09:07:44.000000 jaxip-0.5.5/jaxip/descriptors/base.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     7476 2023-05-01 12:41:07.000000 jaxip-0.5.5/jaxip/descriptors/scaler.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     3739 2023-05-01 12:41:07.000000 jaxip-0.5.5/jaxip/logger.py
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-01 12:41:19.040954 jaxip-0.5.5/jaxip/models/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      170 2023-05-01 12:41:07.000000 jaxip-0.5.5/jaxip/models/__init__.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1125 2023-05-01 12:41:07.000000 jaxip-0.5.5/jaxip/models/activation.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      604 2023-03-14 20:01:39.000000 jaxip-0.5.5/jaxip/models/initializer.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     2846 2023-05-01 12:41:07.000000 jaxip-0.5.5/jaxip/models/nn.py
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-01 12:41:19.044954 jaxip-0.5.5/jaxip/potentials/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      196 2023-05-01 12:41:07.000000 jaxip-0.5.5/jaxip/potentials/__init__.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1949 2023-05-01 12:41:07.000000 jaxip-0.5.5/jaxip/potentials/_energy.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      866 2023-05-01 12:41:07.000000 jaxip-0.5.5/jaxip/potentials/_force.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1799 2023-05-01 12:41:07.000000 jaxip-0.5.5/jaxip/potentials/atomic_potential.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      644 2023-05-01 12:41:07.000000 jaxip-0.5.5/jaxip/potentials/base.py
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-01 12:41:19.044954 jaxip-0.5.5/jaxip/potentials/nnp/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      196 2023-05-01 12:41:07.000000 jaxip-0.5.5/jaxip/potentials/nnp/__init__.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     9053 2023-05-01 12:41:07.000000 jaxip-0.5.5/jaxip/potentials/nnp/gradient_descent.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     9264 2023-05-01 12:41:07.000000 jaxip-0.5.5/jaxip/potentials/nnp/kalman_filter.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     2576 2023-05-01 12:41:07.000000 jaxip-0.5.5/jaxip/potentials/nnp/metrics.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)    18751 2023-05-01 12:41:07.000000 jaxip-0.5.5/jaxip/potentials/nnp/potential.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)    11326 2023-05-01 12:41:07.000000 jaxip-0.5.5/jaxip/potentials/nnp/settings.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      643 2023-01-25 20:59:12.000000 jaxip-0.5.5/jaxip/types.py
--rw-r--r--   0 hossein   (1000) hossein   (1000)      200 2023-01-05 20:40:22.000000 jaxip-0.5.5/jaxip/units.py
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-01 12:41:19.048954 jaxip-0.5.5/jaxip/utils/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)       73 2023-05-01 12:41:07.000000 jaxip-0.5.5/jaxip/utils/__init__.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1427 2023-02-18 20:52:11.000000 jaxip-0.5.5/jaxip/utils/attribute.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      585 2023-05-01 12:41:07.000000 jaxip-0.5.5/jaxip/utils/batch.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     2008 2023-03-23 20:22:06.000000 jaxip-0.5.5/jaxip/utils/compare.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     4410 2023-05-01 12:41:07.000000 jaxip-0.5.5/jaxip/utils/profiler.py
--rw-r--r--   0 hossein   (1000) hossein   (1000)      670 2023-01-18 21:30:52.000000 jaxip-0.5.5/jaxip/utils/tokenize.py
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-01 12:41:19.036954 jaxip-0.5.5/jaxip.egg-info/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     8962 2023-05-01 12:41:18.000000 jaxip-0.5.5/jaxip.egg-info/PKG-INFO
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     2972 2023-05-01 12:41:18.000000 jaxip-0.5.5/jaxip.egg-info/SOURCES.txt
--rw-rw-r--   0 hossein   (1000) hossein   (1000)        1 2023-05-01 12:41:18.000000 jaxip-0.5.5/jaxip.egg-info/dependency_links.txt
--rw-rw-r--   0 hossein   (1000) hossein   (1000)       41 2023-05-01 12:41:18.000000 jaxip-0.5.5/jaxip.egg-info/entry_points.txt
--rw-rw-r--   0 hossein   (1000) hossein   (1000)        1 2023-05-01 12:41:18.000000 jaxip-0.5.5/jaxip.egg-info/not-zip-safe
--rw-rw-r--   0 hossein   (1000) hossein   (1000)       85 2023-05-01 12:41:18.000000 jaxip-0.5.5/jaxip.egg-info/requires.txt
--rw-rw-r--   0 hossein   (1000) hossein   (1000)        6 2023-05-01 12:41:18.000000 jaxip-0.5.5/jaxip.egg-info/top_level.txt
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      137 2023-05-01 12:41:19.056954 jaxip-0.5.5/setup.cfg
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1661 2023-03-22 21:56:02.000000 jaxip-0.5.5/setup.py
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-01 12:41:19.052954 jaxip-0.5.5/tests/
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-01 12:41:19.052954 jaxip-0.5.5/tests/.ipynb_checkpoints/
--rw-r--r--   0 hossein   (1000) hossein   (1000)     3632 2022-12-27 18:25:19.000000 jaxip-0.5.5/tests/.ipynb_checkpoints/h2o-checkpoint.data
--rw-r--r--   0 hossein   (1000) hossein   (1000)     9543 2023-01-26 17:53:14.000000 jaxip-0.5.5/tests/.ipynb_checkpoints/h2o-checkpoint.json
--rw-r--r--   0 hossein   (1000) hossein   (1000)     3632 2022-12-26 17:32:00.000000 jaxip-0.5.5/tests/.ipynb_checkpoints/input.h2o-checkpoint.data
--rw-r--r--   0 hossein   (1000) hossein   (1000)    23707 2023-03-19 08:54:39.000000 jaxip-0.5.5/tests/.ipynb_checkpoints/test-checkpoint.ipynb
--rw-r--r--   0 hossein   (1000) hossein   (1000)       35 2023-01-05 20:40:22.000000 jaxip-0.5.5/tests/__init__.py
--rw-r--r--   0 hossein   (1000) hossein   (1000)     3632 2022-12-27 18:25:19.000000 jaxip-0.5.5/tests/h2o.data
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     2063 2023-03-14 20:01:39.000000 jaxip-0.5.5/tests/h2o.json
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      384 2023-05-01 12:36:35.000000 jaxip-0.5.5/tests/scaling.001.data
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      480 2023-05-01 12:36:35.000000 jaxip-0.5.5/tests/scaling.008.data
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     5117 2023-03-14 20:00:37.000000 jaxip-0.5.5/tests/test_acsf.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     4105 2023-02-06 19:57:38.000000 jaxip-0.5.5/tests/test_nn.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     3420 2023-05-01 12:41:07.000000 jaxip-0.5.5/tests/test_nnp.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     4816 2023-05-01 12:41:07.000000 jaxip-0.5.5/tests/test_runner.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     2859 2023-05-01 12:41:07.000000 jaxip-0.5.5/tests/test_scaler.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     4937 2023-04-24 20:54:27.000000 jaxip-0.5.5/tests/test_structure.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      793 2023-05-01 12:36:35.000000 jaxip-0.5.5/tests/weights.001.pkl
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      813 2023-05-01 12:36:35.000000 jaxip-0.5.5/tests/weights.008.pkl
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-06 13:11:24.739946 jaxip-0.5.6/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      166 2022-12-07 19:09:20.000000 jaxip-0.5.6/AUTHORS.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     3491 2023-04-26 21:18:43.000000 jaxip-0.5.6/CONTRIBUTING.rst
+-rw-r--r--   0 hossein   (1000) hossein   (1000)      569 2023-03-02 17:04:49.000000 jaxip-0.5.6/HISTORY.rst
+-rw-r--r--   0 hossein   (1000) hossein   (1000)     1523 2023-01-05 20:40:22.000000 jaxip-0.5.6/LICENSE
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      262 2022-12-07 20:18:56.000000 jaxip-0.5.6/MANIFEST.in
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     5283 2023-05-06 13:11:24.739946 jaxip-0.5.6/PKG-INFO
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     4696 2023-05-05 21:35:14.000000 jaxip-0.5.6/README.rst
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-06 13:11:24.723946 jaxip-0.5.6/docs/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      606 2023-02-01 19:45:48.000000 jaxip-0.5.6/docs/Makefile
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-06 13:11:24.715947 jaxip-0.5.6/docs/_build/
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-06 13:11:24.715947 jaxip-0.5.6/docs/_build/doctrees/
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-06 13:11:24.723946 jaxip-0.5.6/docs/_build/doctrees/nbsphinx/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)    15512 2023-05-06 13:07:08.000000 jaxip-0.5.6/docs/_build/doctrees/nbsphinx/notebooks_potential_training_29_21.png
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)    11011 2023-05-06 13:07:09.000000 jaxip-0.5.6/docs/_build/doctrees/nbsphinx/notebooks_tutorials_38_0.png
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)    12610 2023-05-06 13:07:09.000000 jaxip-0.5.6/docs/_build/doctrees/nbsphinx/notebooks_tutorials_45_0.png
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)    12610 2023-05-06 13:07:09.000000 jaxip-0.5.6/docs/_build/doctrees/nbsphinx/notebooks_tutorials_51_0.png
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-06 13:11:24.719947 jaxip-0.5.6/docs/_build/html/
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-06 13:11:24.723946 jaxip-0.5.6/docs/_build/html/_images/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)    15512 2023-05-06 13:07:08.000000 jaxip-0.5.6/docs/_build/html/_images/notebooks_potential_training_29_21.png
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)    11011 2023-05-06 13:07:09.000000 jaxip-0.5.6/docs/_build/html/_images/notebooks_tutorials_38_0.png
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)    12610 2023-05-06 13:07:09.000000 jaxip-0.5.6/docs/_build/html/_images/notebooks_tutorials_45_0.png
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)    12610 2023-05-06 13:07:09.000000 jaxip-0.5.6/docs/_build/html/_images/notebooks_tutorials_51_0.png
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-06 13:11:24.723946 jaxip-0.5.6/docs/_build/html/_static/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      286 2023-04-26 21:14:06.000000 jaxip-0.5.6/docs/_build/html/_static/file.png
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)       90 2023-04-26 21:14:06.000000 jaxip-0.5.6/docs/_build/html/_static/minus.png
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)       90 2023-04-26 21:14:06.000000 jaxip-0.5.6/docs/_build/html/_static/plus.png
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)       28 2022-12-28 08:07:09.000000 jaxip-0.5.6/docs/authors.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     6406 2023-05-01 12:49:56.000000 jaxip-0.5.6/docs/conf.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)       33 2022-12-07 19:09:20.000000 jaxip-0.5.6/docs/contributing.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)       81 2023-05-01 12:51:50.000000 jaxip-0.5.6/docs/examples.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)       28 2022-12-07 19:09:20.000000 jaxip-0.5.6/docs/history.rst
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-06 13:11:24.723946 jaxip-0.5.6/docs/images/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)    44314 2023-03-28 20:24:39.000000 jaxip-0.5.6/docs/images/flowchart.drawio.png
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)    96759 2023-02-06 19:53:40.000000 jaxip-0.5.6/docs/images/water.png
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      315 2023-05-04 21:58:24.000000 jaxip-0.5.6/docs/index.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1864 2023-04-26 21:18:43.000000 jaxip-0.5.6/docs/installation.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      760 2023-05-01 12:13:59.000000 jaxip-0.5.6/docs/jaxip.atoms.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      653 2023-05-01 12:13:59.000000 jaxip-0.5.6/docs/jaxip.datasets.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1095 2023-05-01 12:13:59.000000 jaxip-0.5.6/docs/jaxip.descriptors.acsf.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      595 2023-05-01 12:13:59.000000 jaxip-0.5.6/docs/jaxip.descriptors.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      635 2023-05-01 12:13:59.000000 jaxip-0.5.6/docs/jaxip.models.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1129 2023-05-01 12:41:07.000000 jaxip-0.5.6/docs/jaxip.potentials.nnp.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      616 2023-05-01 12:41:07.000000 jaxip-0.5.6/docs/jaxip.potentials.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      935 2023-05-06 13:07:01.000000 jaxip-0.5.6/docs/jaxip.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      915 2023-05-01 12:14:00.000000 jaxip-0.5.6/docs/jaxip.utils.rst
+-rw-r--r--   0 hossein   (1000) hossein   (1000)      803 2023-01-05 20:40:22.000000 jaxip-0.5.6/docs/make.bat
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)       52 2023-05-06 13:07:01.000000 jaxip-0.5.6/docs/modules.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)       27 2022-12-20 21:49:36.000000 jaxip-0.5.6/docs/readme.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     3833 2023-05-05 21:13:22.000000 jaxip-0.5.6/docs/theory.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1158 2023-04-26 21:18:43.000000 jaxip-0.5.6/docs/usage.rst
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-06 13:11:24.727946 jaxip-0.5.6/jaxip/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      575 2023-05-04 21:42:07.000000 jaxip-0.5.6/jaxip/__init__.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      294 2023-05-06 13:06:00.000000 jaxip-0.5.6/jaxip/_version.py
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-06 13:11:24.727946 jaxip-0.5.6/jaxip/atoms/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      174 2023-05-01 12:41:07.000000 jaxip-0.5.6/jaxip/atoms/__init__.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      355 2023-05-01 12:41:07.000000 jaxip-0.5.6/jaxip/atoms/_box.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      779 2023-05-01 12:41:07.000000 jaxip-0.5.6/jaxip/atoms/_neighbor.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1342 2023-05-01 12:41:07.000000 jaxip-0.5.6/jaxip/atoms/_structure.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     3593 2023-05-01 12:41:07.000000 jaxip-0.5.6/jaxip/atoms/box.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     5034 2023-05-01 06:50:37.000000 jaxip-0.5.6/jaxip/atoms/element.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     2865 2023-05-01 12:41:07.000000 jaxip-0.5.6/jaxip/atoms/neighbor.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)    16306 2023-05-06 13:01:56.000000 jaxip-0.5.6/jaxip/atoms/structure.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     2589 2023-02-08 21:09:37.000000 jaxip-0.5.6/jaxip/base.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1131 2023-05-01 12:41:07.000000 jaxip-0.5.6/jaxip/config.py
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-06 13:11:24.727946 jaxip-0.5.6/jaxip/datasets/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      154 2023-05-01 12:41:07.000000 jaxip-0.5.6/jaxip/datasets/__init__.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      444 2023-05-04 19:02:08.000000 jaxip-0.5.6/jaxip/datasets/base.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     6391 2023-05-04 21:19:36.000000 jaxip-0.5.6/jaxip/datasets/runner.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1021 2023-05-01 12:41:07.000000 jaxip-0.5.6/jaxip/datasets/transformer.py
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-06 13:11:24.731946 jaxip-0.5.6/jaxip/descriptors/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      130 2023-05-01 12:41:07.000000 jaxip-0.5.6/jaxip/descriptors/__init__.py
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-06 13:11:24.731946 jaxip-0.5.6/jaxip/descriptors/acsf/
+-rw-r--r--   0 hossein   (1000) hossein   (1000)      400 2023-01-05 20:40:22.000000 jaxip-0.5.6/jaxip/descriptors/acsf/__init__.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     5275 2023-05-06 12:28:36.000000 jaxip-0.5.6/jaxip/descriptors/acsf/_acsf.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     7581 2023-05-01 12:41:07.000000 jaxip-0.5.6/jaxip/descriptors/acsf/acsf.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     2226 2023-03-23 20:22:06.000000 jaxip-0.5.6/jaxip/descriptors/acsf/angular.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     2474 2023-03-23 20:22:06.000000 jaxip-0.5.6/jaxip/descriptors/acsf/cutoff.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1352 2023-03-23 20:22:06.000000 jaxip-0.5.6/jaxip/descriptors/acsf/radial.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1011 2023-05-01 12:41:07.000000 jaxip-0.5.6/jaxip/descriptors/acsf/symmetry.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      765 2023-05-01 09:07:44.000000 jaxip-0.5.6/jaxip/descriptors/base.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     7476 2023-05-01 12:41:07.000000 jaxip-0.5.6/jaxip/descriptors/scaler.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     3739 2023-05-01 12:41:07.000000 jaxip-0.5.6/jaxip/logger.py
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-06 13:11:24.731946 jaxip-0.5.6/jaxip/models/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      170 2023-05-01 12:41:07.000000 jaxip-0.5.6/jaxip/models/__init__.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1125 2023-05-01 12:41:07.000000 jaxip-0.5.6/jaxip/models/activation.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      604 2023-03-14 20:01:39.000000 jaxip-0.5.6/jaxip/models/initializer.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     2846 2023-05-01 12:41:07.000000 jaxip-0.5.6/jaxip/models/nn.py
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-06 13:11:24.731946 jaxip-0.5.6/jaxip/potentials/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      196 2023-05-01 12:41:07.000000 jaxip-0.5.6/jaxip/potentials/__init__.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1949 2023-05-01 12:41:07.000000 jaxip-0.5.6/jaxip/potentials/_energy.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      866 2023-05-01 12:41:07.000000 jaxip-0.5.6/jaxip/potentials/_force.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1799 2023-05-01 12:41:07.000000 jaxip-0.5.6/jaxip/potentials/atomic_potential.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      644 2023-05-01 12:41:07.000000 jaxip-0.5.6/jaxip/potentials/base.py
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-06 13:11:24.735946 jaxip-0.5.6/jaxip/potentials/nnp/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      196 2023-05-01 12:41:07.000000 jaxip-0.5.6/jaxip/potentials/nnp/__init__.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     9053 2023-05-01 12:41:07.000000 jaxip-0.5.6/jaxip/potentials/nnp/gradient_descent.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     9264 2023-05-02 06:46:19.000000 jaxip-0.5.6/jaxip/potentials/nnp/kalman_filter.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     2576 2023-05-01 12:41:07.000000 jaxip-0.5.6/jaxip/potentials/nnp/metrics.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)    18936 2023-05-05 07:59:16.000000 jaxip-0.5.6/jaxip/potentials/nnp/potential.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)    11326 2023-05-01 12:41:07.000000 jaxip-0.5.6/jaxip/potentials/nnp/settings.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      643 2023-01-25 20:59:12.000000 jaxip-0.5.6/jaxip/types.py
+-rw-r--r--   0 hossein   (1000) hossein   (1000)      200 2023-01-05 20:40:22.000000 jaxip-0.5.6/jaxip/units.py
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-06 13:11:24.735946 jaxip-0.5.6/jaxip/utils/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)       73 2023-05-01 12:41:07.000000 jaxip-0.5.6/jaxip/utils/__init__.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1427 2023-02-18 20:52:11.000000 jaxip-0.5.6/jaxip/utils/attribute.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      585 2023-05-01 12:41:07.000000 jaxip-0.5.6/jaxip/utils/batch.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     2008 2023-03-23 20:22:06.000000 jaxip-0.5.6/jaxip/utils/compare.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     4410 2023-05-01 12:41:07.000000 jaxip-0.5.6/jaxip/utils/profiler.py
+-rw-r--r--   0 hossein   (1000) hossein   (1000)      670 2023-01-18 21:30:52.000000 jaxip-0.5.6/jaxip/utils/tokenize.py
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-06 13:11:24.727946 jaxip-0.5.6/jaxip.egg-info/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     5283 2023-05-06 13:11:24.000000 jaxip-0.5.6/jaxip.egg-info/PKG-INFO
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     3121 2023-05-06 13:11:24.000000 jaxip-0.5.6/jaxip.egg-info/SOURCES.txt
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)        1 2023-05-06 13:11:24.000000 jaxip-0.5.6/jaxip.egg-info/dependency_links.txt
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)       41 2023-05-06 13:11:24.000000 jaxip-0.5.6/jaxip.egg-info/entry_points.txt
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)        1 2023-05-06 13:11:24.000000 jaxip-0.5.6/jaxip.egg-info/not-zip-safe
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)       85 2023-05-06 13:11:24.000000 jaxip-0.5.6/jaxip.egg-info/requires.txt
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)        6 2023-05-06 13:11:24.000000 jaxip-0.5.6/jaxip.egg-info/top_level.txt
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      137 2023-05-06 13:11:24.739946 jaxip-0.5.6/setup.cfg
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1661 2023-03-22 21:56:02.000000 jaxip-0.5.6/setup.py
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-06 13:11:24.739946 jaxip-0.5.6/tests/
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-06 13:11:24.739946 jaxip-0.5.6/tests/.ipynb_checkpoints/
+-rw-r--r--   0 hossein   (1000) hossein   (1000)     3632 2022-12-27 18:25:19.000000 jaxip-0.5.6/tests/.ipynb_checkpoints/h2o-checkpoint.data
+-rw-r--r--   0 hossein   (1000) hossein   (1000)     9543 2023-01-26 17:53:14.000000 jaxip-0.5.6/tests/.ipynb_checkpoints/h2o-checkpoint.json
+-rw-r--r--   0 hossein   (1000) hossein   (1000)     3632 2022-12-26 17:32:00.000000 jaxip-0.5.6/tests/.ipynb_checkpoints/input.h2o-checkpoint.data
+-rw-r--r--   0 hossein   (1000) hossein   (1000)    23707 2023-03-19 08:54:39.000000 jaxip-0.5.6/tests/.ipynb_checkpoints/test-checkpoint.ipynb
+-rw-r--r--   0 hossein   (1000) hossein   (1000)       35 2023-01-05 20:40:22.000000 jaxip-0.5.6/tests/__init__.py
+-rw-r--r--   0 hossein   (1000) hossein   (1000)     3632 2022-12-27 18:25:19.000000 jaxip-0.5.6/tests/h2o.data
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     2063 2023-03-14 20:01:39.000000 jaxip-0.5.6/tests/h2o.json
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      384 2023-05-06 13:06:50.000000 jaxip-0.5.6/tests/scaling.001.data
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      480 2023-05-06 13:06:50.000000 jaxip-0.5.6/tests/scaling.008.data
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     5117 2023-03-14 20:00:37.000000 jaxip-0.5.6/tests/test_acsf.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     4105 2023-02-06 19:57:38.000000 jaxip-0.5.6/tests/test_nn.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     3420 2023-05-01 12:41:07.000000 jaxip-0.5.6/tests/test_nnp.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     4816 2023-05-01 12:41:07.000000 jaxip-0.5.6/tests/test_runner.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     2859 2023-05-01 12:41:07.000000 jaxip-0.5.6/tests/test_scaler.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     4937 2023-04-24 20:54:27.000000 jaxip-0.5.6/tests/test_structure.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      793 2023-05-06 13:06:50.000000 jaxip-0.5.6/tests/weights.001.pkl
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      813 2023-05-06 13:06:50.000000 jaxip-0.5.6/tests/weights.008.pkl
```

### Comparing `jaxip-0.5.5/CONTRIBUTING.rst` & `jaxip-0.5.6/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.5/HISTORY.rst` & `jaxip-0.5.6/HISTORY.rst`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.5/LICENSE` & `jaxip-0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.5/docs/Makefile` & `jaxip-0.5.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.5/docs/_build/doctrees/nbsphinx/notebooks_tutorials_38_0.png` & `jaxip-0.5.6/docs/_build/doctrees/nbsphinx/notebooks_tutorials_38_0.png`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.5/docs/_build/doctrees/nbsphinx/notebooks_tutorials_45_0.png` & `jaxip-0.5.6/docs/_build/doctrees/nbsphinx/notebooks_tutorials_45_0.png`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.5/docs/_build/doctrees/nbsphinx/notebooks_tutorials_51_0.png` & `jaxip-0.5.6/docs/_build/doctrees/nbsphinx/notebooks_tutorials_51_0.png`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.5/docs/_build/html/_images/notebooks_tutorials_38_0.png` & `jaxip-0.5.6/docs/_build/html/_images/notebooks_tutorials_38_0.png`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.5/docs/_build/html/_images/notebooks_tutorials_45_0.png` & `jaxip-0.5.6/docs/_build/html/_images/notebooks_tutorials_45_0.png`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.5/docs/_build/html/_images/notebooks_tutorials_51_0.png` & `jaxip-0.5.6/docs/_build/html/_images/notebooks_tutorials_51_0.png`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.5/docs/conf.py` & `jaxip-0.5.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.5/docs/images/flowchart.drawio.png` & `jaxip-0.5.6/docs/images/flowchart.drawio.png`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.5/docs/images/water.png` & `jaxip-0.5.6/docs/images/water.png`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.5/docs/installation.rst` & `jaxip-0.5.6/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.5/docs/jaxip.atoms.rst` & `jaxip-0.5.6/docs/jaxip.atoms.rst`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.5/docs/jaxip.datasets.rst` & `jaxip-0.5.6/docs/jaxip.datasets.rst`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.5/docs/jaxip.descriptors.acsf.rst` & `jaxip-0.5.6/docs/jaxip.descriptors.acsf.rst`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.5/docs/jaxip.descriptors.rst` & `jaxip-0.5.6/docs/jaxip.descriptors.rst`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.5/docs/jaxip.models.rst` & `jaxip-0.5.6/docs/jaxip.models.rst`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.5/docs/jaxip.potentials.nnp.rst` & `jaxip-0.5.6/docs/jaxip.potentials.nnp.rst`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.5/docs/jaxip.potentials.rst` & `jaxip-0.5.6/docs/jaxip.potentials.rst`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.5/docs/jaxip.rst` & `jaxip-0.5.6/docs/jaxip.rst`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.5/docs/jaxip.utils.rst` & `jaxip-0.5.6/docs/jaxip.utils.rst`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.5/docs/make.bat` & `jaxip-0.5.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.5/docs/usage.rst` & `jaxip-0.5.6/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.5/jaxip/__init__.py` & `jaxip-0.5.6/jaxip/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Jaxip - JAX-based Interatomic Potential
 =======================================
 
-Jaxip is an optimized Python library on basis of JAX that enables development of emerging 
+Jaxip is an optimized Python library on basis of Google JAX that enables development of emerging 
 machine learning interatomic potentials for use in computational physics, chemistry, material 
 science. These potentials are necessary for conducting large-scale molecular dynamics simulations 
 of complex materials with ab initio accuracy.
 """
 from jaxip._version import __version__ as version
 
 __author__ = """Hossein Ghorbanfekr"""
```

### Comparing `jaxip-0.5.5/jaxip/atoms/_neighbor.py` & `jaxip-0.5.6/jaxip/atoms/_neighbor.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.5/jaxip/atoms/_structure.py` & `jaxip-0.5.6/jaxip/atoms/_structure.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.5/jaxip/atoms/box.py` & `jaxip-0.5.6/jaxip/atoms/box.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.5/jaxip/atoms/element.py` & `jaxip-0.5.6/jaxip/atoms/element.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.5/jaxip/atoms/neighbor.py` & `jaxip-0.5.6/jaxip/atoms/neighbor.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.5/jaxip/atoms/structure.py` & `jaxip-0.5.6/jaxip/atoms/structure.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 
 from collections import defaultdict
 from dataclasses import dataclass, field
+from functools import cached_property
 from typing import Any, DefaultDict, Dict, Generator, List, NamedTuple, Optional, Tuple
 
 import jax
 import jax.numpy as jnp
 import numpy as np
 from ase import Atoms as AseAtoms
 from jax import tree_util
@@ -166,25 +167,25 @@
             )
             kwargs["box"] = cls._init_box(data_["lattice"], dtype=dtype)
             kwargs["element_map"] = element_map
             kwargs["neighbor"] = Neighbor(r_cutoff=r_cutoff)
 
         except KeyError:
             logger.error(
-                f"Cannot find at least one of the expected keyword in the input data.",
+                "Cannot find at least one of the expected keyword in the input data.",
                 exception=KeyError,
             )
         return cls(**kwargs)
 
     @staticmethod
     def _init_arrays(
         data: Dict, element_map: ElementMap, dtype: Dtype
     ) -> Dict[str, Array]:
         """Initialize a dictionary of arrays of atomic attributes from the input data."""
-        logger.debug("Allocating arrays for the structure:")
+        logger.debug("Allocating arrays for a structure as follows:")
         arrays: Dict[str, Array] = dict()
         for atom_attr in Structure._get_atom_attributes():
             try:
                 array: Array
                 if atom_attr == "atom_type":
                     array = jnp.asarray(
                         [element_map(atom) for atom in data["element"]],
@@ -280,18 +281,22 @@
     @property
     def lattice(self) -> Optional[Array]:
         """Cell 3x3 matrix."""
         return self.box.lattice
 
     @property
     def elements(self) -> tuple[Element, ...]:
-        return tuple(sorted({str(self.element_map(int(at))) for at in self.atom_type}))
+        atom_type_host = jax.device_get(self.atom_type)
+        return tuple(sorted({str(self.element_map(int(at))) for at in atom_type_host}))
 
     def __repr__(self) -> str:
-        return f"{self.__class__.__name__}(natoms={self.natoms}, elements={self.elements}, dtype={self.dtype})"
+        return (
+            f"{self.__class__.__name__}"
+            f"(natoms={self.natoms}, elements={self.elements}, dtype={self.dtype})"
+        )
 
     def select(self, element: Element) -> Array:
         """
         Return all atom indices of the element.
 
         :param element: element name (e.g. `H` for hydrogen)
         :return: atom indices
@@ -384,15 +389,15 @@
 
     def remove_energy_offset(self, atom_energy: Dict[Element, float]) -> None:
         """
         Remove the input atom reference energies from the per-atom and total energy.
 
         :param atom_energy: atom reference energy
         """
-        energy_offset = self._get_energy_offset(atom_energy)
+        energy_offset: Array = self._get_energy_offset(atom_energy)
         self.energy -= energy_offset
         self.total_energy -= energy_offset.sum()
 
     def add_energy_offset(self, atom_energy: Dict[Element, float]) -> None:
         """
         Add the input atom reference energies from the per-atom and total energy.
```

### Comparing `jaxip-0.5.5/jaxip/base.py` & `jaxip-0.5.6/jaxip/base.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.5/jaxip/config.py` & `jaxip-0.5.6/jaxip/config.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.5/jaxip/datasets/runner.py` & `jaxip-0.5.6/jaxip/datasets/runner.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from jaxip.datasets.transformer import ToStructure, Transformer
 from jaxip.logger import logger
 from jaxip.utils.tokenize import tokenize
 
 
 class RunnerDataset(StructureDataset):
     """
-    Structure dataset for `RuNNer`_ data file format.
+    Dataset for `RuNNer`_ data file format.
 
     The input structure file contains atom info and simulation box.
     Each snapshot contains two per-atom and collective properties as follows:
 
     * `per-atom` properties include the element name, positions, energy, charge, force components, etc.
     * `collective` properties such as lattice, total energy, and total charge.
 
@@ -133,14 +133,16 @@
         :rtype: Any
         """
         logger.debug(f"Reading structure[{index}]")
         with open(str(self.filename), "r") as file:
             for _ in range(index):
                 self._ignore_next_structure(file)
             sample = self._read_next_structure(file)
+            if not sample:
+                raise IndexError(f"index {index} is out of bound with size {len(self)}")
         return self.transform(sample)
 
     def _read_from_cache(self, index: int) -> Structure:
         """
         Read from the cached structures if the `persist` input flag is enabled.
 
         :param index: index for structures
@@ -170,17 +172,17 @@
             Due to its slow performance, lack of shuffling, and no parallel loading,
             it is recommended to be only used for testing.
 
         :raises StopIteration: stop iteration
         :return: Return next structure
         :rtype: Transformed structure
         """
-        if self._current_index < len(self):
+        try:
             sample: Structure = self.__getitem__(self._current_index)
             self._current_index += 1
             return sample
-
-        self._current_index = 0
-        raise StopIteration
+        except IndexError:
+            self._current_index = 0
+            raise StopIteration
 
     def __iter__(self) -> RunnerDataset:
         return self
```

### Comparing `jaxip-0.5.5/jaxip/datasets/transformer.py` & `jaxip-0.5.6/jaxip/datasets/transformer.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.5/jaxip/descriptors/acsf/_acsf.py` & `jaxip-0.5.6/jaxip/descriptors/acsf/_acsf.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,22 +9,14 @@
 from jaxip.atoms._structure import _calculate_distance_per_atom
 from jaxip.descriptors.acsf.angular import AngularSymmetryFunction
 from jaxip.descriptors.acsf.radial import RadialSymmetryFunction
 from jaxip.descriptors.acsf.symmetry import EnvironmentElements
 from jaxip.types import Array, Element
 
 
-class AcsfInterface(Protocol):
-    num_symmetry_functions: int
-    num_radial_symmetry_functions: int
-    num_angular_symmetry_functions: int
-    radial_symmetry_functions: Tuple
-    angular_symmetry_functions: Tuple
-
-
 @jit
 def _calculate_radial_acsf_per_atom(
     radial: Dict[EnvironmentElements, RadialSymmetryFunction],
     atype: Array,
     dist_i: Array,
     emap: Dict[Element, Array],
 ) -> Array:
@@ -69,17 +61,18 @@
             _inner_loop_over_angular_acsf_terms,
             mask_ik=mask_cutoff_and_atype_ik,
             diff_i=diff_i,
             dist_i=dist_i,
             lattice=lattice,
             kernel=angular[elements],
         ),
-        jnp.asarray(0.0),
+        jnp.array(0.0),
         (diff_i, dist_i, mask_cutoff_and_atype_ij),
     )
+
     # correct double-counting
     total = lax.cond(
         at_j == at_k,
         lambda x: x * 0.5,
         lambda x: x,
         total,
     )
@@ -111,15 +104,15 @@
     is_zero = operand == 0.0
     true_op = jnp.where(is_zero, 1.0, operand)
     cost = jnp.where(
         mask_ik,
         jnp.inner(Rij, diff_i) / true_op,
         1.0,
     )
-    cost = jnp.where(is_zero, 0.0, cost)
+    cost = jnp.where(is_zero, 0.0, cost)  # type: ignore
 
     rjk = jnp.where(  # diff_jk = diff_ji - diff_ik
         mask_ik,
         _calculate_distance_per_atom(Rij, diff_i, lattice)[0],
         0.0,
     )  # second tuple output for Rjk
 
@@ -128,17 +121,26 @@
         jnp.sum(
             kernel(rij, dist_i, rjk, cost),
             where=mask_ik & (rjk > 0.0),  # exclude k=j # type:ignore
             axis=0,
         ),
         0.0,
     )
+
     return total + value, value
 
 
+class AcsfInterface(Protocol):
+    num_symmetry_functions: int
+    num_radial_symmetry_functions: int
+    num_angular_symmetry_functions: int
+    radial_symmetry_functions: Tuple
+    angular_symmetry_functions: Tuple
+
+
 @jit
 def _calculate_descriptor_per_atom(
     acsf: AcsfInterface,
     single_atom_position: Array,
     neighbor_positions: Array,
     atype: Array,
     lattice: Array,
```

### Comparing `jaxip-0.5.5/jaxip/descriptors/acsf/acsf.py` & `jaxip-0.5.6/jaxip/descriptors/acsf/acsf.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.5/jaxip/descriptors/acsf/angular.py` & `jaxip-0.5.6/jaxip/descriptors/acsf/angular.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.5/jaxip/descriptors/acsf/cutoff.py` & `jaxip-0.5.6/jaxip/descriptors/acsf/cutoff.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.5/jaxip/descriptors/acsf/radial.py` & `jaxip-0.5.6/jaxip/descriptors/acsf/radial.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.5/jaxip/descriptors/acsf/symmetry.py` & `jaxip-0.5.6/jaxip/descriptors/acsf/symmetry.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.5/jaxip/descriptors/base.py` & `jaxip-0.5.6/jaxip/descriptors/base.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.5/jaxip/descriptors/scaler.py` & `jaxip-0.5.6/jaxip/descriptors/scaler.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.5/jaxip/logger.py` & `jaxip-0.5.6/jaxip/logger.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.5/jaxip/models/activation.py` & `jaxip-0.5.6/jaxip/models/activation.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.5/jaxip/models/initializer.py` & `jaxip-0.5.6/jaxip/models/initializer.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.5/jaxip/models/nn.py` & `jaxip-0.5.6/jaxip/models/nn.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.5/jaxip/potentials/_energy.py` & `jaxip-0.5.6/jaxip/potentials/_energy.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.5/jaxip/potentials/_force.py` & `jaxip-0.5.6/jaxip/potentials/_force.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.5/jaxip/potentials/atomic_potential.py` & `jaxip-0.5.6/jaxip/potentials/atomic_potential.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.5/jaxip/potentials/base.py` & `jaxip-0.5.6/jaxip/potentials/base.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.5/jaxip/potentials/nnp/gradient_descent.py` & `jaxip-0.5.6/jaxip/potentials/nnp/gradient_descent.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.5/jaxip/potentials/nnp/kalman_filter.py` & `jaxip-0.5.6/jaxip/potentials/nnp/kalman_filter.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 def _tree_flatten(pytree: Dict) -> Array:
     return flatten_util.ravel_pytree(pytree)[0].reshape(-1, 1)  # type: ignore
 
 
 class KalmanFilterUpdater(Updater):
     """
-    A potential traienr which uses Kalman filter to update model weights (see this_).
+    A potential trainer which uses Kalman filter to update model weights (see this_).
 
     .. _this: https://pubs.acs.org/doi/10.1021/acs.jctc.8b01092
     """
 
     # https://github.com/CompPhysVienna/n2p2/blob/master/src/libnnptrain/KalmanFilter.cpp
 
     def __init__(self, potential: Potential) -> None:
```

### Comparing `jaxip-0.5.5/jaxip/potentials/nnp/metrics.py` & `jaxip-0.5.6/jaxip/potentials/nnp/metrics.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.5/jaxip/potentials/nnp/potential.py` & `jaxip-0.5.6/jaxip/potentials/nnp/potential.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from collections import defaultdict
 from dataclasses import dataclass, field
 from pathlib import Path
 from typing import Dict, Optional, Tuple
 
 import jax.numpy as jnp
+from ase import data
 from frozendict import frozendict
 from jax import random
 from tqdm import tqdm
 
 from jaxip.atoms.element import ElementMap
 from jaxip.atoms.structure import Structure
 from jaxip.datasets.runner import RunnerDataset
@@ -326,16 +327,19 @@
         """
         Fit scaler parameters for each element using the input structure data.
         No gradient history is required here.
         """
         # loader = TorchDataLoader(dataset, collate_fn=lambda batch: batch)
         print("Fitting descriptor scaler...")
         try:
-            for structure in tqdm(dataset):
-                for element in structure.elements:
+            dataset_size: int = len(dataset)
+            for index in tqdm(range(dataset_size)):
+                structure: Structure = dataset[index]
+                elements: Tuple[Element, ...] = structure.elements
+                for element in elements:
                     x: Array = self.atomic_potential[element].descriptor(structure)
                     self.atomic_potential[element].scaler.fit(x)
         except KeyboardInterrupt:
             print("Keyboard Interrupt")
         else:
             print("Done.")
```

### Comparing `jaxip-0.5.5/jaxip/potentials/nnp/settings.py` & `jaxip-0.5.6/jaxip/potentials/nnp/settings.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.5/jaxip/types.py` & `jaxip-0.5.6/jaxip/types.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.5/jaxip/utils/attribute.py` & `jaxip-0.5.6/jaxip/utils/attribute.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.5/jaxip/utils/batch.py` & `jaxip-0.5.6/jaxip/utils/batch.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.5/jaxip/utils/compare.py` & `jaxip-0.5.6/jaxip/utils/compare.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.5/jaxip/utils/profiler.py` & `jaxip-0.5.6/jaxip/utils/profiler.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.5/jaxip/utils/tokenize.py` & `jaxip-0.5.6/jaxip/utils/tokenize.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.5/jaxip.egg-info/SOURCES.txt` & `jaxip-0.5.6/jaxip.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -22,18 +22,21 @@
 docs/jaxip.potentials.nnp.rst
 docs/jaxip.potentials.rst
 docs/jaxip.rst
 docs/jaxip.utils.rst
 docs/make.bat
 docs/modules.rst
 docs/readme.rst
+docs/theory.rst
 docs/usage.rst
+docs/_build/doctrees/nbsphinx/notebooks_potential_training_29_21.png
 docs/_build/doctrees/nbsphinx/notebooks_tutorials_38_0.png
 docs/_build/doctrees/nbsphinx/notebooks_tutorials_45_0.png
 docs/_build/doctrees/nbsphinx/notebooks_tutorials_51_0.png
+docs/_build/html/_images/notebooks_potential_training_29_21.png
 docs/_build/html/_images/notebooks_tutorials_38_0.png
 docs/_build/html/_images/notebooks_tutorials_45_0.png
 docs/_build/html/_images/notebooks_tutorials_51_0.png
 docs/_build/html/_static/file.png
 docs/_build/html/_static/minus.png
 docs/_build/html/_static/plus.png
 docs/images/flowchart.drawio.png
```

### Comparing `jaxip-0.5.5/setup.py` & `jaxip-0.5.6/setup.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.5/tests/.ipynb_checkpoints/h2o-checkpoint.data` & `jaxip-0.5.6/tests/.ipynb_checkpoints/h2o-checkpoint.data`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.5/tests/.ipynb_checkpoints/h2o-checkpoint.json` & `jaxip-0.5.6/tests/.ipynb_checkpoints/h2o-checkpoint.json`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.5/tests/.ipynb_checkpoints/input.h2o-checkpoint.data` & `jaxip-0.5.6/tests/.ipynb_checkpoints/input.h2o-checkpoint.data`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.5/tests/.ipynb_checkpoints/test-checkpoint.ipynb` & `jaxip-0.5.6/tests/.ipynb_checkpoints/test-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.5/tests/h2o.data` & `jaxip-0.5.6/tests/h2o.data`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.5/tests/h2o.json` & `jaxip-0.5.6/tests/h2o.json`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.5/tests/test_acsf.py` & `jaxip-0.5.6/tests/test_acsf.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.5/tests/test_nn.py` & `jaxip-0.5.6/tests/test_nn.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.5/tests/test_nnp.py` & `jaxip-0.5.6/tests/test_nnp.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.5/tests/test_runner.py` & `jaxip-0.5.6/tests/test_runner.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.5/tests/test_scaler.py` & `jaxip-0.5.6/tests/test_scaler.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.5/tests/test_structure.py` & `jaxip-0.5.6/tests/test_structure.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.5/tests/weights.001.pkl` & `jaxip-0.5.6/tests/weights.001.pkl`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.5/tests/weights.008.pkl` & `jaxip-0.5.6/tests/weights.008.pkl`

 * *Files identical despite different names*

