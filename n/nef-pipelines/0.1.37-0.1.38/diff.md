# Comparing `tmp/nef_pipelines-0.1.37.tar.gz` & `tmp/nef_pipelines-0.1.38.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nef_pipelines-0.1.37.tar", last modified: Thu May  4 07:52:41 2023, max compression
+gzip compressed data, was "nef_pipelines-0.1.38.tar", last modified: Sat May  6 21:01:46 2023, max compression
```

## Comparing `nef_pipelines-0.1.37.tar` & `nef_pipelines-0.1.38.tar`

### file list

```diff
@@ -1,353 +1,366 @@
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-04 07:52:41.316365 nef_pipelines-0.1.37/
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-04 07:52:40.349801 nef_pipelines-0.1.37/.github/
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-04 07:52:40.430643 nef_pipelines-0.1.37/.github/workflows/
--rw-r--r--   0 garythompson   (501) staff       (20)     4094 2023-02-01 22:03:42.000000 nef_pipelines-0.1.37/.github/workflows/ci.yml
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-04 07:52:40.458955 nef_pipelines-0.1.37/.idea/
--rw-r--r--   0 garythompson   (501) staff       (20)      176 2022-11-25 17:14:12.000000 nef_pipelines-0.1.37/.idea/.gitignore
--rw-r--r--   0 garythompson   (501) staff       (20)       14 2022-11-26 23:48:55.000000 nef_pipelines-0.1.37/.idea/.name
--rw-r--r--   0 garythompson   (501) staff       (20)      299 2023-01-11 23:02:58.000000 nef_pipelines-0.1.37/.idea/NFC.iml
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-04 07:52:40.462954 nef_pipelines-0.1.37/.idea/inspectionProfiles/
--rw-r--r--   0 garythompson   (501) staff       (20)     1184 2023-01-11 23:02:58.000000 nef_pipelines-0.1.37/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0 garythompson   (501) staff       (20)      175 2023-01-11 23:02:58.000000 nef_pipelines-0.1.37/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 garythompson   (501) staff       (20)      287 2023-01-11 23:02:58.000000 nef_pipelines-0.1.37/.idea/modules.xml
--rw-r--r--   0 garythompson   (501) staff       (20)      325 2023-04-26 19:24:39.000000 nef_pipelines-0.1.37/.idea/vcs.xml
--rw-r--r--   0 garythompson   (501) staff       (20)     1331 2022-11-26 14:34:37.000000 nef_pipelines-0.1.37/.pre-commit-config.yaml
--rw-r--r--   0 garythompson   (501) staff       (20)      490 2022-11-26 14:33:30.000000 nef_pipelines-0.1.37/.readthedocs.yml
--rw-r--r--   0 garythompson   (501) staff       (20)      372 2023-02-07 22:36:51.000000 nef_pipelines-0.1.37/AUTHORS.md
--rw-r--r--   0 garythompson   (501) staff       (20)     3377 2023-05-04 07:51:41.000000 nef_pipelines-0.1.37/CHANGELOG.md
--rw-r--r--   0 garythompson   (501) staff       (20)    12299 2022-11-27 14:11:11.000000 nef_pipelines-0.1.37/CONTRIBUTING.md
--rw-r--r--   0 garythompson   (501) staff       (20)    24410 2022-11-27 14:11:12.000000 nef_pipelines-0.1.37/LICENSE.txt
--rw-r--r--   0 garythompson   (501) staff       (20)     8765 2023-05-04 07:52:41.316712 nef_pipelines-0.1.37/PKG-INFO
--rw-r--r--   0 garythompson   (501) staff       (20)     8212 2023-02-07 22:28:55.000000 nef_pipelines-0.1.37/README.md
--rw-r--r--   0 garythompson   (501) staff       (20)      826 2023-02-05 15:31:16.000000 nef_pipelines-0.1.37/TODO.md
--rw-r--r--   0 garythompson   (501) staff       (20)      346 2023-01-31 22:56:36.000000 nef_pipelines-0.1.37/pyproject.toml
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-04 07:52:40.471753 nef_pipelines-0.1.37/references/
--rw-r--r--   0 garythompson   (501) staff       (20)    22346 2023-04-16 16:41:23.000000 nef_pipelines-0.1.37/references/Nmr Experiment Nomenclature v2.docx
--rw-r--r--   0 garythompson   (501) staff       (20)   282399 2023-04-16 14:33:43.000000 nef_pipelines-0.1.37/references/fogh.vrankenj.bio.nmr.2006.36.147.pdf
--rw-r--r--   0 garythompson   (501) staff       (20)     1229 2023-04-17 21:03:23.000000 nef_pipelines-0.1.37/release_to_pypi.sh
--rw-r--r--   0 garythompson   (501) staff       (20)      354 2023-04-17 20:13:08.000000 nef_pipelines-0.1.37/requirements.txt
--rw-r--r--   0 garythompson   (501) staff       (20)     1630 2023-05-04 07:52:41.321273 nef_pipelines-0.1.37/setup.cfg
--rw-r--r--   0 garythompson   (501) staff       (20)      710 2022-11-26 14:33:30.000000 nef_pipelines-0.1.37/setup.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-04 07:52:40.351180 nef_pipelines-0.1.37/src/
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-04 07:52:40.491038 nef_pipelines-0.1.37/src/nef_pipelines/
--rw-r--r--   0 garythompson   (501) staff       (20)        6 2023-03-23 08:31:34.000000 nef_pipelines-0.1.37/src/nef_pipelines/VERSION
--rw-r--r--   0 garythompson   (501) staff       (20)      577 2022-11-27 18:49:20.000000 nef_pipelines-0.1.37/src/nef_pipelines/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)       62 2022-11-27 18:48:20.000000 nef_pipelines-0.1.37/src/nef_pipelines/__main__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-04 07:52:40.530154 nef_pipelines-0.1.37/src/nef_pipelines/data/
--rw-r--r--   0 garythompson   (501) staff       (20)  1486198 2023-01-31 10:45:30.000000 nef_pipelines-0.1.37/src/nef_pipelines/data/mmcif_nef_v1_1.dic
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-04 07:52:40.583161 nef_pipelines-0.1.37/src/nef_pipelines/lib/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.37/src/nef_pipelines/lib/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)      124 2023-02-07 22:55:44.000000 nef_pipelines-0.1.37/src/nef_pipelines/lib/constants.py
--rw-r--r--   0 garythompson   (501) staff       (20)     1297 2022-11-27 19:40:25.000000 nef_pipelines-0.1.37/src/nef_pipelines/lib/header_lib.py
--rw-r--r--   0 garythompson   (501) staff       (20)      945 2023-03-19 15:38:08.000000 nef_pipelines-0.1.37/src/nef_pipelines/lib/isotope_lib.py
--rw-r--r--   0 garythompson   (501) staff       (20)     2812 2023-04-26 21:04:53.000000 nef_pipelines-0.1.37/src/nef_pipelines/lib/nef_frames_lib.py
--rw-r--r--   0 garythompson   (501) staff       (20)    16143 2023-04-15 16:57:10.000000 nef_pipelines-0.1.37/src/nef_pipelines/lib/nef_lib.py
--rw-r--r--   0 garythompson   (501) staff       (20)    15051 2023-05-04 07:18:02.000000 nef_pipelines-0.1.37/src/nef_pipelines/lib/peak_lib.py
--rw-r--r--   0 garythompson   (501) staff       (20)    21187 2023-04-30 15:31:02.000000 nef_pipelines-0.1.37/src/nef_pipelines/lib/sequence_lib.py
--rw-r--r--   0 garythompson   (501) staff       (20)     6348 2023-02-07 21:12:56.000000 nef_pipelines-0.1.37/src/nef_pipelines/lib/shift_lib.py
--rw-r--r--   0 garythompson   (501) staff       (20)     6548 2023-04-17 20:48:44.000000 nef_pipelines-0.1.37/src/nef_pipelines/lib/spectra_lib.py
--rw-r--r--   0 garythompson   (501) staff       (20)     4083 2023-05-04 07:17:17.000000 nef_pipelines-0.1.37/src/nef_pipelines/lib/structures.py
--rw-r--r--   0 garythompson   (501) staff       (20)    10234 2023-04-26 19:21:33.000000 nef_pipelines-0.1.37/src/nef_pipelines/lib/test_lib.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-04 07:52:40.588466 nef_pipelines-0.1.37/src/nef_pipelines/lib/translation/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.37/src/nef_pipelines/lib/translation/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)      292 2022-11-27 18:48:20.000000 nef_pipelines-0.1.37/src/nef_pipelines/lib/typer_utils.py
--rw-r--r--   0 garythompson   (501) staff       (20)    22250 2023-04-17 20:19:05.000000 nef_pipelines-0.1.37/src/nef_pipelines/lib/util.py
--rwxr-xr-x   0 garythompson   (501) staff       (20)     5239 2023-05-04 07:48:46.000000 nef_pipelines-0.1.37/src/nef_pipelines/main.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-04 07:52:40.588995 nef_pipelines-0.1.37/src/nef_pipelines/nef_app/
--rw-r--r--   0 garythompson   (501) staff       (20)       49 2022-11-27 18:48:20.000000 nef_pipelines-0.1.37/src/nef_pipelines/nef_app/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-04 07:52:40.611157 nef_pipelines-0.1.37/src/nef_pipelines/tests/
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-04 07:52:40.627546 nef_pipelines-0.1.37/src/nef_pipelines/tests/chains/
--rwxr--r--   0 garythompson   (501) staff       (20)        0 2022-11-25 17:14:10.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/chains/__init__.py
--rwxr-xr-x   0 garythompson   (501) staff       (20)     5259 2023-03-18 23:31:39.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/chains/test_clone.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-04 07:52:40.631659 nef_pipelines-0.1.37/src/nef_pipelines/tests/chains/test_data/
--rwxr--r--   0 garythompson   (501) staff       (20)      581 2022-11-25 17:14:10.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/chains/test_data/3aa.nef
--rwxr-xr-x   0 garythompson   (501) staff       (20)      837 2023-03-18 23:31:39.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/chains/test_data/3aa_x3.nef
--rwxr--r--   0 garythompson   (501) staff       (20)     2172 2022-12-16 20:37:04.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/chains/test_data/multi_chain_shifts.nef
--rwxr--r--   0 garythompson   (501) staff       (20)      491 2022-12-16 20:38:38.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/chains/test_list.py
--rwxr-xr-x   0 garythompson   (501) staff       (20)    10032 2023-03-18 23:31:39.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/chains/test_rename.py
--rwxr--r--   0 garythompson   (501) staff       (20)     9304 2023-01-30 23:11:50.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/chains/test_renumber.py
--rw-r--r--   0 garythompson   (501) staff       (20)      709 2023-01-12 09:57:27.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/conftest.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-04 07:52:40.637857 nef_pipelines-0.1.37/src/nef_pipelines/tests/csv/
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-04 07:52:40.640586 nef_pipelines-0.1.37/src/nef_pipelines/tests/csv/test_data/
--rw-r--r--   0 garythompson   (501) staff       (20)       45 2023-01-31 08:50:56.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/csv/test_data/short.csv
--rw-r--r--   0 garythompson   (501) staff       (20)      218 2023-01-31 08:49:14.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/csv/test_data/short_complete.csv
--rw-r--r--   0 garythompson   (501) staff       (20)     5079 2023-01-31 22:17:03.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/csv/test_import_rdcs.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-04 07:52:40.641837 nef_pipelines-0.1.37/src/nef_pipelines/tests/fasta/
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-04 07:52:40.645232 nef_pipelines-0.1.37/src/nef_pipelines/tests/fasta/test_data/
--rwxr--r--   0 garythompson   (501) staff       (20)       11 2022-12-06 19:49:15.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/fasta/test_data/3aa.fasta
--rwxr-xr-x   0 garythompson   (501) staff       (20)       24 2023-03-18 23:31:39.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/fasta/test_data/3aa_x2.fasta
--rwxr-xr-x   0 garythompson   (501) staff       (20)     3178 2023-03-18 23:31:39.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/fasta/test_sequence.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-04 07:52:40.661303 nef_pipelines-0.1.37/src/nef_pipelines/tests/frames/
--rwxr--r--   0 garythompson   (501) staff       (20)        0 2022-12-06 20:53:09.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/frames/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-04 07:52:40.665095 nef_pipelines-0.1.37/src/nef_pipelines/tests/frames/test_data/
--rwxr-xr-x   0 garythompson   (501) staff       (20)     1470 2023-03-18 23:31:39.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/frames/test_data/frames.nef
--rwxr--r--   0 garythompson   (501) staff       (20)     1626 2022-12-16 21:06:02.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/frames/test_data/pales_test_1.nef
--rwxr--r--   0 garythompson   (501) staff       (20)     2690 2022-12-16 21:06:48.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/frames/test_delete.py
--rwxr-xr-x   0 garythompson   (501) staff       (20)     1123 2023-04-15 16:57:25.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/frames/test_list.py
--rwxr--r--   0 garythompson   (501) staff       (20)    10090 2023-04-15 16:15:29.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/frames/test_rename.py
--rwxr-xr-x   0 garythompson   (501) staff       (20)     1312 2023-03-18 23:31:39.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/frames/test_tabulate.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-04 07:52:40.673918 nef_pipelines-0.1.37/src/nef_pipelines/tests/mars/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-02-05 13:08:51.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/mars/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-04 07:52:40.682391 nef_pipelines-0.1.37/src/nef_pipelines/tests/mars/test_data/
--rw-r--r--   0 garythompson   (501) staff       (20)     9631 2023-02-01 22:03:42.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/mars/test_data/sec5_short.neff
--rw-r--r--   0 garythompson   (501) staff       (20)      311 2023-02-05 15:30:43.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/mars/test_data/sec5_short.txt
--rw-r--r--   0 garythompson   (501) staff       (20)      838 2023-02-01 22:29:59.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/mars/test_export_shifts.py
--rw-r--r--   0 garythompson   (501) staff       (20)     2537 2023-02-05 15:30:44.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/mars/test_import_shifts.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-04 07:52:40.706778 nef_pipelines-0.1.37/src/nef_pipelines/tests/nmrpipe/
--rwxr--r--   0 garythompson   (501) staff       (20)        0 2022-12-10 21:27:09.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/nmrpipe/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-04 07:52:40.748385 nef_pipelines-0.1.37/src/nef_pipelines/tests/nmrpipe/test_data/
--rwxr-xr-x   0 garythompson   (501) staff       (20)       12 2023-03-18 23:31:39.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/nmrpipe/test_data/3aa.seq
--rwxr--r--   0 garythompson   (501) staff       (20)       18 2022-12-16 20:31:09.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/nmrpipe/test_data/3aa.tab
--rwxr-xr-x   0 garythompson   (501) staff       (20)       15 2023-03-18 23:31:39.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/nmrpipe/test_data/3aa10.seq
--rwxr--r--   0 garythompson   (501) staff       (20)       16 2022-12-16 20:31:09.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/nmrpipe/test_data/4peaks.seq
--rw-------   0 garythompson   (501) staff       (20)      455 2023-01-10 13:25:00.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/nmrpipe/test_data/P3a_l273R_nmrpipe_shifts_short.tab
--rwxr--r--   0 garythompson   (501) staff       (20)    10961 2022-12-16 20:31:08.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/nmrpipe/test_data/gb3.tab
--rwxr--r--   0 garythompson   (501) staff       (20)    11038 2022-12-16 20:31:08.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned.tab
--rwxr-xr-x   0 garythompson   (501) staff       (20)      943 2023-03-18 23:31:39.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned_trunc.tab
--rwxr-xr-x   0 garythompson   (501) staff       (20)     1878 2023-03-18 23:31:39.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned_trunc_expected.tab
--rwxr--r--   0 garythompson   (501) staff       (20)    26327 2022-12-16 20:31:09.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/nmrpipe/test_data/ns3_S135A_BMRB1.txt
--rwxr--r--   0 garythompson   (501) staff       (20)      247 2022-12-16 20:31:09.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/nmrpipe/test_data/ns3_S135A_BMRB1_short.txt
--rwxr-xr-x   0 garythompson   (501) staff       (20)      800 2023-03-18 23:31:39.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/nmrpipe/test_data/test_header_entry.txt
--rwxr-xr-x   0 garythompson   (501) staff       (20)    14392 2023-04-24 21:03:24.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/nmrpipe/test_gdb.py
--rwxr--r--   0 garythompson   (501) staff       (20)      840 2022-12-16 20:35:58.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/nmrpipe/test_peaks.py
--rwxr--r--   0 garythompson   (501) staff       (20)      486 2022-12-16 20:35:58.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/nmrpipe/test_pipe_lib.py
--rwxr-xr-x   0 garythompson   (501) staff       (20)     4158 2023-03-18 23:31:39.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/nmrpipe/test_sequence.py
--rwxr-xr-x   0 garythompson   (501) staff       (20)     4454 2023-01-18 07:36:14.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/nmrpipe/test_shifts.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-04 07:52:40.780958 nef_pipelines-0.1.37/src/nef_pipelines/tests/nmrview/
--rwxr--r--   0 garythompson   (501) staff       (20)        0 2022-12-11 15:04:32.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/nmrview/__init__.py
--rwxr--r--   0 garythompson   (501) staff       (20)    10752 2022-12-17 11:29:00.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/nmrview/tcl_diag.html
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-04 07:52:40.829890 nef_pipelines-0.1.37/src/nef_pipelines/tests/nmrview/test_data/
--rwxr--r--   0 garythompson   (501) staff       (20)       12 2022-12-11 15:04:32.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/nmrview/test_data/3aa.seq
--rwxr--r--   0 garythompson   (501) staff       (20)       15 2022-12-11 15:04:32.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/nmrview/test_data/3aa10.seq
--rwxr--r--   0 garythompson   (501) staff       (20)       16 2022-12-17 11:29:00.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/nmrview/test_data/4peaks.seq
--rwxr-xr-x   0 garythompson   (501) staff       (20)      980 2023-03-18 23:31:39.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/nmrview/test_data/4peaks.xpk
--rwxr--r--   0 garythompson   (501) staff       (20)      880 2022-12-11 15:04:32.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/nmrview/test_data/expected_nmr_view.xpk
--rwxr-xr-x   0 garythompson   (501) staff       (20)     2178 2023-03-18 23:31:39.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/nmrview/test_data/expected_sequence_and_peaks_nmrview.txt
--rwxr--r--   0 garythompson   (501) staff       (20)      319 2022-12-11 15:04:32.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/nmrview/test_data/joe_clic.xpk
--rwxr--r--   0 garythompson   (501) staff       (20)     2172 2022-12-11 15:04:32.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/nmrview/test_data/nmrview_expected_4aa.txt
--rwxr--r--   0 garythompson   (501) staff       (20)    29631 2022-12-11 15:04:32.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/nmrview/test_data/ppm.out
--rwxr--r--   0 garythompson   (501) staff       (20)      540 2022-12-11 15:04:32.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/nmrview/test_data/ppm_out.seq
--rwxr--r--   0 garythompson   (501) staff       (20)       12 2022-12-11 15:04:32.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/nmrview/test_data/ppm_out_short.seq
--rwxr--r--   0 garythompson   (501) staff       (20)      126 2022-12-11 15:04:32.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/nmrview/test_data/ppm_short.out
--rwxr--r--   0 garythompson   (501) staff       (20)      522 2022-12-17 11:29:00.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/nmrview/test_data/ppm_short_seq.nef
--rwxr--r--   0 garythompson   (501) staff       (20)      800 2022-12-11 15:05:20.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/nmrview/test_data/test_header_entry.txt
--rwxr-xr-x   0 garythompson   (501) staff       (20)     2646 2023-03-18 23:31:39.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/nmrview/test_export_peaks.py
--rwxr--r--   0 garythompson   (501) staff       (20)     3343 2023-01-14 17:44:39.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/nmrview/test_export_sequences.py
--rwxr-xr-x   0 garythompson   (501) staff       (20)     3872 2023-02-15 22:22:17.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/nmrview/test_import_peaks.py
--rwxr-xr-x   0 garythompson   (501) staff       (20)     3915 2023-02-07 23:04:20.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/nmrview/test_import_sequence.py
--rwxr-xr-x   0 garythompson   (501) staff       (20)     4734 2023-01-18 07:36:14.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/nmrview/test_import_shifts.py
--rwxr-xr-x   0 garythompson   (501) staff       (20)     2166 2023-03-18 23:31:39.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/nmrview/test_tcl.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-04 07:52:40.840075 nef_pipelines-0.1.37/src/nef_pipelines/tests/pales/
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-04 07:52:40.844087 nef_pipelines-0.1.37/src/nef_pipelines/tests/pales/test_data/
--rwxr--r--   0 garythompson   (501) staff       (20)     1626 2022-12-17 16:34:00.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/pales/test_data/pales_test_1.nef
--rwxr--r--   0 garythompson   (501) staff       (20)     1627 2022-12-17 16:34:00.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/pales/test_data/pales_test_2.nef
--rwxr--r--   0 garythompson   (501) staff       (20)     1647 2023-01-27 21:30:12.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/pales/test_data/pales_test_segids.nef
--rwxr-xr-x   0 garythompson   (501) staff       (20)     2773 2023-01-30 23:21:17.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/pales/test_rdcs.py
--rwxr-xr-x   0 garythompson   (501) staff       (20)     2043 2023-03-18 23:31:39.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/pales/test_template.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-04 07:52:40.845669 nef_pipelines-0.1.37/src/nef_pipelines/tests/pdbx/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-01-31 19:44:59.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/pdbx/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-04 07:52:40.858910 nef_pipelines-0.1.37/src/nef_pipelines/tests/pdbx/test_data/
--rwxr-xr-x   0 garythompson   (501) staff       (20)     4795 2023-03-18 23:31:39.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/pdbx/test_data/3a_ab.pdb
--rwxr--r--   0 garythompson   (501) staff       (20)     4795 2022-12-17 16:52:18.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/pdbx/test_data/3a_cccc_dddd.pdb
--rwxr--r--   0 garythompson   (501) staff       (20)     4195 2022-12-17 16:52:18.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/pdbx/test_data/3a_no_chain_no_segid.pdb
--rwxr--r--   0 garythompson   (501) staff       (20)     2395 2022-12-17 16:52:18.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/pdbx/test_data/3aa.pdb
--rwxr--r--   0 garythompson   (501) staff       (20)     2254 2022-12-17 16:52:18.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/pdbx/test_data/3aa11_13.pdb
--rwxr--r--   0 garythompson   (501) staff       (20)      800 2022-12-10 20:00:10.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/pdbx/test_data/test_header_entry.txt
--rwxr-xr-x   0 garythompson   (501) staff       (20)     4248 2023-01-15 11:02:28.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/pdbx/test_sequence.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-04 07:52:40.875156 nef_pipelines-0.1.37/src/nef_pipelines/tests/shifts/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-04-16 09:07:56.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/shifts/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)     8438 2023-04-17 20:44:38.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/shifts/test_make_peaks.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-04 07:52:40.880583 nef_pipelines-0.1.37/src/nef_pipelines/tests/shifty/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-02-09 08:07:44.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/shifty/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)      773 2023-02-09 08:08:24.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/shifty/test_export_shifts.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-04 07:52:40.895003 nef_pipelines-0.1.37/src/nef_pipelines/tests/sparky/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-04-26 18:29:03.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/sparky/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-04 07:52:40.936111 nef_pipelines-0.1.37/src/nef_pipelines/tests/sparky/test_data/
--rw-r--r--   0 garythompson   (501) staff       (20)     1393 2023-01-31 21:17:52.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/sparky/test_data/P3a_L273R_sequence_short.neff
--rw-r--r--   0 garythompson   (501) staff       (20)     2342 2023-03-19 00:02:41.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/sparky/test_data/peaks_short_with_assignments.neff
--rw-r--r--   0 garythompson   (501) staff       (20)       40 2023-04-26 18:38:57.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/sparky/test_data/sparky_basic_sequence_dna.txt
--rw-r--r--   0 garythompson   (501) staff       (20)        9 2023-04-26 18:38:57.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/sparky/test_data/sparky_basic_sequence_protein.txt
--rw-r--r--   0 garythompson   (501) staff       (20)      241 2023-04-26 21:06:34.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/sparky/test_data/sparky_manual_basic.peaks
--rw-r--r--   0 garythompson   (501) staff       (20)     1187 2023-04-26 18:24:37.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/sparky/test_data/sparky_manual_basic_sequence.nef
--rw-r--r--   0 garythompson   (501) staff       (20)      359 2023-04-26 19:32:49.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/sparky/test_data/sparky_manual_full.peaks
--rw-r--r--   0 garythompson   (501) staff       (20)      422 2023-04-26 20:35:49.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/sparky/test_data/sparky_manual_full_comment.peaks
--rw-r--r--   0 garythompson   (501) staff       (20)     1718 2023-01-17 09:55:08.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/sparky/test_data/test_shifts_P3a_L273R_shifts_short.txt
--rw-r--r--   0 garythompson   (501) staff       (20)     2342 2023-03-19 00:02:41.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short.neff
--rw-r--r--   0 garythompson   (501) staff       (20)     2157 2023-03-19 00:02:41.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_chains.neff
--rw-r--r--   0 garythompson   (501) staff       (20)     2156 2023-03-19 00:02:41.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_different_residues.neff
--rw-r--r--   0 garythompson   (501) staff       (20)     2803 2023-03-19 00:02:41.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_i_minus_one.neff
--rw-r--r--   0 garythompson   (501) staff       (20)     2326 2023-03-19 00:02:41.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_overlapping_chains.neff
--rw-r--r--   0 garythompson   (501) staff       (20)    12427 2023-03-24 20:06:24.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/sparky/test_export_peaks.py
--rw-r--r--   0 garythompson   (501) staff       (20)     3706 2023-04-26 21:12:14.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/sparky/test_import_peaks.py
--rw-r--r--   0 garythompson   (501) staff       (20)     2475 2023-04-26 18:38:58.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/sparky/test_import_sequence.py
--rw-r--r--   0 garythompson   (501) staff       (20)     2661 2023-01-17 17:17:45.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/sparky/test_import_shifts.py
--rw-r--r--   0 garythompson   (501) staff       (20)     2305 2023-05-04 07:44:44.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/sparky/test_sparky_lib.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-04 07:52:40.944598 nef_pipelines-0.1.37/src/nef_pipelines/tests/test_data/
--rw-r--r--   0 garythompson   (501) staff       (20)      658 2023-01-11 15:13:08.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/test_data/3a_ab.neff
--rw-r--r--   0 garythompson   (501) staff       (20)       11 2023-04-15 14:38:14.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/test_data/empty.nef
--rw-r--r--   0 garythompson   (501) staff       (20)      837 2022-12-15 21:03:33.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/test_data/header.nef
--rwxr-xr-x   0 garythompson   (501) staff       (20)      908 2023-03-18 23:31:39.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/test_data/multi_chain.nef
--rwxr-xr-x   0 garythompson   (501) staff       (20)     2979 2023-03-18 23:31:39.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/test_data/nef_3_peaks.nef
--rwxr--r--   0 garythompson   (501) staff       (20)      979 2023-01-18 17:43:15.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/test_data/tailin_seq_short.nef
--rw-r--r--   0 garythompson   (501) staff       (20)     2958 2023-02-07 21:50:52.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/test_data/test_agv.neff
--rwxr-xr-x   0 garythompson   (501) staff       (20)    64721 2023-04-16 09:21:50.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/test_data/ubiquitin_short.nef
--rw-r--r--   0 garythompson   (501) staff       (20)     1884 2023-02-07 23:05:23.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/test_header.py
--rwxr-xr-x   0 garythompson   (501) staff       (20)     9456 2023-03-18 23:11:48.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/test_nef_lib.py
--rwxr-xr-x   0 garythompson   (501) staff       (20)     7641 2023-04-24 20:39:10.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/test_sequence_lib.py
--rw-r--r--   0 garythompson   (501) staff       (20)     2750 2022-12-14 20:48:12.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/test_test.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-04 07:52:40.952773 nef_pipelines-0.1.37/src/nef_pipelines/tests/xcamshift/
--rw-r--r--   0 garythompson   (501) staff       (20)     1860 2023-02-07 22:05:04.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/xcamshift/test_export_shifts.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-04 07:52:40.986672 nef_pipelines-0.1.37/src/nef_pipelines/tests/xplor/
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-04 07:52:41.011723 nef_pipelines-0.1.37/src/nef_pipelines/tests/xplor/test_data/
--rw-r--r--   0 garythompson   (501) staff       (20)    10948 2022-12-22 19:24:27.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/xplor/test_data/3a_ab.psf
--rw-r--r--   0 garythompson   (501) staff       (20)     2700 2023-01-31 09:42:10.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/xplor/test_data/3a_ab_rdcs.neff
--rw-r--r--   0 garythompson   (501) staff       (20)      417 2022-12-22 19:24:27.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/xplor/test_data/bad_field_count.psf
--rw-r--r--   0 garythompson   (501) staff       (20)        7 2022-12-22 19:24:28.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/xplor/test_data/bad_header.psf
--rw-r--r--   0 garythompson   (501) staff       (20)      434 2022-12-22 19:24:27.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/xplor/test_data/bad_natom.psf
--rw-r--r--   0 garythompson   (501) staff       (20)      429 2022-12-22 19:24:27.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/xplor/test_data/bad_residue_number.psf
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-12-21 15:10:23.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/xplor/test_data/empty.psf
--rw-r--r--   0 garythompson   (501) staff       (20)      216 2022-12-22 19:24:28.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/xplor/test_data/no_residues_found.psf
--rw-r--r--   0 garythompson   (501) staff       (20)      623 2023-01-04 12:41:40.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/xplor/test_data/test_2_dihedrals.tbl
--rw-r--r--   0 garythompson   (501) staff       (20)      580 2023-01-11 14:25:21.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/xplor/test_data/test_2_dihedrals_bad.tbl
--rw-r--r--   0 garythompson   (501) staff       (20)      503 2023-01-11 14:57:02.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/xplor/test_data/test_2_dihedrals_no_segids.tbl
--rw-r--r--   0 garythompson   (501) staff       (20)      197 2023-01-11 22:37:32.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/xplor/test_data/test_2_distances.tbl
--rw-r--r--   0 garythompson   (501) staff       (20)      159 2023-01-11 22:37:32.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/xplor/test_data/test_2_distances_bad.tbl
--rw-r--r--   0 garythompson   (501) staff       (20)      137 2023-01-11 22:37:32.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/xplor/test_data/test_2_distances_no_segids.tbl
--rw-r--r--   0 garythompson   (501) staff       (20)      186 2023-01-04 11:17:43.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/xplor/test_data/test_2_noes.tbl
--rw-r--r--   0 garythompson   (501) staff       (20)     8093 2023-01-15 11:02:28.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/xplor/test_dihedrals.py
--rw-r--r--   0 garythompson   (501) staff       (20)     6535 2023-01-15 10:58:38.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/xplor/test_distances.py
--rw-r--r--   0 garythompson   (501) staff       (20)     1974 2023-01-31 09:53:27.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/xplor/test_export_rdcs.py
--rw-r--r--   0 garythompson   (501) staff       (20)     1487 2023-01-04 12:32:55.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/xplor/test_import_sequence.py
--rw-r--r--   0 garythompson   (501) staff       (20)     3413 2022-12-22 19:24:29.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/xplor/test_psf_lib.py
--rw-r--r--   0 garythompson   (501) staff       (20)    11065 2023-01-11 21:19:43.000000 nef_pipelines-0.1.37/src/nef_pipelines/tests/xplor/test_xplor_lib.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-04 07:52:41.045596 nef_pipelines-0.1.37/src/nef_pipelines/tools/
--rw-r--r--   0 garythompson   (501) staff       (20)     2268 2023-04-02 20:29:58.000000 nef_pipelines-0.1.37/src/nef_pipelines/tools/about.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-04 07:52:41.069121 nef_pipelines-0.1.37/src/nef_pipelines/tools/chains/
--rw-r--r--   0 garythompson   (501) staff       (20)      527 2023-01-02 20:41:38.000000 nef_pipelines-0.1.37/src/nef_pipelines/tools/chains/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)     2593 2023-04-23 18:00:54.000000 nef_pipelines-0.1.37/src/nef_pipelines/tools/chains/clone.py
--rw-r--r--   0 garythompson   (501) staff       (20)     1417 2023-03-21 20:24:03.000000 nef_pipelines-0.1.37/src/nef_pipelines/tools/chains/list.py
--rw-r--r--   0 garythompson   (501) staff       (20)     2670 2023-03-18 23:07:53.000000 nef_pipelines-0.1.37/src/nef_pipelines/tools/chains/rename.py
--rw-r--r--   0 garythompson   (501) staff       (20)     9203 2023-01-10 10:15:33.000000 nef_pipelines-0.1.37/src/nef_pipelines/tools/chains/renumber.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-04 07:52:41.075384 nef_pipelines-0.1.37/src/nef_pipelines/tools/entry/
--rw-r--r--   0 garythompson   (501) staff       (20)      376 2022-11-29 12:15:24.000000 nef_pipelines-0.1.37/src/nef_pipelines/tools/entry/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)      692 2023-02-07 13:11:22.000000 nef_pipelines-0.1.37/src/nef_pipelines/tools/entry/rename.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-04 07:52:41.092464 nef_pipelines-0.1.37/src/nef_pipelines/tools/frames/
--rw-r--r--   0 garythompson   (501) staff       (20)      639 2023-04-15 16:14:41.000000 nef_pipelines-0.1.37/src/nef_pipelines/tools/frames/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)     2556 2023-03-19 00:07:20.000000 nef_pipelines-0.1.37/src/nef_pipelines/tools/frames/delete.py
--rw-r--r--   0 garythompson   (501) staff       (20)     4111 2023-03-21 19:38:23.000000 nef_pipelines-0.1.37/src/nef_pipelines/tools/frames/insert.py
--rw-r--r--   0 garythompson   (501) staff       (20)     6996 2023-04-15 16:55:03.000000 nef_pipelines-0.1.37/src/nef_pipelines/tools/frames/list.py
--rw-r--r--   0 garythompson   (501) staff       (20)     6711 2023-04-17 20:20:20.000000 nef_pipelines-0.1.37/src/nef_pipelines/tools/frames/rename.py
--rw-r--r--   0 garythompson   (501) staff       (20)     8952 2023-03-21 20:29:06.000000 nef_pipelines-0.1.37/src/nef_pipelines/tools/frames/tabulate.py
--rw-r--r--   0 garythompson   (501) staff       (20)      871 2023-02-07 23:05:12.000000 nef_pipelines-0.1.37/src/nef_pipelines/tools/header.py
--rw-r--r--   0 garythompson   (501) staff       (20)     5132 2022-11-27 18:48:20.000000 nef_pipelines-0.1.37/src/nef_pipelines/tools/offset_shifts.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-04 07:52:41.099549 nef_pipelines-0.1.37/src/nef_pipelines/tools/peaks/
--rw-r--r--   0 garythompson   (501) staff       (20)    10891 2023-03-23 08:18:29.000000 nef_pipelines-0.1.37/src/nef_pipelines/tools/peaks/match.py
--rw-r--r--   0 garythompson   (501) staff       (20)    10539 2022-12-22 18:47:15.000000 nef_pipelines-0.1.37/src/nef_pipelines/tools/res_assign.py_unused
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-04 07:52:41.107065 nef_pipelines-0.1.37/src/nef_pipelines/tools/shifts/
--rw-r--r--   0 garythompson   (501) staff       (20)      372 2023-03-20 08:59:26.000000 nef_pipelines-0.1.37/src/nef_pipelines/tools/shifts/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)     7095 2023-04-26 16:43:57.000000 nef_pipelines-0.1.37/src/nef_pipelines/tools/shifts/make_peaks.py
--rw-r--r--   0 garythompson   (501) staff       (20)      200 2022-11-28 23:58:46.000000 nef_pipelines-0.1.37/src/nef_pipelines/tools/sink.py
--rw-r--r--   0 garythompson   (501) staff       (20)      445 2022-11-28 21:57:18.000000 nef_pipelines-0.1.37/src/nef_pipelines/tools/stream.py
--rw-r--r--   0 garythompson   (501) staff       (20)     3753 2023-04-17 20:08:48.000000 nef_pipelines-0.1.37/src/nef_pipelines/tools/test.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-04 07:52:41.109466 nef_pipelines-0.1.37/src/nef_pipelines/transcoders/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.37/src/nef_pipelines/transcoders/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-04 07:52:41.112472 nef_pipelines-0.1.37/src/nef_pipelines/transcoders/csv/
--rw-r--r--   0 garythompson   (501) staff       (20)      409 2023-03-19 00:07:20.000000 nef_pipelines-0.1.37/src/nef_pipelines/transcoders/csv/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-04 07:52:41.114337 nef_pipelines-0.1.37/src/nef_pipelines/transcoders/csv/importers/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-01-18 16:41:09.000000 nef_pipelines-0.1.37/src/nef_pipelines/transcoders/csv/importers/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)    14955 2023-01-31 09:30:29.000000 nef_pipelines-0.1.37/src/nef_pipelines/transcoders/csv/importers/rdcs.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-04 07:52:41.120712 nef_pipelines-0.1.37/src/nef_pipelines/transcoders/fasta/
--rw-r--r--   0 garythompson   (501) staff       (20)      646 2022-11-27 19:51:40.000000 nef_pipelines-0.1.37/src/nef_pipelines/transcoders/fasta/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-04 07:52:41.124409 nef_pipelines-0.1.37/src/nef_pipelines/transcoders/fasta/exporters/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.37/src/nef_pipelines/transcoders/fasta/exporters/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)     3952 2023-03-22 17:47:24.000000 nef_pipelines-0.1.37/src/nef_pipelines/transcoders/fasta/exporters/sequence.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-04 07:52:41.126806 nef_pipelines-0.1.37/src/nef_pipelines/transcoders/fasta/importers/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.37/src/nef_pipelines/transcoders/fasta/importers/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)     5532 2023-04-24 20:34:49.000000 nef_pipelines-0.1.37/src/nef_pipelines/transcoders/fasta/importers/sequence.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-04 07:52:41.132610 nef_pipelines-0.1.37/src/nef_pipelines/transcoders/mars/
--rw-r--r--   0 garythompson   (501) staff       (20)      946 2023-02-15 11:20:25.000000 nef_pipelines-0.1.37/src/nef_pipelines/transcoders/mars/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-04 07:52:41.150885 nef_pipelines-0.1.37/src/nef_pipelines/transcoders/mars/exporters/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.37/src/nef_pipelines/transcoders/mars/exporters/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)     6571 2023-02-15 21:49:23.000000 nef_pipelines-0.1.37/src/nef_pipelines/transcoders/mars/exporters/fragments.py
--rw-r--r--   0 garythompson   (501) staff       (20)     4299 2023-02-15 22:21:34.000000 nef_pipelines-0.1.37/src/nef_pipelines/transcoders/mars/exporters/input.py
--rw-r--r--   0 garythompson   (501) staff       (20)      780 2022-11-28 23:56:55.000000 nef_pipelines-0.1.37/src/nef_pipelines/transcoders/mars/exporters/sequence.py
--rw-r--r--   0 garythompson   (501) staff       (20)     6001 2023-03-11 19:52:09.000000 nef_pipelines-0.1.37/src/nef_pipelines/transcoders/mars/exporters/shifts.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-04 07:52:41.156212 nef_pipelines-0.1.37/src/nef_pipelines/transcoders/mars/importers/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-02-05 10:22:38.000000 nef_pipelines-0.1.37/src/nef_pipelines/transcoders/mars/importers/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)    11657 2023-04-24 20:38:57.000000 nef_pipelines-0.1.37/src/nef_pipelines/transcoders/mars/importers/shifts.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-04 07:52:41.165206 nef_pipelines-0.1.37/src/nef_pipelines/transcoders/nmrpipe/
--rw-r--r--   0 garythompson   (501) staff       (20)      679 2022-11-27 19:52:05.000000 nef_pipelines-0.1.37/src/nef_pipelines/transcoders/nmrpipe/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-04 07:52:41.176869 nef_pipelines-0.1.37/src/nef_pipelines/transcoders/nmrpipe/importers/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.37/src/nef_pipelines/transcoders/nmrpipe/importers/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)     2414 2022-12-13 19:17:42.000000 nef_pipelines-0.1.37/src/nef_pipelines/transcoders/nmrpipe/importers/peaks.py
--rw-r--r--   0 garythompson   (501) staff       (20)     3498 2023-04-24 20:38:57.000000 nef_pipelines-0.1.37/src/nef_pipelines/transcoders/nmrpipe/importers/sequence.py
--rw-r--r--   0 garythompson   (501) staff       (20)     3151 2023-04-24 20:36:47.000000 nef_pipelines-0.1.37/src/nef_pipelines/transcoders/nmrpipe/importers/shifts.py
--rw-r--r--   0 garythompson   (501) staff       (20)    20224 2023-04-24 21:17:19.000000 nef_pipelines-0.1.37/src/nef_pipelines/transcoders/nmrpipe/nmrpipe_lib.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-04 07:52:41.180681 nef_pipelines-0.1.37/src/nef_pipelines/transcoders/nmrview/
--rw-r--r--   0 garythompson   (501) staff       (20)     1056 2023-01-16 22:48:48.000000 nef_pipelines-0.1.37/src/nef_pipelines/transcoders/nmrview/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-04 07:52:41.196750 nef_pipelines-0.1.37/src/nef_pipelines/transcoders/nmrview/exporters/
--rw-r--r--   0 garythompson   (501) staff       (20)    13841 2023-02-07 13:14:10.000000 nef_pipelines-0.1.37/src/nef_pipelines/transcoders/nmrview/exporters/peaks.py
--rw-r--r--   0 garythompson   (501) staff       (20)     7053 2023-01-30 07:39:27.000000 nef_pipelines-0.1.37/src/nef_pipelines/transcoders/nmrview/exporters/sequences.py
--rw-r--r--   0 garythompson   (501) staff       (20)     9136 2023-01-16 22:47:55.000000 nef_pipelines-0.1.37/src/nef_pipelines/transcoders/nmrview/exporters/shifts.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-04 07:52:41.211002 nef_pipelines-0.1.37/src/nef_pipelines/transcoders/nmrview/importers/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.37/src/nef_pipelines/transcoders/nmrview/importers/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)    17212 2022-12-22 18:41:48.000000 nef_pipelines-0.1.37/src/nef_pipelines/transcoders/nmrview/importers/peaks.py
--rw-r--r--   0 garythompson   (501) staff       (20)     2330 2023-04-24 20:38:58.000000 nef_pipelines-0.1.37/src/nef_pipelines/transcoders/nmrview/importers/sequence.py
--rw-r--r--   0 garythompson   (501) staff       (20)     5787 2023-04-24 20:38:58.000000 nef_pipelines-0.1.37/src/nef_pipelines/transcoders/nmrview/importers/shifts.py
--rw-r--r--   0 garythompson   (501) staff       (20)     8866 2023-01-16 22:43:21.000000 nef_pipelines-0.1.37/src/nef_pipelines/transcoders/nmrview/nmrview_lib.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-04 07:52:41.213551 nef_pipelines-0.1.37/src/nef_pipelines/transcoders/pales/
--rw-r--r--   0 garythompson   (501) staff       (20)      660 2022-11-27 19:52:13.000000 nef_pipelines-0.1.37/src/nef_pipelines/transcoders/pales/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-04 07:52:41.221846 nef_pipelines-0.1.37/src/nef_pipelines/transcoders/pales/exporters/
--rw-r--r--   0 garythompson   (501) staff       (20)    10789 2023-01-30 23:23:18.000000 nef_pipelines-0.1.37/src/nef_pipelines/transcoders/pales/exporters/rdcs.py
--rw-r--r--   0 garythompson   (501) staff       (20)     4817 2023-03-06 22:17:20.000000 nef_pipelines-0.1.37/src/nef_pipelines/transcoders/pales/exporters/template.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-04 07:52:41.229524 nef_pipelines-0.1.37/src/nef_pipelines/transcoders/pdbx/
--rw-r--r--   0 garythompson   (501) staff       (20)      454 2022-12-17 16:50:37.000000 nef_pipelines-0.1.37/src/nef_pipelines/transcoders/pdbx/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-04 07:52:41.231304 nef_pipelines-0.1.37/src/nef_pipelines/transcoders/pdbx/importers/
--rw-r--r--   0 garythompson   (501) staff       (20)     4655 2022-12-17 16:51:05.000000 nef_pipelines-0.1.37/src/nef_pipelines/transcoders/pdbx/importers/sequence.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-04 07:52:41.236692 nef_pipelines-0.1.37/src/nef_pipelines/transcoders/rpf/
--rw-r--r--   0 garythompson   (501) staff       (20)      608 2023-03-23 08:19:19.000000 nef_pipelines-0.1.37/src/nef_pipelines/transcoders/rpf/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-04 07:52:41.240980 nef_pipelines-0.1.37/src/nef_pipelines/transcoders/rpf/exporters/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-03-22 21:34:49.000000 nef_pipelines-0.1.37/src/nef_pipelines/transcoders/rpf/exporters/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)    11873 2023-03-22 22:37:50.000000 nef_pipelines-0.1.37/src/nef_pipelines/transcoders/rpf/exporters/shifts.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-04 07:52:41.244001 nef_pipelines-0.1.37/src/nef_pipelines/transcoders/shifty/
--rw-r--r--   0 garythompson   (501) staff       (20)      523 2023-02-08 16:38:07.000000 nef_pipelines-0.1.37/src/nef_pipelines/transcoders/shifty/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-04 07:52:41.245923 nef_pipelines-0.1.37/src/nef_pipelines/transcoders/shifty/exporters/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-02-05 22:19:02.000000 nef_pipelines-0.1.37/src/nef_pipelines/transcoders/shifty/exporters/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)     6339 2023-04-24 20:32:00.000000 nef_pipelines-0.1.37/src/nef_pipelines/transcoders/shifty/exporters/shifts.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-04 07:52:41.250314 nef_pipelines-0.1.37/src/nef_pipelines/transcoders/sparky/
--rw-r--r--   0 garythompson   (501) staff       (20)      804 2023-04-26 18:38:57.000000 nef_pipelines-0.1.37/src/nef_pipelines/transcoders/sparky/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-04 07:52:41.266497 nef_pipelines-0.1.37/src/nef_pipelines/transcoders/sparky/exporters/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-03-18 23:36:58.000000 nef_pipelines-0.1.37/src/nef_pipelines/transcoders/sparky/exporters/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)    15804 2023-05-04 07:46:41.000000 nef_pipelines-0.1.37/src/nef_pipelines/transcoders/sparky/exporters/peaks.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-04 07:52:41.275552 nef_pipelines-0.1.37/src/nef_pipelines/transcoders/sparky/importers/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-01-16 13:30:23.000000 nef_pipelines-0.1.37/src/nef_pipelines/transcoders/sparky/importers/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)    15984 2023-05-04 07:48:00.000000 nef_pipelines-0.1.37/src/nef_pipelines/transcoders/sparky/importers/peaks.py
--rw-r--r--   0 garythompson   (501) staff       (20)     6463 2023-04-26 18:39:25.000000 nef_pipelines-0.1.37/src/nef_pipelines/transcoders/sparky/importers/sequence.py
--rw-r--r--   0 garythompson   (501) staff       (20)     8953 2023-03-19 00:07:20.000000 nef_pipelines-0.1.37/src/nef_pipelines/transcoders/sparky/importers/shifts.py
--rw-r--r--   0 garythompson   (501) staff       (20)     8496 2023-05-04 07:43:57.000000 nef_pipelines-0.1.37/src/nef_pipelines/transcoders/sparky/sparly_lib.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-04 07:52:41.281638 nef_pipelines-0.1.37/src/nef_pipelines/transcoders/xcamshift/
--rw-r--r--   0 garythompson   (501) staff       (20)      554 2023-02-07 22:05:04.000000 nef_pipelines-0.1.37/src/nef_pipelines/transcoders/xcamshift/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-04 07:52:41.284110 nef_pipelines-0.1.37/src/nef_pipelines/transcoders/xcamshift/exporters/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-02-05 22:19:02.000000 nef_pipelines-0.1.37/src/nef_pipelines/transcoders/xcamshift/exporters/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)     3787 2023-02-07 22:05:13.000000 nef_pipelines-0.1.37/src/nef_pipelines/transcoders/xcamshift/exporters/shifts.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-04 07:52:41.294655 nef_pipelines-0.1.37/src/nef_pipelines/transcoders/xplor/
--rw-r--r--   0 garythompson   (501) staff       (20)      933 2023-02-05 22:57:14.000000 nef_pipelines-0.1.37/src/nef_pipelines/transcoders/xplor/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-04 07:52:41.304345 nef_pipelines-0.1.37/src/nef_pipelines/transcoders/xplor/exporters/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-01-20 20:08:15.000000 nef_pipelines-0.1.37/src/nef_pipelines/transcoders/xplor/exporters/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)     7167 2023-01-31 09:54:44.000000 nef_pipelines-0.1.37/src/nef_pipelines/transcoders/xplor/exporters/rdcs.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-04 07:52:41.314667 nef_pipelines-0.1.37/src/nef_pipelines/transcoders/xplor/importers/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-12-17 17:33:41.000000 nef_pipelines-0.1.37/src/nef_pipelines/transcoders/xplor/importers/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)     2834 2023-03-24 21:54:07.000000 nef_pipelines-0.1.37/src/nef_pipelines/transcoders/xplor/importers/dihedrals.py
--rw-r--r--   0 garythompson   (501) staff       (20)     2888 2023-01-11 22:37:57.000000 nef_pipelines-0.1.37/src/nef_pipelines/transcoders/xplor/importers/distances.py
--rw-r--r--   0 garythompson   (501) staff       (20)     3298 2023-01-04 12:32:55.000000 nef_pipelines-0.1.37/src/nef_pipelines/transcoders/xplor/importers/sequence.py
--rw-r--r--   0 garythompson   (501) staff       (20)     3663 2022-12-22 19:24:58.000000 nef_pipelines-0.1.37/src/nef_pipelines/transcoders/xplor/psf_lib.py
--rw-r--r--   0 garythompson   (501) staff       (20)    38877 2023-01-11 22:37:34.000000 nef_pipelines-0.1.37/src/nef_pipelines/transcoders/xplor/xplor_lib.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-04 07:52:40.507989 nef_pipelines-0.1.37/src/nef_pipelines.egg-info/
--rw-r--r--   0 garythompson   (501) staff       (20)     8765 2023-05-04 07:52:40.000000 nef_pipelines-0.1.37/src/nef_pipelines.egg-info/PKG-INFO
--rw-r--r--   0 garythompson   (501) staff       (20)    13422 2023-05-04 07:52:40.000000 nef_pipelines-0.1.37/src/nef_pipelines.egg-info/SOURCES.txt
--rw-r--r--   0 garythompson   (501) staff       (20)        1 2023-05-04 07:52:40.000000 nef_pipelines-0.1.37/src/nef_pipelines.egg-info/dependency_links.txt
--rw-r--r--   0 garythompson   (501) staff       (20)       48 2023-05-04 07:52:40.000000 nef_pipelines-0.1.37/src/nef_pipelines.egg-info/entry_points.txt
--rw-r--r--   0 garythompson   (501) staff       (20)        1 2022-11-27 19:48:54.000000 nef_pipelines-0.1.37/src/nef_pipelines.egg-info/not-zip-safe
--rw-r--r--   0 garythompson   (501) staff       (20)      363 2023-05-04 07:52:40.000000 nef_pipelines-0.1.37/src/nef_pipelines.egg-info/requires.txt
--rw-r--r--   0 garythompson   (501) staff       (20)       14 2023-05-04 07:52:40.000000 nef_pipelines-0.1.37/src/nef_pipelines.egg-info/top_level.txt
--rw-r--r--   0 garythompson   (501) staff       (20)     3032 2023-02-01 22:03:42.000000 nef_pipelines-0.1.37/tox.ini
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:46.171207 nef_pipelines-0.1.38/
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:44.935970 nef_pipelines-0.1.38/.github/
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:45.025175 nef_pipelines-0.1.38/.github/workflows/
+-rw-r--r--   0 garythompson   (501) staff       (20)     4094 2023-02-01 22:03:42.000000 nef_pipelines-0.1.38/.github/workflows/ci.yml
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:45.043286 nef_pipelines-0.1.38/.idea/
+-rw-r--r--   0 garythompson   (501) staff       (20)      176 2022-11-25 17:14:12.000000 nef_pipelines-0.1.38/.idea/.gitignore
+-rw-r--r--   0 garythompson   (501) staff       (20)       14 2022-11-26 23:48:55.000000 nef_pipelines-0.1.38/.idea/.name
+-rw-r--r--   0 garythompson   (501) staff       (20)      299 2023-01-11 23:02:58.000000 nef_pipelines-0.1.38/.idea/NFC.iml
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:45.050392 nef_pipelines-0.1.38/.idea/inspectionProfiles/
+-rw-r--r--   0 garythompson   (501) staff       (20)     1184 2023-01-11 23:02:58.000000 nef_pipelines-0.1.38/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0 garythompson   (501) staff       (20)      175 2023-01-11 23:02:58.000000 nef_pipelines-0.1.38/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 garythompson   (501) staff       (20)      287 2023-01-11 23:02:58.000000 nef_pipelines-0.1.38/.idea/modules.xml
+-rw-r--r--   0 garythompson   (501) staff       (20)      325 2023-04-26 19:24:39.000000 nef_pipelines-0.1.38/.idea/vcs.xml
+-rw-r--r--   0 garythompson   (501) staff       (20)     1331 2022-11-26 14:34:37.000000 nef_pipelines-0.1.38/.pre-commit-config.yaml
+-rw-r--r--   0 garythompson   (501) staff       (20)      490 2022-11-26 14:33:30.000000 nef_pipelines-0.1.38/.readthedocs.yml
+-rw-r--r--   0 garythompson   (501) staff       (20)      372 2023-02-07 22:36:51.000000 nef_pipelines-0.1.38/AUTHORS.md
+-rw-r--r--   0 garythompson   (501) staff       (20)     3449 2023-05-06 21:00:36.000000 nef_pipelines-0.1.38/CHANGELOG.md
+-rw-r--r--   0 garythompson   (501) staff       (20)    12299 2022-11-27 14:11:11.000000 nef_pipelines-0.1.38/CONTRIBUTING.md
+-rw-r--r--   0 garythompson   (501) staff       (20)    24410 2022-11-27 14:11:12.000000 nef_pipelines-0.1.38/LICENSE.txt
+-rw-r--r--   0 garythompson   (501) staff       (20)     8765 2023-05-06 21:01:46.171784 nef_pipelines-0.1.38/PKG-INFO
+-rw-r--r--   0 garythompson   (501) staff       (20)     8212 2023-02-07 22:28:55.000000 nef_pipelines-0.1.38/README.md
+-rw-r--r--   0 garythompson   (501) staff       (20)      826 2023-02-05 15:31:16.000000 nef_pipelines-0.1.38/TODO.md
+-rw-r--r--   0 garythompson   (501) staff       (20)      346 2023-01-31 22:56:36.000000 nef_pipelines-0.1.38/pyproject.toml
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:45.060018 nef_pipelines-0.1.38/references/
+-rw-r--r--   0 garythompson   (501) staff       (20)    22346 2023-04-16 16:41:23.000000 nef_pipelines-0.1.38/references/Nmr Experiment Nomenclature v2.docx
+-rw-r--r--   0 garythompson   (501) staff       (20)   282399 2023-04-16 14:33:43.000000 nef_pipelines-0.1.38/references/fogh.vrankenj.bio.nmr.2006.36.147.pdf
+-rw-r--r--   0 garythompson   (501) staff       (20)     1229 2023-04-17 21:03:23.000000 nef_pipelines-0.1.38/release_to_pypi.sh
+-rw-r--r--   0 garythompson   (501) staff       (20)      354 2023-04-17 20:13:08.000000 nef_pipelines-0.1.38/requirements.txt
+-rw-r--r--   0 garythompson   (501) staff       (20)     1630 2023-05-06 21:01:46.176699 nef_pipelines-0.1.38/setup.cfg
+-rw-r--r--   0 garythompson   (501) staff       (20)      710 2022-11-26 14:33:30.000000 nef_pipelines-0.1.38/setup.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:44.937801 nef_pipelines-0.1.38/src/
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:45.080949 nef_pipelines-0.1.38/src/nef_pipelines/
+-rw-r--r--   0 garythompson   (501) staff       (20)        6 2023-03-23 08:31:34.000000 nef_pipelines-0.1.38/src/nef_pipelines/VERSION
+-rw-r--r--   0 garythompson   (501) staff       (20)      577 2022-11-27 18:49:20.000000 nef_pipelines-0.1.38/src/nef_pipelines/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)       62 2022-11-27 18:48:20.000000 nef_pipelines-0.1.38/src/nef_pipelines/__main__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:45.125773 nef_pipelines-0.1.38/src/nef_pipelines/data/
+-rw-r--r--   0 garythompson   (501) staff       (20)  1486198 2023-05-06 14:31:14.000000 nef_pipelines-0.1.38/src/nef_pipelines/data/mmcif_nef_v1_1.dic
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:45.210481 nef_pipelines-0.1.38/src/nef_pipelines/lib/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.38/src/nef_pipelines/lib/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)      124 2023-02-07 22:55:44.000000 nef_pipelines-0.1.38/src/nef_pipelines/lib/constants.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     1297 2022-11-27 19:40:25.000000 nef_pipelines-0.1.38/src/nef_pipelines/lib/header_lib.py
+-rw-r--r--   0 garythompson   (501) staff       (20)      945 2023-03-19 15:38:08.000000 nef_pipelines-0.1.38/src/nef_pipelines/lib/isotope_lib.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     2812 2023-04-26 21:04:53.000000 nef_pipelines-0.1.38/src/nef_pipelines/lib/nef_frames_lib.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    16143 2023-04-15 16:57:10.000000 nef_pipelines-0.1.38/src/nef_pipelines/lib/nef_lib.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    15051 2023-05-04 07:18:02.000000 nef_pipelines-0.1.38/src/nef_pipelines/lib/peak_lib.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    21187 2023-04-30 15:31:02.000000 nef_pipelines-0.1.38/src/nef_pipelines/lib/sequence_lib.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     6348 2023-02-07 21:12:56.000000 nef_pipelines-0.1.38/src/nef_pipelines/lib/shift_lib.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     6548 2023-04-17 20:48:44.000000 nef_pipelines-0.1.38/src/nef_pipelines/lib/spectra_lib.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     4083 2023-05-04 07:17:17.000000 nef_pipelines-0.1.38/src/nef_pipelines/lib/structures.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    10234 2023-04-26 19:21:33.000000 nef_pipelines-0.1.38/src/nef_pipelines/lib/test_lib.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:45.214172 nef_pipelines-0.1.38/src/nef_pipelines/lib/translation/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.38/src/nef_pipelines/lib/translation/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     1049 2023-05-06 20:57:18.000000 nef_pipelines-0.1.38/src/nef_pipelines/lib/translation_lib.py
+-rw-r--r--   0 garythompson   (501) staff       (20)      292 2022-11-27 18:48:20.000000 nef_pipelines-0.1.38/src/nef_pipelines/lib/typer_utils.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    22250 2023-04-17 20:19:05.000000 nef_pipelines-0.1.38/src/nef_pipelines/lib/util.py
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     5288 2023-05-06 20:58:23.000000 nef_pipelines-0.1.38/src/nef_pipelines/main.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:45.214750 nef_pipelines-0.1.38/src/nef_pipelines/nef_app/
+-rw-r--r--   0 garythompson   (501) staff       (20)       49 2022-11-27 18:48:20.000000 nef_pipelines-0.1.38/src/nef_pipelines/nef_app/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:45.234775 nef_pipelines-0.1.38/src/nef_pipelines/tests/
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:45.246964 nef_pipelines-0.1.38/src/nef_pipelines/tests/chains/
+-rwxr--r--   0 garythompson   (501) staff       (20)        0 2022-11-25 17:14:10.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/chains/__init__.py
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     5259 2023-03-18 23:31:39.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/chains/test_clone.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:45.252581 nef_pipelines-0.1.38/src/nef_pipelines/tests/chains/test_data/
+-rwxr--r--   0 garythompson   (501) staff       (20)      581 2022-11-25 17:14:10.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/chains/test_data/3aa.nef
+-rwxr-xr-x   0 garythompson   (501) staff       (20)      837 2023-03-18 23:31:39.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/chains/test_data/3aa_x3.nef
+-rwxr--r--   0 garythompson   (501) staff       (20)     2172 2022-12-16 20:37:04.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/chains/test_data/multi_chain_shifts.nef
+-rwxr--r--   0 garythompson   (501) staff       (20)      491 2022-12-16 20:38:38.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/chains/test_list.py
+-rwxr-xr-x   0 garythompson   (501) staff       (20)    10032 2023-03-18 23:31:39.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/chains/test_rename.py
+-rwxr--r--   0 garythompson   (501) staff       (20)     9304 2023-01-30 23:11:50.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/chains/test_renumber.py
+-rw-r--r--   0 garythompson   (501) staff       (20)      709 2023-01-12 09:57:27.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/conftest.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:45.254075 nef_pipelines-0.1.38/src/nef_pipelines/tests/csv/
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:45.258135 nef_pipelines-0.1.38/src/nef_pipelines/tests/csv/test_data/
+-rw-r--r--   0 garythompson   (501) staff       (20)       45 2023-01-31 08:50:56.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/csv/test_data/short.csv
+-rw-r--r--   0 garythompson   (501) staff       (20)      218 2023-01-31 08:49:14.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/csv/test_data/short_complete.csv
+-rw-r--r--   0 garythompson   (501) staff       (20)     5079 2023-01-31 22:17:03.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/csv/test_import_rdcs.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:45.260577 nef_pipelines-0.1.38/src/nef_pipelines/tests/echidna/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-05-04 20:35:04.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/echidna/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:45.263880 nef_pipelines-0.1.38/src/nef_pipelines/tests/echidna/test_data/
+-rw-r--r--   0 garythompson   (501) staff       (20)      695 2023-05-06 14:02:40.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/echidna/test_data/echidna_peaks.txt
+-rw-r--r--   0 garythompson   (501) staff       (20)     1775 2023-05-06 14:16:20.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/echidna/test_data/echidna_sequence.nef
+-rw-r--r--   0 garythompson   (501) staff       (20)     3610 2023-05-06 20:59:13.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/echidna/test_import_peaks.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:45.265031 nef_pipelines-0.1.38/src/nef_pipelines/tests/fasta/
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:45.270850 nef_pipelines-0.1.38/src/nef_pipelines/tests/fasta/test_data/
+-rwxr--r--   0 garythompson   (501) staff       (20)       11 2022-12-06 19:49:15.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/fasta/test_data/3aa.fasta
+-rwxr-xr-x   0 garythompson   (501) staff       (20)       24 2023-03-18 23:31:39.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/fasta/test_data/3aa_x2.fasta
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     3178 2023-03-18 23:31:39.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/fasta/test_sequence.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:45.306073 nef_pipelines-0.1.38/src/nef_pipelines/tests/frames/
+-rwxr--r--   0 garythompson   (501) staff       (20)        0 2022-12-06 20:53:09.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/frames/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:45.310770 nef_pipelines-0.1.38/src/nef_pipelines/tests/frames/test_data/
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     1470 2023-03-18 23:31:39.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/frames/test_data/frames.nef
+-rwxr--r--   0 garythompson   (501) staff       (20)     1626 2022-12-16 21:06:02.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/frames/test_data/pales_test_1.nef
+-rwxr--r--   0 garythompson   (501) staff       (20)     2690 2022-12-16 21:06:48.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/frames/test_delete.py
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     1123 2023-04-15 16:57:25.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/frames/test_list.py
+-rwxr--r--   0 garythompson   (501) staff       (20)    10090 2023-04-15 16:15:29.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/frames/test_rename.py
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     1312 2023-03-18 23:31:39.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/frames/test_tabulate.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:45.314581 nef_pipelines-0.1.38/src/nef_pipelines/tests/mars/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-02-05 13:08:51.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/mars/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:45.337521 nef_pipelines-0.1.38/src/nef_pipelines/tests/mars/test_data/
+-rw-r--r--   0 garythompson   (501) staff       (20)     9631 2023-02-01 22:03:42.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/mars/test_data/sec5_short.neff
+-rw-r--r--   0 garythompson   (501) staff       (20)      311 2023-02-05 15:30:43.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/mars/test_data/sec5_short.txt
+-rw-r--r--   0 garythompson   (501) staff       (20)      838 2023-02-01 22:29:59.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/mars/test_export_shifts.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     2537 2023-02-05 15:30:44.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/mars/test_import_shifts.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:45.352620 nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrpipe/
+-rwxr--r--   0 garythompson   (501) staff       (20)        0 2022-12-10 21:27:09.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrpipe/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:45.406764 nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrpipe/test_data/
+-rwxr-xr-x   0 garythompson   (501) staff       (20)       12 2023-03-18 23:31:39.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrpipe/test_data/3aa.seq
+-rwxr--r--   0 garythompson   (501) staff       (20)       18 2022-12-16 20:31:09.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrpipe/test_data/3aa.tab
+-rwxr-xr-x   0 garythompson   (501) staff       (20)       15 2023-03-18 23:31:39.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrpipe/test_data/3aa10.seq
+-rwxr--r--   0 garythompson   (501) staff       (20)       16 2022-12-16 20:31:09.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrpipe/test_data/4peaks.seq
+-rw-------   0 garythompson   (501) staff       (20)      455 2023-01-10 13:25:00.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrpipe/test_data/P3a_l273R_nmrpipe_shifts_short.tab
+-rwxr--r--   0 garythompson   (501) staff       (20)    10961 2022-12-16 20:31:08.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrpipe/test_data/gb3.tab
+-rwxr--r--   0 garythompson   (501) staff       (20)    11038 2022-12-16 20:31:08.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned.tab
+-rwxr-xr-x   0 garythompson   (501) staff       (20)      943 2023-03-18 23:31:39.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned_trunc.tab
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     1878 2023-03-18 23:31:39.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned_trunc_expected.tab
+-rwxr--r--   0 garythompson   (501) staff       (20)    26327 2022-12-16 20:31:09.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrpipe/test_data/ns3_S135A_BMRB1.txt
+-rwxr--r--   0 garythompson   (501) staff       (20)      247 2022-12-16 20:31:09.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrpipe/test_data/ns3_S135A_BMRB1_short.txt
+-rwxr-xr-x   0 garythompson   (501) staff       (20)      800 2023-03-18 23:31:39.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrpipe/test_data/test_header_entry.txt
+-rwxr-xr-x   0 garythompson   (501) staff       (20)    14392 2023-04-24 21:03:24.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrpipe/test_gdb.py
+-rwxr--r--   0 garythompson   (501) staff       (20)      840 2022-12-16 20:35:58.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrpipe/test_peaks.py
+-rwxr--r--   0 garythompson   (501) staff       (20)      486 2022-12-16 20:35:58.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrpipe/test_pipe_lib.py
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     4158 2023-03-18 23:31:39.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrpipe/test_sequence.py
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     4454 2023-01-18 07:36:14.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrpipe/test_shifts.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:45.492861 nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrview/
+-rwxr--r--   0 garythompson   (501) staff       (20)        0 2022-12-11 15:04:32.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrview/__init__.py
+-rwxr--r--   0 garythompson   (501) staff       (20)    10752 2022-12-17 11:29:00.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrview/tcl_diag.html
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:45.541714 nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrview/test_data/
+-rwxr--r--   0 garythompson   (501) staff       (20)       12 2022-12-11 15:04:32.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrview/test_data/3aa.seq
+-rwxr--r--   0 garythompson   (501) staff       (20)       15 2022-12-11 15:04:32.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrview/test_data/3aa10.seq
+-rwxr--r--   0 garythompson   (501) staff       (20)       16 2022-12-17 11:29:00.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrview/test_data/4peaks.seq
+-rwxr-xr-x   0 garythompson   (501) staff       (20)      980 2023-03-18 23:31:39.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrview/test_data/4peaks.xpk
+-rwxr--r--   0 garythompson   (501) staff       (20)      880 2022-12-11 15:04:32.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrview/test_data/expected_nmr_view.xpk
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     2178 2023-03-18 23:31:39.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrview/test_data/expected_sequence_and_peaks_nmrview.txt
+-rwxr--r--   0 garythompson   (501) staff       (20)      319 2022-12-11 15:04:32.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrview/test_data/joe_clic.xpk
+-rwxr--r--   0 garythompson   (501) staff       (20)     2172 2022-12-11 15:04:32.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrview/test_data/nmrview_expected_4aa.txt
+-rwxr--r--   0 garythompson   (501) staff       (20)    29631 2022-12-11 15:04:32.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrview/test_data/ppm.out
+-rwxr--r--   0 garythompson   (501) staff       (20)      540 2022-12-11 15:04:32.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrview/test_data/ppm_out.seq
+-rwxr--r--   0 garythompson   (501) staff       (20)       12 2022-12-11 15:04:32.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrview/test_data/ppm_out_short.seq
+-rwxr--r--   0 garythompson   (501) staff       (20)      126 2022-12-11 15:04:32.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrview/test_data/ppm_short.out
+-rwxr--r--   0 garythompson   (501) staff       (20)      522 2022-12-17 11:29:00.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrview/test_data/ppm_short_seq.nef
+-rwxr--r--   0 garythompson   (501) staff       (20)      800 2022-12-11 15:05:20.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrview/test_data/test_header_entry.txt
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     2646 2023-03-18 23:31:39.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrview/test_export_peaks.py
+-rwxr--r--   0 garythompson   (501) staff       (20)     3343 2023-01-14 17:44:39.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrview/test_export_sequences.py
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     3872 2023-02-15 22:22:17.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrview/test_import_peaks.py
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     3915 2023-02-07 23:04:20.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrview/test_import_sequence.py
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     4734 2023-01-18 07:36:14.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrview/test_import_shifts.py
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     2166 2023-03-18 23:31:39.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrview/test_tcl.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:45.546386 nef_pipelines-0.1.38/src/nef_pipelines/tests/pales/
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:45.551612 nef_pipelines-0.1.38/src/nef_pipelines/tests/pales/test_data/
+-rwxr--r--   0 garythompson   (501) staff       (20)     1626 2022-12-17 16:34:00.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/pales/test_data/pales_test_1.nef
+-rwxr--r--   0 garythompson   (501) staff       (20)     1627 2022-12-17 16:34:00.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/pales/test_data/pales_test_2.nef
+-rwxr--r--   0 garythompson   (501) staff       (20)     1647 2023-01-27 21:30:12.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/pales/test_data/pales_test_segids.nef
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     2773 2023-01-30 23:21:17.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/pales/test_rdcs.py
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     2043 2023-03-18 23:31:39.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/pales/test_template.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:45.553516 nef_pipelines-0.1.38/src/nef_pipelines/tests/pdbx/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-01-31 19:44:59.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/pdbx/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:45.585378 nef_pipelines-0.1.38/src/nef_pipelines/tests/pdbx/test_data/
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     4795 2023-03-18 23:31:39.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/pdbx/test_data/3a_ab.pdb
+-rwxr--r--   0 garythompson   (501) staff       (20)     4795 2022-12-17 16:52:18.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/pdbx/test_data/3a_cccc_dddd.pdb
+-rwxr--r--   0 garythompson   (501) staff       (20)     4195 2022-12-17 16:52:18.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/pdbx/test_data/3a_no_chain_no_segid.pdb
+-rwxr--r--   0 garythompson   (501) staff       (20)     2395 2022-12-17 16:52:18.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/pdbx/test_data/3aa.pdb
+-rwxr--r--   0 garythompson   (501) staff       (20)     2254 2022-12-17 16:52:18.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/pdbx/test_data/3aa11_13.pdb
+-rwxr--r--   0 garythompson   (501) staff       (20)      800 2022-12-10 20:00:10.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/pdbx/test_data/test_header_entry.txt
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     4248 2023-01-15 11:02:28.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/pdbx/test_sequence.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:45.586647 nef_pipelines-0.1.38/src/nef_pipelines/tests/shifts/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-04-16 09:07:56.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/shifts/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     8438 2023-04-17 20:44:38.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/shifts/test_make_peaks.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:45.589043 nef_pipelines-0.1.38/src/nef_pipelines/tests/shifty/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-02-09 08:07:44.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/shifty/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)      773 2023-02-09 08:08:24.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/shifty/test_export_shifts.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:45.624615 nef_pipelines-0.1.38/src/nef_pipelines/tests/sparky/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-04-26 18:29:03.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/sparky/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:45.679737 nef_pipelines-0.1.38/src/nef_pipelines/tests/sparky/test_data/
+-rw-r--r--   0 garythompson   (501) staff       (20)     1393 2023-01-31 21:17:52.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/sparky/test_data/P3a_L273R_sequence_short.neff
+-rw-r--r--   0 garythompson   (501) staff       (20)     2342 2023-03-19 00:02:41.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/sparky/test_data/peaks_short_with_assignments.neff
+-rw-r--r--   0 garythompson   (501) staff       (20)       40 2023-04-26 18:38:57.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/sparky/test_data/sparky_basic_sequence_dna.txt
+-rw-r--r--   0 garythompson   (501) staff       (20)        9 2023-04-26 18:38:57.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/sparky/test_data/sparky_basic_sequence_protein.txt
+-rw-r--r--   0 garythompson   (501) staff       (20)      241 2023-04-26 21:06:34.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/sparky/test_data/sparky_manual_basic.peaks
+-rw-r--r--   0 garythompson   (501) staff       (20)     1187 2023-04-26 18:24:37.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/sparky/test_data/sparky_manual_basic_sequence.nef
+-rw-r--r--   0 garythompson   (501) staff       (20)      359 2023-04-26 19:32:49.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/sparky/test_data/sparky_manual_full.peaks
+-rw-r--r--   0 garythompson   (501) staff       (20)      422 2023-04-26 20:35:49.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/sparky/test_data/sparky_manual_full_comment.peaks
+-rw-r--r--   0 garythompson   (501) staff       (20)      354 2023-05-04 18:45:19.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/sparky/test_data/sparky_manual_full_no_sequence.peaks
+-rw-r--r--   0 garythompson   (501) staff       (20)     1718 2023-01-17 09:55:08.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/sparky/test_data/test_shifts_P3a_L273R_shifts_short.txt
+-rw-r--r--   0 garythompson   (501) staff       (20)     2342 2023-03-19 00:02:41.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short.neff
+-rw-r--r--   0 garythompson   (501) staff       (20)     2157 2023-03-19 00:02:41.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_chains.neff
+-rw-r--r--   0 garythompson   (501) staff       (20)     2156 2023-03-19 00:02:41.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_different_residues.neff
+-rw-r--r--   0 garythompson   (501) staff       (20)     2803 2023-03-19 00:02:41.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_i_minus_one.neff
+-rw-r--r--   0 garythompson   (501) staff       (20)     2326 2023-03-19 00:02:41.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_overlapping_chains.neff
+-rw-r--r--   0 garythompson   (501) staff       (20)    12427 2023-03-24 20:06:24.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/sparky/test_export_peaks.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     4153 2023-05-04 20:25:28.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/sparky/test_import_peaks.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     2475 2023-04-26 18:38:58.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/sparky/test_import_sequence.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     2661 2023-01-17 17:17:45.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/sparky/test_import_shifts.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     2305 2023-05-06 20:53:32.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/sparky/test_sparky_lib.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:45.717273 nef_pipelines-0.1.38/src/nef_pipelines/tests/test_data/
+-rw-r--r--   0 garythompson   (501) staff       (20)      658 2023-01-11 15:13:08.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/test_data/3a_ab.neff
+-rw-r--r--   0 garythompson   (501) staff       (20)       11 2023-04-15 14:38:14.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/test_data/empty.nef
+-rw-r--r--   0 garythompson   (501) staff       (20)      837 2022-12-15 21:03:33.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/test_data/header.nef
+-rwxr-xr-x   0 garythompson   (501) staff       (20)      908 2023-03-18 23:31:39.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/test_data/multi_chain.nef
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     2979 2023-03-18 23:31:39.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/test_data/nef_3_peaks.nef
+-rwxr--r--   0 garythompson   (501) staff       (20)      979 2023-01-18 17:43:15.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/test_data/tailin_seq_short.nef
+-rw-r--r--   0 garythompson   (501) staff       (20)     2958 2023-02-07 21:50:52.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/test_data/test_agv.neff
+-rwxr-xr-x   0 garythompson   (501) staff       (20)    64721 2023-04-16 09:21:50.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/test_data/ubiquitin_short.nef
+-rw-r--r--   0 garythompson   (501) staff       (20)     1884 2023-02-07 23:05:23.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/test_header.py
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     9456 2023-03-18 23:11:48.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/test_nef_lib.py
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     7641 2023-04-24 20:39:10.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/test_sequence_lib.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     2750 2022-12-14 20:48:12.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/test_test.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:45.719578 nef_pipelines-0.1.38/src/nef_pipelines/tests/xcamshift/
+-rw-r--r--   0 garythompson   (501) staff       (20)     1860 2023-02-07 22:05:04.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/xcamshift/test_export_shifts.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:45.733654 nef_pipelines-0.1.38/src/nef_pipelines/tests/xplor/
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:45.770664 nef_pipelines-0.1.38/src/nef_pipelines/tests/xplor/test_data/
+-rw-r--r--   0 garythompson   (501) staff       (20)    10948 2022-12-22 19:24:27.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/xplor/test_data/3a_ab.psf
+-rw-r--r--   0 garythompson   (501) staff       (20)     2700 2023-01-31 09:42:10.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/xplor/test_data/3a_ab_rdcs.neff
+-rw-r--r--   0 garythompson   (501) staff       (20)      417 2022-12-22 19:24:27.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/xplor/test_data/bad_field_count.psf
+-rw-r--r--   0 garythompson   (501) staff       (20)        7 2022-12-22 19:24:28.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/xplor/test_data/bad_header.psf
+-rw-r--r--   0 garythompson   (501) staff       (20)      434 2022-12-22 19:24:27.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/xplor/test_data/bad_natom.psf
+-rw-r--r--   0 garythompson   (501) staff       (20)      429 2022-12-22 19:24:27.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/xplor/test_data/bad_residue_number.psf
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-12-21 15:10:23.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/xplor/test_data/empty.psf
+-rw-r--r--   0 garythompson   (501) staff       (20)      216 2022-12-22 19:24:28.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/xplor/test_data/no_residues_found.psf
+-rw-r--r--   0 garythompson   (501) staff       (20)      623 2023-01-04 12:41:40.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/xplor/test_data/test_2_dihedrals.tbl
+-rw-r--r--   0 garythompson   (501) staff       (20)      580 2023-01-11 14:25:21.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/xplor/test_data/test_2_dihedrals_bad.tbl
+-rw-r--r--   0 garythompson   (501) staff       (20)      503 2023-01-11 14:57:02.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/xplor/test_data/test_2_dihedrals_no_segids.tbl
+-rw-r--r--   0 garythompson   (501) staff       (20)      197 2023-01-11 22:37:32.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/xplor/test_data/test_2_distances.tbl
+-rw-r--r--   0 garythompson   (501) staff       (20)      159 2023-01-11 22:37:32.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/xplor/test_data/test_2_distances_bad.tbl
+-rw-r--r--   0 garythompson   (501) staff       (20)      137 2023-01-11 22:37:32.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/xplor/test_data/test_2_distances_no_segids.tbl
+-rw-r--r--   0 garythompson   (501) staff       (20)      186 2023-01-04 11:17:43.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/xplor/test_data/test_2_noes.tbl
+-rw-r--r--   0 garythompson   (501) staff       (20)     8093 2023-01-15 11:02:28.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/xplor/test_dihedrals.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     6535 2023-01-15 10:58:38.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/xplor/test_distances.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     1974 2023-01-31 09:53:27.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/xplor/test_export_rdcs.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     1487 2023-01-04 12:32:55.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/xplor/test_import_sequence.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     3413 2022-12-22 19:24:29.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/xplor/test_psf_lib.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    11065 2023-01-11 21:19:43.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/xplor/test_xplor_lib.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:45.798408 nef_pipelines-0.1.38/src/nef_pipelines/tools/
+-rw-r--r--   0 garythompson   (501) staff       (20)     2268 2023-04-02 20:29:58.000000 nef_pipelines-0.1.38/src/nef_pipelines/tools/about.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:45.826900 nef_pipelines-0.1.38/src/nef_pipelines/tools/chains/
+-rw-r--r--   0 garythompson   (501) staff       (20)      527 2023-01-02 20:41:38.000000 nef_pipelines-0.1.38/src/nef_pipelines/tools/chains/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     2593 2023-04-23 18:00:54.000000 nef_pipelines-0.1.38/src/nef_pipelines/tools/chains/clone.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     1417 2023-03-21 20:24:03.000000 nef_pipelines-0.1.38/src/nef_pipelines/tools/chains/list.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     2670 2023-03-18 23:07:53.000000 nef_pipelines-0.1.38/src/nef_pipelines/tools/chains/rename.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     9203 2023-01-10 10:15:33.000000 nef_pipelines-0.1.38/src/nef_pipelines/tools/chains/renumber.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:45.834609 nef_pipelines-0.1.38/src/nef_pipelines/tools/entry/
+-rw-r--r--   0 garythompson   (501) staff       (20)      376 2022-11-29 12:15:24.000000 nef_pipelines-0.1.38/src/nef_pipelines/tools/entry/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)      692 2023-02-07 13:11:22.000000 nef_pipelines-0.1.38/src/nef_pipelines/tools/entry/rename.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:45.852593 nef_pipelines-0.1.38/src/nef_pipelines/tools/frames/
+-rw-r--r--   0 garythompson   (501) staff       (20)      639 2023-04-15 16:14:41.000000 nef_pipelines-0.1.38/src/nef_pipelines/tools/frames/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     2556 2023-03-19 00:07:20.000000 nef_pipelines-0.1.38/src/nef_pipelines/tools/frames/delete.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     4111 2023-03-21 19:38:23.000000 nef_pipelines-0.1.38/src/nef_pipelines/tools/frames/insert.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     6996 2023-04-15 16:55:03.000000 nef_pipelines-0.1.38/src/nef_pipelines/tools/frames/list.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     6711 2023-04-17 20:20:20.000000 nef_pipelines-0.1.38/src/nef_pipelines/tools/frames/rename.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     8952 2023-03-21 20:29:06.000000 nef_pipelines-0.1.38/src/nef_pipelines/tools/frames/tabulate.py
+-rw-r--r--   0 garythompson   (501) staff       (20)      871 2023-02-07 23:05:12.000000 nef_pipelines-0.1.38/src/nef_pipelines/tools/header.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     5132 2022-11-27 18:48:20.000000 nef_pipelines-0.1.38/src/nef_pipelines/tools/offset_shifts.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:45.858711 nef_pipelines-0.1.38/src/nef_pipelines/tools/peaks/
+-rw-r--r--   0 garythompson   (501) staff       (20)    10891 2023-03-23 08:18:29.000000 nef_pipelines-0.1.38/src/nef_pipelines/tools/peaks/match.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    10539 2022-12-22 18:47:15.000000 nef_pipelines-0.1.38/src/nef_pipelines/tools/res_assign.py_unused
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:45.862605 nef_pipelines-0.1.38/src/nef_pipelines/tools/shifts/
+-rw-r--r--   0 garythompson   (501) staff       (20)      372 2023-03-20 08:59:26.000000 nef_pipelines-0.1.38/src/nef_pipelines/tools/shifts/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     7095 2023-04-26 16:43:57.000000 nef_pipelines-0.1.38/src/nef_pipelines/tools/shifts/make_peaks.py
+-rw-r--r--   0 garythompson   (501) staff       (20)      200 2022-11-28 23:58:46.000000 nef_pipelines-0.1.38/src/nef_pipelines/tools/sink.py
+-rw-r--r--   0 garythompson   (501) staff       (20)      445 2022-11-28 21:57:18.000000 nef_pipelines-0.1.38/src/nef_pipelines/tools/stream.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     3753 2023-04-17 20:08:48.000000 nef_pipelines-0.1.38/src/nef_pipelines/tools/test.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:45.865449 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:45.866205 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/csv/
+-rw-r--r--   0 garythompson   (501) staff       (20)      409 2023-03-19 00:07:20.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/csv/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:45.873805 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/csv/importers/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-01-18 16:41:09.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/csv/importers/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    14955 2023-01-31 09:30:29.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/csv/importers/rdcs.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:45.875599 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/echidna/
+-rw-r--r--   0 garythompson   (501) staff       (20)      465 2023-05-04 20:35:04.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/echidna/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:45.877932 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/echidna/importers/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-05-04 20:35:04.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/echidna/importers/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    15615 2023-05-06 20:59:02.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/echidna/importers/peaks.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:45.883579 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/fasta/
+-rw-r--r--   0 garythompson   (501) staff       (20)      646 2022-11-27 19:51:40.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/fasta/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:45.890425 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/fasta/exporters/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/fasta/exporters/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     3952 2023-03-22 17:47:24.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/fasta/exporters/sequence.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:45.894256 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/fasta/importers/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/fasta/importers/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     5532 2023-04-24 20:34:49.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/fasta/importers/sequence.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:45.901099 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/mars/
+-rw-r--r--   0 garythompson   (501) staff       (20)      946 2023-02-15 11:20:25.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/mars/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:45.913219 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/mars/exporters/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/mars/exporters/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     6571 2023-02-15 21:49:23.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/mars/exporters/fragments.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     4299 2023-02-15 22:21:34.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/mars/exporters/input.py
+-rw-r--r--   0 garythompson   (501) staff       (20)      780 2022-11-28 23:56:55.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/mars/exporters/sequence.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     6001 2023-03-11 19:52:09.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/mars/exporters/shifts.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:45.932653 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/mars/importers/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-02-05 10:22:38.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/mars/importers/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    11657 2023-04-24 20:38:57.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/mars/importers/shifts.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:45.941429 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/nmrpipe/
+-rw-r--r--   0 garythompson   (501) staff       (20)      679 2022-11-27 19:52:05.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/nmrpipe/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:45.950577 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/nmrpipe/importers/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/nmrpipe/importers/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     2414 2022-12-13 19:17:42.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/nmrpipe/importers/peaks.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     3498 2023-04-24 20:38:57.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/nmrpipe/importers/sequence.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     3151 2023-04-24 20:36:47.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/nmrpipe/importers/shifts.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    20224 2023-04-24 21:17:19.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/nmrpipe/nmrpipe_lib.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:45.959305 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/nmrview/
+-rw-r--r--   0 garythompson   (501) staff       (20)     1056 2023-01-16 22:48:48.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/nmrview/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:45.978678 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/nmrview/exporters/
+-rw-r--r--   0 garythompson   (501) staff       (20)    13841 2023-02-07 13:14:10.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/nmrview/exporters/peaks.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     7053 2023-01-30 07:39:27.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/nmrview/exporters/sequences.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     9136 2023-01-16 22:47:55.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/nmrview/exporters/shifts.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:45.994877 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/nmrview/importers/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/nmrview/importers/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    17212 2022-12-22 18:41:48.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/nmrview/importers/peaks.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     2330 2023-04-24 20:38:58.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/nmrview/importers/sequence.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     5787 2023-04-24 20:38:58.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/nmrview/importers/shifts.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     8866 2023-01-16 22:43:21.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/nmrview/nmrview_lib.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:46.000877 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/pales/
+-rw-r--r--   0 garythompson   (501) staff       (20)      660 2022-11-27 19:52:13.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/pales/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:46.011540 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/pales/exporters/
+-rw-r--r--   0 garythompson   (501) staff       (20)    10961 2023-05-06 20:57:59.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/pales/exporters/rdcs.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     4817 2023-03-06 22:17:20.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/pales/exporters/template.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:46.016721 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/pdbx/
+-rw-r--r--   0 garythompson   (501) staff       (20)      454 2022-12-17 16:50:37.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/pdbx/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:46.018785 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/pdbx/importers/
+-rw-r--r--   0 garythompson   (501) staff       (20)     4655 2022-12-17 16:51:05.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/pdbx/importers/sequence.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:46.023576 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/rpf/
+-rw-r--r--   0 garythompson   (501) staff       (20)      608 2023-03-23 08:19:19.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/rpf/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:46.035619 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/rpf/exporters/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-03-22 21:34:49.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/rpf/exporters/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    11873 2023-03-22 22:37:50.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/rpf/exporters/shifts.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:46.038668 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/shifty/
+-rw-r--r--   0 garythompson   (501) staff       (20)      523 2023-02-08 16:38:07.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/shifty/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:46.049482 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/shifty/exporters/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-02-05 22:19:02.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/shifty/exporters/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     6339 2023-04-24 20:32:00.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/shifty/exporters/shifts.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:46.065195 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/sparky/
+-rw-r--r--   0 garythompson   (501) staff       (20)      804 2023-04-26 18:38:57.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/sparky/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:46.071701 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/sparky/exporters/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-03-18 23:36:58.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/sparky/exporters/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    15804 2023-05-04 07:46:41.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/sparky/exporters/peaks.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:46.090210 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/sparky/importers/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-01-16 13:30:23.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/sparky/importers/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    16125 2023-05-06 20:58:05.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/sparky/importers/peaks.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     6463 2023-04-26 18:39:25.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/sparky/importers/sequence.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     8953 2023-03-19 00:07:20.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/sparky/importers/shifts.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     8510 2023-05-06 14:33:01.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/sparky/sparky_lib.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:46.093904 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/xcamshift/
+-rw-r--r--   0 garythompson   (501) staff       (20)      554 2023-02-07 22:05:04.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/xcamshift/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:46.119815 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/xcamshift/exporters/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-02-05 22:19:02.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/xcamshift/exporters/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     3787 2023-02-07 22:05:13.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/xcamshift/exporters/shifts.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:46.130306 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/xplor/
+-rw-r--r--   0 garythompson   (501) staff       (20)      933 2023-02-05 22:57:14.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/xplor/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:46.144091 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/xplor/exporters/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-01-20 20:08:15.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/xplor/exporters/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     7167 2023-01-31 09:54:44.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/xplor/exporters/rdcs.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:46.169709 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/xplor/importers/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-12-17 17:33:41.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/xplor/importers/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     2834 2023-03-24 21:54:07.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/xplor/importers/dihedrals.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     2888 2023-01-11 22:37:57.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/xplor/importers/distances.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     3298 2023-01-04 12:32:55.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/xplor/importers/sequence.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     3663 2022-12-22 19:24:58.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/xplor/psf_lib.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    38877 2023-01-11 22:37:34.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/xplor/xplor_lib.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:45.099802 nef_pipelines-0.1.38/src/nef_pipelines.egg-info/
+-rw-r--r--   0 garythompson   (501) staff       (20)     8765 2023-05-06 21:01:44.000000 nef_pipelines-0.1.38/src/nef_pipelines.egg-info/PKG-INFO
+-rw-r--r--   0 garythompson   (501) staff       (20)    13928 2023-05-06 21:01:44.000000 nef_pipelines-0.1.38/src/nef_pipelines.egg-info/SOURCES.txt
+-rw-r--r--   0 garythompson   (501) staff       (20)        1 2023-05-06 21:01:44.000000 nef_pipelines-0.1.38/src/nef_pipelines.egg-info/dependency_links.txt
+-rw-r--r--   0 garythompson   (501) staff       (20)       48 2023-05-06 21:01:44.000000 nef_pipelines-0.1.38/src/nef_pipelines.egg-info/entry_points.txt
+-rw-r--r--   0 garythompson   (501) staff       (20)        1 2022-11-27 19:48:54.000000 nef_pipelines-0.1.38/src/nef_pipelines.egg-info/not-zip-safe
+-rw-r--r--   0 garythompson   (501) staff       (20)      363 2023-05-06 21:01:44.000000 nef_pipelines-0.1.38/src/nef_pipelines.egg-info/requires.txt
+-rw-r--r--   0 garythompson   (501) staff       (20)       14 2023-05-06 21:01:44.000000 nef_pipelines-0.1.38/src/nef_pipelines.egg-info/top_level.txt
+-rw-r--r--   0 garythompson   (501) staff       (20)     3032 2023-02-01 22:03:42.000000 nef_pipelines-0.1.38/tox.ini
```

### Comparing `nef_pipelines-0.1.37/.github/workflows/ci.yml` & `nef_pipelines-0.1.38/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/.idea/inspectionProfiles/Project_Default.xml` & `nef_pipelines-0.1.38/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/.pre-commit-config.yaml` & `nef_pipelines-0.1.38/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/CHANGELOG.md` & `nef_pipelines-0.1.38/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -136,7 +136,11 @@
 
 sparky peak import fully supported with all fields shown in the spark manual
 
 ## version 0.1.37
 
 improved sparky assignment parsing which is also refactored into a reusable
 library
