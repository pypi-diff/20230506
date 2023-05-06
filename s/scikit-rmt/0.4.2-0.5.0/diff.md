# Comparing `tmp/scikit-rmt-0.4.2.tar.gz` & `tmp/scikit-rmt-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/scikit-rmt-0.4.2.tar", last modified: Fri Jan 27 19:35:36 2023, max compression
+gzip compressed data, was "dist/scikit-rmt-0.5.0.tar", last modified: Sat May  6 16:07:34 2023, max compression
```

## Comparing `scikit-rmt-0.4.2.tar` & `scikit-rmt-0.5.0.tar`

### file list

```diff
@@ -1,68 +1,72 @@
-drwxr-xr-x   0 santorum   (501) staff       (20)        0 2023-01-27 19:35:36.817065 scikit-rmt-0.4.2/
--rw-r--r--   0 santorum   (501) staff       (20)      337 2021-05-02 17:28:24.000000 scikit-rmt-0.4.2/.coveragerc
--rw-r--r--   0 santorum   (501) staff       (20)      219 2021-05-14 17:37:17.000000 scikit-rmt-0.4.2/.travis.yml
--rw-r--r--   0 santorum   (501) staff       (20)     1563 2021-04-26 20:56:17.000000 scikit-rmt-0.4.2/LICENSE
--rw-r--r--   0 santorum   (501) staff       (20)      325 2023-01-27 18:49:57.000000 scikit-rmt-0.4.2/MANIFEST.in
--rw-r--r--   0 santorum   (501) staff       (20)     2569 2021-05-05 17:08:35.000000 scikit-rmt-0.4.2/Makefile
--rw-r--r--   0 santorum   (501) staff       (20)    14206 2023-01-27 19:35:36.817896 scikit-rmt-0.4.2/PKG-INFO
--rw-r--r--   0 santorum   (501) staff       (20)    10996 2023-01-06 15:03:09.000000 scikit-rmt-0.4.2/README.md
--rw-r--r--   0 santorum   (501) staff       (20)     2843 2022-10-04 14:39:57.000000 scikit-rmt-0.4.2/conf.py
-drwxr-xr-x   0 santorum   (501) staff       (20)        0 2023-01-27 19:35:36.732746 scikit-rmt-0.4.2/docs/
--rw-r--r--   0 santorum   (501) staff       (20)       52 2022-10-04 14:32:13.000000 scikit-rmt-0.4.2/docs/modules.rst
--rw-r--r--   0 santorum   (501) staff       (20)       54 2021-05-08 23:10:40.000000 scikit-rmt-0.4.2/docs/readthedocs-requirements.txt
--rw-r--r--   0 santorum   (501) staff       (20)      522 2022-10-04 14:32:13.000000 scikit-rmt-0.4.2/docs/skrmt.covariance.rst
--rw-r--r--   0 santorum   (501) staff       (20)     1274 2022-10-04 14:32:13.000000 scikit-rmt-0.4.2/docs/skrmt.ensemble.rst
--rw-r--r--   0 santorum   (501) staff       (20)      232 2022-10-04 14:32:13.000000 scikit-rmt-0.4.2/docs/skrmt.rst
-drwxr-xr-x   0 santorum   (501) staff       (20)        0 2023-01-27 19:35:36.744437 scikit-rmt-0.4.2/examples/
--rw-r--r--   0 santorum   (501) staff       (20)       70 2021-05-08 16:13:31.000000 scikit-rmt-0.4.2/examples/README.txt
--rw-r--r--   0 santorum   (501) staff       (20)     2155 2021-05-10 19:43:36.000000 scikit-rmt-0.4.2/examples/plot_boosting_density_representation.py
--rw-r--r--   0 santorum   (501) staff       (20)     2559 2021-05-10 19:22:01.000000 scikit-rmt-0.4.2/examples/plot_circular_ensemble.py
--rw-r--r--   0 santorum   (501) staff       (20)     1385 2022-10-04 14:35:07.000000 scikit-rmt-0.4.2/examples/plot_complex_histograms.py
--rw-r--r--   0 santorum   (501) staff       (20)     2651 2021-05-10 18:16:25.000000 scikit-rmt-0.4.2/examples/plot_gaussian_ensemble.py
--rw-r--r--   0 santorum   (501) staff       (20)     3200 2021-05-10 19:13:42.000000 scikit-rmt-0.4.2/examples/plot_manova_ensemble.py
--rw-r--r--   0 santorum   (501) staff       (20)     2417 2021-05-10 19:07:13.000000 scikit-rmt-0.4.2/examples/plot_wishart_ensemble.py
--rw-r--r--   0 santorum   (501) staff       (20)     2293 2021-05-14 20:07:04.000000 scikit-rmt-0.4.2/index.rst
--rw-r--r--   0 santorum   (501) staff       (20)      464 2021-05-08 23:12:18.000000 scikit-rmt-0.4.2/readthedocs.yml
--rw-r--r--   0 santorum   (501) staff       (20)       22 2021-05-14 17:37:20.000000 scikit-rmt-0.4.2/requirements.txt
-drwxr-xr-x   0 santorum   (501) staff       (20)        0 2023-01-27 19:35:36.752923 scikit-rmt-0.4.2/scikit_rmt.egg-info/
--rw-r--r--   0 santorum   (501) staff       (20)    14206 2023-01-27 19:35:36.000000 scikit-rmt-0.4.2/scikit_rmt.egg-info/PKG-INFO
--rw-r--r--   0 santorum   (501) staff       (20)     1617 2023-01-27 19:35:36.000000 scikit-rmt-0.4.2/scikit_rmt.egg-info/SOURCES.txt
--rw-r--r--   0 santorum   (501) staff       (20)        1 2023-01-27 19:35:36.000000 scikit-rmt-0.4.2/scikit_rmt.egg-info/dependency_links.txt
--rw-r--r--   0 santorum   (501) staff       (20)       23 2023-01-27 19:35:36.000000 scikit-rmt-0.4.2/scikit_rmt.egg-info/requires.txt
--rw-r--r--   0 santorum   (501) staff       (20)        6 2023-01-27 19:35:36.000000 scikit-rmt-0.4.2/scikit_rmt.egg-info/top_level.txt
--rw-r--r--   0 santorum   (501) staff       (20)       38 2023-01-27 19:35:36.823436 scikit-rmt-0.4.2/setup.cfg
--rw-r--r--   0 santorum   (501) staff       (20)     2190 2023-01-27 18:55:32.000000 scikit-rmt-0.4.2/setup.py
-drwxr-xr-x   0 santorum   (501) staff       (20)        0 2023-01-27 19:35:36.754773 scikit-rmt-0.4.2/skrmt/
--rw-r--r--   0 santorum   (501) staff       (20)       95 2023-01-27 19:00:33.000000 scikit-rmt-0.4.2/skrmt/__init__.py
--rw-r--r--   0 santorum   (501) staff       (20)       49 2023-01-27 18:33:27.000000 scikit-rmt-0.4.2/skrmt/_version.py
-drwxr-xr-x   0 santorum   (501) staff       (20)        0 2023-01-27 19:35:36.759468 scikit-rmt-0.4.2/skrmt/covariance/
--rw-r--r--   0 santorum   (501) staff       (20)      734 2021-04-28 22:17:52.000000 scikit-rmt-0.4.2/skrmt/covariance/__init__.py
--rw-r--r--   0 santorum   (501) staff       (20)    10347 2021-05-04 14:06:35.000000 scikit-rmt-0.4.2/skrmt/covariance/estimator.py
--rw-r--r--   0 santorum   (501) staff       (20)     3144 2021-04-28 17:36:36.000000 scikit-rmt-0.4.2/skrmt/covariance/metrics.py
-drwxr-xr-x   0 santorum   (501) staff       (20)        0 2023-01-27 19:35:36.763205 scikit-rmt-0.4.2/skrmt/covariance/tests/
--rw-r--r--   0 santorum   (501) staff       (20)        0 2021-04-13 20:20:47.000000 scikit-rmt-0.4.2/skrmt/covariance/tests/__init__.py
--rw-r--r--   0 santorum   (501) staff       (20)     6356 2021-04-28 22:13:28.000000 scikit-rmt-0.4.2/skrmt/covariance/tests/test_estimator.py
--rw-r--r--   0 santorum   (501) staff       (20)     3823 2021-05-02 17:01:05.000000 scikit-rmt-0.4.2/skrmt/covariance/tests/test_metrics.py
-drwxr-xr-x   0 santorum   (501) staff       (20)        0 2023-01-27 19:35:36.785672 scikit-rmt-0.4.2/skrmt/ensemble/
--rw-r--r--   0 santorum   (501) staff       (20)      948 2023-01-05 15:04:32.000000 scikit-rmt-0.4.2/skrmt/ensemble/__init__.py
--rw-r--r--   0 santorum   (501) staff       (20)     9415 2022-10-04 11:57:59.000000 scikit-rmt-0.4.2/skrmt/ensemble/_base_ensemble.py
--rw-r--r--   0 santorum   (501) staff       (20)    12862 2022-10-03 17:59:21.000000 scikit-rmt-0.4.2/skrmt/ensemble/circular_ensemble.py
--rw-r--r--   0 santorum   (501) staff       (20)    13272 2023-01-06 14:35:35.000000 scikit-rmt-0.4.2/skrmt/ensemble/gaussian_ensemble.py
--rw-r--r--   0 santorum   (501) staff       (20)    13203 2023-01-05 15:04:32.000000 scikit-rmt-0.4.2/skrmt/ensemble/manova_ensemble.py
--rw-r--r--   0 santorum   (501) staff       (20)    22788 2023-01-05 15:12:43.000000 scikit-rmt-0.4.2/skrmt/ensemble/plot_law.py
-drwxr-xr-x   0 santorum   (501) staff       (20)        0 2023-01-27 19:35:36.803200 scikit-rmt-0.4.2/skrmt/ensemble/tests/
--rw-r--r--   0 santorum   (501) staff       (20)        0 2021-03-30 20:39:25.000000 scikit-rmt-0.4.2/skrmt/ensemble/tests/__init__.py
--rw-r--r--   0 santorum   (501) staff       (20)     4937 2021-05-02 16:51:08.000000 scikit-rmt-0.4.2/skrmt/ensemble/tests/test_circular_ens.py
--rw-r--r--   0 santorum   (501) staff       (20)    11575 2022-10-04 09:16:08.000000 scikit-rmt-0.4.2/skrmt/ensemble/tests/test_gaussian_ens.py
--rw-r--r--   0 santorum   (501) staff       (20)     5040 2022-10-04 09:45:41.000000 scikit-rmt-0.4.2/skrmt/ensemble/tests/test_manova_ens.py
--rw-r--r--   0 santorum   (501) staff       (20)    19768 2023-01-05 15:04:32.000000 scikit-rmt-0.4.2/skrmt/ensemble/tests/test_plot_law.py
--rw-r--r--   0 santorum   (501) staff       (20)     1611 2023-01-05 15:04:32.000000 scikit-rmt-0.4.2/skrmt/ensemble/tests/test_tracy_widom_approx.py
--rw-r--r--   0 santorum   (501) staff       (20)     1200 2021-05-04 14:00:53.000000 scikit-rmt-0.4.2/skrmt/ensemble/tests/test_tridiagonalization.py
--rw-r--r--   0 santorum   (501) staff       (20)    14238 2022-10-03 15:36:52.000000 scikit-rmt-0.4.2/skrmt/ensemble/tests/test_wishart_ens.py
--rw-r--r--   0 santorum   (501) staff       (20)    30162 2023-01-05 15:04:32.000000 scikit-rmt-0.4.2/skrmt/ensemble/tracy_widom_approximator.py
--rw-r--r--   0 santorum   (501) staff       (20)     6047 2021-05-02 17:53:58.000000 scikit-rmt-0.4.2/skrmt/ensemble/tridiagonal_utils.py
--rw-r--r--   0 santorum   (501) staff       (20)    14357 2023-01-05 15:19:20.000000 scikit-rmt-0.4.2/skrmt/ensemble/wishart_ensemble.py
-drwxr-xr-x   0 santorum   (501) staff       (20)        0 2023-01-27 19:35:36.811883 scikit-rmt-0.4.2/tutorial/
--rw-r--r--   0 santorum   (501) staff       (20)       64 2021-05-09 15:49:23.000000 scikit-rmt-0.4.2/tutorial/README.txt
--rw-r--r--   0 santorum   (501) staff       (20)     2705 2021-05-10 10:23:13.000000 scikit-rmt-0.4.2/tutorial/plot_introduction.py
--rw-r--r--   0 santorum   (501) staff       (20)     8889 2023-01-09 21:36:26.000000 scikit-rmt-0.4.2/tutorial/plot_spectral_laws.py
+drwxr-xr-x   0 santorum   (501) staff       (20)        0 2023-05-06 16:07:34.811442 scikit-rmt-0.5.0/
+-rw-r--r--   0 santorum   (501) staff       (20)      337 2021-05-02 17:28:24.000000 scikit-rmt-0.5.0/.coveragerc
+-rw-r--r--   0 santorum   (501) staff       (20)      278 2023-03-09 19:40:44.000000 scikit-rmt-0.5.0/.travis.yml
+-rw-r--r--   0 santorum   (501) staff       (20)      382 2023-01-27 19:58:20.000000 scikit-rmt-0.5.0/CITATION.cff
+-rw-r--r--   0 santorum   (501) staff       (20)     1563 2021-04-26 20:56:17.000000 scikit-rmt-0.5.0/LICENSE
+-rw-r--r--   0 santorum   (501) staff       (20)      346 2023-01-27 19:52:49.000000 scikit-rmt-0.5.0/MANIFEST.in
+-rw-r--r--   0 santorum   (501) staff       (20)     2569 2021-05-05 17:08:35.000000 scikit-rmt-0.5.0/Makefile
+-rw-r--r--   0 santorum   (501) staff       (20)    19527 2023-05-06 16:07:34.812171 scikit-rmt-0.5.0/PKG-INFO
+-rw-r--r--   0 santorum   (501) staff       (20)    15299 2023-05-06 14:59:09.000000 scikit-rmt-0.5.0/README.md
+-rw-r--r--   0 santorum   (501) staff       (20)     3189 2023-01-27 19:40:29.000000 scikit-rmt-0.5.0/conf.py
+drwxr-xr-x   0 santorum   (501) staff       (20)        0 2023-05-06 16:07:34.654809 scikit-rmt-0.5.0/docs/
+-rw-r--r--   0 santorum   (501) staff       (20)       52 2022-10-04 14:32:13.000000 scikit-rmt-0.5.0/docs/modules.rst
+-rw-r--r--   0 santorum   (501) staff       (20)       54 2021-05-08 23:10:40.000000 scikit-rmt-0.5.0/docs/readthedocs-requirements.txt
+-rw-r--r--   0 santorum   (501) staff       (20)      522 2022-10-04 14:32:13.000000 scikit-rmt-0.5.0/docs/skrmt.covariance.rst
+-rw-r--r--   0 santorum   (501) staff       (20)     1274 2022-10-04 14:32:13.000000 scikit-rmt-0.5.0/docs/skrmt.ensemble.rst
+-rw-r--r--   0 santorum   (501) staff       (20)      232 2022-10-04 14:32:13.000000 scikit-rmt-0.5.0/docs/skrmt.rst
+drwxr-xr-x   0 santorum   (501) staff       (20)        0 2023-05-06 16:07:34.689918 scikit-rmt-0.5.0/examples/
+-rw-r--r--   0 santorum   (501) staff       (20)       70 2021-05-08 16:13:31.000000 scikit-rmt-0.5.0/examples/README.txt
+-rw-r--r--   0 santorum   (501) staff       (20)     2155 2021-05-10 19:43:36.000000 scikit-rmt-0.5.0/examples/plot_boosting_density_representation.py
+-rw-r--r--   0 santorum   (501) staff       (20)     2559 2021-05-10 19:22:01.000000 scikit-rmt-0.5.0/examples/plot_circular_ensemble.py
+-rw-r--r--   0 santorum   (501) staff       (20)     1385 2022-10-04 14:35:07.000000 scikit-rmt-0.5.0/examples/plot_complex_histograms.py
+-rw-r--r--   0 santorum   (501) staff       (20)     2651 2021-05-10 18:16:25.000000 scikit-rmt-0.5.0/examples/plot_gaussian_ensemble.py
+-rw-r--r--   0 santorum   (501) staff       (20)     3200 2021-05-10 19:13:42.000000 scikit-rmt-0.5.0/examples/plot_manova_ensemble.py
+-rw-r--r--   0 santorum   (501) staff       (20)     2417 2021-05-10 19:07:13.000000 scikit-rmt-0.5.0/examples/plot_wishart_ensemble.py
+-rw-r--r--   0 santorum   (501) staff       (20)     2293 2021-05-14 20:07:04.000000 scikit-rmt-0.5.0/index.rst
+-rw-r--r--   0 santorum   (501) staff       (20)      506 2023-05-06 11:49:55.000000 scikit-rmt-0.5.0/readthedocs.yml
+-rw-r--r--   0 santorum   (501) staff       (20)       22 2021-05-14 17:37:20.000000 scikit-rmt-0.5.0/requirements.txt
+drwxr-xr-x   0 santorum   (501) staff       (20)        0 2023-05-06 16:07:34.697134 scikit-rmt-0.5.0/scikit_rmt.egg-info/
+-rw-r--r--   0 santorum   (501) staff       (20)    19527 2023-05-06 16:07:34.000000 scikit-rmt-0.5.0/scikit_rmt.egg-info/PKG-INFO
+-rw-r--r--   0 santorum   (501) staff       (20)     1727 2023-05-06 16:07:34.000000 scikit-rmt-0.5.0/scikit_rmt.egg-info/SOURCES.txt
+-rw-r--r--   0 santorum   (501) staff       (20)        1 2023-05-06 16:07:34.000000 scikit-rmt-0.5.0/scikit_rmt.egg-info/dependency_links.txt
+-rw-r--r--   0 santorum   (501) staff       (20)       23 2023-05-06 16:07:34.000000 scikit-rmt-0.5.0/scikit_rmt.egg-info/requires.txt
+-rw-r--r--   0 santorum   (501) staff       (20)        6 2023-05-06 16:07:34.000000 scikit-rmt-0.5.0/scikit_rmt.egg-info/top_level.txt
+-rw-r--r--   0 santorum   (501) staff       (20)       38 2023-05-06 16:07:34.814241 scikit-rmt-0.5.0/setup.cfg
+-rw-r--r--   0 santorum   (501) staff       (20)     2239 2023-05-06 11:35:01.000000 scikit-rmt-0.5.0/setup.py
+drwxr-xr-x   0 santorum   (501) staff       (20)        0 2023-05-06 16:07:34.710031 scikit-rmt-0.5.0/skrmt/
+-rw-r--r--   0 santorum   (501) staff       (20)       95 2023-01-27 19:00:33.000000 scikit-rmt-0.5.0/skrmt/__init__.py
+-rw-r--r--   0 santorum   (501) staff       (20)       49 2023-05-06 15:21:13.000000 scikit-rmt-0.5.0/skrmt/_version.py
+drwxr-xr-x   0 santorum   (501) staff       (20)        0 2023-05-06 16:07:34.714296 scikit-rmt-0.5.0/skrmt/covariance/
+-rw-r--r--   0 santorum   (501) staff       (20)      734 2021-04-28 22:17:52.000000 scikit-rmt-0.5.0/skrmt/covariance/__init__.py
+-rw-r--r--   0 santorum   (501) staff       (20)    10347 2021-05-04 14:06:35.000000 scikit-rmt-0.5.0/skrmt/covariance/estimator.py
+-rw-r--r--   0 santorum   (501) staff       (20)     3144 2021-04-28 17:36:36.000000 scikit-rmt-0.5.0/skrmt/covariance/metrics.py
+drwxr-xr-x   0 santorum   (501) staff       (20)        0 2023-05-06 16:07:34.726109 scikit-rmt-0.5.0/skrmt/covariance/tests/
+-rw-r--r--   0 santorum   (501) staff       (20)        0 2021-04-13 20:20:47.000000 scikit-rmt-0.5.0/skrmt/covariance/tests/__init__.py
+-rw-r--r--   0 santorum   (501) staff       (20)     6356 2021-04-28 22:13:28.000000 scikit-rmt-0.5.0/skrmt/covariance/tests/test_estimator.py
+-rw-r--r--   0 santorum   (501) staff       (20)     3823 2021-05-02 17:01:05.000000 scikit-rmt-0.5.0/skrmt/covariance/tests/test_metrics.py
+drwxr-xr-x   0 santorum   (501) staff       (20)        0 2023-05-06 16:07:34.793978 scikit-rmt-0.5.0/skrmt/ensemble/
+-rw-r--r--   0 santorum   (501) staff       (20)     1256 2023-05-06 11:35:01.000000 scikit-rmt-0.5.0/skrmt/ensemble/__init__.py
+-rw-r--r--   0 santorum   (501) staff       (20)     9331 2023-05-06 11:35:01.000000 scikit-rmt-0.5.0/skrmt/ensemble/_base_ensemble.py
+-rw-r--r--   0 santorum   (501) staff       (20)    12876 2023-05-06 11:35:01.000000 scikit-rmt-0.5.0/skrmt/ensemble/circular_ensemble.py
+-rw-r--r--   0 santorum   (501) staff       (20)    14169 2023-05-06 11:35:01.000000 scikit-rmt-0.5.0/skrmt/ensemble/gaussian_ensemble.py
+-rw-r--r--   0 santorum   (501) staff       (20)    33491 2023-05-06 11:35:01.000000 scikit-rmt-0.5.0/skrmt/ensemble/law.py
+-rw-r--r--   0 santorum   (501) staff       (20)    13192 2023-05-06 11:35:01.000000 scikit-rmt-0.5.0/skrmt/ensemble/manova_ensemble.py
+-rw-r--r--   0 santorum   (501) staff       (20)    21317 2023-05-06 11:35:01.000000 scikit-rmt-0.5.0/skrmt/ensemble/plot_law.py
+drwxr-xr-x   0 santorum   (501) staff       (20)        0 2023-05-06 16:07:34.807378 scikit-rmt-0.5.0/skrmt/ensemble/tests/
+-rw-r--r--   0 santorum   (501) staff       (20)        0 2021-03-30 20:39:25.000000 scikit-rmt-0.5.0/skrmt/ensemble/tests/__init__.py
+-rw-r--r--   0 santorum   (501) staff       (20)     4937 2021-05-02 16:51:08.000000 scikit-rmt-0.5.0/skrmt/ensemble/tests/test_circular_ens.py
+-rw-r--r--   0 santorum   (501) staff       (20)    11902 2023-05-06 11:35:01.000000 scikit-rmt-0.5.0/skrmt/ensemble/tests/test_gaussian_ens.py
+-rw-r--r--   0 santorum   (501) staff       (20)    18193 2023-05-06 11:35:01.000000 scikit-rmt-0.5.0/skrmt/ensemble/tests/test_law.py
+-rw-r--r--   0 santorum   (501) staff       (20)     5040 2023-03-18 23:10:48.000000 scikit-rmt-0.5.0/skrmt/ensemble/tests/test_manova_ens.py
+-rw-r--r--   0 santorum   (501) staff       (20)    19622 2023-05-06 11:35:01.000000 scikit-rmt-0.5.0/skrmt/ensemble/tests/test_plot_law.py
+-rw-r--r--   0 santorum   (501) staff       (20)     1611 2023-01-05 15:04:32.000000 scikit-rmt-0.5.0/skrmt/ensemble/tests/test_tracy_widom_approx.py
+-rw-r--r--   0 santorum   (501) staff       (20)     1200 2021-05-04 14:00:53.000000 scikit-rmt-0.5.0/skrmt/ensemble/tests/test_tridiagonalization.py
+-rw-r--r--   0 santorum   (501) staff       (20)    14644 2023-05-06 11:35:01.000000 scikit-rmt-0.5.0/skrmt/ensemble/tests/test_wishart_ens.py
+-rw-r--r--   0 santorum   (501) staff       (20)    33083 2023-05-06 11:35:01.000000 scikit-rmt-0.5.0/skrmt/ensemble/tracy_widom_approximator.py
+-rw-r--r--   0 santorum   (501) staff       (20)     6028 2023-05-06 11:35:01.000000 scikit-rmt-0.5.0/skrmt/ensemble/tridiagonal_utils.py
+-rw-r--r--   0 santorum   (501) staff       (20)    15746 2023-05-06 11:35:01.000000 scikit-rmt-0.5.0/skrmt/ensemble/wishart_ensemble.py
+drwxr-xr-x   0 santorum   (501) staff       (20)        0 2023-05-06 16:07:34.810743 scikit-rmt-0.5.0/tutorial/
+-rw-r--r--   0 santorum   (501) staff       (20)       64 2021-05-09 15:49:23.000000 scikit-rmt-0.5.0/tutorial/README.txt
+-rw-r--r--   0 santorum   (501) staff       (20)     2705 2023-05-06 11:35:01.000000 scikit-rmt-0.5.0/tutorial/plot_0_introduction.py
+-rw-r--r--   0 santorum   (501) staff       (20)    10227 2023-05-06 13:37:21.000000 scikit-rmt-0.5.0/tutorial/plot_1_spectral_laws.py
+-rw-r--r--   0 santorum   (501) staff       (20)     8822 2023-05-06 12:57:57.000000 scikit-rmt-0.5.0/tutorial/plot_2_plot_spectral_laws.py
```

### Comparing `scikit-rmt-0.4.2/LICENSE` & `scikit-rmt-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.4.2/Makefile` & `scikit-rmt-0.5.0/Makefile`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.4.2/PKG-INFO` & `scikit-rmt-0.5.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 Metadata-Version: 2.1
 Name: scikit-rmt
-Version: 0.4.2
+Version: 0.5.0
 Summary: Random Matrix Theory Python package
 Home-page: https://github.com/AlejandroSantorum/scikit-rmt
 Author: Alejandro Santorum Varela
 Author-email: alejandro.santorum@gmail.com
 License: BSD
-Download-URL: https://github.com/AlejandroSantorum/scikit-rmt/archive/refs/tags/v0.4.2.tar.gz
-Description: [![PyPI](https://img.shields.io/pypi/v/scikit-rmt?color=g)](https://pypi.org/project/scikit-rmt/)
+Download-URL: https://github.com/AlejandroSantorum/scikit-rmt/archive/refs/tags/v0.5.0.tar.gz
+Description: ![scikit-rmt logo](https://raw.githubusercontent.com/AlejandroSantorum/scikit-rmt/main/imgs/scikit-rmt_logo_bigger.png)
+        
+        
+        [![PyPI](https://img.shields.io/pypi/v/scikit-rmt?color=g)](https://pypi.org/project/scikit-rmt/)
         [![Documentation Status](https://readthedocs.org/projects/scikit-rmt/badge/?version=latest)](https://scikit-rmt.readthedocs.io/en/latest/?badge=latest)
         [![Build Status](https://travis-ci.com/AlejandroSantorum/scikit-rmt.svg?branch=main)](https://travis-ci.com/AlejandroSantorum/scikit-rmt)
         [![codecov](https://codecov.io/gh/AlejandroSantorum/scikit-rmt/branch/main/graph/badge.svg?token=56TNEASPJK)](https://codecov.io/gh/AlejandroSantorum/scikit-rmt)
         [![License Status](https://img.shields.io/github/license/AlejandroSantorum/scikit-rmt?color=blue)](https://github.com/AlejandroSantorum/scikit-rmt/blob/main/LICENSE)
         [![PyPI-Python Version](https://img.shields.io/pypi/pyversions/scikit-rmt)](https://pypi.org/project/scikit-rmt)
         
         
@@ -196,14 +199,135 @@
         tracy_widom_law(ensemble='goe', n_size=500, times=20000, bins=80, density=True, limit_pdf=True)
         ```
         ![Tracy-Widom Law PDF](https://raw.githubusercontent.com/AlejandroSantorum/scikit-rmt/main/imgs/twl_goe_pdf.png)
         <!---
         <img src="imgs/twl_goe_pdf.png" width=450 height=320 alt="Tracy-Widom Law PDF">
         -->
         
+        The proposed package **scikit-rmt** also provides support for **computing and analyzing** the **probability density function (PDF)** and **cumulative distribution function (CDF)** of the main random matrix ensembles. In particular, the following classes are implemented in the `ensemble.law` module:
+        - `WignerSemicircleDistribution` in `skrmt.ensemble.law`.
+        - `MarchenkoPasturDistribution` in `skrmt.ensemble.law`.
+        - `TracyWidomDistribution` in `skrmt.ensemble.law`.
+        - `ManovaSpectrumDistribution` in `skrmt.ensemble.law`.
+        
+        For example, `WignerSemicircleDistribution` can be used to plot the **Wigner's Semicircle Law PDF**:
+        ```python
+        import numpy as np
+        import matplotlib.pyplot as plt
+        from skrmt.ensemble.law import WignerSemicircleDistribution
+        
+        x1 = np.linspace(-5, 5, num=1000)
+        x2 = np.linspace(-10, 10, num=2000)
+        
+        fig, (ax1, ax2) = plt.subplots(1, 2, figsize=(12,4))
+        
+        for sigma in [0.5, 1.0, 2.0, 4.0]:
+            wsd = WignerSemicircleDistribution(beta=1, center=0.0, sigma=sigma)
+        
+            y1 = wsd.pdf(x1)
+            y2 = wsd.pdf(x2)
+        
+            ax1.plot(x1, y1, label=f"$\sigma$ = {sigma} (R = ${wsd.radius}$)")
+            ax2.plot(x2, y2, label=f"$\sigma$ = {sigma} (R = ${wsd.radius}$)")
+        
+        ax1.legend()
+        ax1.set_xlabel("x", fontweight="bold")
+        ax1.set_xticks([-5, -4, -3, -2, -1, 0, 1, 2, 3, 4, 5])
+        ax1.set_ylabel("density", fontweight="bold")
+        
+        ax2.legend()
+        ax2.set_xlabel("x", fontweight="bold")
+        ax2.set_xticks([-10, -8, -6, -4, -2, 0, 2, 4, 6, 8, 10])
+        ax2.set_ylabel("density", fontweight="bold")
+        
+        fig.suptitle("Wigner Semicircle probability density function (PDF)", fontweight="bold")
+        plt.show()
+        ```
+        ![Wigner Semicircle Law PDF (Analytical)](https://raw.githubusercontent.com/AlejandroSantorum/scikit-rmt/main/imgs/wigner_scl_pdf.png)
+        <!---
+        <img src="imgs/wigner_scl_pdf.png" width=450 height=320 alt="Wigner Semicircle Law PDF (Analytical)">
+        -->
+        
+        Similarly, `MarchenkoPasturDistribution` can be used to plot the **Marchenko-Pastur Law PDF**:
+        ```python
+        import numpy as np
+        import matplotlib.pyplot as plt
+        from skrmt.ensemble.law import MarchenkoPasturDistribution
+        
+        x1 = np.linspace(0, 4, num=1000)
+        x2 = np.linspace(0, 5, num=2000)
+        
+        fig, (ax1, ax2) = plt.subplots(1, 2, figsize=(12,4))
+        
+        for ratio in [0.2, 0.4, 0.6, 1.0, 1.4]:
+            mpl = MarchenkoPasturDistribution(beta=1, ratio=ratio, sigma=1.0)
+        
+            y1 = mpl.pdf(x1)
+            y2 = mpl.pdf(x2)
+        
+            ax1.plot(x1, y1, label=f"$\lambda$ = {ratio} ")
+            ax2.plot(x2, y2, label=f"$\lambda$ = {ratio} ")
+        
+        ax1.legend()
+        ax1.set_ylim(0, 1.4)
+        ax1.set_xlabel("x", fontweight="bold")
+        ax1.set_ylabel("density", fontweight="bold")
+        
+        ax2.legend()
+        ax2.set_ylim(0, 1.4)
+        ax2.set_xlim(0, 1)
+        ax2.set_xlabel("x", fontweight="bold")
+        ax2.set_ylabel("density", fontweight="bold")
+        
+        fig.suptitle("Marchenko-Pastur probability density function (PDF)", fontweight="bold")
+        plt.show()
+        ```
+        ![Marchenko-Pastur Law PDF (Analytical)](https://raw.githubusercontent.com/AlejandroSantorum/scikit-rmt/main/imgs/mpl_pdf.png)
+        <!---
+        <img src="imgs/mpl_pdf.png" width=450 height=320 alt="Marchenko-Pastur Law PDF (Analytical)">
+        -->
+        
+        In the following example, we show how we can plot the **PDF and CDF of the Tracy-Widom distribution** using the class `TracyWidomDistribution`:
+        ```python
+        import numpy as np
+        import matplotlib.pyplot as plt
+        from skrmt.ensemble.law import TracyWidomDistribution
+        
+        x = np.linspace(-5, 2, num=1000)
+        
+        fig, (ax1, ax2) = plt.subplots(1, 2, figsize=(12,4))
+        
+        for beta in [1,2,4]:
+            twd = TracyWidomDistribution(beta=beta)
+        
+            y_pdf = twd.pdf(x)
+            y_cdf = twd.cdf(x)
+        
+            ax1.plot(x, y_pdf, label=f"$\\beta$ = {beta}")
+            ax2.plot(x, y_cdf, label=f"$\\beta$ = {beta}")
+        
+        ax1.legend()
+        ax1.set_xlabel("x", fontweight="bold")
+        ax1.set_ylabel("density", fontweight="bold")
+        ax1.set_title("Probability density function")
+        
+        ax2.legend()
+        ax2.set_xlabel("x", fontweight="bold")
+        ax2.set_ylabel("distribution", fontweight="bold")
+        ax2.set_title("Cumulative distribution function")
+        
+        fig.suptitle("Tracy Widom Law", fontweight="bold")
+        plt.show()
+        ```
+        ![Tracy-Widom Law PDF and CDF(Analytical)](https://raw.githubusercontent.com/AlejandroSantorum/scikit-rmt/main/imgs/twl_pdf_cdf.png)
+        <!---
+        <img src="imgs/twl_pdf_cdf.png" width=450 height=320 alt="Tracy-Widom Law PDF and CDF(Analytical)">
+        -->
+        
+        
         The other module of this library implements **several covariance matrix estimators**:
         * Sample estimator.
         * Finite-sample optimal estimator (FSOpt estimator).
         * Non-linear shrinkage analytical estimator (Ledoit & Wolf, 2020).
         * Linear shrinkage estimator (Ledoit & Wolf, 2004).
         * Empirical Bayesian estimator (Haff, 1980).
         * Minimax estimator (Stain, 1982).
@@ -279,23 +403,21 @@
           title = {scikit-rmt},
           year = {2021},
           howpublished = {\url{https://github.com/AlejandroSantorum/scikit-rmt}},
           note = {GitHub repository}
         }
         ```
         
-        
-        
-        
 Keywords: RMT,Random Matrix Theory,Ensemble,Covariance matrices
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
```

### Comparing `scikit-rmt-0.4.2/README.md` & `scikit-rmt-0.5.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+![scikit-rmt logo](https://raw.githubusercontent.com/AlejandroSantorum/scikit-rmt/main/imgs/scikit-rmt_logo_bigger.png)
+
+
 [![PyPI](https://img.shields.io/pypi/v/scikit-rmt?color=g)](https://pypi.org/project/scikit-rmt/)
 [![Documentation Status](https://readthedocs.org/projects/scikit-rmt/badge/?version=latest)](https://scikit-rmt.readthedocs.io/en/latest/?badge=latest)
 [![Build Status](https://travis-ci.com/AlejandroSantorum/scikit-rmt.svg?branch=main)](https://travis-ci.com/AlejandroSantorum/scikit-rmt)
 [![codecov](https://codecov.io/gh/AlejandroSantorum/scikit-rmt/branch/main/graph/badge.svg?token=56TNEASPJK)](https://codecov.io/gh/AlejandroSantorum/scikit-rmt)
 [![License Status](https://img.shields.io/github/license/AlejandroSantorum/scikit-rmt?color=blue)](https://github.com/AlejandroSantorum/scikit-rmt/blob/main/LICENSE)
 [![PyPI-Python Version](https://img.shields.io/pypi/pyversions/scikit-rmt)](https://pypi.org/project/scikit-rmt)
 
@@ -187,14 +190,135 @@
 tracy_widom_law(ensemble='goe', n_size=500, times=20000, bins=80, density=True, limit_pdf=True)
 ```
 ![Tracy-Widom Law PDF](https://raw.githubusercontent.com/AlejandroSantorum/scikit-rmt/main/imgs/twl_goe_pdf.png)
 <!---
 <img src="imgs/twl_goe_pdf.png" width=450 height=320 alt="Tracy-Widom Law PDF">
 -->
 
+The proposed package **scikit-rmt** also provides support for **computing and analyzing** the **probability density function (PDF)** and **cumulative distribution function (CDF)** of the main random matrix ensembles. In particular, the following classes are implemented in the `ensemble.law` module:
+- `WignerSemicircleDistribution` in `skrmt.ensemble.law`.
+- `MarchenkoPasturDistribution` in `skrmt.ensemble.law`.
+- `TracyWidomDistribution` in `skrmt.ensemble.law`.
+- `ManovaSpectrumDistribution` in `skrmt.ensemble.law`.
+
+For example, `WignerSemicircleDistribution` can be used to plot the **Wigner's Semicircle Law PDF**:
+```python
+import numpy as np
+import matplotlib.pyplot as plt
+from skrmt.ensemble.law import WignerSemicircleDistribution
+
+x1 = np.linspace(-5, 5, num=1000)
+x2 = np.linspace(-10, 10, num=2000)
+
+fig, (ax1, ax2) = plt.subplots(1, 2, figsize=(12,4))
+
+for sigma in [0.5, 1.0, 2.0, 4.0]:
+    wsd = WignerSemicircleDistribution(beta=1, center=0.0, sigma=sigma)
+
+    y1 = wsd.pdf(x1)
+    y2 = wsd.pdf(x2)
+
+    ax1.plot(x1, y1, label=f"$\sigma$ = {sigma} (R = ${wsd.radius}$)")
+    ax2.plot(x2, y2, label=f"$\sigma$ = {sigma} (R = ${wsd.radius}$)")
+
+ax1.legend()
+ax1.set_xlabel("x", fontweight="bold")
+ax1.set_xticks([-5, -4, -3, -2, -1, 0, 1, 2, 3, 4, 5])
+ax1.set_ylabel("density", fontweight="bold")
+
+ax2.legend()
+ax2.set_xlabel("x", fontweight="bold")
+ax2.set_xticks([-10, -8, -6, -4, -2, 0, 2, 4, 6, 8, 10])
+ax2.set_ylabel("density", fontweight="bold")
+
+fig.suptitle("Wigner Semicircle probability density function (PDF)", fontweight="bold")
+plt.show()
+```
+![Wigner Semicircle Law PDF (Analytical)](https://raw.githubusercontent.com/AlejandroSantorum/scikit-rmt/main/imgs/wigner_scl_pdf.png)
+<!---
+<img src="imgs/wigner_scl_pdf.png" width=450 height=320 alt="Wigner Semicircle Law PDF (Analytical)">
+-->
+
+Similarly, `MarchenkoPasturDistribution` can be used to plot the **Marchenko-Pastur Law PDF**:
+```python
+import numpy as np
+import matplotlib.pyplot as plt
+from skrmt.ensemble.law import MarchenkoPasturDistribution
+
+x1 = np.linspace(0, 4, num=1000)
+x2 = np.linspace(0, 5, num=2000)
+
+fig, (ax1, ax2) = plt.subplots(1, 2, figsize=(12,4))
+
+for ratio in [0.2, 0.4, 0.6, 1.0, 1.4]:
+    mpl = MarchenkoPasturDistribution(beta=1, ratio=ratio, sigma=1.0)
+
+    y1 = mpl.pdf(x1)
+    y2 = mpl.pdf(x2)
+
+    ax1.plot(x1, y1, label=f"$\lambda$ = {ratio} ")
+    ax2.plot(x2, y2, label=f"$\lambda$ = {ratio} ")
+
+ax1.legend()
+ax1.set_ylim(0, 1.4)
+ax1.set_xlabel("x", fontweight="bold")
+ax1.set_ylabel("density", fontweight="bold")
+
+ax2.legend()
+ax2.set_ylim(0, 1.4)
+ax2.set_xlim(0, 1)
+ax2.set_xlabel("x", fontweight="bold")
+ax2.set_ylabel("density", fontweight="bold")
+
+fig.suptitle("Marchenko-Pastur probability density function (PDF)", fontweight="bold")
+plt.show()
+```
+![Marchenko-Pastur Law PDF (Analytical)](https://raw.githubusercontent.com/AlejandroSantorum/scikit-rmt/main/imgs/mpl_pdf.png)
+<!---
+<img src="imgs/mpl_pdf.png" width=450 height=320 alt="Marchenko-Pastur Law PDF (Analytical)">
+-->
+
+In the following example, we show how we can plot the **PDF and CDF of the Tracy-Widom distribution** using the class `TracyWidomDistribution`:
+```python
+import numpy as np
+import matplotlib.pyplot as plt
+from skrmt.ensemble.law import TracyWidomDistribution
+
+x = np.linspace(-5, 2, num=1000)
+
+fig, (ax1, ax2) = plt.subplots(1, 2, figsize=(12,4))
+
+for beta in [1,2,4]:
+    twd = TracyWidomDistribution(beta=beta)
+
+    y_pdf = twd.pdf(x)
+    y_cdf = twd.cdf(x)
+
+    ax1.plot(x, y_pdf, label=f"$\\beta$ = {beta}")
+    ax2.plot(x, y_cdf, label=f"$\\beta$ = {beta}")
+
+ax1.legend()
+ax1.set_xlabel("x", fontweight="bold")
+ax1.set_ylabel("density", fontweight="bold")
+ax1.set_title("Probability density function")
+
+ax2.legend()
+ax2.set_xlabel("x", fontweight="bold")
+ax2.set_ylabel("distribution", fontweight="bold")
+ax2.set_title("Cumulative distribution function")
+
+fig.suptitle("Tracy Widom Law", fontweight="bold")
+plt.show()
+```
+![Tracy-Widom Law PDF and CDF(Analytical)](https://raw.githubusercontent.com/AlejandroSantorum/scikit-rmt/main/imgs/twl_pdf_cdf.png)
+<!---
+<img src="imgs/twl_pdf_cdf.png" width=450 height=320 alt="Tracy-Widom Law PDF and CDF(Analytical)">
+-->
+
+
 The other module of this library implements **several covariance matrix estimators**:
 * Sample estimator.
 * Finite-sample optimal estimator (FSOpt estimator).
 * Non-linear shrinkage analytical estimator (Ledoit & Wolf, 2020).
 * Linear shrinkage estimator (Ledoit & Wolf, 2004).
 * Empirical Bayesian estimator (Haff, 1980).
 * Minimax estimator (Stain, 1982).
@@ -269,10 +393,7 @@
   author = {A. Santorum},
   title = {scikit-rmt},
   year = {2021},
   howpublished = {\url{https://github.com/AlejandroSantorum/scikit-rmt}},
   note = {GitHub repository}
 }
 ```
-
-
-
```

### Comparing `scikit-rmt-0.4.2/conf.py` & `scikit-rmt-0.5.0/conf.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,28 +7,39 @@
 # -- Path setup --------------------------------------------------------------
 
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 #
 import os
+import re
 import sys
 sys.path.insert(0, os.path.abspath('.'))
 sys.path.append('skrmt')
 
 
 # -- Project information -----------------------------------------------------
 
 project = 'scikit-rmt'
 copyright = '2021, Alejandro Santorum Varela'
 author = 'Alejandro Santorum Varela'
 
 # The full version, including alpha/beta/rc tags
-with open("VERSION", "r") as version_file:
-    release = version_file.read().strip()
+VERSION_FILEPATH = "skrmt/_version.py"
+with open(
+    os.path.join(os.path.dirname(__file__), VERSION_FILEPATH),
+    "r",
+) as version_file:
+    version_file_text = version_file.read()
+    VSRE = r"^__version__ = ['\"]([^'\"]*)['\"]"
+    match = re.search(VSRE, version_file_text, re.M)
+    if match:
+        release = match.group(1)
+    else:
+        raise RuntimeError(f"Unable to find version in {VERSION_FILEPATH}.")
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
```

### Comparing `scikit-rmt-0.4.2/docs/skrmt.covariance.rst` & `scikit-rmt-0.5.0/docs/skrmt.covariance.rst`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.4.2/docs/skrmt.ensemble.rst` & `scikit-rmt-0.5.0/docs/skrmt.ensemble.rst`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.4.2/examples/plot_boosting_density_representation.py` & `scikit-rmt-0.5.0/examples/plot_boosting_density_representation.py`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.4.2/examples/plot_circular_ensemble.py` & `scikit-rmt-0.5.0/examples/plot_circular_ensemble.py`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.4.2/examples/plot_complex_histograms.py` & `scikit-rmt-0.5.0/examples/plot_complex_histograms.py`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.4.2/examples/plot_gaussian_ensemble.py` & `scikit-rmt-0.5.0/examples/plot_gaussian_ensemble.py`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.4.2/examples/plot_manova_ensemble.py` & `scikit-rmt-0.5.0/examples/plot_manova_ensemble.py`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.4.2/examples/plot_wishart_ensemble.py` & `scikit-rmt-0.5.0/examples/plot_wishart_ensemble.py`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.4.2/index.rst` & `scikit-rmt-0.5.0/index.rst`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.4.2/scikit_rmt.egg-info/PKG-INFO` & `scikit-rmt-0.5.0/scikit_rmt.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 Metadata-Version: 2.1
 Name: scikit-rmt
-Version: 0.4.2
+Version: 0.5.0
 Summary: Random Matrix Theory Python package
 Home-page: https://github.com/AlejandroSantorum/scikit-rmt
 Author: Alejandro Santorum Varela
 Author-email: alejandro.santorum@gmail.com
 License: BSD
-Download-URL: https://github.com/AlejandroSantorum/scikit-rmt/archive/refs/tags/v0.4.2.tar.gz
-Description: [![PyPI](https://img.shields.io/pypi/v/scikit-rmt?color=g)](https://pypi.org/project/scikit-rmt/)
+Download-URL: https://github.com/AlejandroSantorum/scikit-rmt/archive/refs/tags/v0.5.0.tar.gz
+Description: ![scikit-rmt logo](https://raw.githubusercontent.com/AlejandroSantorum/scikit-rmt/main/imgs/scikit-rmt_logo_bigger.png)
+        
+        
+        [![PyPI](https://img.shields.io/pypi/v/scikit-rmt?color=g)](https://pypi.org/project/scikit-rmt/)
         [![Documentation Status](https://readthedocs.org/projects/scikit-rmt/badge/?version=latest)](https://scikit-rmt.readthedocs.io/en/latest/?badge=latest)
         [![Build Status](https://travis-ci.com/AlejandroSantorum/scikit-rmt.svg?branch=main)](https://travis-ci.com/AlejandroSantorum/scikit-rmt)
         [![codecov](https://codecov.io/gh/AlejandroSantorum/scikit-rmt/branch/main/graph/badge.svg?token=56TNEASPJK)](https://codecov.io/gh/AlejandroSantorum/scikit-rmt)
         [![License Status](https://img.shields.io/github/license/AlejandroSantorum/scikit-rmt?color=blue)](https://github.com/AlejandroSantorum/scikit-rmt/blob/main/LICENSE)
         [![PyPI-Python Version](https://img.shields.io/pypi/pyversions/scikit-rmt)](https://pypi.org/project/scikit-rmt)
         
         
@@ -196,14 +199,135 @@
         tracy_widom_law(ensemble='goe', n_size=500, times=20000, bins=80, density=True, limit_pdf=True)
         ```
         ![Tracy-Widom Law PDF](https://raw.githubusercontent.com/AlejandroSantorum/scikit-rmt/main/imgs/twl_goe_pdf.png)
         <!---
         <img src="imgs/twl_goe_pdf.png" width=450 height=320 alt="Tracy-Widom Law PDF">
         -->
         
+        The proposed package **scikit-rmt** also provides support for **computing and analyzing** the **probability density function (PDF)** and **cumulative distribution function (CDF)** of the main random matrix ensembles. In particular, the following classes are implemented in the `ensemble.law` module:
+        - `WignerSemicircleDistribution` in `skrmt.ensemble.law`.
+        - `MarchenkoPasturDistribution` in `skrmt.ensemble.law`.
+        - `TracyWidomDistribution` in `skrmt.ensemble.law`.
+        - `ManovaSpectrumDistribution` in `skrmt.ensemble.law`.
+        
+        For example, `WignerSemicircleDistribution` can be used to plot the **Wigner's Semicircle Law PDF**:
+        ```python
+        import numpy as np
+        import matplotlib.pyplot as plt
+        from skrmt.ensemble.law import WignerSemicircleDistribution
+        
+        x1 = np.linspace(-5, 5, num=1000)
+        x2 = np.linspace(-10, 10, num=2000)
+        
+        fig, (ax1, ax2) = plt.subplots(1, 2, figsize=(12,4))
+        
+        for sigma in [0.5, 1.0, 2.0, 4.0]:
+            wsd = WignerSemicircleDistribution(beta=1, center=0.0, sigma=sigma)
+        
+            y1 = wsd.pdf(x1)
+            y2 = wsd.pdf(x2)
+        
+            ax1.plot(x1, y1, label=f"$\sigma$ = {sigma} (R = ${wsd.radius}$)")
+            ax2.plot(x2, y2, label=f"$\sigma$ = {sigma} (R = ${wsd.radius}$)")
+        
+        ax1.legend()
+        ax1.set_xlabel("x", fontweight="bold")
+        ax1.set_xticks([-5, -4, -3, -2, -1, 0, 1, 2, 3, 4, 5])
+        ax1.set_ylabel("density", fontweight="bold")
+        
+        ax2.legend()
+        ax2.set_xlabel("x", fontweight="bold")
+        ax2.set_xticks([-10, -8, -6, -4, -2, 0, 2, 4, 6, 8, 10])
+        ax2.set_ylabel("density", fontweight="bold")
+        
+        fig.suptitle("Wigner Semicircle probability density function (PDF)", fontweight="bold")
+        plt.show()
+        ```
+        ![Wigner Semicircle Law PDF (Analytical)](https://raw.githubusercontent.com/AlejandroSantorum/scikit-rmt/main/imgs/wigner_scl_pdf.png)
+        <!---
+        <img src="imgs/wigner_scl_pdf.png" width=450 height=320 alt="Wigner Semicircle Law PDF (Analytical)">
+        -->
+        
+        Similarly, `MarchenkoPasturDistribution` can be used to plot the **Marchenko-Pastur Law PDF**:
+        ```python
+        import numpy as np
+        import matplotlib.pyplot as plt
+        from skrmt.ensemble.law import MarchenkoPasturDistribution
+        
+        x1 = np.linspace(0, 4, num=1000)
+        x2 = np.linspace(0, 5, num=2000)
+        
+        fig, (ax1, ax2) = plt.subplots(1, 2, figsize=(12,4))
+        
+        for ratio in [0.2, 0.4, 0.6, 1.0, 1.4]:
+            mpl = MarchenkoPasturDistribution(beta=1, ratio=ratio, sigma=1.0)
+        
+            y1 = mpl.pdf(x1)
+            y2 = mpl.pdf(x2)
+        
+            ax1.plot(x1, y1, label=f"$\lambda$ = {ratio} ")
+            ax2.plot(x2, y2, label=f"$\lambda$ = {ratio} ")
+        
+        ax1.legend()
+        ax1.set_ylim(0, 1.4)
+        ax1.set_xlabel("x", fontweight="bold")
+        ax1.set_ylabel("density", fontweight="bold")
+        
+        ax2.legend()
+        ax2.set_ylim(0, 1.4)
+        ax2.set_xlim(0, 1)
+        ax2.set_xlabel("x", fontweight="bold")
+        ax2.set_ylabel("density", fontweight="bold")
+        
+        fig.suptitle("Marchenko-Pastur probability density function (PDF)", fontweight="bold")
+        plt.show()
+        ```
+        ![Marchenko-Pastur Law PDF (Analytical)](https://raw.githubusercontent.com/AlejandroSantorum/scikit-rmt/main/imgs/mpl_pdf.png)
+        <!---
+        <img src="imgs/mpl_pdf.png" width=450 height=320 alt="Marchenko-Pastur Law PDF (Analytical)">
+        -->
+        
+        In the following example, we show how we can plot the **PDF and CDF of the Tracy-Widom distribution** using the class `TracyWidomDistribution`:
+        ```python
+        import numpy as np
+        import matplotlib.pyplot as plt
+        from skrmt.ensemble.law import TracyWidomDistribution
+        
+        x = np.linspace(-5, 2, num=1000)
+        
+        fig, (ax1, ax2) = plt.subplots(1, 2, figsize=(12,4))
+        
+        for beta in [1,2,4]:
+            twd = TracyWidomDistribution(beta=beta)
+        
+            y_pdf = twd.pdf(x)
+            y_cdf = twd.cdf(x)
+        
+            ax1.plot(x, y_pdf, label=f"$\\beta$ = {beta}")
+            ax2.plot(x, y_cdf, label=f"$\\beta$ = {beta}")
+        
+        ax1.legend()
+        ax1.set_xlabel("x", fontweight="bold")
+        ax1.set_ylabel("density", fontweight="bold")
+        ax1.set_title("Probability density function")
+        
+        ax2.legend()
+        ax2.set_xlabel("x", fontweight="bold")
+        ax2.set_ylabel("distribution", fontweight="bold")
+        ax2.set_title("Cumulative distribution function")
+        
+        fig.suptitle("Tracy Widom Law", fontweight="bold")
+        plt.show()
+        ```
+        ![Tracy-Widom Law PDF and CDF(Analytical)](https://raw.githubusercontent.com/AlejandroSantorum/scikit-rmt/main/imgs/twl_pdf_cdf.png)
+        <!---
+        <img src="imgs/twl_pdf_cdf.png" width=450 height=320 alt="Tracy-Widom Law PDF and CDF(Analytical)">
+        -->
+        
+        
         The other module of this library implements **several covariance matrix estimators**:
         * Sample estimator.
         * Finite-sample optimal estimator (FSOpt estimator).
         * Non-linear shrinkage analytical estimator (Ledoit & Wolf, 2020).
         * Linear shrinkage estimator (Ledoit & Wolf, 2004).
         * Empirical Bayesian estimator (Haff, 1980).
         * Minimax estimator (Stain, 1982).
@@ -279,23 +403,21 @@
           title = {scikit-rmt},
           year = {2021},
           howpublished = {\url{https://github.com/AlejandroSantorum/scikit-rmt}},
           note = {GitHub repository}
         }
         ```
         
-        
-        
-        
 Keywords: RMT,Random Matrix Theory,Ensemble,Covariance matrices
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
```

### Comparing `scikit-rmt-0.4.2/scikit_rmt.egg-info/SOURCES.txt` & `scikit-rmt-0.5.0/scikit_rmt.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 .coveragerc
 .travis.yml
+CITATION.cff
 LICENSE
 MANIFEST.in
 Makefile
 README.md
 conf.py
 index.rst
 readthedocs.yml
@@ -35,23 +36,26 @@
 skrmt/covariance/tests/__init__.py
 skrmt/covariance/tests/test_estimator.py
 skrmt/covariance/tests/test_metrics.py
 skrmt/ensemble/__init__.py
 skrmt/ensemble/_base_ensemble.py
 skrmt/ensemble/circular_ensemble.py
 skrmt/ensemble/gaussian_ensemble.py
+skrmt/ensemble/law.py
 skrmt/ensemble/manova_ensemble.py
 skrmt/ensemble/plot_law.py
 skrmt/ensemble/tracy_widom_approximator.py
 skrmt/ensemble/tridiagonal_utils.py
 skrmt/ensemble/wishart_ensemble.py
 skrmt/ensemble/tests/__init__.py
 skrmt/ensemble/tests/test_circular_ens.py
 skrmt/ensemble/tests/test_gaussian_ens.py
+skrmt/ensemble/tests/test_law.py
 skrmt/ensemble/tests/test_manova_ens.py
 skrmt/ensemble/tests/test_plot_law.py
 skrmt/ensemble/tests/test_tracy_widom_approx.py
 skrmt/ensemble/tests/test_tridiagonalization.py
 skrmt/ensemble/tests/test_wishart_ens.py
 tutorial/README.txt
-tutorial/plot_introduction.py
-tutorial/plot_spectral_laws.py
+tutorial/plot_0_introduction.py
+tutorial/plot_1_spectral_laws.py
+tutorial/plot_2_plot_spectral_laws.py
```

### Comparing `scikit-rmt-0.4.2/setup.py` & `scikit-rmt-0.5.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -56,11 +56,12 @@
         'Intended Audience :: Developers',
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: BSD License',
         'Natural Language :: English',
         'Operating System :: OS Independent',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
         'Topic :: Scientific/Engineering :: Mathematics',
         'Topic :: Software Development :: Libraries :: Python Modules',
     ],
 )
```

### Comparing `scikit-rmt-0.4.2/skrmt/covariance/__init__.py` & `scikit-rmt-0.5.0/skrmt/covariance/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.4.2/skrmt/covariance/estimator.py` & `scikit-rmt-0.5.0/skrmt/covariance/estimator.py`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.4.2/skrmt/covariance/metrics.py` & `scikit-rmt-0.5.0/skrmt/covariance/metrics.py`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.4.2/skrmt/covariance/tests/test_estimator.py` & `scikit-rmt-0.5.0/skrmt/covariance/tests/test_estimator.py`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.4.2/skrmt/covariance/tests/test_metrics.py` & `scikit-rmt-0.5.0/skrmt/covariance/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.4.2/skrmt/ensemble/__init__.py` & `scikit-rmt-0.5.0/skrmt/ensemble/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,26 +4,36 @@
 """
 
 from .gaussian_ensemble import GaussianEnsemble
 from .wishart_ensemble import WishartEnsemble
 from .manova_ensemble import ManovaEnsemble
 from .circular_ensemble import CircularEnsemble
 
-from .plot_law import wigner_semicircular_law
-from .plot_law import marchenko_pastur_law
-from .plot_law import tracy_widom_law
-from .plot_law import manova_spectrum_distr
+from .law import WignerSemicircleDistribution
+from .law import MarchenkoPasturDistribution
+from .law import TracyWidomDistribution
+from .law import ManovaSpectrumDistribution
+
+from .plot_law import wigner_semicircle
+from .plot_law import marchenko_pastur
+from .plot_law import tracy_widom
+from .plot_law import manova_spectrum
 
 from .tridiagonal_utils import tridiag_eigval_neg
 from .tridiagonal_utils import tridiag_eigval_hist
 from .tridiagonal_utils import householder_reduction
 
 
 __all__ = ["GaussianEnsemble", "WishartEnsemble",
            "ManovaEnsemble", "CircularEnsemble",
-           "wigner_semicircular_law",
-           "marchenko_pastur_law",
-           "tracy_widom_law",
-           "manova_spectrum_distr",
+           "WignerSemicircleDistribution",
+           "MarchenkoPasturDistribution",
+           "TracyWidomDistribution",
+           "ManovaSpectrumDistribution",
+           "wigner_semicircle",
+           "marchenko_pastur",
+           "tracy_widom",
+           "manova_spectrum",
            "tridiag_eigval_neg",
            "tridiag_eigval_hist",
-           "householder_reduction"]
+           "householder_reduction"
+        ]
```

### Comparing `scikit-rmt-0.4.2/skrmt/ensemble/_base_ensemble.py` & `scikit-rmt-0.5.0/skrmt/ensemble/_base_ensemble.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
     def eigval_pdf(self):
         # pylint: disable=unnecessary-pass
         # pylint: disable=missing-function-docstring
         # this will be commented at inherited classes
         pass
 
     def eigval_hist(self, bins, interval=None, density=False, norm_const=None, avoid_img=False):
-        """Calculates the histogram of the matrix eigenvalues
+        """Calculates the histogram of the matrix eigenvalues.
 
         Calculates the histogram of the current sampled matrix eigenvalues. Some ensembles
         like Gaussian (Hermite) ensemble or Wishart (Laguerre) ensemble might have
         improved routines to avoid calculating the eigenvalues, so instead the histogram
         is built using certain techniques to boost efficiency.
         It is important to underline that this function works with real eigenvalues,
         if the matrix eigenvalues are complex, they are casted to its real part.
@@ -107,18 +107,18 @@
                 bins (array): The edges of the bins. Length nbins + 1 (nbins left edges and
                 right edge of last bin)
 
         Raises:
             ValueError if interval is not a tuple.
 
         References:
-            Albrecht, J. and Chan, C.P. and Edelman, A.
+            - Albrecht, J. and Chan, C.P. and Edelman, A.
                 "Sturm sequences and random eigenvalue distributions".
                 Foundations of Computational Mathematics. 9.4 (2008): 461-483.
-            Dumitriu, I. and Edelman, A.
+            - Dumitriu, I. and Edelman, A.
                 "Matrix Models for Beta Ensembles".
                 Journal of Mathematical Physics. 43.11 (2002): 5830-5847.
 
         """
         if interval is not None:
             if not isinstance(interval, tuple):
                 raise ValueError("interval argument must be a tuple")
@@ -134,15 +134,15 @@
 
         # using numpy to obtain histogram in the given interval and no. of bins
         observed, bins = np.histogram(eigvals, bins=bins, range=interval, density=density)
         return observed, bins
 
 
     def plot_eigval_hist(self, bins, interval=None, density=False, norm_const=None, fig_path=None, avoid_img=False):
-        """Calculates and plots the histogram of the matrix eigenvalues
+        """Computes and plots the histogram of the matrix eigenvalues.
 
         Calculates and plots the histogram of the current sampled matrix eigenvalues.
         Some ensembles like Gaussian (Hermite) ensemble or Wishart (Laguerre) ensemble
         have improved routines to avoid calculating the eigenvalues, so the histogram
         is built using certain techniques to boost efficiency. It is important to
         underline that this function works with real and complex eigenvalues: if the
         matrix eigenvalues are complex, they are plotted in the complex plane next to a
@@ -165,36 +165,35 @@
                 to specify a normalization constant to observe eigenvalue spectrum, e.g.
                 1/sqrt(n/2) if you want to analyze Wigner's Semicircular Law.
             avoid_img (bool, default=False): If True, eigenvalue imaginary part is ignored.
                 This should be used when the eigenvalue compatation is expected to generate
                 complex eigenvalues with really small imaginary part because of computing
                 rounding errors. E.g.: MANOVA Ensemble eigenvalues.
             fig_path (string, default=None): path to save the created figure. If it is not
-                provided, the plot is shown are the end of the routine.
+                provided, the plot is shown at the end of the routine.
 
         References:
-            Albrecht, J. and Chan, C.P. and Edelman, A.
+            - Albrecht, J. and Chan, C.P. and Edelman, A.
                 "Sturm sequences and random eigenvalue distributions".
                 Foundations of Computational Mathematics. 9.4 (2008): 461-483.
-            Dumitriu, I. and Edelman, A.
+            - Dumitriu, I. and Edelman, A.
                 "Matrix Models for Beta Ensembles".
                 Journal of Mathematical Physics. 43.11 (2002): 5830-5847.
 
         """
         # pylint: disable=too-many-arguments
         if not isinstance(interval, tuple):
             raise ValueError("interval argument must be a tuple")
 
         observed, bins = self.eigval_hist(bins=bins, interval=interval, density=density,
                                           norm_const=norm_const, avoid_img=avoid_img)
         width = bins[1]-bins[0]
         plt.bar(bins[:-1], observed, width=width, align='edge')
 
-        plt.title("Eigenvalue density histogram (matrix size: "+\
-                      str(len(self.matrix))+"x"+str(len(self.matrix))+")", fontweight="bold")
+        plt.title("Eigenvalue density histogram", fontweight="bold")
         plt.xlabel("x")
         plt.ylabel("density")
 
         # Saving plot or showing it
         if fig_path:
             plt.savefig(fig_path, dpi=1200)
         else:
```

### Comparing `scikit-rmt-0.4.2/skrmt/ensemble/circular_ensemble.py` & `scikit-rmt-0.5.0/skrmt/ensemble/circular_ensemble.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,19 +62,19 @@
         beta (int): descriptive integer of the gaussian ensemble type.
             For COE beta=1, for CUE beta=2, for CSE beta=4.
         n (int): random matrix size. Circular ensemble matrices are
             squared matrices. COE and CUE are of size n times n,
             and CSE are of size 2n times 2n.
 
     References:
-        Killip, R. and Zozhan, R.
+        - Killip, R. and Zozhan, R.
             Matrix Models and Eigenvalue Statistics for Truncations of
             Classical Ensembles of Random Unitary Matrices.
             Communications in Mathematical Physics. 349 (2017): 991-1027.
-        "Circular ensemble". Wikipedia.
+        - "Circular ensemble". Wikipedia.
             en.wikipedia.org/wiki/Circular_ensemble
 
     """
 
     def __init__(self, beta, n):
         """Constructor for CircularEnsemble class.
 
@@ -119,19 +119,19 @@
         beta=2 CUE matrix is sampled and if beta=4
         CSE matrix is sampled.
 
         Returns:
             numpy array containing new matrix sampled.
 
         References:
-            Killip, R. and Zozhan, R.
+            - Killip, R. and Zozhan, R.
                 Matrix Models and Eigenvalue Statistics for Truncations of
                 Classical Ensembles of Random Unitary Matrices.
                 Communications in Mathematical Physics. 349 (2017): 991-1027.
-            "Circular ensemble". Wikipedia.
+            - "Circular ensemble". Wikipedia.
                 en.wikipedia.org/wiki/Circular_ensemble
 
         """
         if self.beta == 1:
             return self._sample_coe()
         if self.beta == 2:
             return self._sample_cue()
@@ -172,19 +172,19 @@
         Args:
             n (int): matrix size.
 
         Returns:
             numpy array containing J matrix.
 
         References:
-            Killip, R. and Zozhan, R.
+            - Killip, R. and Zozhan, R.
                 Matrix Models and Eigenvalue Statistics for Truncations of
                 Classical Ensembles of Random Unitary Matrices.
                 Communications in Mathematical Physics. 349 (2017): 991-1027.
-            "Circular ensemble". Wikipedia.
+            - "Circular ensemble". Wikipedia.
                 en.wikipedia.org/wiki/Circular_ensemble
         """
         size = 2*self.n
         j_mtx = np.zeros((size,size))
         # selecting indices
         inds = np.arange(size-1)
         # selecting upper-diagonal indices
@@ -204,15 +204,15 @@
 
         """
         if self.beta == 1:
             return np.linalg.eigvalsh(self.matrix)
         return np.linalg.eigvals(self.matrix)
 
     def plot_eigval_hist(self, bins, interval=None, density=False, norm_const=None, fig_path=None):
-        """Calculates and plots the histogram of the matrix eigenvalues
+        """Computes and plots the histogram of the matrix eigenvalues.
 
         Calculates and plots the histogram of the current sampled matrix eigenvalues.
         It is important to underline that this function works with real and complex
         eigenvalues: if the matrix eigenvalues are complex, they are plotted in the
         complex plane next to a heap map to study eigenvalue density.
 
         Args:
@@ -228,18 +228,18 @@
                 integrates to 1. If set to False, the absolute frequencies of the eigenvalues
                 are returned.
             norm_const (float, default=None): Eigenvalue normalization constant. By default,
                 it is set to None, so eigenvalues are not normalized. However, it is advisable
                 to specify a normalization constant to observe eigenvalue spectrum, e.g.
                 1/sqrt(n/2) if you want to analyze Wigner's Semicircular Law.
             fig_path (string, default=None): path to save the created figure. If it is not
-                provided, the plot is shown are the end of the routine.
+                provided, the plot is shown at the end of the routine.
 
         References:
-            Killip, R. and Zozhan, R.
+            - Killip, R. and Zozhan, R.
                 Matrix Models and Eigenvalue Statistics for Truncations of
                 Classical Ensembles of Random Unitary Matrices.
                 Communications in Mathematical Physics. 349 (2017): 991-1027.
 
         """
         # pylint: disable=too-many-arguments
         # pylint: disable=too-many-locals
@@ -289,29 +289,29 @@
         if fig_path:
             plt.savefig(fig_path, dpi=600)
         else:
             plt.show()
 
 
     def eigval_pdf(self):
-        '''Calculates joint eigenvalue pdf.
+        '''Computes joint eigenvalue pdf.
 
         Calculates joint eigenvalue probability density function given the
             current random matrix (so its eigenvalues). This function depends
             on beta, i.e., in the sub-Circular ensemble.
 
         Returns:
             real number. Value of the joint pdf of the current eigenvalues.
 
         References:
-            Killip, R. and Zozhan, R.
+            - Killip, R. and Zozhan, R.
                 Matrix Models and Eigenvalue Statistics for Truncations of
                 Classical Ensembles of Random Unitary Matrices.
                 Communications in Mathematical Physics. 349 (2017): 991-1027.
-            "Circular ensemble". Wikipedia.
+            - "Circular ensemble". Wikipedia.
                 en.wikipedia.org/wiki/Circular_ensemble
 
         '''
         # calculating Circular eigval pdf constant depeding on beta
         const_beta = (2*np.pi)**self.n * \
                      special.gamma(1 + self.n*self.beta/2)/(special.gamma(1 + self.beta/2)**self.n)
         # calculating eigenvalues
```

### Comparing `scikit-rmt-0.4.2/skrmt/ensemble/gaussian_ensemble.py` & `scikit-rmt-0.5.0/skrmt/ensemble/gaussian_ensemble.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,15 @@
 known as Hermite Ensemble. This ensemble of random matrices contains
 mainly three sub-ensembles: Gaussian Orthogonal Ensemble (GOE),
 Gaussian Unitary Ensemble (GUE) and Gaussian Symplectic Ensemble (GSE).
 
 """
 
 import numpy as np
-from scipy import sparse
-from scipy import special
+from scipy import sparse, special
 import matplotlib.pyplot as plt
 
 from ._base_ensemble import _Ensemble
 from .tridiagonal_utils import tridiag_eigval_hist
 
 #########################################################################
 ### Gaussian Ensemble = Hermite Ensemble
@@ -44,60 +43,68 @@
         n (int): random matrix size. Gaussian ensemble matrices are
             squared matrices. GOE and GUE are of size n times n,
             and GSE are of size 2n times 2n.
         use_tridiagonal (bool): if set to True, Gaussian Ensemble
             matrices are sampled in its tridiagonal form, which has the same
             eigenvalues than its standard form. Otherwise, it is sampled using
             its standard form.
+        sigma (float): scale (standard deviation) of the random entries of the
+            sampled matrix.
 
     References:
-        Albrecht, J. and Chan, C.P. and Edelman, A.
+        - Albrecht, J. and Chan, C.P. and Edelman, A.
             "Sturm sequences and random eigenvalue distributions".
             Foundations of Computational Mathematics. 9.4 (2008): 461-483.
-        Dumitriu, I. and Edelman, A. "Matrix Models for Beta Ensembles".
+        - Dumitriu, I. and Edelman, A. "Matrix Models for Beta Ensembles".
             Journal of Mathematical Physics. 43.11 (2002): 5830-5847.
 
     """
 
-    def __init__(self, beta, n, use_tridiagonal=False):
+    def __init__(self, beta, n, use_tridiagonal=False, sigma=1.0):
         """Constructor for GaussianEnsemble class.
 
         Initializes an instance of this class with the given parameters.
 
         Args:
+            beta (int, default=1): descriptive integer of the gaussian ensemble type.
+                For GOE beta=1, for GUE beta=2, for GSE beta=4.
             n (int): random matrix size. Gaussian ensemble matrices are
                 squared matrices. GOE and GUE are of size n times n,
                 and GSE are of size 2n times 2n.
-            beta (int, default=1): descriptive integer of the gaussian ensemble type.
-                For GOE beta=1, for GUE beta=2, for GSE beta=4.
             use_tridiagonal (bool, default=False): if set to True, Gaussian Ensemble
-            matrices are sampled in its tridiagonal form, which has the same
-            eigenvalues than its standard form. Otherwise, it is sampled using
-            its standard form.
+                matrices are sampled in its tridiagonal form, which has the same
+                eigenvalues than its standard form. Otherwise, it is sampled using
+                its standard form.
+            sigma (float, 1.0): scale (standard deviation) of the random entries of the
+                sampled matrix.
 
         """
+        if beta not in [1,2,4]:
+            raise ValueError(f"Invalid beta: {beta}. Beta value has to be 1, 2 or 4.")
+
         super().__init__()
         # pylint: disable=invalid-name
         self.n = n
         self.beta = beta
         self.use_tridiagonal = use_tridiagonal
+        self.sigma = sigma
         self.matrix = self.sample()
 
 
-    def set_size(self, n, resample_mtx=False):
+    def set_size(self, n, resample_mtx=True):
         # pylint: disable=arguments-differ
         """Setter of matrix size.
 
         Sets the matrix size. Useful if it has been initialized with a different value.
 
         Args:
             n (int): new random matrix size. Gaussian ensemble matrices are
                 squared matrices. GOE and GUE are of size n times n, and
                 GSE are of size 2n times 2n.
-            resample_mtx (bool, default=False): If set to True, the ensemble matrix is
+            resample_mtx (bool, default=True): If set to True, the ensemble matrix is
                 resampled with the new dimensions.
 
         """
         self.n = n
         if resample_mtx:
             self.matrix = self.sample()
 
@@ -111,48 +118,48 @@
         is sampled. Otherwise, it is sampled using the standard
         form.
 
         Returns:
             numpy array containing new matrix sampled.
 
         References:
-            Dumitriu, I. and Edelman, A. "Matrix Models for Beta Ensembles".
+            - Dumitriu, I. and Edelman, A. "Matrix Models for Beta Ensembles".
                 Journal of Mathematical Physics. 43.11 (2002): 5830-5847.
         """
         if self.use_tridiagonal:
             return self.sample_tridiagonal()
 
         if self.beta == 1:
             return self._sample_goe()
         if self.beta == 2:
             return self._sample_gue()
         if self.beta == 4:
             return self._sample_gse()
 
     def _sample_goe(self):
         # n by n matrix of random Gaussians
-        mtx = np.random.randn(self.n,self.n)
+        mtx = np.random.randn(self.n,self.n) * self.sigma
         # symmetrize matrix
         self.matrix = (mtx + mtx.transpose())/np.sqrt(2)
         return self.matrix
 
     def _sample_gue(self):
         size = self.n
         # n by n random complex matrix
-        mtx = np.random.randn(size,size) + 1j*np.random.randn(size,size)
+        mtx = np.random.randn(size,size)*self.sigma + 1j*np.random.randn(size,size)*self.sigma
         # hermitian matrix
         self.matrix = (mtx + mtx.transpose().conj())/np.sqrt(2)
         return self.matrix
 
     def _sample_gse(self):
         size = self.n
         # n by n random complex matrix
-        x_mtx = np.random.randn(size,size) + (0+1j)*np.random.randn(size,size)
+        x_mtx = np.random.randn(size,size)*self.sigma + 1j*np.random.randn(size,size)*self.sigma
         # another n by n random complex matrix
-        y_mtx = np.random.randn(size,size) + (0+1j)*np.random.randn(size,size)
+        y_mtx = np.random.randn(size,size)*self.sigma + 1j*np.random.randn(size,size)*self.sigma
         # [X Y; -conj(Y) conj(X)]
         mtx = np.block([
                        [x_mtx               , y_mtx],
                        [-np.conjugate(y_mtx), np.conjugate(x_mtx)]
                         ])
         # hermitian matrix
         self.matrix = (mtx + mtx.transpose().conj())/np.sqrt(2)
@@ -165,36 +172,42 @@
         beta=1 is GOE, beta=2 is GUE and beta=4 is GSE) in its tridiagonal
         form.
 
         Returns:
             numpy array containing new matrix sampled.
 
         References:
-            Albrecht, J. and Chan, C.P. and Edelman, A.
+            - Albrecht, J. and Chan, C.P. and Edelman, A.
                 "Sturm sequences and random eigenvalue distributions".
                 Foundations of Computational Mathematics. 9.4 (2008): 461-483.
-            Dumitriu, I. and Edelman, A. "Matrix Models for Beta Ensembles".
+            - Dumitriu, I. and Edelman, A. "Matrix Models for Beta Ensembles".
                 Journal of Mathematical Physics. 43.11 (2002): 5830-5847.
 
         '''
+        if self.sigma != 1.0:
+            raise ValueError("Error: cannot sample tridiagonal random matrix using non-unitary scale"
+                             f" (sigma = {self.sigma}).\n"
+                             "\t Set `sigma=1.0` (default) or deactivate tridiagonal sampling.")
+
+        size = 2*self.n if self.beta==4 else self.n
         # sampling diagonal normals
-        normals = (1/np.sqrt(2)) * np.random.normal(loc=0, scale=np.sqrt(2), size=self.n)
+        normals = (1/np.sqrt(2)) * np.random.normal(loc=0, scale=np.sqrt(2), size=size)
         # sampling chi-squares
-        dfs = np.flip(np.arange(1, self.n))
+        dfs = np.flip(np.arange(1, size))
         chisqs = (1/np.sqrt(2)) * \
                  np.array([np.sqrt(np.random.chisquare(df*self.beta)) for df in dfs])
         # inserting diagonals
         diagonals = [chisqs, normals, chisqs]
         mtx = sparse.diags(diagonals, [-1, 0, 1])
         # converting to numpy array
         self.matrix = mtx.toarray()
         return self.matrix
 
     def eigvals(self):
-        """Calculates the random matrix eigenvalues.
+        """Computes the random matrix eigenvalues.
 
         Calculates the random matrix eigenvalues using numpy standard procedure.
         If the matrix ensemble is symmetric, a faster algorithm is used.
 
         Returns:
             numpy array with the calculated eigenvalues.
 
@@ -207,24 +220,24 @@
                 return tridiag_eigval_hist(self.matrix*norm_const, bins=bins,
                                            interval=interval, density=density)
             return tridiag_eigval_hist(self.matrix, bins=bins, interval=interval, density=density)
 
         return super().eigval_hist(bins, interval=interval, density=density,
                                    norm_const=norm_const, avoid_img=avoid_img)
 
-    def plot_eigval_hist(self, bins, interval=None, density=False, norm_const=None, fig_path=None):
-        """Calculates and plots the histogram of the matrix eigenvalues
+    def plot_eigval_hist(self, bins=100, interval=None, density=False, norm_const=None, fig_path=None):
+        """Computes and plots the histogram of the matrix eigenvalues.
 
         Calculates and plots the histogram of the current sampled matrix eigenvalues.
         Gaussian (Hermite) ensemble and Wishart (Laguerre) ensemble have improved
         routines to avoid calculating the eigenvalues, so the histogram
         is built using certain techniques to boost efficiency.
 
         Args:
-            bins (int or sequence): If bins is an integer, it defines the number of
+            bins (int or sequence, default=100): If bins is an integer, it defines the number of
                 equal-width bins in the range. If bins is a sequence, it defines the
                 bin edges, including the left edge of the first bin and the right
                 edge of the last bin; in this case, bins may be unequally spaced.
             interval (tuple, default=None): Delimiters (xmin, xmax) of the histogram.
                 The lower and upper range of the bins. Lower and upper outliers are ignored.
             density (bool, default=False): If True, draw and return a probability
                 density: each bin will display the bin's raw count divided by the total
@@ -232,35 +245,38 @@
                 integrates to 1. If set to False, the absolute frequencies of the eigenvalues
                 are returned.
             norm_const (float, default=None): Eigenvalue normalization constant. By default,
                 it is set to None, so eigenvalues are not normalized. However, it is advisable
                 to specify a normalization constant to observe eigenvalue spectrum, e.g.
                 1/sqrt(n/2) if you want to analyze Wigner's Semicircular Law.
             fig_path (string, default=None): path to save the created figure. If it is not
-                provided, the plot is shown are the end of the routine.
+                provided, the plot is shown at the end of the routine.
 
         References:
-            Albrecht, J. and Chan, C.P. and Edelman, A.
+            - Albrecht, J. and Chan, C.P. and Edelman, A.
                 "Sturm sequences and random eigenvalue distributions".
                 Foundations of Computational Mathematics. 9.4 (2008): 461-483.
-            Dumitriu, I. and Edelman, A.
+            - Dumitriu, I. and Edelman, A.
                 "Matrix Models for Beta Ensembles".
                 Journal of Mathematical Physics. 43.11 (2002): 5830-5847.
 
         """
+        if interval is None:
+            wsl_radius = 2*np.sqrt(self.beta)*self.sigma
+            interval = (-wsl_radius, wsl_radius)
         if self.use_tridiagonal:
             # pylint: disable=too-many-arguments
             if norm_const is None:
-                norm_const = 1/np.sqrt(self.n/2)
+                norm_const = 1/np.sqrt(self.n) if self.beta==4 else 1/np.sqrt(self.n/2)
+
             observed, bins = tridiag_eigval_hist(self.matrix*norm_const, bins=bins,
                                                  interval=interval, density=density)
             width = bins[1]-bins[0]
             plt.bar(bins[:-1], observed, width=width, align='edge')
-            plt.title("Eigenvalue density histogram (matrix size: "+\
-                      str(len(self.matrix))+"x"+str(len(self.matrix))+")", fontweight="bold")
+            plt.title("Eigenvalue density histogram", fontweight="bold")
             plt.xlabel("x")
             plt.ylabel("density")
             # Saving plot or showing it
             if fig_path:
                 plt.savefig(fig_path, dpi=1000)
             else:
                 plt.show()
@@ -269,25 +285,25 @@
             # pylint: disable=too-many-arguments
             if norm_const is None:
                 norm_const = 1/np.sqrt(self.n)
             super().plot_eigval_hist(bins, interval=interval, density=density,
                                      norm_const=norm_const, fig_path=fig_path)
 
     def eigval_pdf(self):
-        '''Calculates joint eigenvalue pdf.
+        '''Computes joint eigenvalue pdf.
 
         Calculates joint eigenvalue probability density function given the current
         random matrix (so its eigenvalues). This function depends on beta, i.e.,
         in the sub-Gaussian ensemble.
 
         Returns:
             real number. Value of the joint pdf of the current eigenvalues.
 
         References:
-            Dumitriu, I. and Edelman, A.
+            - Dumitriu, I. and Edelman, A.
                 "Matrix Models for Beta Ensembles".
                 Journal of Mathematical Physics. 43.11 (2002): 5830-5847.
 
         '''
         # calculating Hermite eigval pdf constant depeding on beta
         const_beta = (2*np.pi)**(-self.n/2)
         for j in range(self.n):
```

### Comparing `scikit-rmt-0.4.2/skrmt/ensemble/manova_ensemble.py` & `scikit-rmt-0.5.0/skrmt/ensemble/manova_ensemble.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 known as Jacobi Ensemble. This ensemble of random matrices contains
 mainly three sub-ensembles: Manova Real Ensemble, Manova Complex Ensemble
 and Manova Quaternion Ensemble.
 
 """
 
 import numpy as np
-import matplotlib.pyplot as plt
 from scipy import special
 
 from ._base_ensemble import _Ensemble
 
 
 #########################################################################
 ### Manova Ensemble = Jacobi Ensemble
@@ -38,36 +37,36 @@
     standard guassian matrices (X1 and X2), both of size m times n1.
     Another two random complex standard guassian matrices (Y1 and Y2),
     both of size m times n2, are sampled. They are stacked forming matrices
     X and Y:
     X = [X1  X2; -conj(X2)  conj(X1)]
     Y = [Y1  Y2; -conj(Y2)  conj(Y1)]
     Finally, matrix A = (X * X') / (X * X' + Y * Y') generates a matrix of
-    the Manova Quaternion Ensemble.
+    the Manova Quaternion Ensemble of size m times m.
 
     Attributes:
         matrix (numpy array): instance of the ManovaReal, ManovaComplex
             or ManovaQuaternion random ensembles. If it is an instance
             of ManovaReal or ManovaComplex, the random matrix is of
-            size n times n. If it is a ManovaQuaternion, the random matrix
-            is of size 2n times 2n.
+            size m times m. If it is a ManovaQuaternion, the random matrix
+            is of size 2m times 2m.
         beta (int): descriptive integer of the Manova ensemble type.
             For Real beta=1, for Complex beta=2, for Quaternion beta=4.
         m (int): number of rows of the random guassian matrices that
             generates the matrix of the corresponding ensemble.
         n1 (int): number of columns of the first random guassian matrix
             that generates the matrix of the corresponding ensemble.
         n2 (int): number of columns of the second random guassian matrix
             that generates the matrix of the corresponding ensemble.
 
     References:
-        Erdos, L. and Farrell, B.
+        - Erdos, L. and Farrell, B.
             "Local Eigenvalue Density for General MANOVA Matrices".
             Journal of Statistical Physics. 152.6 (2013): 1003-1032.
-        Dumitriu, I. and Edelman, A. "Matrix Models for Beta Ensembles".
+        - Dumitriu, I. and Edelman, A. "Matrix Models for Beta Ensembles".
             Journal of Mathematical Physics. 43.11 (2002): 5830-5847.
 
     """
 
     def __init__(self, beta, m, n1, n2):
         """Constructor for ManovaEnsemble class.
 
@@ -88,28 +87,28 @@
         # pylint: disable=invalid-name
         self.m = m
         self.n1 = n1
         self.n2 = n2
         self.beta = beta
         self.matrix = self.sample()
 
-    def set_size(self, m, n1, n2, resample_mtx=False):
+    def set_size(self, m, n1, n2, resample_mtx=True):
         # pylint: disable=arguments-differ
         """Setter of matrix size.
 
         Sets the matrix size. Useful if it has been initialized with a different value.
 
         Args:
             m (int): number of rows of the random guassian matrices that
                 generates the matrix of the corresponding ensemble.
             n1 (int): number of columns of the first random guassian matrix
                 that generates the matrix of the corresponding ensemble.
             n2 (int): number of columns of the second random guassian matrix
                 that generates the matrix of the corresponding ensemble.
-            resample_mtx (bool, default=False): If set to True, the ensemble matrix is
+            resample_mtx (bool, default=True): If set to True, the ensemble matrix is
                 resampled with the new dimensions.
 
         """
         self.m = m
         self.n1 = n1
         self.n2 = n2
         if resample_mtx:
@@ -124,15 +123,15 @@
         beta=2 Manova Complex is sampled and if beta=4
         Manova Quaternion is sampled.
 
         Returns:
             numpy array containing new matrix sampled.
 
         References:
-            Dumitriu, I. and Edelman, A. "Matrix Models for Beta Ensembles".
+            - Dumitriu, I. and Edelman, A. "Matrix Models for Beta Ensembles".
                 Journal of Mathematical Physics. 43.11 (2002): 5830-5847.
 
         """
         if self.beta == 1:
             return self._sample_mre()
         if self.beta == 2:
             return self._sample_mce()
@@ -198,27 +197,27 @@
         # A2 = X * X' + Y * Y'
         a2_mtx = a1_mtx + np.matmul(y_mtx, y_mtx.transpose().conj())
         # A = (X * X') / (X * X' + Y * Y') = (X * X') * (X * X' + Y * Y')^(-1)
         self.matrix = np.matmul(a1_mtx, np.linalg.inv(a2_mtx))
         return self.matrix
 
     def eigvals(self):
-        """Calculates the random matrix eigenvalues.
+        """Computes the random matrix eigenvalues.
 
         Calculates the random matrix eigenvalues using numpy standard procedure.
         If the matrix ensemble is symmetric, a faster algorithm is used.
 
         Returns:
             numpy array with the calculated eigenvalues.
 
         """
         return np.linalg.eigvals(self.matrix)
 
     def plot_eigval_hist(self, bins, interval=(0,1), density=False, norm_const=None, fig_path=None):
-        """Calculates and plots the histogram of the matrix eigenvalues
+        """Computes and plots the histogram of the matrix eigenvalues
 
         Calculates and plots the histogram of the current sampled matrix eigenvalues.
 
         Args:
             bins (int or sequence): If bins is an integer, it defines the number of
                 equal-width bins in the range. If bins is a sequence, it defines the
                 bin edges, including the left edge of the first bin and the right
@@ -231,41 +230,41 @@
                 integrates to 1. If set to False, the absolute frequencies of the eigenvalues
                 are returned.
             norm_const (float, default=None): Eigenvalue normalization constant. By default,
                 it is set to None, so eigenvalues are not normalized. However, it is advisable
                 to specify a normalization constant to observe eigenvalue spectrum, e.g.
                 1/sqrt(n/2) if you want to analyze Wigner's Semicircular Law.
             fig_path (string, default=None): path to save the created figure. If it is not
-                provided, the plot is shown are the end of the routine.
+                provided, the plot is shown at the end of the routine.
 
         References:
-            Erdos, L. and Farrell, B.
+            - Erdos, L. and Farrell, B.
                 "Local Eigenvalue Density for General MANOVA Matrices".
                 Journal of Statistical Physics. 152.6 (2013): 1003-1032.
-            Dumitriu, I. and Edelman, A.
+            - Dumitriu, I. and Edelman, A.
                 "Matrix Models for Beta Ensembles".
                 Journal of Mathematical Physics. 43.11 (2002): 5830-5847.
 
         """
         # pylint: disable=too-many-arguments
         return super().plot_eigval_hist(bins, interval, density,
                                         norm_const=norm_const, avoid_img=True, fig_path=fig_path)
 
     def eigval_pdf(self):
-        '''Calculates joint eigenvalue pdf.
+        '''Computes joint eigenvalue pdf.
 
         Calculates joint eigenvalue probability density function given the current
             random matrix (so its eigenvalues). This function depends on beta, i.e.,
             in the sub-Manova ensemble.
 
         Returns:
             real number. Value of the joint pdf of the current eigenvalues.
 
         References:
-            Dumitriu, I. and Edelman, A. "Matrix Models for Beta Ensembles".
+            - Dumitriu, I. and Edelman, A. "Matrix Models for Beta Ensembles".
                 Journal of Mathematical Physics. 43.11 (2002): 5830-5847.
 
         '''
         # pylint: disable=invalid-name
         a1 = self.beta*self.n1/2
         a2 = self.beta*self.n2/2
         p = 1 + self.beta/2*(self.m - 1)
```

### Comparing `scikit-rmt-0.4.2/skrmt/ensemble/plot_law.py` & `scikit-rmt-0.5.0/skrmt/ensemble/plot_law.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,29 @@
 """Plot Law module
 
 This module contains several functions that simulate various
 random matrix laws, including Wigner's Semicircle Law,
-Marchenko-Pastur Law and Tracy-Widom Law.
+Marchenko-Pastur Law and Tracy-Widom Law. The spectrum of
+the Manova ensemble is also simulated when the matrix size
+goes to infinity.
 
 """
 
-import math
 import numpy as np
 import matplotlib.pyplot as plt
 
 from .gaussian_ensemble import GaussianEnsemble
 from .wishart_ensemble import WishartEnsemble
 from .manova_ensemble import ManovaEnsemble
+from .law import (
+    WignerSemicircleDistribution,
+    MarchenkoPasturDistribution,
+    TracyWidomDistribution,
+    ManovaSpectrumDistribution
+)
 from .tracy_widom_approximator import TW_Approximator
 
 
 def __get_bins_centers_and_contour(bins):
     """Calculates the centers and contour of the given bins.
 
     Computes the centers of the given bins. Also, the smallest and the largest bin
@@ -33,248 +40,218 @@
     l = len(bins)
     for i in range(l-1):
         centers.append((bins[i]+bins[i+1])/2) # Adding centers
     centers.append(bins[-1]) # Adding final contour
     return centers
 
 
-def __relu_func(vals):
-    """Element-wise maximum between the value and zero.
-
-    Args:
-        vals (ndarray): list of numbers to compute its element-wise maximum.
-    
-    Returns:
-        array_like consisting in the element-wise maximum vector of the given values.
-    """
-    return np.maximum(vals, np.zeros_like(vals))
-
-
-def theory_wigner_law(val, beta):
-    """Computes the theoretical Wigner's semicircle law on a given point.
-
-    Args:
-        val (float): point whose evaluation is required.
-        beta (int): integer representing type of matrix entries. beta=1 if real
-            entries are used (GOE), beta=2 if they are complex (GUE) or beta=4
-            if they are quaternions (GSE). 
-    
-    Returns:
-        number (float) which is image of the given value evaluated on Wigner's
-        semicircle law.
-    """
-    radius = 2*math.sqrt(beta)
-    if abs(val) >= radius:
-        return 0
-    return 2*math.sqrt(radius**2 - val**2)/(math.pi*radius**2)
-
-
-def wigner_semicircular_law(ensemble='goe', n_size=1000, bins=100, interval=None,
-                            density=False, limit_pdf=False, savefig_path=None):
-    """Calculates and plots Wigner's Semicircle Law using Gaussian Ensemble.
+def wigner_semicircle(ensemble='goe', n_size=1000, sigma=1.0, bins=100, interval=None,
+                      density=False, plot_law_pdf=False, savefig_path=None):
+    """Computes and plots Wigner's Semicircle Law using Gaussian Ensemble.
 
     Calculates and plots Wigner's Semicircle Law using Gaussian Ensemble random matrices.
     Gaussian (Hermite) ensemble has improved routines (using tridiagonal forms and Sturm
     sequences) to avoid calculating the eigenvalues, so the histogram
     is built using certain techniques to boost efficiency.
 
     Args:
         ensemble ('goe', 'gue' or 'gse', default='goe'): ensemble to draw the
             random matrices to study Wigner's Law.
         n_size (int, default=1000): random matrix size n times n.
+        sigma (float, 1.0): scale (standard deviation) of the random entries of the
+            sampled matrix.
         bins (int or sequence, default=100): If bins is an integer, it defines the number
             of equal-width bins in the range. If bins is a sequence, it defines the
             bin edges, including the left edge of the first bin and the right
             edge of the last bin; in this case, bins may be unequally spaced.
         interval (tuple, default=None): Delimiters (xmin, xmax) of the histogram.
             The lower and upper range of the bins. Lower and upper outliers are ignored.
         density (bool, default=False): If True, draw and return a probability
             density: each bin will display the bin's raw count divided by the total
             number of counts and the bin width, so that the area under the histogram
             integrates to 1. If set to False, the absolute frequencies of the eigenvalues
             are returned.
-        limit_pdf (bool, default=False): If True, the limiting theoretical law is plotted.
+        plot_law_pdf (bool, default=False): If True, the limiting theoretical law is plotted.
             If set to False, just the empirical histogram is shown. This parameter is only
             considered when the argument 'density' is set also to True.
         fig_path (string, default=None): path to save the created figure. If it is not
             provided, the plot is shown are the end of the routine.
 
     References:
-        Albrecht, J. and Chan, C.P. and Edelman, A.
+        - Albrecht, J. and Chan, C.P. and Edelman, A.
             "Sturm sequences and random eigenvalue distributions".
             Foundations of Computational Mathematics. 9.4 (2008): 461-483.
-        Dumitriu, I. and Edelman, A.
+        - Dumitriu, I. and Edelman, A.
             "Matrix Models for Beta Ensembles".
             Journal of Mathematical Physics. 43.11 (2002): 5830-5847.
 
     """
     # pylint: disable=too-many-arguments
     if n_size<1:
         raise ValueError("matrix size must be positive")
-
-    if ensemble == 'goe':
-        beta = 1
-        if interval is None:
-            interval = (-2,2)
-    elif ensemble == 'gue':
-        beta = 2
-        if interval is None:
-            interval = (-3,3)
-    elif ensemble == 'gse':
-        beta = 4
-        if interval is None:
-            interval = (-4,4)
-    else:
-        raise ValueError("ensemble not supported")
     
-    ens = GaussianEnsemble(beta=beta, n=n_size, use_tridiagonal=True)
+    try:
+        beta = ["goe", "gue", None, "gse"].index(ensemble) + 1
+    except ValueError:
+        raise ValueError(f"Ensemble '{ensemble}' not supported."
+                         " Check that ensemble is one of the following: 'goe', 'gue' or 'gse'.")
+    
+    use_tridiag = (sigma == 1.0)
+    if not use_tridiag:
+        print(f"Warning: The given scale is not the standard (sigma = {sigma}).\n"
+              "\t Tridiagonal histogramming is deactivated.\n"
+              "\t It is adviced to set sigma=1.0 to optimize and boost histogramming.")
+
+    ens = GaussianEnsemble(beta=beta, n=n_size, sigma=sigma, use_tridiagonal=use_tridiag)
+
+    # default plotting interval in case it's not provided
+    if interval is None:
+        radius = 2.0 * np.sqrt(beta) * sigma
+        interval = (-radius, radius)
 
     # Wigner eigenvalue normalization constant
-    norm_const = 1/np.sqrt(n_size/2)
+    if use_tridiag:
+        norm_const = 1/np.sqrt(n_size) if beta==4 else 1/np.sqrt(n_size/2)
+    else:
+        norm_const = 1/np.sqrt(n_size)
 
     observed, bins = ens.eigval_hist(bins=bins, interval=interval,
                                      density=density, norm_const=norm_const)
     width = bins[1]-bins[0]
     plt.bar(bins[:-1], observed, width=width, align='edge')
 
-    # Plotting theoretical graphic
-    if limit_pdf and density:
-        centers = __get_bins_centers_and_contour(bins)
-        expected_frec = [theory_wigner_law(cent, beta) for cent in centers]
-        plt.plot(centers, expected_frec, color='red', linewidth=2)
+    # Plotting Wigner Semicircle Law pdf
+    if plot_law_pdf and density:
+        centers = np.asarray(__get_bins_centers_and_contour(bins))
+        wsd = WignerSemicircleDistribution(beta=beta, sigma=sigma)
+        pdf = wsd.pdf(centers)
+        plt.plot(centers, pdf, color='red', linewidth=2)
+    elif plot_law_pdf and not density:
+        print("Warning: Wigner's Semicircle Law PDF is only plotted when density is True.")
 
-    plt.title("Eigenvalue density histogram", fontweight="bold")
+    plt.title("Wigner Semicircle Law - Empirical density histogram", fontweight="bold")
     plt.xlabel("x")
-    plt.ylabel("density")
+    plt.ylabel("probability density")
 
     # Saving plot or showing it
     if savefig_path:
         plt.savefig(savefig_path, dpi=1200)
     else:
         plt.show()
 
 
 
-def theory_marchenko_pastur(vals, ratio, lambda_minus, lambda_plus, beta):
-    """Computes the theoretical Wigner's semicircle law on a given point or points.
-
-    Args:
-        vals (ndarray): numpy array of numbers whose evaluation is required.
-        ratio (float): ratio between the matrix size. ratio is equal to p/n,
-            where p is the number of rows and n is the number of columns of
-            the matrix that generates a Wishart matrix. 'p' is also known as
-            the degrees of freedom and 'n' as the sample size.
-        lambda_minus (float): lower limit of the Marchenko-Pastur distribution.
-        lambda_plus (float): upper limit of the Marchenko-Pastur distribution.
-        beta (int): integer representing type of matrix entries. beta=1 if real
-            entries are used (WRE), beta=2 if they are complex (WCE) or beta=4
-            if they are quaternions (WQE). Beta is considered as the variance
-            of the matrix entries.
-    
-    Returns:
-        array_like (ndarray) which is the image of the given value (or values)
-        evaluated on Marchenko-Pastur Law.
-    """
-    var = beta
-    return np.sqrt(__relu_func(lambda_plus-vals)*__relu_func(vals-lambda_minus)) \
-          / (2*np.pi*ratio*var*vals)
-
-
-def marchenko_pastur_law(ensemble='wre', p_size=3000, n_size=10000, bins=100, interval=None,
-                         density=False, limit_pdf=False, savefig_path=None):
+def marchenko_pastur(ensemble='wre', p_size=1000, n_size=3000, sigma=1.0, bins=100,
+                     interval=None, density=False, plot_law_pdf=False, savefig_path=None):
     """Computes and plots Marchenko-Pastur Law using Wishart Ensemble random matrices.
 
     Calculates and plots Marchenko-Pastur Law using Wishart Ensemble random matrices.
     Wishart (Laguerre) ensemble has improved routines (using tridiagonal forms and Sturm
     sequences) to avoid calculating the eigenvalues, so the histogram
     is built using certain techniques to boost efficiency. This optimization is only used
     when the ratio p_size/n_size is less or equal than 1.
 
     Args:
         ensemble ('wre', 'wce' or 'wqe', default='wre'): ensemble to draw the
             random matrices to study Marchenko-Pastur Law.
-        p_size (int, default=3000): number of rows of the guassian matrix that generates
+        p_size (int, default=1000): number of rows of the guassian matrix that generates
             the matrix of the corresponding ensemble.
-        n_size (int, default=10000): number of columns of the guassian matrix that generates
+        n_size (int, default=3000): number of columns of the guassian matrix that generates
             the matrix of the corresponding ensemble.
+        sigma (float, 1.0): scale (standard deviation) of the random entries of the
+            sampled matrix.
         bins (int or sequence, default=100): If bins is an integer, it defines the number
             of equal-width bins in the range. If bins is a sequence, it defines the
             bin edges, including the left edge of the first bin and the right
             edge of the last bin; in this case, bins may be unequally spaced.
         interval (tuple, default=None): Delimiters (xmin, xmax) of the histogram.
             The lower and upper range of the bins. Lower and upper outliers are ignored.
         density (bool, default=False): If True, draw and return a probability
             density: each bin will display the bin's raw count divided by the total
             number of counts and the bin width, so that the area under the histogram
             integrates to 1. If set to False, the absolute frequencies of the eigenvalues
             are returned.
-        limit_pdf (bool, default=False): If True, the limiting theoretical law is plotted.
+        plot_law_pdf (bool, default=False): If True, the limiting theoretical law is plotted.
             If set to False, just the empirical histogram is shown. This parameter is only
             considered when the argument 'density' is set also to True.
         fig_path (string, default=None): path to save the created figure. If it is not
             provided, the plot is shown are the end of the routine.
 
     References:
-        Albrecht, J. and Chan, C.P. and Edelman, A.
+        - Albrecht, J. and Chan, C.P. and Edelman, A.
             "Sturm sequences and random eigenvalue distributions".
             Foundations of Computational Mathematics. 9.4 (2008): 461-483.
-        Dumitriu, I. and Edelman, A.
+        - Dumitriu, I. and Edelman, A.
             "Matrix Models for Beta Ensembles".
             Journal of Mathematical Physics. 43.11 (2002): 5830-5847.
 
     """
     # pylint: disable=too-many-arguments
     if n_size<1 or p_size<1:
         raise ValueError("matrix size must be positive")
+
+    try:
+        beta = ["wre", "wce", None, "wqe"].index(ensemble) + 1
+    except ValueError:
+        raise ValueError(f"Ensemble '{ensemble}' not supported."
+                         " Check that ensemble is one of the following: 'wre', 'wce' or 'wqe'.")
     
     if interval and interval[0] == 0:
         print("Warning: setting the beginning of the interval to zero may generate numerical errors.")
         print(f"Setting interval to (-0.01, {interval[1]})")
         interval = (-0.01, interval[1])
 
-    try:
-        beta = ["wre", "wce", None, "wqe"].index(ensemble) + 1
-    except ValueError:
-        raise ValueError("ensemble not supported: "+str(ensemble))
     # calculating constants depending on matrix sizes
     ratio = p_size/n_size
-    lambda_plus = beta*(1 + np.sqrt(ratio))**2
-    lambda_minus = beta*(1 - np.sqrt(ratio))**2
-    use_tridiag = (ratio <= 1)
+    lambda_plus = beta * sigma**2 * (1 + np.sqrt(ratio))**2
+    lambda_minus = beta * sigma**2 * (1 - np.sqrt(ratio))**2
+    use_tridiag_ratio = (ratio <= 1)
+    if not use_tridiag_ratio:
+        print("Warning: Cannot use tridiagonal histogramming if 'p' (degrees of freedom) is "
+              " greater than 'n' (sample size).\n"
+              f"\t Provided n={n_size} and p={p_size}. Tridiagonal histogramming is therefore deactivated.\n"
+              "\t It is adviced to increase sample size (`n`) to optimize and boost histogramming.")
 
     # computing interval according to the matrix size ratio and support
     if interval is None:
         if ratio <= 1:
             interval = (lambda_minus, lambda_plus)
         else:
             interval = (min(-0.05, lambda_minus), lambda_plus)
     
-    ens = WishartEnsemble(beta=beta, p=p_size, n=n_size, use_tridiagonal=use_tridiag)
+    use_tridiag_sigma = (sigma == 1.0)
+    if not use_tridiag_sigma:
+        print(f"Warning: The given scale is not the standard (sigma = {sigma}).\n"
+              "\t Tridiagonal histogramming is deactivated.\n"
+              "\t It is adviced to set sigma=1.0 to optimize and boost histogramming.")
+
+    ens = WishartEnsemble(beta=beta, p=p_size, n=n_size, sigma=sigma,
+                          use_tridiagonal=(use_tridiag_ratio and use_tridiag_sigma))
 
     # Wigner eigenvalue normalization constant
-    norm_const = 1/n_size
+    norm_const = 1/n_size 
 
     observed, bins = ens.eigval_hist(bins=bins, interval=interval,
                                      density=density, norm_const=norm_const)
     width = bins[1]-bins[0]
     plt.bar(bins[:-1], observed, width=width, align='edge')
 
     # Plotting theoretical graphic
-    if limit_pdf and density:
+    if plot_law_pdf and density:
         centers = np.array(__get_bins_centers_and_contour(bins))
-        expected_frec = theory_marchenko_pastur(centers, ratio, lambda_minus,
-                                                lambda_plus, beta)
-        plt.plot(centers, expected_frec, color='red', linewidth=2)
+        mpd = MarchenkoPasturDistribution(beta=beta, ratio=ratio, sigma=sigma)
+        pdf = mpd.pdf(centers)
+        plt.plot(centers, pdf, color='red', linewidth=2)
 
-    plt.title("Eigenvalue density histogram", fontweight="bold")
+    plt.title("Marchenko-Pastur Law - Empirical density histogram", fontweight="bold")
     plt.xlabel("x")
-    plt.ylabel("density")
+    plt.ylabel("probability density")
     if ratio > 1:
-        if limit_pdf and density:
-            ylim_vals = expected_frec
+        if plot_law_pdf and density:
+            ylim_vals = pdf
         else:
             ylim_vals = observed
         try:
             plt.ylim(0, np.max(ylim_vals)+0.25*np.max(ylim_vals))
         except ValueError:
             second_highest_val = np.partition(ylim_vals.flatten(), -2)[-2]
             plt.ylim(0, second_highest_val+0.25*second_highest_val)
@@ -283,17 +260,17 @@
     if savefig_path:
         plt.savefig(savefig_path, dpi=1200)
     else:
         plt.show()
 
 
 
-def tracy_widom_law(ensemble='goe', n_size=100, times=1000, bins=100, interval=None,
-                    density=False, limit_pdf=False, savefig_path=None):
-    """Calculates and plots Tracy-Widom Law using Gaussian Ensemble.
+def tracy_widom(ensemble='goe', n_size=100, times=1000, bins=100, interval=None,
+                density=False, plot_law_pdf=False, savefig_path=None):
+    """Computes and plots Tracy-Widom Law using Gaussian Ensemble.
 
     Calculates and plots Tracy-Widom Law using Gaussian Ensemble random matrices.
     Because we need to obtain the largest eigenvalue of each sampled random matrix,
     we need to sample a certain amount them. For each random matrix sammpled, its
     largest eigenvalue is calcualted in order to simulate its density.
 
     Args:
@@ -308,25 +285,25 @@
         interval (tuple, default=None): Delimiters (xmin, xmax) of the histogram.
             The lower and upper range of the bins. Lower and upper outliers are ignored.
         density (bool, default=False): If True, draw and return a probability
             density: each bin will display the bin's raw count divided by the total
             number of counts and the bin width, so that the area under the histogram
             integrates to 1. If set to False, the absolute frequencies of the eigenvalues
             are returned.
-        limit_pdf (bool, default=False): If True, the limiting theoretical law is plotted.
+        plot_law_pdf (bool, default=False): If True, the limiting theoretical law is plotted.
             If set to False, just the empirical histogram is shown. This parameter is only
             considered when the argument 'density' is set also to True.
         fig_path (string, default=None): path to save the created figure. If it is not
             provided, the plot is shown are the end of the routine.
 
     References:
-        Albrecht, J. and Chan, C.P. and Edelman, A.
+        - Albrecht, J. and Chan, C.P. and Edelman, A.
             "Sturm sequences and random eigenvalue distributions".
             Foundations of Computational Mathematics. 9.4 (2008): 461-483.
-        Dumitriu, I. and Edelman, A.
+        - Dumitriu, I. and Edelman, A.
             "Matrix Models for Beta Ensembles".
             Journal of Mathematical Physics. 43.11 (2002): 5830-5847.
 
     """
     # pylint: disable=too-many-arguments
     if n_size<1 or times<1:
         raise ValueError("matrix size or number of repetitions must be positive")
@@ -334,85 +311,62 @@
     try:
         beta = ["goe", "gue", None, "gse"].index(ensemble) + 1
     except ValueError:
         raise ValueError("ensemble not supported: "+str(ensemble))
 
     ens = GaussianEnsemble(beta=beta, n=n_size, use_tridiagonal=False)
 
-    eigvals = np.asarray([])
+    eigvals = []
     for _ in range(times):
-        vals = ens.eigvals()
-        eigvals = np.append(eigvals, vals.max())
+        eigvals.append(ens.eigvals().max())
         ens.sample()
+    eigvals = np.asarray(eigvals)
 
     # Tracy-Widom eigenvalue distr. normalization constants
-    eigval_scale = 1
-    size_scale = 1
+    eigval_scale = 1.0
+    size_scale = 1.0
     if ensemble == 'gue':
         eigval_scale = 1/np.sqrt(2)
-    if ensemble == 'gse':
+    elif ensemble == 'gse':
         eigval_scale = size_scale = 1/np.sqrt(2)
         n_size *= 2
-    eigvals = size_scale*(n_size**(1/6))*(eigval_scale*eigvals - (2*np.sqrt(n_size)))
+    eigvals = size_scale*(n_size**(1/6))*(eigval_scale*eigvals - (2.0*np.sqrt(n_size)))
 
     if interval is None:
         xmin=eigvals.min()
         xmax=eigvals.max()
         interval=(xmin, xmax)
 
     # using numpy to obtain histogram in the given interval and no. of bins
     observed, bins = np.histogram(eigvals, bins=bins, range=interval, density=density)
     width = bins[1]-bins[0]
     plt.bar(bins[:-1], observed, width=width, align='edge')
 
     # Plotting theoretical graphic
-    if limit_pdf and density:
+    if plot_law_pdf and density:
         centers = __get_bins_centers_and_contour(bins)
-        tw_approx = TW_Approximator(beta=beta)
-        expected_frec = tw_approx.pdf(centers)
-        plt.plot(centers, expected_frec, color='red', linewidth=2)
+        twd = TracyWidomDistribution(beta=beta)
+        pdf = twd.pdf(centers)
+        plt.plot(centers, pdf, color='red', linewidth=2)
 
-    plt.title("Eigenvalue density histogram", fontweight="bold")
+    plt.title("Tracy-Widom Law - Empirical density histogram", fontweight="bold")
     plt.xlabel("x")
-    plt.ylabel("density")
+    plt.ylabel("probability density")
 
     # Saving plot or showing it
     if savefig_path:
         plt.savefig(savefig_path, dpi=1200)
     else:
         plt.show()
 
 
 
-def theory_manova_spectrum_distr(vals, a, b, lambda_minus, lambda_plus):
-    """Computes the theoretical Manova spectrum limiting distribution law
-    on a given point or points.
-
-    Args:
-        vals (ndarray): numpy array of numbers whose evaluation is required.
-        a (float): parameter of the theoretical analytical function.
-        b (float): parameter of the theoretical analytical function.
-        lambda_minus (float): lower limit of the Manova spectrum distribution.
-        lambda_plus (float): upper limit of the Manova spectrum distribution.
-        beta (int): integer representing type of matrix entries. beta=1 if real
-            entries are used (MRE), beta=2 if they are complex (MCE) or beta=4
-            if they are quaternions (MQE). Beta is considered as the variance
-            of the matrix entries.
-    
-    Returns:
-        array_like (ndarray) which is the image of the given value (or values)
-        evaluated on the Manova spectrum limiting distribution.
-    """
-    return (a+b) * np.sqrt(__relu_func(lambda_plus-vals)*__relu_func(vals-lambda_minus)) \
-        / (2*np.pi*vals*(1-vals))
-
-
-def manova_spectrum_distr(ensemble='mre', m_size=1000, n1_size=3000, n2_size=3000,
-                          bins=100, interval=None, density=False, limit_pdf=False,
-                          savefig_path=None):
+def manova_spectrum(ensemble='mre', m_size=1000, n1_size=3000, n2_size=3000,
+                    bins=100, interval=None, density=False, plot_law_pdf=False,
+                    savefig_path=None):
     """Computes and plots Manova spectrum limiting and analytical distribution.
 
     Calculates and plots Manova spectrum limiting Law using Manova Ensemble random matrices.
 
     Args:
         ensemble ('mre', 'mce' or 'mqe', default='mre'): Manova Ensemble to draw the
             random matrices to study limiting distribution.
@@ -429,28 +383,28 @@
         interval (tuple, default=None): Delimiters (xmin, xmax) of the histogram.
             The lower and upper range of the bins. Lower and upper outliers are ignored.
         density (bool, default=False): If True, draw and return a probability
             density: each bin will display the bin's raw count divided by the total
             number of counts and the bin width, so that the area under the histogram
             integrates to 1. If set to False, the absolute frequencies of the eigenvalues
             are returned.
-        limit_pdf (bool, default=False): If True, the limiting theoretical law is plotted.
+        plot_law_pdf (bool, default=False): If True, the limiting theoretical law is plotted.
             If set to False, just the empirical histogram is shown. This parameter is only
             considered when the argument 'density' is set also to True.
         fig_path (string, default=None): path to save the created figure. If it is not
             provided, the plot is shown are the end of the routine.
 
     References:
-        Laszlo, L. and Farrel, B.
+        - Laszlo, L. and Farrel, B.
             "Local Eigenvalue Density for General MANOVA Matrices".
             Journal of Statistical Physics. 152.6 (2013): 1003-1032.
-        Albrecht, J. and Chan, C.P. and Edelman, A.
+        - Albrecht, J. and Chan, C.P. and Edelman, A.
             "Sturm sequences and random eigenvalue distributions".
             Foundations of Computational Mathematics. 9.4 (2008): 461-483.
-        Dumitriu, I. and Edelman, A.
+        - Dumitriu, I. and Edelman, A.
             "Matrix Models for Beta Ensembles".
             Journal of Mathematical Physics. 43.11 (2002): 5830-5847.
 
     """
     if m_size<1 or n1_size<1 or n2_size<1:
         raise ValueError("matrix size must be positive")
     
@@ -475,39 +429,38 @@
         interval = [lambda_minus, lambda_plus]
         if a <= 1:
             interval[0] = min(-0.05, lambda_minus)
         if b <= 1:
             interval[1] = max(lambda_plus, 1.05)
         interval = tuple(interval)
 
-    #norm_const = m_size
-    observed, bins = ens.eigval_hist(bins=bins, interval=interval,
-                                     density=density, avoid_img=True) #norm_const = norm_const
+    observed, bins = ens.eigval_hist(bins=bins, interval=interval, density=density, avoid_img=True)
+
     width = bins[1]-bins[0]
     plt.bar(bins[:-1], observed, width=width, align='edge')
 
     # Plotting theoretical graphic
-    if limit_pdf and density:
+    if plot_law_pdf and density:
         centers = np.array(__get_bins_centers_and_contour(bins))
-        expected_frec = theory_manova_spectrum_distr(centers, a, b, 
-                                                    lambda_minus, lambda_plus)
-        plt.plot(centers, expected_frec, color='red', linewidth=2)
+        msd = ManovaSpectrumDistribution(beta=beta, a=a, b=b)
+        pdf = msd.pdf(centers)
+        plt.plot(centers, pdf, color='red', linewidth=2)
 
-    plt.title("Eigenvalue density histogram", fontweight="bold")
+    plt.title("Manova Spectrum - Empirical density histogram", fontweight="bold")
     plt.xlabel("x")
-    plt.ylabel("density")
+    plt.ylabel("probability density")
     if a <= 1 or b <= 1:
-        if limit_pdf and density:
-            ylim_vals = expected_frec
+        if plot_law_pdf and density:
+            ylim_vals = pdf
         else:
             ylim_vals = observed
         try:
-            plt.ylim(0, np.max(ylim_vals)+0.25*np.max(ylim_vals))
+            plt.ylim(0, np.max(ylim_vals) + 0.25*np.max(ylim_vals))
         except ValueError:
             second_highest_val = np.partition(ylim_vals.flatten(), -2)[-2]
-            plt.ylim(0, second_highest_val+0.25*second_highest_val)
+            plt.ylim(0, second_highest_val + 0.25*second_highest_val)
 
     # Saving plot or showing it
     if savefig_path:
         plt.savefig(savefig_path, dpi=1200)
     else:
         plt.show()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `scikit-rmt-0.4.2/skrmt/ensemble/tests/test_circular_ens.py` & `scikit-rmt-0.5.0/skrmt/ensemble/tests/test_circular_ens.py`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.4.2/skrmt/ensemble/tests/test_gaussian_ens.py` & `scikit-rmt-0.5.0/skrmt/ensemble/tests/test_gaussian_ens.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,32 @@
 '''Gaussian Ensemble Test module
 
 Testing GaussianEnsemble module
 '''
 
+import pytest
 import numpy as np
 from numpy.testing import (
     assert_almost_equal,
     assert_array_equal,
 )
 
 from skrmt.ensemble import GaussianEnsemble
 
+
+
+def test_init_exception():
+    with pytest.raises(ValueError):
+        _ = GaussianEnsemble(beta=3, n=100)
+
+def test_build_tridiagonal_exception():
+    with pytest.raises(ValueError):
+        _ = GaussianEnsemble(beta=1, n=100, sigma=2.0, use_tridiagonal=True)
+
+
 ##########################################
 ### Gaussian Orthogonal Ensemble = GOE
 
 def test_goe_init():
     '''Testing GOE init
     '''
     n_size = 3
@@ -308,14 +320,15 @@
     n_size = 5
     beta = 4
 
     np.random.seed(1)
     gse = GaussianEnsemble(beta=4, n=n_size, use_tridiagonal=True)
 
     np.random.seed(1)
+    n_size *= 2  # WQE matrices are 2p times 2p
     normals = (1/np.sqrt(2)) * np.random.normal(loc=0, scale=np.sqrt(2), size=n_size)
     dfs = np.flip(np.arange(1, n_size))
     chisqs = (1/np.sqrt(2)) * np.array([np.sqrt(np.random.chisquare(df*beta)) for df in dfs])
 
     for i in range(n_size):
         assert normals[i] == gse.matrix[i][i]
     for i in range(n_size-1):
```

### Comparing `scikit-rmt-0.4.2/skrmt/ensemble/tests/test_manova_ens.py` & `scikit-rmt-0.5.0/skrmt/ensemble/tests/test_manova_ens.py`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.4.2/skrmt/ensemble/tests/test_plot_law.py` & `scikit-rmt-0.5.0/skrmt/ensemble/tests/test_plot_law.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 Testing module that plots spectrum limiting laws
 '''
 
 import os
 import shutil
 import pytest
 
-from skrmt.ensemble import wigner_semicircular_law
-from skrmt.ensemble import marchenko_pastur_law
-from skrmt.ensemble import tracy_widom_law
-from skrmt.ensemble import manova_spectrum_distr
+from skrmt.ensemble import wigner_semicircle
+from skrmt.ensemble import marchenko_pastur
+from skrmt.ensemble import tracy_widom
+from skrmt.ensemble import manova_spectrum
 
 
 TMP_DIR_PATH = os.path.join(os.getcwd(), "skrmt/ensemble/tests/tmp")
 
 
-@pytest.fixture(scope="session", autouse=True)
+@pytest.fixture(scope="module", autouse=True)
 def _setup_tmp_dir(request):
     """Function that is run before all tests in this script.
 
     It creates a temporary folder in order to store useful files
     for the following tests.
     """
     # if the directory already exists, it is deleted
@@ -29,635 +29,634 @@
     # creating temporary directory  
     os.mkdir(TMP_DIR_PATH)
 
     # specifying a function that will be run after all tests are completed
     request.addfinalizer(_remove_tmp_dir)
 
 
-
 def _remove_tmp_dir():
     """Function that removes the created temporary directory.
 
     The function is run when all tests in this module are completed.
     """
     shutil.rmtree(TMP_DIR_PATH)
 
 
 
 class TestWignerSemicircleLaw:
 
     def test_goe_abs_freq(self):
         fig_name = "test_wsl_goe_absfreq.png"
-        wigner_semicircular_law(
+        wigner_semicircle(
             ensemble='goe',
             n_size=100,
             bins=100,
             density=False,
-            limit_pdf=False,
+            plot_law_pdf=False,
             savefig_path=TMP_DIR_PATH+"/"+fig_name
         )
         assert os.path.isfile(os.path.join(TMP_DIR_PATH, fig_name)) == True
     
     def test_gue_abs_freq(self):
         fig_name = "test_wsl_gue_absfreq.png"
-        wigner_semicircular_law(
+        wigner_semicircle(
             ensemble='gue',
             n_size=100,
             bins=100,
             density=False,
-            limit_pdf=False,
+            plot_law_pdf=False,
             savefig_path=TMP_DIR_PATH+"/"+fig_name
         )
         assert os.path.isfile(os.path.join(TMP_DIR_PATH, fig_name)) == True
     
     def test_gse_abs_freq(self):
         fig_name = "test_wsl_gse_absfreq.png"
-        wigner_semicircular_law(
+        wigner_semicircle(
             ensemble='gse',
             n_size=50,
             bins=100,
             density=False,
-            limit_pdf=False,
+            plot_law_pdf=False,
             savefig_path=TMP_DIR_PATH+"/"+fig_name
         )
         assert os.path.isfile(os.path.join(TMP_DIR_PATH, fig_name)) == True
     
     def test_goe_normalized(self):
         fig_name = "test_wsl_goe_norm.png"
-        wigner_semicircular_law(
+        wigner_semicircle(
             ensemble='goe',
             n_size=100,
             bins=100,
             density=True,
-            limit_pdf=False,
+            plot_law_pdf=False,
             savefig_path=TMP_DIR_PATH+"/"+fig_name
         )
         assert os.path.isfile(os.path.join(TMP_DIR_PATH, fig_name)) == True
     
     def test_gue_normalized(self):
         fig_name = "test_wsl_gue_norm.png"
-        wigner_semicircular_law(
+        wigner_semicircle(
             ensemble='gue',
             n_size=100,
             bins=100,
             density=True,
-            limit_pdf=False,
+            plot_law_pdf=False,
             savefig_path=TMP_DIR_PATH+"/"+fig_name
         )
         assert os.path.isfile(os.path.join(TMP_DIR_PATH, fig_name)) == True
     
     def test_gse_normalized(self):
         fig_name = "test_wsl_gse_norm.png"
-        wigner_semicircular_law(
+        wigner_semicircle(
             ensemble='gse',
             n_size=50,
             bins=100,
             density=True,
-            limit_pdf=False,
+            plot_law_pdf=False,
             savefig_path=TMP_DIR_PATH+"/"+fig_name
         )
         assert os.path.isfile(os.path.join(TMP_DIR_PATH, fig_name)) == True
     
     def test_goe_theoretical(self):
         fig_name = "test_wsl_goe_theory.png"
-        wigner_semicircular_law(
+        wigner_semicircle(
             ensemble='goe',
             n_size=100,
             bins=100,
             density=True,
-            limit_pdf=True,
+            plot_law_pdf=True,
             savefig_path=TMP_DIR_PATH+"/"+fig_name
         )
         assert os.path.isfile(os.path.join(TMP_DIR_PATH, fig_name)) == True
     
     def test_gue_theoretical(self):
         fig_name = "test_wsl_gue_theory.png"
-        wigner_semicircular_law(
+        wigner_semicircle(
             ensemble='gue',
             n_size=100,
             bins=100,
             density=True,
-            limit_pdf=True,
+            plot_law_pdf=True,
             savefig_path=TMP_DIR_PATH+"/"+fig_name
         )
         assert os.path.isfile(os.path.join(TMP_DIR_PATH, fig_name)) == True
     
     def test_gse_theoretical(self):
         fig_name = "test_wsl_gse_theory.png"
-        wigner_semicircular_law(
+        wigner_semicircle(
             ensemble='gse',
             n_size=50,
             bins=100,
             density=True,
-            limit_pdf=True,
+            plot_law_pdf=True,
             savefig_path=TMP_DIR_PATH+"/"+fig_name
         )
         assert os.path.isfile(os.path.join(TMP_DIR_PATH, fig_name)) == True
     
     def test_wscl_size_exception(self):
         with pytest.raises(ValueError):
-            wigner_semicircular_law(
+            wigner_semicircle(
             ensemble='goe',
             n_size=0,
         )
     
     def test_wscl_ensemble_exception(self):
         with pytest.raises(ValueError):
-            wigner_semicircular_law(
+            wigner_semicircle(
             ensemble='foo',
         )
 
 
 
 class TestMarchenkoPasturLaw():
 
     def test_wre_abs_freq(self):
         fig_name = "test_mpl_wre_absfreq.png"
-        marchenko_pastur_law(
+        marchenko_pastur(
             ensemble='wre',
             p_size=40,
             n_size=100,
             bins=100,
             density=False,
-            limit_pdf=False,
+            plot_law_pdf=False,
             savefig_path=TMP_DIR_PATH+"/"+fig_name
         )
         assert os.path.isfile(os.path.join(TMP_DIR_PATH, fig_name)) == True
 
     def test_wce_abs_freq(self):
         fig_name = "test_mpl_wce_absfreq.png"
-        marchenko_pastur_law(
+        marchenko_pastur(
             ensemble='wce',
             p_size=40,
             n_size=100,
             bins=100,
             density=False,
-            limit_pdf=False,
+            plot_law_pdf=False,
             savefig_path=TMP_DIR_PATH+"/"+fig_name
         )
         assert os.path.isfile(os.path.join(TMP_DIR_PATH, fig_name)) == True
     
     def test_wqe_abs_freq(self):
         fig_name = "test_mpl_wqe_absfreq.png"
-        marchenko_pastur_law(
+        marchenko_pastur(
             ensemble='wqe',
             p_size=40,
             n_size=100,
             bins=100,
             density=False,
-            limit_pdf=False,
+            plot_law_pdf=False,
             savefig_path=TMP_DIR_PATH+"/"+fig_name
         )
         assert os.path.isfile(os.path.join(TMP_DIR_PATH, fig_name)) == True
     
     def test_wre_normalized(self):
         fig_name = "test_mpl_wre_norm.png"
-        marchenko_pastur_law(
+        marchenko_pastur(
             ensemble='wre',
             p_size=40,
             n_size=100,
             bins=100,
             density=True,
-            limit_pdf=False,
+            plot_law_pdf=False,
             savefig_path=TMP_DIR_PATH+"/"+fig_name
         )
         assert os.path.isfile(os.path.join(TMP_DIR_PATH, fig_name)) == True
 
     def test_wce_normalized(self):
         fig_name = "test_mpl_wce_norm.png"
-        marchenko_pastur_law(
+        marchenko_pastur(
             ensemble='wce',
             p_size=40,
             n_size=100,
             bins=100,
             density=True,
-            limit_pdf=False,
+            plot_law_pdf=False,
             savefig_path=TMP_DIR_PATH+"/"+fig_name
         )
         assert os.path.isfile(os.path.join(TMP_DIR_PATH, fig_name)) == True
     
     def test_wqe_normalized(self):
         fig_name = "test_mpl_wqe_norm.png"
-        marchenko_pastur_law(
+        marchenko_pastur(
             ensemble='wqe',
             p_size=40,
             n_size=100,
             bins=100,
             density=True,
-            limit_pdf=False,
+            plot_law_pdf=False,
             savefig_path=TMP_DIR_PATH+"/"+fig_name
         )
         assert os.path.isfile(os.path.join(TMP_DIR_PATH, fig_name)) == True
     
     def test_wre_theoretical(self):
         fig_name = "test_mpl_wre_theory.png"
-        marchenko_pastur_law(
+        marchenko_pastur(
             ensemble='wre',
             p_size=40,
             n_size=100,
             bins=100,
             density=True,
-            limit_pdf=True,
+            plot_law_pdf=True,
             savefig_path=TMP_DIR_PATH+"/"+fig_name
         )
         assert os.path.isfile(os.path.join(TMP_DIR_PATH, fig_name)) == True
 
     def test_wce_theoretical(self):
         fig_name = "test_mpl_wce_theory.png"
-        marchenko_pastur_law(
+        marchenko_pastur(
             ensemble='wce',
             p_size=40,
             n_size=100,
             bins=100,
             density=True,
-            limit_pdf=True,
+            plot_law_pdf=True,
             savefig_path=TMP_DIR_PATH+"/"+fig_name
         )
         assert os.path.isfile(os.path.join(TMP_DIR_PATH, fig_name)) == True
     
     def test_wqe_theoretical(self):
         fig_name = "test_mpl_wqe_theory.png"
-        marchenko_pastur_law(
+        marchenko_pastur(
             ensemble='wqe',
             p_size=40,
             n_size=100,
             bins=100,
             density=True,
-            limit_pdf=True,
+            plot_law_pdf=True,
             savefig_path=TMP_DIR_PATH+"/"+fig_name
         )
         assert os.path.isfile(os.path.join(TMP_DIR_PATH, fig_name)) == True
     
     def test_wre_ratio_ge1(self):
         fig_name = "test_mpl_wre_ratio_ge1.png"
-        marchenko_pastur_law(
+        marchenko_pastur(
             ensemble='wre',
             p_size=200,
             n_size=100,
             bins=100,
             density=False,
-            limit_pdf=False,
+            plot_law_pdf=False,
             savefig_path=TMP_DIR_PATH+"/"+fig_name
         )
         assert os.path.isfile(os.path.join(TMP_DIR_PATH, fig_name)) == True
     
     def test_wre_theoretical_ratio_ge1(self):
         fig_name = "test_mpl_wre_theory_ratio_ge1.png"
-        marchenko_pastur_law(
+        marchenko_pastur(
             ensemble='wre',
             p_size=200,
             n_size=100,
             bins=100,
             density=True,
-            limit_pdf=True,
+            plot_law_pdf=True,
             savefig_path=TMP_DIR_PATH+"/"+fig_name
         )
         assert os.path.isfile(os.path.join(TMP_DIR_PATH, fig_name)) == True
     
     def test_wre_interval(self):
         fig_name = "test_mpl_wre_interval.png"
-        marchenko_pastur_law(
+        marchenko_pastur(
             ensemble='wre',
             p_size=200,
             n_size=100,
             bins=100,
             interval=(0,10),
             density=False,
-            limit_pdf=False,
+            plot_law_pdf=False,
             savefig_path=TMP_DIR_PATH+"/"+fig_name
         )
         assert os.path.isfile(os.path.join(TMP_DIR_PATH, fig_name)) == True
     
     def test_mpl_size_exception(self):
         with pytest.raises(ValueError):
-            marchenko_pastur_law(
+            marchenko_pastur(
             ensemble='mre',
             n_size=0,
         )
     
     def test_mpl_ensemble_exception(self):
         with pytest.raises(ValueError):
-            marchenko_pastur_law(
+            marchenko_pastur(
             ensemble='foo',
         )
 
 
 
 class TestTracyWidomLaw:
 
     def test_goe_abs_freq(self):
         fig_name = "test_twl_goe_abs_freq.png"
-        tracy_widom_law(
+        tracy_widom(
             ensemble='goe',
             n_size=50,
             times=100,
             bins=100,
             density=False,
-            limit_pdf=False,
+            plot_law_pdf=False,
             savefig_path=TMP_DIR_PATH+"/"+fig_name
         )
         assert os.path.isfile(os.path.join(TMP_DIR_PATH, fig_name)) == True
     
     def test_gue_abs_freq(self):
         fig_name = "test_twl_gue_abs_freq.png"
-        tracy_widom_law(
+        tracy_widom(
             ensemble='gue',
             n_size=50,
             times=100,
             bins=100,
             density=False,
-            limit_pdf=False,
+            plot_law_pdf=False,
             savefig_path=TMP_DIR_PATH+"/"+fig_name
         )
         assert os.path.isfile(os.path.join(TMP_DIR_PATH, fig_name)) == True
     
     def test_gse_abs_freq(self):
         fig_name = "test_twl_gse_abs_freq.png"
-        tracy_widom_law(
+        tracy_widom(
             ensemble='gse',
             n_size=25,
             times=100,
             bins=100,
             density=False,
-            limit_pdf=False,
+            plot_law_pdf=False,
             savefig_path=TMP_DIR_PATH+"/"+fig_name
         )
         assert os.path.isfile(os.path.join(TMP_DIR_PATH, fig_name)) == True
     
     def test_goe_normalized(self):
         fig_name = "test_twl_goe_normalized.png"
-        tracy_widom_law(
+        tracy_widom(
             ensemble='goe',
             n_size=50,
             times=100,
             bins=100,
             density=True,
-            limit_pdf=False,
+            plot_law_pdf=False,
             savefig_path=TMP_DIR_PATH+"/"+fig_name
         )
         assert os.path.isfile(os.path.join(TMP_DIR_PATH, fig_name)) == True
     
     def test_gue_normalized(self):
         fig_name = "test_twl_gue_normalized.png"
-        tracy_widom_law(
+        tracy_widom(
             ensemble='gue',
             n_size=50,
             times=100,
             bins=100,
             density=True,
-            limit_pdf=False,
+            plot_law_pdf=False,
             savefig_path=TMP_DIR_PATH+"/"+fig_name
         )
         assert os.path.isfile(os.path.join(TMP_DIR_PATH, fig_name)) == True
     
     def test_gse_normalized(self):
         fig_name = "test_twl_gse_normalized.png"
-        tracy_widom_law(
+        tracy_widom(
             ensemble='gse',
             n_size=25,
             times=100,
             bins=100,
             density=True,
-            limit_pdf=False,
+            plot_law_pdf=False,
             savefig_path=TMP_DIR_PATH+"/"+fig_name
         )
         assert os.path.isfile(os.path.join(TMP_DIR_PATH, fig_name)) == True
     
     def test_goe_theoretical(self):
         fig_name = "test_twl_goe_theory.png"
-        tracy_widom_law(
+        tracy_widom(
             ensemble='goe',
             n_size=50,
             times=100,
             bins=100,
             density=True,
-            limit_pdf=True,
+            plot_law_pdf=True,
             savefig_path=TMP_DIR_PATH+"/"+fig_name
         )
         assert os.path.isfile(os.path.join(TMP_DIR_PATH, fig_name)) == True
     
     def test_gue_theoretical(self):
         fig_name = "test_twl_gue_theory.png"
-        tracy_widom_law(
+        tracy_widom(
             ensemble='gue',
             n_size=50,
             times=100,
             bins=100,
             density=True,
-            limit_pdf=True,
+            plot_law_pdf=True,
             savefig_path=TMP_DIR_PATH+"/"+fig_name
         )
         assert os.path.isfile(os.path.join(TMP_DIR_PATH, fig_name)) == True
     
     def test_gse_theoretical(self):
         fig_name = "test_twl_gse_theory.png"
-        tracy_widom_law(
+        tracy_widom(
             ensemble='gse',
             n_size=25,
             times=100,
             bins=100,
             density=True,
-            limit_pdf=True,
+            plot_law_pdf=True,
             savefig_path=TMP_DIR_PATH+"/"+fig_name
         )
         assert os.path.isfile(os.path.join(TMP_DIR_PATH, fig_name)) == True
     
     def test_twl_size_exception(self):
         with pytest.raises(ValueError):
-            tracy_widom_law(
+            tracy_widom(
             ensemble='goe',
             n_size=0,
         )
     
     def test_twl_ensemble_exception(self):
         with pytest.raises(ValueError):
-            tracy_widom_law(
+            tracy_widom(
             ensemble='foo',
         )
 
 
 
 class TestManovaSpectrumDistr():
 
     def test_mre_abs_freq(self):
         fig_name = "test_msd_mre_absfreq.png"
-        manova_spectrum_distr(
+        manova_spectrum(
             ensemble='mre',
             m_size=40,
             n1_size=100,
             n2_size=100,
             bins=100,
             density=False,
-            limit_pdf=False,
+            plot_law_pdf=False,
             savefig_path=TMP_DIR_PATH+"/"+fig_name
         )
         assert os.path.isfile(os.path.join(TMP_DIR_PATH, fig_name)) == True
 
     def test_mce_abs_freq(self):
         fig_name = "test_msd_mce_absfreq.png"
-        manova_spectrum_distr(
+        manova_spectrum(
             ensemble='mce',
             m_size=40,
             n1_size=100,
             n2_size=100,
             bins=100,
             density=False,
-            limit_pdf=False,
+            plot_law_pdf=False,
             savefig_path=TMP_DIR_PATH+"/"+fig_name
         )
         assert os.path.isfile(os.path.join(TMP_DIR_PATH, fig_name)) == True
     
     def test_mqe_abs_freq(self):
         fig_name = "test_msd_mqe_absfreq.png"
-        manova_spectrum_distr(
+        manova_spectrum(
             ensemble='mqe',
             m_size=40,
             n1_size=100,
             n2_size=100,
             bins=100,
             density=False,
-            limit_pdf=False,
+            plot_law_pdf=False,
             savefig_path=TMP_DIR_PATH+"/"+fig_name
         )
         assert os.path.isfile(os.path.join(TMP_DIR_PATH, fig_name)) == True
     
     def test_mre_normalized(self):
         fig_name = "test_msd_mre_norm.png"
-        manova_spectrum_distr(
+        manova_spectrum(
             ensemble='mre',
             m_size=40,
             n1_size=100,
             n2_size=100,
             bins=100,
             density=True,
-            limit_pdf=False,
+            plot_law_pdf=False,
             savefig_path=TMP_DIR_PATH+"/"+fig_name
         )
         assert os.path.isfile(os.path.join(TMP_DIR_PATH, fig_name)) == True
 
     def test_mce_normalized(self):
         fig_name = "test_msd_mce_norm.png"
-        manova_spectrum_distr(
+        manova_spectrum(
             ensemble='mce',
             m_size=40,
             n1_size=100,
             n2_size=100,
             bins=100,
             density=True,
-            limit_pdf=False,
+            plot_law_pdf=False,
             savefig_path=TMP_DIR_PATH+"/"+fig_name
         )
         assert os.path.isfile(os.path.join(TMP_DIR_PATH, fig_name)) == True
     
     def test_mqe_normalized(self):
         fig_name = "test_msd_mqe_norm.png"
-        manova_spectrum_distr(
+        manova_spectrum(
             ensemble='mqe',
             m_size=40,
             n1_size=100,
             n2_size=100,
             bins=100,
             density=True,
-            limit_pdf=False,
+            plot_law_pdf=False,
             savefig_path=TMP_DIR_PATH+"/"+fig_name
         )
         assert os.path.isfile(os.path.join(TMP_DIR_PATH, fig_name)) == True
     
     def test_mre_theoretical(self):
         fig_name = "test_msd_mre_theory.png"
-        manova_spectrum_distr(
+        manova_spectrum(
             ensemble='mre',
             m_size=40,
             n1_size=100,
             n2_size=100,
             bins=100,
             density=True,
-            limit_pdf=True,
+            plot_law_pdf=True,
             savefig_path=TMP_DIR_PATH+"/"+fig_name
         )
         assert os.path.isfile(os.path.join(TMP_DIR_PATH, fig_name)) == True
 
     def test_mce_theoretical(self):
         fig_name = "test_msd_mce_theory.png"
-        manova_spectrum_distr(
+        manova_spectrum(
             ensemble='mce',
             m_size=40,
             n1_size=100,
             n2_size=100,
             bins=100,
             density=True,
-            limit_pdf=True,
+            plot_law_pdf=True,
             savefig_path=TMP_DIR_PATH+"/"+fig_name
         )
         assert os.path.isfile(os.path.join(TMP_DIR_PATH, fig_name)) == True
     
     def test_mqe_theoretical(self):
         fig_name = "test_msd_mqe_theory.png"
-        manova_spectrum_distr(
+        manova_spectrum(
             ensemble='mqe',
             m_size=40,
             n1_size=100,
             n2_size=100,
             bins=100,
             density=True,
-            limit_pdf=True,
+            plot_law_pdf=True,
             savefig_path=TMP_DIR_PATH+"/"+fig_name
         )
         assert os.path.isfile(os.path.join(TMP_DIR_PATH, fig_name)) == True
     
     def test_mre_ratio_ge1(self):
         fig_name = "test_msd_mre_ratio_ge1.png"
-        manova_spectrum_distr(
+        manova_spectrum(
             ensemble='mre',
             m_size=200,
             n1_size=100,
             n2_size=100,
             bins=100,
             density=False,
-            limit_pdf=False,
+            plot_law_pdf=False,
             savefig_path=TMP_DIR_PATH+"/"+fig_name
         )
         assert os.path.isfile(os.path.join(TMP_DIR_PATH, fig_name)) == True
     
     def test_msd_mre_theoretical_ratio_ge1(self):
         fig_name = "test_msd_wre_theory_ratio_ge1.png"
-        manova_spectrum_distr(
+        manova_spectrum(
             ensemble='mre',
             m_size=1000,
             n1_size=800,
             n2_size=800,
             bins=100,
             density=True,
-            limit_pdf=True,
+            plot_law_pdf=True,
             savefig_path=TMP_DIR_PATH+"/"+fig_name
         )
         assert os.path.isfile(os.path.join(TMP_DIR_PATH, fig_name)) == True
     
     def test_mre_interval(self):
         fig_name = "test_msd_mre_interval.png"
-        manova_spectrum_distr(
+        manova_spectrum(
             ensemble='mre',
             m_size=200,
             n1_size=100,
             n2_size=100,
             bins=100,
             interval=(0,10),
             density=False,
-            limit_pdf=False,
+            plot_law_pdf=False,
             savefig_path=TMP_DIR_PATH+"/"+fig_name
         )
         assert os.path.isfile(os.path.join(TMP_DIR_PATH, fig_name)) == True
     
     def test_msd_size_exception(self):
         with pytest.raises(ValueError):
-            manova_spectrum_distr(
+            manova_spectrum(
             ensemble='mre',
             m_size=0,
             n1_size=0
         )
     
     def test_msd_ensemble_exception(self):
         with pytest.raises(ValueError):
-            manova_spectrum_distr(
+            manova_spectrum(
             ensemble='foo',
         )
```

### Comparing `scikit-rmt-0.4.2/skrmt/ensemble/tests/test_tracy_widom_approx.py` & `scikit-rmt-0.5.0/skrmt/ensemble/tests/test_tracy_widom_approx.py`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.4.2/skrmt/ensemble/tests/test_tridiagonalization.py` & `scikit-rmt-0.5.0/skrmt/ensemble/tests/test_tridiagonalization.py`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.4.2/skrmt/ensemble/tests/test_wishart_ens.py` & `scikit-rmt-0.5.0/skrmt/ensemble/tests/test_wishart_ens.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,37 @@
 '''Wishart Ensemble Test module
 
 Testing WishartEnsemble module
 '''
 
-from unicodedata import decimal
+import pytest
 import numpy as np
 from scipy import sparse
 from numpy.testing import (
     assert_almost_equal,
     assert_array_equal,
 )
 
 from skrmt.ensemble import WishartEnsemble
 
 
+
+def test_init_exception():
+    with pytest.raises(ValueError):
+        _ = WishartEnsemble(beta=3, p=100, n=300)
+
+def test_tridiagonal_ratio_exception():
+    with pytest.raises(ValueError):
+        _ = WishartEnsemble(beta=1, p=300, n=100, use_tridiagonal=True)
+
+def test_tridiagonal_sigma_exception():
+    with pytest.raises(ValueError):
+        _ = WishartEnsemble(beta=1, p=100, n=300, sigma=2.0, use_tridiagonal=True)
+
+
 ##########################################
 ### Wishart Real Ensemble = WRE
 
 def test_wishart_real_init():
     '''Testing WRE init
     '''
     p_size = 3
@@ -75,15 +89,15 @@
 
     # sampling WishartReal tridiagonal
     np.random.seed(1)
     wre = WishartEnsemble(beta=1, p=p_size, n=n_size, use_tridiagonal=True)
 
     # sampling chi-squares and finding tridiagonal matrix in two ways
     np.random.seed(1)
-    a_val = n_size*beta/ 2
+    a_val = n_size*beta/2
     dfs = np.arange(p_size)
     chisqs_diag = np.array([np.sqrt(np.random.chisquare(2*a_val - beta*df)) for df in dfs])
     dfs = np.flip(dfs)
     chisqs_offdiag = np.array([np.sqrt(np.random.chisquare(beta*df)) for df in dfs[:-1]])
     diagonals = [chisqs_offdiag, chisqs_diag]
     mtx = sparse.diags(diagonals, [-1, 0])
     mtx = mtx.toarray()
@@ -346,15 +360,15 @@
     assert ens.n == n_size2
     assert ens.matrix.shape == (2*p_size2,2*p_size2)
 
 
 def test_wqe_build_tridiagonal():
     '''Testing tridiagonal form of WQE
     '''
-    p_size, n_size = 3, 5
+    p_size, n_size = 2, 5
     beta = 4
 
     # sampling WishartQuaternion tridiagonal
     np.random.seed(1)
     wqe = WishartEnsemble(beta=4, p=p_size, n=n_size, use_tridiagonal=True)
 
     # sampling chi-squares and finding tridiagonal matrix in two ways
```

### Comparing `scikit-rmt-0.4.2/skrmt/ensemble/tracy_widom_approximator.py` & `scikit-rmt-0.5.0/skrmt/ensemble/tracy_widom_approximator.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,36 +2,88 @@
 
 This module implements an approximator of the Tracy-Widom distribution.
 The code is based on the open source GitHub repository
 https://github.com/yymao/TracyWidom. Tracy-Widom distribution
 functions for beta = 1, 2 and 4 are provided.
 
 References:
-    Bejan, A.
+    - Bejan, A.
         "Largest eigenvalues and sample covariance matrices".
         Tracy-Widom and Painleve II: Computational aspects and
         realization in S-Plus with applications, M.Sc. dissertation,
         Department of Statistics, The University of Warwick. (2005).
-
-    Borot, G. and Nadal, C.
+    - Borot, G. and Nadal, C.
         "Right tail expansion of Tracy-Widom beta laws".
         Random Matrices: Theory and Applications. 01.03. (2012).
-    
-    Yao-Yuan Mao.
+    - Yao-Yuan Mao.
         TracyWidom GitHUb repository. (2013).
         https://github.com/yymao/TracyWidom
 
+
+Original License from https://github.com/yymao/TracyWidom:  
+    MIT License
+
+    Copyright (c) 2021 Yao-Yuan Mao
+
+    Permission is hereby granted, free of charge, to any person obtaining a copy
+    of this software and associated documentation files (the "Software"), to deal
+    in the Software without restriction, including without limitation the rights
+    to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+    copies of the Software, and to permit persons to whom the Software is
+    furnished to do so, subject to the following conditions:
+
+    The above copyright notice and this permission notice shall be included in all
+    copies or substantial portions of the Software.
+
+    THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+    IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+    FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+    AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+    LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+    OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+    SOFTWARE.
+
+
+Modifications by Alejandro Santorum under the following license:
+    BSD 3-Clause License
+
+    Copyright (c) 2021, Alejandro Santorum Varela - alejandro.santorum@gmail.com
+    All rights reserved.
+
+    Redistribution and use in source and binary forms, with or without
+    modification, are permitted provided that the following conditions are met:
+
+    1. Redistributions of source code must retain the above copyright notice, this
+    list of conditions and the following disclaimer.
+
+    2. Redistributions in binary form must reproduce the above copyright notice,
+    this list of conditions and the following disclaimer in the documentation
+    and/or other materials provided with the distribution.
+
+    3. Neither the name of the copyright holder nor the names of its
+    contributors may be used to endorse or promote products derived from
+    this software without specific prior written permission.
+
+    THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+    AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+    IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+    DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
+    FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
+    DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
+    SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
+    CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
+    OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+    OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 """
 
 import numpy as np
 from scipy.interpolate import interp1d
 from scipy.misc import derivative
 from scipy.optimize import brentq
 
-#__all__ = ['TracyWidom']
 
 _digits_1 = b'\xc6\'\x00\x00\xd1(\x00\x00\xe2)\x00\x00\xf9*\x00\x00\x16,\x00\x009-\x00\x00c.\x00\x00\x93/\x00\x00\xc90\x00\x00\x062\x00\x00J3\x00\x00\x944\x00\x00\xe65\x00\x00>7\x00\x00\x9e8\x00\x00\x05:\x00\x00s;\x00\x00\xe9<\x00\x00f>\x00\x00\xeb?\x00\x00xA\x00\x00\rC\x00\x00\xa9D\x00\x00NF\x00\x00\xfbG\x00\x00\xb1I\x00\x00oK\x00\x005M\x00\x00\x05O\x00\x00\xddP\x00\x00\xbeR\x00\x00\xa8T\x00\x00\x9bV\x00\x00\x98X\x00\x00\x9eZ\x00\x00\xae\\\x00\x00\xc7^\x00\x00\xea`\x00\x00\x17c\x00\x00Ne\x00\x00\x8fg\x00\x00\xdai\x00\x000l\x00\x00\x90n\x00\x00\xfap\x00\x00ps\x00\x00\xf0u\x00\x00|x\x00\x00\x12{\x00\x00\xb4}\x00\x00a\x80\x00\x00\x19\x83\x00\x00\xdd\x85\x00\x00\xad\x88\x00\x00\x88\x8b\x00\x00o\x8e\x00\x00c\x91\x00\x00b\x94\x00\x00n\x97\x00\x00\x87\x9a\x00\x00\xab\x9d\x00\x00\xdd\xa0\x00\x00\x1b\xa4\x00\x00f\xa7\x00\x00\xbe\xaa\x00\x00#\xae\x00\x00\x95\xb1\x00\x00\x14\xb5\x00\x00\xa1\xb8\x00\x00<\xbc\x00\x00\xe4\xbf\x00\x00\x9a\xc3\x00\x00]\xc7\x00\x00/\xcb\x00\x00\x0e\xcf\x00\x00\xfc\xd2\x00\x00\xf8\xd6\x00\x00\x03\xdb\x00\x00\x1c\xdf\x00\x00C\xe3\x00\x00y\xe7\x00\x00\xbe\xeb\x00\x00\x12\xf0\x00\x00u\xf4\x00\x00\xe6\xf8\x00\x00g\xfd\x00\x00\xf7\x01\x01\x00\x97\x06\x01\x00E\x0b\x01\x00\x04\x10\x01\x00\xd1\x14\x01\x00\xaf\x19\x01\x00\x9c\x1e\x01\x00\x99#\x01\x00\xa6(\x01\x00\xc3-\x01\x00\xf02\x01\x00-8\x01\x00z=\x01\x00\xd7B\x01\x00EH\x01\x00\xc3M\x01\x00RS\x01\x00\xf1X\x01\x00\xa0^\x01\x00`d\x01\x001j\x01\x00\x13p\x01\x00\x05v\x01\x00\x08|\x01\x00\x1c\x82\x01\x00A\x88\x01\x00v\x8e\x01\x00\xbd\x94\x01\x00\x15\x9b\x01\x00}\xa1\x01\x00\xf7\xa7\x01\x00\x82\xae\x01\x00\x1e\xb5\x01\x00\xcb\xbb\x01\x00\x8a\xc2\x01\x00Y\xc9\x01\x00:\xd0\x01\x00,\xd7\x01\x00/\xde\x01\x00C\xe5\x01\x00i\xec\x01\x00\xa0\xf3\x01\x00\xe8\xfa\x01\x00A\x02\x02\x00\xab\t\x02\x00\'\x11\x02\x00\xb4\x18\x02\x00R \x02\x00\x02(\x02\x00\xc2/\x02\x00\x947\x02\x00w?\x02\x00jG\x02\x00oO\x02\x00\x85W\x02\x00\xac_\x02\x00\xe4g\x02\x00-p\x02\x00\x87x\x02\x00\xf1\x80\x02\x00l\x89\x02\x00\xf8\x91\x02\x00\x95\x9a\x02\x00B\xa3\x02\x00\x00\xac\x02\x00\xce\xb4\x02\x00\xad\xbd\x02\x00\x9c\xc6\x02\x00\x9c\xcf\x02\x00\xab\xd8\x02\x00\xcb\xe1\x02\x00\xfb\xea\x02\x00:\xf4\x02\x00\x8a\xfd\x02\x00\xe9\x06\x03\x00Y\x10\x03\x00\xd7\x19\x03\x00f#\x03\x00\x03-\x03\x00\xb06\x03\x00l@\x03\x008J\x03\x00\x12T\x03\x00\xfb]\x03\x00\xf3g\x03\x00\xfaq\x03\x00\x0f|\x03\x002\x86\x03\x00d\x90\x03\x00\xa4\x9a\x03\x00\xf2\xa4\x03\x00N\xaf\x03\x00\xb8\xb9\x03\x00/\xc4\x03\x00\xb4\xce\x03\x00G\xd9\x03\x00\xe6\xe3\x03\x00\x93\xee\x03\x00L\xf9\x03\x00\x12\x04\x04\x00\xe5\x0e\x04\x00\xc4\x19\x04\x00\xb0$\x04\x00\xa8/\x04\x00\xab:\x04\x00\xbbE\x04\x00\xd6P\x04\x00\xfd[\x04\x00/g\x04\x00lr\x04\x00\xb4}\x04\x00\x07\x89\x04\x00e\x94\x04\x00\xcd\x9f\x04\x00?\xab\x04\x00\xbc\xb6\x04\x00B\xc2\x04\x00\xd3\xcd\x04\x00l\xd9\x04\x00\x0f\xe5\x04\x00\xbc\xf0\x04\x00q\xfc\x04\x00/\x08\x05\x00\xf6\x13\x05\x00\xc5\x1f\x05\x00\x9c+\x05\x00|7\x05\x00cC\x05\x00RO\x05\x00H[\x05\x00Fg\x05\x00Js\x05\x00V\x7f\x05\x00h\x8b\x05\x00\x80\x97\x05\x00\x9f\xa3\x05\x00\xc3\xaf\x05\x00\xee\xbb\x05\x00\x1e\xc8\x05\x00T\xd4\x05\x00\x8e\xe0\x05\x00\xce\xec\x05\x00\x13\xf9\x05\x00\\\x05\x06\x00\xa9\x11\x06\x00\xfb\x1d\x06\x00P*\x06\x00\xa96\x06\x00\x06C\x06\x00fO\x06\x00\xc9[\x06\x00/h\x06\x00\x98t\x06\x00\x03\x81\x06\x00q\x8d\x06\x00\xe0\x99\x06\x00Q\xa6\x06\x00\xc4\xb2\x06\x009\xbf\x06\x00\xae\xcb\x06\x00%\xd8\x06\x00\x9c\xe4\x06\x00\x14\xf1\x06\x00\x8c\xfd\x06\x00\x05\n\x07\x00}\x16\x07\x00\xf5"\x07\x00m/\x07\x00\xe3;\x07\x00ZH\x07\x00\xceT\x07\x00Ba\x07\x00\xb4m\x07\x00%z\x07\x00\x93\x86\x07\x00\x00\x93\x07\x00j\x9f\x07\x00\xd2\xab\x07\x007\xb8\x07\x00\x99\xc4\x07\x00\xf8\xd0\x07\x00S\xdd\x07\x00\xac\xe9\x07\x00\x00\xf6\x07\x00Q\x02\x08\x00\x9e\x0e\x08\x00\xe6\x1a\x08\x00*\'\x08\x00i3\x08\x00\xa4?\x08\x00\xd9K\x08\x00\nX\x08\x005d\x08\x00Zp\x08\x00z|\x08\x00\x94\x88\x08\x00\xa8\x94\x08\x00\xb5\xa0\x08\x00\xbc\xac\x08\x00\xbd\xb8\x08\x00\xb7\xc4\x08\x00\xaa\xd0\x08\x00\x95\xdc\x08\x00z\xe8\x08\x00W\xf4\x08\x00-\x00\t\x00\xfb\x0b\t\x00\xc1\x17\t\x00\x7f#\t\x004/\t\x00\xe2:\t\x00\x87F\t\x00#R\t\x00\xb6]\t\x00Ai\t\x00\xc2t\t\x00:\x80\t\x00\xa9\x8b\t\x00\x0e\x97\t\x00j\xa2\t\x00\xbc\xad\t\x00\x04\xb9\t\x00B\xc4\t\x00v\xcf\t\x00\x9f\xda\t\x00\xbf\xe5\t\x00\xd3\xf0\t\x00\xdd\xfb\t\x00\xdc\x06\n\x00\xd1\x11\n\x00\xba\x1c\n\x00\x98\'\n\x00k2\n\x003=\n\x00\xefG\n\x00\xa0R\n\x00E]\n\x00\xdfg\n\x00lr\n\x00\xee|\n\x00d\x87\n\x00\xcd\x91\n\x00+\x9c\n\x00|\xa6\n\x00\xc1\xb0\n\x00\xf9\xba\n\x00%\xc5\n\x00D\xcf\n\x00W\xd9\n\x00]\xe3\n\x00V\xed\n\x00B\xf7\n\x00!\x01\x0b\x00\xf3\n\x0b\x00\xb8\x14\x0b\x00p\x1e\x0b\x00\x1b(\x0b\x00\xb81\x0b\x00H;\x0b\x00\xcbD\x0b\x00@N\x0b\x00\xa8W\x0b\x00\x02a\x0b\x00Oj\x0b\x00\x8es\x0b\x00\xc0|\x0b\x00\xe3\x85\x0b\x00\xf9\x8e\x0b\x00\x02\x98\x0b\x00\xfc\xa0\x0b\x00\xe9\xa9\x0b\x00\xc7\xb2\x0b\x00\x98\xbb\x0b\x00[\xc4\x0b\x00\x10\xcd\x0b\x00\xb7\xd5\x0b\x00P\xde\x0b\x00\xdb\xe6\x0b\x00X\xef\x0b\x00\xc7\xf7\x0b\x00(\x00\x0c\x00{\x08\x0c\x00\xbf\x10\x0c\x00\xf6\x18\x0c\x00\x1e!\x0c\x009)\x0c\x00E1\x0c\x00C9\x0c\x003A\x0c\x00\x15I\x0c\x00\xe9P\x0c\x00\xaeX\x0c\x00f`\x0c\x00\x0fh\x0c\x00\xabo\x0c\x008w\x0c\x00\xb7~\x0c\x00(\x86\x0c\x00\x8c\x8d\x0c\x00\xe1\x94\x0c\x00(\x9c\x0c\x00a\xa3\x0c\x00\x8c\xaa\x0c\x00\xa9\xb1\x0c\x00\xb8\xb8\x0c\x00\xb9\xbf\x0c\x00\xad\xc6\x0c\x00\x92\xcd\x0c\x00j\xd4\x0c\x004\xdb\x0c\x00\xf0\xe1\x0c\x00\x9e\xe8\x0c\x00?\xef\x0c\x00\xd2\xf5\x0c\x00W\xfc\x0c\x00\xcf\x02\r\x009\t\r\x00\x96\x0f\r\x00\xe5\x15\r\x00\'\x1c\r\x00["\r\x00\x82(\r\x00\x9b.\r\x00\xa84\r\x00\xa7:\r\x00\x99@\r\x00}F\r\x00UL\r\x00 R\r\x00\xddW\r\x00\x8e]\r\x002c\r\x00\xc9h\r\x00Sn\r\x00\xd0s\r\x00Ay\r\x00\xa5~\r\x00\xfc\x83\r\x00G\x89\r\x00\x86\x8e\r\x00\xb8\x93\r\x00\xde\x98\r\x00\xf7\x9d\r\x00\x04\xa3\r\x00\x05\xa8\r\x00\xfa\xac\r\x00\xe3\xb1\r\x00\xc0\xb6\r\x00\x91\xbb\r\x00V\xc0\r\x00\x10\xc5\r\x00\xbd\xc9\r\x00_\xce\r\x00\xf6\xd2\r\x00\x81\xd7\r\x00\x00\xdc\r\x00t\xe0\r\x00\xdd\xe4\r\x00:\xe9\r\x00\x8c\xed\r\x00\xd3\xf1\r\x00\x0f\xf6\r\x00@\xfa\r\x00f\xfe\r\x00\x82\x02\x0e\x00\x92\x06\x0e\x00\x98\n\x0e\x00\x93\x0e\x0e\x00\x83\x12\x0e\x00i\x16\x0e\x00E\x1a\x0e\x00\x16\x1e\x0e\x00\xdd!\x0e\x00\x99%\x0e\x00L)\x0e\x00\xf4,\x0e\x00\x920\x0e\x00\'4\x0e\x00\xb17\x0e\x002;\x0e\x00\xa9>\x0e\x00\x16B\x0e\x00zE\x0e\x00\xd4H\x0e\x00%L\x0e\x00lO\x0e\x00\xaaR\x0e\x00\xdfU\x0e\x00\x0bY\x0e\x00-\\\x0e\x00G_\x0e\x00Wb\x0e\x00_e\x0e\x00^h\x0e\x00Tk\x0e\x00Bn\x0e\x00\'q\x0e\x00\x03t\x0e\x00\xd7v\x0e\x00\xa3y\x0e\x00f|\x0e\x00!\x7f\x0e\x00\xd4\x81\x0e\x00\x7f\x84\x0e\x00!\x87\x0e\x00\xbc\x89\x0e\x00O\x8c\x0e\x00\xda\x8e\x0e\x00]\x91\x0e\x00\xd9\x93\x0e\x00M\x96\x0e\x00\xba\x98\x0e\x00\x1f\x9b\x0e\x00|\x9d\x0e\x00\xd2\x9f\x0e\x00!\xa2\x0e\x00i\xa4\x0e\x00\xaa\xa6\x0e\x00\xe3\xa8\x0e\x00\x16\xab\x0e\x00B\xad\x0e\x00f\xaf\x0e\x00\x84\xb1\x0e\x00\x9b\xb3\x0e\x00\xac\xb5\x0e\x00\xb6\xb7\x0e\x00\xb9\xb9\x0e\x00\xb6\xbb\x0e\x00\xad\xbd\x0e\x00\x9d\xbf\x0e\x00\x86\xc1\x0e\x00j\xc3\x0e\x00G\xc5\x0e\x00\x1f\xc7\x0e\x00\xf0\xc8\x0e\x00\xbb\xca\x0e\x00\x80\xcc\x0e\x00@\xce\x0e\x00\xfa\xcf\x0e\x00\xad\xd1\x0e\x00\\\xd3\x0e\x00\x04\xd5\x0e\x00\xa7\xd6\x0e\x00E\xd8\x0e\x00\xdd\xd9\x0e\x00p\xdb\x0e\x00\xfd\xdc\x0e\x00\x85\xde\x0e\x00\x08\xe0\x0e\x00\x86\xe1\x0e\x00\xff\xe2\x0e\x00r\xe4\x0e\x00\xe1\xe5\x0e\x00J\xe7\x0e\x00\xaf\xe8\x0e\x00\x0f\xea\x0e\x00j\xeb\x0e\x00\xc1\xec\x0e\x00\x12\xee\x0e\x00`\xef\x0e\x00\xa8\xf0\x0e\x00\xec\xf1\x0e\x00,\xf3\x0e\x00g\xf4\x0e\x00\x9e\xf5\x0e\x00\xd0\xf6\x0e\x00\xff\xf7\x0e\x00)\xf9\x0e\x00N\xfa\x0e\x00p\xfb\x0e\x00\x8e\xfc\x0e\x00\xa8\xfd\x0e\x00\xbd\xfe\x0e\x00\xcf\xff\x0e\x00\xdd\x00\x0f\x00\xe7\x01\x0f\x00\xed\x02\x0f\x00\xf0\x03\x0f\x00\xef\x04\x0f\x00\xea\x05\x0f\x00\xe2\x06\x0f\x00\xd6\x07\x0f\x00\xc6\x08\x0f\x00\xb3\t\x0f\x00\x9d\n\x0f\x00\x83\x0b\x0f\x00f\x0c\x0f\x00F\r\x0f\x00"\x0e\x0f\x00\xfb\x0e\x0f\x00\xd1\x0f\x0f\x00\xa4\x10\x0f\x00s\x11\x0f\x00@\x12\x0f\x00\n\x13\x0f\x00\xd0\x13\x0f\x00\x94\x14\x0f\x00U\x15\x0f\x00\x12\x16\x0f\x00\xcd\x16\x0f\x00\x86\x17\x0f\x00;\x18\x0f\x00\xee\x18\x0f\x00\x9e\x19\x0f\x00K\x1a\x0f\x00\xf6\x1a\x0f\x00\x9e\x1b\x0f\x00D\x1c\x0f\x00\xe7\x1c\x0f\x00\x87\x1d\x0f\x00&\x1e\x0f\x00\xc1\x1e\x0f\x00[\x1f\x0f\x00\xf2\x1f\x0f\x00\x86 \x0f\x00\x19!\x0f\x00\xa9!\x0f\x007"\x0f\x00\xc2"\x0f\x00L#\x0f\x00\xd3#\x0f\x00X$\x0f\x00\xdc$\x0f\x00]%\x0f\x00\xdc%\x0f\x00Y&\x0f\x00\xd4&\x0f\x00M\'\x0f\x00\xc4\'\x0f\x00:(\x0f\x00\xad(\x0f\x00\x1f)\x0f\x00\x8f)\x0f\x00\xfd)\x0f\x00i*\x0f\x00\xd4*\x0f\x00=+\x0f\x00\xa4+\x0f\x00\t,\x0f\x00m,\x0f\x00\xcf,\x0f\x000-\x0f\x00\x8f-\x0f\x00\xed-\x0f\x00I.\x0f\x00\xa3.\x0f\x00\xfc.\x0f\x00T/\x0f\x00\xaa/\x0f\x00\xff/\x0f\x00R0\x0f\x00\xa40\x0f\x00\xf50\x0f\x00D1\x0f\x00\x921\x0f\x00\xdf1\x0f\x00*2\x0f\x00t2\x0f\x00\xbd2\x0f\x00\x053\x0f\x00L3\x0f\x00\x913\x0f\x00\xd53\x0f\x00\x184\x0f\x00Z4\x0f\x00\x9b4\x0f\x00\xda4\x0f\x00\x195\x0f\x00W5\x0f\x00\x935\x0f\x00\xcf5\x0f\x00\t6\x0f\x00C6\x0f\x00{6\x0f\x00\xb36\x0f\x00\xe96\x0f\x00\x1f7\x0f\x00S7\x0f\x00\x877\x0f\x00\xba7\x0f\x00\xec7\x0f\x00\x1d8\x0f\x00N8\x0f\x00}8\x0f\x00\xac8\x0f\x00\xda8\x0f\x00\x079\x0f\x0039\x0f\x00^9\x0f\x00\x899\x0f\x00\xb39\x0f\x00\xdc9\x0f\x00\x05:\x0f\x00,:\x0f\x00T:\x0f\x00z:\x0f\x00\xa0:\x0f\x00\xc5:\x0f\x00\xe9:\x0f\x00\r;\x0f\x000;\x0f\x00R;\x0f\x00t;\x0f\x00\x96;\x0f\x00\xb6;\x0f\x00\xd6;\x0f\x00\xf6;\x0f\x00\x15<\x0f\x003<\x0f\x00Q<\x0f\x00n<\x0f\x00\x8b<\x0f\x00\xa7<\x0f\x00\xc3<\x0f\x00\xde<\x0f\x00\xf9<\x0f\x00\x13=\x0f\x00-=\x0f\x00F=\x0f\x00_=\x0f\x00w=\x0f\x00\x8f=\x0f\x00\xa7=\x0f\x00\xbe=\x0f\x00\xd4=\x0f\x00\xeb=\x0f\x00\x00>\x0f\x00\x16>\x0f\x00+>\x0f\x00?>\x0f\x00T>\x0f\x00g>\x0f\x00{>\x0f\x00\x8e>\x0f\x00\xa1>\x0f\x00\xb3>\x0f\x00\xc5>\x0f\x00\xd7>\x0f\x00\xe8>\x0f\x00\xfa>\x0f\x00\n?\x0f\x00\x1b?\x0f\x00+?\x0f\x00;?\x0f\x00J?\x0f\x00Y?\x0f\x00h?\x0f\x00w?\x0f\x00\x85?\x0f\x00\x93?\x0f\x00\xa1?\x0f\x00\xaf?\x0f\x00\xbc?\x0f\x00\xc9?\x0f\x00\xd6?\x0f\x00\xe2?\x0f\x00\xef?\x0f\x00\xfb?\x0f\x00\x07@\x0f\x00\x12@\x0f\x00\x1e@\x0f\x00)@\x0f\x004@\x0f\x00'
 
 _digits_2 = b'g\x15\x00\x00;\x16\x00\x00\x16\x17\x00\x00\xf9\x17\x00\x00\xe2\x18\x00\x00\xd4\x19\x00\x00\xcd\x1a\x00\x00\xcf\x1b\x00\x00\xd8\x1c\x00\x00\xeb\x1d\x00\x00\x05\x1f\x00\x00) \x00\x00V!\x00\x00\x8c"\x00\x00\xcc#\x00\x00\x16%\x00\x00i&\x00\x00\xc7\'\x00\x000)\x00\x00\xa3*\x00\x00!,\x00\x00\xab-\x00\x00@/\x00\x00\xe10\x00\x00\x8d2\x00\x00G4\x00\x00\x0c6\x00\x00\xdf7\x00\x00\xbe9\x00\x00\xab;\x00\x00\xa6=\x00\x00\xae?\x00\x00\xc5A\x00\x00\xeaC\x00\x00\x1eF\x00\x00aH\x00\x00\xb3J\x00\x00\x15M\x00\x00\x86O\x00\x00\x08R\x00\x00\x9bT\x00\x00>W\x00\x00\xf2Y\x00\x00\xb8\\\x00\x00\x8f_\x00\x00yb\x00\x00te\x00\x00\x83h\x00\x00\xa4k\x00\x00\xd8n\x00\x00 r\x00\x00|u\x00\x00\xecx\x00\x00p|\x00\x00\t\x80\x00\x00\xb7\x83\x00\x00{\x87\x00\x00T\x8b\x00\x00C\x8f\x00\x00H\x93\x00\x00d\x97\x00\x00\x97\x9b\x00\x00\xe1\x9f\x00\x00B\xa4\x00\x00\xbb\xa8\x00\x00L\xad\x00\x00\xf6\xb1\x00\x00\xb8\xb6\x00\x00\x93\xbb\x00\x00\x87\xc0\x00\x00\x95\xc5\x00\x00\xbd\xca\x00\x00\xff\xcf\x00\x00[\xd5\x00\x00\xd1\xda\x00\x00c\xe0\x00\x00\x0f\xe6\x00\x00\xd7\xeb\x00\x00\xbb\xf1\x00\x00\xbb\xf7\x00\x00\xd6\xfd\x00\x00\x0e\x04\x01\x00c\n\x01\x00\xd5\x10\x01\x00d\x17\x01\x00\x10\x1e\x01\x00\xd9$\x01\x00\xc0+\x01\x00\xc62\x01\x00\xe99\x01\x00+A\x01\x00\x8bH\x01\x00\nP\x01\x00\xa8W\x01\x00e_\x01\x00Ag\x01\x00=o\x01\x00Xw\x01\x00\x92\x7f\x01\x00\xed\x87\x01\x00g\x90\x01\x00\x02\x99\x01\x00\xbc\xa1\x01\x00\x97\xaa\x01\x00\x92\xb3\x01\x00\xae\xbc\x01\x00\xea\xc5\x01\x00G\xcf\x01\x00\xc4\xd8\x01\x00b\xe2\x01\x00 \xec\x01\x00\xff\xf5\x01\x00\xff\xff\x01\x00 \n\x02\x00b\x14\x02\x00\xc4\x1e\x02\x00G)\x02\x00\xeb3\x02\x00\xb0>\x02\x00\x95I\x02\x00\x9aT\x02\x00\xc1_\x02\x00\x07k\x02\x00nv\x02\x00\xf6\x81\x02\x00\x9d\x8d\x02\x00e\x99\x02\x00M\xa5\x02\x00T\xb1\x02\x00{\xbd\x02\x00\xc1\xc9\x02\x00\'\xd6\x02\x00\xac\xe2\x02\x00P\xef\x02\x00\x13\xfc\x02\x00\xf5\x08\x03\x00\xf5\x15\x03\x00\x13#\x03\x00O0\x03\x00\xa8=\x03\x00\x1fK\x03\x00\xb4X\x03\x00ef\x03\x003t\x03\x00\x1d\x82\x03\x00#\x90\x03\x00E\x9e\x03\x00\x83\xac\x03\x00\xdb\xba\x03\x00N\xc9\x03\x00\xdc\xd7\x03\x00\x84\xe6\x03\x00E\xf5\x03\x00 \x04\x04\x00\x14\x13\x04\x00 "\x04\x00D1\x04\x00\x81@\x04\x00\xd4O\x04\x00?_\x04\x00\xc0n\x04\x00W~\x04\x00\x04\x8e\x04\x00\xc6\x9d\x04\x00\x9d\xad\x04\x00\x88\xbd\x04\x00\x87\xcd\x04\x00\x99\xdd\x04\x00\xbe\xed\x04\x00\xf5\xfd\x04\x00?\x0e\x05\x00\x99\x1e\x05\x00\x05/\x05\x00\x81?\x05\x00\rP\x05\x00\xa8`\x05\x00Sq\x05\x00\x0b\x82\x05\x00\xd1\x92\x05\x00\xa5\xa3\x05\x00\x85\xb4\x05\x00q\xc5\x05\x00i\xd6\x05\x00l\xe7\x05\x00z\xf8\x05\x00\x91\t\x06\x00\xb2\x1a\x06\x00\xdc+\x06\x00\x0e=\x06\x00HN\x06\x00\x89_\x06\x00\xd1p\x06\x00\x1f\x82\x06\x00r\x93\x06\x00\xca\xa4\x06\x00\'\xb6\x06\x00\x87\xc7\x06\x00\xeb\xd8\x06\x00Q\xea\x06\x00\xb9\xfb\x06\x00#\r\x07\x00\x8e\x1e\x07\x00\xf9/\x07\x00dA\x07\x00\xceR\x07\x007d\x07\x00\x9eu\x07\x00\x03\x87\x07\x00e\x98\x07\x00\xc3\xa9\x07\x00\x1e\xbb\x07\x00s\xcc\x07\x00\xc4\xdd\x07\x00\x0f\xef\x07\x00T\x00\x08\x00\x91\x11\x08\x00\xc8"\x08\x00\xf73\x08\x00\x1eE\x08\x00;V\x08\x00Pg\x08\x00[x\x08\x00[\x89\x08\x00P\x9a\x08\x00;\xab\x08\x00\x19\xbc\x08\x00\xeb\xcc\x08\x00\xb0\xdd\x08\x00h\xee\x08\x00\x13\xff\x08\x00\xaf\x0f\t\x00= \t\x00\xbc0\t\x00+A\t\x00\x8aQ\t\x00\xd9a\t\x00\x17r\t\x00D\x82\t\x00`\x92\t\x00i\xa2\t\x00a\xb2\t\x00E\xc2\t\x00\x17\xd2\t\x00\xd5\xe1\t\x00\x7f\xf1\t\x00\x15\x01\n\x00\x96\x10\n\x00\x02 \n\x00Z/\n\x00\x9c>\n\x00\xc8M\n\x00\xdd\\\n\x00\xddk\n\x00\xc5z\n\x00\x97\x89\n\x00Q\x98\n\x00\xf4\xa6\n\x00\x7f\xb5\n\x00\xf2\xc3\n\x00L\xd2\n\x00\x8e\xe0\n\x00\xb7\xee\n\x00\xc8\xfc\n\x00\xbe\n\x0b\x00\x9c\x18\x0b\x00`&\x0b\x00\n4\x0b\x00\x9aA\x0b\x00\x10O\x0b\x00k\\\x0b\x00\xaci\x0b\x00\xd3v\x0b\x00\xde\x83\x0b\x00\xcf\x90\x0b\x00\xa4\x9d\x0b\x00_\xaa\x0b\x00\xfe\xb6\x0b\x00\x82\xc3\x0b\x00\xea\xcf\x0b\x007\xdc\x0b\x00h\xe8\x0b\x00}\xf4\x0b\x00v\x00\x0c\x00T\x0c\x0c\x00\x15\x18\x0c\x00\xbb#\x0c\x00E/\x0c\x00\xb2:\x0c\x00\x04F\x0c\x009Q\x0c\x00R\\\x0c\x00Pg\x0c\x001r\x0c\x00\xf6|\x0c\x00\x9e\x87\x0c\x00+\x92\x0c\x00\x9c\x9c\x0c\x00\xf0\xa6\x0c\x00)\xb1\x0c\x00F\xbb\x0c\x00G\xc5\x0c\x00+\xcf\x0c\x00\xf5\xd8\x0c\x00\xa2\xe2\x0c\x004\xec\x0c\x00\xaa\xf5\x0c\x00\x04\xff\x0c\x00D\x08\r\x00g\x11\r\x00p\x1a\r\x00]#\r\x000,\r\x00\xe74\r\x00\x84=\r\x00\x06F\r\x00mN\r\x00\xbaV\r\x00\xec^\r\x00\x04g\r\x00\x03o\r\x00\xe7v\r\x00\xb1~\r\x00b\x86\r\x00\xf9\x8d\r\x00w\x95\r\x00\xdc\x9c\r\x00(\xa4\r\x00Z\xab\r\x00t\xb2\r\x00v\xb9\r\x00_\xc0\r\x000\xc7\r\x00\xe9\xcd\r\x00\x8a\xd4\r\x00\x14\xdb\r\x00\x86\xe1\r\x00\xe0\xe7\r\x00$\xee\r\x00P\xf4\r\x00f\xfa\r\x00e\x00\x0e\x00N\x06\x0e\x00!\x0c\x0e\x00\xde\x11\x0e\x00\x84\x17\x0e\x00\x16\x1d\x0e\x00\x92"\x0e\x00\xf9\'\x0e\x00J-\x0e\x00\x872\x0e\x00\xb07\x0e\x00\xc4<\x0e\x00\xc4A\x0e\x00\xafF\x0e\x00\x88K\x0e\x00LP\x0e\x00\xfdT\x0e\x00\x9bY\x0e\x00&^\x0e\x00\x9fb\x0e\x00\x04g\x0e\x00Xk\x0e\x00\x99o\x0e\x00\xc9s\x0e\x00\xe6w\x0e\x00\xf3{\x0e\x00\xed\x7f\x0e\x00\xd7\x83\x0e\x00\xb0\x87\x0e\x00x\x8b\x0e\x000\x8f\x0e\x00\xd7\x92\x0e\x00o\x96\x0e\x00\xf6\x99\x0e\x00n\x9d\x0e\x00\xd6\xa0\x0e\x00/\xa4\x0e\x00y\xa7\x0e\x00\xb4\xaa\x0e\x00\xe0\xad\x0e\x00\xfe\xb0\x0e\x00\x0e\xb4\x0e\x00\x0f\xb7\x0e\x00\x03\xba\x0e\x00\xe9\xbc\x0e\x00\xc1\xbf\x0e\x00\x8c\xc2\x0e\x00J\xc5\x0e\x00\xfb\xc7\x0e\x00\x9f\xca\x0e\x006\xcd\x0e\x00\xc1\xcf\x0e\x00@\xd2\x0e\x00\xb3\xd4\x0e\x00\x1a\xd7\x0e\x00u\xd9\x0e\x00\xc4\xdb\x0e\x00\t\xde\x0e\x00B\xe0\x0e\x00p\xe2\x0e\x00\x93\xe4\x0e\x00\xac\xe6\x0e\x00\xba\xe8\x0e\x00\xbe\xea\x0e\x00\xb7\xec\x0e\x00\xa7\xee\x0e\x00\x8d\xf0\x0e\x00i\xf2\x0e\x00;\xf4\x0e\x00\x05\xf6\x0e\x00\xc5\xf7\x0e\x00{\xf9\x0e\x00)\xfb\x0e\x00\xcf\xfc\x0e\x00k\xfe\x0e\x00\xff\xff\x0e\x00\x8b\x01\x0f\x00\x0f\x03\x0f\x00\x8a\x04\x0f\x00\xfe\x05\x0f\x00j\x07\x0f\x00\xce\x08\x0f\x00+\n\x0f\x00\x80\x0b\x0f\x00\xce\x0c\x0f\x00\x15\x0e\x0f\x00U\x0f\x0f\x00\x8e\x10\x0f\x00\xc1\x11\x0f\x00\xed\x12\x0f\x00\x12\x14\x0f\x001\x15\x0f\x00J\x16\x0f\x00\\\x17\x0f\x00i\x18\x0f\x00o\x19\x0f\x00p\x1a\x0f\x00k\x1b\x0f\x00a\x1c\x0f\x00Q\x1d\x0f\x00<\x1e\x0f\x00!\x1f\x0f\x00\x02 \x0f\x00\xdd \x0f\x00\xb3!\x0f\x00\x85"\x0f\x00Q#\x0f\x00\x19$\x0f\x00\xdd$\x0f\x00\x9c%\x0f\x00V&\x0f\x00\x0c\'\x0f\x00\xbe\'\x0f\x00l(\x0f\x00\x16)\x0f\x00\xbc)\x0f\x00^*\x0f\x00\xfc*\x0f\x00\x96+\x0f\x00-,\x0f\x00\xc0,\x0f\x00P-\x0f\x00\xdc-\x0f\x00e.\x0f\x00\xea.\x0f\x00m/\x0f\x00\xec/\x0f\x00h0\x0f\x00\xe10\x0f\x00W1\x0f\x00\xcb1\x0f\x00;2\x0f\x00\xa92\x0f\x00\x143\x0f\x00|3\x0f\x00\xe23\x0f\x00E4\x0f\x00\xa64\x0f\x00\x045\x0f\x00`5\x0f\x00\xba5\x0f\x00\x116\x0f\x00g6\x0f\x00\xba6\x0f\x00\x0b7\x0f\x00Z7\x0f\x00\xa67\x0f\x00\xf17\x0f\x00:8\x0f\x00\x828\x0f\x00\xc78\x0f\x00\n9\x0f\x00L9\x0f\x00\x8c9\x0f\x00\xcb9\x0f\x00\x08:\x0f\x00C:\x0f\x00|:\x0f\x00\xb5:\x0f\x00\xeb:\x0f\x00!;\x0f\x00T;\x0f\x00\x87;\x0f\x00\xb8;\x0f\x00\xe8;\x0f\x00\x16<\x0f\x00D<\x0f\x00p<\x0f\x00\x9a<\x0f\x00\xc4<\x0f\x00\xed<\x0f\x00\x14=\x0f\x00;=\x0f\x00`=\x0f\x00\x85=\x0f\x00\xa8=\x0f\x00\xca=\x0f\x00\xec=\x0f\x00\x0c>\x0f\x00,>\x0f\x00K>\x0f\x00i>\x0f\x00\x86>\x0f\x00\xa2>\x0f\x00\xbe>\x0f\x00\xd8>\x0f\x00\xf2>\x0f\x00\x0c?\x0f\x00$?\x0f\x00<?\x0f\x00S?\x0f\x00j?\x0f\x00\x80?\x0f\x00\x95?\x0f\x00\xaa?\x0f\x00\xbe?\x0f\x00\xd1?\x0f\x00\xe4?\x0f\x00\xf6?\x0f\x00\x08@\x0f\x00\x1a@\x0f\x00+@\x0f\x00;@\x0f\x00K@\x0f\x00Z@\x0f\x00i@\x0f\x00x@\x0f\x00\x86@\x0f\x00\x94@\x0f\x00\xa1@\x0f\x00\xae@\x0f\x00\xba@\x0f\x00\xc6@\x0f\x00\xd2@\x0f\x00\xde@\x0f\x00\xe9@\x0f\x00\xf4@\x0f\x00\xfe@\x0f\x00\x08A\x0f\x00\x12A\x0f\x00\x1cA\x0f\x00%A\x0f\x00.A\x0f\x007A\x0f\x00?A\x0f\x00GA\x0f\x00OA\x0f\x00WA\x0f\x00^A\x0f\x00fA\x0f\x00mA\x0f\x00sA\x0f\x00zA\x0f\x00\x80A\x0f\x00\x87A\x0f\x00\x8dA\x0f\x00\x93A\x0f\x00\x98A\x0f\x00\x9eA\x0f\x00\xa3A\x0f\x00\xa8A\x0f\x00\xadA\x0f\x00\xb2A\x0f\x00\xb7A\x0f\x00\xbbA\x0f\x00\xbfA\x0f\x00\xc4A\x0f\x00\xc8A\x0f\x00\xccA\x0f\x00\xd0A\x0f\x00\xd3A\x0f\x00\xd7A\x0f\x00\xdaA\x0f\x00\xdeA\x0f\x00\xe1A\x0f\x00\xe4A\x0f\x00\xe7A\x0f\x00\xeaA\x0f\x00\xedA\x0f\x00\xf0A\x0f\x00\xf3A\x0f\x00\xf5A\x0f\x00\xf8A\x0f\x00\xfaA\x0f\x00\xfdA\x0f\x00\xffA\x0f\x00\x01B\x0f\x00\x03B\x0f\x00\x05B\x0f\x00\x07B\x0f\x00\tB\x0f\x00\x0bB\x0f\x00\rB\x0f\x00\x0fB\x0f\x00\x10B\x0f\x00\x12B\x0f\x00\x14B\x0f\x00\x15B\x0f\x00\x17B\x0f\x00\x18B\x0f\x00\x19B\x0f\x00\x1bB\x0f\x00\x1cB\x0f\x00\x1dB\x0f\x00\x1fB\x0f\x00 B\x0f\x00!B\x0f\x00"B\x0f\x00#B\x0f\x00$B\x0f\x00%B\x0f\x00&B\x0f\x00\'B\x0f\x00(B\x0f\x00)B\x0f\x00)B\x0f\x00*B\x0f\x00+B\x0f\x00,B\x0f\x00'
 
 _digits_4 = b'\xfa\x19\x00\x00&\x1b\x00\x00_\x1c\x00\x00\xa4\x1d\x00\x00\xf5\x1e\x00\x00S \x00\x00\xbe!\x00\x007#\x00\x00\xbe$\x00\x00T&\x00\x00\xf8\'\x00\x00\xac)\x00\x00o+\x00\x00C-\x00\x00\'/\x00\x00\x1c1\x00\x00#3\x00\x00<5\x00\x00h7\x00\x00\xa69\x00\x00\xf8;\x00\x00^>\x00\x00\xd8@\x00\x00gC\x00\x00\x0cF\x00\x00\xc7H\x00\x00\x98K\x00\x00\x80N\x00\x00\x80Q\x00\x00\x97T\x00\x00\xc8W\x00\x00\x11[\x00\x00u^\x00\x00\xf2a\x00\x00\x8ae\x00\x00>i\x00\x00\x0em\x00\x00\xfap\x00\x00\x03u\x00\x00*y\x00\x00n}\x00\x00\xd2\x81\x00\x00U\x86\x00\x00\xf8\x8a\x00\x00\xbb\x8f\x00\x00\x9f\x94\x00\x00\xa4\x99\x00\x00\xcc\x9e\x00\x00\x16\xa4\x00\x00\x84\xa9\x00\x00\x15\xaf\x00\x00\xcb\xb4\x00\x00\xa5\xba\x00\x00\xa5\xc0\x00\x00\xcb\xc6\x00\x00\x17\xcd\x00\x00\x8a\xd3\x00\x00$\xda\x00\x00\xe7\xe0\x00\x00\xd2\xe7\x00\x00\xe6\xee\x00\x00$\xf6\x00\x00\x8b\xfd\x00\x00\x1d\x05\x01\x00\xda\x0c\x01\x00\xc2\x14\x01\x00\xd6\x1c\x01\x00\x16%\x01\x00\x82-\x01\x00\x1c6\x01\x00\xe3>\x01\x00\xd8G\x01\x00\xfbP\x01\x00MZ\x01\x00\xcdc\x01\x00|m\x01\x00[w\x01\x00j\x81\x01\x00\xa9\x8b\x01\x00\x18\x96\x01\x00\xb7\xa0\x01\x00\x88\xab\x01\x00\x89\xb6\x01\x00\xbb\xc1\x01\x00\x1f\xcd\x01\x00\xb4\xd8\x01\x00{\xe4\x01\x00t\xf0\x01\x00\x9e\xfc\x01\x00\xfa\x08\x02\x00\x88\x15\x02\x00H"\x02\x00:/\x02\x00^<\x02\x00\xb4I\x02\x00;W\x02\x00\xf4d\x02\x00\xdfr\x02\x00\xfc\x80\x02\x00J\x8f\x02\x00\xc9\x9d\x02\x00y\xac\x02\x00Z\xbb\x02\x00l\xca\x02\x00\xae\xd9\x02\x00 \xe9\x02\x00\xc2\xf8\x02\x00\x93\x08\x03\x00\x93\x18\x03\x00\xc2(\x03\x00\x1f9\x03\x00\xaaI\x03\x00bZ\x03\x00Gk\x03\x00Y|\x03\x00\x96\x8d\x03\x00\x00\x9f\x03\x00\x93\xb0\x03\x00R\xc2\x03\x009\xd4\x03\x00J\xe6\x03\x00\x84\xf8\x03\x00\xe5\n\x04\x00m\x1d\x04\x00\x1b0\x04\x00\xefB\x04\x00\xe8U\x04\x00\x05i\x04\x00F|\x04\x00\xa9\x8f\x04\x00.\xa3\x04\x00\xd3\xb6\x04\x00\x99\xca\x04\x00~\xde\x04\x00\x81\xf2\x04\x00\xa2\x06\x05\x00\xdf\x1a\x05\x007/\x05\x00\xabC\x05\x007X\x05\x00\xddl\x05\x00\x9a\x81\x05\x00o\x96\x05\x00X\xab\x05\x00W\xc0\x05\x00i\xd5\x05\x00\x8e\xea\x05\x00\xc4\xff\x05\x00\x0b\x15\x06\x00b*\x06\x00\xc7?\x06\x009U\x06\x00\xb8j\x06\x00B\x80\x06\x00\xd6\x95\x06\x00\x87\xab\x06\x00\x19\xc1\x06\x00\xc5\xd6\x06\x00w\xec\x06\x00-\x02\x07\x00\xe7\x17\x07\x00\xa4-\x07\x00bC\x07\x00!Y\x07\x00\xden\x07\x00\x9a\x84\x07\x00S\x9a\x07\x00\x08\xb0\x07\x00\xb8\xc5\x07\x00b\xdb\x07\x00\x04\xf1\x07\x00\x9f\x06\x08\x000\x1c\x08\x00\xb71\x08\x002G\x08\x00\xa1\\\x08\x00\x03r\x08\x00V\x87\x08\x00\x9a\x9c\x08\x00\xcd\xb1\x08\x00\xef\xc6\x08\x00\xff\xdb\x08\x00\xfc\xf0\x08\x00\xe4\x05\t\x00\xb8\x1a\t\x00u/\t\x00\x1cD\t\x00\xabX\t\x00!m\t\x00~\x81\t\x00\xc0\x95\t\x00\xe7\xa9\t\x00\xf3\xbd\t\x00\xe2\xd1\t\x00\xb3\xe5\t\x00f\xf9\t\x00\xfb\x0c\n\x00o \n\x00\xc43\n\x00\xf7F\n\x00\tZ\n\x00\xf8l\n\x00\xc5\x7f\n\x00n\x92\n\x00\xf3\xa4\n\x00S\xb7\n\x00\x8e\xc9\n\x00\xa4\xdb\n\x00\x93\xed\n\x00[\xff\n\x00\xfd\x10\x0b\x00v"\x0b\x00\xc83\x0b\x00\xf1D\x0b\x00\xf2U\x0b\x00\xc9f\x0b\x00vw\x0b\x00\xfa\x87\x0b\x00T\x98\x0b\x00\x83\xa8\x0b\x00\x87\xb8\x0b\x00a\xc8\x0b\x00\x0f\xd8\x0b\x00\x91\xe7\x0b\x00\xe9\xf6\x0b\x00\x14\x06\x0c\x00\x13\x15\x0c\x00\xe6#\x0c\x00\x8d2\x0c\x00\x07A\x0c\x00UO\x0c\x00w]\x0c\x00lk\x0c\x004y\x0c\x00\xd0\x86\x0c\x00?\x94\x0c\x00\x81\xa1\x0c\x00\x97\xae\x0c\x00\x80\xbb\x0c\x00=\xc8\x0c\x00\xcd\xd4\x0c\x001\xe1\x0c\x00i\xed\x0c\x00u\xf9\x0c\x00T\x05\r\x00\x08\x11\r\x00\x90\x1c\r\x00\xed\'\r\x00\x1e3\r\x00$>\r\x00\xffH\r\x00\xafS\r\x005^\r\x00\x91h\r\x00\xc2r\r\x00\xca|\r\x00\xa8\x86\r\x00^\x90\r\x00\xea\x99\r\x00M\xa3\r\x00\x88\xac\r\x00\x9c\xb5\r\x00\x87\xbe\r\x00K\xc7\r\x00\xe8\xcf\r\x00_\xd8\r\x00\xaf\xe0\r\x00\xd9\xe8\r\x00\xde\xf0\r\x00\xbd\xf8\r\x00w\x00\x0e\x00\r\x08\x0e\x00\x7f\x0f\x0e\x00\xcd\x16\x0e\x00\xf8\x1d\x0e\x00\xff$\x0e\x00\xe5+\x0e\x00\xa82\x0e\x00I9\x0e\x00\xc9?\x0e\x00(F\x0e\x00gL\x0e\x00\x85R\x0e\x00\x84X\x0e\x00c^\x0e\x00$d\x0e\x00\xc6i\x0e\x00Ko\x0e\x00\xb1t\x0e\x00\xfby\x0e\x00\'\x7f\x0e\x008\x84\x0e\x00,\x89\x0e\x00\x05\x8e\x0e\x00\xc3\x92\x0e\x00g\x97\x0e\x00\xf0\x9b\x0e\x00_\xa0\x0e\x00\xb5\xa4\x0e\x00\xf2\xa8\x0e\x00\x16\xad\x0e\x00"\xb1\x0e\x00\x17\xb5\x0e\x00\xf4\xb8\x0e\x00\xba\xbc\x0e\x00i\xc0\x0e\x00\x02\xc4\x0e\x00\x86\xc7\x0e\x00\xf4\xca\x0e\x00M\xce\x0e\x00\x92\xd1\x0e\x00\xc2\xd4\x0e\x00\xde\xd7\x0e\x00\xe7\xda\x0e\x00\xdd\xdd\x0e\x00\xc0\xe0\x0e\x00\x91\xe3\x0e\x00P\xe6\x0e\x00\xfd\xe8\x0e\x00\x98\xeb\x0e\x00#\xee\x0e\x00\x9d\xf0\x0e\x00\x07\xf3\x0e\x00a\xf5\x0e\x00\xab\xf7\x0e\x00\xe6\xf9\x0e\x00\x12\xfc\x0e\x000\xfe\x0e\x00?\x00\x0f\x00@\x02\x0f\x003\x04\x0f\x00\x19\x06\x0f\x00\xf2\x07\x0f\x00\xbe\t\x0f\x00}\x0b\x0f\x000\r\x0f\x00\xd8\x0e\x0f\x00s\x10\x0f\x00\x03\x12\x0f\x00\x88\x13\x0f\x00\x02\x15\x0f\x00q\x16\x0f\x00\xd6\x17\x0f\x001\x19\x0f\x00\x82\x1a\x0f\x00\xc9\x1b\x0f\x00\x07\x1d\x0f\x00;\x1e\x0f\x00g\x1f\x0f\x00\x8a \x0f\x00\xa4!\x0f\x00\xb6"\x0f\x00\xc0#\x0f\x00\xc2$\x0f\x00\xbd%\x0f\x00\xaf&\x0f\x00\x9b\'\x0f\x00\x7f(\x0f\x00])\x0f\x004*\x0f\x00\x04+\x0f\x00\xce+\x0f\x00\x91,\x0f\x00O-\x0f\x00\x06.\x0f\x00\xb8.\x0f\x00d/\x0f\x00\x0b0\x0f\x00\xad0\x0f\x00J1\x0f\x00\xe11\x0f\x00t2\x0f\x00\x023\x0f\x00\x8b3\x0f\x00\x104\x0f\x00\x914\x0f\x00\x0e5\x0f\x00\x865\x0f\x00\xfa5\x0f\x00k6\x0f\x00\xd86\x0f\x00A7\x0f\x00\xa77\x0f\x00\n8\x0f\x00i8\x0f\x00\xc58\x0f\x00\x1e9\x0f\x00t9\x0f\x00\xc69\x0f\x00\x17:\x0f\x00d:\x0f\x00\xaf:\x0f\x00\xf7:\x0f\x00<;\x0f\x00\x80;\x0f\x00\xc1;\x0f\x00\xff;\x0f\x00<<\x0f\x00v<\x0f\x00\xae<\x0f\x00\xe5<\x0f\x00\x19=\x0f\x00K=\x0f\x00|=\x0f\x00\xab=\x0f\x00\xd8=\x0f\x00\x04>\x0f\x00.>\x0f\x00W>\x0f\x00~>\x0f\x00\xa3>\x0f\x00\xc8>\x0f\x00\xea>\x0f\x00\x0c?\x0f\x00,?\x0f\x00L?\x0f\x00j?\x0f\x00\x87?\x0f\x00\xa2?\x0f\x00\xbd?\x0f\x00\xd7?\x0f\x00\xf0?\x0f\x00\x08@\x0f\x00\x1f@\x0f\x005@\x0f\x00J@\x0f\x00_@\x0f\x00r@\x0f\x00\x85@\x0f\x00\x97@\x0f\x00\xa9@\x0f\x00\xba@\x0f\x00\xca@\x0f\x00\xd9@\x0f\x00\xe8@\x0f\x00\xf6@\x0f\x00\x04A\x0f\x00\x11A\x0f\x00\x1eA\x0f\x00*A\x0f\x006A\x0f\x00AA\x0f\x00LA\x0f\x00VA\x0f\x00`A\x0f\x00jA\x0f\x00sA\x0f\x00|A\x0f\x00\x84A\x0f\x00\x8cA\x0f\x00\x94A\x0f\x00\x9bA\x0f\x00\xa2A\x0f\x00\xa9A\x0f\x00\xb0A\x0f\x00\xb6A\x0f\x00\xbcA\x0f\x00\xc2A\x0f\x00\xc7A\x0f\x00\xcdA\x0f\x00\xd2A\x0f\x00\xd7A\x0f\x00\xdbA\x0f\x00\xe0A\x0f\x00\xe4A\x0f\x00\xe8A\x0f\x00\xecA\x0f\x00\xf0A\x0f\x00\xf3A\x0f\x00'
 
@@ -73,26 +125,24 @@
             break
     else:
         raise ValueError("Cannot find u with brentq")
     v = vv(u)
     return u, v
 
 
-
 class TW_Approximator(object):
     """Provide the Tracy-Widom distribution functions for beta = 1, 2, or 4.
 
     References:
-        Bejan, A.
+        - Bejan, A.
             "Largest eigenvalues and sample covariance matrices".
             Tracy-Widom and Painleve II: Computational aspects and
             realization in S-Plus with applications, M.Sc. dissertation,
             Department of Statistics, The University of Warwick. (2005).
-
-        Borot, G. and Nadal, C.
+        - Borot, G. and Nadal, C.
             "Right tail expansion of Tracy-Widom beta laws".
             Random Matrices: Theory and Applications. 01.03. (2012).
     """
 
     def __init__(self, beta=1):
         """Construnct a TW_Approximator class for a given beta.
 
@@ -120,15 +170,15 @@
         self.beta = b
         ib = [1, 2, 4].index(b)
 
         x = np.arange(*xlim, dtype=np.int32).astype(float) * 1.e-2
         # y = np.fromstring(digits, dtype=np.int32).astype(float) * 1.e-6
         y = np.frombuffer(digits, dtype=np.int32).astype(float) * 1.e-6
         self.__xlim = (x[1], x[-2])
-        self.__cdf    = interp1d(x, y, kind='cubic', bounds_error=False)
+        self.__cdf = interp1d(x, y, kind='cubic', bounds_error=False)
 
         dlnf = derivative(lambda xx: np.log(self.__cdf(-xx)), -x[1], \
                 dx=3.33e-3, order=7)
         self.__para_n = _para_n[ib] \
                 + list(_find_u_v(-x[1], y[1], dlnf, *_para_n[ib]))
         self.__asym_n = lambda xx: _f(-xx, *self.__para_n)
         self.__asym_inv_n = lambda yy: -(_finv(yy, *self.__para_n))
@@ -144,15 +194,15 @@
         y = self.cdf(x)
         self.__ylim = (y[0], y[-1])
         self.__cdfinv = interp1d(self.cdf(x), x, bounds_error=False)
 
 
     def cdf(self, x):
         """Return the cumulative distribution function at x.
-        cdf(x) = P(TW < x)
+        :math:`cdf(x) = \mathbb{P}(TW < x)`.
 
         Args:
             x (float or array-like): value to evaluate the cdf.
 
         Returns:
             y (float or array-like): result of y = cdf(x).
         """
@@ -165,15 +215,15 @@
         flag = xa > self.__xlim[1]
         y[flag] = self.__asym_p(xa[flag])
         return y[0] if scalar else y
 
 
     def pdf(self, x):
         """Return the probability distribution function at x.
-        pdf(x) = d P(TW < x) / dx.
+        :math:`pdf(x) = \frac{d}{dx} \mathbb{P}(TW < x)`.
 
         Args:
             x (float or array-like): value to evaluate the pdf.
 
         Returns:
             y (float or array-like): result of y = pdf(x).
         """
```

### Comparing `scikit-rmt-0.4.2/skrmt/ensemble/tridiagonal_utils.py` & `scikit-rmt-0.5.0/skrmt/ensemble/tridiagonal_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,30 +28,30 @@
         sturm_seq[i] = tridiag_mtx[n_size-i-1][n_size-i-1] - \
                         ((tridiag_mtx[n_size-i-1][n_size-i]**2)/sturm_seq[i-1])
 
     # number of negative values in R sequence
     return (sturm_seq<0).sum()
 
 
-def tridiag_eigval_hist(tridiag_mtx, bins=100, interval=(-2,2), density=False):
+def tridiag_eigval_hist(tridiag_mtx, interval, bins=100, density=False):
     """Computes efficiently eigenvalue histogram.
 
-    Computes the eigenvalue histogram of the given matrix, using the
+    Calculates the eigenvalue histogram of the given matrix, using the
     specified bins between the introduced interval. The given matrix has
     to be tridiagonal, so this function builds the histogram efficiently
     using Sturm sequences, avoiding to calculate eigenvalues.
 
     Args:
         tridiag_mtx (numpy array): tridiagonal matrix
+        interval (tuple): Delimiters (xmin, xmax) of the histogram. The lower and upper
+            range of the bins. Lower and upper outliers are ignored.
         bins (int or sequence, default=100): If bins is an integer, it defines the number of
             equal-width bins in the range. If bins is a sequence, it defines the
             bin edges, including the left edge of the first bin and the right
             edge of the last bin; in this case, bins may be unequally spaced.
-        interval (tuple, default=(-2,2)): Delimiters (xmin, xmax) of the histogram.
-            The lower and upper range of the bins. Lower and upper outliers are ignored.
         density (bool, default=False): If True, draw and return a probability
             density: each bin will display the bin's raw count divided by the total
             number of counts and the bin width, so that the area under the histogram
             integrates to 1. If set to False, the absolute frequencies of the eigenvalues
             are returned.
 
     Returns:
@@ -118,15 +118,15 @@
             mtx (nparray): tridiagonalized matrix.
             mtx_list (nparray): list of matrices representing the evolution of the given matrix
             after each rotation. Only returned if ret_iterations is set to True.
             rot_list (nparray): list of applied rotation matrices. Only returned if
             ret_iterations is set to True.
 
     References:
-        R. Hildebrand. “Householder numerically with mathematica.” 2007.
+        - R. Hildebrand. “Householder numerically with mathematica.” 2007.
             http://buzzard.ups.edu/courses/2007spring/projects/hildebrand-paper-revised.pdf
     """
     n_size = len(mtx)
 
     mtx_list = [mtx]
     rot_list = []
```

### Comparing `scikit-rmt-0.4.2/skrmt/ensemble/wishart_ensemble.py` & `scikit-rmt-0.5.0/skrmt/ensemble/wishart_ensemble.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,16 +5,15 @@
 mainly three sub-ensembles: Wishart Real Ensemble, Wishart Complex Ensemble
 and Wishart Quaternion Ensemble.
 
 """
 
 import numpy as np
 import matplotlib.pyplot as plt
-from scipy import special
-from scipy import sparse
+from scipy import sparse, special
 
 from ._base_ensemble import _Ensemble
 from .tridiagonal_utils import tridiag_eigval_hist
 
 
 #########################################################################
 ### Wishart Ensemble = Laguerre Ensemble
@@ -37,73 +36,84 @@
     multiplied by its transpose in order to generate a matrix of
     the Wishart Quaternion Ensemble.
 
     Attributes:
         matrix (numpy array): instance of the WishartReal, WishartComplex
             or WishartQuaternion random ensembles. If it is an instance
             of WishartReal or WishartComplex, the random matrix is of
-            size n times n. If it is a WishartQuaternion, the random matrix
-            is of size 2n times 2n.
+            size p times p. If it is a WishartQuaternion, the random matrix
+            is of size 2p times 2p.
         beta (int): descriptive integer of the Wishart ensemble type.
             For Real beta=1, for Complex beta=2, for Quaternion beta=4.
         p (int): number of rows of the guassian matrix that generates
             the matrix of the corresponding ensemble.
         n (int): number of columns of the guassian matrix that generates
             the matrix of the corresponding ensemble.
         use_tridiagonal (bool): if set to True, Gaussian Ensemble
             matrices are sampled in its tridiagonal form, which has the same
             eigenvalues than its standard form. Otherwise, it is sampled using
             its standard form.
+        sigma (float): scale (standard deviation) of the random entries of the
+            sampled matrix.
 
     References:
-        Albrecht, J. and Chan, C.P. and Edelman, A.
+        - Albrecht, J. and Chan, C.P. and Edelman, A.
             "Sturm sequences and random eigenvalue distributions".
             Foundations of Computational Mathematics. 9.4 (2008): 461-483.
-        Dumitriu, I. and Edelman, A. "Matrix Models for Beta Ensembles".
+        - Dumitriu, I. and Edelman, A. "Matrix Models for Beta Ensembles".
             Journal of Mathematical Physics. 43.11 (2002): 5830-5847.
+        - Bar, Z.D. and Silverstain, J.W.
+            Spectral Analysis of Large Dimensional Random Matrices.
+            2nd edition. Springer. (2010).
 
     """
 
-    def __init__(self, beta, p, n, use_tridiagonal=False):
+    def __init__(self, beta, p, n, use_tridiagonal=False, sigma=1.0):
         """Constructor for WishartEnsemble class.
 
         Initializes an instance of this class with the given parameters.
 
         Args:
             beta (int): descriptive integer of the Wishart ensemble type.
                 For Real beta=1, for Complex beta=2, for Quaternion beta=4
             p (int): number of rows of the guassian matrix that generates
                 the matrix of the corresponding ensemble.
             n (int): number of columns of the guassian matrix that generates
                 the matrix of the corresponding ensemble.
             use_tridiagonal (bool, default=False): if set to True, Wishart Ensemble
-            matrices are sampled in its tridiagonal form, which has the same
-            eigenvalues than its standard form.
+                matrices are sampled in its tridiagonal form, which has the same
+                eigenvalues than its standard form.
+            sigma (float, 1.0): scale (standard deviation) of the random entries of the
+                sampled matrix.
 
         """
+        if beta not in [1,2,4]:
+            raise ValueError(f"Invalid beta: {beta}. Beta value has to be 1, 2 or 4.")
+
         super().__init__()
         # pylint: disable=invalid-name
         self.p = p
         self.n = n
         self.beta = beta
         self.use_tridiagonal = use_tridiagonal
+        self.sigma = sigma
         self.matrix = self.sample()
 
-    def set_size(self, p, n, resample_mtx=False):
+    def set_size(self, p, n, resample_mtx=True):
         # pylint: disable=arguments-differ
         """Setter of matrix size.
 
         Sets the matrix size. Useful if it has been initialized with a different value.
 
         Args:
             p (int): number of rows of the guassian matrix that generates
                 the matrix of the corresponding ensemble.
             n (int): number of columns of the guassian matrix that generates
                 the matrix of the corresponding ensemble.
-            resample_mtx (bool, default=False): If set to True, the ensemble matrix is
+            resample_mtx (bool, default=True): If set to True, the ensemble matrix is
                 resampled with the new dimensions.
 
         """
         self.p = p
         self.n = n
         if resample_mtx:
             self.matrix = self.sample()
@@ -118,52 +128,63 @@
         is sampled. Otherwise, it is sampled using the standard
         form.
 
         Returns:
             numpy array containing new matrix sampled.
 
         References:
-            Dumitriu, I. and Edelman, A. "Matrix Models for Beta Ensembles".
+            - Dumitriu, I. and Edelman, A. "Matrix Models for Beta Ensembles".
                 Journal of Mathematical Physics. 43.11 (2002): 5830-5847.
         """
         if self.use_tridiagonal:
+            if self.p > self.n:  # check reference ("Matrix Models for Beta Ensembles"): page 5, table 1.
+                raise ValueError("Error: cannot use tridiagonal form if 'p' (degrees of freedom)"
+                                 " is greater than 'n' (sample size).\n"
+                                 f"\t Provided n={self.n} and p={self.p}."
+                                 " Set `use_tridiagonal=False` or increase sample size (`n`).")
+            
+            if self.sigma != 1.0:
+                raise ValueError("Error: cannot sample tridiagonal random matrix using non-unitary scale"
+                                f" (sigma = {self.sigma}).\n"
+                                "\t Set `sigma=1.0` (default) or deactivate tridiagonal sampling.")
+
             return self.sample_tridiagonal()
 
         if self.beta == 1:
             return self._sample_wre()
         if self.beta == 2:
             return self._sample_wce()
         if self.beta == 4:
             return self._sample_wqe()
 
     def _sample_wre(self):
         p_size = self.p
         n_size = self.n
         # p by n matrix of random Gaussians
-        mtx = np.random.randn(p_size,n_size)
+        mtx = np.random.randn(p_size,n_size) * self.sigma
         # symmetrize matrix
         self.matrix = np.matmul(mtx, mtx.transpose())
         return self.matrix
 
     def _sample_wce(self):
         p_size = self.p
         n_size = self.n
         # p by n random complex matrix of random Gaussians
-        mtx = np.random.randn(p_size,n_size) + (0+1j)*np.random.randn(p_size,n_size)
+        mtx = np.random.randn(p_size,n_size)*self.sigma + 1j*np.random.randn(p_size,n_size)*self.sigma
         # hermitian matrix
         self.matrix = np.matmul(mtx, mtx.transpose().conj())
         return self.matrix
 
     def _sample_wqe(self):
         p_size = self.p
         n_size = self.n
         # p by n random complex matrix of random Gaussians
-        x_mtx = np.random.randn(p_size,n_size) + (0+1j)*np.random.randn(p_size,n_size)
+        x_mtx = np.random.randn(p_size,n_size)*self.sigma + 1j*np.random.randn(p_size,n_size)*self.sigma
         # p by n random complex matrix of random Gaussians
-        y_mtx = np.random.randn(p_size,n_size) + (0+1j)*np.random.randn(p_size,n_size)
+        y_mtx = np.random.randn(p_size,n_size)*self.sigma + 1j*np.random.randn(p_size,n_size)*self.sigma
         # [X Y; -conj(Y) conj(X)]
         mtx = np.block([
                         [x_mtx              , y_mtx],
                         [-np.conjugate(y_mtx), np.conjugate(x_mtx)]
                     ])
         # hermitian matrix
         self.matrix = np.matmul(mtx, mtx.transpose().conj())
@@ -176,22 +197,22 @@
         beta=1 is Real, beta=2 is Complex and beta=4 is Quaternion) in its
         tridiagonal form.
 
         Returns:
             numpy array containing new matrix sampled.
 
         References:
-            Albrecht, J. and Chan, C.P. and Edelman, A.
+            - Albrecht, J. and Chan, C.P. and Edelman, A.
                 "Sturm sequences and random eigenvalue distributions".
                 Foundations of Computational Mathematics. 9.4 (2008): 461-483.
-            Dumitriu, I. and Edelman, A. "Matrix Models for Beta Ensembles".
+            - Dumitriu, I. and Edelman, A. "Matrix Models for Beta Ensembles".
                 Journal of Mathematical Physics. 43.11 (2002): 5830-5847.
 
         '''
-        a_val = self.n*self.beta/ 2
+        a_val = self.n*self.beta/2
         # sampling chi-squares
         dfs = np.arange(self.p)
         chisqs_diag = np.array([np.sqrt(np.random.chisquare(2*a_val - self.beta*df)) for df in dfs])
         dfs = np.flip(dfs)
         chisqs_offdiag = np.array([np.sqrt(np.random.chisquare(self.beta*df)) for df in dfs[:-1]])
         # calculating tridiagonal diagonals
         diag = np.array([chisqs_diag[0]**2]+[chisqs_diag[i+1]**2 + \
@@ -202,15 +223,15 @@
         mtx = sparse.diags(diagonals, [-1, 0, 1])
         # converting to numpy array
         self.matrix = mtx.toarray()
         return self.matrix
 
 
     def eigvals(self):
-        """Calculates the random matrix eigenvalues.
+        """Computes the random matrix eigenvalues.
 
         Calculates the random matrix eigenvalues using numpy standard procedure.
         If the matrix ensemble is symmetric, a faster algorithm is used.
 
         Returns:
             numpy array with the calculated eigenvalues.
 
@@ -222,24 +243,24 @@
             if norm_const:
                 return tridiag_eigval_hist(self.matrix*norm_const, bins=bins,
                                            interval=interval, density=density)
             return tridiag_eigval_hist(self.matrix, bins=bins, interval=interval, density=density)
 
         return super().eigval_hist(bins, interval, density, norm_const, avoid_img=avoid_img)
 
-    def plot_eigval_hist(self, bins, interval=None, density=False, norm_const=None, fig_path=None):
-        """Calculates and plots the histogram of the matrix eigenvalues
+    def plot_eigval_hist(self, bins=100, interval=None, density=False, norm_const=None, fig_path=None):
+        """Computes and plots the histogram of the matrix eigenvalues.
 
         Calculates and plots the histogram of the current sampled matrix eigenvalues.
         Gaussian (Hermite) ensemble and Wishart (Laguerre) ensemble have improved
         routines to avoid calculating the eigenvalues, so the histogram
         is built using certain techniques to boost efficiency.
 
         Args:
-            bins (int or sequence): If bins is an integer, it defines the number of
+            bins (int or sequence, default=100): If bins is an integer, it defines the number of
                 equal-width bins in the range. If bins is a sequence, it defines the
                 bin edges, including the left edge of the first bin and the right
                 edge of the last bin; in this case, bins may be unequally spaced.
             interval (tuple, default=None): Delimiters (xmin, xmax) of the histogram.
                 The lower and upper range of the bins. Lower and upper outliers are ignored.
             density (bool, default=False): If True, draw and return a probability
                 density: each bin will display the bin's raw count divided by the total
@@ -247,64 +268,64 @@
                 integrates to 1. If set to False, the absolute frequencies of the eigenvalues
                 are returned.
             norm_const (float, default=None): Eigenvalue normalization constant. By default,
                 it is set to None, so eigenvalues are not normalized. However, it is advisable
                 to specify a normalization constant to observe eigenvalue spectrum, e.g.
                 1/sqrt(n/2) if you want to analyze Wigner's Semicircular Law.
             fig_path (string, default=None): path to save the created figure. If it is not
-                provided, the plot is shown are the end of the routine.
+                provided, the plot is shown at the end of the routine.
 
         References:
-            Albrecht, J. and Chan, C.P. and Edelman, A.
+            - Albrecht, J. and Chan, C.P. and Edelman, A.
                 "Sturm sequences and random eigenvalue distributions".
                 Foundations of Computational Mathematics. 9.4 (2008): 461-483.
-            Dumitriu, I. and Edelman, A.
+            - Dumitriu, I. and Edelman, A.
                 "Matrix Models for Beta Ensembles".
                 Journal of Mathematical Physics. 43.11 (2002): 5830-5847.
 
         """
         # pylint: disable=too-many-arguments
         if norm_const is None:
-            norm_const = 1/self.n
+            norm_const = 1/self.n 
         if interval is None:
+            # calculating constants depending on matrix sizes
             ratio = self.p/self.n
-            lambda_plus = self.beta * (1 + np.sqrt(ratio))**2
-            lambda_minus = self.beta * (1 - np.sqrt(ratio))**2
+            lambda_plus = self.beta * self.sigma**2 * (1 + np.sqrt(ratio))**2
+            lambda_minus = self.beta * self.sigma**2 * (1 - np.sqrt(ratio))**2
             interval = (lambda_minus, lambda_plus)
 
         if self.use_tridiagonal:
             observed, bins = tridiag_eigval_hist(self.matrix*norm_const, bins=bins,
                                                  interval=interval, density=density)
             width = bins[1]-bins[0]
             plt.bar(bins[:-1], observed, width=width, align='edge')
-            plt.title("Eigenvalue density histogram (matrix size: "+\
-                      str(len(self.matrix))+"x"+str(len(self.matrix))+")", fontweight="bold")
+            plt.title("Eigenvalue density histogram", fontweight="bold")
             plt.xlabel("x")
             plt.ylabel("density")
             # Saving plot or showing it
             if fig_path:
                 plt.savefig(fig_path, dpi=1000)
             else:
                 plt.show()
 
         else:
             super().plot_eigval_hist(bins, interval, density, norm_const, fig_path)
 
     def eigval_pdf(self):
-        '''Calculates joint eigenvalue pdf.
+        '''Computes joint eigenvalue pdf.
 
         Calculates joint eigenvalue probability density function given the current
             random matrix (so its eigenvalues). This function depends on beta, i.e.,
             in the sub-Wishart ensemble.
 
         Returns:
             real number. Value of the joint pdf of the current eigenvalues.
 
         References:
-            Dumitriu, I. and Edelman, A. "Matrix Models for Beta Ensembles".
+            - Dumitriu, I. and Edelman, A. "Matrix Models for Beta Ensembles".
                 Journal of Mathematical Physics. 43.11 (2002): 5830-5847.
 
         '''
         a_val = self.beta*self.n/2
         p_aux = 1 + self.beta/2*(self.p - 1)
         # calculating Laguerre eigval pdf constant depeding on beta
         const_beta = 2**(-self.p*a_val)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `scikit-rmt-0.4.2/tutorial/plot_introduction.py` & `scikit-rmt-0.5.0/tutorial/plot_0_introduction.py`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.4.2/tutorial/plot_spectral_laws.py` & `scikit-rmt-0.5.0/tutorial/plot_2_plot_spectral_laws.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Analyzing spectral laws 
+Plotting spectral laws 
 =======================
 
 In this section, we will briefly explain what is the spectral distribution
 of a random matrix and how to plot it in order to study its properties.
 Most ensembles spectral distribution are explained through spectral laws,
 that are going to be detailed as well. 
 
@@ -102,15 +102,15 @@
 # to a semicircle. Thats because Gaussian Ensemble random matrices spectrum
 # follow *Wigner's Semicircle Law*. In the second example, the shown density
 # has a very particular shape too, it is known as the *Marchenko-Pastur Law*.
 # But, what is a spectral law?
 
 ##############################################################################
 # Spectral laws
-# ------------------------------
+# --------------------------
 # 
 # Spectral laws define random matrix eigenvalue distribution when its size
 # goes to infinity. So the spectral laws describes the limiting behavior
 # of the spectrum of a random matrix ensemble.
 #
 # The most known spectral laws, and implemented by scikit-rmt, are the
 # following:
@@ -127,79 +127,79 @@
 ##############################################################################
 # Anyone can forget about the specific plotting details and directly study
 # those laws by using the functions provided in scikit-rmt.
 
 ##############################################################################
 # We can easily analyze **Wigner's Semicircle Law** as follows.
 
-from skrmt.ensemble import wigner_semicircular_law
+from skrmt.ensemble import wigner_semicircle
 
-wigner_semicircular_law(ensemble='goe', n_size=2000, bins=80)
+wigner_semicircle(ensemble='goe', n_size=2000, bins=80)
 
 ##############################################################################
 # We can also study **Marchenko-Pastur Law** as by:
 
-from skrmt.ensemble import marchenko_pastur_law
+from skrmt.ensemble import marchenko_pastur
 
-marchenko_pastur_law(ensemble='wre', p_size=2000, n_size=6000, bins=80)
+marchenko_pastur(ensemble='wre', p_size=2000, n_size=6000, bins=80)
 
 ##############################################################################
 # Finally, **Tracy-Widom Law** can be represented using:
 
-from skrmt.ensemble import tracy_widom_law
+from skrmt.ensemble import tracy_widom
 
-tracy_widom_law(ensemble='goe', n_size=100, times=10000, bins=80)
+tracy_widom(ensemble='goe', n_size=100, times=10000, bins=80)
 
 ##############################################################################
-# Spectral Laws analytical expression
+# Spectral laws analytical expression
 # -----------------------------------
 # 
 # The spectral laws described so far have been proven to converge to certain
 # analytical functions that defines the limiting behaviour of the eigenvalue
 # distribution of the random matrices. The functions of scikit-rmt that are
 # capable of plotting the spectral laws also support the representation of the
 # theoretical eigenvalue pdf.
 
 ##############################################################################
 # The analytical probability function for the Gaussian Ensemble, known as
 # Wigner Semicircle Law, supported on :math:`[-R, R]` and centered at :math:`(0,0)`
 # is :math:`f(x) = \frac{2}{\pi R^2} \sqrt{R^2 - x^2}`.
 
-from skrmt.ensemble import wigner_semicircular_law
+from skrmt.ensemble import wigner_semicircle
 
-wigner_semicircular_law(ensemble='goe', n_size=2000, bins=80, density=True, limit_pdf=True)
+wigner_semicircle(ensemble='goe', n_size=2000, bins=80, density=True, plot_law_pdf=True)
 
 ##############################################################################
 # The analytical probability function for the Wishart Ensemble known as
 # Marchenko-Pastur Law with parameter :math:`\lambda = p/n \in (0,1]` is
 # :math:`f_{\lambda}(x) = \frac{1}{2\pi \sigma^2}\frac{\sqrt{(\lambda_+ - x)(x - \lambda_-)}}{\lambda x}`,
 # where :math:`\lambda_{\pm} = \sigma^2 (1 \pm \sqrt{\lambda})^2`. 
 # If :math:`\lambda > 1` then the limiting distribution has an additional
 # mass probability point in the origin of size :math:`1 - \frac{1}{\lambda}`.
 
-from skrmt.ensemble import marchenko_pastur_law
+from skrmt.ensemble import marchenko_pastur
 
-marchenko_pastur_law(ensemble='wre', p_size=2000, n_size=6000, bins=80, density=True, limit_pdf=True)
+marchenko_pastur(ensemble='wre', p_size=2000, n_size=6000, bins=80, density=True, plot_law_pdf=True)
 
 ##############################################################################
 # In the other hand, the Tracy-Widom Law has a complex analytical expression,
 # that is the solution of a particular non-linear differential equation, described
 # in detail in:
 # S. Bauman. "The Tracy-Widom Distribution and its Application to Statistical Physics".
 # MIT Department of Physics. 2017.
 # The package scikit-rmt represents a precise
 # approximation of the theoretical Tracy-Widom pdf.
 
-from skrmt.ensemble import tracy_widom_law
+from skrmt.ensemble import tracy_widom
 
-tracy_widom_law(ensemble='goe', n_size=10, times=5000, bins=80, density=True, limit_pdf=True)
+tracy_widom(ensemble='goe', n_size=10, times=5000, bins=80, density=True, plot_law_pdf=True)
 
 ##############################################################################
 # Finally, the limiting distribution of the Manova Ensemble is not described
 # by any famous Law, but its expression has been determined. This library
 # provides functionality to show it on top of the empirical histogram of the
 # eigenvalue spectrum.
 
-from skrmt.ensemble import manova_spectrum_distr
+from skrmt.ensemble import manova_spectrum
 
-manova_spectrum_distr(ensemble='mre', m_size=1000, n1_size=3000, n2_size=3000,
-                      bins=80, density=True, limit_pdf=True)
+manova_spectrum(ensemble='mre', m_size=1000, n1_size=3000, n2_size=3000,
+                bins=80, density=True, plot_law_pdf=True)
```

