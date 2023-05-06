# Comparing `tmp/napari-bacseg-1.0.5.tar.gz` & `tmp/napari-bacseg-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-bacseg-1.0.5.tar", last modified: Wed May  3 11:59:06 2023, max compression
+gzip compressed data, was "napari-bacseg-1.0.6.tar", last modified: Sat May  6 06:44:33 2023, max compression
```

## Comparing `napari-bacseg-1.0.5.tar` & `napari-bacseg-1.0.6.tar`

### file list

```diff
@@ -1,116 +1,118 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 11:59:06.168787 napari-bacseg-1.0.5/
-drwxrwxrwx   0        0        0        0 2023-05-03 11:59:05.982743 napari-bacseg-1.0.5/.github/
-drwxrwxrwx   0        0        0        0 2023-05-03 11:59:05.999644 napari-bacseg-1.0.5/.github/workflows/
--rw-rw-rw-   0        0        0     2904 2023-02-24 11:00:35.000000 napari-bacseg-1.0.5/.github/workflows/test_and_deploy.yml
--rw-rw-rw-   0        0        0     1239 2023-03-08 16:30:28.000000 napari-bacseg-1.0.5/.gitignore
-drwxrwxrwx   0        0        0        0 2023-05-03 11:59:06.003644 napari-bacseg-1.0.5/.napari-hub/
--rw-rw-rw-   0        0        0      472 2023-02-24 11:00:35.000000 napari-bacseg-1.0.5/.napari-hub/DESCRIPTION.md
--rw-rw-rw-   0        0        0      551 2023-02-24 11:00:35.000000 napari-bacseg-1.0.5/.napari-hub/config.yml
--rw-rw-rw-   0        0        0     1211 2023-02-24 11:01:10.000000 napari-bacseg-1.0.5/.pre-commit-config.yaml
--rw-rw-rw-   0        0        0     1515 2023-02-24 11:00:35.000000 napari-bacseg-1.0.5/LICENSE
--rw-rw-rw-   0        0        0      101 2023-02-24 11:00:35.000000 napari-bacseg-1.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0     4732 2023-05-03 11:59:06.168787 napari-bacseg-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     3859 2023-02-27 13:15:54.000000 napari-bacseg-1.0.5/README.md
--rw-rw-rw-   0        0        0      271 2023-02-27 13:15:54.000000 napari-bacseg-1.0.5/bacseg_ui.py
--rw-rw-rw-   0        0        0      988 2023-05-03 11:58:10.000000 napari-bacseg-1.0.5/pyproject.toml
--rw-rw-rw-   0        0        0     2035 2023-05-03 11:59:06.172787 napari-bacseg-1.0.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-03 11:59:05.984746 napari-bacseg-1.0.5/src/
-drwxrwxrwx   0        0        0        0 2023-05-03 11:59:06.110818 napari-bacseg-1.0.5/src/_dev/
--rw-rw-rw-   0        0        0      560 2022-10-16 10:26:58.000000 napari-bacseg-1.0.5/src/_dev/Export Masks to AKSEG v5 dev.py
--rw-rw-rw-   0        0        0     8279 2023-02-24 14:29:04.000000 napari-bacseg-1.0.5/src/_dev/ScanR dev.py
--rw-rw-rw-   0        0        0      482 2022-05-26 11:42:59.000000 napari-bacseg-1.0.5/src/_dev/Troodos dev.py
--rw-rw-rw-   0        0        0        0 2022-04-28 17:23:51.000000 napari-bacseg-1.0.5/src/_dev/__init__.py
--rw-rw-rw-   0        0        0     1878 2023-02-24 12:15:54.000000 napari-bacseg-1.0.5/src/_dev/akseg_db_stats.py
--rw-rw-rw-   0        0        0    11262 2023-02-24 14:19:52.000000 napari-bacseg-1.0.5/src/_dev/akseg_dev.py
--rw-rw-rw-   0        0        0     4463 2023-02-24 14:19:52.000000 napari-bacseg-1.0.5/src/_dev/akseg_dev2.py
--rw-rw-rw-   0        0        0    10114 2023-02-24 14:36:34.000000 napari-bacseg-1.0.5/src/_dev/akseg_txt_metadata.py
--rw-rw-rw-   0        0        0    10960 2023-02-24 14:19:52.000000 napari-bacseg-1.0.5/src/_dev/align_alex_datadump.py
--rw-rw-rw-   0        0        0    28052 2023-02-24 14:19:52.000000 napari-bacseg-1.0.5/src/_dev/alison_datadump.py
--rw-rw-rw-   0        0        0     4168 2023-02-24 14:19:11.000000 napari-bacseg-1.0.5/src/_dev/autocontast_dev.py
--rw-rw-rw-   0        0        0      454 2023-02-24 14:19:52.000000 napari-bacseg-1.0.5/src/_dev/cellposedev.py
--rw-rw-rw-   0        0        0      367 2022-09-22 16:01:43.000000 napari-bacseg-1.0.5/src/_dev/cellposeshapely.py
--rw-rw-rw-   0        0        0     1279 2023-03-27 16:45:42.000000 napari-bacseg-1.0.5/src/_dev/chatGPT_midlines.py
--rw-rw-rw-   0        0        0     4328 2023-05-03 08:47:29.000000 napari-bacseg-1.0.5/src/_dev/check_AluGasketv12_DFP.py
--rw-rw-rw-   0        0        0     6452 2023-02-24 14:19:52.000000 napari-bacseg-1.0.5/src/_dev/check_metadata.py
--rw-rw-rw-   0        0        0     1650 2023-02-24 14:19:11.000000 napari-bacseg-1.0.5/src/_dev/colicoords_cellldist_dev.py
--rw-rw-rw-   0        0        0     3442 2023-02-24 14:19:11.000000 napari-bacseg-1.0.5/src/_dev/colicoords_ldist_dev.py
--rw-rw-rw-   0        0        0    11185 2023-02-24 14:36:34.000000 napari-bacseg-1.0.5/src/_dev/database_dev.py
--rw-rw-rw-   0        0        0     1023 2023-03-23 14:05:20.000000 napari-bacseg-1.0.5/src/_dev/deepsegmattest.py
--rw-rw-rw-   0        0        0      666 2023-03-22 14:37:10.000000 napari-bacseg-1.0.5/src/_dev/edit_database_columns.py
--rw-rw-rw-   0        0        0     1701 2023-02-24 12:15:54.000000 napari-bacseg-1.0.5/src/_dev/fits_dev.py
--rw-rw-rw-   0        0        0     7216 2023-02-24 14:19:52.000000 napari-bacseg-1.0.5/src/_dev/fix_alison_missing_file_list.py
--rw-rw-rw-   0        0        0     1126 2023-02-24 14:19:52.000000 napari-bacseg-1.0.5/src/_dev/generate_scanr_movie.py
--rw-rw-rw-   0        0        0    24393 2023-02-24 14:19:52.000000 napari-bacseg-1.0.5/src/_dev/get_akseg_stats.py
--rw-rw-rw-   0        0        0     2623 2022-11-14 15:25:24.000000 napari-bacseg-1.0.5/src/_dev/get_species_info.py
--rw-rw-rw-   0        0        0     4255 2023-02-24 14:19:52.000000 napari-bacseg-1.0.5/src/_dev/luke__script.py
--rw-rw-rw-   0        0        0     5550 2023-02-24 14:21:12.000000 napari-bacseg-1.0.5/src/_dev/matplotlib_Events.py
--rw-rw-rw-   0        0        0    40825 2023-03-22 17:47:52.000000 napari-bacseg-1.0.5/src/_dev/move_AluGasketDFP.py
--rw-rw-rw-   0        0        0    44028 2023-04-04 10:28:53.000000 napari-bacseg-1.0.5/src/_dev/move_AluGasketDFP_poster.py
--rw-rw-rw-   0        0        0    48241 2023-04-26 15:22:38.000000 napari-bacseg-1.0.5/src/_dev/move_AluGasketv12_DFP.py
--rw-rw-rw-   0        0        0    35330 2023-03-13 15:20:23.000000 napari-bacseg-1.0.5/src/_dev/move_conor_nim_dfp_data.py
--rw-rw-rw-   0        0        0    34295 2023-03-08 10:06:11.000000 napari-bacseg-1.0.5/src/_dev/move_pillar_data.py
--rw-rw-rw-   0        0        0    37169 2023-02-24 14:19:52.000000 napari-bacseg-1.0.5/src/_dev/move_pillar_zstack_data.py
--rw-rw-rw-   0        0        0    57720 2023-02-24 14:29:03.000000 napari-bacseg-1.0.5/src/_dev/move_unlearning_files.py
--rw-rw-rw-   0        0        0      686 2023-02-14 15:45:10.000000 napari-bacseg-1.0.5/src/_dev/new_metadata2.pickle.py
--rw-rw-rw-   0        0        0     5989 2023-02-24 14:29:03.000000 napari-bacseg-1.0.5/src/_dev/new_read_akseg_directory.py
--rw-rw-rw-   0        0        0     7222 2023-02-24 14:19:52.000000 napari-bacseg-1.0.5/src/_dev/nim_dev.py
--rw-rw-rw-   0        0        0     3173 2023-02-24 14:19:52.000000 napari-bacseg-1.0.5/src/_dev/omnipose_dev.py
--rw-rw-rw-   0        0        0     4398 2023-02-24 14:29:04.000000 napari-bacseg-1.0.5/src/_dev/omnipose_midlines.py
--rw-rw-rw-   0        0        0     3032 2023-02-24 14:29:04.000000 napari-bacseg-1.0.5/src/_dev/omnipose_train.py
--rw-rw-rw-   0        0        0    33520 2023-02-24 14:29:03.000000 napari-bacseg-1.0.5/src/_dev/oufti_dilate.py
--rw-rw-rw-   0        0        0    37571 2023-03-06 10:55:01.000000 napari-bacseg-1.0.5/src/_dev/oufti_dilate_with_midlines.py
--rw-rw-rw-   0        0        0    32011 2023-02-24 14:19:52.000000 napari-bacseg-1.0.5/src/_dev/process_alex_datadump.py
--rw-rw-rw-   0        0        0    32643 2023-02-24 14:19:52.000000 napari-bacseg-1.0.5/src/_dev/process_alex_datadump_clinical.py
--rw-rw-rw-   0        0        0    28804 2023-02-24 14:19:52.000000 napari-bacseg-1.0.5/src/_dev/process_conor_datadump.py
--rw-rw-rw-   0        0        0    30160 2023-02-24 14:19:52.000000 napari-bacseg-1.0.5/src/_dev/process_gramstain_datadump.py
--rw-rw-rw-   0        0        0      576 2022-08-16 09:34:20.000000 napari-bacseg-1.0.5/src/_dev/read_non_tif.py
--rw-rw-rw-   0        0        0     7794 2023-02-24 14:19:52.000000 napari-bacseg-1.0.5/src/_dev/rebuild_usermeta.py
--rw-rw-rw-   0        0        0    10440 2023-02-24 14:19:52.000000 napari-bacseg-1.0.5/src/_dev/rebuild_usermeta_2.py
--rw-rw-rw-   0        0        0     3034 2023-03-23 13:58:59.000000 napari-bacseg-1.0.5/src/_dev/recreate_user_metadata.py
--rw-rw-rw-   0        0        0     2117 2023-04-20 14:14:30.000000 napari-bacseg-1.0.5/src/_dev/scalebar_dev.py
--rw-rw-rw-   0        0        0    25122 2023-02-24 14:19:52.000000 napari-bacseg-1.0.5/src/_dev/sort_midlines.py
--rw-rw-rw-   0        0        0     9633 2023-02-24 14:19:52.000000 napari-bacseg-1.0.5/src/_dev/stelios_stats.py
--rw-rw-rw-   0        0        0      644 2023-02-24 14:19:52.000000 napari-bacseg-1.0.5/src/_dev/tile_meta_check.py
--rw-rw-rw-   0        0        0     1615 2022-07-22 11:43:30.000000 napari-bacseg-1.0.5/src/_dev/tiler_dev.py
--rw-rw-rw-   0        0        0     3064 2023-02-24 14:29:04.000000 napari-bacseg-1.0.5/src/_dev/updade_akseg_metadata.py
--rw-rw-rw-   0        0        0     2057 2023-02-24 12:22:32.000000 napari-bacseg-1.0.5/src/_dev/update_img_metadata.py
--rw-rw-rw-   0        0        0     6859 2023-02-24 14:19:52.000000 napari-bacseg-1.0.5/src/_dev/video_iamges.py
--rw-rw-rw-   0        0        0     7767 2023-03-13 16:18:11.000000 napari-bacseg-1.0.5/src/_dev/zooniverse.py
--rw-rw-rw-   0        0        0     5624 2023-02-24 14:21:12.000000 napari-bacseg-1.0.5/src/_dev/zooniverse_move.py
--rw-rw-rw-   0        0        0     5742 2023-03-15 10:15:29.000000 napari-bacseg-1.0.5/src/_dev/zooniverse_move_titrations.py
--rw-rw-rw-   0        0        0    30267 2023-03-13 16:29:04.000000 napari-bacseg-1.0.5/src/_dev/zooniverse_titration_upload.py
--rw-rw-rw-   0        0        0     7503 2023-03-13 17:00:21.000000 napari-bacseg-1.0.5/src/_dev/zooniverse_titrations.py
--rw-rw-rw-   0        0        0    30267 2023-03-13 16:09:34.000000 napari-bacseg-1.0.5/src/_dev/zooniverse_upload.py
-drwxrwxrwx   0        0        0        0 2023-05-03 11:59:06.146818 napari-bacseg-1.0.5/src/napari_bacseg/
--rw-rw-rw-   0        0        0      155 2023-05-03 08:55:44.000000 napari-bacseg-1.0.5/src/napari_bacseg/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 11:59:06.168787 napari-bacseg-1.0.5/src/napari_bacseg/_tests/
--rw-rw-rw-   0        0        0        0 2023-02-24 11:00:35.000000 napari-bacseg-1.0.5/src/napari_bacseg/_tests/__init__.py
--rw-rw-rw-   0        0        0    26398 2023-05-03 08:53:54.000000 napari-bacseg-1.0.5/src/napari_bacseg/_tests/test_bacseg.py
--rw-rw-rw-   0        0        0     1276 2023-02-27 13:15:54.000000 napari-bacseg-1.0.5/src/napari_bacseg/_tests/test_widget.py
--rw-rw-rw-   0        0        0    88996 2023-05-03 08:53:54.000000 napari-bacseg-1.0.5/src/napari_bacseg/_utils.py
--rw-rw-rw-   0        0        0    13550 2023-04-21 11:56:56.000000 napari-bacseg-1.0.5/src/napari_bacseg/_utils_cellpose.py
--rw-rw-rw-   0        0        0    17465 2023-02-27 13:15:54.000000 napari-bacseg-1.0.5/src/napari_bacseg/_utils_colicoords.py
--rw-rw-rw-   0        0        0    20495 2023-05-03 08:53:54.000000 napari-bacseg-1.0.5/src/napari_bacseg/_utils_database.py
--rw-rw-rw-   0        0        0    57080 2023-05-03 08:53:54.000000 napari-bacseg-1.0.5/src/napari_bacseg/_utils_database_IO.py
--rw-rw-rw-   0        0        0     1645 2023-03-09 18:16:07.000000 napari-bacseg-1.0.5/src/napari_bacseg/_utils_imagej.py
--rw-rw-rw-   0        0        0    39007 2023-05-03 08:53:54.000000 napari-bacseg-1.0.5/src/napari_bacseg/_utils_interface_events.py
--rw-rw-rw-   0        0        0     4279 2023-05-03 08:53:54.000000 napari-bacseg-1.0.5/src/napari_bacseg/_utils_json.py
--rw-rw-rw-   0        0        0    34168 2023-03-07 17:38:57.000000 napari-bacseg-1.0.5/src/napari_bacseg/_utils_oufti.py
--rw-rw-rw-   0        0        0     2132 2023-02-27 13:15:54.000000 napari-bacseg-1.0.5/src/napari_bacseg/_utils_refine.py
--rw-rw-rw-   0        0        0    21190 2023-03-27 09:54:48.000000 napari-bacseg-1.0.5/src/napari_bacseg/_utils_statistics.py
--rw-rw-rw-   0        0        0     7055 2023-02-27 13:15:54.000000 napari-bacseg-1.0.5/src/napari_bacseg/_utils_tiler.py
--rw-rw-rw-   0        0        0      164 2023-05-03 11:59:05.000000 napari-bacseg-1.0.5/src/napari_bacseg/_version.py
--rw-rw-rw-   0        0        0    92177 2023-05-03 08:53:54.000000 napari-bacseg-1.0.5/src/napari_bacseg/_widget.py
--rw-rw-rw-   0        0        0   158964 2023-04-21 13:35:29.000000 napari-bacseg-1.0.5/src/napari_bacseg/bacseg_ui.py
--rw-rw-rw-   0        0        0   156906 2023-04-21 13:28:54.000000 napari-bacseg-1.0.5/src/napari_bacseg/bacseg_ui.ui
--rw-rw-rw-   0        0        0      271 2023-02-27 13:15:54.000000 napari-bacseg-1.0.5/src/napari_bacseg/gapseq_ui.py
--rw-rw-rw-   0        0        0      501 2023-03-07 17:38:57.000000 napari-bacseg-1.0.5/src/napari_bacseg/napari.yaml
--rw-rw-rw-   0        0        0      271 2023-02-27 13:15:54.000000 napari-bacseg-1.0.5/src/napari_bacseg/napari_ui.py
-drwxrwxrwx   0        0        0        0 2023-05-03 11:59:06.164787 napari-bacseg-1.0.5/src/napari_bacseg.egg-info/
--rw-rw-rw-   0        0        0     4732 2023-05-03 11:59:05.000000 napari-bacseg-1.0.5/src/napari_bacseg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3202 2023-05-03 11:59:05.000000 napari-bacseg-1.0.5/src/napari_bacseg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 11:59:05.000000 napari-bacseg-1.0.5/src/napari_bacseg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2023-05-03 11:59:05.000000 napari-bacseg-1.0.5/src/napari_bacseg.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      352 2023-05-03 11:59:05.000000 napari-bacseg-1.0.5/src/napari_bacseg.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-05-03 11:59:05.000000 napari-bacseg-1.0.5/src/napari_bacseg.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      644 2023-02-24 11:00:35.000000 napari-bacseg-1.0.5/tox.ini
+drwxrwxrwx   0        0        0        0 2023-05-06 06:44:33.572559 napari-bacseg-1.0.6/
+drwxrwxrwx   0        0        0        0 2023-05-06 06:44:33.211103 napari-bacseg-1.0.6/.github/
+drwxrwxrwx   0        0        0        0 2023-05-06 06:44:33.234044 napari-bacseg-1.0.6/.github/workflows/
+-rw-rw-rw-   0        0        0     2904 2023-02-24 11:00:35.000000 napari-bacseg-1.0.6/.github/workflows/test_and_deploy.yml
+-rw-rw-rw-   0        0        0     1239 2023-03-08 16:30:28.000000 napari-bacseg-1.0.6/.gitignore
+drwxrwxrwx   0        0        0        0 2023-05-06 06:44:33.240028 napari-bacseg-1.0.6/.napari-hub/
+-rw-rw-rw-   0        0        0      472 2023-02-24 11:00:35.000000 napari-bacseg-1.0.6/.napari-hub/DESCRIPTION.md
+-rw-rw-rw-   0        0        0      551 2023-02-24 11:00:35.000000 napari-bacseg-1.0.6/.napari-hub/config.yml
+-rw-rw-rw-   0        0        0     1211 2023-02-24 11:01:10.000000 napari-bacseg-1.0.6/.pre-commit-config.yaml
+-rw-rw-rw-   0        0        0     1515 2023-02-24 11:00:35.000000 napari-bacseg-1.0.6/LICENSE
+-rw-rw-rw-   0        0        0      101 2023-02-24 11:00:35.000000 napari-bacseg-1.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     4732 2023-05-06 06:44:33.573557 napari-bacseg-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     3859 2023-02-27 13:15:54.000000 napari-bacseg-1.0.6/README.md
+-rw-rw-rw-   0        0        0      271 2023-02-27 13:15:54.000000 napari-bacseg-1.0.6/bacseg_ui.py
+-rw-rw-rw-   0        0        0      988 2023-05-06 06:42:46.000000 napari-bacseg-1.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0     2035 2023-05-06 06:44:33.576549 napari-bacseg-1.0.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-06 06:44:33.213098 napari-bacseg-1.0.6/src/
+drwxrwxrwx   0        0        0        0 2023-05-06 06:44:33.478899 napari-bacseg-1.0.6/src/_dev/
+-rw-rw-rw-   0        0        0      560 2022-10-16 10:26:58.000000 napari-bacseg-1.0.6/src/_dev/Export Masks to AKSEG v5 dev.py
+-rw-rw-rw-   0        0        0     8279 2023-02-24 14:29:04.000000 napari-bacseg-1.0.6/src/_dev/ScanR dev.py
+-rw-rw-rw-   0        0        0      482 2022-05-26 11:42:59.000000 napari-bacseg-1.0.6/src/_dev/Troodos dev.py
+-rw-rw-rw-   0        0        0        0 2022-04-28 17:23:51.000000 napari-bacseg-1.0.6/src/_dev/__init__.py
+-rw-rw-rw-   0        0        0     1878 2023-02-24 12:15:54.000000 napari-bacseg-1.0.6/src/_dev/akseg_db_stats.py
+-rw-rw-rw-   0        0        0    11262 2023-02-24 14:19:52.000000 napari-bacseg-1.0.6/src/_dev/akseg_dev.py
+-rw-rw-rw-   0        0        0     4463 2023-02-24 14:19:52.000000 napari-bacseg-1.0.6/src/_dev/akseg_dev2.py
+-rw-rw-rw-   0        0        0    10114 2023-02-24 14:36:34.000000 napari-bacseg-1.0.6/src/_dev/akseg_txt_metadata.py
+-rw-rw-rw-   0        0        0    10960 2023-02-24 14:19:52.000000 napari-bacseg-1.0.6/src/_dev/align_alex_datadump.py
+-rw-rw-rw-   0        0        0    28052 2023-02-24 14:19:52.000000 napari-bacseg-1.0.6/src/_dev/alison_datadump.py
+-rw-rw-rw-   0        0        0     4168 2023-02-24 14:19:11.000000 napari-bacseg-1.0.6/src/_dev/autocontast_dev.py
+-rw-rw-rw-   0        0        0      454 2023-02-24 14:19:52.000000 napari-bacseg-1.0.6/src/_dev/cellposedev.py
+-rw-rw-rw-   0        0        0      367 2022-09-22 16:01:43.000000 napari-bacseg-1.0.6/src/_dev/cellposeshapely.py
+-rw-rw-rw-   0        0        0     1279 2023-03-27 16:45:42.000000 napari-bacseg-1.0.6/src/_dev/chatGPT_midlines.py
+-rw-rw-rw-   0        0        0     6105 2023-05-05 10:49:23.000000 napari-bacseg-1.0.6/src/_dev/check_AluGasketv12_DFP.py
+-rw-rw-rw-   0        0        0     6452 2023-02-24 14:19:52.000000 napari-bacseg-1.0.6/src/_dev/check_metadata.py
+-rw-rw-rw-   0        0        0     1650 2023-02-24 14:19:11.000000 napari-bacseg-1.0.6/src/_dev/colicoords_cellldist_dev.py
+-rw-rw-rw-   0        0        0     3442 2023-02-24 14:19:11.000000 napari-bacseg-1.0.6/src/_dev/colicoords_ldist_dev.py
+-rw-rw-rw-   0        0        0    11185 2023-02-24 14:36:34.000000 napari-bacseg-1.0.6/src/_dev/database_dev.py
+-rw-rw-rw-   0        0        0     1023 2023-03-23 14:05:20.000000 napari-bacseg-1.0.6/src/_dev/deepsegmattest.py
+-rw-rw-rw-   0        0        0      666 2023-03-22 14:37:10.000000 napari-bacseg-1.0.6/src/_dev/edit_database_columns.py
+-rw-rw-rw-   0        0        0     1701 2023-02-24 12:15:54.000000 napari-bacseg-1.0.6/src/_dev/fits_dev.py
+-rw-rw-rw-   0        0        0     7216 2023-02-24 14:19:52.000000 napari-bacseg-1.0.6/src/_dev/fix_alison_missing_file_list.py
+-rw-rw-rw-   0        0        0     1126 2023-02-24 14:19:52.000000 napari-bacseg-1.0.6/src/_dev/generate_scanr_movie.py
+-rw-rw-rw-   0        0        0    24393 2023-02-24 14:19:52.000000 napari-bacseg-1.0.6/src/_dev/get_akseg_stats.py
+-rw-rw-rw-   0        0        0     2623 2022-11-14 15:25:24.000000 napari-bacseg-1.0.6/src/_dev/get_species_info.py
+-rw-rw-rw-   0        0        0     4255 2023-02-24 14:19:52.000000 napari-bacseg-1.0.6/src/_dev/luke__script.py
+-rw-rw-rw-   0        0        0     5550 2023-02-24 14:21:12.000000 napari-bacseg-1.0.6/src/_dev/matplotlib_Events.py
+-rw-rw-rw-   0        0        0    40825 2023-03-22 17:47:52.000000 napari-bacseg-1.0.6/src/_dev/move_AluGasketDFP.py
+-rw-rw-rw-   0        0        0    44028 2023-04-04 10:28:53.000000 napari-bacseg-1.0.6/src/_dev/move_AluGasketDFP_poster.py
+-rw-rw-rw-   0        0        0    48241 2023-04-26 15:22:38.000000 napari-bacseg-1.0.6/src/_dev/move_AluGasketv12_DFP.py
+-rw-rw-rw-   0        0        0    46551 2023-05-05 08:15:07.000000 napari-bacseg-1.0.6/src/_dev/move_AluGasketv12_DFP_Titration.py
+-rw-rw-rw-   0        0        0    35330 2023-03-13 15:20:23.000000 napari-bacseg-1.0.6/src/_dev/move_conor_nim_dfp_data.py
+-rw-rw-rw-   0        0        0    34295 2023-03-08 10:06:11.000000 napari-bacseg-1.0.6/src/_dev/move_pillar_data.py
+-rw-rw-rw-   0        0        0    37169 2023-02-24 14:19:52.000000 napari-bacseg-1.0.6/src/_dev/move_pillar_zstack_data.py
+-rw-rw-rw-   0        0        0    57720 2023-02-24 14:29:03.000000 napari-bacseg-1.0.6/src/_dev/move_unlearning_files.py
+-rw-rw-rw-   0        0        0      686 2023-02-14 15:45:10.000000 napari-bacseg-1.0.6/src/_dev/new_metadata2.pickle.py
+-rw-rw-rw-   0        0        0     5989 2023-02-24 14:29:03.000000 napari-bacseg-1.0.6/src/_dev/new_read_akseg_directory.py
+-rw-rw-rw-   0        0        0     7222 2023-02-24 14:19:52.000000 napari-bacseg-1.0.6/src/_dev/nim_dev.py
+-rw-rw-rw-   0        0        0     3173 2023-02-24 14:19:52.000000 napari-bacseg-1.0.6/src/_dev/omnipose_dev.py
+-rw-rw-rw-   0        0        0     4398 2023-02-24 14:29:04.000000 napari-bacseg-1.0.6/src/_dev/omnipose_midlines.py
+-rw-rw-rw-   0        0        0     3032 2023-02-24 14:29:04.000000 napari-bacseg-1.0.6/src/_dev/omnipose_train.py
+-rw-rw-rw-   0        0        0    33520 2023-02-24 14:29:03.000000 napari-bacseg-1.0.6/src/_dev/oufti_dilate.py
+-rw-rw-rw-   0        0        0    37571 2023-03-06 10:55:01.000000 napari-bacseg-1.0.6/src/_dev/oufti_dilate_with_midlines.py
+-rw-rw-rw-   0        0        0     4449 2023-05-04 09:42:23.000000 napari-bacseg-1.0.6/src/_dev/pandas_speed.py
+-rw-rw-rw-   0        0        0    32011 2023-02-24 14:19:52.000000 napari-bacseg-1.0.6/src/_dev/process_alex_datadump.py
+-rw-rw-rw-   0        0        0    32643 2023-02-24 14:19:52.000000 napari-bacseg-1.0.6/src/_dev/process_alex_datadump_clinical.py
+-rw-rw-rw-   0        0        0    28804 2023-02-24 14:19:52.000000 napari-bacseg-1.0.6/src/_dev/process_conor_datadump.py
+-rw-rw-rw-   0        0        0    30160 2023-02-24 14:19:52.000000 napari-bacseg-1.0.6/src/_dev/process_gramstain_datadump.py
+-rw-rw-rw-   0        0        0      576 2022-08-16 09:34:20.000000 napari-bacseg-1.0.6/src/_dev/read_non_tif.py
+-rw-rw-rw-   0        0        0     7794 2023-02-24 14:19:52.000000 napari-bacseg-1.0.6/src/_dev/rebuild_usermeta.py
+-rw-rw-rw-   0        0        0    10440 2023-02-24 14:19:52.000000 napari-bacseg-1.0.6/src/_dev/rebuild_usermeta_2.py
+-rw-rw-rw-   0        0        0     3034 2023-03-23 13:58:59.000000 napari-bacseg-1.0.6/src/_dev/recreate_user_metadata.py
+-rw-rw-rw-   0        0        0     2117 2023-04-20 14:14:30.000000 napari-bacseg-1.0.6/src/_dev/scalebar_dev.py
+-rw-rw-rw-   0        0        0    25122 2023-02-24 14:19:52.000000 napari-bacseg-1.0.6/src/_dev/sort_midlines.py
+-rw-rw-rw-   0        0        0     9633 2023-02-24 14:19:52.000000 napari-bacseg-1.0.6/src/_dev/stelios_stats.py
+-rw-rw-rw-   0        0        0      644 2023-02-24 14:19:52.000000 napari-bacseg-1.0.6/src/_dev/tile_meta_check.py
+-rw-rw-rw-   0        0        0     1615 2022-07-22 11:43:30.000000 napari-bacseg-1.0.6/src/_dev/tiler_dev.py
+-rw-rw-rw-   0        0        0     3064 2023-02-24 14:29:04.000000 napari-bacseg-1.0.6/src/_dev/updade_akseg_metadata.py
+-rw-rw-rw-   0        0        0     2057 2023-02-24 12:22:32.000000 napari-bacseg-1.0.6/src/_dev/update_img_metadata.py
+-rw-rw-rw-   0        0        0     6859 2023-02-24 14:19:52.000000 napari-bacseg-1.0.6/src/_dev/video_iamges.py
+-rw-rw-rw-   0        0        0     7767 2023-03-13 16:18:11.000000 napari-bacseg-1.0.6/src/_dev/zooniverse.py
+-rw-rw-rw-   0        0        0     5624 2023-02-24 14:21:12.000000 napari-bacseg-1.0.6/src/_dev/zooniverse_move.py
+-rw-rw-rw-   0        0        0     5742 2023-03-15 10:15:29.000000 napari-bacseg-1.0.6/src/_dev/zooniverse_move_titrations.py
+-rw-rw-rw-   0        0        0    30267 2023-03-13 16:29:04.000000 napari-bacseg-1.0.6/src/_dev/zooniverse_titration_upload.py
+-rw-rw-rw-   0        0        0     7503 2023-03-13 17:00:21.000000 napari-bacseg-1.0.6/src/_dev/zooniverse_titrations.py
+-rw-rw-rw-   0        0        0    30267 2023-03-13 16:09:34.000000 napari-bacseg-1.0.6/src/_dev/zooniverse_upload.py
+drwxrwxrwx   0        0        0        0 2023-05-06 06:44:33.544724 napari-bacseg-1.0.6/src/napari_bacseg/
+-rw-rw-rw-   0        0        0      155 2023-05-06 06:42:46.000000 napari-bacseg-1.0.6/src/napari_bacseg/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 06:44:33.571563 napari-bacseg-1.0.6/src/napari_bacseg/_tests/
+-rw-rw-rw-   0        0        0        0 2023-02-24 11:00:35.000000 napari-bacseg-1.0.6/src/napari_bacseg/_tests/__init__.py
+-rw-rw-rw-   0        0        0    26398 2023-05-03 08:53:54.000000 napari-bacseg-1.0.6/src/napari_bacseg/_tests/test_bacseg.py
+-rw-rw-rw-   0        0        0     1276 2023-02-27 13:15:54.000000 napari-bacseg-1.0.6/src/napari_bacseg/_tests/test_widget.py
+-rw-rw-rw-   0        0        0    88965 2023-05-06 06:32:34.000000 napari-bacseg-1.0.6/src/napari_bacseg/_utils.py
+-rw-rw-rw-   0        0        0    13550 2023-04-21 11:56:56.000000 napari-bacseg-1.0.6/src/napari_bacseg/_utils_cellpose.py
+-rw-rw-rw-   0        0        0    17465 2023-02-27 13:15:54.000000 napari-bacseg-1.0.6/src/napari_bacseg/_utils_colicoords.py
+-rw-rw-rw-   0        0        0    20495 2023-05-03 08:53:54.000000 napari-bacseg-1.0.6/src/napari_bacseg/_utils_database.py
+-rw-rw-rw-   0        0        0    46793 2023-05-06 06:37:46.000000 napari-bacseg-1.0.6/src/napari_bacseg/_utils_database_IO.py
+-rw-rw-rw-   0        0        0     1645 2023-03-09 18:16:07.000000 napari-bacseg-1.0.6/src/napari_bacseg/_utils_imagej.py
+-rw-rw-rw-   0        0        0    37022 2023-05-06 06:32:34.000000 napari-bacseg-1.0.6/src/napari_bacseg/_utils_interface_events.py
+-rw-rw-rw-   0        0        0     4279 2023-05-03 08:53:54.000000 napari-bacseg-1.0.6/src/napari_bacseg/_utils_json.py
+-rw-rw-rw-   0        0        0    34168 2023-03-07 17:38:57.000000 napari-bacseg-1.0.6/src/napari_bacseg/_utils_oufti.py
+-rw-rw-rw-   0        0        0     2132 2023-02-27 13:15:54.000000 napari-bacseg-1.0.6/src/napari_bacseg/_utils_refine.py
+-rw-rw-rw-   0        0        0    21190 2023-03-27 09:54:48.000000 napari-bacseg-1.0.6/src/napari_bacseg/_utils_statistics.py
+-rw-rw-rw-   0        0        0     7055 2023-02-27 13:15:54.000000 napari-bacseg-1.0.6/src/napari_bacseg/_utils_tiler.py
+-rw-rw-rw-   0        0        0      164 2023-05-06 06:44:32.000000 napari-bacseg-1.0.6/src/napari_bacseg/_version.py
+-rw-rw-rw-   0        0        0    79705 2023-05-06 06:34:35.000000 napari-bacseg-1.0.6/src/napari_bacseg/_widget.py
+-rw-rw-rw-   0        0        0   162470 2023-05-05 08:42:27.000000 napari-bacseg-1.0.6/src/napari_bacseg/bacseg_ui.py
+-rw-rw-rw-   0        0        0   160468 2023-05-05 08:42:22.000000 napari-bacseg-1.0.6/src/napari_bacseg/bacseg_ui.ui
+-rw-rw-rw-   0        0        0      271 2023-02-27 13:15:54.000000 napari-bacseg-1.0.6/src/napari_bacseg/gapseq_ui.py
+-rw-rw-rw-   0        0        0      501 2023-03-07 17:38:57.000000 napari-bacseg-1.0.6/src/napari_bacseg/napari.yaml
+-rw-rw-rw-   0        0        0      271 2023-02-27 13:15:54.000000 napari-bacseg-1.0.6/src/napari_bacseg/napari_ui.py
+drwxrwxrwx   0        0        0        0 2023-05-06 06:44:33.561589 napari-bacseg-1.0.6/src/napari_bacseg.egg-info/
+-rw-rw-rw-   0        0        0     4732 2023-05-06 06:44:32.000000 napari-bacseg-1.0.6/src/napari_bacseg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3271 2023-05-06 06:44:33.000000 napari-bacseg-1.0.6/src/napari_bacseg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 06:44:32.000000 napari-bacseg-1.0.6/src/napari_bacseg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2023-05-06 06:44:32.000000 napari-bacseg-1.0.6/src/napari_bacseg.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      352 2023-05-06 06:44:32.000000 napari-bacseg-1.0.6/src/napari_bacseg.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-05-06 06:44:32.000000 napari-bacseg-1.0.6/src/napari_bacseg.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      644 2023-02-24 11:00:35.000000 napari-bacseg-1.0.6/tox.ini
```

### Comparing `napari-bacseg-1.0.5/.github/workflows/test_and_deploy.yml` & `napari-bacseg-1.0.6/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.5/.gitignore` & `napari-bacseg-1.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.5/.napari-hub/config.yml` & `napari-bacseg-1.0.6/.napari-hub/config.yml`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.5/.pre-commit-config.yaml` & `napari-bacseg-1.0.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.5/LICENSE` & `napari-bacseg-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.5/PKG-INFO` & `napari-bacseg-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-bacseg
-Version: 1.0.5
+Version: 1.0.6
 Summary: Bacterial segmentation and analysis platform than can inport/export files in multiple formats. Integrating many tools such as Cellpose, ColiCoords, Oufti/MicrobeTracker.
 Home-page: https://github.com/piedrro/napari-bacseg
 Author: Piers Turner
 Author-email: Piers Turner <piers.turner@physics.ox.ac.uk>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/piedrro/napari-bacseg
 Project-URL: Bug Tracker, https://github.com/piedrro/napari-bacseg/issues
```