+
+## version 0.1.37
+
+initial experiments support for echidna peaks files
```

### Comparing `nef_pipelines-0.1.37/CONTRIBUTING.md` & `nef_pipelines-0.1.38/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/LICENSE.txt` & `nef_pipelines-0.1.38/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/PKG-INFO` & `nef_pipelines-0.1.38/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nef_pipelines
-Version: 0.1.37
+Version: 0.1.38
 Summary: Tools for Manipulating NEF [NMR Exchange Format] Files and Foreign File Access
 Home-page: https://github.com/varioustoxins/NEF-Pipelines
 Author: varioustoxins
 Author-email: g.s.thompson@kent.ac.uk
 License: LGPL-2.1
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
```

### Comparing `nef_pipelines-0.1.37/README.md` & `nef_pipelines-0.1.38/README.md`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/TODO.md` & `nef_pipelines-0.1.38/TODO.md`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/references/Nmr Experiment Nomenclature v2.docx` & `nef_pipelines-0.1.38/references/Nmr Experiment Nomenclature v2.docx`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/references/fogh.vrankenj.bio.nmr.2006.36.147.pdf` & `nef_pipelines-0.1.38/references/fogh.vrankenj.bio.nmr.2006.36.147.pdf`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/release_to_pypi.sh` & `nef_pipelines-0.1.38/release_to_pypi.sh`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/setup.cfg` & `nef_pipelines-0.1.38/setup.cfg`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/setup.py` & `nef_pipelines-0.1.38/setup.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/__init__.py` & `nef_pipelines-0.1.38/src/nef_pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/data/mmcif_nef_v1_1.dic` & `nef_pipelines-0.1.38/src/nef_pipelines/data/mmcif_nef_v1_1.dic`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/lib/header_lib.py` & `nef_pipelines-0.1.38/src/nef_pipelines/lib/header_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/lib/isotope_lib.py` & `nef_pipelines-0.1.38/src/nef_pipelines/lib/isotope_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/lib/nef_frames_lib.py` & `nef_pipelines-0.1.38/src/nef_pipelines/lib/nef_frames_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/lib/nef_lib.py` & `nef_pipelines-0.1.38/src/nef_pipelines/lib/nef_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/lib/peak_lib.py` & `nef_pipelines-0.1.38/src/nef_pipelines/lib/peak_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/lib/sequence_lib.py` & `nef_pipelines-0.1.38/src/nef_pipelines/lib/sequence_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/lib/shift_lib.py` & `nef_pipelines-0.1.38/src/nef_pipelines/lib/shift_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/lib/spectra_lib.py` & `nef_pipelines-0.1.38/src/nef_pipelines/lib/spectra_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/lib/structures.py` & `nef_pipelines-0.1.38/src/nef_pipelines/lib/structures.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/lib/test_lib.py` & `nef_pipelines-0.1.38/src/nef_pipelines/lib/test_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/lib/util.py` & `nef_pipelines-0.1.38/src/nef_pipelines/lib/util.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/main.py` & `nef_pipelines-0.1.38/src/nef_pipelines/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,14 +82,15 @@
             "nef_pipelines.tools.frames",
             "nef_pipelines.tools.header",
             "nef_pipelines.tools.peaks",
             "nef_pipelines.tools.shifts",
             "nef_pipelines.tools.stream",
             "nef_pipelines.tools.test",
             "nef_pipelines.transcoders.csv",
+            "nef_pipelines.transcoders.echidna",
             "nef_pipelines.transcoders.fasta",
             "nef_pipelines.transcoders.mars",
             "nef_pipelines.transcoders.nmrpipe",
             "nef_pipelines.transcoders.nmrview",
             "nef_pipelines.transcoders.pales",
             "nef_pipelines.transcoders.pdbx",
             "nef_pipelines.transcoders.rpf",
```

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/tests/chains/test_clone.py` & `nef_pipelines-0.1.38/src/nef_pipelines/tests/chains/test_clone.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/tests/chains/test_data/3aa.nef` & `nef_pipelines-0.1.38/src/nef_pipelines/tests/chains/test_data/3aa.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/tests/chains/test_data/3aa_x3.nef` & `nef_pipelines-0.1.38/src/nef_pipelines/tests/chains/test_data/3aa_x3.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/tests/chains/test_data/multi_chain_shifts.nef` & `nef_pipelines-0.1.38/src/nef_pipelines/tests/chains/test_data/multi_chain_shifts.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/tests/chains/test_rename.py` & `nef_pipelines-0.1.38/src/nef_pipelines/tests/chains/test_rename.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/tests/chains/test_renumber.py` & `nef_pipelines-0.1.38/src/nef_pipelines/tests/chains/test_renumber.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/tests/conftest.py` & `nef_pipelines-0.1.38/src/nef_pipelines/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/tests/csv/test_import_rdcs.py` & `nef_pipelines-0.1.38/src/nef_pipelines/tests/csv/test_import_rdcs.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/tests/fasta/test_sequence.py` & `nef_pipelines-0.1.38/src/nef_pipelines/tests/fasta/test_sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/tests/frames/test_data/frames.nef` & `nef_pipelines-0.1.38/src/nef_pipelines/tests/frames/test_data/frames.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/tests/frames/test_data/pales_test_1.nef` & `nef_pipelines-0.1.38/src/nef_pipelines/tests/frames/test_data/pales_test_1.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/tests/frames/test_delete.py` & `nef_pipelines-0.1.38/src/nef_pipelines/tests/frames/test_delete.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/tests/frames/test_list.py` & `nef_pipelines-0.1.38/src/nef_pipelines/tests/frames/test_list.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/tests/frames/test_rename.py` & `nef_pipelines-0.1.38/src/nef_pipelines/tests/frames/test_rename.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/tests/frames/test_tabulate.py` & `nef_pipelines-0.1.38/src/nef_pipelines/tests/frames/test_tabulate.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/tests/mars/test_data/sec5_short.neff` & `nef_pipelines-0.1.38/src/nef_pipelines/tests/mars/test_data/sec5_short.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/tests/mars/test_export_shifts.py` & `nef_pipelines-0.1.38/src/nef_pipelines/tests/mars/test_export_shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/tests/mars/test_import_shifts.py` & `nef_pipelines-0.1.38/src/nef_pipelines/tests/mars/test_import_shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/tests/nmrpipe/test_data/gb3.tab` & `nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrpipe/test_data/gb3.tab`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned.tab` & `nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned.tab`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned_trunc.tab` & `nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned_trunc.tab`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned_trunc_expected.tab` & `nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned_trunc_expected.tab`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/tests/nmrpipe/test_data/ns3_S135A_BMRB1.txt` & `nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrpipe/test_data/ns3_S135A_BMRB1.txt`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/tests/nmrpipe/test_data/test_header_entry.txt` & `nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrpipe/test_data/test_header_entry.txt`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/tests/nmrpipe/test_gdb.py` & `nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrpipe/test_gdb.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/tests/nmrpipe/test_peaks.py` & `nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrpipe/test_peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/tests/nmrpipe/test_sequence.py` & `nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrpipe/test_sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/tests/nmrpipe/test_shifts.py` & `nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrpipe/test_shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/tests/nmrview/tcl_diag.html` & `nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrview/tcl_diag.html`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/tests/nmrview/test_data/4peaks.xpk` & `nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrview/test_data/4peaks.xpk`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/tests/nmrview/test_data/expected_nmr_view.xpk` & `nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrview/test_data/expected_nmr_view.xpk`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/tests/nmrview/test_data/expected_sequence_and_peaks_nmrview.txt` & `nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrview/test_data/expected_sequence_and_peaks_nmrview.txt`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/tests/nmrview/test_data/nmrview_expected_4aa.txt` & `nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrview/test_data/nmrview_expected_4aa.txt`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/tests/nmrview/test_data/ppm.out` & `nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrview/test_data/ppm.out`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/tests/nmrview/test_data/ppm_out.seq` & `nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrview/test_data/ppm_out.seq`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/tests/nmrview/test_data/ppm_short_seq.nef` & `nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrview/test_data/ppm_short_seq.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/tests/nmrview/test_data/test_header_entry.txt` & `nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrview/test_data/test_header_entry.txt`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/tests/nmrview/test_export_peaks.py` & `nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrview/test_export_peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/tests/nmrview/test_export_sequences.py` & `nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrview/test_export_sequences.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/tests/nmrview/test_import_peaks.py` & `nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrview/test_import_peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/tests/nmrview/test_import_sequence.py` & `nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrview/test_import_sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/tests/nmrview/test_import_shifts.py` & `nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrview/test_import_shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/tests/nmrview/test_tcl.py` & `nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrview/test_tcl.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/tests/pales/test_data/pales_test_1.nef` & `nef_pipelines-0.1.38/src/nef_pipelines/tests/pales/test_data/pales_test_1.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/tests/pales/test_data/pales_test_2.nef` & `nef_pipelines-0.1.38/src/nef_pipelines/tests/pales/test_data/pales_test_2.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/tests/pales/test_data/pales_test_segids.nef` & `nef_pipelines-0.1.38/src/nef_pipelines/tests/pales/test_data/pales_test_segids.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/tests/pales/test_rdcs.py` & `nef_pipelines-0.1.38/src/nef_pipelines/tests/pales/test_rdcs.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/tests/pales/test_template.py` & `nef_pipelines-0.1.38/src/nef_pipelines/tests/pales/test_template.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/tests/pdbx/test_data/3a_ab.pdb` & `nef_pipelines-0.1.38/src/nef_pipelines/tests/pdbx/test_data/3a_ab.pdb`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/tests/pdbx/test_data/3a_cccc_dddd.pdb` & `nef_pipelines-0.1.38/src/nef_pipelines/tests/pdbx/test_data/3a_cccc_dddd.pdb`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/tests/pdbx/test_data/3a_no_chain_no_segid.pdb` & `nef_pipelines-0.1.38/src/nef_pipelines/tests/pdbx/test_data/3a_no_chain_no_segid.pdb`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/tests/pdbx/test_data/3aa.pdb` & `nef_pipelines-0.1.38/src/nef_pipelines/tests/pdbx/test_data/3aa.pdb`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/tests/pdbx/test_data/3aa11_13.pdb` & `nef_pipelines-0.1.38/src/nef_pipelines/tests/pdbx/test_data/3aa11_13.pdb`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/tests/pdbx/test_data/test_header_entry.txt` & `nef_pipelines-0.1.38/src/nef_pipelines/tests/pdbx/test_data/test_header_entry.txt`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/tests/pdbx/test_sequence.py` & `nef_pipelines-0.1.38/src/nef_pipelines/tests/pdbx/test_sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/tests/shifts/test_make_peaks.py` & `nef_pipelines-0.1.38/src/nef_pipelines/tests/shifts/test_make_peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/tests/shifty/test_export_shifts.py` & `nef_pipelines-0.1.38/src/nef_pipelines/tests/shifty/test_export_shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/tests/sparky/test_data/P3a_L273R_sequence_short.neff` & `nef_pipelines-0.1.38/src/nef_pipelines/tests/sparky/test_data/P3a_L273R_sequence_short.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/tests/sparky/test_data/peaks_short_with_assignments.neff` & `nef_pipelines-0.1.38/src/nef_pipelines/tests/sparky/test_data/peaks_short_with_assignments.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/tests/sparky/test_data/sparky_manual_basic_sequence.nef` & `nef_pipelines-0.1.38/src/nef_pipelines/tests/sparky/test_data/sparky_manual_basic_sequence.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/tests/sparky/test_data/test_shifts_P3a_L273R_shifts_short.txt` & `nef_pipelines-0.1.38/src/nef_pipelines/tests/sparky/test_data/test_shifts_P3a_L273R_shifts_short.txt`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short.neff` & `nef_pipelines-0.1.38/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_chains.neff` & `nef_pipelines-0.1.38/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_chains.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_different_residues.neff` & `nef_pipelines-0.1.38/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_different_residues.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_i_minus_one.neff` & `nef_pipelines-0.1.38/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_i_minus_one.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_overlapping_chains.neff` & `nef_pipelines-0.1.38/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_overlapping_chains.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/tests/sparky/test_export_peaks.py` & `nef_pipelines-0.1.38/src/nef_pipelines/tests/sparky/test_export_peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/tests/sparky/test_import_peaks.py` & `nef_pipelines-0.1.38/src/nef_pipelines/tests/sparky/test_import_peaks.py`

 * *Files 11% similar despite different names*

