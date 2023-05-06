# Comparing `tmp/featurebox-0.0.9999.tar.gz` & `tmp/featurebox-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "featurebox-0.0.9999.tar", last modified: Wed Apr 26 13:47:46 2023, max compression
+gzip compressed data, was "featurebox-0.1.1.tar", last modified: Sat May  6 09:11:45 2023, max compression
```

## Comparing `featurebox-0.0.9999.tar` & `featurebox-0.1.1.tar`

### file list

```diff
@@ -1,102 +1,102 @@
-drwxrwxrwx   0        0        0        0 2023-04-26 13:47:46.031925 featurebox-0.0.9999/
--rw-rw-rw-   0        0        0     7797 2021-12-17 11:27:06.000000 featurebox-0.0.9999/LICENSE
--rw-rw-rw-   0        0        0      129 2021-12-17 11:27:06.000000 featurebox-0.0.9999/MANIFEST.in
--rw-rw-rw-   0        0        0     2553 2023-04-26 13:47:46.031925 featurebox-0.0.9999/PKG-INFO
--rw-rw-rw-   0        0        0     1372 2022-01-04 11:52:43.000000 featurebox-0.0.9999/README.md
-drwxrwxrwx   0        0        0        0 2023-04-26 13:47:45.961898 featurebox-0.0.9999/featurebox/
--rw-rw-rw-   0        0        0       64 2022-08-08 06:09:08.000000 featurebox-0.0.9999/featurebox/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-26 13:47:45.977716 featurebox-0.0.9999/featurebox/cli/
--rw-rw-rw-   0        0        0      747 2022-10-15 08:34:40.000000 featurebox-0.0.9999/featurebox/cli/__init__.py
--rw-rw-rw-   0        0        0    13414 2023-02-17 07:06:06.000000 featurebox-0.0.9999/featurebox/cli/_basepathout.py
--rw-rw-rw-   0        0        0     6745 2023-02-22 15:08:51.000000 featurebox-0.0.9999/featurebox/cli/main.py
--rw-rw-rw-   0        0        0      320 2022-10-15 08:34:40.000000 featurebox-0.0.9999/featurebox/cli/template.py
--rw-rw-rw-   0        0        0    10232 2022-11-25 11:15:33.000000 featurebox-0.0.9999/featurebox/cli/vasp_bader.py
--rw-rw-rw-   0        0        0    11807 2022-11-25 11:15:33.000000 featurebox-0.0.9999/featurebox/cli/vasp_bgp.py
--rw-rw-rw-   0        0        0      913 2022-08-06 15:06:02.000000 featurebox-0.0.9999/featurebox/cli/vasp_chg_diff.py
--rw-rw-rw-   0        0        0    10397 2022-10-15 08:46:16.000000 featurebox-0.0.9999/featurebox/cli/vasp_cohp.py
--rw-rw-rw-   0        0        0     5435 2023-02-21 09:35:25.000000 featurebox-0.0.9999/featurebox/cli/vasp_converge.py
--rw-rw-rw-   0        0        0    37796 2022-11-25 11:15:33.000000 featurebox-0.0.9999/featurebox/cli/vasp_dbc.py
--rw-rw-rw-   0        0        0    25116 2022-08-12 08:59:00.000000 featurebox-0.0.9999/featurebox/cli/vasp_dos.py
--rw-rw-rw-   0        0        0     4942 2023-02-17 07:12:55.000000 featurebox-0.0.9999/featurebox/cli/vasp_empty.py
--rw-rw-rw-   0        0        0     7019 2023-02-21 09:34:22.000000 featurebox-0.0.9999/featurebox/cli/vasp_general_diff.py
--rw-rw-rw-   0        0        0     7809 2023-02-19 16:30:44.000000 featurebox-0.0.9999/featurebox/cli/vasp_general_single.py
-drwxrwxrwx   0        0        0        0 2023-04-26 13:47:45.987716 featurebox-0.0.9999/featurebox/data/
--rw-rw-rw-   0        0        0      167 2022-08-01 08:22:20.000000 featurebox-0.0.9999/featurebox/data/__init__.py
--rw-rw-rw-   0        0        0     6491 2022-11-25 11:15:33.000000 featurebox-0.0.9999/featurebox/data/check_data.py
--rw-rw-rw-   0        0        0    10393 2022-10-15 08:47:37.000000 featurebox-0.0.9999/featurebox/data/data_sep.py
--rw-rw-rw-   0        0        0    38626 2021-12-27 15:28:19.000000 featurebox-0.0.9999/featurebox/data/ele_megnet.json
--rw-rw-rw-   0        0        0    37806 2021-12-27 15:28:19.000000 featurebox-0.0.9999/featurebox/data/ele_table.csv
--rw-rw-rw-   0        0        0    47340 2021-12-27 15:28:19.000000 featurebox-0.0.9999/featurebox/data/ele_table_norm.csv
--rw-rw-rw-   0        0        0     2917 2021-12-17 11:27:06.000000 featurebox-0.0.9999/featurebox/data/ie.json
--rw-rw-rw-   0        0        0     6763 2022-10-15 08:50:02.000000 featurebox-0.0.9999/featurebox/data/mp_access.py
--rw-rw-rw-   0        0        0     8745 2023-02-19 10:31:47.000000 featurebox-0.0.9999/featurebox/data/name_split.py
--rw-rw-rw-   0        0        0      476 2023-02-05 08:28:56.000000 featurebox-0.0.9999/featurebox/data/namesplit.py
--rw-rw-rw-   0        0        0     7822 2021-12-17 11:27:06.000000 featurebox-0.0.9999/featurebox/data/oe.csv
-drwxrwxrwx   0        0        0        0 2023-04-26 13:47:45.990716 featurebox-0.0.9999/featurebox/featurizers/
--rw-rw-rw-   0        0        0       84 2022-10-12 08:15:47.000000 featurebox-0.0.9999/featurebox/featurizers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-26 13:47:45.992716 featurebox-0.0.9999/featurebox/featurizers/atom/
--rw-rw-rw-   0        0        0       22 2021-12-17 11:27:06.000000 featurebox-0.0.9999/featurebox/featurizers/atom/__init__.py
--rw-rw-rw-   0        0        0    27629 2022-10-15 09:31:37.000000 featurebox-0.0.9999/featurebox/featurizers/atom/mapper.py
--rw-rw-rw-   0        0        0    17825 2022-12-07 05:24:08.000000 featurebox-0.0.9999/featurebox/featurizers/base_feature.py
--rw-rw-rw-   0        0        0     4086 2022-08-12 09:00:19.000000 featurebox-0.0.9999/featurebox/featurizers/batch_feature.py
-drwxrwxrwx   0        0        0        0 2023-04-26 13:47:45.997677 featurebox-0.0.9999/featurebox/featurizers/envir/
--rw-rw-rw-   0        0        0      145 2021-12-17 11:27:06.000000 featurebox-0.0.9999/featurebox/featurizers/envir/__init__.py
--rw-rw-rw-   0        0        0     3078 2022-11-25 11:15:33.000000 featurebox-0.0.9999/featurebox/featurizers/envir/_get_radius_in_spheres.py
--rw-rw-rw-   0        0        0     6732 2022-12-07 05:24:08.000000 featurebox-0.0.9999/featurebox/featurizers/envir/_get_xyz_in_spheres.py
--rw-rw-rw-   0        0        0     2861 2022-11-04 08:32:06.000000 featurebox-0.0.9999/featurebox/featurizers/envir/desc_env.py
-drwxrwxrwx   0        0        0        0 2023-04-26 13:47:46.010625 featurebox-0.0.9999/featurebox/featurizers/envir/descriptors/
--rw-rw-rw-   0        0        0    46046 2022-10-15 09:17:09.000000 featurebox-0.0.9999/featurebox/featurizers/envir/descriptors/ACSF.py
--rw-rw-rw-   0        0        0    17182 2022-12-07 05:24:08.000000 featurebox-0.0.9999/featurebox/featurizers/envir/descriptors/EAD.py
--rw-rw-rw-   0        0        0    16250 2021-12-17 11:27:06.000000 featurebox-0.0.9999/featurebox/featurizers/envir/descriptors/EAMD.py
--rw-rw-rw-   0        0        0    45331 2022-10-15 09:17:09.000000 featurebox-0.0.9999/featurebox/featurizers/envir/descriptors/SO3.py
--rw-rw-rw-   0        0        0    62762 2021-12-17 11:27:06.000000 featurebox-0.0.9999/featurebox/featurizers/envir/descriptors/SO4.py
--rw-rw-rw-   0        0        0    33591 2022-10-15 09:31:37.000000 featurebox-0.0.9999/featurebox/featurizers/envir/descriptors/SOAP.py
--rw-rw-rw-   0        0        0      271 2022-10-12 08:15:47.000000 featurebox-0.0.9999/featurebox/featurizers/envir/descriptors/__init__.py
--rw-rw-rw-   0        0        0      904 2021-12-17 11:27:06.000000 featurebox-0.0.9999/featurebox/featurizers/envir/descriptors/_generate_coefs.py
--rw-rw-rw-   0        0        0    16420 2021-12-17 11:27:06.000000 featurebox-0.0.9999/featurebox/featurizers/envir/descriptors/angular_momentum.py
--rw-rw-rw-   0        0        0    43536 2022-10-15 09:17:09.000000 featurebox-0.0.9999/featurebox/featurizers/envir/descriptors/behlerparrinello.py
--rw-rw-rw-   0        0        0    50664 2021-12-17 11:27:06.000000 featurebox-0.0.9999/featurebox/featurizers/envir/descriptors/bispectrum.py
--rw-rw-rw-   0        0        0     4877 2021-12-17 11:27:06.000000 featurebox-0.0.9999/featurebox/featurizers/envir/descriptors/cutoff.py
--rw-rw-rw-   0        0        0     9684 2022-10-15 09:17:09.000000 featurebox-0.0.9999/featurebox/featurizers/envir/descriptors/lbispectrum.py
--rw-rw-rw-   0        0        0      999 2021-12-17 11:27:06.000000 featurebox-0.0.9999/featurebox/featurizers/envir/descriptors/utils.py
--rw-rw-rw-   0        0        0    34379 2022-10-15 09:31:37.000000 featurebox-0.0.9999/featurebox/featurizers/envir/descriptors/wACSF.py
--rw-rw-rw-   0        0        0    16373 2022-11-04 08:32:06.000000 featurebox-0.0.9999/featurebox/featurizers/envir/environment.py
--rw-rw-rw-   0        0        0     7980 2022-10-15 09:31:37.000000 featurebox-0.0.9999/featurebox/featurizers/envir/local_env.py
-drwxrwxrwx   0        0        0        0 2023-04-26 13:47:46.014369 featurebox-0.0.9999/featurebox/featurizers/state/
--rw-rw-rw-   0        0        0       65 2022-10-15 09:31:37.000000 featurebox-0.0.9999/featurebox/featurizers/state/__init__.py
--rw-rw-rw-   0        0        0    12441 2022-10-15 09:31:37.000000 featurebox-0.0.9999/featurebox/featurizers/state/extrastats.py
--rw-rw-rw-   0        0        0      954 2021-12-17 11:27:06.000000 featurebox-0.0.9999/featurebox/featurizers/state/state_mapper.py
--rw-rw-rw-   0        0        0    10989 2022-10-20 14:50:35.000000 featurebox-0.0.9999/featurebox/featurizers/state/statistics.py
--rw-rw-rw-   0        0        0     8329 2022-03-06 10:25:09.000000 featurebox-0.0.9999/featurebox/featurizers/state/union.py
-drwxrwxrwx   0        0        0        0 2023-04-26 13:47:46.021371 featurebox-0.0.9999/featurebox/pbs/
--rw-rw-rw-   0        0        0      157 2023-02-19 17:25:28.000000 featurebox-0.0.9999/featurebox/pbs/__init__.py
--rw-rw-rw-   0        0        0     3519 2023-02-10 07:49:23.000000 featurebox-0.0.9999/featurebox/pbs/cli.py
--rw-rw-rw-   0        0        0     1683 2023-02-19 17:25:28.000000 featurebox-0.0.9999/featurebox/pbs/jmk.py
--rw-rw-rw-   0        0        0    10498 2023-02-19 17:25:28.000000 featurebox-0.0.9999/featurebox/pbs/job_manager.py
--rw-rw-rw-   0        0        0     4877 2022-12-07 01:59:25.000000 featurebox-0.0.9999/featurebox/pbs/misc.py
--rw-rw-rw-   0        0        0    12164 2023-02-22 04:00:03.000000 featurebox-0.0.9999/featurebox/pbs/misc_slurm.py
--rw-rw-rw-   0        0        0     7827 2023-02-18 07:12:20.000000 featurebox-0.0.9999/featurebox/pbs/misc_torque.py
--rw-rw-rw-   0        0        0     9286 2023-02-19 18:13:40.000000 featurebox-0.0.9999/featurebox/pbs/misc_unischeduler.py
--rw-rw-rw-   0        0        0     2922 2023-02-19 16:42:40.000000 featurebox-0.0.9999/featurebox/pbs/pbs_conf.py
-drwxrwxrwx   0        0        0        0 2023-04-26 13:47:46.027371 featurebox-0.0.9999/featurebox/selection/
--rw-rw-rw-   0        0        0       68 2022-08-24 14:23:26.000000 featurebox-0.0.9999/featurebox/selection/__init__.py
--rw-rw-rw-   0        0        0    26778 2023-04-26 10:02:44.000000 featurebox-0.0.9999/featurebox/selection/backforward.py
--rw-rw-rw-   0        0        0     9201 2023-04-26 10:03:21.000000 featurebox-0.0.9999/featurebox/selection/corr.py
--rw-rw-rw-   0        0        0    12564 2023-04-26 09:52:37.000000 featurebox-0.0.9999/featurebox/selection/exhaustion.py
--rw-rw-rw-   0        0        0    15219 2023-04-26 10:46:56.000000 featurebox-0.0.9999/featurebox/selection/ga.py
--rw-rw-rw-   0        0        0     6230 2023-04-25 13:59:08.000000 featurebox-0.0.9999/featurebox/selection/multibase.py
-drwxrwxrwx   0        0        0        0 2023-04-26 13:47:46.030919 featurebox-0.0.9999/featurebox/utils/
--rw-rw-rw-   0        0        0       48 2022-10-15 09:08:29.000000 featurebox-0.0.9999/featurebox/utils/__init__.py
--rw-rw-rw-   0        0        0       95 2022-01-04 13:19:58.000000 featurebox-0.0.9999/featurebox/utils/general.py
--rw-rw-rw-   0        0        0      221 2022-11-25 11:15:33.000000 featurebox-0.0.9999/featurebox/utils/predefined_typing.py
--rw-rw-rw-   0        0        0    19519 2022-11-25 11:15:33.000000 featurebox-0.0.9999/featurebox/utils/quickmethod.py
-drwxrwxrwx   0        0        0        0 2023-04-26 13:47:45.966716 featurebox-0.0.9999/featurebox.egg-info/
--rw-rw-rw-   0        0        0     2553 2023-04-26 13:47:45.000000 featurebox-0.0.9999/featurebox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3047 2023-04-26 13:47:45.000000 featurebox-0.0.9999/featurebox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-26 13:47:45.000000 featurebox-0.0.9999/featurebox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      146 2023-04-26 13:47:45.000000 featurebox-0.0.9999/featurebox.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      130 2023-04-26 13:47:45.000000 featurebox-0.0.9999/featurebox.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-26 13:47:45.000000 featurebox-0.0.9999/featurebox.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      245 2022-08-01 10:04:12.000000 featurebox-0.0.9999/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-04-26 13:47:46.031925 featurebox-0.0.9999/setup.cfg
--rw-rw-rw-   0        0        0     2534 2023-04-26 13:47:25.000000 featurebox-0.0.9999/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-06 09:11:45.176034 featurebox-0.1.1/
+-rw-rw-rw-   0        0        0     7797 2021-12-17 11:27:06.000000 featurebox-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      129 2021-12-17 11:27:06.000000 featurebox-0.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2528 2023-05-06 09:11:45.175034 featurebox-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1372 2022-01-04 11:52:43.000000 featurebox-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-06 09:11:45.092965 featurebox-0.1.1/featurebox/
+-rw-rw-rw-   0        0        0       64 2022-08-08 06:09:08.000000 featurebox-0.1.1/featurebox/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 09:11:45.111463 featurebox-0.1.1/featurebox/cli/
+-rw-rw-rw-   0        0        0      747 2022-10-15 08:34:40.000000 featurebox-0.1.1/featurebox/cli/__init__.py
+-rw-rw-rw-   0        0        0    13414 2023-02-17 07:06:06.000000 featurebox-0.1.1/featurebox/cli/_basepathout.py
+-rw-rw-rw-   0        0        0     6741 2023-04-27 07:41:40.000000 featurebox-0.1.1/featurebox/cli/main.py
+-rw-rw-rw-   0        0        0      320 2022-10-15 08:34:40.000000 featurebox-0.1.1/featurebox/cli/template.py
+-rw-rw-rw-   0        0        0    10232 2022-11-25 11:15:33.000000 featurebox-0.1.1/featurebox/cli/vasp_bader.py
+-rw-rw-rw-   0        0        0    11807 2022-11-25 11:15:33.000000 featurebox-0.1.1/featurebox/cli/vasp_bgp.py
+-rw-rw-rw-   0        0        0      913 2022-08-06 15:06:02.000000 featurebox-0.1.1/featurebox/cli/vasp_chg_diff.py
+-rw-rw-rw-   0        0        0    10397 2022-10-15 08:46:16.000000 featurebox-0.1.1/featurebox/cli/vasp_cohp.py
+-rw-rw-rw-   0        0        0     5435 2023-02-21 09:35:25.000000 featurebox-0.1.1/featurebox/cli/vasp_converge.py
+-rw-rw-rw-   0        0        0    37796 2022-11-25 11:15:33.000000 featurebox-0.1.1/featurebox/cli/vasp_dbc.py
+-rw-rw-rw-   0        0        0    25116 2022-08-12 08:59:00.000000 featurebox-0.1.1/featurebox/cli/vasp_dos.py
+-rw-rw-rw-   0        0        0     4942 2023-02-17 07:12:55.000000 featurebox-0.1.1/featurebox/cli/vasp_empty.py
+-rw-rw-rw-   0        0        0     7019 2023-02-21 09:34:22.000000 featurebox-0.1.1/featurebox/cli/vasp_general_diff.py
+-rw-rw-rw-   0        0        0     7808 2023-04-27 07:41:40.000000 featurebox-0.1.1/featurebox/cli/vasp_general_single.py
+drwxrwxrwx   0        0        0        0 2023-05-06 09:11:45.121922 featurebox-0.1.1/featurebox/data/
+-rw-rw-rw-   0        0        0      167 2022-08-01 08:22:20.000000 featurebox-0.1.1/featurebox/data/__init__.py
+-rw-rw-rw-   0        0        0     6491 2022-11-25 11:15:33.000000 featurebox-0.1.1/featurebox/data/check_data.py
+-rw-rw-rw-   0        0        0    10393 2022-10-15 08:47:37.000000 featurebox-0.1.1/featurebox/data/data_sep.py
+-rw-rw-rw-   0        0        0    38626 2021-12-27 15:28:19.000000 featurebox-0.1.1/featurebox/data/ele_megnet.json
+-rw-rw-rw-   0        0        0    37806 2021-12-27 15:28:19.000000 featurebox-0.1.1/featurebox/data/ele_table.csv
+-rw-rw-rw-   0        0        0    47340 2021-12-27 15:28:19.000000 featurebox-0.1.1/featurebox/data/ele_table_norm.csv
+-rw-rw-rw-   0        0        0     2917 2021-12-17 11:27:06.000000 featurebox-0.1.1/featurebox/data/ie.json
+-rw-rw-rw-   0        0        0     6763 2022-10-15 08:50:02.000000 featurebox-0.1.1/featurebox/data/mp_access.py
+-rw-rw-rw-   0        0        0     8747 2023-04-27 07:41:40.000000 featurebox-0.1.1/featurebox/data/name_split.py
+-rw-rw-rw-   0        0        0      329 2023-05-06 09:04:31.000000 featurebox-0.1.1/featurebox/data/namesplit.py
+-rw-rw-rw-   0        0        0     7822 2021-12-17 11:27:06.000000 featurebox-0.1.1/featurebox/data/oe.csv
+drwxrwxrwx   0        0        0        0 2023-05-06 09:11:45.124915 featurebox-0.1.1/featurebox/featurizers/
+-rw-rw-rw-   0        0        0       84 2022-10-12 08:15:47.000000 featurebox-0.1.1/featurebox/featurizers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 09:11:45.126970 featurebox-0.1.1/featurebox/featurizers/atom/
+-rw-rw-rw-   0        0        0       22 2021-12-17 11:27:06.000000 featurebox-0.1.1/featurebox/featurizers/atom/__init__.py
+-rw-rw-rw-   0        0        0    28473 2023-04-27 07:41:40.000000 featurebox-0.1.1/featurebox/featurizers/atom/mapper.py
+-rw-rw-rw-   0        0        0    18644 2023-04-27 07:41:46.000000 featurebox-0.1.1/featurebox/featurizers/base_feature.py
+-rw-rw-rw-   0        0        0     4086 2022-08-12 09:00:19.000000 featurebox-0.1.1/featurebox/featurizers/batch_feature.py
+drwxrwxrwx   0        0        0        0 2023-05-06 09:11:45.133915 featurebox-0.1.1/featurebox/featurizers/envir/
+-rw-rw-rw-   0        0        0      145 2021-12-17 11:27:06.000000 featurebox-0.1.1/featurebox/featurizers/envir/__init__.py
+-rw-rw-rw-   0        0        0     3075 2023-04-27 07:41:46.000000 featurebox-0.1.1/featurebox/featurizers/envir/_get_radius_in_spheres.py
+-rw-rw-rw-   0        0        0     6732 2023-04-27 07:41:40.000000 featurebox-0.1.1/featurebox/featurizers/envir/_get_xyz_in_spheres.py
+-rw-rw-rw-   0        0        0     2861 2022-11-04 08:32:06.000000 featurebox-0.1.1/featurebox/featurizers/envir/desc_env.py
+drwxrwxrwx   0        0        0        0 2023-05-06 09:11:45.150915 featurebox-0.1.1/featurebox/featurizers/envir/descriptors/
+-rw-rw-rw-   0        0        0    46046 2022-10-15 09:17:09.000000 featurebox-0.1.1/featurebox/featurizers/envir/descriptors/ACSF.py
+-rw-rw-rw-   0        0        0    17184 2023-04-27 07:41:40.000000 featurebox-0.1.1/featurebox/featurizers/envir/descriptors/EAD.py
+-rw-rw-rw-   0        0        0    16250 2021-12-17 11:27:06.000000 featurebox-0.1.1/featurebox/featurizers/envir/descriptors/EAMD.py
+-rw-rw-rw-   0        0        0    45331 2022-10-15 09:17:09.000000 featurebox-0.1.1/featurebox/featurizers/envir/descriptors/SO3.py
+-rw-rw-rw-   0        0        0    62762 2021-12-17 11:27:06.000000 featurebox-0.1.1/featurebox/featurizers/envir/descriptors/SO4.py
+-rw-rw-rw-   0        0        0    33591 2022-10-15 09:31:37.000000 featurebox-0.1.1/featurebox/featurizers/envir/descriptors/SOAP.py
+-rw-rw-rw-   0        0        0      271 2022-10-12 08:15:47.000000 featurebox-0.1.1/featurebox/featurizers/envir/descriptors/__init__.py
+-rw-rw-rw-   0        0        0      904 2021-12-17 11:27:06.000000 featurebox-0.1.1/featurebox/featurizers/envir/descriptors/_generate_coefs.py
+-rw-rw-rw-   0        0        0    16420 2021-12-17 11:27:06.000000 featurebox-0.1.1/featurebox/featurizers/envir/descriptors/angular_momentum.py
+-rw-rw-rw-   0        0        0    43536 2022-10-15 09:17:09.000000 featurebox-0.1.1/featurebox/featurizers/envir/descriptors/behlerparrinello.py
+-rw-rw-rw-   0        0        0    50664 2021-12-17 11:27:06.000000 featurebox-0.1.1/featurebox/featurizers/envir/descriptors/bispectrum.py
+-rw-rw-rw-   0        0        0     4877 2021-12-17 11:27:06.000000 featurebox-0.1.1/featurebox/featurizers/envir/descriptors/cutoff.py
+-rw-rw-rw-   0        0        0     9684 2022-10-15 09:17:09.000000 featurebox-0.1.1/featurebox/featurizers/envir/descriptors/lbispectrum.py
+-rw-rw-rw-   0        0        0      999 2021-12-17 11:27:06.000000 featurebox-0.1.1/featurebox/featurizers/envir/descriptors/utils.py
+-rw-rw-rw-   0        0        0    34379 2022-10-15 09:31:37.000000 featurebox-0.1.1/featurebox/featurizers/envir/descriptors/wACSF.py
+-rw-rw-rw-   0        0        0    16373 2022-11-04 08:32:06.000000 featurebox-0.1.1/featurebox/featurizers/envir/environment.py
+-rw-rw-rw-   0        0        0     7974 2023-04-27 07:41:40.000000 featurebox-0.1.1/featurebox/featurizers/envir/local_env.py
+drwxrwxrwx   0        0        0        0 2023-05-06 09:11:45.156034 featurebox-0.1.1/featurebox/featurizers/state/
+-rw-rw-rw-   0        0        0       65 2022-10-15 09:31:37.000000 featurebox-0.1.1/featurebox/featurizers/state/__init__.py
+-rw-rw-rw-   0        0        0    12441 2022-10-15 09:31:37.000000 featurebox-0.1.1/featurebox/featurizers/state/extrastats.py
+-rw-rw-rw-   0        0        0      954 2021-12-17 11:27:06.000000 featurebox-0.1.1/featurebox/featurizers/state/state_mapper.py
+-rw-rw-rw-   0        0        0    11838 2023-05-06 09:05:28.000000 featurebox-0.1.1/featurebox/featurizers/state/statistics.py
+-rw-rw-rw-   0        0        0     8888 2023-04-27 07:41:46.000000 featurebox-0.1.1/featurebox/featurizers/state/union.py
+drwxrwxrwx   0        0        0        0 2023-05-06 09:11:45.164034 featurebox-0.1.1/featurebox/pbs/
+-rw-rw-rw-   0        0        0      159 2023-04-27 07:41:40.000000 featurebox-0.1.1/featurebox/pbs/__init__.py
+-rw-rw-rw-   0        0        0     3519 2023-02-10 07:49:23.000000 featurebox-0.1.1/featurebox/pbs/cli.py
+-rw-rw-rw-   0        0        0     1683 2023-02-19 17:25:28.000000 featurebox-0.1.1/featurebox/pbs/jmk.py
+-rw-rw-rw-   0        0        0    10503 2023-04-27 07:41:40.000000 featurebox-0.1.1/featurebox/pbs/job_manager.py
+-rw-rw-rw-   0        0        0     4877 2022-12-07 01:59:25.000000 featurebox-0.1.1/featurebox/pbs/misc.py
+-rw-rw-rw-   0        0        0    12164 2023-04-27 07:41:40.000000 featurebox-0.1.1/featurebox/pbs/misc_slurm.py
+-rw-rw-rw-   0        0        0     7827 2023-02-18 07:12:20.000000 featurebox-0.1.1/featurebox/pbs/misc_torque.py
+-rw-rw-rw-   0        0        0     9288 2023-04-27 07:41:40.000000 featurebox-0.1.1/featurebox/pbs/misc_unischeduler.py
+-rw-rw-rw-   0        0        0     2920 2023-04-27 07:41:40.000000 featurebox-0.1.1/featurebox/pbs/pbs_conf.py
+drwxrwxrwx   0        0        0        0 2023-05-06 09:11:45.170034 featurebox-0.1.1/featurebox/selection/
+-rw-rw-rw-   0        0        0       68 2022-08-24 14:23:26.000000 featurebox-0.1.1/featurebox/selection/__init__.py
+-rw-rw-rw-   0        0        0    27074 2023-05-06 08:40:25.000000 featurebox-0.1.1/featurebox/selection/backforward.py
+-rw-rw-rw-   0        0        0     9218 2023-04-27 07:41:40.000000 featurebox-0.1.1/featurebox/selection/corr.py
+-rw-rw-rw-   0        0        0    12878 2023-05-06 09:04:31.000000 featurebox-0.1.1/featurebox/selection/exhaustion.py
+-rw-rw-rw-   0        0        0    15436 2023-05-06 08:26:57.000000 featurebox-0.1.1/featurebox/selection/ga.py
+-rw-rw-rw-   0        0        0     6230 2023-04-25 13:59:08.000000 featurebox-0.1.1/featurebox/selection/multibase.py
+drwxrwxrwx   0        0        0        0 2023-05-06 09:11:45.174034 featurebox-0.1.1/featurebox/utils/
+-rw-rw-rw-   0        0        0       48 2022-10-15 09:08:29.000000 featurebox-0.1.1/featurebox/utils/__init__.py
+-rw-rw-rw-   0        0        0       95 2022-01-04 13:19:58.000000 featurebox-0.1.1/featurebox/utils/general.py
+-rw-rw-rw-   0        0        0      221 2022-11-25 11:15:33.000000 featurebox-0.1.1/featurebox/utils/predefined_typing.py
+-rw-rw-rw-   0        0        0    19470 2023-05-06 09:04:31.000000 featurebox-0.1.1/featurebox/utils/quickmethod.py
+drwxrwxrwx   0        0        0        0 2023-05-06 09:11:45.097970 featurebox-0.1.1/featurebox.egg-info/
+-rw-rw-rw-   0        0        0     2528 2023-05-06 09:11:44.000000 featurebox-0.1.1/featurebox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3047 2023-05-06 09:11:45.000000 featurebox-0.1.1/featurebox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 09:11:44.000000 featurebox-0.1.1/featurebox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      146 2023-05-06 09:11:44.000000 featurebox-0.1.1/featurebox.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      130 2023-05-06 09:11:44.000000 featurebox-0.1.1/featurebox.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-06 09:11:44.000000 featurebox-0.1.1/featurebox.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      237 2023-05-06 09:01:10.000000 featurebox-0.1.1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-05-06 09:11:45.176034 featurebox-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     2532 2023-05-06 08:58:47.000000 featurebox-0.1.1/setup.py
```

### Comparing `featurebox-0.0.9999/LICENSE` & `featurebox-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `featurebox-0.0.9999/PKG-INFO` & `featurebox-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: featurebox
-Version: 0.0.9999
+Version: 0.1.1
 Summary: This is an box contains tools for machine learning.Some of code are non-originality, just copy for use. All the referenced code are marked,details can be shown in their sources
 Home-page: https://github.com/boliqq07/featurebox
 Author: wangchangxin
 Author-email: 986798607@qq.com
 Maintainer: wangchangxin
-License: UNKNOWN
 Keywords: features,combination,selection
 Platform: Windows
 Platform: Unix
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
@@ -70,9 +69,7 @@
 
 Support
 ----------------------
 [![Jetbrains](jetbrains.svg)](https://jb.gg/OpenSource)
 
 
 
-
-
```

