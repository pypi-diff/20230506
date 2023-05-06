# Comparing `tmp/vasprocar-1.1.15.3.tar.gz` & `tmp/vasprocar-1.1.15.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vasprocar-1.1.15.3.tar", last modified: Thu May  4 15:52:38 2023, max compression
+gzip compressed data, was "vasprocar-1.1.15.4.tar", last modified: Sat May  6 13:10:21 2023, max compression
```

## Comparing `vasprocar-1.1.15.3.tar` & `vasprocar-1.1.15.4.tar`

### file list

```diff
@@ -1,95 +1,95 @@
-drwxrwxrwx   0        0        0        0 2023-05-04 15:52:38.965438 vasprocar-1.1.15.3/
--rw-rw-rw-   0        0        0    35822 2023-01-01 17:34:12.000000 vasprocar-1.1.15.3/LICENSE.txt
--rw-rw-rw-   0        0        0     2220 2023-05-04 15:52:38.965438 vasprocar-1.1.15.3/PKG-INFO
--rw-rw-rw-   0        0        0     1589 2023-01-17 12:07:08.000000 vasprocar-1.1.15.3/README.md
--rw-rw-rw-   0        0        0      167 2023-05-04 15:52:38.965438 vasprocar-1.1.15.3/setup.cfg
--rw-rw-rw-   0        0        0     1234 2023-05-04 15:52:24.000000 vasprocar-1.1.15.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-04 15:52:38.777938 vasprocar-1.1.15.3/vasprocar/
--rw-rw-rw-   0        0        0      360 2023-04-28 15:54:36.000000 vasprocar-1.1.15.3/vasprocar/BibTeX.dat
--rw-rw-rw-   0        0        0    47799 2022-03-23 22:06:30.000000 vasprocar-1.1.15.3/vasprocar/DOI.png
--rw-rw-rw-   0        0        0     3673 2023-04-28 15:54:42.000000 vasprocar-1.1.15.3/vasprocar/VASProcar.py
--rw-rw-rw-   0        0        0      201 2023-03-10 21:53:46.000000 vasprocar-1.1.15.3/vasprocar/__init__.py
--rw-rw-rw-   0        0        0     3673 2023-04-28 15:54:15.000000 vasprocar-1.1.15.3/vasprocar/__main__.py
-drwxrwxrwx   0        0        0        0 2023-05-04 15:52:38.840436 vasprocar-1.1.15.3/vasprocar/src/
-drwxrwxrwx   0        0        0        0 2023-05-04 15:52:38.887311 vasprocar-1.1.15.3/vasprocar/src/_VASP/
--rw-rw-rw-   0        0        0    18256 2023-04-26 12:33:54.000000 vasprocar-1.1.15.3/vasprocar/src/_VASP/_info.py
--rw-rw-rw-   0        0        0    13975 2023-02-01 18:32:31.000000 vasprocar-1.1.15.3/vasprocar/src/_VASP/_info_b.py
--rw-rw-rw-   0        0        0    15741 2023-02-05 19:46:41.000000 vasprocar-1.1.15.3/vasprocar/src/_VASP/_label.py
--rw-rw-rw-   0        0        0    31402 2023-04-16 15:59:10.000000 vasprocar-1.1.15.3/vasprocar/src/_VASP/_nscf.py
--rw-rw-rw-   0        0        0     9428 2023-02-07 22:29:38.000000 vasprocar-1.1.15.3/vasprocar/src/_VASP/_var_kpoints.py
--rw-rw-rw-   0        0        0    18445 2023-05-04 15:52:04.000000 vasprocar-1.1.15.3/vasprocar/src/_VASP/chgcar.py
--rw-rw-rw-   0        0        0    32155 2023-02-06 18:01:33.000000 vasprocar-1.1.15.3/vasprocar/src/_VASP/contribuicao.py
--rw-rw-rw-   0        0        0    14022 2023-02-07 16:02:48.000000 vasprocar-1.1.15.3/vasprocar/src/_VASP/dielectric_function.py
--rw-rw-rw-   0        0        0    26245 2023-02-07 16:02:09.000000 vasprocar-1.1.15.3/vasprocar/src/_VASP/dos_pdos_ldos.py
--rw-rw-rw-   0        0        0    28274 2023-02-07 16:01:48.000000 vasprocar-1.1.15.3/vasprocar/src/_VASP/dos_pdos_ldos_[polarizado].py
--rw-rw-rw-   0        0        0    24344 2023-04-01 21:06:45.000000 vasprocar-1.1.15.3/vasprocar/src/_VASP/kpoints_2D_3D.py
--rw-rw-rw-   0        0        0    15068 2023-05-04 13:02:49.000000 vasprocar-1.1.15.3/vasprocar/src/_VASP/parchg.py
--rw-rw-rw-   0        0        0     8140 2023-04-27 16:07:00.000000 vasprocar-1.1.15.3/vasprocar/src/_VASP/poscar_replace.py
--rw-rw-rw-   0        0        0    14843 2023-05-04 13:03:13.000000 vasprocar-1.1.15.3/vasprocar/src/_VASP/potencial.py
--rw-rw-rw-   0        0        0    15029 2023-05-04 13:03:33.000000 vasprocar-1.1.15.3/vasprocar/src/_VASP/wave_function.py
--rw-rw-rw-   0        0        0      626 2023-02-07 16:00:07.000000 vasprocar-1.1.15.3/vasprocar/src/_loop.py
--rw-rw-rw-   0        0        0    16703 2023-05-04 12:41:29.000000 vasprocar-1.1.15.3/vasprocar/src/_settings.py
--rw-rw-rw-   0        0        0     2897 2023-03-23 12:12:59.000000 vasprocar-1.1.15.3/vasprocar/src/_update.py
--rw-rw-rw-   0        0        0    17291 2023-02-07 15:59:42.000000 vasprocar-1.1.15.3/vasprocar/src/bandas_2D.py
--rw-rw-rw-   0        0        0    16604 2023-02-07 22:46:17.000000 vasprocar-1.1.15.3/vasprocar/src/bandas_3D.py
--rw-rw-rw-   0        0        0    14962 2023-02-07 22:46:24.000000 vasprocar-1.1.15.3/vasprocar/src/bandas_4D.py
--rw-rw-rw-   0        0        0     2100 2023-02-06 17:36:59.000000 vasprocar-1.1.15.3/vasprocar/src/correction_file.py
-drwxrwxrwx   0        0        0        0 2023-05-04 15:52:38.887311 vasprocar-1.1.15.3/vasprocar/src/etc/
--rw-rw-rw-   0        0        0      360 2023-04-28 15:54:36.000000 vasprocar-1.1.15.3/vasprocar/src/etc/BibTeX.dat
--rw-rw-rw-   0        0        0    47799 2022-03-23 22:06:30.000000 vasprocar-1.1.15.3/vasprocar/src/etc/DOI.png
--rw-rw-rw-   0        0        0   374410 2022-06-01 18:31:32.000000 vasprocar-1.1.15.3/vasprocar/src/etc/Greek_alphabet.jpg
--rw-rw-rw-   0        0        0    20078 2023-02-07 22:46:33.000000 vasprocar-1.1.15.3/vasprocar/src/fermi_surface.py
--rw-rw-rw-   0        0        0    16978 2023-04-27 19:31:37.000000 vasprocar-1.1.15.3/vasprocar/src/level_countour.py
-drwxrwxrwx   0        0        0        0 2023-05-04 15:52:38.934186 vasprocar-1.1.15.3/vasprocar/src/plot/
-drwxrwxrwx   0        0        0        0 2023-05-04 15:52:38.965438 vasprocar-1.1.15.3/vasprocar/src/plot/Grace/
--rw-rw-rw-   0        0        0     5204 2023-04-28 13:13:46.000000 vasprocar-1.1.15.3/vasprocar/src/plot/Grace/plot_bandas_2D.py
--rw-rw-rw-   0        0        0     4322 2023-05-04 14:16:22.000000 vasprocar-1.1.15.3/vasprocar/src/plot/Grace/plot_chgcar.py
--rw-rw-rw-   0        0        0     4960 2023-04-28 13:17:27.000000 vasprocar-1.1.15.3/vasprocar/src/plot/Grace/plot_dielectric_function.py
--rw-rw-rw-   0        0        0    13180 2023-04-28 13:22:43.000000 vasprocar-1.1.15.3/vasprocar/src/plot/Grace/plot_dos_pdos_ldos.py
--rw-rw-rw-   0        0        0    13278 2023-04-28 15:25:56.000000 vasprocar-1.1.15.3/vasprocar/src/plot/Grace/plot_dos_pdos_ldos_[polarizado].py
--rw-rw-rw-   0        0        0    11204 2023-04-28 15:27:51.000000 vasprocar-1.1.15.3/vasprocar/src/plot/Grace/plot_dos_pdos_ldos_[polarizado_delta].py
--rw-rw-rw-   0        0        0     3883 2023-05-03 16:43:07.000000 vasprocar-1.1.15.3/vasprocar/src/plot/Grace/plot_parchg.py
--rw-rw-rw-   0        0        0     3807 2023-04-28 15:30:54.000000 vasprocar-1.1.15.3/vasprocar/src/plot/Grace/plot_potencial.py
--rw-rw-rw-   0        0        0     6272 2023-04-28 15:35:06.000000 vasprocar-1.1.15.3/vasprocar/src/plot/Grace/plot_projecao_localizacao.py
--rw-rw-rw-   0        0        0    11195 2023-04-28 15:41:27.000000 vasprocar-1.1.15.3/vasprocar/src/plot/Grace/plot_projecao_orbitais.py
--rw-rw-rw-   0        0        0     6149 2023-04-28 15:45:01.000000 vasprocar-1.1.15.3/vasprocar/src/plot/Grace/plot_projecao_psi.py
--rw-rw-rw-   0        0        0    10949 2023-04-28 15:49:29.000000 vasprocar-1.1.15.3/vasprocar/src/plot/Grace/plot_projecao_spin.py
--rw-rw-rw-   0        0        0     4002 2023-04-28 15:51:35.000000 vasprocar-1.1.15.3/vasprocar/src/plot/Grace/plot_wave_function.py
--rw-rw-rw-   0        0        0     6459 2023-04-26 19:46:07.000000 vasprocar-1.1.15.3/vasprocar/src/plot/_plot_settings.py
--rw-rw-rw-   0        0        0     5859 2023-04-26 19:52:01.000000 vasprocar-1.1.15.3/vasprocar/src/plot/plot_bandas_2D.py
--rw-rw-rw-   0        0        0     5094 2023-04-27 16:26:15.000000 vasprocar-1.1.15.3/vasprocar/src/plot/plot_bandas_3D_matplotlib.py
--rw-rw-rw-   0        0        0     5789 2023-04-27 16:25:56.000000 vasprocar-1.1.15.3/vasprocar/src/plot/plot_bandas_3D_plotly.py
--rw-rw-rw-   0        0        0     5212 2023-04-27 16:30:27.000000 vasprocar-1.1.15.3/vasprocar/src/plot/plot_bandas_4D_plotly.py
--rw-rw-rw-   0        0        0     5022 2023-05-04 14:15:37.000000 vasprocar-1.1.15.3/vasprocar/src/plot/plot_chgcar.py
--rw-rw-rw-   0        0        0     4311 2023-04-27 16:32:25.000000 vasprocar-1.1.15.3/vasprocar/src/plot/plot_dielectric_function.py
--rw-rw-rw-   0        0        0    12937 2023-04-27 16:41:40.000000 vasprocar-1.1.15.3/vasprocar/src/plot/plot_dos_pdos_ldos.py
--rw-rw-rw-   0        0        0    34063 2023-04-27 16:53:46.000000 vasprocar-1.1.15.3/vasprocar/src/plot/plot_dos_pdos_ldos_[polarizado].py
--rw-rw-rw-   0        0        0     8368 2023-04-27 16:59:55.000000 vasprocar-1.1.15.3/vasprocar/src/plot/plot_fermi_surface.py
--rw-rw-rw-   0        0        0     6527 2023-04-27 17:03:00.000000 vasprocar-1.1.15.3/vasprocar/src/plot/plot_level_countour.py
--rw-rw-rw-   0        0        0     4693 2023-05-03 16:43:27.000000 vasprocar-1.1.15.3/vasprocar/src/plot/plot_parchg.py
--rw-rw-rw-   0        0        0     4693 2023-04-27 17:09:05.000000 vasprocar-1.1.15.3/vasprocar/src/plot/plot_potencial.py
--rw-rw-rw-   0        0        0    14161 2023-04-27 18:34:47.000000 vasprocar-1.1.15.3/vasprocar/src/plot/plot_projecao_localizacao.py
--rw-rw-rw-   0        0        0    26915 2023-04-27 18:40:15.000000 vasprocar-1.1.15.3/vasprocar/src/plot/plot_projecao_orbitais.py
--rw-rw-rw-   0        0        0    14283 2023-04-27 18:48:44.000000 vasprocar-1.1.15.3/vasprocar/src/plot/plot_projecao_psi.py
--rw-rw-rw-   0        0        0     7782 2023-04-27 18:53:12.000000 vasprocar-1.1.15.3/vasprocar/src/plot/plot_projecao_spin.py
--rw-rw-rw-   0        0        0    11866 2023-04-27 19:17:24.000000 vasprocar-1.1.15.3/vasprocar/src/plot/plot_spin_texture_2D.py
--rw-rw-rw-   0        0        0     9865 2023-04-27 19:05:41.000000 vasprocar-1.1.15.3/vasprocar/src/plot/plot_spin_texture_3D.py
--rw-rw-rw-   0        0        0     6287 2023-04-27 19:06:44.000000 vasprocar-1.1.15.3/vasprocar/src/plot/plot_spin_texture_4D.py
--rw-rw-rw-   0        0        0     6345 2023-04-27 19:08:37.000000 vasprocar-1.1.15.3/vasprocar/src/plot/plot_spin_texture_4D_[iso].py
--rw-rw-rw-   0        0        0    15772 2023-04-27 19:29:40.000000 vasprocar-1.1.15.3/vasprocar/src/plot/plot_spin_texture_contour.py
--rw-rw-rw-   0        0        0    17321 2023-04-27 19:30:01.000000 vasprocar-1.1.15.3/vasprocar/src/plot/plot_spin_texture_contour_video.py
--rw-rw-rw-   0        0        0     4600 2023-04-27 17:12:08.000000 vasprocar-1.1.15.3/vasprocar/src/plot/plot_wave_function.py
--rw-rw-rw-   0        0        0    26728 2023-02-09 23:53:36.000000 vasprocar-1.1.15.3/vasprocar/src/projecao_localizacao.py
--rw-rw-rw-   0        0        0    27714 2023-04-26 12:02:26.000000 vasprocar-1.1.15.3/vasprocar/src/projecao_orbitais.py
--rw-rw-rw-   0        0        0    33246 2023-02-14 20:05:13.000000 vasprocar-1.1.15.3/vasprocar/src/projecao_psi.py
--rw-rw-rw-   0        0        0    24325 2023-02-16 16:44:51.000000 vasprocar-1.1.15.3/vasprocar/src/projecao_spin.py
--rw-rw-rw-   0        0        0    22748 2023-02-14 20:11:56.000000 vasprocar-1.1.15.3/vasprocar/src/spin_texture.py
--rw-rw-rw-   0        0        0    22318 2023-04-27 19:32:03.000000 vasprocar-1.1.15.3/vasprocar/src/spin_texture_contour.py
--rw-rw-rw-   0        0        0    23728 2023-04-27 19:32:28.000000 vasprocar-1.1.15.3/vasprocar/src/spin_texture_contour_video.py
-drwxrwxrwx   0        0        0        0 2023-05-04 15:52:38.809200 vasprocar-1.1.15.3/vasprocar.egg-info/
--rw-rw-rw-   0        0        0     2220 2023-05-04 15:52:38.000000 vasprocar-1.1.15.3/vasprocar.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3134 2023-05-04 15:52:38.000000 vasprocar-1.1.15.3/vasprocar.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-04 15:52:38.000000 vasprocar-1.1.15.3/vasprocar.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-05-04 15:52:38.000000 vasprocar-1.1.15.3/vasprocar.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       91 2023-05-04 15:52:38.000000 vasprocar-1.1.15.3/vasprocar.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-04 15:52:38.000000 vasprocar-1.1.15.3/vasprocar.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-06 13:10:21.827152 vasprocar-1.1.15.4/
+-rw-rw-rw-   0        0        0    35822 2023-01-01 17:34:12.000000 vasprocar-1.1.15.4/LICENSE.txt
+-rw-rw-rw-   0        0        0     2220 2023-05-06 13:10:21.827152 vasprocar-1.1.15.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1589 2023-01-17 12:07:08.000000 vasprocar-1.1.15.4/README.md
+-rw-rw-rw-   0        0        0      167 2023-05-06 13:10:21.827152 vasprocar-1.1.15.4/setup.cfg
+-rw-rw-rw-   0        0        0     1234 2023-05-06 13:10:03.000000 vasprocar-1.1.15.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-06 13:10:21.655278 vasprocar-1.1.15.4/vasprocar/
+-rw-rw-rw-   0        0        0      360 2023-04-28 15:54:36.000000 vasprocar-1.1.15.4/vasprocar/BibTeX.dat
+-rw-rw-rw-   0        0        0    47799 2022-03-23 22:06:30.000000 vasprocar-1.1.15.4/vasprocar/DOI.png
+-rw-rw-rw-   0        0        0     3673 2023-04-28 15:54:42.000000 vasprocar-1.1.15.4/vasprocar/VASProcar.py
+-rw-rw-rw-   0        0        0      201 2023-03-10 21:53:46.000000 vasprocar-1.1.15.4/vasprocar/__init__.py
+-rw-rw-rw-   0        0        0     3673 2023-04-28 15:54:15.000000 vasprocar-1.1.15.4/vasprocar/__main__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 13:10:21.717776 vasprocar-1.1.15.4/vasprocar/src/
+drwxrwxrwx   0        0        0        0 2023-05-06 13:10:21.749028 vasprocar-1.1.15.4/vasprocar/src/_VASP/
+-rw-rw-rw-   0        0        0    18256 2023-04-26 12:33:54.000000 vasprocar-1.1.15.4/vasprocar/src/_VASP/_info.py
+-rw-rw-rw-   0        0        0    13975 2023-02-01 18:32:31.000000 vasprocar-1.1.15.4/vasprocar/src/_VASP/_info_b.py
+-rw-rw-rw-   0        0        0    15741 2023-02-05 19:46:41.000000 vasprocar-1.1.15.4/vasprocar/src/_VASP/_label.py
+-rw-rw-rw-   0        0        0    31402 2023-04-16 15:59:10.000000 vasprocar-1.1.15.4/vasprocar/src/_VASP/_nscf.py
+-rw-rw-rw-   0        0        0     9428 2023-02-07 22:29:38.000000 vasprocar-1.1.15.4/vasprocar/src/_VASP/_var_kpoints.py
+-rw-rw-rw-   0        0        0    20816 2023-05-06 13:08:43.000000 vasprocar-1.1.15.4/vasprocar/src/_VASP/chgcar.py
+-rw-rw-rw-   0        0        0    32155 2023-02-06 18:01:33.000000 vasprocar-1.1.15.4/vasprocar/src/_VASP/contribuicao.py
+-rw-rw-rw-   0        0        0    14022 2023-02-07 16:02:48.000000 vasprocar-1.1.15.4/vasprocar/src/_VASP/dielectric_function.py
+-rw-rw-rw-   0        0        0    26245 2023-02-07 16:02:09.000000 vasprocar-1.1.15.4/vasprocar/src/_VASP/dos_pdos_ldos.py
+-rw-rw-rw-   0        0        0    28274 2023-02-07 16:01:48.000000 vasprocar-1.1.15.4/vasprocar/src/_VASP/dos_pdos_ldos_[polarizado].py
+-rw-rw-rw-   0        0        0    24344 2023-04-01 21:06:45.000000 vasprocar-1.1.15.4/vasprocar/src/_VASP/kpoints_2D_3D.py
+-rw-rw-rw-   0        0        0    15068 2023-05-04 13:02:49.000000 vasprocar-1.1.15.4/vasprocar/src/_VASP/parchg.py
+-rw-rw-rw-   0        0        0     8140 2023-04-27 16:07:00.000000 vasprocar-1.1.15.4/vasprocar/src/_VASP/poscar_replace.py
+-rw-rw-rw-   0        0        0    14843 2023-05-04 13:03:13.000000 vasprocar-1.1.15.4/vasprocar/src/_VASP/potencial.py
+-rw-rw-rw-   0        0        0    15029 2023-05-04 13:03:33.000000 vasprocar-1.1.15.4/vasprocar/src/_VASP/wave_function.py
+-rw-rw-rw-   0        0        0      626 2023-02-07 16:00:07.000000 vasprocar-1.1.15.4/vasprocar/src/_loop.py
+-rw-rw-rw-   0        0        0    16703 2023-05-04 12:41:29.000000 vasprocar-1.1.15.4/vasprocar/src/_settings.py
+-rw-rw-rw-   0        0        0     2897 2023-03-23 12:12:59.000000 vasprocar-1.1.15.4/vasprocar/src/_update.py
+-rw-rw-rw-   0        0        0    17291 2023-02-07 15:59:42.000000 vasprocar-1.1.15.4/vasprocar/src/bandas_2D.py
+-rw-rw-rw-   0        0        0    16604 2023-02-07 22:46:17.000000 vasprocar-1.1.15.4/vasprocar/src/bandas_3D.py
+-rw-rw-rw-   0        0        0    14962 2023-02-07 22:46:24.000000 vasprocar-1.1.15.4/vasprocar/src/bandas_4D.py
+-rw-rw-rw-   0        0        0     2100 2023-02-06 17:36:59.000000 vasprocar-1.1.15.4/vasprocar/src/correction_file.py
+drwxrwxrwx   0        0        0        0 2023-05-06 13:10:21.749028 vasprocar-1.1.15.4/vasprocar/src/etc/
+-rw-rw-rw-   0        0        0      360 2023-04-28 15:54:36.000000 vasprocar-1.1.15.4/vasprocar/src/etc/BibTeX.dat
+-rw-rw-rw-   0        0        0    47799 2022-03-23 22:06:30.000000 vasprocar-1.1.15.4/vasprocar/src/etc/DOI.png
+-rw-rw-rw-   0        0        0   374410 2022-06-01 18:31:32.000000 vasprocar-1.1.15.4/vasprocar/src/etc/Greek_alphabet.jpg
+-rw-rw-rw-   0        0        0    20078 2023-02-07 22:46:33.000000 vasprocar-1.1.15.4/vasprocar/src/fermi_surface.py
+-rw-rw-rw-   0        0        0    16978 2023-04-27 19:31:37.000000 vasprocar-1.1.15.4/vasprocar/src/level_countour.py
+drwxrwxrwx   0        0        0        0 2023-05-06 13:10:21.795903 vasprocar-1.1.15.4/vasprocar/src/plot/
+drwxrwxrwx   0        0        0        0 2023-05-06 13:10:21.827152 vasprocar-1.1.15.4/vasprocar/src/plot/Grace/
+-rw-rw-rw-   0        0        0     5204 2023-04-28 13:13:46.000000 vasprocar-1.1.15.4/vasprocar/src/plot/Grace/plot_bandas_2D.py
+-rw-rw-rw-   0        0        0     4322 2023-05-04 14:16:22.000000 vasprocar-1.1.15.4/vasprocar/src/plot/Grace/plot_chgcar.py
+-rw-rw-rw-   0        0        0     4960 2023-04-28 13:17:27.000000 vasprocar-1.1.15.4/vasprocar/src/plot/Grace/plot_dielectric_function.py
+-rw-rw-rw-   0        0        0    13180 2023-04-28 13:22:43.000000 vasprocar-1.1.15.4/vasprocar/src/plot/Grace/plot_dos_pdos_ldos.py
+-rw-rw-rw-   0        0        0    13278 2023-04-28 15:25:56.000000 vasprocar-1.1.15.4/vasprocar/src/plot/Grace/plot_dos_pdos_ldos_[polarizado].py
+-rw-rw-rw-   0        0        0    11204 2023-04-28 15:27:51.000000 vasprocar-1.1.15.4/vasprocar/src/plot/Grace/plot_dos_pdos_ldos_[polarizado_delta].py
+-rw-rw-rw-   0        0        0     3883 2023-05-03 16:43:07.000000 vasprocar-1.1.15.4/vasprocar/src/plot/Grace/plot_parchg.py
+-rw-rw-rw-   0        0        0     3807 2023-04-28 15:30:54.000000 vasprocar-1.1.15.4/vasprocar/src/plot/Grace/plot_potencial.py
+-rw-rw-rw-   0        0        0     6272 2023-04-28 15:35:06.000000 vasprocar-1.1.15.4/vasprocar/src/plot/Grace/plot_projecao_localizacao.py
+-rw-rw-rw-   0        0        0    11195 2023-04-28 15:41:27.000000 vasprocar-1.1.15.4/vasprocar/src/plot/Grace/plot_projecao_orbitais.py
+-rw-rw-rw-   0        0        0     6149 2023-04-28 15:45:01.000000 vasprocar-1.1.15.4/vasprocar/src/plot/Grace/plot_projecao_psi.py
+-rw-rw-rw-   0        0        0    10949 2023-04-28 15:49:29.000000 vasprocar-1.1.15.4/vasprocar/src/plot/Grace/plot_projecao_spin.py
+-rw-rw-rw-   0        0        0     4002 2023-04-28 15:51:35.000000 vasprocar-1.1.15.4/vasprocar/src/plot/Grace/plot_wave_function.py
+-rw-rw-rw-   0        0        0     6459 2023-04-26 19:46:07.000000 vasprocar-1.1.15.4/vasprocar/src/plot/_plot_settings.py
+-rw-rw-rw-   0        0        0     5859 2023-04-26 19:52:01.000000 vasprocar-1.1.15.4/vasprocar/src/plot/plot_bandas_2D.py
+-rw-rw-rw-   0        0        0     5094 2023-04-27 16:26:15.000000 vasprocar-1.1.15.4/vasprocar/src/plot/plot_bandas_3D_matplotlib.py
+-rw-rw-rw-   0        0        0     5789 2023-04-27 16:25:56.000000 vasprocar-1.1.15.4/vasprocar/src/plot/plot_bandas_3D_plotly.py
+-rw-rw-rw-   0        0        0     5212 2023-04-27 16:30:27.000000 vasprocar-1.1.15.4/vasprocar/src/plot/plot_bandas_4D_plotly.py
+-rw-rw-rw-   0        0        0     5022 2023-05-04 14:15:37.000000 vasprocar-1.1.15.4/vasprocar/src/plot/plot_chgcar.py
+-rw-rw-rw-   0        0        0     4311 2023-04-27 16:32:25.000000 vasprocar-1.1.15.4/vasprocar/src/plot/plot_dielectric_function.py
+-rw-rw-rw-   0        0        0    12937 2023-04-27 16:41:40.000000 vasprocar-1.1.15.4/vasprocar/src/plot/plot_dos_pdos_ldos.py
+-rw-rw-rw-   0        0        0    34063 2023-04-27 16:53:46.000000 vasprocar-1.1.15.4/vasprocar/src/plot/plot_dos_pdos_ldos_[polarizado].py
+-rw-rw-rw-   0        0        0     8368 2023-04-27 16:59:55.000000 vasprocar-1.1.15.4/vasprocar/src/plot/plot_fermi_surface.py
+-rw-rw-rw-   0        0        0     6527 2023-04-27 17:03:00.000000 vasprocar-1.1.15.4/vasprocar/src/plot/plot_level_countour.py
+-rw-rw-rw-   0        0        0     4693 2023-05-03 16:43:27.000000 vasprocar-1.1.15.4/vasprocar/src/plot/plot_parchg.py
+-rw-rw-rw-   0        0        0     4693 2023-04-27 17:09:05.000000 vasprocar-1.1.15.4/vasprocar/src/plot/plot_potencial.py
+-rw-rw-rw-   0        0        0    14161 2023-04-27 18:34:47.000000 vasprocar-1.1.15.4/vasprocar/src/plot/plot_projecao_localizacao.py
+-rw-rw-rw-   0        0        0    26915 2023-04-27 18:40:15.000000 vasprocar-1.1.15.4/vasprocar/src/plot/plot_projecao_orbitais.py
+-rw-rw-rw-   0        0        0    14283 2023-04-27 18:48:44.000000 vasprocar-1.1.15.4/vasprocar/src/plot/plot_projecao_psi.py
+-rw-rw-rw-   0        0        0     7782 2023-04-27 18:53:12.000000 vasprocar-1.1.15.4/vasprocar/src/plot/plot_projecao_spin.py
+-rw-rw-rw-   0        0        0    11866 2023-04-27 19:17:24.000000 vasprocar-1.1.15.4/vasprocar/src/plot/plot_spin_texture_2D.py
+-rw-rw-rw-   0        0        0     9865 2023-04-27 19:05:41.000000 vasprocar-1.1.15.4/vasprocar/src/plot/plot_spin_texture_3D.py
+-rw-rw-rw-   0        0        0     6287 2023-04-27 19:06:44.000000 vasprocar-1.1.15.4/vasprocar/src/plot/plot_spin_texture_4D.py
+-rw-rw-rw-   0        0        0     6345 2023-04-27 19:08:37.000000 vasprocar-1.1.15.4/vasprocar/src/plot/plot_spin_texture_4D_[iso].py
+-rw-rw-rw-   0        0        0    15772 2023-04-27 19:29:40.000000 vasprocar-1.1.15.4/vasprocar/src/plot/plot_spin_texture_contour.py
+-rw-rw-rw-   0        0        0    17321 2023-04-27 19:30:01.000000 vasprocar-1.1.15.4/vasprocar/src/plot/plot_spin_texture_contour_video.py
+-rw-rw-rw-   0        0        0     4600 2023-04-27 17:12:08.000000 vasprocar-1.1.15.4/vasprocar/src/plot/plot_wave_function.py
+-rw-rw-rw-   0        0        0    26728 2023-02-09 23:53:36.000000 vasprocar-1.1.15.4/vasprocar/src/projecao_localizacao.py
+-rw-rw-rw-   0        0        0    27714 2023-04-26 12:02:26.000000 vasprocar-1.1.15.4/vasprocar/src/projecao_orbitais.py
+-rw-rw-rw-   0        0        0    33246 2023-02-14 20:05:13.000000 vasprocar-1.1.15.4/vasprocar/src/projecao_psi.py
+-rw-rw-rw-   0        0        0    24325 2023-02-16 16:44:51.000000 vasprocar-1.1.15.4/vasprocar/src/projecao_spin.py
+-rw-rw-rw-   0        0        0    22748 2023-02-14 20:11:56.000000 vasprocar-1.1.15.4/vasprocar/src/spin_texture.py
+-rw-rw-rw-   0        0        0    22318 2023-04-27 19:32:03.000000 vasprocar-1.1.15.4/vasprocar/src/spin_texture_contour.py
+-rw-rw-rw-   0        0        0    23728 2023-04-27 19:32:28.000000 vasprocar-1.1.15.4/vasprocar/src/spin_texture_contour_video.py
+drwxrwxrwx   0        0        0        0 2023-05-06 13:10:21.686530 vasprocar-1.1.15.4/vasprocar.egg-info/
+-rw-rw-rw-   0        0        0     2220 2023-05-06 13:10:21.000000 vasprocar-1.1.15.4/vasprocar.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3134 2023-05-06 13:10:21.000000 vasprocar-1.1.15.4/vasprocar.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 13:10:21.000000 vasprocar-1.1.15.4/vasprocar.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-05-06 13:10:21.000000 vasprocar-1.1.15.4/vasprocar.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       91 2023-05-06 13:10:21.000000 vasprocar-1.1.15.4/vasprocar.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-06 13:10:21.000000 vasprocar-1.1.15.4/vasprocar.egg-info/top_level.txt
```

### Comparing `vasprocar-1.1.15.3/LICENSE.txt` & `vasprocar-1.1.15.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.3/PKG-INFO` & `vasprocar-1.1.15.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vasprocar
-Version: 1.1.15.3
+Version: 1.1.15.4
 Summary: VASProcar is an open-source package written in the Python 3 programming language, which aims to provide an intuitive tool for the post-processing of the output files produced by the DFT VASP code, through an interactive user interface.
 Home-page: https://doi.org/10.5281/zenodo.6343960
 Download-URL: https://doi.org/10.5281/zenodo.6343960
 Author: Augusto de Lelis Araujo and Renan da Paixao Maciel
 Author-email: augusto-lelis@outlook.com, renan.maciel@physics.uu.se
 License: GNU GPLv3
 Description-Content-Type: text/markdown