```diff
@@ -67,14 +67,31 @@
     result = run_and_report(app, ["--molecule-type", "dna", path])
 
     loop = isolate_loop(result.stdout, "sparky_sparky_manual_basic", "nef_peak")
 
     assert_lines_match(EXPECTED, str(loop))
 
 
+def test_basic_no_sequence_requires_sequence():
+
+    path = path_in_test_data(__file__, "sparky_manual_full_no_sequence.peaks")
+
+    sequence = open(
+        path_in_test_data(__file__, "sparky_manual_basic_sequence.nef")
+    ).read()
+
+    result = run_and_report(app, [path], input=sequence)
+
+    loop = isolate_loop(
+        result.stdout, "sparky_sparky_manual_full_no_sequence", "nef_peak"
+    )
+
+    assert_lines_match(EXPECTED, str(loop))
+
+
 def test_full():
 
     path = path_in_test_data(__file__, "sparky_manual_full.peaks")
 
     result = run_and_report(app, ["--molecule-type", "dna", path])
 
     loop = isolate_loop(result.stdout, "sparky_sparky_manual_full", "nef_peak")
```

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/tests/sparky/test_import_sequence.py` & `nef_pipelines-0.1.38/src/nef_pipelines/tests/sparky/test_import_sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/tests/sparky/test_import_shifts.py` & `nef_pipelines-0.1.38/src/nef_pipelines/tests/sparky/test_import_shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/tests/sparky/test_sparky_lib.py` & `nef_pipelines-0.1.38/src/nef_pipelines/tests/sparky/test_sparky_lib.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import string
 
 import pytest
 