### Comparing `featurebox-0.0.9999/README.md` & `featurebox-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `featurebox-0.0.9999/featurebox/cli/__init__.py` & `featurebox-0.1.1/featurebox/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `featurebox-0.0.9999/featurebox/cli/_basepathout.py` & `featurebox-0.1.1/featurebox/cli/_basepathout.py`

 * *Files identical despite different names*

### Comparing `featurebox-0.0.9999/featurebox/cli/main.py` & `featurebox-0.1.1/featurebox/cli/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,21 +38,21 @@
     'cohp': ('featurebox.cli.vasp_cohp',
              "fbx cohp    : Batching 'COHP'."),
     'dos': ('featurebox.cli.vasp_dos',
             "fbx dos     : Batching 'Density of States'."),
     'general': ('featurebox.cli.vasp_general_single',
                 "fbx general : Batching 'Vasprun.xml property'."),
     'energy': ('featurebox.cli.vasp_general_single',
-                "fbx energy  : Batching 'free energy property'."),
+               "fbx energy  : Batching 'free energy property'."),
     'diff': ('featurebox.cli.vasp_general_diff',
              "fbx diff    : Batching 'Energy difference'."),
     'converge': ('featurebox.cli.vasp_converge',
                  "fbx converge: Batching 'Check vasp converge'."),
     'empty': ('featurebox.cli.vasp_empty',
-                 "fbx empty   : Batching 'Check vasp CONTCAR'."),
+              "fbx empty   : Batching 'Check vasp CONTCAR'."),
 
 }
 
 cmd_help = """-----------------------------------------------------
 Sub-Command : Function
 ------------ ----------------------------------------
 {}
```

### Comparing `featurebox-0.0.9999/featurebox/cli/vasp_bader.py` & `featurebox-0.1.1/featurebox/cli/vasp_bader.py`

 * *Files identical despite different names*

### Comparing `featurebox-0.0.9999/featurebox/cli/vasp_bgp.py` & `featurebox-0.1.1/featurebox/cli/vasp_bgp.py`

 * *Files identical despite different names*

### Comparing `featurebox-0.0.9999/featurebox/cli/vasp_chg_diff.py` & `featurebox-0.1.1/featurebox/cli/vasp_chg_diff.py`

 * *Files identical despite different names*

### Comparing `featurebox-0.0.9999/featurebox/cli/vasp_cohp.py` & `featurebox-0.1.1/featurebox/cli/vasp_cohp.py`

 * *Files identical despite different names*

### Comparing `featurebox-0.0.9999/featurebox/cli/vasp_converge.py` & `featurebox-0.1.1/featurebox/cli/vasp_converge.py`

 * *Files identical despite different names*

### Comparing `featurebox-0.0.9999/featurebox/cli/vasp_dbc.py` & `featurebox-0.1.1/featurebox/cli/vasp_dbc.py`

 * *Files identical despite different names*

### Comparing `featurebox-0.0.9999/featurebox/cli/vasp_dos.py` & `featurebox-0.1.1/featurebox/cli/vasp_dos.py`

 * *Files identical despite different names*

### Comparing `featurebox-0.0.9999/featurebox/cli/vasp_empty.py` & `featurebox-0.1.1/featurebox/cli/vasp_empty.py`

 * *Files identical despite different names*

### Comparing `featurebox-0.0.9999/featurebox/cli/vasp_general_diff.py` & `featurebox-0.1.1/featurebox/cli/vasp_general_diff.py`

 * *Files identical despite different names*

### Comparing `featurebox-0.0.9999/featurebox/cli/vasp_general_single.py` & `featurebox-0.1.1/featurebox/cli/vasp_general_single.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,14 @@
             except:
                 ii = pis[1]
                 return getattr(obj, pi[0])(ii)
     else:
         return getattr(obj, pi)
 
 
-
 class General(_BasePathOut):
     """Get data from paths and return csv file.
 
     Default keys Notes::
 
         mod="pymatgen.io.vasp"         # Module to get class.
         cmd="Vasprun"                  # class to get object.