```

### Comparing `vasprocar-1.1.15.3/README.md` & `vasprocar-1.1.15.4/README.md`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.3/setup.py` & `vasprocar-1.1.15.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 import json
 from pathlib import Path
 from typing import Optional
 
 setup(
     name = "vasprocar",
-    version = "1.1.15.3",
+    version = "1.1.15.4",
     entry_points={'console_scripts': ['vasprocar = vasprocar:main']},
     description = "VASProcar is an open-source package written in the Python 3 programming language, which aims to provide an intuitive tool for the post-processing of the output files produced by the DFT VASP code, through an interactive user interface.",
     author = "Augusto de Lelis Araujo and Renan da Paixao Maciel", 
     author_email = "augusto-lelis@outlook.com, renan.maciel@physics.uu.se",
     url = "https://doi.org/10.5281/zenodo.6343960",
     download_url = "https://doi.org/10.5281/zenodo.6343960",
     license = "GNU GPLv3",
```

### Comparing `vasprocar-1.1.15.3/vasprocar/DOI.png` & `vasprocar-1.1.15.4/vasprocar/DOI.png`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.3/vasprocar/VASProcar.py` & `vasprocar-1.1.15.4/vasprocar/VASProcar.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.3/vasprocar/__main__.py` & `vasprocar-1.1.15.4/vasprocar/__main__.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.3/vasprocar/src/_VASP/_info.py` & `vasprocar-1.1.15.4/vasprocar/src/_VASP/_info.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.3/vasprocar/src/_VASP/_info_b.py` & `vasprocar-1.1.15.4/vasprocar/src/_VASP/_info_b.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.3/vasprocar/src/_VASP/_label.py` & `vasprocar-1.1.15.4/vasprocar/src/_VASP/_label.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.3/vasprocar/src/_VASP/_nscf.py` & `vasprocar-1.1.15.4/vasprocar/src/_VASP/_nscf.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.3/vasprocar/src/_VASP/_var_kpoints.py` & `vasprocar-1.1.15.4/vasprocar/src/_VASP/_var_kpoints.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.3/vasprocar/src/_VASP/chgcar.py` & `vasprocar-1.1.15.4/vasprocar/src/_VASP/chgcar.py`

 * *Files 10% similar despite different names*