-from nef_pipelines.transcoders.sparky.sparly_lib import (
+from nef_pipelines.transcoders.sparky.sparky_lib import (
     _strip_characters_left,
     parse_single_assignment,
 )
 
 
 def test_strip_characters_left_empty():
```

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/tests/test_data/3a_ab.neff` & `nef_pipelines-0.1.38/src/nef_pipelines/tests/test_data/3a_ab.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/tests/test_data/header.nef` & `nef_pipelines-0.1.38/src/nef_pipelines/tests/test_data/header.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/tests/test_data/multi_chain.nef` & `nef_pipelines-0.1.38/src/nef_pipelines/tests/test_data/multi_chain.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/tests/test_data/nef_3_peaks.nef` & `nef_pipelines-0.1.38/src/nef_pipelines/tests/test_data/nef_3_peaks.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/tests/test_data/tailin_seq_short.nef` & `nef_pipelines-0.1.38/src/nef_pipelines/tests/test_data/tailin_seq_short.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/tests/test_data/test_agv.neff` & `nef_pipelines-0.1.38/src/nef_pipelines/tests/test_data/test_agv.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/tests/test_data/ubiquitin_short.nef` & `nef_pipelines-0.1.38/src/nef_pipelines/tests/test_data/ubiquitin_short.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/tests/test_header.py` & `nef_pipelines-0.1.38/src/nef_pipelines/tests/test_header.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/tests/test_nef_lib.py` & `nef_pipelines-0.1.38/src/nef_pipelines/tests/test_nef_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/tests/test_sequence_lib.py` & `nef_pipelines-0.1.38/src/nef_pipelines/tests/test_sequence_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/tests/test_test.py` & `nef_pipelines-0.1.38/src/nef_pipelines/tests/test_test.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/tests/xcamshift/test_export_shifts.py` & `nef_pipelines-0.1.38/src/nef_pipelines/tests/xcamshift/test_export_shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/tests/xplor/test_data/3a_ab.psf` & `nef_pipelines-0.1.38/src/nef_pipelines/tests/xplor/test_data/3a_ab.psf`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/tests/xplor/test_data/3a_ab_rdcs.neff` & `nef_pipelines-0.1.38/src/nef_pipelines/tests/xplor/test_data/3a_ab_rdcs.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/tests/xplor/test_data/test_2_dihedrals.tbl` & `nef_pipelines-0.1.38/src/nef_pipelines/tests/xplor/test_data/test_2_dihedrals.tbl`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/tests/xplor/test_data/test_2_dihedrals_bad.tbl` & `nef_pipelines-0.1.38/src/nef_pipelines/tests/xplor/test_data/test_2_dihedrals_bad.tbl`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/tests/xplor/test_dihedrals.py` & `nef_pipelines-0.1.38/src/nef_pipelines/tests/xplor/test_dihedrals.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/tests/xplor/test_distances.py` & `nef_pipelines-0.1.38/src/nef_pipelines/tests/xplor/test_distances.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/tests/xplor/test_export_rdcs.py` & `nef_pipelines-0.1.38/src/nef_pipelines/tests/xplor/test_export_rdcs.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/tests/xplor/test_import_sequence.py` & `nef_pipelines-0.1.38/src/nef_pipelines/tests/xplor/test_import_sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/tests/xplor/test_psf_lib.py` & `nef_pipelines-0.1.38/src/nef_pipelines/tests/xplor/test_psf_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/tests/xplor/test_xplor_lib.py` & `nef_pipelines-0.1.38/src/nef_pipelines/tests/xplor/test_xplor_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/tools/about.py` & `nef_pipelines-0.1.38/src/nef_pipelines/tools/about.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/tools/chains/__init__.py` & `nef_pipelines-0.1.38/src/nef_pipelines/tools/chains/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/tools/chains/clone.py` & `nef_pipelines-0.1.38/src/nef_pipelines/tools/chains/clone.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/tools/chains/list.py` & `nef_pipelines-0.1.38/src/nef_pipelines/tools/chains/list.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/tools/chains/rename.py` & `nef_pipelines-0.1.38/src/nef_pipelines/tools/chains/rename.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/tools/chains/renumber.py` & `nef_pipelines-0.1.38/src/nef_pipelines/tools/chains/renumber.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/tools/entry/rename.py` & `nef_pipelines-0.1.38/src/nef_pipelines/tools/entry/rename.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/tools/frames/__init__.py` & `nef_pipelines-0.1.38/src/nef_pipelines/tools/frames/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/tools/frames/delete.py` & `nef_pipelines-0.1.38/src/nef_pipelines/tools/frames/delete.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/tools/frames/insert.py` & `nef_pipelines-0.1.38/src/nef_pipelines/tools/frames/insert.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/tools/frames/list.py` & `nef_pipelines-0.1.38/src/nef_pipelines/tools/frames/list.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/tools/frames/rename.py` & `nef_pipelines-0.1.38/src/nef_pipelines/tools/frames/rename.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/tools/frames/tabulate.py` & `nef_pipelines-0.1.38/src/nef_pipelines/tools/frames/tabulate.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/tools/header.py` & `nef_pipelines-0.1.38/src/nef_pipelines/tools/header.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/tools/offset_shifts.py` & `nef_pipelines-0.1.38/src/nef_pipelines/tools/offset_shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/tools/peaks/match.py` & `nef_pipelines-0.1.38/src/nef_pipelines/tools/peaks/match.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/tools/res_assign.py_unused` & `nef_pipelines-0.1.38/src/nef_pipelines/tools/res_assign.py_unused`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/tools/shifts/make_peaks.py` & `nef_pipelines-0.1.38/src/nef_pipelines/tools/shifts/make_peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/tools/test.py` & `nef_pipelines-0.1.38/src/nef_pipelines/tools/test.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/transcoders/csv/importers/rdcs.py` & `nef_pipelines-0.1.38/src/nef_pipelines/transcoders/csv/importers/rdcs.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/transcoders/fasta/__init__.py` & `nef_pipelines-0.1.38/src/nef_pipelines/transcoders/fasta/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/transcoders/fasta/exporters/sequence.py` & `nef_pipelines-0.1.38/src/nef_pipelines/transcoders/fasta/exporters/sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/transcoders/fasta/importers/sequence.py` & `nef_pipelines-0.1.38/src/nef_pipelines/transcoders/fasta/importers/sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/transcoders/mars/__init__.py` & `nef_pipelines-0.1.38/src/nef_pipelines/transcoders/mars/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/transcoders/mars/exporters/fragments.py` & `nef_pipelines-0.1.38/src/nef_pipelines/transcoders/mars/exporters/fragments.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/transcoders/mars/exporters/input.py` & `nef_pipelines-0.1.38/src/nef_pipelines/transcoders/mars/exporters/input.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/transcoders/mars/exporters/sequence.py` & `nef_pipelines-0.1.38/src/nef_pipelines/transcoders/mars/exporters/sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/transcoders/mars/exporters/shifts.py` & `nef_pipelines-0.1.38/src/nef_pipelines/transcoders/mars/exporters/shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/transcoders/mars/importers/shifts.py` & `nef_pipelines-0.1.38/src/nef_pipelines/transcoders/mars/importers/shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/transcoders/nmrpipe/__init__.py` & `nef_pipelines-0.1.38/src/nef_pipelines/transcoders/nmrpipe/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/transcoders/nmrpipe/importers/peaks.py` & `nef_pipelines-0.1.38/src/nef_pipelines/transcoders/nmrpipe/importers/peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/transcoders/nmrpipe/importers/sequence.py` & `nef_pipelines-0.1.38/src/nef_pipelines/transcoders/nmrpipe/importers/sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/transcoders/nmrpipe/importers/shifts.py` & `nef_pipelines-0.1.38/src/nef_pipelines/transcoders/nmrpipe/importers/shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/transcoders/nmrpipe/nmrpipe_lib.py` & `nef_pipelines-0.1.38/src/nef_pipelines/transcoders/nmrpipe/nmrpipe_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/transcoders/nmrview/__init__.py` & `nef_pipelines-0.1.38/src/nef_pipelines/transcoders/nmrview/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/transcoders/nmrview/exporters/peaks.py` & `nef_pipelines-0.1.38/src/nef_pipelines/transcoders/nmrview/exporters/peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/transcoders/nmrview/exporters/sequences.py` & `nef_pipelines-0.1.38/src/nef_pipelines/transcoders/nmrview/exporters/sequences.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/transcoders/nmrview/exporters/shifts.py` & `nef_pipelines-0.1.38/src/nef_pipelines/transcoders/nmrview/exporters/shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/transcoders/nmrview/importers/peaks.py` & `nef_pipelines-0.1.38/src/nef_pipelines/transcoders/nmrview/importers/peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/transcoders/nmrview/importers/sequence.py` & `nef_pipelines-0.1.38/src/nef_pipelines/transcoders/nmrview/importers/sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/transcoders/nmrview/importers/shifts.py` & `nef_pipelines-0.1.38/src/nef_pipelines/transcoders/nmrview/importers/shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/transcoders/nmrview/nmrview_lib.py` & `nef_pipelines-0.1.38/src/nef_pipelines/transcoders/nmrview/nmrview_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/transcoders/pales/__init__.py` & `nef_pipelines-0.1.38/src/nef_pipelines/transcoders/pales/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/transcoders/pales/exporters/rdcs.py` & `nef_pipelines-0.1.38/src/nef_pipelines/transcoders/pales/exporters/rdcs.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     UNUSED,
     loop_row_dict_iter,
     read_entry_from_file_or_stdin_or_exit_error,
     select_frames_by_name,
 )
 from nef_pipelines.lib.sequence_lib import sequence_from_entry, sequence_to_chains
 from nef_pipelines.lib.structures import AtomLabel, RdcRestraint, SequenceResidue
+from nef_pipelines.lib.translation_lib import translate_atom_label
 from nef_pipelines.lib.util import (
     STDIN,
     exit_error,
     flatten,
     get_display_file_name,
     read_float_or_exit,
 )
@@ -132,26 +133,28 @@
 
         print()
 
         _print_restraints(restraints, weights, segids)
 
 
 def _translate_atom_names(
-    restraints: List[RdcRestraint], naming_scheme="iupac"
+    restraints: List[RdcRestraint], naming_scheme="xplor_to_iupac"
 ) -> List[RdcRestraint]:
     result = []
     for restraint in restraints:
         atom_1 = restraint.atom_1
         atom_2 = restraint.atom_2
 
-        if atom_1.atom_name == "H":
-            restraint.atom_1 = replace(atom_1, atom_name="HN")
-
-        if atom_2.atom_name == "H":
-            restraint.atom_1 = replace(atom_2, atom_name="HN")
+        translation = {"H": "HN"}
+        atom_1 = translate_atom_label(atom_1, translation)
+        atom_2 = translate_atom_label(atom_2, translation)
+
+        restraint = replace(restraint, atom_1=atom_1)
+        restraint = replace(restraint, atom_2=atom_2)
+        restraint.atom_1 = atom_1
 
         result.append(restraint)
 
     return result
 
 
 def _rdc_restraints_from_frame(frame: Saveframe, weights: Dict[Tuple[str, str], float]):
```

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/transcoders/pales/exporters/template.py` & `nef_pipelines-0.1.38/src/nef_pipelines/transcoders/pales/exporters/template.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/transcoders/pdbx/importers/sequence.py` & `nef_pipelines-0.1.38/src/nef_pipelines/transcoders/pdbx/importers/sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/transcoders/rpf/__init__.py` & `nef_pipelines-0.1.38/src/nef_pipelines/transcoders/rpf/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/transcoders/rpf/exporters/shifts.py` & `nef_pipelines-0.1.38/src/nef_pipelines/transcoders/rpf/exporters/shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/transcoders/shifty/__init__.py` & `nef_pipelines-0.1.38/src/nef_pipelines/transcoders/shifty/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/transcoders/shifty/exporters/shifts.py` & `nef_pipelines-0.1.38/src/nef_pipelines/transcoders/shifty/exporters/shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/transcoders/sparky/__init__.py` & `nef_pipelines-0.1.38/src/nef_pipelines/transcoders/sparky/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/transcoders/sparky/exporters/peaks.py` & `nef_pipelines-0.1.38/src/nef_pipelines/transcoders/sparky/exporters/peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/transcoders/sparky/importers/peaks.py` & `nef_pipelines-0.1.38/src/nef_pipelines/transcoders/sparky/importers/peaks.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,25 +13,26 @@
     UNUSED,
     add_frames_to_entry,
     read_or_create_entry_exit_error_on_bad_file,
 )
 from nef_pipelines.lib.peak_lib import peaks_to_frame
 from nef_pipelines.lib.sequence_lib import MoleculeTypes, sequence_from_entry
 from nef_pipelines.lib.structures import LineInfo, NewPeak, PeakFitMethod, ShiftData