@@ -104,15 +103,15 @@
             data = data
         elif isinstance(data, (float, int)):
             data = {self.prop: data}
         else:
             raise NotImplementedError(f"Unavailable data {type(data)}.")
 
         if self.store_single:
-            result = pd.DataFrame.from_dict({str(path):data}).T
+            result = pd.DataFrame.from_dict({str(path): data}).T
             result.to_csv("general_single.csv")
 
         return data
 
     def batch_after_treatment(self, paths, res_code):
         """4. Organize batch of data in tabular form, return one or more csv file. (force!!!)."""
         data_all = {pi: ri for pi, ri in zip(paths, res_code)}
```

### Comparing `featurebox-0.0.9999/featurebox/data/check_data.py` & `featurebox-0.1.1/featurebox/data/check_data.py`

 * *Files identical despite different names*

### Comparing `featurebox-0.0.9999/featurebox/data/data_sep.py` & `featurebox-0.1.1/featurebox/data/data_sep.py`

 * *Files identical despite different names*

### Comparing `featurebox-0.0.9999/featurebox/data/ele_megnet.json` & `featurebox-0.1.1/featurebox/data/ele_megnet.json`

 * *Files identical despite different names*

### Comparing `featurebox-0.0.9999/featurebox/data/ele_table.csv` & `featurebox-0.1.1/featurebox/data/ele_table.csv`

 * *Files identical despite different names*

### Comparing `featurebox-0.0.9999/featurebox/data/ele_table_norm.csv` & `featurebox-0.1.1/featurebox/data/ele_table_norm.csv`

 * *Files identical despite different names*

### Comparing `featurebox-0.0.9999/featurebox/data/ie.json` & `featurebox-0.1.1/featurebox/data/ie.json`

 * *Files identical despite different names*

### Comparing `featurebox-0.0.9999/featurebox/data/mp_access.py` & `featurebox-0.1.1/featurebox/data/mp_access.py`

 * *Files identical despite different names*

### Comparing `featurebox-0.0.9999/featurebox/data/name_split.py` & `featurebox-0.1.1/featurebox/data/name_split.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 # @License: BSD 3-Clause
 
 import copy
 import os
 import re
 from itertools import chain
 from typing import List
+
 import pandas as pd
 
 
 class _Ele:
     """Element type."""
 
     def __init__(self, name):
```

### Comparing `featurebox-0.0.9999/featurebox/data/oe.csv` & `featurebox-0.1.1/featurebox/data/oe.csv`

 * *Files identical despite different names*

### Comparing `featurebox-0.0.9999/featurebox/featurizers/atom/mapper.py` & `featurebox-0.1.1/featurebox/featurizers/atom/mapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,16 +67,16 @@
 ##############################################################
 
 class AtomMap(BaseFeature):
     """
     Base class for atom converter. Map the element type and weight to element data.
     """
 
-    def __init__(self, n_jobs: int = 1, on_errors: str = 'raise', return_type: str = 'any'):
-        super(AtomMap, self).__init__(n_jobs=n_jobs, on_errors=on_errors, return_type=return_type)
+    def __init__(self, n_jobs: int = 1, on_errors: str = 'raise', return_type: str = 'any', **kwargs):
+        super(AtomMap, self).__init__(n_jobs=n_jobs, on_errors=on_errors, return_type=return_type, **kwargs)
 
     @staticmethod
     def get_json_embeddings(file_name: str = "ele_megnet.json") -> Dict:
         """get json preprocessing"""
         data = loadfn(MODULE_DIR / "data" / file_name)
         data = {i: np.array(j) for i, j in data.items()}
         return data