```diff
@@ -47,20 +47,25 @@
 plot_type = input (" "); plot_type = int(plot_type)
 print (" ")
 
 if (plot_type != 1):
    nfiles = 1
 
 if (plot_type == 1):
+
    print ("##############################################################")
    print ("How many CHGCAR files do you want to analyze:                 ")
    print ("##############################################################") 
    nfiles = input (" "); nfiles = int(nfiles)
    print (" ")
 
+   #----------------------------------------------------------------------
+   new_chgcar = open(dir_files + '/' + 'CHGCAR_Charge_Transfer.vasp', 'w')
+   #----------------------------------------------------------------------
+
 names = [0]*nfiles
 
 for i in range(nfiles):
     if (i == 0):
        print ("##############################################################")
        print ("Enter the name of the main CHGCAR file:                       ")
        print ("##############################################################") 
@@ -69,14 +74,26 @@
     if (i != 0):
        print ("##############################################################")
        print ("Enter the name of the CHGCAR file to be subtracted:           ")
        print ("##############################################################") 
        names[i] = input (" "); names[i] = str(names[i])
        print (" ")
 
+if (plot_type == 1):
+   print ("==============================================================")
+   print ("Calculation to be performed:                                  ")
+   print ("--------------------------------------------------------------") 
+   for i in range(nfiles):
+       if (i == 0):
+          print (f'+ ({names[i]})')
+       if (i != 0):
+          print (f'- ({names[i]}) ')
+   print ("==============================================================")
+   print (" ")
+
 if (escolha == -1): 
    print ("##############################################################")
    print ("Choose the Plot's x-axis (abscissa) dimension: ===============")
    print ("[1] to Angs. (Default) =======================================")
    print ("[2] to nm. ===================================================")
    print ("##############################################################") 
    Dimensao = input (" "); Dimensao = int(Dimensao)
@@ -98,14 +115,18 @@
    destaque = 0
 
 #----------------------------------------------------------------------
 # Obtaining the results from the files CHGCAR -------------------------
 #----------------------------------------------------------------------
 
 for m in range(nfiles):
+
+    if (m == 0): fator = +1
+    if (m != 0): fator = -1
+
     name = str(names[m])
     print (".........................................................")
     print (f'Readind {name} ')
     print ("please, wait a moment ...................................")
     print (".........................................................")
     print (" ")
 
@@ -123,68 +144,92 @@
         print ("--------------------------------------------------------------")
         confirmacao = input (" "); confirmacao = str(confirmacao)
 
     #-----------------------------------------
     chgcar = open(dir_files + '/' + name, 'r')
     #-----------------------------------------
 
-    VTemp = chgcar.readline()
+    VTemp = chgcar.readline()  
+    if (plot_type == 1 and m == 0): new_chgcar.write(f'{VTemp}') 
 
     VTemp = chgcar.readline()
+    if (plot_type == 1 and m == 0): new_chgcar.write(f'{VTemp}') 
+
     Parametro = float(VTemp)
 
-    VTemp = chgcar.readline().split()
+    VTemp = chgcar.readline()
+    if (plot_type == 1 and m == 0): new_chgcar.write(f'{VTemp}') 
+
+    VTemp = VTemp.split()
     A1x = float(VTemp[0]); A1y = float(VTemp[1]); A1z = float(VTemp[2])
 
-    VTemp = chgcar.readline().split()
+    VTemp = chgcar.readline()
+    if (plot_type == 1 and m == 0): new_chgcar.write(f'{VTemp}') 
+    
+    VTemp = VTemp.split()
     A2x = float(VTemp[0]); A2y = float(VTemp[1]); A2z = float(VTemp[2])
 
-    VTemp = chgcar.readline().split()
+    VTemp = chgcar.readline()
+    if (plot_type == 1 and m == 0): new_chgcar.write(f'{VTemp}') 
+
+    VTemp = VTemp.split()
     A3x = float(VTemp[0]); A3y = float(VTemp[1]); A3z = float(VTemp[2])
 
     VTemp = chgcar.readline()
+    if (plot_type == 1 and m == 0): new_chgcar.write(f'{VTemp}') 
+   
+    VTemp = chgcar.readline()
+    if (plot_type == 1 and m == 0): new_chgcar.write(f'{VTemp}') 
+
+    VTemp = VTemp.split()
 
     ni = 0
-    VTemp = chgcar.readline().split()
     passo = len(VTemp)
     for i in range(passo):
         ni = ni + int(VTemp[i])
 
     VTemp = chgcar.readline()
+    if (plot_type == 1 and m == 0): new_chgcar.write(f'{VTemp}') 
 
     Ax = [A1x*Parametro, A2x*Parametro, A3x*Parametro]
     Ay = [A1y*Parametro, A2y*Parametro, A3y*Parametro]
     Az = [A1z*Parametro, A2z*Parametro, A3z*Parametro]
 
     ion_x = [0]*(ni)
     ion_y = [0]*(ni)
     ion_z = [0]*(ni)
 
     for i in range (ni):
-        VTemp = chgcar.readline().split()
+        VTemp = chgcar.readline()
+        if (plot_type == 1 and m == 0): new_chgcar.write(f'{VTemp}') 
+        VTemp = VTemp.split()
         #---------------------------------------------------------------
         m1 = float(VTemp[0]); m2 = float(VTemp[1]); m3 = float(VTemp[2])
         #---------------------------------------------------------------
         ion_x[i] = ((m1*A1x) + (m2*A2x) + (m3*A3x))*Parametro; ion_x[i] = ion_x[i] - min(Ax)
         ion_y[i] = ((m1*A1y) + (m2*A2y) + (m3*A3y))*Parametro; ion_y[i] = ion_y[i] - min(Ay)
         ion_z[i] = ((m1*A1z) + (m2*A2z) + (m3*A3z))*Parametro; ion_z[i] = ion_z[i] - min(Az)
     
     VTemp = chgcar.readline()
+    if (plot_type == 1 and m == 0): new_chgcar.write(f'{VTemp}') 
+
     VTemp = chgcar.readline()
+    if (plot_type == 1 and m == 0): new_chgcar.write(f'{VTemp}') 
 
     palavra = str(VTemp)
 
     VTemp = VTemp.split()
 
     Grid_x = int(VTemp[0])
     Grid_y = int(VTemp[1])
     Grid_z = int(VTemp[2])
     GRID = Grid_x*Grid_y*Grid_z
     
     V_local = [0]*(GRID)
+    if (plot_type == 1 and m == 0): new_V_local = [0]*(GRID)
 
     if (m == 0):
        Vx = [0.0]*(Grid_x)
        Vy = [0.0]*(Grid_y)
        Vz = [0.0]*(Grid_z)
 
     passo1 = (GRID/5)
@@ -204,27 +249,33 @@
             if palavra in line: 
                break    
     #---------------------------------------------------------
 
     for i in range (passo1):
 
         VTemp = chgcar.readline()
-        if (i == 0 or i == 1):
-           print(VTemp)
         #-----------------------------------------------------
         for k in range(10):
             VTemp = VTemp.replace(str(k) + '-', str(k) + 'E-')
             VTemp = VTemp.replace(str(k) + '+', str(k) + 'E+')
         VTemp = VTemp.split()    
         #----------------------------------------------------- 
 
         if (i < (passo1-1)):
-           for j in range(5): V_local[((i)*5) + j] = float(VTemp[j])
+           for j in range(5):
+               V_local[((i)*5) + j] = float(VTemp[j])
+           if (plot_type == 1):
+              for j in range(5):
+                  new_V_local[((i)*5) + j] = new_V_local[((i)*5) + j] + V_local[((i)*5) + j]*fator
         if (i == (passo1-1)):
-           for j in range(passo2): V_local[((i)*5) + j] = float(VTemp[j])
+           for j in range(passo2):
+               V_local[((i)*5) + j] = float(VTemp[j])
+           if (plot_type == 1):
+              for j in range(passo2):
+                  new_V_local[((i)*5) + j] = new_V_local[((i)*5) + j] + V_local[((i)*5) + j]*fator
 
     #-------------
     chgcar.close()
     #-------------
   
     #-------------------------------------------------------------------------------------
 
@@ -242,25 +293,54 @@
     escala_y = 1.0/float(GRID); Y = [0]*(Grid_y)
     escala_z = 1.0/float(GRID); Z = [0]*(Grid_z)
     
     #----------------------------------------------------------------------------
     # Analyzing the data: Obtaining the average Charge value in a given direction
     #----------------------------------------------------------------------------
 
-    if (m == 0): fator = +1
-    if (m != 0): fator = -1
-
     for i in range (Grid_x):
         for j in range (Grid_y):  
             for k in range (Grid_z):                          
                 indice = i + (j + k*Grid_y)*Grid_x
                 Vx[i] = Vx[i] + V_local[indice]*escala_x*fator
                 Vy[j] = Vy[j] + V_local[indice]*escala_y*fator
                 Vz[k] = Vz[k] + V_local[indice]*escala_z*fator
 
+
+
+
+
+
+
+
+
+if (plot_type == 1): 
+
+   for i in range (passo1):
+
+       if (i < (passo1-1)):
+          for j in range(5):
+              new_chgcar.write(f'{new_V_local[((i)*5) + j]} ')
+       if (i == (passo1-1)):
+          for j in range(passo2):
+              new_chgcar.write(f'{new_V_local[((i)*5) + j]} ')
+       new_chgcar.write(f' \n')
+   new_chgcar.close()
+
+
+
+
+
+
+
+
+
+
+
+
 #=======================================================================
 # Saving data to plot the Charge =======================================
 #=======================================================================            
 
 #---------------------------------------------------------------------------------
 densidade = open(dir_files + '/output/Charge/Charge_X.dat', "w")
 #---------------------------------------------------------------------------------
```