+from nef_pipelines.lib.translation_lib import translate_new_peak
 from nef_pipelines.lib.util import (
     STDIN,
     exit_error,
     is_float,
     parse_comma_separated_options,
 )
 from nef_pipelines.transcoders.sparky import import_app
 from nef_pipelines.transcoders.sparky.importers.shifts import (
     _exit_if_chain_codes_and_file_name_dont_match,
 )
-from nef_pipelines.transcoders.sparky.sparly_lib import parse_assignments
+from nef_pipelines.transcoders.sparky.sparky_lib import parse_assignments
 
 
 # TODO: this needs to be moved to a library
 class SparkyPeakListException(Exception):
     pass
 
 
@@ -161,14 +162,16 @@
             lines,
             file_name=file_name,
             molecule_type=molecule_type,
             chain_code=chain_code,
             sequence=sequence,
         )
 
+        sparky_peaks = [translate_new_peak(peak) for peak in sparky_peaks]
+
         dimensions = _guess_dimensions_if_not_defined_or_throw(
             sparky_peaks, input_dimensions
         )
 
         dimensions = [{"axis_code": dimension} for dimension in dimensions]
 
         frame = peaks_to_frame(sparky_peaks, dimensions, spectrometer_frequency)
```

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/transcoders/sparky/importers/sequence.py` & `nef_pipelines-0.1.38/src/nef_pipelines/transcoders/sparky/importers/sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/transcoders/sparky/importers/shifts.py` & `nef_pipelines-0.1.38/src/nef_pipelines/transcoders/sparky/importers/shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/transcoders/sparky/sparly_lib.py` & `nef_pipelines-0.1.38/src/nef_pipelines/transcoders/sparky/sparky_lib.py`

 * *Files 1% similar despite different names*