@@ -91,35 +91,49 @@
 
 
 class BinaryMap(AtomMap):
     """Base converter with 2 different search_tp.
 
     """
 
-    def __init__(self, search_tp: str = "number", weight: bool = False, **kwargs):
+    def __init__(self, search_tp: str = "auto", weight: bool = False, **kwargs):
         """
 
         Args:
             search_tp: (str)
             weight: (bool) , For true,the same key data are summed together.
             **kwargs:
         """
         super().__init__(**kwargs)
         self.search_tp = search_tp
         self.weight = weight
         self.ndim = 1
 
     def _convert(self, d: Any) -> Any:
-        if self.search_tp in ["name", "name_dict"]:
+        if self.search_tp == 'auto':
+            if isinstance(d, Structure):
+                d = get_atom_fea_number(d)
+            if isinstance(d, dict):
+                d = [{k: v} for k, v in d.items()]
+            if isinstance(d[0], dict):
+                return self.convert_dict(d)
+            else:
+                return self.convert_number(d)
+
+        elif self.search_tp in ["name", "name_dict", "dict"]:
             if isinstance(d, Structure):
                 d = get_atom_fea_name(d)
+            if isinstance(d, dict):
+                d = [{k: v} for k, v in d.items()]
             return self.convert_dict(d)
         elif self.search_tp == "ion_name":
             if isinstance(d, Structure):
                 d = get_ion_fea_name(d)
+            if isinstance(d, dict):
+                d = [{k: v} for k, v in d.items()]
             return self.convert_dict(d)
         else:
             if isinstance(d, Structure):
                 d = get_atom_fea_number(d)
             return self.convert_number(d)
 
     @abstractmethod
@@ -158,28 +172,31 @@
     >>>
     >>> tmps = AtomJsonMap(search_tp="name")
     >>> s = [[{"H": 2, }, {"Ce": 1}],[{"H": 2, }, {"Al": 1}]]
     >>> a = tmps.transform(s)
 
     """
 
-    def __init__(self, embedding_dict: Union[str, Dict] = None, search_tp: str = "name", **kwargs):
+    def __init__(self, embedding_dict: Union[str, Dict] = None, search_tp: str = "auto",
+                 feature_labels=None, **kwargs):
         """
 
         Args:
             embedding_dict: (str,dict)
                 Name of file or dict,element to element vector dictionary
 
                 Provides the pre-trained elemental embeddings using formation energies,
                 which can be used to speed up the training. The embeddings
                 are also extremely useful elemental descriptors that encode chemical
                 similarity that may be used in other ways.
         """
 
         super(AtomJsonMap, self).__init__(**kwargs)
+        if feature_labels is None:
+            self._feature_labels = []
         if embedding_dict is None:
             embedding_dict = self.get_json_embeddings()
         elif isinstance(embedding_dict, str):
             embedding_dict = self.get_json_embeddings(embedding_dict)
 
         assert len(set([len(i) for i in embedding_dict.values()])) == 1, \
             "The element number should be same with `ele_megnet.json`, " \
@@ -285,15 +302,15 @@
     >>> s = [{"H": 2, }, {"Pd": 1}]
     >>> b = tmps.convert(s)
     ...
 
     """
 
     def __init__(self, tablename: Union[str, np.ndarray, pd.DataFrame, None] = "oe.csv",
-                 search_tp: str = "name", **kwargs):
+                 search_tp: str = "auto", **kwargs):
         """
 
         Parameters
         ----------
         tablename: str,np.ndarray, pd.Dateframe
             1. Name of table in bgnet.preprocessing.resources. if tablename is None,
             use the embedding "ele_table.csv".\n
@@ -387,14 +404,16 @@
 
     def __add__(self, other):
         if isinstance(other, AtomTableMap):
             assert other.search_tp == self.search_tp, "should be same"
             if self.search_tp == "number":
                 self.dax = np.concatenate((self.dax, other.dax), axis=1)
                 self.da = None
+                if self.da_columns is not None and other.da_columns is not None:
+                    self.da_columns = self.da_columns + other.da_columns
             else:
                 self.da = pd.concat((self.da, other.da), axis=1)
                 self.dax = None
         else:
             raise TypeError("only same class can be added.")
         return self
 
@@ -736,14 +755,15 @@
 
     def convert(self, structure: [Structure, Lattice]) -> np.ndarray:
         data_all = []
         datai = []
         for pi in self.prop_name:
             datai.append(_getter_arr(structure, pi))
         datai = [self.func[i](j) for i, j in enumerate(datai)]
+
         if not self.lengths:
             self.lengths = [len(i) if isinstance(i, (np.ndarray, tuple, list)) else 1 for i in datai]
         [data_all.extend(i) for i in datai]
 
         return np.array(data_all).ravel()
 
     def __add__(self, other):
```

### Comparing `featurebox-0.0.9999/featurebox/featurizers/base_feature.py` & `featurebox-0.1.1/featurebox/featurizers/base_feature.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import warnings
 from itertools import chain
 from multiprocessing import cpu_count
 from typing import List, Tuple, Iterable, Any
 
 import numpy as np
 import pandas as pd
+
 from mgetool.tool import parallelize
 
 
 class BaseFeature:
     """
     **Using a BaseFeature Class**
 
@@ -63,15 +64,15 @@
     __authors__ = ['boliqq07']
     __citations__ = ['No citations']
     _n_jobs = 1
     _feature_labels = []
 
     def __init__(self, n_jobs: int = 1, *, on_errors: str = 'raise', return_type: str = 'any',
                  batch_calculate: bool = False,
-                 batch_size: int = 30):
+                 batch_size: int = 30, feature_labels_mark: str = None, **kwargs):
         """
         Parameters
         ----------
         batch_size: int
             size of batch.
         batch_calculate :bool
             batch_calculate or not.
@@ -88,22 +89,36 @@
             'array' and 'df' force return type to np.ndarray and pd.DataFrame respectively.
             If 'any', without type conversion .
             Default is 'any'
         """
         self.return_type = return_type
         self.n_jobs = n_jobs
         self.on_errors = on_errors
-        self._kwargs = {"x_labels": None, "feature_labels_mark": None}
         self.support_ = []
         self.ndim = None
-        self._feature_labels = []
         self.batch_calculate = batch_calculate
         self.batch_size = batch_size
         # import inspect
         # inspect.getfullargspec(self.convert)
+        self._kwargs = {"x_labels": None, "feature_labels_mark": feature_labels_mark}
+        self._feature_labels = []
+
+    @staticmethod
+    def nonetoempty(d):
+        if d is None:
+            return []
+        else:
+            return d
+
+    @staticmethod
+    def emptytonone(d):
+        if not d:
+            return None
+        else:
+            return d
 
     @property
     def n_jobs(self):
         """
         n_jobs: int
             Parallel number.
         """
@@ -116,18 +131,15 @@
             self._n_jobs = cpu_count()
         else:
             self._n_jobs = n_jobs
 
     def fit(self, *args, **kwargs):
         """fit function in :class:`BaseFeature` are weakened and just pass parameter."""
         _ = args
-        if kwargs is {}:
-            pass
-        else:
-            self._kwargs.update(kwargs)
+        self._kwargs.update(kwargs)
         return self
 
     def fit_transform(self, X: List, y=None, **kwargs) -> Any:
         """
         If `convert` takes multiple inputs, supply inputs as a list of tuples.
 
         Copy from Mixin class for all transformers in scikit-learn. TransformerMixin
@@ -215,27 +227,35 @@
 
         ret, self.support_ = zip(*rets)
 
         if self.return_type == 'any':
             return ret
 
         if self.return_type == 'array' or self.return_type == 'np':
-            return np.array(ret)
+            try:
+                return np.array(ret)
+            except (NotImplementedError, TypeError):
+                warnings.warn(f"Try to convert result from {type(ret)} to ndarray failed.")
+                return ret
 
         if self.return_type == 'df' or self.return_type == 'pd':
             try:
+                ret = np.vstack(ret)
+
                 labels_len = len(self.feature_labels)
-                if labels_len > 0:
+                if ret.shape[1] == labels_len:
                     labels = self.feature_labels
                 else:
+                    warnings.warn("The feature name must be the same size with shape[1] for result (np.ndarray).")
                     labels = None
-            except (NotImplementedError, TypeError):
-                labels = None
-
-            return pd.DataFrame(ret, columns=labels, index=self._kwargs["x_labels"])
+                return pd.DataFrame(ret, columns=labels, index=self._kwargs["x_labels"])
+            except (NotImplementedError, TypeError, ValueError):
+                warnings.warn(f"Try to convert result from {type(ret)} to DataFrame failed."
+                              f"To build pd.Dataframe, The each result must be np.ndarray.")
+                return ret
 
     def _wrapper(self, *args, **kwargs):
         """
         An exception wrapper for convert, used in transform and
         changes the parameter passed to convert, and return the result with an bool mark.
 
         Notes
@@ -288,15 +308,15 @@
     def convert(self, d):
         """
         Main feature function, which has to be implemented
         in any derived feature subclass.
 
         Notes
         -----
-        It cannot be passed np.array in default unless:
+        It cannot be passed np.ndarray in default unless:
 
         1. useful for bond_converter.
         For np.array we check the ndim and for ndim 2, or 3.
         we decide whether to pass them the data to ``_converter``
         together or separately by ``self.ndim`` attribute. Now max support 3d.
         due to for some functions, using ``ufunc`` in numpy is very efficient.
 
@@ -341,15 +361,15 @@
         Returns:
             ([str]) attribute labels.
         """
         mark = self._kwargs["feature_labels_mark"]
         if mark is None:
             return self._feature_labels
         else:
-            return ["{}_{}".format(i, mark) for i in self._feature_labels]
+            return ["{}_{}".format(mark, i) for i in self._feature_labels]
 
     def set_feature_labels(self, values: List[str]):
         """Generate attribute names.
 
         Returns:
             ([str]) attribute labels.
         """
```

### Comparing `featurebox-0.0.9999/featurebox/featurizers/batch_feature.py` & `featurebox-0.1.1/featurebox/featurizers/batch_feature.py`

 * *Files identical despite different names*

### Comparing `featurebox-0.0.9999/featurebox/featurizers/envir/_get_radius_in_spheres.py` & `featurebox-0.1.1/featurebox/featurizers/envir/_get_radius_in_spheres.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,15 +66,15 @@
     neighbor_indices = neighbor_indices.astype(np.int64)
     # images = images.astype(np.int64)
     distances = distances.astype(np.float32)
     exclude_self = (distances > numerical_tol)
     # exclude_self = (center_indices != neighbor_indices) | (distances > numerical_tol)
 
     return center_indices[exclude_self], neighbor_indices[exclude_self], \
-           distances[exclude_self].reshape(-1, 1), distances[exclude_self], np.array(np.NaN)
+        distances[exclude_self].reshape(-1, 1), distances[exclude_self], np.array(np.NaN)
 
 # if __name__ == "__main__":
 #     from mgetool.tool import tt
 #
 #     structure = Structure.from_file("../../data/temp_test_structure/W2C.cif")
 #     tt.t
 #     get_points_ = get_radius_in_spheres(structure,
```

### Comparing `featurebox-0.0.9999/featurebox/featurizers/envir/_get_xyz_in_spheres.py` & `featurebox-0.1.1/featurebox/featurizers/envir/_get_xyz_in_spheres.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import itertools
+import math
 from collections import abc
 from typing import Tuple, Union, List
 
-import math
 import numpy as np
 
 from featurebox.utils.predefined_typing import StructureOrMolecule
 
 
 def _re_pbc(pbc: Union[bool, List[bool], np.ndarray], return_type="bool"):
     if pbc is True:
```

### Comparing `featurebox-0.0.9999/featurebox/featurizers/envir/desc_env.py` & `featurebox-0.1.1/featurebox/featurizers/envir/desc_env.py`

 * *Files identical despite different names*

### Comparing `featurebox-0.0.9999/featurebox/featurizers/envir/descriptors/ACSF.py` & `featurebox-0.1.1/featurebox/featurizers/envir/descriptors/ACSF.py`

 * *Files identical despite different names*

### Comparing `featurebox-0.0.9999/featurebox/featurizers/envir/descriptors/EAD.py` & `featurebox-0.1.1/featurebox/featurizers/envir/descriptors/EAD.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import math
+
 import numpy as np
 from ase.neighborlist import NeighborList
 
 from .cutoff import Cutoff
 
 
 class EAD:
```

### Comparing `featurebox-0.0.9999/featurebox/featurizers/envir/descriptors/EAMD.py` & `featurebox-0.1.1/featurebox/featurizers/envir/descriptors/EAMD.py`

 * *Files identical despite different names*

### Comparing `featurebox-0.0.9999/featurebox/featurizers/envir/descriptors/SO3.py` & `featurebox-0.1.1/featurebox/featurizers/envir/descriptors/SO3.py`

 * *Files identical despite different names*

### Comparing `featurebox-0.0.9999/featurebox/featurizers/envir/descriptors/SO4.py` & `featurebox-0.1.1/featurebox/featurizers/envir/descriptors/SO4.py`

 * *Files identical despite different names*

### Comparing `featurebox-0.0.9999/featurebox/featurizers/envir/descriptors/SOAP.py` & `featurebox-0.1.1/featurebox/featurizers/envir/descriptors/SOAP.py`

 * *Files identical despite different names*

### Comparing `featurebox-0.0.9999/featurebox/featurizers/envir/descriptors/_generate_coefs.py` & `featurebox-0.1.1/featurebox/featurizers/envir/descriptors/_generate_coefs.py`

 * *Files identical despite different names*

### Comparing `featurebox-0.0.9999/featurebox/featurizers/envir/descriptors/angular_momentum.py` & `featurebox-0.1.1/featurebox/featurizers/envir/descriptors/angular_momentum.py`

 * *Files identical despite different names*

### Comparing `featurebox-0.0.9999/featurebox/featurizers/envir/descriptors/behlerparrinello.py` & `featurebox-0.1.1/featurebox/featurizers/envir/descriptors/behlerparrinello.py`

 * *Files identical despite different names*

### Comparing `featurebox-0.0.9999/featurebox/featurizers/envir/descriptors/bispectrum.py` & `featurebox-0.1.1/featurebox/featurizers/envir/descriptors/bispectrum.py`

 * *Files identical despite different names*

### Comparing `featurebox-0.0.9999/featurebox/featurizers/envir/descriptors/cutoff.py` & `featurebox-0.1.1/featurebox/featurizers/envir/descriptors/cutoff.py`

 * *Files identical despite different names*

### Comparing `featurebox-0.0.9999/featurebox/featurizers/envir/descriptors/lbispectrum.py` & `featurebox-0.1.1/featurebox/featurizers/envir/descriptors/lbispectrum.py`

 * *Files identical despite different names*

### Comparing `featurebox-0.0.9999/featurebox/featurizers/envir/descriptors/utils.py` & `featurebox-0.1.1/featurebox/featurizers/envir/descriptors/utils.py`

 * *Files identical despite different names*

### Comparing `featurebox-0.0.9999/featurebox/featurizers/envir/descriptors/wACSF.py` & `featurebox-0.1.1/featurebox/featurizers/envir/descriptors/wACSF.py`

 * *Files identical despite different names*

### Comparing `featurebox-0.0.9999/featurebox/featurizers/envir/environment.py` & `featurebox-0.1.1/featurebox/featurizers/envir/environment.py`

 * *Files identical despite different names*

### Comparing `featurebox-0.0.9999/featurebox/featurizers/envir/local_env.py` & `featurebox-0.1.1/featurebox/featurizers/envir/local_env.py`

 * *Files 0% similar despite different names*

```diff
@@ -236,9 +236,9 @@
 
     distances = np.array(distances)
 
     exclude_self = (distances > numerical_tol)
     # exclude_self = (center_indices != neighbor_indices) | (distances > numerical_tol)
 
     return np.array(center_indices)[exclude_self], np.array(neighbor_indices)[exclude_self], \
-           np.array(images)[exclude_self], np.array(distances)[exclude_self], \
-           np.array(center_prop)
+        np.array(images)[exclude_self], np.array(distances)[exclude_self], \
+        np.array(center_prop)
```

### Comparing `featurebox-0.0.9999/featurebox/featurizers/state/extrastats.py` & `featurebox-0.1.1/featurebox/featurizers/state/extrastats.py`

 * *Files identical despite different names*

### Comparing `featurebox-0.0.9999/featurebox/featurizers/state/state_mapper.py` & `featurebox-0.1.1/featurebox/featurizers/state/state_mapper.py`

 * *Files identical despite different names*

### Comparing `featurebox-0.0.9999/featurebox/featurizers/state/statistics.py` & `featurebox-0.1.1/featurebox/featurizers/state/statistics.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # @Time    : 2019/11/1 13:18
 # @Email   : 986798607@qq.ele_ratio
 # @Software: PyCharm
 # @License: BSD 3-Clause
 
 from abc import abstractmethod
-from typing import List, Tuple, Union
+from typing import List, Tuple, Union, Type
 
 import numpy as np
 from pymatgen.core.composition import Composition as PMGComp
 from pymatgen.core.periodic_table import get_el_sp
 from pymatgen.util.string import formula_double_format
 
 from featurebox.featurizers.atom.mapper import AtomTableMap, BinaryMap
@@ -25,27 +25,29 @@
 
         def mix_function(self, elems:List, nums:List):
             w_ = np.array(nums)
             return w_.dot(elems)
 
     """
 
-    def __init__(self, data_map: BinaryMap, n_jobs: int = 1, on_errors: str = 'raise', return_type: str = 'df'):
+    def __init__(self, data_map: BinaryMap, n_jobs: int = 1, on_errors: str = 'raise',
+                 return_type: str = 'df', feature_labels_mark: str = None):
         """
         Base class for composition feature.
         """
-        super().__init__(n_jobs=n_jobs, on_errors=on_errors, return_type=return_type)
+        super().__init__(n_jobs=n_jobs, on_errors=on_errors, return_type=return_type,
+                         feature_labels_mark=feature_labels_mark)
         if data_map is None:
-            data_map = AtomTableMap(tablename="oe.csv", search_tp="name")
+            data_map = AtomTableMap(tablename="oe.csv", search_tp="auto")
         self.data_map = data_map
         # change
         self.data_map.weight = False
         self.data_map.n_jobs = 1
-
         self.search_tp = self.data_map.search_tp
+        self._feature_labels = self.data_map.feature_labels
 
     def convert_dict(self, atoms: dict) -> np.ndarray:
         """
         Convert atom {symbol: fraction} list to numeric features
         """
         if isinstance(atoms, dict):
             atoms = [{k: v} for k, v in atoms.items()]
@@ -53,25 +55,34 @@
         numbers = np.array([list(ai.values())[0] for ai in atoms])
 
         ele = self.data_map.convert(atoms)
         if len(atoms) == 1:
             ele = np.array(ele).reshape((len(atoms), -1))
         return self.mix_function(ele, numbers)
 
-    def convert_number(self, atoms: List) -> np.ndarray:
+    def convert_number(self, atoms: List):
         """
         Convert atom {symbol: fraction} list to numeric features
         """
         numbers = np.ones(len(atoms))
 
         ele = self.data_map.convert(atoms)
         if len(atoms) == 1:
             ele = np.array(ele).reshape((len(atoms), -1))
         return self.mix_function(ele, numbers)
 
+    def fit(self, *args, x_labels=None, **kwargs):
+        """fit function in :class:`BaseFeature` are weakened and just pass parameter."""
+        _ = args
+        if x_labels is not None:
+            assert len(args[0]) == x_labels
+        self._kwargs.update({"x_labels": x_labels})
+        self._kwargs.update(kwargs)
+        return self
+
     @abstractmethod
     def mix_function(self, elems: List, nums: Union[List, np.ndarray]):
         """
 
         Parameters
         ----------
         elems: list
@@ -83,116 +94,114 @@
         -------
         descriptor: numpy.ndarray
         """
 
 
 class WeightedAverage(BaseCompositionFeature):
     """
+
     Examples
     ---------
-    >>> from featurebox.featurizers.atom import AtomTableMap, AtomJsonMap
+    >>> from featurebox.featurizers.atom.mapper import AtomTableMap, AtomJsonMap
     >>> data_map = AtomJsonMap(search_tp="name", n_jobs=1)
     >>> wa = WeightedAverage(data_map, n_jobs=1,return_type="df")
     >>> x3 = [{"H": 2, "Pd": 1},{"He":1,"Al":4}]
     >>> wa.fit_transform(x3)
              0         1         2   ...        13        14        15
     0  0.422068  0.360958  0.201433  ... -0.459164 -0.064783 -0.250939
     1  0.007163 -0.471498 -0.072860  ...  0.206306 -0.041006  0.055843
     <BLANKLINE>
     [2 rows x 16 columns]
 
     >>> wa.set_feature_labels(["fea_{}".format(_) for _ in range(16)])
     >>> wa.fit_transform(x3)
-          fea_0     fea_1     fea_2  ...    fea_13    fea_14    fea_15
-    0  0.422068  0.360958  0.201433  ... -0.459164 -0.064783 -0.250939
-    1  0.007163 -0.471498 -0.072860  ...  0.206306 -0.041006  0.055843
+       wt_ave_fea_0  wt_ave_fea_1  ...  wt_ave_fea_14  wt_ave_fea_15
+    0      0.422068      0.360958  ...      -0.064783      -0.250939
+    1      0.007163     -0.471498  ...      -0.041006       0.055843
     <BLANKLINE>
     [2 rows x 16 columns]
 
     """
 
     def __init__(self, data_map: BinaryMap, n_jobs: int = 1, on_errors: str = 'raise', return_type: str = 'df'):
-        super().__init__(data_map, n_jobs=n_jobs, on_errors=on_errors, return_type=return_type)
+        super().__init__(data_map, n_jobs=n_jobs, on_errors=on_errors, return_type=return_type,
+                         feature_labels_mark="wt_ave")
 
     def mix_function(self, elems, nums):
         w_ = nums / np.sum(nums)
         return w_.dot(elems)
 
 
 class WeightedSum(BaseCompositionFeature):
     """
     Examples
     --------
-    >>> from featurebox.featurizers.atom import AtomTableMap, AtomJsonMap
-    >>> data_map = AtomJsonMap(search_tp="name", n_jobs=1)
+    >>> from featurebox.featurizers.atom.mapper import AtomTableMap, AtomJsonMap
+    >>> data_map = AtomTableMap(search_tp="name", n_jobs=1)
     >>> wa = WeightedSum(data_map, n_jobs=1,return_type="df")
     >>> x3 = [{"H": 2, "Pd": 1},{"He":1,"Al":4}]
     >>> wa.fit_transform(x3)
-             0         1         2   ...        13        14        15
-    0  1.266204  1.082873  0.604300  ... -1.377492 -0.194350 -0.752816
-    1  0.035813 -2.357490 -0.364302  ...  1.031530 -0.205029  0.279215
+       wt_sum_1s  wt_sum_2s  wt_sum_2p  ...  wt_sum_6d  wt_sum_6f  wt_sum_7s
+    0    8320.18   11837.27      11.80  ...        0.0        0.0        0.0
+    1    2188.73    1513.40     986.16  ...        0.0        0.0        0.0
     <BLANKLINE>