### Comparing `vasprocar-1.1.15.3/vasprocar/src/_VASP/contribuicao.py` & `vasprocar-1.1.15.4/vasprocar/src/_VASP/contribuicao.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.3/vasprocar/src/_VASP/dielectric_function.py` & `vasprocar-1.1.15.4/vasprocar/src/_VASP/dielectric_function.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.3/vasprocar/src/_VASP/dos_pdos_ldos.py` & `vasprocar-1.1.15.4/vasprocar/src/_VASP/dos_pdos_ldos.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.3/vasprocar/src/_VASP/dos_pdos_ldos_[polarizado].py` & `vasprocar-1.1.15.4/vasprocar/src/_VASP/dos_pdos_ldos_[polarizado].py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.3/vasprocar/src/_VASP/kpoints_2D_3D.py` & `vasprocar-1.1.15.4/vasprocar/src/_VASP/kpoints_2D_3D.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.3/vasprocar/src/_VASP/parchg.py` & `vasprocar-1.1.15.4/vasprocar/src/_VASP/parchg.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.3/vasprocar/src/_VASP/poscar_replace.py` & `vasprocar-1.1.15.4/vasprocar/src/_VASP/poscar_replace.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.3/vasprocar/src/_VASP/potencial.py` & `vasprocar-1.1.15.4/vasprocar/src/_VASP/potencial.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.3/vasprocar/src/_VASP/wave_function.py` & `vasprocar-1.1.15.4/vasprocar/src/_VASP/wave_function.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.3/vasprocar/src/_loop.py` & `vasprocar-1.1.15.4/vasprocar/src/_loop.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.3/vasprocar/src/_settings.py` & `vasprocar-1.1.15.4/vasprocar/src/_settings.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.3/vasprocar/src/_update.py` & `vasprocar-1.1.15.4/vasprocar/src/_update.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.3/vasprocar/src/bandas_2D.py` & `vasprocar-1.1.15.4/vasprocar/src/bandas_2D.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.3/vasprocar/src/bandas_3D.py` & `vasprocar-1.1.15.4/vasprocar/src/bandas_3D.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.3/vasprocar/src/bandas_4D.py` & `vasprocar-1.1.15.4/vasprocar/src/bandas_4D.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.3/vasprocar/src/correction_file.py` & `vasprocar-1.1.15.4/vasprocar/src/correction_file.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.3/vasprocar/src/etc/DOI.png` & `vasprocar-1.1.15.4/vasprocar/src/etc/DOI.png`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.3/vasprocar/src/etc/Greek_alphabet.jpg` & `vasprocar-1.1.15.4/vasprocar/src/etc/Greek_alphabet.jpg`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.3/vasprocar/src/fermi_surface.py` & `vasprocar-1.1.15.4/vasprocar/src/fermi_surface.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.3/vasprocar/src/level_countour.py` & `vasprocar-1.1.15.4/vasprocar/src/level_countour.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.3/vasprocar/src/plot/Grace/plot_bandas_2D.py` & `vasprocar-1.1.15.4/vasprocar/src/plot/Grace/plot_bandas_2D.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.3/vasprocar/src/plot/Grace/plot_chgcar.py` & `vasprocar-1.1.15.4/vasprocar/src/plot/Grace/plot_chgcar.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.3/vasprocar/src/plot/Grace/plot_dielectric_function.py` & `vasprocar-1.1.15.4/vasprocar/src/plot/Grace/plot_dielectric_function.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.3/vasprocar/src/plot/Grace/plot_dos_pdos_ldos.py` & `vasprocar-1.1.15.4/vasprocar/src/plot/Grace/plot_dos_pdos_ldos.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.3/vasprocar/src/plot/Grace/plot_dos_pdos_ldos_[polarizado].py` & `vasprocar-1.1.15.4/vasprocar/src/plot/Grace/plot_dos_pdos_ldos_[polarizado].py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.3/vasprocar/src/plot/Grace/plot_dos_pdos_ldos_[polarizado_delta].py` & `vasprocar-1.1.15.4/vasprocar/src/plot/Grace/plot_dos_pdos_ldos_[polarizado_delta].py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.3/vasprocar/src/plot/Grace/plot_parchg.py` & `vasprocar-1.1.15.4/vasprocar/src/plot/Grace/plot_parchg.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.3/vasprocar/src/plot/Grace/plot_potencial.py` & `vasprocar-1.1.15.4/vasprocar/src/plot/Grace/plot_potencial.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.3/vasprocar/src/plot/Grace/plot_projecao_localizacao.py` & `vasprocar-1.1.15.4/vasprocar/src/plot/Grace/plot_projecao_localizacao.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.3/vasprocar/src/plot/Grace/plot_projecao_orbitais.py` & `vasprocar-1.1.15.4/vasprocar/src/plot/Grace/plot_projecao_orbitais.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.3/vasprocar/src/plot/Grace/plot_projecao_psi.py` & `vasprocar-1.1.15.4/vasprocar/src/plot/Grace/plot_projecao_psi.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.3/vasprocar/src/plot/Grace/plot_projecao_spin.py` & `vasprocar-1.1.15.4/vasprocar/src/plot/Grace/plot_projecao_spin.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.3/vasprocar/src/plot/Grace/plot_wave_function.py` & `vasprocar-1.1.15.4/vasprocar/src/plot/Grace/plot_wave_function.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.3/vasprocar/src/plot/_plot_settings.py` & `vasprocar-1.1.15.4/vasprocar/src/plot/_plot_settings.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.3/vasprocar/src/plot/plot_bandas_2D.py` & `vasprocar-1.1.15.4/vasprocar/src/plot/plot_bandas_2D.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.3/vasprocar/src/plot/plot_bandas_3D_matplotlib.py` & `vasprocar-1.1.15.4/vasprocar/src/plot/plot_bandas_3D_matplotlib.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.3/vasprocar/src/plot/plot_bandas_3D_plotly.py` & `vasprocar-1.1.15.4/vasprocar/src/plot/plot_bandas_3D_plotly.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.3/vasprocar/src/plot/plot_bandas_4D_plotly.py` & `vasprocar-1.1.15.4/vasprocar/src/plot/plot_bandas_4D_plotly.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.3/vasprocar/src/plot/plot_chgcar.py` & `vasprocar-1.1.15.4/vasprocar/src/plot/plot_chgcar.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.3/vasprocar/src/plot/plot_dielectric_function.py` & `vasprocar-1.1.15.4/vasprocar/src/plot/plot_dielectric_function.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.3/vasprocar/src/plot/plot_dos_pdos_ldos.py` & `vasprocar-1.1.15.4/vasprocar/src/plot/plot_dos_pdos_ldos.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.3/vasprocar/src/plot/plot_dos_pdos_ldos_[polarizado].py` & `vasprocar-1.1.15.4/vasprocar/src/plot/plot_dos_pdos_ldos_[polarizado].py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.3/vasprocar/src/plot/plot_fermi_surface.py` & `vasprocar-1.1.15.4/vasprocar/src/plot/plot_fermi_surface.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.3/vasprocar/src/plot/plot_level_countour.py` & `vasprocar-1.1.15.4/vasprocar/src/plot/plot_level_countour.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.3/vasprocar/src/plot/plot_parchg.py` & `vasprocar-1.1.15.4/vasprocar/src/plot/plot_parchg.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.3/vasprocar/src/plot/plot_potencial.py` & `vasprocar-1.1.15.4/vasprocar/src/plot/plot_potencial.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.3/vasprocar/src/plot/plot_projecao_localizacao.py` & `vasprocar-1.1.15.4/vasprocar/src/plot/plot_projecao_localizacao.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.3/vasprocar/src/plot/plot_projecao_orbitais.py` & `vasprocar-1.1.15.4/vasprocar/src/plot/plot_projecao_orbitais.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.3/vasprocar/src/plot/plot_projecao_psi.py` & `vasprocar-1.1.15.4/vasprocar/src/plot/plot_projecao_psi.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.3/vasprocar/src/plot/plot_projecao_spin.py` & `vasprocar-1.1.15.4/vasprocar/src/plot/plot_projecao_spin.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.3/vasprocar/src/plot/plot_spin_texture_2D.py` & `vasprocar-1.1.15.4/vasprocar/src/plot/plot_spin_texture_2D.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.3/vasprocar/src/plot/plot_spin_texture_3D.py` & `vasprocar-1.1.15.4/vasprocar/src/plot/plot_spin_texture_3D.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.3/vasprocar/src/plot/plot_spin_texture_4D.py` & `vasprocar-1.1.15.4/vasprocar/src/plot/plot_spin_texture_4D.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.3/vasprocar/src/plot/plot_spin_texture_4D_[iso].py` & `vasprocar-1.1.15.4/vasprocar/src/plot/plot_spin_texture_4D_[iso].py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.3/vasprocar/src/plot/plot_spin_texture_contour.py` & `vasprocar-1.1.15.4/vasprocar/src/plot/plot_spin_texture_contour.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.3/vasprocar/src/plot/plot_spin_texture_contour_video.py` & `vasprocar-1.1.15.4/vasprocar/src/plot/plot_spin_texture_contour_video.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.3/vasprocar/src/plot/plot_wave_function.py` & `vasprocar-1.1.15.4/vasprocar/src/plot/plot_wave_function.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.3/vasprocar/src/projecao_localizacao.py` & `vasprocar-1.1.15.4/vasprocar/src/projecao_localizacao.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.3/vasprocar/src/projecao_orbitais.py` & `vasprocar-1.1.15.4/vasprocar/src/projecao_orbitais.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.3/vasprocar/src/projecao_psi.py` & `vasprocar-1.1.15.4/vasprocar/src/projecao_psi.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.3/vasprocar/src/projecao_spin.py` & `vasprocar-1.1.15.4/vasprocar/src/projecao_spin.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.3/vasprocar/src/spin_texture.py` & `vasprocar-1.1.15.4/vasprocar/src/spin_texture.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.3/vasprocar/src/spin_texture_contour.py` & `vasprocar-1.1.15.4/vasprocar/src/spin_texture_contour.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.3/vasprocar/src/spin_texture_contour_video.py` & `vasprocar-1.1.15.4/vasprocar/src/spin_texture_contour_video.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.3/vasprocar.egg-info/PKG-INFO` & `vasprocar-1.1.15.4/vasprocar.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vasprocar
-Version: 1.1.15.3
+Version: 1.1.15.4
 Summary: VASProcar is an open-source package written in the Python 3 programming language, which aims to provide an intuitive tool for the post-processing of the output files produced by the DFT VASP code, through an interactive user interface.
 Home-page: https://doi.org/10.5281/zenodo.6343960
 Download-URL: https://doi.org/10.5281/zenodo.6343960
 Author: Augusto de Lelis Araujo and Renan da Paixao Maciel
 Author-email: augusto-lelis@outlook.com, renan.maciel@physics.uu.se
 License: GNU GPLv3
 Description-Content-Type: text/markdown
```

### Comparing `vasprocar-1.1.15.3/vasprocar.egg-info/SOURCES.txt` & `vasprocar-1.1.15.4/vasprocar.egg-info/SOURCES.txt`

 * *Files identical despite different names*