```diff
@@ -182,21 +182,14 @@
                 msg = f"""
                     The residue name {residue_name} is not defined for the molecule type {molecule_type}
                     at line {line_info.line_no} in file {line_info.file_name} the line was
                     {line_info.line}
                 """
                 exit_error(msg)
 
-        residue = Residue(
-            chain_code=chain_code,
-            sequence_code=sequence_code,
-            residue_name=translated_residue_name,
-        )
-        assignment = AtomLabel(residue, atom_name)
-
         residue_name_key = (chain_code, sequence_code)
 
         if residue_name == UNUSED and residue_name_lookup is None:
             msg = f"""
                 no sequence was loaded and the assignment {assignments} while it has a sequence code {sequence_code}
                 and chain code {chain_code} doesn't define a residue type, please provide a sequence in the input
                 stream
@@ -206,26 +199,33 @@
 
             if (
                 residue_name_lookup is not None
                 and residue_name_key in residue_name_lookup
             ):
                 translated_residue_name = residue_name_lookup[residue_name_key]
 
-        if sequence and (residue_name_key not in residue_name_lookup):
+        if len(sequence) > 0 and (residue_name_key not in residue_name_lookup):
             msg = f"""
-                the chain code {chain_code} and sequence_code {sequence} from
+                the chain code {chain_code} and sequence_code {sequence_code} from
                 line {line_info.line_no} in file {line_info.file_name} were not found
                 in the input sequence, the full line was
 
                 {line_info.line}
 
                 if you wish to input the peaks without validating against the input sequence use the
                 --no-validate option of sparky import peaks
             """
             exit_error(msg)
 
+        residue = Residue(
+            chain_code=chain_code,
+            sequence_code=sequence_code,
+            residue_name=translated_residue_name,
+        )
+        assignment = AtomLabel(residue, atom_name)
+
         result.append(assignment)
 
         last_sequence_code = sequence_code
         last_residue_name = residue_name
 
     return result
```

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/transcoders/xcamshift/__init__.py` & `nef_pipelines-0.1.38/src/nef_pipelines/transcoders/xcamshift/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/transcoders/xcamshift/exporters/shifts.py` & `nef_pipelines-0.1.38/src/nef_pipelines/transcoders/xcamshift/exporters/shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/transcoders/xplor/__init__.py` & `nef_pipelines-0.1.38/src/nef_pipelines/transcoders/xplor/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/transcoders/xplor/exporters/rdcs.py` & `nef_pipelines-0.1.38/src/nef_pipelines/transcoders/xplor/exporters/rdcs.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/transcoders/xplor/importers/dihedrals.py` & `nef_pipelines-0.1.38/src/nef_pipelines/transcoders/xplor/importers/dihedrals.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/transcoders/xplor/importers/distances.py` & `nef_pipelines-0.1.38/src/nef_pipelines/transcoders/xplor/importers/distances.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/transcoders/xplor/importers/sequence.py` & `nef_pipelines-0.1.38/src/nef_pipelines/transcoders/xplor/importers/sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/transcoders/xplor/psf_lib.py` & `nef_pipelines-0.1.38/src/nef_pipelines/transcoders/xplor/psf_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines/transcoders/xplor/xplor_lib.py` & `nef_pipelines-0.1.38/src/nef_pipelines/transcoders/xplor/xplor_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines.egg-info/PKG-INFO` & `nef_pipelines-0.1.38/src/nef_pipelines.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nef-pipelines
-Version: 0.1.37
+Version: 0.1.38
 Summary: Tools for Manipulating NEF [NMR Exchange Format] Files and Foreign File Access
 Home-page: https://github.com/varioustoxins/NEF-Pipelines
 Author: varioustoxins
 Author-email: g.s.thompson@kent.ac.uk
 License: LGPL-2.1
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
```

### Comparing `nef_pipelines-0.1.37/src/nef_pipelines.egg-info/SOURCES.txt` & `nef_pipelines-0.1.38/src/nef_pipelines.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -42,14 +42,15 @@
 src/nef_pipelines/lib/nef_lib.py
 src/nef_pipelines/lib/peak_lib.py
 src/nef_pipelines/lib/sequence_lib.py
 src/nef_pipelines/lib/shift_lib.py
 src/nef_pipelines/lib/spectra_lib.py
 src/nef_pipelines/lib/structures.py
 src/nef_pipelines/lib/test_lib.py