-    [2 rows x 16 columns]
-
-    >>> wa.set_feature_labels(["fea_{}".format(_) for _ in range(16)])
-    >>> wa.fit_transform(x3)
-          fea_0     fea_1     fea_2  ...    fea_13    fea_14    fea_15
-    0  1.266204  1.082873  0.604300  ... -1.377492 -0.194350 -0.752816
-    1  0.035813 -2.357490 -0.364302  ...  1.031530 -0.205029  0.279215
-    <BLANKLINE>
-    [2 rows x 16 columns]
+    [2 rows x 19 columns]
 
     """
 
     def __init__(self, data_map: BinaryMap, n_jobs: int = 1, on_errors: str = 'raise', return_type: str = 'df'):
-        super().__init__(data_map, n_jobs=n_jobs, on_errors=on_errors, return_type=return_type)
+        super().__init__(data_map, n_jobs=n_jobs, on_errors=on_errors, return_type=return_type,
+                         feature_labels_mark="wt_sum")
 
     def mix_function(self, elems, nums):
         w_ = np.array(nums)
         return w_.dot(elems)
 
 
 class GeometricMean(BaseCompositionFeature):
     """
     See Also:
         :class:`WeightedSum`
     """
 
     def __init__(self, data_map: BinaryMap, n_jobs: int = 1, on_errors: str = 'raise', return_type: str = 'df'):
-        super().__init__(data_map, n_jobs=n_jobs, on_errors=on_errors, return_type=return_type)
+        super().__init__(data_map, n_jobs=n_jobs, on_errors=on_errors, return_type=return_type,
+                         feature_labels_mark="geo_mean")
 
     def mix_function(self, elems: np.ndarray, nums):
         w_ = np.array(nums).reshape(-1, 1)
         tmp = elems ** w_
         return np.power(tmp.prod(axis=0), 1 / sum(w_))
 
 
 class HarmonicMean(BaseCompositionFeature):
     """
     See Also:
         :class:`WeightedSum`
     """
 
     def __init__(self, data_map: BinaryMap, n_jobs: int = 1, on_errors: str = 'raise', return_type: str = 'df'):
-        super().__init__(data_map, n_jobs=n_jobs, on_errors=on_errors, return_type=return_type)
+        super().__init__(data_map, n_jobs=n_jobs, on_errors=on_errors, return_type=return_type,
+                         feature_labels_mark="Harm_mean")
 
     def mix_function(self, elems, nums):
         w_ = np.array(nums)
         tmp = w_.dot(elems)
         return sum(w_) / tmp
 
 
 class WeightedVariance(BaseCompositionFeature):
     """
     See Also:
         :class:`WeightedSum`
     """
 
     def __init__(self, data_map: BinaryMap, n_jobs: int = 1, on_errors: str = 'raise', return_type: str = 'df'):
-        super().__init__(data_map, n_jobs=n_jobs, on_errors=on_errors, return_type=return_type)
+        super().__init__(data_map, n_jobs=n_jobs, on_errors=on_errors, return_type=return_type,
+                         feature_labels_mark="wt_var")
 
     def mix_function(self, elems: np.ndarray, nums):
         w_ = nums / np.sum(nums)
         mean_ = w_.dot(elems)
         var_ = elems - mean_
         return w_.dot(var_ ** 2)
 
@@ -200,42 +209,45 @@
 class MaxPooling(BaseCompositionFeature):
     """
     See Also:
         :class:`WeightedSum`
     """
 
     def __init__(self, data_map: BinaryMap, n_jobs: int = 1, on_errors: str = 'raise', return_type: str = 'df'):
-        super().__init__(data_map, n_jobs=n_jobs, on_errors=on_errors, return_type=return_type)
+        super().__init__(data_map, n_jobs=n_jobs, on_errors=on_errors, return_type=return_type,
+                         feature_labels_mark="max")
 
     def mix_function(self, elems, _):
         return np.max(elems, axis=0)
 
 
 class MinPooling(BaseCompositionFeature):
     """
     See Also:
         :class:`WeightedSum`
     """
 
     def __init__(self, data_map: BinaryMap, n_jobs: int = 1, on_errors: str = 'raise', return_type: str = 'df'):
-        super().__init__(data_map=data_map, n_jobs=n_jobs, on_errors=on_errors, return_type=return_type)
+        super().__init__(data_map=data_map, n_jobs=n_jobs, on_errors=on_errors, return_type=return_type,
+                         feature_labels_mark="min")
 
     def mix_function(self, elems, _):
         return np.min(elems, axis=0)
 
 
 class ExtraMix(BaseCompositionFeature):
     """
     See Also:
         :class:`WeightedSum`
     """
 
     def __init__(self, data_map: BinaryMap, stats: Tuple[str] = ("mean",), n_jobs: int = 1,
                  on_errors: str = 'raise', return_type: str = 'df'):
-        super().__init__(data_map=data_map, n_jobs=n_jobs, on_errors=on_errors, return_type=return_type)
+        super().__init__(data_map=data_map, n_jobs=n_jobs, on_errors=on_errors, return_type=return_type,
+                         feature_labels_mark="extra")
         self.stats = stats
 
     def mix_function(self, elems, nums):
         all_attributes = []
         for stat in self.stats:
             all_attributes.append(PropertyStats.calc_stat(elems, stat, nums))
 
@@ -251,28 +263,31 @@
     >>> from featurebox.featurizers.atom.mapper import AtomJsonMap
     >>> from featurebox.featurizers.state.union import UnionFeature
     >>> from featurebox.featurizers.state.statistics import DepartElementFeature
     >>> data_map = AtomJsonMap(search_tp="name",embedding_dict="ele_megnet.json", n_jobs=1) # keep this n_jobs=1 and return_type="np"
     >>> wa = DepartElementFeature(data_map,n_composition=2, n_jobs=1, return_type="pd")
     >>> comp = [{"H": 2, "Pd": 1},{"He":1, "Al":4}]
     >>> wa.set_feature_labels(["fea_{}".format(_) for _ in range(16)]) # 16 this the feature number of built-in "ele_megnet.json"
-    >>> couple_data = wa.fit_transform(comp)
-        fea_0_0   fea_0_1   fea_1_0  ...  fea_14_1  fea_15_0  fea_15_1
-    0  0.352363  0.561478  0.635952  ... -0.236541 -0.270104 -0.212607
-    1 -0.067220  0.025758  0.141113  ... -0.092577 -0.042185  0.080350
+    >>> wa.fit_transform(comp)
+       depart_fea_0_0  depart_fea_0_1  ...  depart_fea_15_0  depart_fea_15_1
+    0        0.352363        0.561478  ...        -0.270104        -0.212607
+    1       -0.067220        0.025758  ...        -0.042185         0.080350
     <BLANKLINE>
     [2 rows x 32 columns]
 
     """
 
     def __init__(self, data_map: BinaryMap, n_composition: int, n_jobs: int = 1, on_errors: str = 'raise',
                  return_type: str = 'df'):
 
-        super().__init__(data_map=data_map, n_jobs=n_jobs, on_errors=on_errors, return_type=return_type)
+        super().__init__(data_map=data_map, n_jobs=n_jobs, on_errors=on_errors, return_type=return_type,
+                         feature_labels_mark="depart")
         self.n_composition = n_composition
+        self._feature_labels = ["_".join((s, n)) for s in self.data_map.feature_labels
+                                for n in range(self.n_composition)]
 
     def mix_function(self, elems: np.ndarray, nums=None):
 
         return np.array(elems).ravel(order='F')
 
     def convert_dict(self, atoms: Union[dict, PMGComp]) -> np.ndarray:
         """
```

### Comparing `featurebox-0.0.9999/featurebox/featurizers/state/union.py` & `featurebox-0.1.1/featurebox/featurizers/state/union.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,35 +27,35 @@
     ---------
     >>> from featurebox.featurizers.atom.mapper import AtomTableMap, AtomJsonMap
     >>> data_map = AtomJsonMap(search_tp="name", n_jobs=1)
     >>> wa = DepartElementFeature(data_map,n_composition=2, n_jobs=1,return_type="df")
     >>> x3 = [{"H": 2, "Pd": 1},{"He":1,"Al":4}]
     >>> wa.set_feature_labels(["fea_{}".format(_) for _ in range(16)])
     >>> wa.fit_transform(x3)
-        fea_0_0   fea_0_1   fea_1_0  ...  fea_14_1  fea_15_0  fea_15_1
-    0  0.352363  0.561478  0.635952  ... -0.236541 -0.270104 -0.212607
-    1 -0.067220  0.025758  0.141113  ... -0.092577 -0.042185  0.080350
+       depart_fea_0_0  depart_fea_0_1  ...  depart_fea_15_0  depart_fea_15_1
+    0        0.352363        0.561478  ...        -0.270104        -0.212607
+    1       -0.067220        0.025758  ...        -0.042185         0.080350
     <BLANKLINE>
     [2 rows x 32 columns]
 
     >>> couple_data = wa.fit_transform(x3)
     >>> uf = UnionFeature(x3,couple_data,couple=2,stats=("mean","maximum"))
     >>> uf.fit_transform()
-        feamean  feamaximum   feamean  ...  feamaximum   feamean  feamaximum
-    0  0.422068    0.360958  0.201433  ...   -0.113506  0.021095   -0.212607
-    1  0.007163   -0.471498 -0.072860  ...    0.312183  0.165278    0.080350
+       mean_fea_0  maximum_fea_0  ...  mean_fea_15  maximum_fea_15
+    0    0.422068       0.360958  ...     0.021095       -0.212607
+    1    0.007163      -0.471498  ...     0.165278        0.080350
     <BLANKLINE>
     [2 rows x 32 columns]
 
     >>> couple_data = wa.fit_transform(x3)
     >>> uf = UnionFeature(x3,couple_data,couple=2,stats=("std_dev",))
     >>> uf.fit_transform()
-       feastd_dev  feastd_dev  feastd_dev  ...  feastd_dev  feastd_dev  feastd_dev
-    0    0.147867    0.583352    0.033739  ...    0.366625    0.182177    0.040657
-    1    0.065745    0.541477    0.209795  ...    0.374331    0.182331    0.086646
+       std_dev_fea_0  std_dev_fea_1  ...  std_dev_fea_14  std_dev_fea_15
+    0       0.147867       0.583352  ...        0.182177        0.040657
+    1       0.065745       0.541477  ...        0.182331        0.086646
     <BLANKLINE>
     [2 rows x 16 columns]
 
     """
 
     def __init__(self, comp: List[Dict], couple_data: Union[pd.DataFrame, np.ndarray], couple=2, stats=("mean",),
                  n_jobs: int = 1, on_errors: str = 'raise',
@@ -107,15 +107,16 @@
         self_elem_data_columns_values:List
             name
         Returns
         ---------
             ([str]) attribute labels.
         """
         name = np.array(self_elem_data_columns_values)[::self.couple]
-        name = [i.split("_")[0] + "%s" % j for i in name for j in self.stats]
+        name = ["%s" % j + "_" + "_".join(i.split("_")[:-1]) for i in name for j in self.stats]
+        name = [j.replace("depart_", "") for j in name if "depart_" in j]
         self._feature_labels = name
         return name
 
     fit_transform = transform
 
 
 class PolyFeature(BaseFeature, ABC):
@@ -126,16 +127,15 @@
 
     Examples
     -----------
     >>> n = np.array([[0,1,2,3,4,5],[0.422068,0.360958,0.201433,-0.459164,-0.064783,-0.250939]]).T
     >>> ps = pd.DataFrame(n,columns=["f1","f2"],index= ["x0","x1","x2","x3","x4","x5"])
     >>> pf = PolyFeature(degree=[1,2])
     >>> pf.fit_transform(n)
-
-    n   f0^1     f1^1  f0^2  f0^1*f1^1      f1^2
+       f0^1      f1^1  f0^2  f0^1*f1^1      f1^2
     0   0.0  0.422068   0.0   0.000000  0.178141
     1   1.0  0.360958   1.0   0.360958  0.130291
     2   2.0  0.201433   4.0   0.402866  0.040575
     3   3.0 -0.459164   9.0  -1.377492  0.210832
     4   4.0 -0.064783  16.0  -0.259132  0.004197
     5   5.0 -0.250939  25.0  -1.254695  0.062970
 
@@ -212,11 +212,25 @@
             rows = Counter(rows).items()
             nas = ["{}^{}".format(input_features[k], v) for k, v in rows]
             names = "*".join(nas)
 
             feature_names.append(names)
         self._feature_labels = feature_names
 
+
 # n = np.array([[0, 1, 2, 3, 4, 5], [0.422068, 0.360958, 0.201433, -0.459164, -0.064783, -0.250939]]).T
 # ps = pd.DataFrame(n, columns=["f1", "f2"], index=["x0", "x1", "x2", "x3", "x4", "x5"])
 # pf = PolyFeature(degree=[2, 3])
 # a = pf.fit_transform(n)
+
+
+if __name__ == "__main__":
+    from featurebox.featurizers.atom.mapper import AtomJsonMap
+
+    data_map = AtomJsonMap(search_tp="name", n_jobs=1)
+    wa = DepartElementFeature(data_map, n_composition=2, n_jobs=1, return_type="df")
+    x3 = [{"H": 2, "Pd": 1}, {"He": 1, "Al": 4}]
+    wa.set_feature_labels(["fea_{}".format(_) for _ in range(16)])
+
+    couple_data = wa.fit_transform(x3)
+    uf = UnionFeature(x3, couple_data, couple=2, stats=("mean", "maximum"))
+    res2 = uf.fit_transform()
```

### Comparing `featurebox-0.0.9999/featurebox/pbs/cli.py` & `featurebox-0.1.1/featurebox/pbs/cli.py`

 * *Files identical despite different names*

### Comparing `featurebox-0.0.9999/featurebox/pbs/jmk.py` & `featurebox-0.1.1/featurebox/pbs/jmk.py`

 * *Files identical despite different names*

### Comparing `featurebox-0.0.9999/featurebox/pbs/job_manager.py` & `featurebox-0.1.1/featurebox/pbs/job_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 #!/bin/bash
 import json
 import os.path
 import time
+from pathlib import Path
 from typing import Union, List, Sequence
 
 import pandas as pd
-from pathlib import Path
 
 from featurebox.pbs.pbs_conf import set_bachrc, reform_log_path, get_manager
 
 """
 JUST for LINUX
 """
+
+
 class JobPATH:
 
     def __init__(self, manager: Union[str, None] = "torque", simple=True):
 
         if manager is None:
             manager = get_manager()
         self.manager = manager
@@ -110,15 +112,15 @@
                 old_msg.update(self.msg)
         else:
             old_msg = self.msg
 
         with open(file, "w") as fp:
             json.dump(old_msg, fp)
 
-    def sparse(self,):
+    def sparse(self, ):
         res = {}
         cwd = Path.cwd()
         hm = Path.home()
 
         if cwd == hm:
             to_path = str(hm)
             mark = "~"
```

### Comparing `featurebox-0.0.9999/featurebox/pbs/misc.py` & `featurebox-0.1.1/featurebox/pbs/misc.py`

 * *Files identical despite different names*

### Comparing `featurebox-0.0.9999/featurebox/pbs/misc_slurm.py` & `featurebox-0.1.1/featurebox/pbs/misc_slurm.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
                 for i in souts:
                     if f"UserId={username}" in i:
                         if jobid is not None:
                             if any([f"JobId={ji}" in i for ji in jobid]):
                                 sout.append(i)
                         else:
                             sout.append(i)
-                if len(sout)>0:
+                if len(sout) > 0:
                     sout = "\n\n".join(sout)
                 else:
                     sout = None
             else:
                 sout = None
 
     else:
@@ -324,8 +324,7 @@
 
 
 if __name__ == "__main__":
     # res21 = find_executable("qsub")
     res1 = job_rundir(jobid=None)
 
     print(res1)
-
```

### Comparing `featurebox-0.0.9999/featurebox/pbs/misc_torque.py` & `featurebox-0.1.1/featurebox/pbs/misc_torque.py`

 * *Files identical despite different names*

### Comparing `featurebox-0.0.9999/featurebox/pbs/misc_unischeduler.py` & `featurebox-0.1.1/featurebox/pbs/misc_unischeduler.py`

 * *Files 0% similar despite different names*

```diff
@@ -270,12 +270,13 @@
     """qrls a PBS job."""
     if isinstance(jobid, str):
         res = run_popen(f"jctrl resume {jobid}")
     else:
         res = run_popen(f"jctrl resume " + " ".join(jobid))
     return jobid
 
+
 if __name__ == "__main__":
     # res21 = find_executable("qsub")
     print(job_status())
     # res = _jjobs(jobid=None)
     # print(res)
```

### Comparing `featurebox-0.0.9999/featurebox/pbs/pbs_conf.py` & `featurebox-0.1.1/featurebox/pbs/pbs_conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 
 
 def get_manager():
     return _get_manager()[0]
 
 
 def _get_manager():
-
     res2 = os.popen("whereis jsub").readlines()[0]
     res22 = re.search("(/\S+)+", res2)
     if res22:
         return "jsub", res22.group()
 
     res1 = os.popen("whereis sbatch").readlines()[0]
     res11 = re.search("(/\S+)+", res1)
```

### Comparing `featurebox-0.0.9999/featurebox/selection/backforward.py` & `featurebox-0.1.1/featurebox/selection/backforward.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,26 +10,26 @@
 
 import copy
 import warnings
 from functools import partial
 from typing import List
 
 import numpy as np
-from mgetool.tool import parallelize
 from sklearn.base import BaseEstimator
 from sklearn.base import MetaEstimatorMixin
 from sklearn.base import clone
 from sklearn.feature_selection import SelectorMixin
 from sklearn.metrics import check_scoring
 from sklearn.model_selection._search import BaseSearchCV
 from sklearn.model_selection._validation import _score, cross_val_score
 from sklearn.utils.metaestimators import if_delegate_has_method, _safe_split
 from sklearn.utils.validation import check_is_fitted, check_X_y, check_random_state
 
 from featurebox.selection.multibase import MultiBase
+from mgetool.tool import parallelize
 
 
 class BackForward(BaseEstimator, MetaEstimatorMixin, SelectorMixin, MultiBase):
     """
     BackForward method to selected features.
     
 
@@ -114,15 +114,15 @@
     >>> bf.estimator_.best_score_ # re cv_score in manually.
     -0.5919173121895709
     """
 
     def __init__(self, estimator: BaseEstimator, n_type_feature_to_select: int = None, primary_feature: int = None,
                  multi_grade: int = 2, multi_index: List = None, refit=True, cv=5, min_type_feature_to_select: int = 3,
                  must_index: List = None, tolerant: float = 0.01, verbose: int = 1, random_state: int = None,
-                 scoring: str = None, note=True):
+                 scoring: str = None, note: bool = True, filter_warn: bool = False):
         """
 
         Parameters
         ----------
         estimator : estimator object
             This is assumed to implement the scikit-learn estimator interface.
             A supervised sklearn learning estimator with ``fit`` method.
@@ -146,49 +146,51 @@
             random_state.
         refit:bool
             refit or not. if refit, the model would use all data.
         scoring:None,str
             scoring method name.
         note:bool
             print note or not.
+        filter_warn: bool
+            warnings.filterwarnings or not.
         """
         super().__init__(multi_grade=multi_grade, multi_index=multi_index, must_index=must_index)
         if any((hasattr(estimator, "max_features") and refit,
                 isinstance(estimator, BaseSearchCV) and hasattr(estimator.estimator, "max_features") and refit)):
             warnings.warn("For estimator with 'max_features' attribute, \n"
                           "the 'max_features' would changed with each sub-data. \n"
                           "Please change and define 'max_features' by manual testing \n"
                           "after Backforward!\n", UserWarning)
         if refit and note:
             if isinstance(estimator, BaseSearchCV) and estimator.refit is True:
                 print(
-f"""Note:
+                    f"""Note:
     If refit, the self.estimator_ :{estimator.__class__.__name__} would use all the data in ``fit`` function,
     1. Be careful with the 'score' and 'predict' functions,
     Those are **training** score/predict if data in ``predict`` function not changed!
     Those are **testing** score/predict if data in ``predict`` function changed!
     2. To get CV result for evaluation:
     self.estimator_ is the SearchCV object, check 'self.estimator_.cv_result' to get CV result.
     Using 'self.best_score_' or 'self.estimator_.best_score_' for evaluation,
-    Use 'cross_val_predict(self.estimator_,X[:, self.support_],y)' for plotting.""")
+    Use 'cross_val_predict(self.estimator_.best_estimator_,X[:, self.support_],y)' for plotting.""")
             else:
                 print(
-f"""Note:
+                    f"""Note:
     If refit, the self.estimator_ :{estimator.__class__.__name__} would use all the data in ``fit`` function,
     1. Be careful with the 'score' and 'predict' functions:
     Those are **training** score/predict, if data in ``predict`` function not changed!
     Those are **testing** score/predict, if data in ``predict`` function changed!
     2. To get CV result for evaluation:
     Use 'self.best_score_' or 'cross_val_score(self.estimator_,X[:, self.support_],y)' for evaluation,
     Use 'cross_val_predict(self.estimator_,X[:, self.support_],y)' for plotting.""")
 
         assert cv >= 3
 
         if isinstance(estimator, BaseSearchCV):