### Comparing `napari-bacseg-1.0.5/README.md` & `napari-bacseg-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.5/pyproject.toml` & `napari-bacseg-1.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 [tool.isort]
 profile = "black"
 line_length = 79
 
 [project]
 name = "napari-bacseg"
-version = "1.0.5"
+version = "1.0.6"
 authors = [
   { name="Piers Turner", email="piers.turner@physics.ox.ac.uk"},
 ]
 description = "Bacterial segmentation and analysis platform than can inport/export files in multiple formats. Integrating many tools such as Cellpose, ColiCoords, Oufti/MicrobeTracker."
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `napari-bacseg-1.0.5/setup.cfg` & `napari-bacseg-1.0.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.5/src/_dev/Export Masks to AKSEG v5 dev.py` & `napari-bacseg-1.0.6/src/_dev/Export Masks to AKSEG v5 dev.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.5/src/_dev/ScanR dev.py` & `napari-bacseg-1.0.6/src/_dev/ScanR dev.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.5/src/_dev/akseg_db_stats.py` & `napari-bacseg-1.0.6/src/_dev/akseg_db_stats.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.5/src/_dev/akseg_dev.py` & `napari-bacseg-1.0.6/src/_dev/akseg_dev.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.5/src/_dev/akseg_dev2.py` & `napari-bacseg-1.0.6/src/_dev/akseg_dev2.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.5/src/_dev/akseg_txt_metadata.py` & `napari-bacseg-1.0.6/src/_dev/akseg_txt_metadata.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.5/src/_dev/align_alex_datadump.py` & `napari-bacseg-1.0.6/src/_dev/align_alex_datadump.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.5/src/_dev/alison_datadump.py` & `napari-bacseg-1.0.6/src/_dev/alison_datadump.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.5/src/_dev/autocontast_dev.py` & `napari-bacseg-1.0.6/src/_dev/autocontast_dev.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.5/src/_dev/chatGPT_midlines.py` & `napari-bacseg-1.0.6/src/_dev/chatGPT_midlines.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.5/src/_dev/check_AluGasketv12_DFP.py` & `napari-bacseg-1.0.6/src/_dev/check_AluGasketv12_DFP.py`

 * *Files 24% similar despite different names*

```diff
@@ -25,14 +25,19 @@
 import tqdm
 import traceback
 from functools import partial
 import matplotlib.pyplot as plt
 
 
 
+metadata_columns = ["date_uploaded", "date_created", "date_modified", "file_name", "channel", "file_list", "channel_list", "segmentation_file", "segmentation_channel", "akseg_hash",
+    "user_initial", "content", "microscope", "modality", "source", "strain", "phenotype", "stain_target", "antibiotic", "treatment time (mins)", "antibiotic concentration", "mounting method", "protocol",
+    "folder", "parent_folder", "num_segmentations", "image_laplacian", "image_focus","image_debris","segmented", "labelled", "segmentation_curated", "label_curated", "posX", "posY", "posZ",
+    "image_load_path", "image_save_path", "mask_load_path", "mask_save_path", "label_load_path", "label_save_path"]
+
 def fix_strain_phenotype(dat):
     
     folder = dat["folder"]
     antibiotic = dat["antibiotic"]
     
     strain = folder.split("_")[2]
 
@@ -78,18 +83,37 @@
     total_cell_count = cell_count["num_segmentations"].sum()
     
     return cell_count, total_cell_count
 
 
 
 
-user_initial = "AF"
+user_initial = "CF"
 
 user_metadata_path = os.path.join(r"\\physics\dfs\DAQ\CondensedMatterGroups\AKGroup\Piers\AKSEG\Images", user_initial, f"{user_initial}_file_metadata.txt")
-user_metadata = pd.read_csv(user_metadata_path, sep="\t", low_memory=False)
+user_metadata = pd.read_csv(user_metadata_path, sep=",", low_memory=False)
+
+# user_metadata["treatment time (mins)"] = user_metadata["treatment time (mins)"].apply(pd.to_numeric(errors='ignore', downcast='float'))
+
+user_metadata[["treatment time (mins)"]] = user_metadata[["treatment time (mins)"]].apply(pd.to_numeric, downcast="float")
+user_metadata["treatment time (mins)"] = user_metadata["treatment time (mins)"].astype(str)
+
+
+user_metadata = user_metadata[user_metadata["user_meta1"] == "Direct From Plate 100X Titration"]
+
+user_metadata.loc[user_metadata["antibiotic"].isin(["None",None, np.nan]), "antibiotic"] = "None"
+user_metadata.loc[user_metadata["antibiotic"].isin(["None",None, np.nan]), "phenotype"] = "Untreated"
+
+phenotype_data = user_metadata[["user_meta1","user_meta2","user_meta3","strain","antibiotic","antibiotic concentration","treatment time (mins)","phenotype"]].drop_duplicates()
+phenotype_data = phenotype_data.sort_values(["strain","antibiotic","treatment time (mins)","antibiotic concentration",])
+
+for col in phenotype_data.columns:
+    values = list(phenotype_data[col].unique())
+    print(col, values)
+
 
 # print(user_metadata.columns.tolist())
 
 
 # xx = user_metadata.to_dict("records")
```

