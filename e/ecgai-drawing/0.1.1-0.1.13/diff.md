# Comparing `tmp/ecgai-drawing-0.1.1.tar.gz` & `tmp/ecgai_drawing-0.1.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecgai-drawing-0.1.1.tar", max compression
+gzip compressed data, was "ecgai_drawing-0.1.13.tar", max compression
```

## Comparing `ecgai-drawing-0.1.1.tar` & `ecgai_drawing-0.1.13.tar`

### file list

```diff
@@ -1,4 +1,17 @@
--rw-r--r--   0        0        0      344 2022-08-17 10:05:10.288438 ecgai-drawing-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       78 2022-08-17 10:05:10.288438 ecgai-drawing-0.1.1/src/ecgai_drawing/__init__.py
--rw-r--r--   0        0        0      652 2022-08-17 10:05:19.677771 ecgai-drawing-0.1.1/setup.py
--rw-r--r--   0        0        0      284 2022-08-17 10:05:19.677992 ecgai-drawing-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      993 2023-05-06 16:19:51.225548 ecgai_drawing-0.1.13/pyproject.toml
+-rw-r--r--   0        0        0       78 2023-05-06 16:19:51.225548 ecgai_drawing-0.1.13/src/ecgai_drawing/__init__.py
+-rw-r--r--   0        0        0     5709 2023-05-06 16:19:51.225548 ecgai_drawing-0.1.13/src/ecgai_drawing/create_ecg_plot.py
+-rw-r--r--   0        0        0      988 2023-05-06 16:19:51.225548 ecgai_drawing-0.1.13/src/ecgai_drawing/ecg_plot_image.py
+-rw-r--r--   0        0        0    11995 2023-05-06 16:19:51.225548 ecgai_drawing-0.1.13/src/ecgai_drawing/ecg_plotter.py
+-rw-r--r--   0        0        0        0 2023-05-06 16:19:51.225548 ecgai_drawing-0.1.13/src/ecgai_drawing/enums/__init__.py
+-rw-r--r--   0        0        0      178 2023-05-06 16:19:51.225548 ecgai_drawing-0.1.13/src/ecgai_drawing/enums/artifact.py
+-rw-r--r--   0        0        0      481 2023-05-06 16:19:51.225548 ecgai_drawing-0.1.13/src/ecgai_drawing/enums/color_style.py
+-rw-r--r--   0        0        0      563 2023-05-06 16:19:51.225548 ecgai_drawing-0.1.13/src/ecgai_drawing/enums/ecg_lead_name.py
+-rw-r--r--   0        0        0      676 2023-05-06 16:19:51.225548 ecgai_drawing-0.1.13/src/ecgai_drawing/enums/enum_ordered_base.py
+-rw-r--r--   0        0        0      105 2023-05-06 16:19:51.225548 ecgai_drawing-0.1.13/src/ecgai_drawing/enums/show_grid.py
+-rw-r--r--   0        0        0     8622 2023-05-06 16:19:51.225548 ecgai_drawing-0.1.13/src/ecgai_drawing/images.py
+-rw-r--r--   0        0        0        0 2023-05-06 16:19:51.225548 ecgai_drawing-0.1.13/src/ecgai_drawing/models/__init__.py
+-rw-r--r--   0        0        0      812 2023-05-06 16:19:51.229548 ecgai_drawing-0.1.13/src/ecgai_drawing/models/ecg_lead.py
+-rw-r--r--   0        0        0      647 2023-05-06 16:19:51.229548 ecgai_drawing-0.1.13/src/ecgai_drawing/models/ecg_leads.py
+-rw-r--r--   0        0        0      851 2023-05-06 16:19:51.229548 ecgai_drawing-0.1.13/src/ecgai_drawing/models/model_base.py
+-rw-r--r--   0        0        0      639 1970-01-01 00:00:00.000000 ecgai_drawing-0.1.13/PKG-INFO
```