-            print(f"Uniform parameter in SearchCV and Exhaustion:\n"
+            print(f"Uniform parameters in SearchCV and Exhaustion:\n"
                   f"(scoring={scoring}, cv={cv}, refit={refit})")
             estimator.scoring = scoring
             estimator.cv = cv
             estimator.refit = refit
             estimator.n_jobs = 1
 
         self.scoring = scoring
@@ -201,14 +203,16 @@
         self.score_ = []
         self.random_state = random_state
         self.tolerant = tolerant
         self.refit = refit
         self.min_type_feature_to_select = min_type_feature_to_select
         self.cv = cv
         self.note = note
+        self.filter_warn = filter_warn
+
         if isinstance(n_type_feature_to_select, int):
             assert n_type_feature_to_select >= min_type_feature_to_select, "Max numbers should be large than Min numbers."
 
     @property
     def _estimator_type(self):
         return self.estimator._estimator_type
 
@@ -242,15 +246,15 @@
                     best0 = test_
                     slice10 = slice1_
                 elif test > max(best0, test_) + 2 * self.tolerant:
                     best0 = test
                 else:
                     slice10.remove(add1)
                 if self.verbose > 0:
-                    print("Fitting estimator with {} feature {}".format(len(slice10), best0))
+                    print("Fitting estimator with {} features {}".format(len(slice10), best0))
                 self.score_.append((tuple(slice10), best0))
             return slice10, best0
 
         def sub_slice(slice10):
             best0 = score(slices=slice10)
             slice0 = list(copy.deepcopy(slice10))
             slice10 = list(slice10)
@@ -289,19 +293,23 @@
                     slice_.remove(sub)
                 test0 = [score(slices=i) for i in slice_all]
                 index = int(np.argmax(test0))
                 best0 = max(test0)
                 slice0 = slice_all[index]
                 # print(slice0, best0)
                 if self.verbose > 0:
-                    print("Fitting estimator with {} feature {}".format(len(slice0), best0))
+                    print("Fitting estimator with {} features {}".format(len(slice0), best0))
                 self.score_.append((tuple(slice0), best0))
             return slice0, best0
 
         def score_pri(slices, x0, y0):
+
+            if self.filter_warn:
+                warnings.filterwarnings("ignore")
+
             slices = list(slices)
             if len(slices) <= 1:
                 score0 = - np.inf
             else:
                 slices = self.feature_unfold(slices)
                 data_x0 = x0[:, slices]
 
@@ -334,15 +342,15 @@
             n_feature = (self.multi_index[1] - self.multi_index[0]) // self.multi_grade + self.multi_index[0]
         else:
             n_feature = x.shape[1]
         if self.primary_feature is None:
             primary_feature = n_feature // 2
         else:
             primary_feature = self.primary_feature
-        assert primary_feature < n_feature, "Too large for primary_feature."
+        assert primary_feature < n_feature, "Too large for primary_features."
 
         feature_list = list(range(n_feature))
         fold_feature_list = self.feature_fold(feature_list)
 
         ran = check_random_state(self.random_state)
         slice1 = ran.choice(fold_feature_list, primary_feature, replace=False)
         slice1 = list(self.feature_fold(slice1))
@@ -571,15 +579,14 @@
         self.score_ = []
         self.random_state = random_state
         self.refit = refit
         self.tolerant = tolerant
         self.cv = cv
         self.note = note
 
-
     def fit(self, X, y, groups=None):
         """Fit the baf model and automatically tune the number of selected feature.
 
         Parameters
         ----------
         X : {array-like, sparse matrix}, shape = [n_samples, n_feature]
             Training vector, where `n_samples` is the number of samples and
```

### Comparing `featurebox-0.0.9999/featurebox/selection/corr.py` & `featurebox-0.1.1/featurebox/selection/corr.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,21 +10,21 @@
 Calculate the correction of columns.
 """
 import copy
 import warnings
 from typing import List
 
 import numpy as np
-from mgetool.tool import name_to_name
 from sklearn.base import BaseEstimator, MetaEstimatorMixin
 from sklearn.feature_selection import SelectorMixin
 from sklearn.utils import check_random_state
 from sklearn.utils.validation import check_is_fitted
 
 from featurebox.selection.multibase import MultiBase
+from mgetool.tool import name_to_name
 
 
 class Corr(BaseEstimator, MetaEstimatorMixin, SelectorMixin, MultiBase):
     """
     Calculate correlation. (Where the result are changed with random state.)
 
     **1. Used for filter automatically by machine**
@@ -112,16 +112,17 @@
             cov = pre_cal
         else:
             raise TypeError("pre_cal is None or coef of data_cluster with shape(data_cluster[0],data_cluster[0])")
 
         # for nan
         self.nan_index_mark = ~np.array([np.all(np.isnan(cov[i])) for i in range(cov.shape[0])])
         if not np.all(self.nan_index_mark):
-            warnings.warn("There are some NAN values in correlation coefficient matrix, which could be constant features.\n"
-                  "The NAN features would removed later. See more in 'nan_index_mark' attribute.",UserWarning)
+            warnings.warn(
+                "There are some NAN values in correlation coefficient matrix, which could be constant features.\n"
+                "The NAN features would removed later. See more in 'nan_index_mark' attribute.", UserWarning)
 
         cov = np.nan_to_num(cov)
         self.cov = cov
         self.data = data
         self.shrink_list = list(range(self.cov.shape[0]))
         self._shrink_coef(method=method)
         self.filter()
```

### Comparing `featurebox-0.0.9999/featurebox/selection/exhaustion.py` & `featurebox-0.1.1/featurebox/selection/exhaustion.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,26 +8,26 @@
 
 import warnings
 from functools import partial
 from itertools import combinations
 from typing import Tuple, List
 
 import numpy as np
-from mgetool.tool import parallelize
 from sklearn.base import BaseEstimator
 from sklearn.base import MetaEstimatorMixin
 from sklearn.base import clone
 from sklearn.feature_selection import SelectorMixin
 from sklearn.metrics import check_scoring
 from sklearn.model_selection import cross_val_score
 from sklearn.model_selection._search import BaseSearchCV
 from sklearn.utils.metaestimators import if_delegate_has_method
 from sklearn.utils.validation import check_is_fitted, check_X_y
 
 from featurebox.selection.multibase import MultiBase
+from mgetool.tool import parallelize
 
 
 class Exhaustion(BaseEstimator, MetaEstimatorMixin, SelectorMixin, MultiBase):
     """
     Exhaustion features combination.
 
     Attributes
@@ -85,15 +85,16 @@
     array([False, False, False,  True, False,  True, False, False])
     >>> bf.best_score_
     -0.7336740728050252
     """
 
     def __init__(self, estimator: BaseEstimator, n_select: Tuple = (2, 3, 4),
                  multi_grade: int = None, multi_index: List = None, must_index: List = None,
-                 n_jobs: int = 1, refit: bool = False, cv: int = 5, scoring: str = None, note=True):
+                 n_jobs: int = 1, refit: bool = False, cv: int = 5, scoring: str = None, note=True,
+                 filter_warn=False):
         """
 
         Parameters
         ----------
         estimator:
             sklearn model or GridSearchCV.
         n_select:tuple
@@ -110,36 +111,39 @@
             refit or not, if refit the model would use all data.
         cv:bool
             if estimator is sklearn model, used cv, else pass.
         scoring:None,str
             scoring method name.
         note:bool
             print note or not.
+        filter_warn: bool
+            warnings.filterwarnings or not.
         """
         super().__init__(multi_grade=multi_grade, multi_index=multi_index, must_index=must_index)
         if any((hasattr(estimator, "max_features") and refit,
                 isinstance(estimator, BaseSearchCV) and hasattr(estimator.estimator, "max_features") and refit)):
-            warnings.warn("For estimator with 'max_features' attribute, the 'max_features' would changed with each sub-data. \n"
-                  "Please change and define 'max_features' by SearchCV testing after Exhaustion.\n",UserWarning)
+            warnings.warn(
+                "For estimator with 'max_features' attribute, the 'max_features' would changed with each sub-data. \n"
+                "Please change and define 'max_features' by SearchCV testing after Exhaustion.\n", UserWarning)
 
         if refit and note:
             if isinstance(estimator, BaseSearchCV) and estimator.refit is True:
                 print(
-f"""Note:
+                    f"""Note:
     If refit, the self.estimator_ :{estimator.__class__.__name__} would use all the data in ``fit`` function,
     1. Be careful with the 'score' and 'predict' functions,
     Those are **training** score/predict if data in ``predict`` function not changed!
     Those are **testing** score/predict if data in ``predict`` function changed!
     2. To get CV result for evaluation:
     self.estimator_ is the SearchCV object, check 'self.estimator_.cv_result' to get CV result.
     Using 'self.best_score_' or 'self.estimator_.best_score_' for evaluation,
-    Use 'cross_val_predict(self.estimator_,X[:, self.support_],y)' for plotting.""")
+    Use 'cross_val_predict(self.estimator_.best_estimator_,X[:, self.support_],y)' for plotting.""")
             else:
                 print(
-f"""Note:
+                    f"""Note:
     If refit, the self.estimator_ :{estimator.__class__.__name__} would use all the data in ``fit`` function,
     1. Be careful with the 'score' and 'predict' functions:
     Those are **training** score/predict, if data in ``predict`` function not changed!
     Those are **testing** score/predict, if data in ``predict`` function changed!
     2. To get CV result for evaluation:
     Use 'self.best_score_' or 'cross_val_score(self.estimator_,X[:, self.support_],y)' for evaluation,
     Use 'cross_val_predict(self.estimator_,X[:, self.support_],y)' for plotting.""")