### Comparing `napari-bacseg-1.0.5/src/_dev/check_metadata.py` & `napari-bacseg-1.0.6/src/_dev/check_metadata.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.5/src/_dev/colicoords_cellldist_dev.py` & `napari-bacseg-1.0.6/src/_dev/colicoords_cellldist_dev.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.5/src/_dev/colicoords_ldist_dev.py` & `napari-bacseg-1.0.6/src/_dev/colicoords_ldist_dev.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.5/src/_dev/database_dev.py` & `napari-bacseg-1.0.6/src/_dev/database_dev.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.5/src/_dev/deepsegmattest.py` & `napari-bacseg-1.0.6/src/_dev/deepsegmattest.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.5/src/_dev/edit_database_columns.py` & `napari-bacseg-1.0.6/src/_dev/edit_database_columns.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.5/src/_dev/fits_dev.py` & `napari-bacseg-1.0.6/src/_dev/fits_dev.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.5/src/_dev/fix_alison_missing_file_list.py` & `napari-bacseg-1.0.6/src/_dev/fix_alison_missing_file_list.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.5/src/_dev/generate_scanr_movie.py` & `napari-bacseg-1.0.6/src/_dev/generate_scanr_movie.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.5/src/_dev/get_akseg_stats.py` & `napari-bacseg-1.0.6/src/_dev/get_akseg_stats.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.5/src/_dev/get_species_info.py` & `napari-bacseg-1.0.6/src/_dev/get_species_info.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.5/src/_dev/luke__script.py` & `napari-bacseg-1.0.6/src/_dev/luke__script.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.5/src/_dev/matplotlib_Events.py` & `napari-bacseg-1.0.6/src/_dev/matplotlib_Events.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.5/src/_dev/move_AluGasketDFP.py` & `napari-bacseg-1.0.6/src/_dev/move_AluGasketDFP.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.5/src/_dev/move_AluGasketDFP_poster.py` & `napari-bacseg-1.0.6/src/_dev/move_AluGasketDFP_poster.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.5/src/_dev/move_AluGasketv12_DFP.py` & `napari-bacseg-1.0.6/src/_dev/move_AluGasketv12_DFP.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.5/src/_dev/move_conor_nim_dfp_data.py` & `napari-bacseg-1.0.6/src/_dev/move_conor_nim_dfp_data.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.5/src/_dev/move_pillar_data.py` & `napari-bacseg-1.0.6/src/_dev/move_pillar_data.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.5/src/_dev/move_pillar_zstack_data.py` & `napari-bacseg-1.0.6/src/_dev/move_pillar_zstack_data.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.5/src/_dev/move_unlearning_files.py` & `napari-bacseg-1.0.6/src/_dev/move_unlearning_files.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.5/src/_dev/new_metadata2.pickle.py` & `napari-bacseg-1.0.6/src/_dev/new_metadata2.pickle.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.5/src/_dev/new_read_akseg_directory.py` & `napari-bacseg-1.0.6/src/_dev/new_read_akseg_directory.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.5/src/_dev/nim_dev.py` & `napari-bacseg-1.0.6/src/_dev/nim_dev.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.5/src/_dev/omnipose_dev.py` & `napari-bacseg-1.0.6/src/_dev/omnipose_dev.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.5/src/_dev/omnipose_midlines.py` & `napari-bacseg-1.0.6/src/_dev/omnipose_midlines.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.5/src/_dev/omnipose_train.py` & `napari-bacseg-1.0.6/src/_dev/omnipose_train.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.5/src/_dev/oufti_dilate.py` & `napari-bacseg-1.0.6/src/_dev/oufti_dilate.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.5/src/_dev/oufti_dilate_with_midlines.py` & `napari-bacseg-1.0.6/src/_dev/oufti_dilate_with_midlines.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.5/src/_dev/process_alex_datadump.py` & `napari-bacseg-1.0.6/src/_dev/process_alex_datadump.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.5/src/_dev/process_alex_datadump_clinical.py` & `napari-bacseg-1.0.6/src/_dev/process_alex_datadump_clinical.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.5/src/_dev/process_conor_datadump.py` & `napari-bacseg-1.0.6/src/_dev/process_conor_datadump.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.5/src/_dev/process_gramstain_datadump.py` & `napari-bacseg-1.0.6/src/_dev/process_gramstain_datadump.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.5/src/_dev/read_non_tif.py` & `napari-bacseg-1.0.6/src/_dev/read_non_tif.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.5/src/_dev/rebuild_usermeta.py` & `napari-bacseg-1.0.6/src/_dev/rebuild_usermeta.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.5/src/_dev/rebuild_usermeta_2.py` & `napari-bacseg-1.0.6/src/_dev/rebuild_usermeta_2.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.5/src/_dev/recreate_user_metadata.py` & `napari-bacseg-1.0.6/src/_dev/recreate_user_metadata.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.5/src/_dev/scalebar_dev.py` & `napari-bacseg-1.0.6/src/_dev/scalebar_dev.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.5/src/_dev/sort_midlines.py` & `napari-bacseg-1.0.6/src/_dev/sort_midlines.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.5/src/_dev/stelios_stats.py` & `napari-bacseg-1.0.6/src/_dev/stelios_stats.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.5/src/_dev/tile_meta_check.py` & `napari-bacseg-1.0.6/src/_dev/tile_meta_check.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.5/src/_dev/tiler_dev.py` & `napari-bacseg-1.0.6/src/_dev/tiler_dev.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.5/src/_dev/updade_akseg_metadata.py` & `napari-bacseg-1.0.6/src/_dev/updade_akseg_metadata.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.5/src/_dev/update_img_metadata.py` & `napari-bacseg-1.0.6/src/_dev/update_img_metadata.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.5/src/_dev/video_iamges.py` & `napari-bacseg-1.0.6/src/_dev/video_iamges.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.5/src/_dev/zooniverse.py` & `napari-bacseg-1.0.6/src/_dev/zooniverse.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.5/src/_dev/zooniverse_move.py` & `napari-bacseg-1.0.6/src/_dev/zooniverse_move.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.5/src/_dev/zooniverse_move_titrations.py` & `napari-bacseg-1.0.6/src/_dev/zooniverse_move_titrations.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.5/src/_dev/zooniverse_titration_upload.py` & `napari-bacseg-1.0.6/src/_dev/zooniverse_titration_upload.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.5/src/_dev/zooniverse_titrations.py` & `napari-bacseg-1.0.6/src/_dev/zooniverse_titrations.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.5/src/_dev/zooniverse_upload.py` & `napari-bacseg-1.0.6/src/_dev/zooniverse_upload.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.5/src/napari_bacseg/_tests/test_bacseg.py` & `napari-bacseg-1.0.6/src/napari_bacseg/_tests/test_bacseg.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.5/src/napari_bacseg/_tests/test_widget.py` & `napari-bacseg-1.0.6/src/napari_bacseg/_tests/test_widget.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.5/src/napari_bacseg/_utils.py` & `napari-bacseg-1.0.6/src/napari_bacseg/_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -2341,16 +2341,14 @@
                     pixel_resolution_units=pixel_resolution_units,
                     scalebar_size=scalebar_size,
                     scalebar_size_units=scalebar_size_units,
                     scalebar_colour=scalebar_colour,
                     scalebar_thickness=scalebar_thickness,
                 )
 
-                print(True)
-
             image.append(blank)
 
     if mode == "rgb":
         image = np.stack(image, axis=-1)
 
         image = rescale01(image)
         image = image * (2**16 - 1)
```

### Comparing `napari-bacseg-1.0.5/src/napari_bacseg/_utils_cellpose.py` & `napari-bacseg-1.0.6/src/napari_bacseg/_utils_cellpose.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.5/src/napari_bacseg/_utils_colicoords.py` & `napari-bacseg-1.0.6/src/napari_bacseg/_utils_colicoords.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.5/src/napari_bacseg/_utils_database.py` & `napari-bacseg-1.0.6/src/napari_bacseg/_utils_database.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.5/src/napari_bacseg/_utils_database_IO.py` & `napari-bacseg-1.0.6/src/napari_bacseg/_utils_database_IO.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,44 +15,28 @@
 import tifffile
 from napari.utils.notifications import show_info
 
 from napari_bacseg._utils_json import export_coco_json, import_coco_json
 
 
 def check_metadata_format(metadata, expected_columns):
-    missing_columns = list(
-        set(expected_columns) - set(metadata.columns.tolist())
-    )
-    extra_columns = list(
-        set(metadata.columns.tolist()) - set(expected_columns)
-    )
+    missing_columns = list(set(expected_columns) - set(metadata.columns.tolist()))
+    extra_columns = list(set(metadata.columns.tolist()) - set(expected_columns))
 
     all_columns = list(set(expected_columns + extra_columns))
 
-    metadata[missing_columns] = pd.DataFrame(
-        [[None] * len(missing_columns)], index=metadata.index
-    )
+    metadata[missing_columns] = pd.DataFrame([[None] * len(missing_columns)], index=metadata.index)
 
     date = datetime.datetime.now()
 
-    metadata.loc[
-        metadata["date_uploaded"].isin(["None", None, np.nan, 0]),
-        ["date_uploaded", "date_created", "date_modified"],
-    ] = str(date)
+    metadata.loc[metadata["date_uploaded"].isin(["None", None, np.nan, 0]), ["date_uploaded", "date_created", "date_modified"],] = str(date)
 
     metadata = metadata[all_columns]
 
-    metadata = metadata.astype(
-        {
-            "segmented": bool,
-            "labelled": bool,
-            "segmentation_curated": bool,
-            "label_curated": bool,
-        }
-    )
+    metadata = metadata.astype({"segmented": bool, "labelled": bool, "segmentation_curated": bool, "label_curated": bool, })
 
     return metadata, all_columns
 
 
 def get_meta_value(meta, value):
     if value in meta.keys():
         data = meta[value]
@@ -80,27 +64,25 @@
 
     if import_limit == "All":
         import_limit = len(measurements)
     else:
         if int(import_limit) > len(measurements):
             import_limit = len(measurements)
 
+    show_info(f"Downloading {len(measurements)} files.")
+
     if import_limit == str(1):
         try:
             measurement = measurements.get_group(list(measurements.groups)[0])
-            imported_data = [
-                download_bacseg_files(measurement, channels, database_path)
-            ]
+            imported_data = [download_bacseg_files(measurement, channels, database_path)]
             progress_callback.emit(100)
         except:
             pass
     else:
-        measurements = [
-            measurements.get_group(i) for i in measurements.groups
-        ][: int(import_limit)]
+        measurements = [measurements.get_group(i) for i in measurements.groups][: int(import_limit)]
         with Pool(4) as pool:
             iter = []
 
             def callback(*args):
                 iter.append(1)
                 progress = (len(iter) / int(import_limit)) * 100
 
@@ -108,22 +90,15 @@
                     try:
                         progress_callback.emit(progress)
                     except:
                         pass
 
                 return
 
-            results = [
-                pool.apply_async(
-                    download_bacseg_files,
-                    args=(measurement, channels, database_path),
-                    callback=callback,
-                )
-                for measurement in measurements
-            ]
+            results = [pool.apply_async(download_bacseg_files, args=(measurement, channels, database_path), callback=callback, ) for measurement in measurements]
 
             try:
                 results[-1].get()
             except:
                 print(traceback.format_exc())
             else:
                 results = [r.get() for r in results]
@@ -138,20 +113,15 @@
             for channel, channel_data in dat.items():
                 image = channel_data["images"]
                 mask = channel_data["masks"]
                 label = channel_data["classes"]
                 meta = channel_data["metadata"]
 
                 if channel not in imported_images.keys():
-                    imported_images[channel] = dict(
-                        images=[image],
-                        masks=[mask],
-                        classes=[label],
-                        metadata={0: meta},
-                    )
+                    imported_images[channel] = dict(images=[image], masks=[mask], classes=[label], metadata={0: meta}, )
                 else:
                     image_index = len(imported_images[channel]["images"])
 
                     imported_images[channel]["images"].append(image)
                     imported_images[channel]["masks"].append(mask)
                     imported_images[channel]["classes"].append(label)
                     imported_images[channel]["metadata"][image_index] = meta
@@ -194,40 +164,25 @@
     if self.upload_label_combo.currentIndex() == 2:
         labelled = True
         labelled_curated = False
     if self.upload_label_combo.currentIndex() == 3:
         labelled = True
         labelled_curated = True
 
-    metadata = dict(
-        user_initial=user_initial,
-        content=content,
-        microscope=microscope,
-        antibiotic=antibiotic,
-        abxconcentration=abxconcentration,
-        treatmenttime=treatmenttime,
-        mount=mount,
-        protocol=protocol,
-        strain=strain,
-        phenotype=phenotype,
-    )
+    metadata = dict(user_initial=user_initial, content=content, microscope=microscope, antibiotic=antibiotic, abxconcentration=abxconcentration, treatmenttime=treatmenttime, mount=mount, protocol=protocol, strain=strain, phenotype=phenotype, )
 
     num_user_keys = self.user_metadata_keys
 
     for key in range(1, num_user_keys + 1):
         control_name = f"upload_usermeta{key}"
         combo_box = getattr(self, control_name)
         combo_box_value = combo_box.currentText()
         metadata[f"usermeta{key}"] = combo_box_value
 
-    layer_names = [
-        layer.name
-        for layer in self.viewer.layers
-        if layer.name not in ["Segmentations", "Classes", "center_lines"]
-    ]
+    layer_names = [layer.name for layer in self.viewer.layers if layer.name not in ["Segmentations", "Classes", "center_lines"]]
 
     layer_names.reverse()
 
     # put segmentation channel as first channel in stack
     segChannel = self.cellpose_segchannel.currentText()
     layer_names.remove(segChannel)
     layer_names.insert(0, segChannel)
@@ -241,33 +196,28 @@
         rgb_images = []
         rgb_meta = {}
         file_list = []
         layer_list = []
 
         try:
             for j in range(len(layer_names)):
-                segmentation_file = self.viewer.layers[segChannel].metadata[i][
-                    "image_name"
-                ]
+                segmentation_file = self.viewer.layers[segChannel].metadata[i]["image_name"]
 
                 layer = str(layer_names[j])
 
                 img = self.viewer.layers[layer].data[i]
                 meta = self.viewer.layers[layer].metadata[i]
 
                 if meta["image_name"] != "missing image channel":
                     file_list.append(meta["image_name"])
                     layer_list.append(layer)
 
                     meta["user_initial"] = user_initial
 
-                    if (
-                        meta["import_mode"] != "BacSeg"
-                        or overwrite_all_metadata is True
-                    ):
+                    if (meta["import_mode"] != "BacSeg" or overwrite_all_metadata is True):
                         meta["microscope"] = microscope
                         meta["image_content"] = content
                         meta["antibiotic"] = antibiotic
                         meta["strain"] = strain
                         meta["phenotype"] = phenotype
                         meta["treatmenttime"] = treatmenttime
                         meta["abxconcentration"] = abxconcentration
@@ -277,69 +227,40 @@
                         meta["segmentation_channel"] = segChannel
                         meta["file_list"] = []
                         meta["layer_list"] = []
                         meta["segmentation_file"] = segmentation_file
 
                         for key in range(1, num_user_keys + 1):
                             meta[f"usermeta{key}"] = metadata[f"usermeta{key}"]
-                            print(
-                                meta[f"usermeta{key}"],
-                                metadata[f"usermeta{key}"],
-                            )
-
-                    if (
-                        meta["import_mode"] == "BacSeg"
-                        and overwrite_all_metadata is True
-                    ):
-                        metadata = {
-                            key: val
-                            for key, val in metadata.items()
-                            if val != "Required for upload"
-                        }
+
+                    if (meta["import_mode"] == "BacSeg" and overwrite_all_metadata is True):
+                        metadata = {key: val for key, val in metadata.items() if val != "Required for upload"}
 
                         for key, value in metadata.items():
                             meta[key] = value
 
                     if overwrite_selected_metadata is True:
-                        metadata = {
-                            key: val
-                            for key, val in metadata.items()
-                            if val not in ["", "Required for upload"]
-                        }
+                        metadata = {key: val for key, val in metadata.items() if val not in ["", "Required for upload"]}
 
                         for key, value in metadata.items():
                             meta[key] = value
 
                     meta["segmented"] = segmented
                     meta["labelled"] = labelled
                     meta["segmentations_curated"] = segmented_curated
                     meta["labels_curated"] = labelled_curated
 
                     if self.cellpose_segmentation == True:
-                        meta[
-                            "cellpose_segmentation"
-                        ] = self.cellpose_segmentation
-                        meta["flow_threshold"] = float(
-                            self.cellpose_flowthresh_label.text()
-                        )
-                        meta["mask_threshold"] = float(
-                            self.cellpose_maskthresh_label.text()
-                        )
-                        meta["min_size"] = int(
-                            self.cellpose_minsize_label.text()
-                        )
-                        meta["diameter"] = int(
-                            self.cellpose_diameter_label.text()
-                        )
-                        meta[
-                            "cellpose_model"
-                        ] = self.cellpose_segmodel.currentText()
-                        meta["custom_model"] = os.path.abspath(
-                            self.cellpose_custom_model_path
-                        )
+                        meta["cellpose_segmentation"] = self.cellpose_segmentation
+                        meta["flow_threshold"] = float(self.cellpose_flowthresh_label.text())
+                        meta["mask_threshold"] = float(self.cellpose_maskthresh_label.text())
+                        meta["min_size"] = int(self.cellpose_minsize_label.text())
+                        meta["diameter"] = int(self.cellpose_diameter_label.text())
+                        meta["cellpose_model"] = self.cellpose_segmodel.currentText()
+                        meta["custom_model"] = os.path.abspath(self.cellpose_custom_model_path)
 
                     rgb_images.append(img)
                     rgb_meta[layer] = meta
 
             for layer in layer_names:
                 if layer in rgb_meta.keys():
                     rgb_meta[layer]["file_list"] = file_list
@@ -359,32 +280,19 @@
 
 def download_bacseg_files(measurement, channels, database_path):
     imported_images = {}
 
     try:
         segmentation_channel = measurement["segmentation_channel"].unique()[0]
 
-        segmentation_file = measurement[
-            measurement["channel"] == segmentation_channel
-        ]["file_name"].item()
-        user_initial = measurement[
-            measurement["channel"] == segmentation_channel
-        ]["user_initial"].item()
-        folder = measurement[measurement["channel"] == segmentation_channel][
-            "folder"
-        ].item()
-
-        json_path = os.path.join(
-            database_path,
-            "Images",
-            user_initial,
-            "json",
-            folder,
-            segmentation_file,
-        )
+        segmentation_file = measurement[measurement["channel"] == segmentation_channel]["file_name"].item()
+        user_initial = measurement[measurement["channel"] == segmentation_channel]["user_initial"].item()
+        folder = measurement[measurement["channel"] == segmentation_channel]["folder"].item()
+
+        json_path = os.path.join(database_path, "Images", user_initial, "json", folder, segmentation_file, )
 
         mask, label = import_coco_json(json_path)
 
         for j in range(len(channels)):
             channel = channels[j]
 
             measurement_channels = measurement["channel"].unique()
@@ -392,22 +300,15 @@
             if channel in measurement_channels:
                 dat = measurement[measurement["channel"] == channel]
 
                 file_name = dat["file_name"].item()
                 user_initial = dat["user_initial"].item()
                 folder = dat["folder"].item()
 
-                image_path = os.path.join(
-                    database_path,
-                    "Images",
-                    user_initial,
-                    "images",
-                    folder,
-                    file_name,
-                )
+                image_path = os.path.join(database_path, "Images", user_initial, "images", folder, file_name, )
                 image_path = os.path.abspath(image_path)
 
                 image = tifffile.imread(image_path)
 
                 with tifffile.TiffFile(image_path) as tif:
                     try:
                         meta = tif.pages[0].tags["ImageDescription"].value
@@ -418,20 +319,16 @@
                 meta["import_mode"] = "BacSeg"
 
                 for key, value in dat.to_dict("records")[0].items():
                     meta[key] = value
 
                 if "segmentation_file" in meta.keys():
                     if meta["segmentation_file"] in [None, "None"]:
-                        meta["segmentation_file"] = list_from_string(
-                            measurement["file_list"].iloc[0]
-                        )[0]
-                        meta["segmentation_channel"] = list_from_string(
-                            measurement["channel_list"].iloc[0]
-                        )[0]
+                        meta["segmentation_file"] = list_from_string(measurement["file_list"].iloc[0])[0]
+                        meta["segmentation_channel"] = list_from_string(measurement["channel_list"].iloc[0])[0]
 
             else:
                 image = np.zeros((100, 100), dtype=np.uint16)
                 mask = np.zeros((100, 100), dtype=np.uint16)
                 label = np.zeros((100, 100), dtype=np.uint16)
 
                 meta = {}
@@ -447,17 +344,15 @@
                 meta["contrast_alpha"] = None
                 meta["contrast_beta"] = None
                 meta["contrast_gamma"] = None
                 meta["dims"] = [image.shape[-1], image.shape[-2]]
                 meta["crop"] = [0, image.shape[-2], 0, image.shape[-1]]
                 meta["light_source"] = channel
 
-            imported_images[channel] = dict(
-                images=image, masks=mask, classes=label, metadata=meta
-            )
+            imported_images[channel] = dict(images=image, masks=mask, classes=label, metadata=meta)
 
     except:
         pass
 
     return imported_images
 
 
@@ -512,257 +407,131 @@
             elif "StagePos_um" in meta.keys():
                 posX, posY, posZ = meta["StagePos_um"]
             else:
                 posX, posY, posZ = 0, 0, 0
 
             if file_name in metadata_file_names:
                 try:
-                    date_uploaded = user_metadata[
-                        (user_metadata["file_name"] == file_name)
-                        & (user_metadata["folder"] == folder)
-                    ]["date_uploaded"].item()
+                    date_uploaded = user_metadata[(user_metadata["file_name"] == file_name) & (user_metadata["folder"] == folder)]["date_uploaded"].item()
                 except:
                     date_uploaded = datetime.datetime.now()
             else:
                 date_uploaded = datetime.datetime.now()
 
             if "date_created" in meta.keys():
                 date_created = meta["date_created"]
             elif file_name in metadata_file_names:
                 try:
-                    date_created = user_metadata[
-                        (user_metadata["file_name"] == file_name)
-                        & (user_metadata["folder"] == folder)
-                    ]["date_created"].item()
+                    date_created = user_metadata[(user_metadata["file_name"] == file_name) & (user_metadata["folder"] == folder)]["date_created"].item()
                 except:
                     date_created = datetime.datetime.now()
             else:
                 date_created = datetime.datetime.now()
 
             date_modified = datetime.datetime.now()
 
             # stops user from overwriting BacSeg files, unless they have opened them from BacSeg for curation
-            if (
-                akseg_hash in metadata_akseg_hash
-                and import_mode != "BacSeg"
-                and overwrite_images == False
-                and overwrite_masks == False
-                and overwrite_metadata is False
-            ):
+            if (akseg_hash in metadata_akseg_hash and import_mode != "BacSeg" and overwrite_images == False and overwrite_masks == False and overwrite_metadata is False):
                 if widget_notifications:
-                    show_info(
-                        "file already exists  in BacSeg Database:   "
-                        + file_name
-                    )
+                    show_info("file already exists  in BacSeg Database:   " + file_name)
 
                 file_metadata = None
 
             else:
                 if import_mode == "BacSeg":
                     if overwrite_selected_metadata is True:
                         if widget_notifications:
-                            show_info(
-                                "Overwriting selected metadata on BacSeg Database:   "
-                                + file_name
-                            )
+                            show_info("Overwriting selected metadata on BacSeg Database:   " + file_name)
 
                     elif overwrite_all_metadata is True:
                         if widget_notifications:
-                            show_info(
-                                "Overwriting all metadata on BacSeg Database:   "
-                                + file_name
-                            )
+                            show_info("Overwriting all metadata on BacSeg Database:   " + file_name)
 
                     else:
                         if widget_notifications:
-                            show_info(
-                                "Editing file on BacSeg Database:   "
-                                + file_name
-                            )
+                            show_info("Editing file on BacSeg Database:   " + file_name)
 
                 elif overwrite_images is True and overwrite_masks is True:
                     if widget_notifications:
-                        show_info(
-                            "Overwriting image + mask/label on BacSeg Database:   "
-                            + file_name
-                        )
+                        show_info("Overwriting image + mask/label on BacSeg Database:   " + file_name)
 
                 elif overwrite_images is True:
                     if widget_notifications:
-                        show_info(
-                            "Overwriting image on BacSeg Database:   "
-                            + file_name
-                        )
+                        show_info("Overwriting image on BacSeg Database:   " + file_name)
 
                 elif overwrite_masks is True:
                     if widget_notifications:
-                        show_info(
-                            "Overwriting mask/label on BacSeg Database:   "
-                            + file_name
-                        )
+                        show_info("Overwriting mask/label on BacSeg Database:   " + file_name)
 
                 else:
                     if widget_notifications:
-                        show_info(
-                            "Uploading file to BacSeg Database:   " + file_name
-                        )
+                        show_info("Uploading file to BacSeg Database:   " + file_name)
 
                 y1, y2, x1, x2 = meta["crop"]
 
                 if len(img.shape) > 2:
                     img = img[:, y1:y2, x1:x2]
                 else:
                     img = img[y1:y2, x1:x2]
 
                 mask = mask[y1:y2, x1:x2]
                 class_mask = class_mask[y1:y2, x1:x2]
 
                 unique_segmentations = np.unique(mask)
-                unique_segmentations = np.delete(
-                    unique_segmentations, np.where(unique_segmentations == 0)
-                )
+                unique_segmentations = np.delete(unique_segmentations, np.where(unique_segmentations == 0))
 
                 num_segmentations = len(unique_segmentations)
                 image_laplacian = cv2.Laplacian(img, cv2.CV_64F).var()
 
                 meta.pop("shape", None)
 
                 file_name = os.path.splitext(meta["image_name"])[0] + ".tif"
 
                 image_path = os.path.join(image_dir, file_name)
                 mask_path = os.path.join(mask_dir, file_name)
-                json_path = os.path.join(
-                    json_dir, file_name.replace(".tif", ".txt")
-                )
+                json_path = os.path.join(json_dir, file_name.replace(".tif", ".txt"))
                 class_path = os.path.join(class_dir, file_name)
 
                 segmentation_file = get_meta_value(meta, "segmentation_file")
 
                 if segmentation_file is None:
                     segmentation_channel = channel_list[0]
-                    segmentation_file = image_meta[segmentation_channel][
-                        "image_name"
-                    ]
+                    segmentation_file = image_meta[segmentation_channel]["image_name"]
                     meta["segmentation_file"] = segmentation_file
                     meta["segmentation_channel"] = segmentation_channel
 
                 if upload_images is True:
-                    if (
-                        os.path.isfile(image_path) is False
-                        or import_mode == "BacSeg"
-                        or overwrite_images is True
-                        or overwrite_metadata is True
-                    ):
-                        tifffile.imwrite(
-                            os.path.abspath(image_path), img, metadata=meta
-                        )
+                    if (os.path.isfile(image_path) is False or import_mode == "BacSeg" or overwrite_images is True or overwrite_metadata is True):
+                        tifffile.imwrite(os.path.abspath(image_path), img, metadata=meta)
 
                 if upload_segmentations is True:
-                    if (
-                        os.path.isfile(mask_path) is False
-                        or import_mode == "BacSeg"
-                        or overwrite_masks is True
-                        or overwrite_metadata is True
-                    ):
+                    if (os.path.isfile(mask_path) is False or import_mode == "BacSeg" or overwrite_masks is True or overwrite_metadata is True):
                         if file_name == segmentation_file:
-                            export_coco_json(
-                                file_name, img, mask, class_mask, json_path
-                            )
+                            export_coco_json(file_name, img, mask, class_mask, json_path)
 
                 if "mask_path" not in meta.keys():
                     meta["mask_path"] = None
                 if "label_path" not in meta.keys():
                     meta["label_path"] = None
 
-                file_metadata = {
-                    "date_uploaded": date_uploaded,
-                    "date_created": date_created,
-                    "date_modified": date_modified,
-                    "file_name": file_name,
-                    "channel": get_meta_value(meta, "channel"),
-                    "file_list": get_meta_value(meta, "file_list"),
-                    "channel_list": get_meta_value(meta, "channel_list"),
-                    "segmentation_file": get_meta_value(
-                        meta, "segmentation_file"
-                    ),
-                    "segmentation_channel": get_meta_value(
-                        meta, "segmentation_channel"
-                    ),
-                    "strain": get_meta_value(meta, "strain"),
-                    "phenotype": get_meta_value(meta, "phenotype"),
-                    "akseg_hash": get_meta_value(meta, "akseg_hash"),
-                    "user_initial": get_meta_value(meta, "user_initial"),
-                    "content": get_meta_value(meta, "image_content"),
-                    "microscope": get_meta_value(meta, "microscope"),
-                    "modality": get_meta_value(meta, "modality"),
-                    "source": get_meta_value(meta, "light_source"),
-                    "stain": get_meta_value(meta, "stain"),
-                    "stain_target": get_meta_value(meta, "stain_target"),
-                    "antibiotic": get_meta_value(meta, "antibiotic"),
-                    "treatment time (mins)": get_meta_value(
-                        meta, "treatmenttime"
-                    ),
-                    "antibiotic concentration": get_meta_value(
-                        meta, "abxconcentration"
-                    ),
-                    "mounting method": get_meta_value(meta, "mount"),
-                    "protocol": get_meta_value(meta, "protocol"),
-                    "folder": get_meta_value(meta, "folder"),
-                    "parent_folder": get_meta_value(meta, "parent_folder"),
-                    "num_segmentations": num_segmentations,
-                    "image_laplacian": image_laplacian,
-                    "image_focus": get_meta_value(meta, "image_focus"),
-                    "image_debris": get_meta_value(meta, "image_debris"),
-                    "segmented": get_meta_value(meta, "segmented"),
-                    "labelled": get_meta_value(meta, "labelled"),
-                    "segmentation_curated": get_meta_value(
-                        meta, "segmentations_curated"
-                    ),
-                    "label_curated": get_meta_value(meta, "labels_curated"),
-                    "posX": posX,
-                    "posY": posY,
-                    "posZ": posZ,
-                    "image_load_path": get_meta_value(meta, "image_path"),
-                    "image_save_path": image_path,
-                    "mask_load_path": get_meta_value(meta, "mask_path"),
-                    "mask_save_path": mask_path,
-                    "label_load_path": get_meta_value(meta, "label_path"),
-                    "label_save_path": class_path,
-                }
+                file_metadata = {"date_uploaded": date_uploaded, "date_created": date_created, "date_modified": date_modified, "file_name": file_name, "channel": get_meta_value(meta, "channel"), "file_list": get_meta_value(meta, "file_list"), "channel_list": get_meta_value(meta, "channel_list"), "segmentation_file": get_meta_value(meta, "segmentation_file"), "segmentation_channel": get_meta_value(meta, "segmentation_channel"), "strain": get_meta_value(meta, "strain"), "phenotype": get_meta_value(meta, "phenotype"), "akseg_hash": get_meta_value(meta, "akseg_hash"), "user_initial": get_meta_value(meta, "user_initial"), "content": get_meta_value(meta, "image_content"), "microscope": get_meta_value(meta, "microscope"), "modality": get_meta_value(meta, "modality"), "source": get_meta_value(meta, "light_source"), "stain": get_meta_value(meta, "stain"), "stain_target": get_meta_value(meta, "stain_target"), "antibiotic": get_meta_value(meta, "antibiotic"), "treatment time (mins)": get_meta_value(meta, "treatmenttime"), "antibiotic concentration": get_meta_value(meta, "abxconcentration"), "mounting method": get_meta_value(meta, "mount"), "protocol": get_meta_value(meta, "protocol"), "folder": get_meta_value(meta, "folder"), "parent_folder": get_meta_value(meta, "parent_folder"), "num_segmentations": num_segmentations, "image_laplacian": image_laplacian, "image_focus": get_meta_value(meta, "image_focus"), "image_debris": get_meta_value(meta, "image_debris"), "segmented": get_meta_value(meta, "segmented"), "labelled": get_meta_value(meta, "labelled"), "segmentation_curated": get_meta_value(meta, "segmentations_curated"), "label_curated": get_meta_value(meta, "labels_curated"), "posX": posX, "posY": posY, "posZ": posZ, "image_load_path": get_meta_value(meta, "image_path"), "image_save_path": image_path, "mask_load_path": get_meta_value(meta, "mask_path"), "mask_save_path": mask_path, "label_load_path": get_meta_value(meta, "label_path"), "label_save_path": class_path, }
 
                 for key in range(1, num_user_keys + 1):
-                    file_metadata[f"user_meta{key}"] = get_meta_value(
-                        meta, f"usermeta{key}"
-                    )
+                    file_metadata[f"user_meta{key}"] = get_meta_value(meta, f"usermeta{key}")
 
                 file_metadata_list.append(file_metadata)
 
     except:
         file_metadata_list = []
         print(traceback.format_exc())
 
     return file_metadata_list
 
 
-def generate_upload_tempfiles(
-    user_metadata,
-    image_stack,
-    meta_stack,
-    mask_stack,
-    class_stack,
-    save_dir,
-    overwrite_images,
-    overwrite_masks,
-    overwrite_metadata,
-    overwrite_selected_metadata,
-    overwrite_all_metadata,
-    upload_images,
-    upload_segmentations,
-    upload_metadata,
-):
+def generate_upload_tempfiles(user_metadata, image_stack, meta_stack, mask_stack, class_stack, save_dir, overwrite_images, overwrite_masks, overwrite_metadata, overwrite_selected_metadata, overwrite_all_metadata, upload_images, upload_segmentations, upload_metadata, ):
     upload_tempfiles = []
 
     upload_dir = os.path.join(tempfile.gettempdir(), "BacSeg")
 
     if os.path.isdir(upload_dir) != True:
         os.mkdir(upload_dir)
     else:
@@ -793,48 +562,27 @@
 
             if os.path.exists(json_dir) == False:
                 os.makedirs(json_dir)
 
             if os.path.exists(class_dir) == False:
                 os.makedirs(class_dir)
 
-            upload_data = dict(
-                user_metadata=user_metadata,
-                image=image,
-                image_meta=image_meta,
-                mask=mask,
-                class_mask=class_mask,
-                save_dir=save_dir,
-                overwrite_images=overwrite_images,
-                overwrite_masks=overwrite_masks,
-                overwrite_metadata=overwrite_metadata,
-                overwrite_selected_metadata=overwrite_selected_metadata,
-                overwrite_all_metadata=overwrite_all_metadata,
-                image_dir=image_dir,
-                mask_dir=mask_dir,
-                json_dir=json_dir,
-                class_dir=class_dir,
-                upload_images=upload_images,
-                upload_segmentations=upload_segmentations,
-                upload_metadata=upload_metadata,
-            )
+            upload_data = dict(user_metadata=user_metadata, image=image, image_meta=image_meta, mask=mask, class_mask=class_mask, save_dir=save_dir, overwrite_images=overwrite_images, overwrite_masks=overwrite_masks, overwrite_metadata=overwrite_metadata, overwrite_selected_metadata=overwrite_selected_metadata, overwrite_all_metadata=overwrite_all_metadata, image_dir=image_dir, mask_dir=mask_dir, json_dir=json_dir, class_dir=class_dir, upload_images=upload_images, upload_segmentations=upload_segmentations, upload_metadata=upload_metadata, )
 
             # if "segmentation_file" in user_metadata:
             #     print("segmentation_file in user_metadata")
             # elif "segmentation_channel" in image_meta:
             #     print("segmentation_channel in image_meta")
             # else:
             #     print("segmentation_file not in user_metadata and segmentation_channel not in image_meta")
 
             if os.path.isdir(upload_dir) is False:
                 os.mkdir(upload_dir)
 
-            temp_path = tempfile.TemporaryFile(
-                prefix="BacSeg", suffix=".npy", dir=upload_dir
-            ).name
+            temp_path = tempfile.TemporaryFile(prefix="BacSeg", suffix=".npy", dir=upload_dir).name
 
             np.save(temp_path, upload_data)
 
             upload_tempfiles.append(temp_path)
 
         except:
             pass
@@ -857,320 +605,179 @@
             source = self.label_light_source.currentText()
             stain = self.label_stain.currentText()
             stain_target = self.label_stain_target.currentText()
             date_modified = datetime.datetime.now()
             overwrite_images = self.upload_overwrite_images.isChecked()
             overwrite_masks = self.upload_overwrite_masks.isChecked()
             overwrite_all_metadata = self.overwrite_all_metadata.isChecked()
-            overwrite_selected_metadata = (
-                self.overwrite_selected_metadata.isChecked()
-            )
+            overwrite_selected_metadata = (self.overwrite_selected_metadata.isChecked())
             upload_images = self.upload_images_setting.isChecked()
-            upload_segmentations = (
-                self.upload_segmentations_setting.isChecked()
-            )
+            upload_segmentations = (self.upload_segmentations_setting.isChecked())
             upload_metadata = self.upload_metadata_setting.isChecked()
             strain = self.upload_strain.currentText()
             phenotype = self.upload_phenotype.currentText()
 
             num_user_keys = self.user_metadata_keys
 
             save_dir = os.path.join(database_path, "Images", user_initial)
 
-            if (
-                overwrite_all_metadata is True
-                or overwrite_selected_metadata is True
-            ):
+            if (overwrite_all_metadata is True or overwrite_selected_metadata is True):
                 overwrite_metadata = True
             else:
                 overwrite_metadata = False
 
-            user_metadata_path = os.path.join(
-                database_path,
-                "Images",
-                user_initial,
-                f"{user_initial}_file_metadata.txt",
-            )
+            user_metadata_path = os.path.join(database_path, "Images", user_initial, f"{user_initial}_file_metadata.txt", )
 
             if os.path.exists(user_metadata_path):
-                user_metadata, expected_columns = read_user_metadata(
-                    self, user_metadata_path=user_metadata_path
-                )
+                user_metadata, expected_columns = read_user_metadata(self, user_metadata_path=user_metadata_path)
 
                 metadata_file_names = user_metadata["file_name"].tolist()
                 metadata_akseg_hash = user_metadata["akseg_hash"].tolist()
 
             else:
                 expected_columns = self.metadata_columns
 
                 metadata_file_names = []
                 metadata_akseg_hash = []
 
                 user_metadata = pd.DataFrame(columns=self.metadata_columns)
 
-            channel_labels = [
-                "modality",
-                "light_source",
-                "stain",
-                "stain_target",
-            ]
-            channel_metadata = [
-                layer.metadata[0]
-                for layer in self.viewer.layers
-                if layer.name
-                not in ["Segmentations", "Classes", "center_lines"]
-            ]
+            channel_labels = ["modality", "light_source", "stain", "stain_target", ]
+            channel_metadata = [layer.metadata[0] for layer in self.viewer.layers if layer.name not in ["Segmentations", "Classes", "center_lines"]]
 
             metalabels = []
 
             for label in channel_labels:
                 for channel_meta in channel_metadata:
                     if label in channel_meta.keys():
                         metalabels.append(channel_meta[label])
                     else:
                         metalabels.append("Required for upload")
 
             metalabels = metalabels + [user_initial, content, microscope]
 
-            if (
-                "Required for upload" in metalabels
-                and self.active_import_mode != "BacSeg"
-            ):
+            if ("Required for upload" in metalabels and self.active_import_mode != "BacSeg"):
                 if self.widget_notifications:
-                    show_info(
-                        "Please fill out channel (all channels) and image metadata before uploading files"
-                    )
+                    show_info("Please fill out channel (all channels) and image metadata before uploading files")
 
             else:
                 segChannel = self.cellpose_segchannel.currentText()
-                channel_list = [
-                    layer.name
-                    for layer in self.viewer.layers
-                    if layer.name
-                    not in ["Segmentations", "Classes", "center_lines"]
-                ]
+                channel_list = [layer.name for layer in self.viewer.layers if layer.name not in ["Segmentations", "Classes", "center_lines"]]
 
                 if segChannel == "":
                     if self.widget_notifications:
                         show_info("Please pick an image channel to upload")
 
                 else:
                     backup_user_metadata(self, user_metadata)
 
                     image_layer = self.viewer.layers[segChannel]
 
-                    (
-                        image_stack,
-                        meta_stack,
-                        channel_list,
-                    ) = generate_multichannel_stack(self)
+                    (image_stack, meta_stack, channel_list,) = generate_multichannel_stack(self)
                     mask_stack = self.segLayer.data
                     class_stack = self.classLayer.data
 
                     if len(image_stack) >= 1:
                         if mode == "active":
                             current_step = self.viewer.dims.current_step[0]
 
-                            image_stack = np.expand_dims(
-                                image_stack[current_step], axis=0
-                            )
-                            mask_stack = np.expand_dims(
-                                mask_stack[current_step], axis=0
-                            )
-                            class_stack = np.expand_dims(
-                                class_stack[current_step], axis=0
-                            )
-                            meta_stack = np.expand_dims(
-                                meta_stack[current_step], axis=0
-                            )
-
-                    upload_tempfiles = generate_upload_tempfiles(
-                        user_metadata,
-                        image_stack,
-                        meta_stack,
-                        mask_stack,
-                        class_stack,
-                        save_dir,
-                        overwrite_images,
-                        overwrite_masks,
-                        overwrite_metadata,
-                        overwrite_selected_metadata,
-                        overwrite_all_metadata,
-                        upload_images,
-                        upload_segmentations,
-                        upload_metadata,
-                    )
+                            image_stack = np.expand_dims(image_stack[current_step], axis=0)
+                            mask_stack = np.expand_dims(mask_stack[current_step], axis=0)
+                            class_stack = np.expand_dims(class_stack[current_step], axis=0)
+                            meta_stack = np.expand_dims(meta_stack[current_step], axis=0)
+
+                    upload_tempfiles = generate_upload_tempfiles(user_metadata, image_stack, meta_stack, mask_stack, class_stack, save_dir, overwrite_images, overwrite_masks, overwrite_metadata, overwrite_selected_metadata, overwrite_all_metadata, upload_images, upload_segmentations, upload_metadata, )
 
                     if mode == "active":
-                        results = upload_bacseg_files(
-                            upload_tempfiles[0], num_user_keys
-                        )
+                        results = upload_bacseg_files(upload_tempfiles[0], num_user_keys)
 
                     else:
                         with Pool(4) as pool:
                             iter = []
 
                             def callback(*args):
                                 iter.append(1)
-                                progress = (
-                                    len(iter) / len(upload_tempfiles)
-                                ) * 100
+                                progress = (len(iter) / len(upload_tempfiles)) * 100
 
                                 if progress_callback != None:
                                     try:
                                         progress_callback.emit(progress)
                                     except:
                                         pass
 
                                 return
 
-                            results = [
-                                pool.apply_async(
-                                    upload_bacseg_files,
-                                    args=(i, num_user_keys),
-                                    callback=callback,
-                                )
-                                for i in upload_tempfiles
-                            ]
+                            results = [pool.apply_async(upload_bacseg_files, args=(i, num_user_keys), callback=callback, ) for i in upload_tempfiles]
 
                             try:
                                 results[-1].get()
                             except:
                                 print(traceback.format_exc())
                             else:
                                 results = [r.get() for r in results]
-                                results = [
-                                    file_metadata
-                                    for file_metadata_list in results
-                                    for file_metadata in file_metadata_list
-                                    if file_metadata != None
-                                ]
+                                results = [file_metadata for file_metadata_list in results for file_metadata in file_metadata_list if file_metadata != None]
                                 pool.close()
                                 pool.join()
 
-                            results = [
-                                dat for dat in results if results != None
-                            ]
+                            results = [dat for dat in results if results != None]
 
                     if upload_metadata is True:
                         for file_metadata in results:
                             if file_metadata != None:
                                 akseg_hash = file_metadata["akseg_hash"]
 
-                                file_metadata = pd.DataFrame.from_dict(
-                                    file_metadata, dtype=object
-                                )
+                                file_metadata = pd.DataFrame.from_dict(file_metadata, dtype=object)
 
                                 columns = file_metadata.columns.tolist()
-                                column_dict = {
-                                    col: "first"
-                                    for col in columns
-                                    if col not in ["file_list", "channel_list"]
-                                }
-
-                                df = (
-                                    file_metadata.groupby(["file_name"]).agg(
-                                        {
-                                            **{
-                                                "file_list": lambda x: x.tolist(),
-                                                "channel_list": lambda x: x.tolist(),
-                                            },
-                                            **column_dict,
-                                        }
-                                    )
-                                ).reset_index(drop=True)
+                                column_dict = {col: "first" for col in columns if col not in ["file_list", "channel_list"]}
+
+                                df = (file_metadata.groupby(["file_name"]).agg({**{"file_list": lambda x: x.tolist(), "channel_list": lambda x: x.tolist(), }, **column_dict, })).reset_index(drop=True)
 
                                 file_metadata = df[columns]
 
-                                file_metadata = file_metadata.astype(
-                                    {
-                                        "segmented": bool,
-                                        "labelled": bool,
-                                        "segmentation_curated": bool,
-                                        "label_curated": bool,
-                                    }
-                                )
-
-                                user_metadata = user_metadata.astype(
-                                    {
-                                        "segmented": bool,
-                                        "labelled": bool,
-                                        "segmentation_curated": bool,
-                                        "label_curated": bool,
-                                    }
-                                )
-
-                                user_metadata.reset_index(
-                                    drop=True, inplace=True
-                                )
-                                file_metadata.reset_index(
-                                    drop=True, inplace=True
-                                )
-
-                                user_metadata = user_metadata.loc[
-                                    :, ~user_metadata.columns.duplicated()
-                                ].copy()
-                                file_metadata = file_metadata.loc[
-                                    :, ~file_metadata.columns.duplicated()
-                                ].copy()
+                                file_metadata = file_metadata.astype({"segmented": bool, "labelled": bool, "segmentation_curated": bool, "label_curated": bool, })
+
+                                user_metadata = user_metadata.astype({"segmented": bool, "labelled": bool, "segmentation_curated": bool, "label_curated": bool, })
+
+                                user_metadata.reset_index(drop=True, inplace=True)
+                                file_metadata.reset_index(drop=True, inplace=True)
+
+                                user_metadata = user_metadata.loc[:, ~user_metadata.columns.duplicated()].copy()
+                                file_metadata = file_metadata.loc[:, ~file_metadata.columns.duplicated()].copy()
 
                                 for column in user_metadata.columns.tolist():