+src/nef_pipelines/lib/translation_lib.py
 src/nef_pipelines/lib/typer_utils.py
 src/nef_pipelines/lib/util.py
 src/nef_pipelines/lib/translation/__init__.py
 src/nef_pipelines/nef_app/__init__.py
 src/nef_pipelines/tests/conftest.py
 src/nef_pipelines/tests/test_header.py
 src/nef_pipelines/tests/test_nef_lib.py
@@ -62,14 +63,18 @@
 src/nef_pipelines/tests/chains/test_renumber.py
 src/nef_pipelines/tests/chains/test_data/3aa.nef
 src/nef_pipelines/tests/chains/test_data/3aa_x3.nef
 src/nef_pipelines/tests/chains/test_data/multi_chain_shifts.nef
 src/nef_pipelines/tests/csv/test_import_rdcs.py
 src/nef_pipelines/tests/csv/test_data/short.csv
 src/nef_pipelines/tests/csv/test_data/short_complete.csv
+src/nef_pipelines/tests/echidna/__init__.py
+src/nef_pipelines/tests/echidna/test_import_peaks.py
+src/nef_pipelines/tests/echidna/test_data/echidna_peaks.txt
+src/nef_pipelines/tests/echidna/test_data/echidna_sequence.nef
 src/nef_pipelines/tests/fasta/test_sequence.py
 src/nef_pipelines/tests/fasta/test_data/3aa.fasta
 src/nef_pipelines/tests/fasta/test_data/3aa_x2.fasta
 src/nef_pipelines/tests/frames/__init__.py
 src/nef_pipelines/tests/frames/test_delete.py
 src/nef_pipelines/tests/frames/test_list.py
 src/nef_pipelines/tests/frames/test_rename.py