@@ -147,28 +151,29 @@
         if cv <= 1:
             warnings.warn(
                 "\nThe cv <= 1, the exhaustion would not use cross validate, and treat all data as train data, \n"
                 "cv<=1 is just used for debug!!!".format(
                     estimator.__class__.__name__), UserWarning)
 
         if isinstance(estimator, BaseSearchCV):
-            print(f"Uniform parameter in SearchCV and Exhaustion:\n"
+            print(f"Uniform parameters in SearchCV and Exhaustion:\n"
                   f"(scoring={scoring}, cv={cv}, refit={refit})")
             estimator.scoring = scoring
             estimator.cv = cv
             estimator.n_jobs = 1
             estimator.refit = refit
 
         self.scoring = scoring
         self.estimator = estimator
         self.score_ = []
         self.n_jobs = n_jobs
         self.n_select = [n_select, ] if isinstance(n_select, int) else n_select
         self.refit = refit
         self.cv = cv
+        self.filter_warn = filter_warn
 
     @property
     def _estimator_type(self):
         return self.estimator._estimator_type
 
     def fit(self, X, y):
         """Fit the baf model and then the underlying estimator on the selected feature.
@@ -177,21 +182,26 @@
         ----------
         X : {array-like, sparse matrix}, shape = [n_samples, n_feature]
             The training input0 samples.
 
         y : array-like, shape = [n_samples]
             The target values.
         """
+
         return self._fit(X, y)
 
     def _fit(self, x, y):
 
         estimator = clone(self.estimator)
 
         def score_pri(slices, x0, y0):
+
+            if self.filter_warn:
+                warnings.filterwarnings("ignore")
+
             slices = list(slices)
             if len(slices) < 1:
                 score0 = - np.inf
             else:
                 slices = self.feature_unfold(slices)
                 data_x0 = x0[:, slices]
```

### Comparing `featurebox-0.0.9999/featurebox/selection/ga.py` & `featurebox-0.1.1/featurebox/selection/ga.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 import random
+import warnings
 from collections import deque
 from functools import partial
 
 import numpy as np
 from deap import base
 from deap import tools
 from deap.algorithms import varAnd
 from deap.tools import mutShuffleIndexes
-from mgetool.newclass import create
-from mgetool.tool import check_random_state, parallelize
 from sklearn.base import BaseEstimator, MetaEstimatorMixin
 from sklearn.feature_selection import SelectorMixin
-from sklearn.metrics import r2_score, check_scoring
+from sklearn.metrics import check_scoring
 from sklearn.model_selection import cross_val_score
 from sklearn.model_selection._search import BaseSearchCV
 from sklearn.utils.validation import check_is_fitted
 
 from featurebox.selection.multibase import MultiBase
+from mgetool.newclass import create
+from mgetool.tool import check_random_state, parallelize
 
 
 def eaSimple(population, toolbox, cxpb, mutpb, ngen, stats=None, n_jobs=2,
              halloffame=None, verbose=__debug__):
     """This algorithm reproduce the simplest evolutionary algorithm.
 
     :param population: A list of individuals.
@@ -163,15 +164,15 @@
     >>> ga.score(X_test, y_test)
     -28.542309712899435
 
     """
 
     def __init__(self, estimator, n_jobs=2, pop_n=1000, hof_n=1, cxpb=0.6, mutpb=0.3, ngen=40, max_or_min="max",
                  mut_indpb=0.05, max_=None, min_=2, random_state=None, multi_grade=2, multi_index=None, must_index=None,
-                 cv: int = 5, scoring=None):
+                 cv: int = 5, scoring=None, filter_warn=False):
         """
 
         Parameters
         ----------
         estimator:
             sklearn estimator
         n_jobs:int
@@ -200,14 +201,16 @@
             binding grade
         multi_index:
             binding range [min,max]
         scoring:None,str
             scoring method name.
         cv:bool
             if estimator is sklearn model, used cv, else pass.
+        filter_warn: bool
+            warnings.filterwarnings or not.
         """
         super().__init__(multi_grade=multi_grade, multi_index=multi_index, must_index=must_index)
         assert cv >= 3
         if isinstance(estimator, BaseSearchCV):
             print(f"Using scoring:{scoring},and cv:{cv}")
             estimator.scoring = scoring
             estimator.cv = cv
@@ -223,14 +226,15 @@
         self.ngen = ngen
         self.mut_indpb = mut_indpb
         self.max_ = max_
         self.min_ = min_
         self.max_or_min = max_or_min
         self.random_state = random_state
         self.cv = cv
+        self.filter_warn = filter_warn
 
         check_random_state(random_state)
         random.seed(random_state)
         np.random.seed(random_state)
 
         self.toolbox = base.Toolbox()
         if max_or_min == "max":
@@ -304,14 +308,17 @@
         sss = []
         [sss.extend([i] * j) for i, j in zip(ind, self.x_space_fold)]
         if self.must_index is not None:
             [sss.__setitem__(i, 1) for i in self.must_index]
         return sss
 
     def fitness_func(self, ind, model, x, y, return_model=False):
+        if self.filter_warn:
+            warnings.filterwarnings("ignore")
+
         sss = self.unfold(ind)
         index = np.where(np.array(sss) == 1)[0]
         x = x[:, index]
         if x.shape[1] > 1:
             svr = model
             if hasattr(svr, "max_features"):
                 svr.max_features = x.shape[1]
```

### Comparing `featurebox-0.0.9999/featurebox/selection/multibase.py` & `featurebox-0.1.1/featurebox/selection/multibase.py`

 * *Files identical despite different names*

### Comparing `featurebox-0.0.9999/featurebox/utils/quickmethod.py` & `featurebox-0.1.1/featurebox/utils/quickmethod.py`

 * *Files 1% similar despite different names*

```diff
@@ -250,37 +250,37 @@
     cv10 = 5
     scoring10 = 'r2'
     param_grid10 = [
         {'max_depth': [2, 3, 4, 5, 6, 7, 8], "min_samples_split": [2, 3, 4], "min_samples_leaf": [1, 2]}]
     dict_method.update({'DTR-em': [me10, cv10, scoring10, param_grid10]})
 
     'ElasticNet'
-    me11 = ElasticNet(alpha=1.0, l1_ratio=0.7, fit_intercept=True, normalize=False, precompute=False, max_iter=1000,
+    me11 = ElasticNet(alpha=1.0, l1_ratio=0.7, fit_intercept=True, precompute=False, max_iter=1000,
                       copy_X=True, tol=0.0001, warm_start=False, positive=False, random_state=None)
 
     cv11 = 5
     scoring11 = 'r2'
     param_grid11 = [{'alpha': [0.0001, 0.001, 0.01, 0.1, 1, 10], 'l1_ratio': [0.3, 0.5, 0.8]}]
     dict_method.update({"EN-L1": [me11, cv11, scoring11, param_grid11]})
 
     'Lasso'
-    me12 = Lasso(alpha=1.0, fit_intercept=True, normalize=True, precompute=False, copy_X=True, max_iter=3000,
+    me12 = Lasso(alpha=1.0, fit_intercept=True,  precompute=False, copy_X=True, max_iter=3000,
                  tol=0.001,
                  warm_start=False, positive=False, random_state=None, )
 
     cv12 = 5
     scoring12 = 'r2'
     param_grid12 = [
         {'alpha': [0.0001, 0.0005, 0.001, 0.005, 0.01, 0.05, 0.1, 0.5, 1, 10, 100, 1000], "tol": [0.001, 0.01, 0.1]}, ]
     dict_method.update({"LASSO-L1": [me12, cv12, scoring12, param_grid12]})
 
     """2BayesianRidge"""
     me2 = BayesianRidge(alpha_1=1e-06, alpha_2=1e-06, compute_score=False,
                         copy_X=True, fit_intercept=True, lambda_1=1e-06, lambda_2=1e-06,
-                        n_iter=300, normalize=False, tol=0.01, verbose=False)
+                        n_iter=300, tol=0.01, verbose=False)
     cv2 = 5
     scoring2 = 'r2'
     param_grid2 = [{'alpha_1': [1e-07, 1e-06, 1e-05], 'alpha_2': [1e-07, 1e-06, 1e-05]}]
     dict_method.update({'BRR-L1': [me2, cv2, scoring2, param_grid2]})
 
     """3SGDRL2"""
     me3 = SGDRegressor(alpha=0.0001, average=False,
```

### Comparing `featurebox-0.0.9999/featurebox.egg-info/PKG-INFO` & `featurebox-0.1.1/featurebox.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: featurebox
-Version: 0.0.9999
+Version: 0.1.1
 Summary: This is an box contains tools for machine learning.Some of code are non-originality, just copy for use. All the referenced code are marked,details can be shown in their sources
 Home-page: https://github.com/boliqq07/featurebox
 Author: wangchangxin
 Author-email: 986798607@qq.com
 Maintainer: wangchangxin
-License: UNKNOWN
 Keywords: features,combination,selection
 Platform: Windows
 Platform: Unix
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
@@ -70,9 +69,7 @@
 
 Support
 ----------------------
 [![Jetbrains](jetbrains.svg)](https://jb.gg/OpenSource)
 
 
 
-
-
```

### Comparing `featurebox-0.0.9999/featurebox.egg-info/SOURCES.txt` & `featurebox-0.1.1/featurebox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `featurebox-0.0.9999/setup.py` & `featurebox-0.1.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='featurebox',
-    version='0.0.9999',
+    version='0.1.01',
     keywords=['features', "combination", "selection"],
     description='This is an box contains tools for machine learning.'
                 'Some of code are non-originality, just copy for use. All the referenced code are marked,'
                 'details can be shown in their sources',
     install_requires=['path', 'pandas', 'numpy', 'sympy', 'scipy', 'scikit-learn', 'joblib', 'matplotlib',
                       'deprecated',
                       'requests', 'tqdm', 'six', "pymatgen", "deap", "numba", "ase", "mgetool>=0.0.62"],
```