-                                    if (
-                                        column
-                                        not in file_metadata.columns.tolist()
-                                    ):
+                                    if (column not in file_metadata.columns.tolist()):
                                         file_metadata[column] = ""
 
                                 if akseg_hash in metadata_akseg_hash:
-                                    user_metadata = pd.concat(
-                                        (user_metadata, file_metadata),
-                                        ignore_index=True,
-                                        axis=0,
-                                    )  # .reset_index(drop=True)
-                                    user_metadata.drop_duplicates(
-                                        subset=["akseg_hash"],
-                                        keep="last",
-                                        inplace=True,
-                                    )
+                                    user_metadata = pd.concat((user_metadata, file_metadata), ignore_index=True, axis=0, )  # .reset_index(drop=True)
+                                    user_metadata.drop_duplicates(subset=["akseg_hash"], keep="last", inplace=True, )
 
                                 else:
-                                    user_metadata = pd.concat(
-                                        (user_metadata, file_metadata),
-                                        ignore_index=True,
-                                        axis=0,
-                                    ).reset_index(drop=True)
+                                    user_metadata = pd.concat((user_metadata, file_metadata), ignore_index=True, axis=0, ).reset_index(drop=True)
 
                     if upload_metadata is True:
                         user_metadata = user_metadata.astype("str")
 
-                        user_metadata.drop_duplicates(
-                            subset=["akseg_hash"], keep="first", inplace=True
-                        )
+                        user_metadata.drop_duplicates(subset=["akseg_hash"], keep="first", inplace=True)
                         user_metadata = user_metadata[expected_columns]
 
-                        user_metadata.to_csv(
-                            user_metadata_path, sep=",", index=False
-                        )
+                        user_metadata.to_csv(user_metadata_path, sep=",", index=False)
 
     except:
         print(traceback.format_exc())
 
 
 def read_user_metadata(self, user_metadata_path=""):
     try:
         if user_metadata_path == "":
             database_path = self.database_path
             user_initial = self.upload_initial.currentText()
 
-            user_metadata_path = os.path.join(
-                database_path,
-                "Images",
-                user_initial,
-                f"{user_initial}_file_metadata.txt",
-            )
+            user_metadata_path = os.path.join(database_path, "Images", user_initial, f"{user_initial}_file_metadata.txt", )
 
         if os.path.isfile(user_metadata_path) == False:
             if self.widget_notifications:
                 show_info("Could not find metadata for user: " + user_initial)
 
             measurements = []
             file_paths = []
@@ -1182,25 +789,21 @@
             # checks the delimiter of the metadata file
 
             with open(user_metadata_path) as f:
                 for row in range(10):
                     line = next(f).strip()
                     delim = sniffer.sniff(line)
 
-            user_metadata = pd.read_csv(
-                user_metadata_path, sep=delim.delimiter, low_memory=False
-            )
-
-            user_metadata, expected_columns = check_metadata_format(
-                user_metadata, self.metadata_columns
-            )
-
-            user_metadata["segmentation_channel"] = user_metadata[
-                "segmentation_channel"
-            ].astype(str)
+            user_metadata = pd.read_csv(user_metadata_path, sep=delim.delimiter, low_memory=False)
+
+            user_metadata[["treatment time (mins)"]] = user_metadata[["treatment time (mins)"]].apply(pd.to_numeric, downcast="float")
+
+            user_metadata, expected_columns = check_metadata_format(user_metadata, self.metadata_columns)
+
+            user_metadata["segmentation_channel"] = user_metadata["segmentation_channel"].astype(str)
 
             self.user_metadata = user_metadata
             self.expected_columns = expected_columns
 
     except:
         user_metadata = None
 
@@ -1214,137 +817,83 @@
 
         database_path = self.database_path
 
         user_initial = self.upload_initial.currentText()
 
         todays_date = datetime.datetime.now().strftime("%y%m%d-%H%M")
 
-        user_metadata_path = os.path.join(
-            database_path,
-            "Images",
-            user_initial,
-            "file metadata backup",
-            f"{user_initial}_file_metadata_{todays_date}.txt",
-        )
+        user_metadata_path = os.path.join(database_path, "Images", user_initial, "file metadata backup", f"{user_initial}_file_metadata_{todays_date}.txt", )
 
         if os.path.exists(os.path.dirname(user_metadata_path)) == False:
             os.makedirs(os.path.dirname(user_metadata_path))
 
         user_metadata = user_metadata.astype("str")
 
-        user_metadata.drop_duplicates(
-            subset=["akseg_hash"], keep="first", inplace=True
-        )
+        user_metadata.drop_duplicates(subset=["akseg_hash"], keep="first", inplace=True)
 
         show_info("Creating metadata backup for user: " + user_initial)
 
         user_metadata.to_csv(user_metadata_path, sep=",", index=False)
 
     except:
         print(traceback.format_exc())
 
 
 def get_filtered_database_metadata(self):
     try:
-        database_metadata = {
-            "user_initial": self.upload_initial.currentText(),
-            "content": self.upload_content.currentText(),
-            "microscope": self.upload_microscope.currentText(),
-            "phenotype": self.upload_phenotype.currentText(),
-            "strain": self.upload_strain.currentText(),
-            "antibiotic": self.upload_antibiotic.currentText(),
-            "antibiotic concentration": self.upload_abxconcentration.currentText(),
-            "treatment time (mins)": self.upload_treatmenttime.currentText(),
-            "mounting method": self.upload_mount.currentText(),
-            "protocol": self.upload_protocol.currentText(),
-        }
+        database_metadata = {"user_initial": self.upload_initial.currentText(), "content": self.upload_content.currentText(), "microscope": self.upload_microscope.currentText(), "phenotype": self.upload_phenotype.currentText(), "strain": self.upload_strain.currentText(), "antibiotic": self.upload_antibiotic.currentText(), "antibiotic concentration": self.upload_abxconcentration.currentText(), "treatment time (mins)": self.upload_treatmenttime.currentText(), "mounting method": self.upload_mount.currentText(), "protocol": self.upload_protocol.currentText(), }
 
         num_user_keys = self.user_metadata_keys
 
         for key in range(1, num_user_keys + 1):
             control_name = f"upload_usermeta{key}"
             combo_box = getattr(self, control_name)
             combo_box_text = combo_box.currentText()
             database_metadata[f"user_meta{key}"] = combo_box_text
 
-        database_metadata = {
-            key: val
-            for key, val in database_metadata.items()
-            if val
-            not in [
-                "",
-                "Required for upload",
-                "example_item1",
-                "example_item2",
-                "example_item3",
-            ]
-        }
+        database_metadata = {key: val for key, val in database_metadata.items() if val not in ["", "Required for upload", "example_item1", "example_item2", "example_item3", ]}
 
         database_path = self.database_path
 
         user_initial = database_metadata["user_initial"]
 
-        user_metadata_path = os.path.join(
-            database_path,
-            "Images",
-            user_initial,
-            f"{user_initial}_file_metadata.txt",
-        )
+        user_metadata_path = os.path.join(database_path, "Images", user_initial, f"{user_initial}_file_metadata.txt", )
 
         if os.path.isfile(user_metadata_path) == False:
             if self.widget_notifications:
                 show_info("Could not find metadata for user: " + user_initial)
 
             measurements = []
             file_paths = []
             channels = []
 
         else:
             user_metadata, expected_columns = read_user_metadata(self)
 
-            user_metadata["segmentation_channel"] = user_metadata[
-                "segmentation_channel"
-            ].astype(str)
+            user_metadata["segmentation_channel"] = user_metadata["segmentation_channel"].astype(str)
+            user_metadata["treatment time (mins)"] = user_metadata["treatment time (mins)"].astype(str)
 
             for key, value in database_metadata.items():
                 if key in user_metadata.columns:
                     user_metadata = user_metadata[user_metadata[key] == value]
 
             if self.upload_segmentation_combo.currentIndex() == 1:
-                user_metadata = user_metadata[
-                    user_metadata["segmented"] == False
-                ]
+                user_metadata = user_metadata[user_metadata["segmented"] == False]
             if self.upload_segmentation_combo.currentIndex() == 2:
-                user_metadata = user_metadata[
-                    user_metadata["segmented"]
-                    == True & (user_metadata["segmentation_curated"] == False)
-                ]
+                user_metadata = user_metadata[user_metadata["segmented"] == True & (user_metadata["segmentation_curated"] == False)]
             if self.upload_segmentation_combo.currentIndex() == 3:
-                user_metadata = user_metadata[
-                    (user_metadata["segmented"] == True)
-                    & (user_metadata["segmentation_curated"] == True)
-                ]
+                user_metadata = user_metadata[(user_metadata["segmented"] == True) & (user_metadata["segmentation_curated"] == True)]
             if self.upload_label_combo.currentIndex() == 1:
-                user_metadata = user_metadata[
-                    user_metadata["labelled"] == False
-                ]
+                user_metadata = user_metadata[user_metadata["labelled"] == False]
             if self.upload_label_combo.currentIndex() == 2:
-                user_metadata = user_metadata[
-                    user_metadata["labelled"]
-                    == True & (user_metadata["label_curated"] == False)
-                ]
+                user_metadata = user_metadata[user_metadata["labelled"] == True & (user_metadata["label_curated"] == False)]
             if self.upload_label_combo.currentIndex() == 3:
-                user_metadata = user_metadata[
-                    (user_metadata["labelled"] == True)
-                    & (user_metadata["label_curated"] == True)
-                ]
-
-            user_metadata.sort_values(
-                by=["posX", "posY", "posZ"], ascending=True
-            )
+                user_metadata = user_metadata[(user_metadata["labelled"] == True) & (user_metadata["label_curated"] == True)]
+
+            user_metadata.sort_values(by=["posX", "posY", "posZ"], ascending=True)
 
             sort_names = []
             sort_directions = []
 
             if self.download_sort_order_1.currentIndex() > 1:
                 if self.download_sort_direction_1.currentIndex() == 1:
                     sort_directions.append(True)
@@ -1354,17 +903,15 @@
             if self.download_sort_order_2.currentIndex() > 1:
                 if self.download_sort_direction_2.currentIndex() == 1:
                     sort_directions.append(True)
                 if self.download_sort_direction_2.currentIndex() == 2:
                     sort_directions.append(False)
 
             if self.download_sort_order_1.currentIndex() == 1:
-                user_metadata = user_metadata.sample(frac=1).reset_index(
-                    drop=True
-                )
+                user_metadata = user_metadata.sample(frac=1).reset_index(drop=True)
             if self.download_sort_order_1.currentIndex() == 2:
                 sort_names.append("date_uploaded")
             if self.download_sort_order_1.currentIndex() == 3:
                 sort_names.append("date_modified")
             if self.download_sort_order_1.currentIndex() == 4:
                 if "image_laplacian" in user_metadata.columns:
                     sort_names.append("image_laplacian")
@@ -1375,17 +922,15 @@
                 if "image_focus" in user_metadata.columns:
                     sort_names.append("image_focus")
             if self.download_sort_order_1.currentIndex() == 7:
                 if "image_debris" in user_metadata.columns:
                     sort_names.append("image_debris")
 
             if self.download_sort_order_2.currentIndex() == 1:
-                user_metadata = user_metadata.sample(frac=1).reset_index(
-                    drop=True
-                )
+                user_metadata = user_metadata.sample(frac=1).reset_index(drop=True)
             if self.download_sort_order_2.currentIndex() == 2:
                 sort_names.append("date_uploaded")
             if self.download_sort_order_2.currentIndex() == 3:
                 sort_names.append("date_modified")
             if self.download_sort_order_2.currentIndex() == 4:
                 if "image_laplacian" in user_metadata.columns:
                     sort_names.append("image_laplacian")
@@ -1398,81 +943,64 @@
             if self.download_sort_order_2.currentIndex() == 7:
                 if "image_debris" in user_metadata.columns:
                     sort_names.append("image_debris")
 
             if len(sort_names) > 0:
                 if len(sort_names) != len(sort_directions):
                     sort_directions = [False] * len(sort_names)
-                user_metadata = user_metadata.sort_values(
-                    sort_names, ascending=sort_directions
-                ).reset_index(drop=True)
+                user_metadata = user_metadata.sort_values(sort_names, ascending=sort_directions).reset_index(drop=True)
 
             import_limit = self.database_download_limit.currentText()
 
             segmentation_files = user_metadata["segmentation_file"].unique()
             num_measurements = len(segmentation_files)
 
             if import_limit == "All":
                 import_limit = num_measurements
             else:
                 if int(import_limit) > num_measurements:
                     import_limit = num_measurements
 
-            user_metadata = user_metadata[
-                user_metadata["segmentation_file"].isin(
-                    segmentation_files[: int(import_limit)]
-                )
-            ]
+            user_metadata = user_metadata[user_metadata["segmentation_file"].isin(segmentation_files[: int(import_limit)])]
 
             user_metadata["path"] = user_metadata["image_save_path"]
 
             channels = user_metadata["channel"].unique().tolist()
             file_paths = user_metadata["image_save_path"].tolist()
 
             len1 = len(user_metadata)
 
-            user_metadata = user_metadata[
-                ~user_metadata["segmentation_file"].isin(
-                    ["None", None, np.nan]
-                )
-            ]
-            user_metadata = user_metadata[
-                ~user_metadata["folder"].isin(["None", None, np.nan])
-            ]
+            user_metadata = user_metadata[~user_metadata["segmentation_file"].isin(["None", None, np.nan])]
+            user_metadata = user_metadata[~user_metadata["folder"].isin(["None", None, np.nan])]
 
             len2 = len(user_metadata)
 
             if len2 < len1:
-                show_info(
-                    f"{len1 - len2} files with missing critical metadata removed."
-                )
+                show_info(f"{len1 - len2} files with missing critical metadata removed.")
 
             sort_columns = []
 
             if "folder" in user_metadata.columns:
                 sort_columns.append("folder")
-                user_metadata.loc[
-                    user_metadata["folder"].isna(), "folder"
-                ] = "None"
+                user_metadata.loc[user_metadata["folder"].isna(), "folder"] = "None"
             if "segmentation_file" in user_metadata.columns:
                 sort_columns.append("segmentation_file")
-                user_metadata.loc[
-                    user_metadata["segmentation_file"].isna(),
-                    "segmentation_file",
-                ] = "None"
+                user_metadata.loc[user_metadata["segmentation_file"].isna(), "segmentation_file",] = "None"
             if "posX" in user_metadata.columns:
                 sort_columns.append("posX")
                 user_metadata.loc[user_metadata["posX"].isna(), "posX"] = 0
             if "posY" in user_metadata.columns:
                 sort_columns.append("posY")
                 user_metadata.loc[user_metadata["posY"].isna(), "posY"] = 0
             if "posZ" in user_metadata.columns:
                 sort_columns.append("posZ")
                 user_metadata.loc[user_metadata["posZ"].isna(), "posZ"] = 0
 
             measurements = user_metadata.groupby(sort_columns)
 
+            show_info(f"Found {len(file_paths)//len(channels)} matching database files.")
+
     except:
         print(traceback.format_exc())
         measurements, file_paths, channels = None, None, None
 
     return measurements, file_paths, channels
```

### Comparing `napari-bacseg-1.0.5/src/napari_bacseg/_utils_imagej.py` & `napari-bacseg-1.0.6/src/napari_bacseg/_utils_imagej.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.5/src/napari_bacseg/_utils_interface_events.py` & `napari-bacseg-1.0.6/src/napari_bacseg/_utils_interface_events.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,17 +5,15 @@
 import cv2
 import numpy as np
 from napari.utils.notifications import show_info
 
 
 def find_contours(img):
     # finds contours of shapes, only returns the external contours of the shapes
-    contours, hierarchy = cv2.findContours(
-        img, cv2.RETR_EXTERNAL, cv2.CHAIN_APPROX_NONE
-    )
+    contours, hierarchy = cv2.findContours(img, cv2.RETR_EXTERNAL, cv2.CHAIN_APPROX_NONE)
     contours = sorted(contours, key=cv2.contourArea, reverse=True)
     return contours
 
 
 def fill_holes(mask, colour):
     try:
         fill_mask = mask.copy()
@@ -51,17 +49,15 @@
                 stored_mask = self.segLayer.data.copy()
                 stored_class = self.classLayer.data.copy()
                 meta = self.segLayer.metadata.copy()
 
                 if self.segmentation_mode == "add":
                     new_colour = _newSegColour(self)
                 else:
-                    data_coordinates = self.segLayer.world_to_data(
-                        event.position
-                    )
+                    data_coordinates = self.segLayer.world_to_data(event.position)
                     coord = np.round(data_coordinates).astype(int)
                     new_colour = self.segLayer.get_value(coord)
 
                     self.segLayer.selected_label = new_colour
                     new_colour = self.segLayer.get_value(coord)
 
                     new_class = self.classLayer.get_value(coord)
@@ -78,37 +74,29 @@
                 while event.type == "mouse_move":
                     coordinates.append(event.position)
                     dragged = True
                     yield
 
                 # on release
                 if dragged:
-                    if (
-                        new_colour != 0
-                        and new_colour != None
-                        and self.class_colour != None
-                    ):
-                        coordinates = np.round(np.array(coordinates)).astype(
-                            np.int32
-                        )
+                    if (new_colour != 0 and new_colour != None and self.class_colour != None):
+                        coordinates = np.round(np.array(coordinates)).astype(np.int32)
 
                         mask_dim = tuple(list(coordinates[0][:-2]) + [...])
 
                         cnt = coordinates[:, -2:]
 
                         cnt = np.fliplr(cnt)
                         cnt = cnt.reshape((-1, 1, 2))
 
                         seg_stack = self.segLayer.data
 
                         seg_mask = seg_stack[mask_dim]
 
-                        cv2.drawContours(
-                            seg_mask, [cnt], -1, int(new_colour), -1
-                        )
+                        cv2.drawContours(seg_mask, [cnt], -1, int(new_colour), -1)
 
                         seg_mask = fill_holes(seg_mask, new_colour)
 
                         seg_stack[mask_dim] = seg_mask
 
                         self.segLayer.data = seg_stack
 
@@ -163,17 +151,15 @@
                 colours = []
                 classes = []
                 coords = []
                 yield
 
                 # on move
                 while event.type == "mouse_move":
-                    data_coordinates = self.segLayer.world_to_data(
-                        event.position
-                    )
+                    data_coordinates = self.segLayer.world_to_data(event.position)
                     coord = np.round(data_coordinates).astype(int)
                     mask_val = self.segLayer.get_value(coord)
                     class_val = self.classLayer.get_value(coord)
                     colours.append(mask_val)
                     classes.append(class_val)
                     coords.append(coord)
                     dragged = True
@@ -182,23 +168,17 @@
                 # on release
                 if dragged:
                     colours = np.array(colours)
                     colours = np.unique(colours)
                     colours = np.delete(colours, np.where(colours == 0))
 
                     if new_colour in colours:
-                        colours = np.delete(
-                            colours, np.where(colours == new_colour)
-                        )
-
-                    if (
-                        len(colours) == 1
-                        and new_colour not in colours
-                        and new_colour != None
-                    ):
+                        colours = np.delete(colours, np.where(colours == new_colour))
+
+                    if (len(colours) == 1 and new_colour not in colours and new_colour != None):
                         mask_stack = self.segLayer.data
 
                         mask_dim = tuple(list(coords[0][:-2]) + [...])
 
                         mask = mask_stack[mask_dim]
 
                         mask[mask == colours[0]] = new_colour
@@ -246,46 +226,37 @@
 
                 dragged = False
                 colours = []
                 yield
 
                 # on move
                 while event.type == "mouse_move":
-                    data_coordinates = self.segLayer.world_to_data(
-                        event.position
-                    )
+                    data_coordinates = self.segLayer.world_to_data(event.position)
                     coords = np.round(data_coordinates).astype(int)
                     mask_val = self.segLayer.get_value(coords)
                     colours.append(mask_val)
                     dragged = True
                     yield
 
                 # on release
                 if dragged:
                     colours = np.array(colours)
-                    colours = np.delete(
-                        colours, np.where(colours == new_colour)
-                    )
+                    colours = np.delete(colours, np.where(colours == new_colour))
 
                     colours[colours == None] = 0
 
                     num_colours = len(np.unique(colours))
 
                     if num_colours == 2 or num_colours == 3:
                         if num_colours == 2:
                             maskref = colours[colours != 0][0]
                         else:
-                            maskref = sorted(
-                                set(colours.tolist()),
-                                key=lambda x: colours.tolist().index(x),
-                            )[1]
-
-                        bisection = (
-                            colours[0] != maskref and colours[-1] != maskref
-                        )
+                            maskref = sorted(set(colours.tolist()), key=lambda x: colours.tolist().index(x), )[1]
+
+                        bisection = (colours[0] != maskref and colours[-1] != maskref)
 
                         if bisection and new_colour != None:
                             mask_dim = tuple(list(coords[:-2]) + [...])
                             shape_mask = stored_mask[mask_dim].copy()
 
                             class_mask = stored_class[mask_dim].copy()
                             class_mask[shape_mask == maskref] = 3
@@ -300,30 +271,25 @@
                             line_mask = line_mask[mask_dim]
                             line_mask[line_mask != new_colour] = 0
                             line_mask[line_mask == new_colour] = 255
                             line_mask = line_mask.astype(np.uint8)
 
                             overlap = cv2.bitwise_and(shape_mask, line_mask)
 
-                            shape_mask_split = cv2.bitwise_xor(
-                                shape_mask, overlap
-                            ).astype(np.uint8)
+                            shape_mask_split = cv2.bitwise_xor(shape_mask, overlap).astype(np.uint8)
 
                             # update labels layers with split shape
                             split_mask = stored_mask[mask_dim]
                             split_mask[overlap == 255] = new_colour
                             stored_mask[mask_dim] = split_mask
                             self.segLayer.data = stored_mask
 
                             # fill one have of the split shape with the new colour
                             indices = np.where(shape_mask_split == 255)