@@ -148,14 +153,15 @@
 src/nef_pipelines/tests/sparky/test_data/peaks_short_with_assignments.neff
 src/nef_pipelines/tests/sparky/test_data/sparky_basic_sequence_dna.txt
 src/nef_pipelines/tests/sparky/test_data/sparky_basic_sequence_protein.txt
 src/nef_pipelines/tests/sparky/test_data/sparky_manual_basic.peaks
 src/nef_pipelines/tests/sparky/test_data/sparky_manual_basic_sequence.nef
 src/nef_pipelines/tests/sparky/test_data/sparky_manual_full.peaks
 src/nef_pipelines/tests/sparky/test_data/sparky_manual_full_comment.peaks
+src/nef_pipelines/tests/sparky/test_data/sparky_manual_full_no_sequence.peaks
 src/nef_pipelines/tests/sparky/test_data/test_shifts_P3a_L273R_shifts_short.txt
 src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short.neff
 src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_chains.neff
 src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_different_residues.neff
 src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_i_minus_one.neff
 src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_overlapping_chains.neff
 src/nef_pipelines/tests/test_data/3a_ab.neff
@@ -211,14 +217,17 @@
 src/nef_pipelines/tools/peaks/match.py
 src/nef_pipelines/tools/shifts/__init__.py
 src/nef_pipelines/tools/shifts/make_peaks.py
 src/nef_pipelines/transcoders/__init__.py
 src/nef_pipelines/transcoders/csv/__init__.py
 src/nef_pipelines/transcoders/csv/importers/__init__.py
 src/nef_pipelines/transcoders/csv/importers/rdcs.py
+src/nef_pipelines/transcoders/echidna/__init__.py
+src/nef_pipelines/transcoders/echidna/importers/__init__.py
+src/nef_pipelines/transcoders/echidna/importers/peaks.py
 src/nef_pipelines/transcoders/fasta/__init__.py
 src/nef_pipelines/transcoders/fasta/exporters/__init__.py
 src/nef_pipelines/transcoders/fasta/exporters/sequence.py
 src/nef_pipelines/transcoders/fasta/importers/__init__.py
 src/nef_pipelines/transcoders/fasta/importers/sequence.py
 src/nef_pipelines/transcoders/mars/__init__.py
 src/nef_pipelines/transcoders/mars/exporters/__init__.py
@@ -251,15 +260,15 @@
 src/nef_pipelines/transcoders/rpf/__init__.py
 src/nef_pipelines/transcoders/rpf/exporters/__init__.py
 src/nef_pipelines/transcoders/rpf/exporters/shifts.py
 src/nef_pipelines/transcoders/shifty/__init__.py
 src/nef_pipelines/transcoders/shifty/exporters/__init__.py
 src/nef_pipelines/transcoders/shifty/exporters/shifts.py
 src/nef_pipelines/transcoders/sparky/__init__.py
-src/nef_pipelines/transcoders/sparky/sparly_lib.py
+src/nef_pipelines/transcoders/sparky/sparky_lib.py
 src/nef_pipelines/transcoders/sparky/exporters/__init__.py
 src/nef_pipelines/transcoders/sparky/exporters/peaks.py
 src/nef_pipelines/transcoders/sparky/importers/__init__.py
 src/nef_pipelines/transcoders/sparky/importers/peaks.py
 src/nef_pipelines/transcoders/sparky/importers/sequence.py
 src/nef_pipelines/transcoders/sparky/importers/shifts.py
 src/nef_pipelines/transcoders/xcamshift/__init__.py
```

### Comparing `nef_pipelines-0.1.37/tox.ini` & `nef_pipelines-0.1.38/tox.ini`

 * *Files identical despite different names*