-                            split_dim = list(
-                                list(mask_dim[:-1])
-                                + [indices[0][0], indices[1][0]]
-                            )
+                            split_dim = list(list(mask_dim[:-1]) + [indices[0][0], indices[1][0]])
                             split_dim = np.array(split_dim).flatten().tolist()
 
                             self.segLayer.fill(split_dim, new_colour)
 
                             meta["manual_segmentation"] = True
                             self.segLayer.metadata = meta
                             self.segLayer.mode = "pan_zoom"
@@ -359,17 +325,15 @@
                     dragged = True
                     yield
 
                 # on release
                 if dragged:
                     self.segLayer.data = stored_mask
 
-                    coordinates = np.round(np.array(coordinates)).astype(
-                        np.int32
-                    )
+                    coordinates = np.round(np.array(coordinates)).astype(np.int32)
                     cnt = coordinates[:, -2:]
 
                     cnt = np.fliplr(cnt)
                     cnt = cnt.reshape((-1, 1, 2))
 
                     mask_dim = tuple(list(coordinates[0][:-2]) + [...])
 
@@ -398,17 +362,15 @@
                 else:
                     self.segLayer.data = stored_mask
                     self.segLayer.mode = "pan_zoom"
                     self.update_image_folds()
 
                     meta = self.segLayer.metadata.copy()
 
-                    data_coordinates = self.segLayer.world_to_data(
-                        event.position
-                    )
+                    data_coordinates = self.segLayer.world_to_data(event.position)
                     coord = np.round(data_coordinates).astype(int)
                     mask_val = self.segLayer.get_value(coord)
 
                     if mask_val != 0:
                         mask_dim = tuple(list(coord[:-2]) + [...])[0]
 
                         mask_stack = self.segLayer.data
@@ -430,20 +392,15 @@
 
                         meta["manual_segmentation"] = True
                         self.segLayer.metadata = meta
                         self.segLayer.mode = "pan_zoom"
                         self.update_image_folds()
 
             if self.segmentation_mode == "refine":
-                layer_names = [
-                    layer.name
-                    for layer in self.viewer.layers
-                    if layer.name
-                    not in ["Segmentations", "Classes", "center_lines"]
-                ]
+                layer_names = [layer.name for layer in self.viewer.layers if layer.name not in ["Segmentations", "Classes", "center_lines"]]
 
                 self.segLayer.mode == "pan_zoom"
                 self.segLayer.brush_size = 1
 
                 data_coordinates = self.segLayer.world_to_data(event.position)
                 coord = np.round(data_coordinates).astype(int)
                 mask_id = self.segLayer.get_value(coord)
@@ -460,53 +417,33 @@
                     mask_stack = self.segLayer.data
 
                     mask = mask_stack[current_fov, :, :].copy()
                     label = label_stack[current_fov, :, :].copy()
 
                     image = []
                     for layer in layer_names:
-                        image.append(
-                            self.viewer.layers[layer].data[current_fov]
-                        )
+                        image.append(self.viewer.layers[layer].data[current_fov])
                     image = np.stack(image, axis=0)
 
                     cell_mask = np.zeros(mask.shape, dtype=np.uint8)
 
                     mask[mask != mask_id] = 0
                     cell_mask[mask != mask_id] = 0
                     cell_mask[mask == mask_id] = 1
 
-                    from napari_bacseg._utils_colicoords import (
-                        process_colicoords,
-                        run_colicoords,
-                    )
+                    from napari_bacseg._utils_colicoords import (process_colicoords, run_colicoords, )
                     from napari_bacseg._utils_statistics import get_cell_images
 
-                    colicoords_dir = os.path.join(
-                        tempfile.gettempdir(), "colicoords"
-                    )
-
-                    cell_images_path = get_cell_images(
-                        self,
-                        image,
-                        mask,
-                        cell_mask,
-                        mask_id,
-                        layer_names,
-                        colicoords_dir,
-                    )
+                    colicoords_dir = os.path.join(tempfile.gettempdir(), "colicoords")
+
+                    cell_images_path = get_cell_images(self, image, mask, cell_mask, mask_id, layer_names, colicoords_dir, )
 
                     cell_data = {"cell_images_path": cell_images_path}
 
-                    colicoords_data = run_colicoords(
-                        self,
-                        cell_data=[cell_data],
-                        colicoords_channel=channel,
-                        multithreaded=True,
-                    )
+                    colicoords_data = run_colicoords(self, cell_data=[cell_data], colicoords_channel=channel, multithreaded=True, )
 
                     process_colicoords(self, colicoords_data)
 
         if self.interface_mode == "classify":
             self.segLayer.mode == "pan_zoom"
             self.segLayer.brush_size = 1
 
@@ -603,18 +540,15 @@
             self.modify_segment.setEnabled(True)
             self.modify_classify.setEnabled(False)
 
         if mode == "clicktozoom":
             self.viewer.layers.selection.select_only(self.segLayer)
 
             self.interface_mode = "segment"
-            self.segmentation_mode = "clicktozoom"
-            # self.modify_panzoom.setEnabled(True)
-            # self.modify_segment.setEnabled(True)
-            # self.modify_classify.setEnabled(True)
+            self.segmentation_mode = "clicktozoom"  # self.modify_panzoom.setEnabled(True)  # self.modify_segment.setEnabled(True)  # self.modify_classify.setEnabled(True)
 
         if mode == "add":
             self.viewer.layers.selection.select_only(self.segLayer)
 
             self.interface_mode = "segment"
             self.segmentation_mode = "add"
             self.modify_panzoom.setEnabled(True)
@@ -745,15 +679,15 @@
             show_info("Edge (click to classify)")
 
     return _event
 
 
 def autocontrast_values(image, clip_hist_percent=0.001):
     # calculate histogram
-    hist, bin_edges = np.histogram(image, bins=(2**16) - 1)
+    hist, bin_edges = np.histogram(image, bins=(2 ** 16) - 1)
     hist_size = len(hist)
 
     # calculate cumulative distribution from the histogram
     accumulator = cumsum(hist)
 
     # Locate points to clip
     maximum = accumulator[-1]
@@ -861,55 +795,39 @@
         if key == "viewlabels":
             self.classLayer.visible = self.modify_viewlabels.isChecked()
 
         if key == "viewmasks":
             self.segLayer.visible = self.modify_viewmasks.isChecked()
 
         if key == "c":
-            layer_names = [
-                layer.name
-                for layer in self.viewer.layers
-                if layer.name
-                not in ["Segmentations", "Classes", "center_lines"]
-            ]
+            layer_names = [layer.name for layer in self.viewer.layers if layer.name not in ["Segmentations", "Classes", "center_lines"]]
 
             if len(layer_names) != 0:
                 active_layer = layer_names[-1]
 
-                image_dims = tuple(
-                    list(self.viewer.dims.current_step[:-2]) + [...]
-                )
-
-                image = (
-                    self.viewer.layers[str(active_layer)]
-                    .data[image_dims]
-                    .copy()
-                )
-
-                crop = self.viewer.layers[str(active_layer)].corner_pixels[
-                    :, -2:
-                ]
+                image_dims = tuple(list(self.viewer.dims.current_step[:-2]) + [...])
+
+                image = (self.viewer.layers[str(active_layer)].data[image_dims].copy())
+
+                crop = self.viewer.layers[str(active_layer)].corner_pixels[:, -2:]
 
                 [[y1, x1], [y2, x2]] = crop
 
                 image_crop = image[y1:y2, x1:x2]
 
                 contrast_limit = [np.min(image_crop), np.max(image_crop)]
 
                 if contrast_limit[1] > contrast_limit[0]:
-                    self.viewer.layers[
-                        str(active_layer)
-                    ].contrast_limits = contrast_limit
+                    self.viewer.layers[str(active_layer)].contrast_limits = contrast_limit
 
     return _event
 
 
 def _imageControls(self, key, viewer=None):
     def _event(viewer):
-        print(True)
 
         if key == "Upload":
             self._uploadDatabase("active")
 
         if len(self.viewer.dims.current_step) == 3:
             current_frame = self.viewer.dims.current_step[0]
             frame_range = int(self.viewer.dims.range[0][1]) - 1
@@ -1006,17 +924,15 @@
 
             else:
                 for image_index in range(*viewer_dims[0]):
                     mask = self.segLayer.data[image_index].copy()
                     mask_ids = np.unique(mask)
 
                     if len(viewer_dims) == 2:
-                        self.update_image_folds(
-                            mask_ids=mask_ids, image_index=image_index
-                        )
+                        self.update_image_folds(mask_ids=mask_ids, image_index=image_index)
 
                     else:
                         for mask_id in mask_ids:
                             mask[mask == mask_id] = 0
 
                         self.segLayer.data[image_index] = mask
                         self.segLayer.refresh()
```

### Comparing `napari-bacseg-1.0.5/src/napari_bacseg/_utils_json.py` & `napari-bacseg-1.0.6/src/napari_bacseg/_utils_json.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.5/src/napari_bacseg/_utils_oufti.py` & `napari-bacseg-1.0.6/src/napari_bacseg/_utils_oufti.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.5/src/napari_bacseg/_utils_refine.py` & `napari-bacseg-1.0.6/src/napari_bacseg/_utils_refine.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.5/src/napari_bacseg/_utils_statistics.py` & `napari-bacseg-1.0.6/src/napari_bacseg/_utils_statistics.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.5/src/napari_bacseg/_utils_tiler.py` & `napari-bacseg-1.0.6/src/napari_bacseg/_utils_tiler.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.5/src/napari_bacseg/bacseg_ui.py` & `napari-bacseg-1.0.6/src/napari_bacseg/bacseg_ui.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,21 +149,21 @@
         spacerItem4 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
         self.verticalLayout.addItem(spacerItem4)
         tab_widget.addTab(self.import_tab, "")
         self.tab = QtWidgets.QWidget()
         self.tab.setObjectName("tab")
         self.verticalLayout_5 = QtWidgets.QVBoxLayout(self.tab)
         self.verticalLayout_5.setObjectName("verticalLayout_5")
-        self.tabWidget = QtWidgets.QTabWidget(self.tab)
+        self.zoom_ = QtWidgets.QTabWidget(self.tab)
         sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Preferred)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
-        sizePolicy.setHeightForWidth(self.tabWidget.sizePolicy().hasHeightForWidth())
-        self.tabWidget.setSizePolicy(sizePolicy)
-        self.tabWidget.setObjectName("tabWidget")
+        sizePolicy.setHeightForWidth(self.zoom_.sizePolicy().hasHeightForWidth())
+        self.zoom_.setSizePolicy(sizePolicy)
+        self.zoom_.setObjectName("zoom_")
         self.tab_16 = QtWidgets.QWidget()
         self.tab_16.setObjectName("tab_16")
         self.verticalLayout_23 = QtWidgets.QVBoxLayout(self.tab_16)
         self.verticalLayout_23.setObjectName("verticalLayout_23")
         self.label_60 = QtWidgets.QLabel(self.tab_16)
         font = QtGui.QFont()
         font.setPointSize(10)
@@ -198,15 +198,15 @@
         self.gridLayout_6.addWidget(self.modify_viewlabels, 1, 1, 1, 1)
         self.modify_viewmasks = QtWidgets.QCheckBox(self.tab_16)
         self.modify_viewmasks.setObjectName("modify_viewmasks")
         self.gridLayout_6.addWidget(self.modify_viewmasks, 1, 0, 1, 1)
         self.verticalLayout_23.addLayout(self.gridLayout_6)
         spacerItem6 = QtWidgets.QSpacerItem(20, 1, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
         self.verticalLayout_23.addItem(spacerItem6)
-        self.tabWidget.addTab(self.tab_16, "")
+        self.zoom_.addTab(self.tab_16, "")
         self.tab_7 = QtWidgets.QWidget()
         self.tab_7.setObjectName("tab_7")
         self.verticalLayout_21 = QtWidgets.QVBoxLayout(self.tab_7)
         self.verticalLayout_21.setObjectName("verticalLayout_21")
         self.line_26 = QtWidgets.QFrame(self.tab_7)
         self.line_26.setFrameShape(QtWidgets.QFrame.HLine)
         self.line_26.setFrameShadow(QtWidgets.QFrame.Sunken)
@@ -237,15 +237,15 @@
         self.gridLayout_20.addWidget(self.scalebar_units, 0, 2, 1, 1)
         self.label_48 = QtWidgets.QLabel(self.tab_7)
         self.label_48.setObjectName("label_48")
         self.gridLayout_20.addWidget(self.label_48, 0, 0, 1, 1)
         self.verticalLayout_21.addLayout(self.gridLayout_20)
         spacerItem7 = QtWidgets.QSpacerItem(20, 1, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
         self.verticalLayout_21.addItem(spacerItem7)
-        self.tabWidget.addTab(self.tab_7, "")
+        self.zoom_.addTab(self.tab_7, "")
         self.tab_15 = QtWidgets.QWidget()
         self.tab_15.setObjectName("tab_15")
         self.verticalLayout_22 = QtWidgets.QVBoxLayout(self.tab_15)
         self.verticalLayout_22.setObjectName("verticalLayout_22")
         self.line_27 = QtWidgets.QFrame(self.tab_15)
         self.line_27.setFrameShape(QtWidgets.QFrame.HLine)
         self.line_27.setFrameShadow(QtWidgets.QFrame.Sunken)
@@ -315,15 +315,15 @@
         self.gridLayout_30.addWidget(self.overlay_debris, 0, 1, 1, 1)
         self.overlay_range = QtWidgets.QCheckBox(self.tab_15)
         self.overlay_range.setObjectName("overlay_range")
         self.gridLayout_30.addWidget(self.overlay_range, 0, 3, 1, 1)
         self.verticalLayout_22.addLayout(self.gridLayout_30)
         spacerItem8 = QtWidgets.QSpacerItem(20, 1, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
         self.verticalLayout_22.addItem(spacerItem8)
-        self.tabWidget.addTab(self.tab_15, "")
+        self.zoom_.addTab(self.tab_15, "")
         self.tab_17 = QtWidgets.QWidget()
         self.tab_17.setObjectName("tab_17")
         self.verticalLayout_24 = QtWidgets.QVBoxLayout(self.tab_17)
         self.verticalLayout_24.setObjectName("verticalLayout_24")
         self.line_28 = QtWidgets.QFrame(self.tab_17)
         self.line_28.setFrameShape(QtWidgets.QFrame.HLine)
         self.line_28.setFrameShadow(QtWidgets.QFrame.Sunken)
@@ -379,33 +379,77 @@
         self.unfold_mode.setObjectName("unfold_mode")
         self.unfold_mode.addItem("")
         self.unfold_mode.addItem("")
         self.formLayout_3.setWidget(0, QtWidgets.QFormLayout.FieldRole, self.unfold_mode)
         self.verticalLayout_24.addLayout(self.formLayout_3)
         spacerItem9 = QtWidgets.QSpacerItem(20, 1, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
         self.verticalLayout_24.addItem(spacerItem9)
-        self.tabWidget.addTab(self.tab_17, "")
-        self.verticalLayout_5.addWidget(self.tabWidget)
+        self.zoom_.addTab(self.tab_17, "")
+        self.tab_5 = QtWidgets.QWidget()
+        self.tab_5.setObjectName("tab_5")
+        self.verticalLayout_20 = QtWidgets.QVBoxLayout(self.tab_5)
+        self.verticalLayout_20.setObjectName("verticalLayout_20")
+        self.line_30 = QtWidgets.QFrame(self.tab_5)
+        self.line_30.setFrameShape(QtWidgets.QFrame.HLine)
+        self.line_30.setFrameShadow(QtWidgets.QFrame.Sunken)
+        self.line_30.setObjectName("line_30")
+        self.verticalLayout_20.addWidget(self.line_30)
+        self.label_86 = QtWidgets.QLabel(self.tab_5)
+        font = QtGui.QFont()
+        font.setPointSize(10)
+        font.setBold(True)
+        font.setWeight(75)
+        self.label_86.setFont(font)
+        self.label_86.setObjectName("label_86")
+        self.verticalLayout_20.addWidget(self.label_86)
+        self.formLayout_20 = QtWidgets.QFormLayout()
+        self.formLayout_20.setObjectName("formLayout_20")
+        self.label_93 = QtWidgets.QLabel(self.tab_5)
+        self.label_93.setObjectName("label_93")
+        self.formLayout_20.setWidget(0, QtWidgets.QFormLayout.LabelRole, self.label_93)
+        self.zoom_magnification = QtWidgets.QComboBox(self.tab_5)
+        self.zoom_magnification.setEditable(True)
+        self.zoom_magnification.setObjectName("zoom_magnification")
+        self.zoom_magnification.addItem("")
+        self.zoom_magnification.addItem("")
+        self.zoom_magnification.addItem("")
+        self.zoom_magnification.addItem("")
+        self.zoom_magnification.addItem("")
+        self.zoom_magnification.addItem("")
+        self.zoom_magnification.addItem("")
+        self.zoom_magnification.addItem("")
+        self.zoom_magnification.addItem("")
+        self.zoom_magnification.addItem("")
+        self.zoom_magnification.addItem("")
+        self.formLayout_20.setWidget(0, QtWidgets.QFormLayout.FieldRole, self.zoom_magnification)
+        self.verticalLayout_20.addLayout(self.formLayout_20)
+        self.zoom_apply = QtWidgets.QPushButton(self.tab_5)
+        self.zoom_apply.setObjectName("zoom_apply")
+        self.verticalLayout_20.addWidget(self.zoom_apply)
         spacerItem10 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
-        self.verticalLayout_5.addItem(spacerItem10)
+        self.verticalLayout_20.addItem(spacerItem10)
+        self.zoom_.addTab(self.tab_5, "")
+        self.verticalLayout_5.addWidget(self.zoom_)
+        spacerItem11 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        self.verticalLayout_5.addItem(spacerItem11)
         tab_widget.addTab(self.tab, "")
         self.segement_tab = QtWidgets.QWidget()
         self.segement_tab.setObjectName("segement_tab")
         self.verticalLayout_2 = QtWidgets.QVBoxLayout(self.segement_tab)
         self.verticalLayout_2.setObjectName("verticalLayout_2")
         self.line_12 = QtWidgets.QFrame(self.segement_tab)
         self.line_12.setFrameShape(QtWidgets.QFrame.HLine)
         self.line_12.setFrameShadow(QtWidgets.QFrame.Sunken)
         self.line_12.setObjectName("line_12")
         self.verticalLayout_2.addWidget(self.line_12)
         self.cellpose_select_custom_model = QtWidgets.QPushButton(self.segement_tab)
         self.cellpose_select_custom_model.setObjectName("cellpose_select_custom_model")
         self.verticalLayout_2.addWidget(self.cellpose_select_custom_model)
-        spacerItem11 = QtWidgets.QSpacerItem(20, 10, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
-        self.verticalLayout_2.addItem(spacerItem11)
+        spacerItem12 = QtWidgets.QSpacerItem(20, 10, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
+        self.verticalLayout_2.addItem(spacerItem12)
         self.tabWidget_3 = QtWidgets.QTabWidget(self.segement_tab)
         sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Preferred)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.tabWidget_3.sizePolicy().hasHeightForWidth())
         self.tabWidget_3.setSizePolicy(sizePolicy)
         self.tabWidget_3.setObjectName("tabWidget_3")
@@ -431,24 +475,24 @@
         self.cellpose_segmodel.addItem("")
         self.cellpose_segmodel.addItem("")
         self.cellpose_segmodel.addItem("")
         self.cellpose_segmodel.addItem("")
         self.cellpose_segmodel.addItem("")
         self.formLayout_12.setWidget(1, QtWidgets.QFormLayout.FieldRole, self.cellpose_segmodel)
         self.verticalLayout_10.addLayout(self.formLayout_12)
-        spacerItem12 = QtWidgets.QSpacerItem(20, 10, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
-        self.verticalLayout_10.addItem(spacerItem12)
+        spacerItem13 = QtWidgets.QSpacerItem(20, 10, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
+        self.verticalLayout_10.addItem(spacerItem13)
         self.cellpose_segment_active = QtWidgets.QPushButton(self.tab_6)
         self.cellpose_segment_active.setObjectName("cellpose_segment_active")
         self.verticalLayout_10.addWidget(self.cellpose_segment_active)
         self.cellpose_segment_all = QtWidgets.QPushButton(self.tab_6)
         self.cellpose_segment_all.setObjectName("cellpose_segment_all")
         self.verticalLayout_10.addWidget(self.cellpose_segment_all)
-        spacerItem13 = QtWidgets.QSpacerItem(20, 10, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
-        self.verticalLayout_10.addItem(spacerItem13)
+        spacerItem14 = QtWidgets.QSpacerItem(20, 10, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
+        self.verticalLayout_10.addItem(spacerItem14)
         self.formLayout_13 = QtWidgets.QFormLayout()
         self.formLayout_13.setObjectName("formLayout_13")
         self.cellpose_progressbar = QtWidgets.QProgressBar(self.tab_6)
         self.cellpose_progressbar.setMaximumSize(QtCore.QSize(16777215, 20))
         self.cellpose_progressbar.setProperty("value", 0)
         self.cellpose_progressbar.setObjectName("cellpose_progressbar")
         self.formLayout_13.setWidget(0, QtWidgets.QFormLayout.FieldRole, self.cellpose_progressbar)
@@ -506,16 +550,16 @@
         self.cellpose_trainmodel.addItem("")
         self.cellpose_trainmodel.addItem("")
         self.cellpose_trainmodel.addItem("")
         self.cellpose_trainmodel.addItem("")
         self.cellpose_trainmodel.addItem("")
         self.formLayout_15.setWidget(1, QtWidgets.QFormLayout.FieldRole, self.cellpose_trainmodel)
         self.verticalLayout_13.addLayout(self.formLayout_15)
-        spacerItem14 = QtWidgets.QSpacerItem(20, 10, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
-        self.verticalLayout_13.addItem(spacerItem14)
+        spacerItem15 = QtWidgets.QSpacerItem(20, 10, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        self.verticalLayout_13.addItem(spacerItem15)
         self.cellpose_save_dir = QtWidgets.QPushButton(self.tab_11)
         self.cellpose_save_dir.setObjectName("cellpose_save_dir")
         self.verticalLayout_13.addWidget(self.cellpose_save_dir)
         self.cellpose_train_model = QtWidgets.QPushButton(self.tab_11)
         self.cellpose_train_model.setObjectName("cellpose_train_model")
         self.verticalLayout_13.addWidget(self.cellpose_train_model)
         self.tabWidget_3.addTab(self.tab_11, "")
@@ -581,16 +625,16 @@
         self.label_4 = QtWidgets.QLabel(self.tab_12)
         self.label_4.setObjectName("label_4")
         self.gridLayout_2.addWidget(self.label_4, 3, 0, 1, 1)
         self.cellpose_diameter_label = QtWidgets.QLabel(self.tab_12)
         self.cellpose_diameter_label.setObjectName("cellpose_diameter_label")
         self.gridLayout_2.addWidget(self.cellpose_diameter_label, 3, 2, 1, 1)
         self.verticalLayout_14.addLayout(self.gridLayout_2)
-        spacerItem15 = QtWidgets.QSpacerItem(20, 10, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
-        self.verticalLayout_14.addItem(spacerItem15)
+        spacerItem16 = QtWidgets.QSpacerItem(20, 10, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        self.verticalLayout_14.addItem(spacerItem16)
         self.cellpose_clear_previous = QtWidgets.QCheckBox(self.tab_12)
         self.cellpose_clear_previous.setChecked(True)
         self.cellpose_clear_previous.setObjectName("cellpose_clear_previous")
         self.verticalLayout_14.addWidget(self.cellpose_clear_previous)
         self.cellpose_usegpu = QtWidgets.QCheckBox(self.tab_12)
         self.cellpose_usegpu.setChecked(True)
         self.cellpose_usegpu.setObjectName("cellpose_usegpu")
@@ -602,16 +646,16 @@
         self.tabWidget_3.addTab(self.tab_12, "")
         self.verticalLayout_2.addWidget(self.tabWidget_3)
         self.line_6 = QtWidgets.QFrame(self.segement_tab)
         self.line_6.setFrameShape(QtWidgets.QFrame.HLine)
         self.line_6.setFrameShadow(QtWidgets.QFrame.Sunken)
         self.line_6.setObjectName("line_6")
         self.verticalLayout_2.addWidget(self.line_6)
-        spacerItem16 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
-        self.verticalLayout_2.addItem(spacerItem16)
+        spacerItem17 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        self.verticalLayout_2.addItem(spacerItem17)
         tab_widget.addTab(self.segement_tab, "")
         self.tab_3 = QtWidgets.QWidget()
         self.tab_3.setEnabled(True)
         self.tab_3.setObjectName("tab_3")
         self.verticalLayout_3 = QtWidgets.QVBoxLayout(self.tab_3)
         self.verticalLayout_3.setObjectName("verticalLayout_3")
         self.line_4 = QtWidgets.QFrame(self.tab_3)
@@ -639,16 +683,16 @@
         self.modify_segment.setObjectName("modify_segment")
         self.gridLayout_3.addWidget(self.modify_segment, 0, 1, 1, 1)
         self.verticalLayout_3.addLayout(self.gridLayout_3)
         self.modify_auto_panzoom = QtWidgets.QCheckBox(self.tab_3)
         self.modify_auto_panzoom.setChecked(True)
         self.modify_auto_panzoom.setObjectName("modify_auto_panzoom")
         self.verticalLayout_3.addWidget(self.modify_auto_panzoom)
-        spacerItem17 = QtWidgets.QSpacerItem(334, 14, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
-        self.verticalLayout_3.addItem(spacerItem17)
+        spacerItem18 = QtWidgets.QSpacerItem(334, 14, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
+        self.verticalLayout_3.addItem(spacerItem18)
         self.line_18 = QtWidgets.QFrame(self.tab_3)
         self.line_18.setFrameShape(QtWidgets.QFrame.HLine)
         self.line_18.setFrameShadow(QtWidgets.QFrame.Sunken)
         self.line_18.setObjectName("line_18")
         self.verticalLayout_3.addWidget(self.line_18)
         self.label_16 = QtWidgets.QLabel(self.tab_3)
         font = QtGui.QFont()
@@ -675,16 +719,16 @@
         self.modify_split = QtWidgets.QPushButton(self.tab_3)
         self.modify_split.setObjectName("modify_split")
         self.gridLayout_4.addWidget(self.modify_split, 1, 0, 1, 1)
         self.modify_extend = QtWidgets.QPushButton(self.tab_3)
         self.modify_extend.setObjectName("modify_extend")
         self.gridLayout_4.addWidget(self.modify_extend, 0, 1, 1, 1)
         self.verticalLayout_3.addLayout(self.gridLayout_4)
-        spacerItem18 = QtWidgets.QSpacerItem(334, 14, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
-        self.verticalLayout_3.addItem(spacerItem18)
+        spacerItem19 = QtWidgets.QSpacerItem(334, 14, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
+        self.verticalLayout_3.addItem(spacerItem19)
         self.line_19 = QtWidgets.QFrame(self.tab_3)
         self.line_19.setFrameShape(QtWidgets.QFrame.HLine)
         self.line_19.setFrameShadow(QtWidgets.QFrame.Sunken)
         self.line_19.setObjectName("line_19")
         self.verticalLayout_3.addWidget(self.line_19)
         self.label_28 = QtWidgets.QLabel(self.tab_3)
         font = QtGui.QFont()
@@ -718,16 +762,16 @@
         self.classify_broken.setObjectName("classify_broken")
         self.gridLayout_5.addWidget(self.classify_broken, 1, 1, 1, 1)
         self.classify_single = QtWidgets.QPushButton(self.tab_3)
         self.classify_single.setStyleSheet("color: rgb(255, 255, 255);")
         self.classify_single.setObjectName("classify_single")
         self.gridLayout_5.addWidget(self.classify_single, 0, 0, 1, 1)
         self.verticalLayout_3.addLayout(self.gridLayout_5)
-        spacerItem19 = QtWidgets.QSpacerItem(334, 14, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
-        self.verticalLayout_3.addItem(spacerItem19)
+        spacerItem20 = QtWidgets.QSpacerItem(334, 14, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
+        self.verticalLayout_3.addItem(spacerItem20)
         self.line_21 = QtWidgets.QFrame(self.tab_3)
         self.line_21.setFrameShape(QtWidgets.QFrame.HLine)
         self.line_21.setFrameShadow(QtWidgets.QFrame.Sunken)
         self.line_21.setObjectName("line_21")
         self.verticalLayout_3.addWidget(self.line_21)
         self.label_14 = QtWidgets.QLabel(self.tab_3)
         font = QtGui.QFont()
@@ -810,16 +854,16 @@
         self.set_debris_4 = QtWidgets.QPushButton(self.tab_3)
         self.set_debris_4.setObjectName("set_debris_4")
         self.gridLayout_22.addWidget(self.set_debris_4, 0, 4, 1, 1)
         self.set_debris_5 = QtWidgets.QPushButton(self.tab_3)
         self.set_debris_5.setObjectName("set_debris_5")
         self.gridLayout_22.addWidget(self.set_debris_5, 0, 5, 1, 1)
         self.verticalLayout_3.addLayout(self.gridLayout_22)
-        spacerItem20 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
-        self.verticalLayout_3.addItem(spacerItem20)
+        spacerItem21 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        self.verticalLayout_3.addItem(spacerItem21)
         tab_widget.addTab(self.tab_3, "")
         self.tab_2 = QtWidgets.QWidget()
         self.tab_2.setObjectName("tab_2")
         self.verticalLayout_7 = QtWidgets.QVBoxLayout(self.tab_2)
         self.verticalLayout_7.setObjectName("verticalLayout_7")
         self.label_29 = QtWidgets.QLabel(self.tab_2)
         font = QtGui.QFont()
@@ -834,16 +878,16 @@
         self.oufti_panzoom_mode = QtWidgets.QRadioButton(self.tab_2)
         self.oufti_panzoom_mode.setObjectName("oufti_panzoom_mode")
         self.gridLayout_10.addWidget(self.oufti_panzoom_mode, 0, 0, 1, 1)
         self.oufti_edit_mode = QtWidgets.QRadioButton(self.tab_2)
         self.oufti_edit_mode.setObjectName("oufti_edit_mode")
         self.gridLayout_10.addWidget(self.oufti_edit_mode, 0, 1, 1, 1)
         self.verticalLayout_7.addLayout(self.gridLayout_10)
-        spacerItem21 = QtWidgets.QSpacerItem(360, 13, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
-        self.verticalLayout_7.addItem(spacerItem21)
+        spacerItem22 = QtWidgets.QSpacerItem(360, 13, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
+        self.verticalLayout_7.addItem(spacerItem22)
         self.label_20 = QtWidgets.QLabel(self.tab_2)
         font = QtGui.QFont()
         font.setPointSize(10)
         font.setBold(True)
         font.setWeight(75)
         self.label_20.setFont(font)
         self.label_20.setObjectName("label_20")
@@ -871,16 +915,16 @@
         self.gridLayout_17 = QtWidgets.QGridLayout()
         self.gridLayout_17.setObjectName("gridLayout_17")
         self.oufti_generate_all_midlines = QtWidgets.QPushButton(self.tab_2)
         self.oufti_generate_all_midlines.setObjectName("oufti_generate_all_midlines")
         self.gridLayout_17.addWidget(self.oufti_generate_all_midlines, 0, 0, 1, 1)
         self.gridLayout_16.addLayout(self.gridLayout_17, 0, 1, 1, 1)
         self.verticalLayout_7.addLayout(self.gridLayout_16)
-        spacerItem22 = QtWidgets.QSpacerItem(360, 13, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
-        self.verticalLayout_7.addItem(spacerItem22)
+        spacerItem23 = QtWidgets.QSpacerItem(360, 13, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
+        self.verticalLayout_7.addItem(spacerItem23)
         self.label_63 = QtWidgets.QLabel(self.tab_2)
         font = QtGui.QFont()
         font.setPointSize(10)
         font.setBold(True)
         font.setWeight(75)
         self.label_63.setFont(font)
         self.label_63.setObjectName("label_63")
@@ -890,16 +934,16 @@
         self.oufti_centre_active_midlines = QtWidgets.QPushButton(self.tab_2)
         self.oufti_centre_active_midlines.setObjectName("oufti_centre_active_midlines")
         self.gridLayout_15.addWidget(self.oufti_centre_active_midlines, 0, 0, 1, 1)
         self.oufti_centre_all_midlines = QtWidgets.QPushButton(self.tab_2)
         self.oufti_centre_all_midlines.setObjectName("oufti_centre_all_midlines")
         self.gridLayout_15.addWidget(self.oufti_centre_all_midlines, 0, 1, 1, 1)
         self.verticalLayout_7.addLayout(self.gridLayout_15)
-        spacerItem23 = QtWidgets.QSpacerItem(360, 13, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
-        self.verticalLayout_7.addItem(spacerItem23)
+        spacerItem24 = QtWidgets.QSpacerItem(360, 13, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
+        self.verticalLayout_7.addItem(spacerItem24)
         self.label_61 = QtWidgets.QLabel(self.tab_2)
         font = QtGui.QFont()
         font.setPointSize(10)
         font.setBold(True)
         font.setWeight(75)
         self.label_61.setFont(font)
         self.label_61.setObjectName("label_61")
@@ -935,16 +979,16 @@
         self.oufti_mesh_dilation.addItem("")
         self.oufti_mesh_dilation.addItem("")
         self.oufti_mesh_dilation.addItem("")
         self.oufti_mesh_dilation.addItem("")
         self.oufti_mesh_dilation.addItem("")
         self.formLayout_7.setWidget(1, QtWidgets.QFormLayout.FieldRole, self.oufti_mesh_dilation)
         self.verticalLayout_7.addLayout(self.formLayout_7)
-        spacerItem24 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
-        self.verticalLayout_7.addItem(spacerItem24)
+        spacerItem25 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        self.verticalLayout_7.addItem(spacerItem25)
         tab_widget.addTab(self.tab_2, "")
         self.upload_tab = QtWidgets.QWidget()
         self.upload_tab.setEnabled(True)
         self.upload_tab.setObjectName("upload_tab")
         self.verticalLayout_4 = QtWidgets.QVBoxLayout(self.upload_tab)
         self.verticalLayout_4.setObjectName("verticalLayout_4")
         self.line_24 = QtWidgets.QFrame(self.upload_tab)
@@ -977,16 +1021,16 @@
         self.display_database_path = QtWidgets.QLineEdit(self.upload_tab)
         self.display_database_path.setAlignment(QtCore.Qt.AlignCenter)
         self.display_database_path.setReadOnly(True)
         self.display_database_path.setClearButtonEnabled(False)
         self.display_database_path.setObjectName("display_database_path")
         self.formLayout_9.setWidget(0, QtWidgets.QFormLayout.FieldRole, self.display_database_path)
         self.verticalLayout_4.addLayout(self.formLayout_9)
-        spacerItem25 = QtWidgets.QSpacerItem(435, 20, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
-        self.verticalLayout_4.addItem(spacerItem25)
+        spacerItem26 = QtWidgets.QSpacerItem(435, 20, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
+        self.verticalLayout_4.addItem(spacerItem26)
         self.metadata_controls = QtWidgets.QTabWidget(self.upload_tab)
         sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Preferred)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.metadata_controls.sizePolicy().hasHeightForWidth())
         self.metadata_controls.setSizePolicy(sizePolicy)
         font = QtGui.QFont()
@@ -1322,16 +1366,16 @@
         self.label_stain_target.addItem("")
         self.label_stain_target.addItem("")
         self.formLayout_10.setWidget(3, QtWidgets.QFormLayout.FieldRole, self.label_stain_target)
         self.verticalLayout_8.addLayout(self.formLayout_10)
         self.label_overwrite = QtWidgets.QPushButton(self.image_metadata)
         self.label_overwrite.setObjectName("label_overwrite")
         self.verticalLayout_8.addWidget(self.label_overwrite)
-        spacerItem26 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
-        self.verticalLayout_8.addItem(spacerItem26)
+        spacerItem27 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        self.verticalLayout_8.addItem(spacerItem27)
         self.metadata_controls.addTab(self.image_metadata, "")
         self.user_metadata = QtWidgets.QWidget()
         self.user_metadata.setObjectName("user_metadata")
         self.verticalLayout_19 = QtWidgets.QVBoxLayout(self.user_metadata)
         self.verticalLayout_19.setObjectName("verticalLayout_19")
         self.formLayout_2 = QtWidgets.QFormLayout()
         self.formLayout_2.setObjectName("formLayout_2")
@@ -1380,23 +1424,23 @@
         self.formLayout_2.setWidget(5, QtWidgets.QFormLayout.LabelRole, self.label_92)
         self.upload_usermeta6 = QtWidgets.QComboBox(self.user_metadata)
         self.upload_usermeta6.setEnabled(True)
         self.upload_usermeta6.setEditable(True)
         self.upload_usermeta6.setObjectName("upload_usermeta6")
         self.formLayout_2.setWidget(5, QtWidgets.QFormLayout.FieldRole, self.upload_usermeta6)
         self.verticalLayout_19.addLayout(self.formLayout_2)
-        spacerItem27 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
-        self.verticalLayout_19.addItem(spacerItem27)
+        spacerItem28 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        self.verticalLayout_19.addItem(spacerItem28)
         self.metadata_controls.addTab(self.user_metadata, "")
         self.verticalLayout_4.addWidget(self.metadata_controls)
         self.update_metadata = QtWidgets.QPushButton(self.upload_tab)
         self.update_metadata.setObjectName("update_metadata")
         self.verticalLayout_4.addWidget(self.update_metadata)
-        spacerItem28 = QtWidgets.QSpacerItem(435, 20, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
-        self.verticalLayout_4.addItem(spacerItem28)
+        spacerItem29 = QtWidgets.QSpacerItem(435, 20, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
+        self.verticalLayout_4.addItem(spacerItem29)
         self.label_87 = QtWidgets.QLabel(self.upload_tab)
         font = QtGui.QFont()
         font.setPointSize(10)
         font.setBold(True)
         font.setWeight(75)
         self.label_87.setFont(font)
         self.label_87.setObjectName("label_87")
@@ -1422,16 +1466,16 @@
         self.upload_label_combo.addItem("")
         self.upload_label_combo.setItemText(0, "")
         self.upload_label_combo.addItem("")
         self.upload_label_combo.addItem("")
         self.upload_label_combo.addItem("")
         self.formLayout_16.setWidget(1, QtWidgets.QFormLayout.FieldRole, self.upload_label_combo)
         self.verticalLayout_4.addLayout(self.formLayout_16)
-        spacerItem29 = QtWidgets.QSpacerItem(435, 20, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
-        self.verticalLayout_4.addItem(spacerItem29)
+        spacerItem30 = QtWidgets.QSpacerItem(435, 20, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
+        self.verticalLayout_4.addItem(spacerItem30)
         self.tabWidget_2 = QtWidgets.QTabWidget(self.upload_tab)
         sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Preferred)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.tabWidget_2.sizePolicy().hasHeightForWidth())
         self.tabWidget_2.setSizePolicy(sizePolicy)
         self.tabWidget_2.setMaximumSize(QtCore.QSize(16777215, 500))
@@ -1561,16 +1605,16 @@
         self.overwrite_all_metadata.setObjectName("overwrite_all_metadata")
         self.gridLayout_25.addWidget(self.overwrite_all_metadata, 1, 0, 1, 1)
         self.overwrite_selected_metadata = QtWidgets.QCheckBox(self.tab_4)
         self.overwrite_selected_metadata.setEnabled(True)
         self.overwrite_selected_metadata.setObjectName("overwrite_selected_metadata")
         self.gridLayout_25.addWidget(self.overwrite_selected_metadata, 1, 1, 1, 1)
         self.verticalLayout_11.addLayout(self.gridLayout_25)
-        spacerItem30 = QtWidgets.QSpacerItem(435, 20, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
-        self.verticalLayout_11.addItem(spacerItem30)
+        spacerItem31 = QtWidgets.QSpacerItem(435, 20, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
+        self.verticalLayout_11.addItem(spacerItem31)
         self.database_upload_buttons_2 = QtWidgets.QGridLayout()
         self.database_upload_buttons_2.setObjectName("database_upload_buttons_2")
         self.upload_all = QtWidgets.QPushButton(self.tab_4)
         self.upload_all.setEnabled(True)
         self.upload_all.setObjectName("upload_all")
         self.database_upload_buttons_2.addWidget(self.upload_all, 0, 1, 1, 1)
         self.upload_active = QtWidgets.QPushButton(self.tab_4)
@@ -1587,16 +1631,16 @@
         self.gridLayout_18.addWidget(self.label_89, 0, 0, 1, 1)
         self.upload_progressbar = QtWidgets.QProgressBar(self.upload_tab)
         self.upload_progressbar.setEnabled(True)
         self.upload_progressbar.setProperty("value", 0)
         self.upload_progressbar.setObjectName("upload_progressbar")
         self.gridLayout_18.addWidget(self.upload_progressbar, 0, 1, 1, 1)
         self.verticalLayout_4.addLayout(self.gridLayout_18)
-        spacerItem31 = QtWidgets.QSpacerItem(20, 20, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
-        self.verticalLayout_4.addItem(spacerItem31)
+        spacerItem32 = QtWidgets.QSpacerItem(20, 20, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        self.verticalLayout_4.addItem(spacerItem32)
         tab_widget.addTab(self.upload_tab, "")
         self.export_tab = QtWidgets.QWidget()
         self.export_tab.setEnabled(True)
         self.export_tab.setObjectName("export_tab")
         self.verticalLayout_6 = QtWidgets.QVBoxLayout(self.export_tab)
         self.verticalLayout_6.setObjectName("verticalLayout_6")
         self.tabWidget_4 = QtWidgets.QTabWidget(self.export_tab)
@@ -1658,16 +1702,16 @@
         self.export_overwrite_setting.setObjectName("export_overwrite_setting")
         self.gridLayout_14.addWidget(self.export_overwrite_setting, 1, 1, 1, 1)
         self.export_image_setting = QtWidgets.QCheckBox(self.tab_8)
         self.export_image_setting.setChecked(True)
         self.export_image_setting.setObjectName("export_image_setting")
         self.gridLayout_14.addWidget(self.export_image_setting, 1, 0, 1, 1)
         self.verticalLayout_15.addLayout(self.gridLayout_14)
-        spacerItem32 = QtWidgets.QSpacerItem(20, 10, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
-        self.verticalLayout_15.addItem(spacerItem32)
+        spacerItem33 = QtWidgets.QSpacerItem(20, 10, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
+        self.verticalLayout_15.addItem(spacerItem33)
         self.label_12 = QtWidgets.QLabel(self.tab_8)
         font = QtGui.QFont()
         font.setPointSize(10)
         font.setBold(True)
         font.setWeight(75)
         self.label_12.setFont(font)
         self.label_12.setObjectName("label_12")
@@ -1689,16 +1733,16 @@
         self.export_mask_background = QtWidgets.QCheckBox(self.tab_8)
         self.export_mask_background.setObjectName("export_mask_background")
         self.gridLayout_19.addWidget(self.export_mask_background, 2, 1, 1, 1)
         self.export_crop_zoom = QtWidgets.QCheckBox(self.tab_8)
         self.export_crop_zoom.setObjectName("export_crop_zoom")
         self.gridLayout_19.addWidget(self.export_crop_zoom, 2, 2, 1, 1)
         self.verticalLayout_15.addLayout(self.gridLayout_19)
-        spacerItem33 = QtWidgets.QSpacerItem(20, 10, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
-        self.verticalLayout_15.addItem(spacerItem33)
+        spacerItem34 = QtWidgets.QSpacerItem(20, 10, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        self.verticalLayout_15.addItem(spacerItem34)
         self.export_active = QtWidgets.QPushButton(self.tab_8)
         self.export_active.setObjectName("export_active")
         self.verticalLayout_15.addWidget(self.export_active)
         self.export_all = QtWidgets.QPushButton(self.tab_8)
         self.export_all.setObjectName("export_all")
         self.verticalLayout_15.addWidget(self.export_all)
         self.tabWidget_4.addTab(self.tab_8, "")
@@ -1732,16 +1776,16 @@
         self.export_colicoords_mode.addItem("")
         self.export_colicoords_mode.addItem("")
         self.gridLayout_11.addWidget(self.export_colicoords_mode, 1, 1, 1, 1)
         self.label_52 = QtWidgets.QLabel(self.tab_9)
         self.label_52.setObjectName("label_52")
         self.gridLayout_11.addWidget(self.label_52, 0, 0, 1, 1)
         self.verticalLayout_17.addLayout(self.gridLayout_11)
-        spacerItem34 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
-        self.verticalLayout_17.addItem(spacerItem34)
+        spacerItem35 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        self.verticalLayout_17.addItem(spacerItem35)
         self.export_statistics_multithreaded = QtWidgets.QCheckBox(self.tab_9)
         self.export_statistics_multithreaded.setChecked(True)
         self.export_statistics_multithreaded.setObjectName("export_statistics_multithreaded")
         self.verticalLayout_17.addWidget(self.export_statistics_multithreaded)
         self.export_statistics_active = QtWidgets.QPushButton(self.tab_9)
         self.export_statistics_active.setObjectName("export_statistics_active")
         self.verticalLayout_17.addWidget(self.export_statistics_active)
@@ -1784,16 +1828,16 @@
         self.export_edge.setObjectName("export_edge")
         self.gridLayout.addWidget(self.export_edge, 1, 2, 1, 1)
         self.export_broken = QtWidgets.QCheckBox(self.tab_13)
         self.export_broken.setChecked(True)
         self.export_broken.setObjectName("export_broken")
         self.gridLayout.addWidget(self.export_broken, 1, 1, 1, 1)
         self.verticalLayout_16.addLayout(self.gridLayout)
-        spacerItem35 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
-        self.verticalLayout_16.addItem(spacerItem35)
+        spacerItem36 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        self.verticalLayout_16.addItem(spacerItem36)
         self.label_49 = QtWidgets.QLabel(self.tab_13)
         font = QtGui.QFont()
         font.setPointSize(10)
         font.setBold(True)
         font.setWeight(75)
         self.label_49.setFont(font)
         self.label_49.setObjectName("label_49")
@@ -1846,30 +1890,30 @@
         self.export_scalebar_thickness.addItem("")
         self.export_scalebar_thickness.addItem("")
         self.export_scalebar_thickness.addItem("")
         self.export_scalebar_thickness.addItem("")
         self.export_scalebar_thickness.addItem("")
         self.formLayout_19.setWidget(1, QtWidgets.QFormLayout.FieldRole, self.export_scalebar_thickness)
         self.verticalLayout_16.addLayout(self.formLayout_19)
-        spacerItem36 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
-        self.verticalLayout_16.addItem(spacerItem36)
+        spacerItem37 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        self.verticalLayout_16.addItem(spacerItem37)
         self.tabWidget_4.addTab(self.tab_13, "")
         self.verticalLayout_6.addWidget(self.tabWidget_4)
         self.formLayout_11 = QtWidgets.QFormLayout()
         self.formLayout_11.setObjectName("formLayout_11")
         self.label_33 = QtWidgets.QLabel(self.export_tab)
         self.label_33.setObjectName("label_33")
         self.formLayout_11.setWidget(0, QtWidgets.QFormLayout.LabelRole, self.label_33)
         self.export_progressbar = QtWidgets.QProgressBar(self.export_tab)
         self.export_progressbar.setProperty("value", 0)
         self.export_progressbar.setObjectName("export_progressbar")
         self.formLayout_11.setWidget(0, QtWidgets.QFormLayout.FieldRole, self.export_progressbar)
         self.verticalLayout_6.addLayout(self.formLayout_11)
-        spacerItem37 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
-        self.verticalLayout_6.addItem(spacerItem37)
+        spacerItem38 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        self.verticalLayout_6.addItem(spacerItem38)
         tab_widget.addTab(self.export_tab, "")
         self.tab_14 = QtWidgets.QWidget()
         self.tab_14.setObjectName("tab_14")
         self.verticalLayout_18 = QtWidgets.QVBoxLayout(self.tab_14)
         self.verticalLayout_18.setObjectName("verticalLayout_18")
         self.line_20 = QtWidgets.QFrame(self.tab_14)
         self.line_20.setFrameShape(QtWidgets.QFrame.HLine)
@@ -1887,16 +1931,16 @@
         self.verticalLayout_18.addWidget(self.modify_deleteotherimages)
         self.modify_deleteactivemasks = QtWidgets.QPushButton(self.tab_14)
         self.modify_deleteactivemasks.setObjectName("modify_deleteactivemasks")
         self.verticalLayout_18.addWidget(self.modify_deleteactivemasks)
         self.modify_deleteallmasks = QtWidgets.QPushButton(self.tab_14)
         self.modify_deleteallmasks.setObjectName("modify_deleteallmasks")
         self.verticalLayout_18.addWidget(self.modify_deleteallmasks)
-        spacerItem38 = QtWidgets.QSpacerItem(20, 20, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
-        self.verticalLayout_18.addItem(spacerItem38)
+        spacerItem39 = QtWidgets.QSpacerItem(20, 20, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
+        self.verticalLayout_18.addItem(spacerItem39)
         self.line_22 = QtWidgets.QFrame(self.tab_14)
         self.line_22.setFrameShape(QtWidgets.QFrame.HLine)
         self.line_22.setFrameShadow(QtWidgets.QFrame.Sunken)
         self.line_22.setObjectName("line_22")
         self.verticalLayout_18.addWidget(self.line_22)
         self.label_31 = QtWidgets.QLabel(self.tab_14)
         font = QtGui.QFont()
@@ -1926,16 +1970,16 @@
         self.formLayout.setWidget(0, QtWidgets.QFormLayout.LabelRole, self.label_17)
         self.modify_progressbar = QtWidgets.QProgressBar(self.tab_14)
         self.modify_progressbar.setProperty("value", 0)
         self.modify_progressbar.setTextVisible(True)
         self.modify_progressbar.setObjectName("modify_progressbar")
         self.formLayout.setWidget(0, QtWidgets.QFormLayout.FieldRole, self.modify_progressbar)
         self.verticalLayout_18.addLayout(self.formLayout)
-        spacerItem39 = QtWidgets.QSpacerItem(20, 20, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
-        self.verticalLayout_18.addItem(spacerItem39)
+        spacerItem40 = QtWidgets.QSpacerItem(20, 20, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
+        self.verticalLayout_18.addItem(spacerItem40)
         self.line_23 = QtWidgets.QFrame(self.tab_14)
         self.line_23.setFrameShape(QtWidgets.QFrame.HLine)
         self.line_23.setFrameShadow(QtWidgets.QFrame.Sunken)
         self.line_23.setObjectName("line_23")
         self.verticalLayout_18.addWidget(self.line_23)
         self.label_56 = QtWidgets.QLabel(self.tab_14)
         font = QtGui.QFont()
@@ -1961,16 +2005,16 @@
         self.find_criterion = QtWidgets.QComboBox(self.tab_14)
         self.find_criterion.setObjectName("find_criterion")
         self.find_criterion.addItem("")
         self.find_criterion.addItem("")
         self.find_criterion.addItem("")
         self.gridLayout_7.addWidget(self.find_criterion, 0, 0, 1, 1)
         self.verticalLayout_18.addLayout(self.gridLayout_7)
-        spacerItem40 = QtWidgets.QSpacerItem(20, 20, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
-        self.verticalLayout_18.addItem(spacerItem40)
+        spacerItem41 = QtWidgets.QSpacerItem(20, 20, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
+        self.verticalLayout_18.addItem(spacerItem41)
         self.label_70 = QtWidgets.QLabel(self.tab_14)
         font = QtGui.QFont()
         font.setPointSize(10)
         font.setBold(True)
         font.setWeight(75)
         self.label_70.setFont(font)
         self.label_70.setObjectName("label_70")
@@ -1989,23 +2033,23 @@
         self.align_active_image = QtWidgets.QPushButton(self.tab_14)
         self.align_active_image.setObjectName("align_active_image")
         self.gridLayout_26.addWidget(self.align_active_image, 0, 0, 1, 1)
         self.align_all_images = QtWidgets.QPushButton(self.tab_14)
         self.align_all_images.setObjectName("align_all_images")
         self.gridLayout_26.addWidget(self.align_all_images, 0, 1, 1, 1)
         self.verticalLayout_18.addLayout(self.gridLayout_26)
-        spacerItem41 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
-        self.verticalLayout_18.addItem(spacerItem41)
+        spacerItem42 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        self.verticalLayout_18.addItem(spacerItem42)
         tab_widget.addTab(self.tab_14, "")
 
         self.retranslateUi(tab_widget)
         tab_widget.setCurrentIndex(0)
         self.import_limit.setCurrentIndex(6)
         self.import_precision.setCurrentIndex(1)
-        self.tabWidget.setCurrentIndex(0)
+        self.zoom_.setCurrentIndex(0)
         self.unfold_tile_size.setCurrentIndex(3)
         self.unfold_tile_overlap.setCurrentIndex(3)
         self.tabWidget_3.setCurrentIndex(0)
         self.cellpose_nepochs.setCurrentIndex(3)
         self.cellpose_batchsize.setCurrentIndex(1)
         self.oufti_midline_vertexes.setCurrentIndex(0)
         self.oufti_mesh_length.setCurrentIndex(4)
@@ -2065,21 +2109,21 @@
         self.label_36.setText(_translate("tab_widget", "Progress"))
         tab_widget.setTabText(tab_widget.indexOf(self.import_tab), _translate("tab_widget", "Import"))
         self.label_60.setText(_translate("tab_widget", "Auto Contrast Adjustment"))
         self.import_auto_contrast.setText(_translate("tab_widget", "Auto Contrast Adjustment"))
         self.label_38.setText(_translate("tab_widget", "View Mask/Class Labels"))
         self.modify_viewlabels.setText(_translate("tab_widget", "View Class Labels [x]"))
         self.modify_viewmasks.setText(_translate("tab_widget", "View Masks [Z]"))
-        self.tabWidget.setTabText(self.tabWidget.indexOf(self.tab_16), _translate("tab_widget", "General"))
+        self.zoom_.setTabText(self.zoom_.indexOf(self.tab_16), _translate("tab_widget", "General"))
         self.label_47.setText(_translate("tab_widget", "Scale Bar Settings"))
         self.scalebar_show.setText(_translate("tab_widget", "Show Scale Bar"))
         self.scalebar_units.setItemText(0, _translate("tab_widget", "um"))
         self.scalebar_units.setItemText(1, _translate("tab_widget", "nm"))
         self.label_48.setText(_translate("tab_widget", "Pixel Resolution (um)"))
-        self.tabWidget.setTabText(self.tabWidget.indexOf(self.tab_7), _translate("tab_widget", "Scale Bar"))
+        self.zoom_.setTabText(self.zoom_.indexOf(self.tab_7), _translate("tab_widget", "Scale Bar"))
         self.label_73.setText(_translate("tab_widget", "Information Overlay Settings"))
         self.overlay_filename.setText(_translate("tab_widget", "File Name"))
         self.overlay_folder.setText(_translate("tab_widget", "Folder"))
         self.overlay_antibiotic.setText(_translate("tab_widget", "Antibiotic"))
         self.overlay_phenotype.setText(_translate("tab_widget", "Phenotype"))
         self.overlay_strain.setText(_translate("tab_widget", "Strain"))
         self.overlay_content.setText(_translate("tab_widget", "Content"))
@@ -2089,15 +2133,15 @@
         self.overlay_staintarget.setText(_translate("tab_widget", "Stain Target"))
         self.overlay_modality.setText(_translate("tab_widget", "Modality"))
         self.overlay_stain.setText(_translate("tab_widget", "Stain"))
         self.overlay_focus.setText(_translate("tab_widget", "Image Focus"))
         self.overlay_laplacian.setText(_translate("tab_widget", "Image Laplacian"))
         self.overlay_debris.setText(_translate("tab_widget", "Image Debris"))
         self.overlay_range.setText(_translate("tab_widget", "Image Range"))
-        self.tabWidget.setTabText(self.tabWidget.indexOf(self.tab_15), _translate("tab_widget", "Overlay"))
+        self.zoom_.setTabText(self.zoom_.indexOf(self.tab_15), _translate("tab_widget", "Overlay"))
         self.label_57.setText(_translate("tab_widget", "Unfold/Fold into Tiles"))
         self.unfold.setText(_translate("tab_widget", "Unfold"))
         self.fold.setText(_translate("tab_widget", "Fold"))
         self.label_58.setText(_translate("tab_widget", "Tile Size (Pixels)"))
         self.unfold_tile_size.setItemText(0, _translate("tab_widget", "100"))
         self.unfold_tile_size.setItemText(1, _translate("tab_widget", "200"))
         self.unfold_tile_size.setItemText(2, _translate("tab_widget", "300"))
@@ -2108,15 +2152,30 @@
         self.unfold_tile_overlap.setItemText(1, _translate("tab_widget", "20"))
         self.unfold_tile_overlap.setItemText(2, _translate("tab_widget", "30"))
         self.unfold_tile_overlap.setItemText(3, _translate("tab_widget", "50"))
         self.unfold_tile_overlap.setItemText(4, _translate("tab_widget", "100"))
         self.label_62.setText(_translate("tab_widget", "Mode"))
         self.unfold_mode.setItemText(0, _translate("tab_widget", "Nested Tiles"))
         self.unfold_mode.setItemText(1, _translate("tab_widget", "Smaller Images (Extra FOVs)"))
-        self.tabWidget.setTabText(self.tabWidget.indexOf(self.tab_17), _translate("tab_widget", "Fold/Unfold"))
+        self.zoom_.setTabText(self.zoom_.indexOf(self.tab_17), _translate("tab_widget", "Fold/Unfold"))
+        self.label_86.setText(_translate("tab_widget", "Zoom in/out at Specific Intervals"))
+        self.label_93.setText(_translate("tab_widget", "Magnification (%)"))
+        self.zoom_magnification.setItemText(0, _translate("tab_widget", "0 (Home)"))
+        self.zoom_magnification.setItemText(1, _translate("tab_widget", "10"))
+        self.zoom_magnification.setItemText(2, _translate("tab_widget", "20"))
+        self.zoom_magnification.setItemText(3, _translate("tab_widget", "30"))
+        self.zoom_magnification.setItemText(4, _translate("tab_widget", "40"))
+        self.zoom_magnification.setItemText(5, _translate("tab_widget", "50"))
+        self.zoom_magnification.setItemText(6, _translate("tab_widget", "100"))
+        self.zoom_magnification.setItemText(7, _translate("tab_widget", "200"))
+        self.zoom_magnification.setItemText(8, _translate("tab_widget", "300"))
+        self.zoom_magnification.setItemText(9, _translate("tab_widget", "400"))
+        self.zoom_magnification.setItemText(10, _translate("tab_widget", "500"))
+        self.zoom_apply.setText(_translate("tab_widget", "Apply Zoom"))
+        self.zoom_.setTabText(self.zoom_.indexOf(self.tab_5), _translate("tab_widget", "Zoom"))
         tab_widget.setTabText(tab_widget.indexOf(self.tab), _translate("tab_widget", "View"))
         self.cellpose_select_custom_model.setText(_translate("tab_widget", "Select Custom Cellpose Model"))
         self.label_2.setText(_translate("tab_widget", "Segmentation Channel"))
         self.label.setText(_translate("tab_widget", "Cellpose Model"))
         self.cellpose_segmodel.setItemText(0, _translate("tab_widget", "cyto"))
         self.cellpose_segmodel.setItemText(1, _translate("tab_widget", "nuclei"))
         self.cellpose_segmodel.setItemText(2, _translate("tab_widget", "tissuenet"))
```

### Comparing `napari-bacseg-1.0.5/src/napari_bacseg/bacseg_ui.ui` & `napari-bacseg-1.0.6/src/napari_bacseg/bacseg_ui.ui`

 * *Files 0% similar despite different names*

#### Comparing `napari-bacseg-1.0.5/src/napari_bacseg/bacseg_ui.ui` & `napari-bacseg-1.0.6/src/napari_bacseg/bacseg_ui.ui`

```diff
@@ -428,15 +428,15 @@
     </widget>
     <widget class="QWidget" name="tab">
       <attribute name="title">
         <string>View</string>
       </attribute>
       <layout class="QVBoxLayout" name="verticalLayout_5">
         <item>
-          <widget class="QTabWidget" name="tabWidget">
+          <widget class="QTabWidget" name="zoom_">
             <property name="sizePolicy">
               <sizepolicy hsizetype="Expanding" vsizetype="Preferred">
                 <horstretch>0</horstretch>
                 <verstretch>0</verstretch>
               </sizepolicy>
             </property>
             <property name="currentIndex">
@@ -962,14 +962,135 @@
                         <height>1</height>
                       </size>
                     </property>
                   </spacer>
                 </item>
               </layout>
             </widget>
+            <widget class="QWidget" name="tab_5">
+              <attribute name="title">
+                <string>Zoom</string>
+              </attribute>
+              <layout class="QVBoxLayout" name="verticalLayout_20">
+                <item>
+                  <widget class="Line" name="line_30">
+                    <property name="orientation">
+                      <enum>Qt::Horizontal</enum>
+                    </property>
+                  </widget>
+                </item>
+                <item>
+                  <widget class="QLabel" name="label_86">
+                    <property name="font">
+                      <font>
+                        <pointsize>10</pointsize>
+                        <weight>75</weight>
+                        <bold>true</bold>
+                      </font>
+                    </property>
+                    <property name="text">
+                      <string>Zoom in/out at Specific Intervals</string>
+                    </property>
+                  </widget>
+                </item>
+                <item>
+                  <layout class="QFormLayout" name="formLayout_20">
+                    <item row="0" column="0">
+                      <widget class="QLabel" name="label_93">
+                        <property name="text">
+                          <string>Magnification (%)</string>
+                        </property>
+                      </widget>
+                    </item>
+                    <item row="0" column="1">
+                      <widget class="QComboBox" name="zoom_magnification">
+                        <property name="editable">
+                          <bool>true</bool>
+                        </property>
+                        <item>
+                          <property name="text">
+                            <string>0 (Home)</string>
+                          </property>
+                        </item>
+                        <item>
+                          <property name="text">
+                            <string>10</string>
+                          </property>
+                        </item>
+                        <item>
+                          <property name="text">
+                            <string>20</string>
+                          </property>
+                        </item>
+                        <item>
+                          <property name="text">
+                            <string>30</string>
+                          </property>
+                        </item>
+                        <item>
+                          <property name="text">
+                            <string>40</string>
+                          </property>
+                        </item>
+                        <item>
+                          <property name="text">
+                            <string>50</string>
+                          </property>
+                        </item>
+                        <item>
+                          <property name="text">
+                            <string>100</string>
+                          </property>
+                        </item>
+                        <item>
+                          <property name="text">
+                            <string>200</string>
+                          </property>
+                        </item>
+                        <item>
+                          <property name="text">
+                            <string>300</string>
+                          </property>
+                        </item>
+                        <item>
+                          <property name="text">
+                            <string>400</string>
+                          </property>
+                        </item>
+                        <item>
+                          <property name="text">
+                            <string>500</string>
+                          </property>
+                        </item>
+                      </widget>
+                    </item>
+                  </layout>
+                </item>
+                <item>
+                  <widget class="QPushButton" name="zoom_apply">
+                    <property name="text">
+                      <string>Apply Zoom</string>
+                    </property>
+                  </widget>
+                </item>
+                <item>
+                  <spacer name="verticalSpacer_7">
+                    <property name="orientation">
+                      <enum>Qt::Vertical</enum>
+                    </property>
+                    <property name="sizeHint" stdset="0">
+                      <size>
+                        <width>20</width>
+                        <height>40</height>
+                      </size>
+                    </property>
+                  </spacer>
+                </item>
+              </layout>
+            </widget>
           </widget>
         </item>
         <item>
           <spacer name="verticalSpacer_6">
             <property name="orientation">
               <enum>Qt::Vertical</enum>
             </property>
```

### Comparing `napari-bacseg-1.0.5/src/napari_bacseg.egg-info/PKG-INFO` & `napari-bacseg-1.0.6/src/napari_bacseg.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-bacseg
-Version: 1.0.5
+Version: 1.0.6
 Summary: Bacterial segmentation and analysis platform than can inport/export files in multiple formats. Integrating many tools such as Cellpose, ColiCoords, Oufti/MicrobeTracker.
 Home-page: https://github.com/piedrro/napari-bacseg
 Author: Piers Turner
 Author-email: Piers Turner <piers.turner@physics.ox.ac.uk>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/piedrro/napari-bacseg
 Project-URL: Bug Tracker, https://github.com/piedrro/napari-bacseg/issues
```

### Comparing `napari-bacseg-1.0.5/src/napari_bacseg.egg-info/SOURCES.txt` & `napari-bacseg-1.0.6/src/napari_bacseg.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -37,26 +37,28 @@
 src/_dev/get_akseg_stats.py
 src/_dev/get_species_info.py
 src/_dev/luke__script.py
 src/_dev/matplotlib_Events.py
 src/_dev/move_AluGasketDFP.py
 src/_dev/move_AluGasketDFP_poster.py
 src/_dev/move_AluGasketv12_DFP.py
+src/_dev/move_AluGasketv12_DFP_Titration.py
 src/_dev/move_conor_nim_dfp_data.py
 src/_dev/move_pillar_data.py
 src/_dev/move_pillar_zstack_data.py
 src/_dev/move_unlearning_files.py
 src/_dev/new_metadata2.pickle.py
 src/_dev/new_read_akseg_directory.py
 src/_dev/nim_dev.py
 src/_dev/omnipose_dev.py
 src/_dev/omnipose_midlines.py
 src/_dev/omnipose_train.py
 src/_dev/oufti_dilate.py
 src/_dev/oufti_dilate_with_midlines.py
+src/_dev/pandas_speed.py
 src/_dev/process_alex_datadump.py
 src/_dev/process_alex_datadump_clinical.py
 src/_dev/process_conor_datadump.py
 src/_dev/process_gramstain_datadump.py
 src/_dev/read_non_tif.py
 src/_dev/rebuild_usermeta.py
 src/_dev/rebuild_usermeta_2.py
```

### Comparing `napari-bacseg-1.0.5/tox.ini` & `napari-bacseg-1.0.6/tox.ini`

 * *Files identical despite different names*

