# Comparing `tmp/carefree-drawboard-0.0.0a9.tar.gz` & `tmp/carefree-drawboard-0.0.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "carefree-drawboard-0.0.0a9.tar", last modified: Thu Apr 27 15:24:45 2023, max compression
+gzip compressed data, was "carefree-drawboard-0.0.1a0.tar", last modified: Sat May  6 16:27:55 2023, max compression
```

## Comparing `carefree-drawboard-0.0.0a9.tar` & `carefree-drawboard-0.0.1a0.tar`

### file list

```diff
@@ -1,202 +1,212 @@
-drwxrwxrwx   0        0        0        0 2023-04-27 15:24:45.546952 carefree-drawboard-0.0.0a9/
--rw-rw-rw-   0        0        0    11557 2023-04-12 06:16:04.000000 carefree-drawboard-0.0.0a9/LICENSE
--rw-rw-rw-   0        0        0      121 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/MANIFEST.in
--rw-rw-rw-   0        0        0     9233 2023-04-27 15:24:45.546952 carefree-drawboard-0.0.0a9/PKG-INFO
--rw-rw-rw-   0        0        0     8950 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/README.md
-drwxrwxrwx   0        0        0        0 2023-04-27 15:24:45.475951 carefree-drawboard-0.0.0a9/carefree_drawboard.egg-info/
--rw-rw-rw-   0        0        0     9233 2023-04-27 15:24:45.000000 carefree-drawboard-0.0.0a9/carefree_drawboard.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     5867 2023-04-27 15:24:45.000000 carefree-drawboard-0.0.0a9/carefree_drawboard.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-27 15:24:45.000000 carefree-drawboard-0.0.0a9/carefree_drawboard.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2023-04-27 15:24:45.000000 carefree-drawboard-0.0.0a9/carefree_drawboard.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      164 2023-04-27 15:24:45.000000 carefree-drawboard-0.0.0a9/carefree_drawboard.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-27 15:24:45.000000 carefree-drawboard-0.0.0a9/carefree_drawboard.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-27 15:24:45.477949 carefree-drawboard-0.0.0a9/cfdraw/
-drwxrwxrwx   0        0        0        0 2023-04-27 15:24:45.481949 carefree-drawboard-0.0.0a9/cfdraw/.web/
--rw-rw-rw-   0        0        0      121 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/.env
--rw-rw-rw-   0        0        0      143 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/.prettierrc
--rw-rw-rw-   0        0        0      323 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/index.html
--rw-rw-rw-   0        0        0     1628 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/package.json
-drwxrwxrwx   0        0        0        0 2023-04-27 15:24:45.485949 carefree-drawboard-0.0.0a9/cfdraw/.web/src/
--rw-rw-rw-   0        0        0      992 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/App.tsx
--rw-rw-rw-   0        0        0     1454 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/BoardPanel.tsx
--rw-rw-rw-   0        0        0     6410 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/_settings.ts
-drwxrwxrwx   0        0        0        0 2023-04-27 15:24:45.489949 carefree-drawboard-0.0.0a9/cfdraw/.web/src/actions/
--rw-rw-rw-   0        0        0     2263 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/actions/addImage.ts
--rw-rw-rw-   0        0        0      960 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/actions/addText.ts
--rw-rw-rw-   0        0        0     9418 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/actions/arrange.ts
--rw-rw-rw-   0        0        0     1776 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/actions/download.ts
--rw-rw-rw-   0        0        0     1970 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/actions/export.ts
--rw-rw-rw-   0        0        0     5628 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/actions/importMeta.ts
--rw-rw-rw-   0        0        0     1292 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/actions/managePlugins.ts
--rw-rw-rw-   0        0        0     3304 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/actions/manageProjects.ts
--rw-rw-rw-   0        0        0      272 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/actions/update.ts
--rw-rw-rw-   0        0        0     1018 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/actions/uploadImage.ts
-drwxrwxrwx   0        0        0        0 2023-04-27 15:24:45.451465 carefree-drawboard-0.0.0a9/cfdraw/.web/src/assets/
-drwxrwxrwx   0        0        0        0 2023-04-27 15:24:45.489949 carefree-drawboard-0.0.0a9/cfdraw/.web/src/assets/icons/
--rw-rw-rw-   0        0        0      257 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/assets/icons/arrow-down.svg
-drwxrwxrwx   0        0        0        0 2023-04-27 15:24:45.495950 carefree-drawboard-0.0.0a9/cfdraw/.web/src/components/
--rw-rw-rw-   0        0        0      763 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/components/CFButton.tsx
--rw-rw-rw-   0        0        0      640 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/components/CFCircularProgress.tsx
--rw-rw-rw-   0        0        0      359 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/components/CFDivider.tsx
--rw-rw-rw-   0        0        0      243 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/components/CFHeading.tsx
-drwxrwxrwx   0        0        0        0 2023-04-27 15:24:45.496949 carefree-drawboard-0.0.0a9/cfdraw/.web/src/components/CFIcon/
--rw-rw-rw-   0        0        0      546 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/components/CFIcon/index.scss
--rw-rw-rw-   0        0        0     1568 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/components/CFIcon/index.tsx
--rw-rw-rw-   0        0        0     1484 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/components/CFImageUploader.tsx
--rw-rw-rw-   0        0        0      346 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/components/CFInput.tsx
-drwxrwxrwx   0        0        0        0 2023-04-27 15:24:45.497949 carefree-drawboard-0.0.0a9/cfdraw/.web/src/components/CFSelect/
--rw-rw-rw-   0        0        0       70 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/components/CFSelect/index.scss
--rw-rw-rw-   0        0        0     3483 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/components/CFSelect/index.tsx
--rw-rw-rw-   0        0        0     4606 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/components/CFSlider.tsx
--rw-rw-rw-   0        0        0     1644 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/components/CFSwitch.tsx
--rw-rw-rw-   0        0        0      324 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/components/CFText.tsx
--rw-rw-rw-   0        0        0      408 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/components/CFTooltip.tsx
-drwxrwxrwx   0        0        0        0 2023-04-27 15:24:45.499949 carefree-drawboard-0.0.0a9/cfdraw/.web/src/hooks/
--rw-rw-rw-   0        0        0     2924 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/hooks/useFileDropper.ts
--rw-rw-rw-   0        0        0     4289 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/hooks/useGridLines.ts
--rw-rw-rw-   0        0        0     2003 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/hooks/useInitBoard.ts
--rw-rw-rw-   0        0        0      445 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/hooks/usePreventDefaults.ts
--rw-rw-rw-   0        0        0     5154 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/hooks/usePython.ts
--rw-rw-rw-   0        0        0      131 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/index.scss
--rw-rw-rw-   0        0        0      345 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/index.tsx
-drwxrwxrwx   0        0        0        0 2023-04-27 15:24:45.503949 carefree-drawboard-0.0.0a9/cfdraw/.web/src/lang/
--rw-rw-rw-   0        0        0      792 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/lang/add.ts
--rw-rw-rw-   0        0        0      849 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/lang/brush.ts
--rw-rw-rw-   0        0        0     1148 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/lang/download.ts
--rw-rw-rw-   0        0        0     1508 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/lang/index.ts
--rw-rw-rw-   0        0        0      404 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/lang/nodeEditor.ts
--rw-rw-rw-   0        0        0     2302 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/lang/plugins.ts
--rw-rw-rw-   0        0        0     1746 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/lang/projects.ts
--rw-rw-rw-   0        0        0      896 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/lang/settings.ts
--rw-rw-rw-   0        0        0     7075 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/lang/toast.ts
--rw-rw-rw-   0        0        0     2343 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/lang/tooltip.ts
--rw-rw-rw-   0        0        0     1788 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/lang/ui.ts
-drwxrwxrwx   0        0        0        0 2023-04-27 15:24:45.503949 carefree-drawboard-0.0.0a9/cfdraw/.web/src/plugins/
-drwxrwxrwx   0        0        0        0 2023-04-27 15:24:45.507949 carefree-drawboard-0.0.0a9/cfdraw/.web/src/plugins/_python/
--rw-rw-rw-   0        0        0      681 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/plugins/_python/DefinitionFields.tsx
--rw-rw-rw-   0        0        0     4421 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/plugins/_python/FieldsPlugin.tsx
--rw-rw-rw-   0        0        0     2699 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/plugins/_python/PluginWithSubmit.tsx
--rw-rw-rw-   0        0        0     1936 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/plugins/_python/QAPlugin.tsx
--rw-rw-rw-   0        0        0     1627 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/plugins/_python/TextAreaPlugin.tsx
--rw-rw-rw-   0        0        0      847 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/plugins/_python/hooks.ts
-drwxrwxrwx   0        0        0        0 2023-04-27 15:24:45.513949 carefree-drawboard-0.0.0a9/cfdraw/.web/src/plugins/_react/
--rw-rw-rw-   0        0        0     2690 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/plugins/_react/AddPlugin.tsx
--rw-rw-rw-   0        0        0      714 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/plugins/_react/ArrangePlugin.tsx
--rw-rw-rw-   0        0        0     4628 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/plugins/_react/BrushPlugin.tsx
--rw-rw-rw-   0        0        0      854 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/plugins/_react/DeletePlugin.tsx
--rw-rw-rw-   0        0        0     3430 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/plugins/_react/DownloadPlugin.tsx
--rw-rw-rw-   0        0        0     1083 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/plugins/_react/GroupPlugin.tsx
--rw-rw-rw-   0        0        0     1123 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/plugins/_react/LinksPlugin.tsx
--rw-rw-rw-   0        0        0     1311 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/plugins/_react/MetaPlugin.tsx
--rw-rw-rw-   0        0        0     6321 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/plugins/_react/ProjectPlugin.tsx
--rw-rw-rw-   0        0        0     5074 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/plugins/_react/SettingsPlugin.tsx
--rw-rw-rw-   0        0        0     2374 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/plugins/_react/TextEditorPlugin.tsx
--rw-rw-rw-   0        0        0     1253 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/plugins/_react/UndoRedoPlugin.tsx
-drwxrwxrwx   0        0        0        0 2023-04-27 15:24:45.515949 carefree-drawboard-0.0.0a9/cfdraw/.web/src/plugins/components/
-drwxrwxrwx   0        0        0        0 2023-04-27 15:24:45.517949 carefree-drawboard-0.0.0a9/cfdraw/.web/src/plugins/components/Fields/
--rw-rw-rw-   0        0        0     1317 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/plugins/components/Fields/NumberField.tsx
--rw-rw-rw-   0        0        0      689 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/plugins/components/Fields/SelectField.tsx
--rw-rw-rw-   0        0        0      780 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/plugins/components/Fields/TextField.tsx
--rw-rw-rw-   0        0        0     1129 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/plugins/components/Fields/index.tsx
--rw-rw-rw-   0        0        0      580 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/plugins/components/Fields/utils.ts
--rw-rw-rw-   0        0        0    11507 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/plugins/components/Floating.tsx
--rw-rw-rw-   0        0        0      307 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/plugins/components/Link.tsx
--rw-rw-rw-   0        0        0     7028 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/plugins/components/Render.tsx
--rw-rw-rw-   0        0        0      225 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/plugins/components/hooks.ts
--rw-rw-rw-   0        0        0     2441 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/plugins/index.tsx
-drwxrwxrwx   0        0        0        0 2023-04-27 15:24:45.518949 carefree-drawboard-0.0.0a9/cfdraw/.web/src/plugins/utils/
--rw-rw-rw-   0        0        0     1575 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/plugins/utils/factory.ts
--rw-rw-rw-   0        0        0      583 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/plugins/utils/renderFilters.ts
--rw-rw-rw-   0        0        0      841 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/react-app-env.d.ts
-drwxrwxrwx   0        0        0        0 2023-04-27 15:24:45.519949 carefree-drawboard-0.0.0a9/cfdraw/.web/src/requests/
--rw-rw-rw-   0        0        0     1028 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/requests/actions.ts
--rw-rw-rw-   0        0        0     3151 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/requests/hooks.ts
-drwxrwxrwx   0        0        0        0 2023-04-27 15:24:45.520949 carefree-drawboard-0.0.0a9/cfdraw/.web/src/requests/interceptors/
--rw-rw-rw-   0        0        0      880 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/requests/interceptors/_python.ts
--rw-rw-rw-   0        0        0      752 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/requests/interceptors/index.ts
--rw-rw-rw-   0        0        0       38 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/reset.d.ts
-drwxrwxrwx   0        0        0        0 2023-04-27 15:24:45.522949 carefree-drawboard-0.0.0a9/cfdraw/.web/src/schema/
--rw-rw-rw-   0        0        0     4081 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/schema/_python.ts
--rw-rw-rw-   0        0        0     1169 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/schema/fields.ts
--rw-rw-rw-   0        0        0     1806 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/schema/meta.ts
--rw-rw-rw-   0        0        0      190 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/schema/misc.ts
--rw-rw-rw-   0        0        0     3154 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/schema/plugins.ts
--rw-rw-rw-   0        0        0      850 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/schema/requests.ts
-drwxrwxrwx   0        0        0        0 2023-04-27 15:24:45.529950 carefree-drawboard-0.0.0a9/cfdraw/.web/src/stores/
--rw-rw-rw-   0        0        0     2918 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/stores/_python.ts
--rw-rw-rw-   0        0        0      586 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/stores/debug.ts
--rw-rw-rw-   0        0        0     1495 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/stores/gridLines.ts
--rw-rw-rw-   0        0        0      578 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/stores/hooks.ts
--rw-rw-rw-   0        0        0     1457 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/stores/init.ts
--rw-rw-rw-   0        0        0     1107 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/stores/meta.ts
--rw-rw-rw-   0        0        0     1561 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/stores/pluginVisible.ts
--rw-rw-rw-   0        0        0     2874 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/stores/plugins.ts
--rw-rw-rw-   0        0        0     2060 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/stores/pointerEvents.ts
--rw-rw-rw-   0        0        0     1704 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/stores/projects.ts
--rw-rw-rw-   0        0        0      525 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/stores/settings.ts
--rw-rw-rw-   0        0        0     7004 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/stores/socket.ts
--rw-rw-rw-   0        0        0     3859 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/stores/theme.ts
--rw-rw-rw-   0        0        0     2031 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/stores/ui.ts
--rw-rw-rw-   0        0        0      866 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/stores/user.ts
-drwxrwxrwx   0        0        0        0 2023-04-27 15:24:45.531949 carefree-drawboard-0.0.0a9/cfdraw/.web/src/utils/
--rw-rw-rw-   0        0        0      467 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/utils/bem.ts
--rw-rw-rw-   0        0        0      533 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/utils/constants.ts
--rw-rw-rw-   0        0        0      934 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/utils/event.ts
--rw-rw-rw-   0        0        0     1091 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/utils/misc.ts
--rw-rw-rw-   0        0        0     2012 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/utils/toast.ts
--rw-rw-rw-   0        0        0       39 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/src/vite-env.d.ts
--rw-rw-rw-   0        0        0      656 2023-04-27 15:22:10.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/tsconfig.json
--rw-rw-rw-   0        0        0      193 2023-04-27 15:22:10.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/tsconfig.node.json
--rw-rw-rw-   0        0        0      103 2023-04-27 15:22:10.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/tsconfig.paths.json
--rw-rw-rw-   0        0        0     1849 2023-04-27 15:22:10.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/vite.config.ts
--rw-rw-rw-   0        0        0   214083 2023-04-27 15:22:10.000000 carefree-drawboard-0.0.0a9/cfdraw/.web/yarn.lock
--rw-rw-rw-   0        0        0      487 2023-04-27 15:22:10.000000 carefree-drawboard-0.0.0a9/cfdraw/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-27 15:24:45.532948 carefree-drawboard-0.0.0a9/cfdraw/app/
--rw-rw-rw-   0        0        0       20 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a9/cfdraw/app/__init__.py
--rw-rw-rw-   0        0        0     3163 2023-04-27 15:22:10.000000 carefree-drawboard-0.0.0a9/cfdraw/app/app.py
-drwxrwxrwx   0        0        0        0 2023-04-27 15:24:45.535948 carefree-drawboard-0.0.0a9/cfdraw/app/endpoints/
--rw-rw-rw-   0        0        0      139 2023-04-27 15:22:10.000000 carefree-drawboard-0.0.0a9/cfdraw/app/endpoints/__init__.py
--rw-rw-rw-   0        0        0      745 2023-04-27 15:22:10.000000 carefree-drawboard-0.0.0a9/cfdraw/app/endpoints/assets.py
--rw-rw-rw-   0        0        0      493 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a9/cfdraw/app/endpoints/base.py
--rw-rw-rw-   0        0        0     5713 2023-04-27 15:22:10.000000 carefree-drawboard-0.0.0a9/cfdraw/app/endpoints/project.py
--rw-rw-rw-   0        0        0     6920 2023-04-27 15:22:10.000000 carefree-drawboard-0.0.0a9/cfdraw/app/endpoints/queue.py
--rw-rw-rw-   0        0        0     2158 2023-04-27 15:22:10.000000 carefree-drawboard-0.0.0a9/cfdraw/app/endpoints/upload.py
--rw-rw-rw-   0        0        0     3674 2023-04-27 15:22:10.000000 carefree-drawboard-0.0.0a9/cfdraw/app/endpoints/websocket.py
--rw-rw-rw-   0        0        0     1277 2023-04-27 15:22:10.000000 carefree-drawboard-0.0.0a9/cfdraw/app/schema.py
--rw-rw-rw-   0        0        0     3333 2023-04-27 15:22:10.000000 carefree-drawboard-0.0.0a9/cfdraw/cli.py
--rw-rw-rw-   0        0        0     2245 2023-04-27 15:22:10.000000 carefree-drawboard-0.0.0a9/cfdraw/config.py
--rw-rw-rw-   0        0        0     1456 2023-04-27 15:22:10.000000 carefree-drawboard-0.0.0a9/cfdraw/constants.py
-drwxrwxrwx   0        0        0        0 2023-04-27 15:24:45.536948 carefree-drawboard-0.0.0a9/cfdraw/parsers/
--rw-rw-rw-   0        0        0       44 2023-04-09 01:57:56.000000 carefree-drawboard-0.0.0a9/cfdraw/parsers/__init__.py
--rw-rw-rw-   0        0        0      609 2023-04-12 06:16:04.000000 carefree-drawboard-0.0.0a9/cfdraw/parsers/chakra.py
--rw-rw-rw-   0        0        0     6847 2023-04-27 15:22:10.000000 carefree-drawboard-0.0.0a9/cfdraw/parsers/noli.py
-drwxrwxrwx   0        0        0        0 2023-04-27 15:24:45.538948 carefree-drawboard-0.0.0a9/cfdraw/plugins/
--rw-rw-rw-   0        0        0       92 2023-04-27 15:22:10.000000 carefree-drawboard-0.0.0a9/cfdraw/plugins/__init__.py
--rw-rw-rw-   0        0        0     4774 2023-04-27 15:22:10.000000 carefree-drawboard-0.0.0a9/cfdraw/plugins/base.py
-drwxrwxrwx   0        0        0        0 2023-04-27 15:24:45.538948 carefree-drawboard-0.0.0a9/cfdraw/plugins/community/
--rw-rw-rw-   0        0        0        0 2023-04-14 05:16:37.000000 carefree-drawboard-0.0.0a9/cfdraw/plugins/community/__init__.py
--rw-rw-rw-   0        0        0     2472 2023-04-27 15:22:10.000000 carefree-drawboard-0.0.0a9/cfdraw/plugins/factory.py
-drwxrwxrwx   0        0        0        0 2023-04-27 15:24:45.540948 carefree-drawboard-0.0.0a9/cfdraw/plugins/middlewares/
--rw-rw-rw-   0        0        0      100 2023-04-27 15:22:10.000000 carefree-drawboard-0.0.0a9/cfdraw/plugins/middlewares/__init__.py
--rw-rw-rw-   0        0        0      908 2023-04-27 15:22:10.000000 carefree-drawboard-0.0.0a9/cfdraw/plugins/middlewares/fields.py
--rw-rw-rw-   0        0        0      735 2023-04-27 15:22:10.000000 carefree-drawboard-0.0.0a9/cfdraw/plugins/middlewares/send_message.py
--rw-rw-rw-   0        0        0      500 2023-04-27 15:22:10.000000 carefree-drawboard-0.0.0a9/cfdraw/plugins/middlewares/text_area.py
--rw-rw-rw-   0        0        0      643 2023-04-27 15:22:10.000000 carefree-drawboard-0.0.0a9/cfdraw/plugins/middlewares/timer.py
--rw-rw-rw-   0        0        0      959 2023-04-27 15:22:10.000000 carefree-drawboard-0.0.0a9/cfdraw/plugins/sync.py
-drwxrwxrwx   0        0        0        0 2023-04-27 15:24:45.541949 carefree-drawboard-0.0.0a9/cfdraw/schema/
--rw-rw-rw-   0        0        0       47 2023-04-13 15:19:11.000000 carefree-drawboard-0.0.0a9/cfdraw/schema/__init__.py
--rw-rw-rw-   0        0        0     3153 2023-04-27 15:22:10.000000 carefree-drawboard-0.0.0a9/cfdraw/schema/fields.py
--rw-rw-rw-   0        0        0    14769 2023-04-27 15:22:10.000000 carefree-drawboard-0.0.0a9/cfdraw/schema/plugins.py
-drwxrwxrwx   0        0        0        0 2023-04-27 15:24:45.546952 carefree-drawboard-0.0.0a9/cfdraw/utils/
--rw-rw-rw-   0        0        0        0 2023-04-08 03:23:05.000000 carefree-drawboard-0.0.0a9/cfdraw/utils/__init__.py
--rw-rw-rw-   0        0        0      833 2023-04-27 15:22:10.000000 carefree-drawboard-0.0.0a9/cfdraw/utils/cache.py
--rw-rw-rw-   0        0        0      875 2023-04-27 15:22:10.000000 carefree-drawboard-0.0.0a9/cfdraw/utils/console.py
--rw-rw-rw-   0        0        0     6551 2023-04-27 15:22:10.000000 carefree-drawboard-0.0.0a9/cfdraw/utils/data_structures.py
--rw-rw-rw-   0        0        0     2622 2023-04-27 15:22:10.000000 carefree-drawboard-0.0.0a9/cfdraw/utils/exec.py
--rw-rw-rw-   0        0        0     2337 2023-04-27 15:22:10.000000 carefree-drawboard-0.0.0a9/cfdraw/utils/misc.py
--rw-rw-rw-   0        0        0      638 2023-04-27 15:22:10.000000 carefree-drawboard-0.0.0a9/cfdraw/utils/prerequisites.py
--rw-rw-rw-   0        0        0     1766 2023-04-27 15:22:10.000000 carefree-drawboard-0.0.0a9/cfdraw/utils/processes.py
--rw-rw-rw-   0        0        0     3667 2023-04-27 15:22:10.000000 carefree-drawboard-0.0.0a9/cfdraw/utils/server.py
--rw-rw-rw-   0        0        0     2744 2023-04-27 15:22:10.000000 carefree-drawboard-0.0.0a9/cfdraw/utils/template.py
--rw-rw-rw-   0        0        0      113 2023-04-27 15:24:45.550951 carefree-drawboard-0.0.0a9/setup.cfg
--rw-rw-rw-   0        0        0     1063 2023-04-27 15:24:12.000000 carefree-drawboard-0.0.0a9/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-06 16:27:55.162707 carefree-drawboard-0.0.1a0/
+-rw-rw-rw-   0        0        0    11557 2023-04-20 17:03:10.000000 carefree-drawboard-0.0.1a0/LICENSE
+-rw-rw-rw-   0        0        0      121 2023-04-20 17:03:10.000000 carefree-drawboard-0.0.1a0/MANIFEST.in
+-rw-rw-rw-   0        0        0     9112 2023-05-06 16:27:55.163704 carefree-drawboard-0.0.1a0/PKG-INFO
+-rw-rw-rw-   0        0        0     8829 2023-05-06 11:47:25.000000 carefree-drawboard-0.0.1a0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-06 16:27:54.805445 carefree-drawboard-0.0.1a0/carefree_drawboard.egg-info/
+-rw-rw-rw-   0        0        0     9112 2023-05-06 16:27:50.000000 carefree-drawboard-0.0.1a0/carefree_drawboard.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     6277 2023-05-06 16:27:54.000000 carefree-drawboard-0.0.1a0/carefree_drawboard.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 16:27:50.000000 carefree-drawboard-0.0.1a0/carefree_drawboard.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2023-05-06 16:27:50.000000 carefree-drawboard-0.0.1a0/carefree_drawboard.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      164 2023-05-06 16:27:50.000000 carefree-drawboard-0.0.1a0/carefree_drawboard.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-06 16:27:50.000000 carefree-drawboard-0.0.1a0/carefree_drawboard.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-06 16:27:54.811428 carefree-drawboard-0.0.1a0/cfdraw/
+drwxrwxrwx   0        0        0        0 2023-05-06 16:27:54.825363 carefree-drawboard-0.0.1a0/cfdraw/.web/
+-rw-rw-rw-   0        0        0      121 2023-04-20 17:03:10.000000 carefree-drawboard-0.0.1a0/cfdraw/.web/.env
+-rw-rw-rw-   0        0        0      143 2023-04-20 17:03:10.000000 carefree-drawboard-0.0.1a0/cfdraw/.web/.prettierrc
+-rw-rw-rw-   0        0        0      323 2023-05-04 14:02:39.000000 carefree-drawboard-0.0.1a0/cfdraw/.web/index.html
+-rw-rw-rw-   0        0        0     1669 2023-05-06 11:14:50.000000 carefree-drawboard-0.0.1a0/cfdraw/.web/package.json
+drwxrwxrwx   0        0        0        0 2023-05-06 16:27:54.838329 carefree-drawboard-0.0.1a0/cfdraw/.web/src/
+-rw-rw-rw-   0        0        0     1007 2023-05-04 14:02:39.000000 carefree-drawboard-0.0.1a0/cfdraw/.web/src/App.tsx
+-rw-rw-rw-   0        0        0     1470 2023-05-04 14:02:39.000000 carefree-drawboard-0.0.1a0/cfdraw/.web/src/BoardPanel.tsx
+-rw-rw-rw-   0        0        0     5509 2023-05-06 11:14:50.000000 carefree-drawboard-0.0.1a0/cfdraw/.web/src/_settings.ts
+drwxrwxrwx   0        0        0        0 2023-05-06 16:27:54.857312 carefree-drawboard-0.0.1a0/cfdraw/.web/src/actions/
+-rw-rw-rw-   0        0        0     2334 2023-05-04 14:02:39.000000 carefree-drawboard-0.0.1a0/cfdraw/.web/src/actions/addImage.ts
+-rw-rw-rw-   0        0        0      960 2023-04-20 17:03:10.000000 carefree-drawboard-0.0.1a0/cfdraw/.web/src/actions/addText.ts
+-rw-rw-rw-   0        0        0     9418 2023-05-04 14:02:39.000000 carefree-drawboard-0.0.1a0/cfdraw/.web/src/actions/arrange.ts
+-rw-rw-rw-   0        0        0     1806 2023-05-04 14:02:39.000000 carefree-drawboard-0.0.1a0/cfdraw/.web/src/actions/download.ts
+-rw-rw-rw-   0        0        0     1970 2023-05-04 14:02:39.000000 carefree-drawboard-0.0.1a0/cfdraw/.web/src/actions/export.ts
+-rw-rw-rw-   0        0        0      236 2023-05-04 14:02:39.000000 carefree-drawboard-0.0.1a0/cfdraw/.web/src/actions/i18n.ts
+-rw-rw-rw-   0        0        0     8242 2023-05-06 11:14:50.000000 carefree-drawboard-0.0.1a0/cfdraw/.web/src/actions/importMeta.ts
+-rw-rw-rw-   0        0        0     1448 2023-05-04 14:02:39.000000 carefree-drawboard-0.0.1a0/cfdraw/.web/src/actions/managePlugins.ts
+-rw-rw-rw-   0        0        0     5032 2023-05-04 14:02:39.000000 carefree-drawboard-0.0.1a0/cfdraw/.web/src/actions/manageProjects.ts
+-rw-rw-rw-   0        0        0      272 2023-04-20 17:03:10.000000 carefree-drawboard-0.0.1a0/cfdraw/.web/src/actions/update.ts
+-rw-rw-rw-   0        0        0     1118 2023-05-06 11:14:50.000000 carefree-drawboard-0.0.1a0/cfdraw/.web/src/actions/uploadImage.ts
+drwxrwxrwx   0        0        0        0 2023-05-06 16:27:54.860297 carefree-drawboard-0.0.1a0/cfdraw/.web/src/assets/
+-rw-rw-rw-   0        0        0     6591 2023-05-04 14:02:39.000000 carefree-drawboard-0.0.1a0/cfdraw/.web/src/assets/icon-loading.json
+drwxrwxrwx   0        0        0        0 2023-05-06 16:27:54.863261 carefree-drawboard-0.0.1a0/cfdraw/.web/src/assets/icons/
+-rw-rw-rw-   0        0        0      257 2023-04-20 17:03:10.000000 carefree-drawboard-0.0.1a0/cfdraw/.web/src/assets/icons/arrow-down.svg
+-rw-rw-rw-   0        0        0      925 2023-05-04 14:02:39.000000 carefree-drawboard-0.0.1a0/cfdraw/.web/src/assets/icons/delete.svg
+-rw-rw-rw-   0        0        0     6681 2023-05-04 14:02:39.000000 carefree-drawboard-0.0.1a0/cfdraw/.web/src/assets/loading-page.json
+drwxrwxrwx   0        0        0        0 2023-05-06 16:27:54.884208 carefree-drawboard-0.0.1a0/cfdraw/.web/src/components/
+-rw-rw-rw-   0        0        0     2740 2023-05-06 11:14:50.000000 carefree-drawboard-0.0.1a0/cfdraw/.web/src/components/CFButton.tsx
+-rw-rw-rw-   0        0        0      640 2023-04-24 13:50:54.000000 carefree-drawboard-0.0.1a0/cfdraw/.web/src/components/CFCircularProgress.tsx
+-rw-rw-rw-   0        0        0      359 2023-04-20 17:03:10.000000 carefree-drawboard-0.0.1a0/cfdraw/.web/src/components/CFDivider.tsx
+-rw-rw-rw-   0        0        0      235 2023-05-04 14:02:39.000000 carefree-drawboard-0.0.1a0/cfdraw/.web/src/components/CFHeading.tsx
+drwxrwxrwx   0        0        0        0 2023-05-06 16:27:54.887201 carefree-drawboard-0.0.1a0/cfdraw/.web/src/components/CFIcon/
+-rw-rw-rw-   0        0        0      546 2023-04-20 17:03:10.000000 carefree-drawboard-0.0.1a0/cfdraw/.web/src/components/CFIcon/index.scss
+-rw-rw-rw-   0        0        0     1568 2023-04-20 17:03:10.000000 carefree-drawboard-0.0.1a0/cfdraw/.web/src/components/CFIcon/index.tsx
+-rw-rw-rw-   0        0        0     1484 2023-05-04 14:02:39.000000 carefree-drawboard-0.0.1a0/cfdraw/.web/src/components/CFImageUploader.tsx
+-rw-rw-rw-   0        0        0      522 2023-05-04 14:02:39.000000 carefree-drawboard-0.0.1a0/cfdraw/.web/src/components/CFInput.tsx
+-rw-rw-rw-   0        0        0     1382 2023-05-04 14:02:39.000000 carefree-drawboard-0.0.1a0/cfdraw/.web/src/components/CFLoadingPage.tsx
+-rw-rw-rw-   0        0        0      984 2023-05-04 14:02:40.000000 carefree-drawboard-0.0.1a0/cfdraw/.web/src/components/CFLottie.tsx
+drwxrwxrwx   0        0        0        0 2023-05-06 16:27:54.890194 carefree-drawboard-0.0.1a0/cfdraw/.web/src/components/CFSelect/
+-rw-rw-rw-   0        0        0       70 2023-04-20 17:03:10.000000 carefree-drawboard-0.0.1a0/cfdraw/.web/src/components/CFSelect/index.scss
+-rw-rw-rw-   0        0        0     3514 2023-05-04 14:02:40.000000 carefree-drawboard-0.0.1a0/cfdraw/.web/src/components/CFSelect/index.tsx
+-rw-rw-rw-   0        0        0     5223 2023-05-04 14:02:40.000000 carefree-drawboard-0.0.1a0/cfdraw/.web/src/components/CFSlider.tsx
+-rw-rw-rw-   0        0        0     1738 2023-05-04 14:02:40.000000 carefree-drawboard-0.0.1a0/cfdraw/.web/src/components/CFSwitch.tsx
+-rw-rw-rw-   0        0        0      740 2023-05-04 14:02:40.000000 carefree-drawboard-0.0.1a0/cfdraw/.web/src/components/CFText.tsx
+-rw-rw-rw-   0        0        0      531 2023-05-04 14:02:40.000000 carefree-drawboard-0.0.1a0/cfdraw/.web/src/components/CFTextarea.tsx
+-rw-rw-rw-   0        0        0      417 2023-05-04 14:02:40.000000 carefree-drawboard-0.0.1a0/cfdraw/.web/src/components/CFTooltip.tsx
+drwxrwxrwx   0        0        0        0 2023-05-06 16:27:54.902671 carefree-drawboard-0.0.1a0/cfdraw/.web/src/hooks/
+-rw-rw-rw-   0        0        0     1022 2023-05-04 14:02:40.000000 carefree-drawboard-0.0.1a0/cfdraw/.web/src/hooks/useAuth.ts
+-rw-rw-rw-   0        0        0     3077 2023-05-04 14:02:40.000000 carefree-drawboard-0.0.1a0/cfdraw/.web/src/hooks/useFileDropper.ts
+-rw-rw-rw-   0        0        0     4289 2023-04-20 17:03:10.000000 carefree-drawboard-0.0.1a0/cfdraw/.web/src/hooks/useGridLines.ts
+-rw-rw-rw-   0        0        0     3763 2023-05-06 11:14:50.000000 carefree-drawboard-0.0.1a0/cfdraw/.web/src/hooks/useInitBoard.ts
+-rw-rw-rw-   0        0        0      445 2023-04-20 17:03:10.000000 carefree-drawboard-0.0.1a0/cfdraw/.web/src/hooks/usePreventDefaults.ts
+-rw-rw-rw-   0        0        0     5838 2023-05-06 12:17:22.000000 carefree-drawboard-0.0.1a0/cfdraw/.web/src/hooks/usePython.ts
+-rw-rw-rw-   0        0        0    10948 2023-05-06 11:14:50.000000 carefree-drawboard-0.0.1a0/cfdraw/.web/src/hooks/useSetup.ts
+-rw-rw-rw-   0        0        0      131 2023-04-20 17:03:10.000000 carefree-drawboard-0.0.1a0/cfdraw/.web/src/index.scss
+-rw-rw-rw-   0        0        0      345 2023-05-04 14:02:40.000000 carefree-drawboard-0.0.1a0/cfdraw/.web/src/index.tsx
+drwxrwxrwx   0        0        0        0 2023-05-06 16:27:54.923614 carefree-drawboard-0.0.1a0/cfdraw/.web/src/lang/
+-rw-rw-rw-   0        0        0      954 2023-05-06 11:14:50.000000 carefree-drawboard-0.0.1a0/cfdraw/.web/src/lang/add.ts
+-rw-rw-rw-   0        0        0      849 2023-04-20 17:03:10.000000 carefree-drawboard-0.0.1a0/cfdraw/.web/src/lang/brush.ts
+-rw-rw-rw-   0        0        0     1148 2023-04-20 17:03:10.000000 carefree-drawboard-0.0.1a0/cfdraw/.web/src/lang/download.ts
+-rw-rw-rw-   0        0        0     1466 2023-05-04 14:02:40.000000 carefree-drawboard-0.0.1a0/cfdraw/.web/src/lang/index.ts
+-rw-rw-rw-   0        0        0      404 2023-04-20 17:03:10.000000 carefree-drawboard-0.0.1a0/cfdraw/.web/src/lang/nodeEditor.ts
+-rw-rw-rw-   0        0        0     2372 2023-05-06 11:14:50.000000 carefree-drawboard-0.0.1a0/cfdraw/.web/src/lang/plugins.ts
+-rw-rw-rw-   0        0        0     1746 2023-04-20 17:03:10.000000 carefree-drawboard-0.0.1a0/cfdraw/.web/src/lang/projects.ts
+-rw-rw-rw-   0        0        0      896 2023-04-20 17:03:10.000000 carefree-drawboard-0.0.1a0/cfdraw/.web/src/lang/settings.ts
+-rw-rw-rw-   0        0        0    10105 2023-05-06 11:14:50.000000 carefree-drawboard-0.0.1a0/cfdraw/.web/src/lang/toast.ts
+-rw-rw-rw-   0        0        0     2343 2023-05-04 14:02:40.000000 carefree-drawboard-0.0.1a0/cfdraw/.web/src/lang/tooltip.ts
+-rw-rw-rw-   0        0        0      976 2023-05-06 11:14:50.000000 carefree-drawboard-0.0.1a0/cfdraw/.web/src/lang/ui.ts
+drwxrwxrwx   0        0        0        0 2023-05-06 16:27:54.925609 carefree-drawboard-0.0.1a0/cfdraw/.web/src/plugins/
+drwxrwxrwx   0        0        0        0 2023-05-06 16:27:54.938575 carefree-drawboard-0.0.1a0/cfdraw/.web/src/plugins/_python/
+-rw-rw-rw-   0        0        0     2196 2023-05-06 11:14:50.000000 carefree-drawboard-0.0.1a0/cfdraw/.web/src/plugins/_python/ChatPlugin.tsx
+-rw-rw-rw-   0        0        0     3027 2023-05-06 11:14:50.000000 carefree-drawboard-0.0.1a0/cfdraw/.web/src/plugins/_python/FieldsPlugin.tsx
+-rw-rw-rw-   0        0        0     2920 2023-05-04 14:02:40.000000 carefree-drawboard-0.0.1a0/cfdraw/.web/src/plugins/_python/PluginGroup.tsx
+-rw-rw-rw-   0        0        0     3394 2023-05-06 11:14:50.000000 carefree-drawboard-0.0.1a0/cfdraw/.web/src/plugins/_python/PluginWithSubmit.tsx
+-rw-rw-rw-   0        0        0     1909 2023-05-06 11:14:50.000000 carefree-drawboard-0.0.1a0/cfdraw/.web/src/plugins/_python/QAPlugin.tsx
+-rw-rw-rw-   0        0        0     2127 2023-05-06 11:14:50.000000 carefree-drawboard-0.0.1a0/cfdraw/.web/src/plugins/_python/TextAreaPlugin.tsx
+-rw-rw-rw-   0        0        0     2613 2023-05-06 11:14:50.000000 carefree-drawboard-0.0.1a0/cfdraw/.web/src/plugins/_python/hooks.ts
+drwxrwxrwx   0        0        0        0 2023-05-06 16:27:54.958522 carefree-drawboard-0.0.1a0/cfdraw/.web/src/plugins/_react/
+-rw-rw-rw-   0        0        0     3760 2023-05-06 11:14:50.000000 carefree-drawboard-0.0.1a0/cfdraw/.web/src/plugins/_react/AddPlugin.tsx
+-rw-rw-rw-   0        0        0      714 2023-05-04 14:02:40.000000 carefree-drawboard-0.0.1a0/cfdraw/.web/src/plugins/_react/ArrangePlugin.tsx
+-rw-rw-rw-   0        0        0     4598 2023-05-04 14:02:40.000000 carefree-drawboard-0.0.1a0/cfdraw/.web/src/plugins/_react/BrushPlugin.tsx
+-rw-rw-rw-   0        0        0      854 2023-04-26 01:34:04.000000 carefree-drawboard-0.0.1a0/cfdraw/.web/src/plugins/_react/DeletePlugin.tsx
+-rw-rw-rw-   0        0        0     3430 2023-05-04 14:02:40.000000 carefree-drawboard-0.0.1a0/cfdraw/.web/src/plugins/_react/DownloadPlugin.tsx
+-rw-rw-rw-   0        0        0     1083 2023-04-26 01:34:25.000000 carefree-drawboard-0.0.1a0/cfdraw/.web/src/plugins/_react/GroupPlugin.tsx
+-rw-rw-rw-   0        0        0     1123 2023-04-26 01:34:38.000000 carefree-drawboard-0.0.1a0/cfdraw/.web/src/plugins/_react/LinksPlugin.tsx
+-rw-rw-rw-   0        0        0     1315 2023-05-04 14:02:40.000000 carefree-drawboard-0.0.1a0/cfdraw/.web/src/plugins/_react/MetaPlugin.tsx
+-rw-rw-rw-   0        0        0     8594 2023-05-04 14:02:40.000000 carefree-drawboard-0.0.1a0/cfdraw/.web/src/plugins/_react/ProjectPlugin.tsx
+-rw-rw-rw-   0        0        0     4927 2023-05-04 14:02:40.000000 carefree-drawboard-0.0.1a0/cfdraw/.web/src/plugins/_react/SettingsPlugin.tsx
+-rw-rw-rw-   0        0        0     2204 2023-05-04 14:02:40.000000 carefree-drawboard-0.0.1a0/cfdraw/.web/src/plugins/_react/TextEditorPlugin.tsx
+-rw-rw-rw-   0        0        0     1266 2023-05-04 14:02:40.000000 carefree-drawboard-0.0.1a0/cfdraw/.web/src/plugins/_react/UndoRedoPlugin.tsx
+drwxrwxrwx   0        0        0        0 2023-05-06 16:27:54.966500 carefree-drawboard-0.0.1a0/cfdraw/.web/src/plugins/components/
+drwxrwxrwx   0        0        0        0 2023-05-06 16:27:54.976474 carefree-drawboard-0.0.1a0/cfdraw/.web/src/plugins/components/Fields/
+-rw-rw-rw-   0        0        0     1116 2023-05-04 14:02:40.000000 carefree-drawboard-0.0.1a0/cfdraw/.web/src/plugins/components/Fields/BooleanField.tsx
+-rw-rw-rw-   0        0        0     2043 2023-05-04 14:02:40.000000 carefree-drawboard-0.0.1a0/cfdraw/.web/src/plugins/components/Fields/NumberField.tsx
+-rw-rw-rw-   0        0        0     1510 2023-05-04 14:02:40.000000 carefree-drawboard-0.0.1a0/cfdraw/.web/src/plugins/components/Fields/SelectField.tsx
+-rw-rw-rw-   0        0        0     2291 2023-05-04 14:02:40.000000 carefree-drawboard-0.0.1a0/cfdraw/.web/src/plugins/components/Fields/TextField.tsx
+-rw-rw-rw-   0        0        0     2620 2023-05-04 14:02:40.000000 carefree-drawboard-0.0.1a0/cfdraw/.web/src/plugins/components/Fields/index.tsx
+-rw-rw-rw-   0        0        0      720 2023-05-04 14:02:40.000000 carefree-drawboard-0.0.1a0/cfdraw/.web/src/plugins/components/Fields/utils.ts
+-rw-rw-rw-   0        0        0     7821 2023-05-06 11:29:48.000000 carefree-drawboard-0.0.1a0/cfdraw/.web/src/plugins/components/Floating.tsx
+-rw-rw-rw-   0        0        0      307 2023-04-20 17:03:10.000000 carefree-drawboard-0.0.1a0/cfdraw/.web/src/plugins/components/Link.tsx
+-rw-rw-rw-   0        0        0    10915 2023-05-06 11:14:50.000000 carefree-drawboard-0.0.1a0/cfdraw/.web/src/plugins/components/Render.tsx
+-rw-rw-rw-   0        0        0      214 2023-05-04 14:02:40.000000 carefree-drawboard-0.0.1a0/cfdraw/.web/src/plugins/components/hooks.ts
+-rw-rw-rw-   0        0        0     2295 2023-05-06 11:14:50.000000 carefree-drawboard-0.0.1a0/cfdraw/.web/src/plugins/index.tsx
+drwxrwxrwx   0        0        0        0 2023-05-06 16:27:54.981462 carefree-drawboard-0.0.1a0/cfdraw/.web/src/plugins/utils/
+-rw-rw-rw-   0        0        0     1960 2023-05-06 11:14:50.000000 carefree-drawboard-0.0.1a0/cfdraw/.web/src/plugins/utils/cleanup.ts
+-rw-rw-rw-   0        0        0     1450 2023-05-04 14:02:40.000000 carefree-drawboard-0.0.1a0/cfdraw/.web/src/plugins/utils/factory.ts
+-rw-rw-rw-   0        0        0     5167 2023-05-06 11:14:50.000000 carefree-drawboard-0.0.1a0/cfdraw/.web/src/plugins/utils/renderFilters.ts
+-rw-rw-rw-   0        0        0      841 2023-04-20 17:03:10.000000 carefree-drawboard-0.0.1a0/cfdraw/.web/src/react-app-env.d.ts
+drwxrwxrwx   0        0        0        0 2023-05-06 16:27:54.985452 carefree-drawboard-0.0.1a0/cfdraw/.web/src/requests/
+-rw-rw-rw-   0        0        0     1290 2023-05-04 14:02:40.000000 carefree-drawboard-0.0.1a0/cfdraw/.web/src/requests/actions.ts
+-rw-rw-rw-   0        0        0     3091 2023-05-06 11:14:50.000000 carefree-drawboard-0.0.1a0/cfdraw/.web/src/requests/hooks.ts
+drwxrwxrwx   0        0        0        0 2023-05-06 16:27:54.988473 carefree-drawboard-0.0.1a0/cfdraw/.web/src/requests/interceptors/
+-rw-rw-rw-   0        0        0      880 2023-05-04 14:02:40.000000 carefree-drawboard-0.0.1a0/cfdraw/.web/src/requests/interceptors/_python.ts
+-rw-rw-rw-   0        0        0      752 2023-04-20 17:03:10.000000 carefree-drawboard-0.0.1a0/cfdraw/.web/src/requests/interceptors/index.ts
+-rw-rw-rw-   0        0        0       38 2023-04-20 17:03:10.000000 carefree-drawboard-0.0.1a0/cfdraw/.web/src/reset.d.ts
+drwxrwxrwx   0        0        0        0 2023-05-06 16:27:54.997941 carefree-drawboard-0.0.1a0/cfdraw/.web/src/schema/
+-rw-rw-rw-   0        0        0     5005 2023-05-06 11:14:50.000000 carefree-drawboard-0.0.1a0/cfdraw/.web/src/schema/_python.ts
+-rw-rw-rw-   0        0        0     1642 2023-05-04 14:02:40.000000 carefree-drawboard-0.0.1a0/cfdraw/.web/src/schema/fields.ts
+-rw-rw-rw-   0        0        0     2076 2023-05-06 11:14:50.000000 carefree-drawboard-0.0.1a0/cfdraw/.web/src/schema/meta.ts
+-rw-rw-rw-   0        0        0      313 2023-05-04 14:02:40.000000 carefree-drawboard-0.0.1a0/cfdraw/.web/src/schema/misc.ts
+-rw-rw-rw-   0        0        0     3514 2023-05-06 11:14:50.000000 carefree-drawboard-0.0.1a0/cfdraw/.web/src/schema/plugins.ts
+-rw-rw-rw-   0        0        0      850 2023-04-20 17:03:10.000000 carefree-drawboard-0.0.1a0/cfdraw/.web/src/schema/requests.ts
+drwxrwxrwx   0        0        0        0 2023-05-06 16:27:55.021871 carefree-drawboard-0.0.1a0/cfdraw/.web/src/stores/
+-rw-rw-rw-   0        0        0      792 2023-05-04 14:02:40.000000 carefree-drawboard-0.0.1a0/cfdraw/.web/src/stores/debug.ts
+-rw-rw-rw-   0        0        0     1495 2023-04-21 15:33:42.000000 carefree-drawboard-0.0.1a0/cfdraw/.web/src/stores/gridLines.ts
+-rw-rw-rw-   0        0        0      578 2023-04-20 17:03:10.000000 carefree-drawboard-0.0.1a0/cfdraw/.web/src/stores/hooks.ts
+-rw-rw-rw-   0        0        0     1107 2023-04-20 17:03:10.000000 carefree-drawboard-0.0.1a0/cfdraw/.web/src/stores/meta.ts
+-rw-rw-rw-   0        0        0     7336 2023-05-06 11:14:50.000000 carefree-drawboard-0.0.1a0/cfdraw/.web/src/stores/pluginsInfo.ts
+-rw-rw-rw-   0        0        0     2060 2023-04-26 15:39:26.000000 carefree-drawboard-0.0.1a0/cfdraw/.web/src/stores/pointerEvents.ts
+-rw-rw-rw-   0        0        0     1858 2023-05-04 14:02:40.000000 carefree-drawboard-0.0.1a0/cfdraw/.web/src/stores/projects.ts
+-rw-rw-rw-   0        0        0     1692 2023-05-04 14:02:40.000000 carefree-drawboard-0.0.1a0/cfdraw/.web/src/stores/settings.ts
+-rw-rw-rw-   0        0        0     7764 2023-05-06 11:14:50.000000 carefree-drawboard-0.0.1a0/cfdraw/.web/src/stores/socket.ts
+-rw-rw-rw-   0        0        0     4852 2023-05-04 14:02:40.000000 carefree-drawboard-0.0.1a0/cfdraw/.web/src/stores/theme.ts
+-rw-rw-rw-   0        0        0     2054 2023-05-04 14:02:40.000000 carefree-drawboard-0.0.1a0/cfdraw/.web/src/stores/ui.ts
+-rw-rw-rw-   0        0        0      501 2023-05-04 14:02:40.000000 carefree-drawboard-0.0.1a0/cfdraw/.web/src/stores/user.ts
+drwxrwxrwx   0        0        0        0 2023-05-06 16:27:55.029849 carefree-drawboard-0.0.1a0/cfdraw/.web/src/utils/
+-rw-rw-rw-   0        0        0      467 2023-04-20 17:03:10.000000 carefree-drawboard-0.0.1a0/cfdraw/.web/src/utils/bem.ts
+-rw-rw-rw-   0        0        0     3876 2023-05-06 11:29:48.000000 carefree-drawboard-0.0.1a0/cfdraw/.web/src/utils/constants.ts
+-rw-rw-rw-   0        0        0     1266 2023-05-04 14:02:40.000000 carefree-drawboard-0.0.1a0/cfdraw/.web/src/utils/event.ts
+-rw-rw-rw-   0        0        0     1091 2023-04-24 13:50:54.000000 carefree-drawboard-0.0.1a0/cfdraw/.web/src/utils/misc.ts
+-rw-rw-rw-   0        0        0     2041 2023-05-04 14:02:40.000000 carefree-drawboard-0.0.1a0/cfdraw/.web/src/utils/toast.ts
+-rw-rw-rw-   0        0        0       39 2023-04-20 17:03:10.000000 carefree-drawboard-0.0.1a0/cfdraw/.web/src/vite-env.d.ts
+-rw-rw-rw-   0        0        0      656 2023-04-20 17:03:10.000000 carefree-drawboard-0.0.1a0/cfdraw/.web/tsconfig.json
+-rw-rw-rw-   0        0        0      193 2023-04-20 17:03:10.000000 carefree-drawboard-0.0.1a0/cfdraw/.web/tsconfig.node.json
+-rw-rw-rw-   0        0        0      103 2023-04-20 17:03:10.000000 carefree-drawboard-0.0.1a0/cfdraw/.web/tsconfig.paths.json
+-rw-rw-rw-   0        0        0     1811 2023-05-04 14:02:40.000000 carefree-drawboard-0.0.1a0/cfdraw/.web/vite.config.ts
+-rw-rw-rw-   0        0        0   213456 2023-05-06 11:14:50.000000 carefree-drawboard-0.0.1a0/cfdraw/.web/yarn.lock
+-rw-rw-rw-   0        0        0      551 2023-05-04 14:02:40.000000 carefree-drawboard-0.0.1a0/cfdraw/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 16:27:55.034835 carefree-drawboard-0.0.1a0/cfdraw/app/
+-rw-rw-rw-   0        0        0       20 2023-04-20 17:03:10.000000 carefree-drawboard-0.0.1a0/cfdraw/app/__init__.py
+-rw-rw-rw-   0        0        0     3163 2023-05-06 12:17:45.000000 carefree-drawboard-0.0.1a0/cfdraw/app/app.py
+drwxrwxrwx   0        0        0        0 2023-05-06 16:27:55.048916 carefree-drawboard-0.0.1a0/cfdraw/app/endpoints/
+-rw-rw-rw-   0        0        0      139 2023-04-23 16:07:30.000000 carefree-drawboard-0.0.1a0/cfdraw/app/endpoints/__init__.py
+-rw-rw-rw-   0        0        0      745 2023-04-21 15:33:42.000000 carefree-drawboard-0.0.1a0/cfdraw/app/endpoints/assets.py
+-rw-rw-rw-   0        0        0      493 2023-04-20 17:03:10.000000 carefree-drawboard-0.0.1a0/cfdraw/app/endpoints/base.py
+-rw-rw-rw-   0        0        0     6862 2023-05-04 14:02:40.000000 carefree-drawboard-0.0.1a0/cfdraw/app/endpoints/project.py
+-rw-rw-rw-   0        0        0     6918 2023-05-04 14:02:40.000000 carefree-drawboard-0.0.1a0/cfdraw/app/endpoints/queue.py
+-rw-rw-rw-   0        0        0     3419 2023-05-06 12:17:45.000000 carefree-drawboard-0.0.1a0/cfdraw/app/endpoints/upload.py
+-rw-rw-rw-   0        0        0     3672 2023-05-04 14:02:40.000000 carefree-drawboard-0.0.1a0/cfdraw/app/endpoints/websocket.py
+-rw-rw-rw-   0        0        0     1277 2023-04-25 15:43:23.000000 carefree-drawboard-0.0.1a0/cfdraw/app/schema.py
+-rw-rw-rw-   0        0        0     3518 2023-05-04 14:02:40.000000 carefree-drawboard-0.0.1a0/cfdraw/cli.py
+-rw-rw-rw-   0        0        0     2361 2023-05-04 14:02:40.000000 carefree-drawboard-0.0.1a0/cfdraw/config.py
+-rw-rw-rw-   0        0        0     2874 2023-05-04 14:02:40.000000 carefree-drawboard-0.0.1a0/cfdraw/constants.py
+drwxrwxrwx   0        0        0        0 2023-05-06 16:27:55.053903 carefree-drawboard-0.0.1a0/cfdraw/parsers/
+-rw-rw-rw-   0        0        0       44 2023-04-20 17:03:10.000000 carefree-drawboard-0.0.1a0/cfdraw/parsers/__init__.py
+-rw-rw-rw-   0        0        0      710 2023-05-04 14:02:40.000000 carefree-drawboard-0.0.1a0/cfdraw/parsers/chakra.py
+-rw-rw-rw-   0        0        0    13291 2023-05-06 11:14:50.000000 carefree-drawboard-0.0.1a0/cfdraw/parsers/noli.py
+drwxrwxrwx   0        0        0        0 2023-05-06 16:27:55.062879 carefree-drawboard-0.0.1a0/cfdraw/plugins/
+-rw-rw-rw-   0        0        0      123 2023-05-04 14:02:40.000000 carefree-drawboard-0.0.1a0/cfdraw/plugins/__init__.py
+-rw-rw-rw-   0        0        0     6755 2023-05-06 11:14:50.000000 carefree-drawboard-0.0.1a0/cfdraw/plugins/base.py
+drwxrwxrwx   0        0        0        0 2023-05-06 16:27:55.064873 carefree-drawboard-0.0.1a0/cfdraw/plugins/community/
+-rw-rw-rw-   0        0        0        0 2023-04-20 17:03:10.000000 carefree-drawboard-0.0.1a0/cfdraw/plugins/community/__init__.py
+-rw-rw-rw-   0        0        0     2796 2023-05-06 11:14:50.000000 carefree-drawboard-0.0.1a0/cfdraw/plugins/factory.py
+drwxrwxrwx   0        0        0        0 2023-05-06 16:27:55.107881 carefree-drawboard-0.0.1a0/cfdraw/plugins/middlewares/
+-rw-rw-rw-   0        0        0       76 2023-05-06 11:14:50.000000 carefree-drawboard-0.0.1a0/cfdraw/plugins/middlewares/__init__.py
+-rw-rw-rw-   0        0        0     1651 2023-05-06 12:17:45.000000 carefree-drawboard-0.0.1a0/cfdraw/plugins/middlewares/response.py
+-rw-rw-rw-   0        0        0      904 2023-05-06 11:14:50.000000 carefree-drawboard-0.0.1a0/cfdraw/plugins/middlewares/send_message.py
+-rw-rw-rw-   0        0        0      643 2023-04-25 15:43:23.000000 carefree-drawboard-0.0.1a0/cfdraw/plugins/middlewares/timer.py
+-rw-rw-rw-   0        0        0     1399 2023-05-04 14:02:40.000000 carefree-drawboard-0.0.1a0/cfdraw/plugins/node_validator.py
+-rw-rw-rw-   0        0        0     1040 2023-05-04 14:02:40.000000 carefree-drawboard-0.0.1a0/cfdraw/plugins/sync.py
+drwxrwxrwx   0        0        0        0 2023-05-06 16:27:55.114835 carefree-drawboard-0.0.1a0/cfdraw/schema/
+-rw-rw-rw-   0        0        0       72 2023-05-04 14:02:40.000000 carefree-drawboard-0.0.1a0/cfdraw/schema/__init__.py
+-rw-rw-rw-   0        0        0     4164 2023-05-06 11:14:50.000000 carefree-drawboard-0.0.1a0/cfdraw/schema/fields.py
+-rw-rw-rw-   0        0        0    17859 2023-05-06 11:14:50.000000 carefree-drawboard-0.0.1a0/cfdraw/schema/plugins.py
+-rw-rw-rw-   0        0        0     1615 2023-05-04 14:02:40.000000 carefree-drawboard-0.0.1a0/cfdraw/schema/settings.py
+drwxrwxrwx   0        0        0        0 2023-05-06 16:27:55.147745 carefree-drawboard-0.0.1a0/cfdraw/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-20 17:03:10.000000 carefree-drawboard-0.0.1a0/cfdraw/utils/__init__.py
+-rw-rw-rw-   0        0        0      833 2023-04-20 17:03:10.000000 carefree-drawboard-0.0.1a0/cfdraw/utils/cache.py
+-rw-rw-rw-   0        0        0      875 2023-04-20 17:03:10.000000 carefree-drawboard-0.0.1a0/cfdraw/utils/console.py
+-rw-rw-rw-   0        0        0     6551 2023-04-24 15:25:35.000000 carefree-drawboard-0.0.1a0/cfdraw/utils/data_structures.py
+-rw-rw-rw-   0        0        0     2622 2023-04-22 18:06:29.000000 carefree-drawboard-0.0.1a0/cfdraw/utils/exec.py
+-rw-rw-rw-   0        0        0     2415 2023-05-04 14:02:40.000000 carefree-drawboard-0.0.1a0/cfdraw/utils/misc.py
+-rw-rw-rw-   0        0        0      638 2023-04-20 17:03:10.000000 carefree-drawboard-0.0.1a0/cfdraw/utils/prerequisites.py
+-rw-rw-rw-   0        0        0     1766 2023-04-20 17:03:10.000000 carefree-drawboard-0.0.1a0/cfdraw/utils/processes.py
+-rw-rw-rw-   0        0        0     3914 2023-05-06 11:14:50.000000 carefree-drawboard-0.0.1a0/cfdraw/utils/server.py
+-rw-rw-rw-   0        0        0     2732 2023-05-04 14:02:40.000000 carefree-drawboard-0.0.1a0/cfdraw/utils/template.py
+-rw-rw-rw-   0        0        0      113 2023-05-06 16:27:55.165697 carefree-drawboard-0.0.1a0/setup.cfg
+-rw-rw-rw-   0        0        0     1063 2023-05-06 16:26:30.000000 carefree-drawboard-0.0.1a0/setup.py
```

### Comparing `carefree-drawboard-0.0.0a9/LICENSE` & `carefree-drawboard-0.0.1a0/LICENSE`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a9/PKG-INFO` & `carefree-drawboard-0.0.1a0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,30 @@
-Metadata-Version: 2.1
-Name: carefree-drawboard
-Version: 0.0.0a9
-Summary: 🎨 Infinite Drawboard in Python
-Author: carefree0910
-Author-email: syameimaru.saki@gmail.com
-Keywords: python carefree-learn drawboard
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # carefree-drawboard 🎨
 
 ![Stable Diffusion](examples/assets/stable-diffusion.png)
 
-> This is the screenshot I used for the [Stable Diffusion](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/stable_diffusion) example and I don't know what should be the proper banner, help!
-
 <div align="center">
 
+<br>
+
+**✨ Build performant, Infinite Drawboard based web apps in pure Python.**
+
+<br>
+
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/carefree0910/carefree-drawboard/blob/dev/examples/server.ipynb)
 [![PyPI version](https://badge.fury.io/py/carefree-drawboard.svg)](https://badge.fury.io/py/carefree-drawboard.svg)
 ![Checks](https://github.com/carefree0910/carefree-drawboard/actions/workflows/checks.yml/badge.svg)
 [![License](https://img.shields.io/badge/License-Apache_2.0-yellowgreen.svg)](https://opensource.org/licenses/Apache-2.0)
 
 ### [Wiki](https://github.com/carefree0910/carefree-drawboard/wiki) | [Examples](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples) | [Stable Diffusion](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/stable_diffusion) | [Caption & Diffusion](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/caption_and_diffusion) | [Inpainting](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/stable_diffusion_inpainting) | [ControlNet](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/stable_diffusion_controlnet)
 
 <div align="left">
 
+<br>
+
 ## Installation
 
 `carefree-drawboard` 🎨 requires the following to get started:
 
 * Python 3.8+
 * [Node.js 18+](https://nodejs.org/en/)
 
@@ -74,19 +70,19 @@
 > Notice that the generated template implements a `GaussianBlur` plugin, which requires an image to pop up. You can upload an image either by dragging it directly to the drawboard 🎨, or by clicking the `Plus` button at the top right corner and select `Upload Image`.
 
 [Demo Video](https://user-images.githubusercontent.com/15677328/234529497-8d7f5b61-9154-4211-8d99-ec09fca0dc2d.mp4)
 
 ## Examples
 
 * [**Getting Started**](https://github.com/carefree0910/carefree-drawboard/wiki/Getting-Started), which is a more detailed tutorial to guide you step by step.
-* [Image Processing](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/image_processing), which implements three common image processing plugins with `carefree-drawboard` 🎨.
-* [Stable Diffusion](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/stable_diffusion), which utilizes the famous `diffusers` library and implements two common Stable Diffusion plugins with `carefree-drawboard` 🎨.
+* [Image Processing](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/image_processing), which implements three common image processing plugins. It also shows how to use the `IPluginGroup` in `carefree-drawboard` 🎨 to group the plugins together and make the UI cleaner.
+* [Stable Diffusion](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/stable_diffusion), which utilizes the famous `diffusers` library and implements two common SD plugins.
 * [**Caption & Diffusion**](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/caption_and_diffusion), which shows how can we combine two different kinds of models (`Image Captioning` & `Stable Diffusion`) and make them work together.
-* [Stable Diffusion Inpainting](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/stable_diffusion_inpainting), which shows how can we implement complicated plugins like `StableDiffusionInpainting` very easily with `carefree-drawboard` 🎨.
-* [Stable Diffusion ControlNet](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/stable_diffusion_controlnet), which shows how can we decouple complicated workflows like `ControlNet` into separate, lightweight, and reusable plugins very easily with `carefree-drawboard` 🎨.
+* [Stable Diffusion Inpainting](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/stable_diffusion_inpainting), which shows how can we implement complicated plugins like `StableDiffusionInpainting` very easily.
+* [Stable Diffusion ControlNet](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/stable_diffusion_controlnet), which shows how can we decouple complicated workflows like `ControlNet` into separate, lightweight, and reusable plugins very easily.
 
 ## Documentation
 
 Check the [Wiki](https://github.com/carefree0910/carefree-drawboard/wiki) page for documentation!
 
 ## Status
```

### Comparing `carefree-drawboard-0.0.0a9/README.md` & `carefree-drawboard-0.0.1a0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,40 @@
+Metadata-Version: 2.1
+Name: carefree-drawboard
+Version: 0.0.1a0
+Summary: 🎨 Infinite Drawboard in Python
+Author: carefree0910
+Author-email: syameimaru.saki@gmail.com
+Keywords: python carefree-learn drawboard
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # carefree-drawboard 🎨
 
 ![Stable Diffusion](examples/assets/stable-diffusion.png)
 
-> This is the screenshot I used for the [Stable Diffusion](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/stable_diffusion) example and I don't know what should be the proper banner, help!
-
 <div align="center">
 
+<br>
+
+**✨ Build performant, Infinite Drawboard based web apps in pure Python.**
+
+<br>
+
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/carefree0910/carefree-drawboard/blob/dev/examples/server.ipynb)
 [![PyPI version](https://badge.fury.io/py/carefree-drawboard.svg)](https://badge.fury.io/py/carefree-drawboard.svg)
 ![Checks](https://github.com/carefree0910/carefree-drawboard/actions/workflows/checks.yml/badge.svg)
 [![License](https://img.shields.io/badge/License-Apache_2.0-yellowgreen.svg)](https://opensource.org/licenses/Apache-2.0)
 
 ### [Wiki](https://github.com/carefree0910/carefree-drawboard/wiki) | [Examples](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples) | [Stable Diffusion](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/stable_diffusion) | [Caption & Diffusion](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/caption_and_diffusion) | [Inpainting](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/stable_diffusion_inpainting) | [ControlNet](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/stable_diffusion_controlnet)
 
 <div align="left">
 
+<br>
+
 ## Installation
 
 `carefree-drawboard` 🎨 requires the following to get started:
 
 * Python 3.8+
 * [Node.js 18+](https://nodejs.org/en/)
 
@@ -64,19 +80,19 @@
 > Notice that the generated template implements a `GaussianBlur` plugin, which requires an image to pop up. You can upload an image either by dragging it directly to the drawboard 🎨, or by clicking the `Plus` button at the top right corner and select `Upload Image`.
 
 [Demo Video](https://user-images.githubusercontent.com/15677328/234529497-8d7f5b61-9154-4211-8d99-ec09fca0dc2d.mp4)
 
 ## Examples
 
 * [**Getting Started**](https://github.com/carefree0910/carefree-drawboard/wiki/Getting-Started), which is a more detailed tutorial to guide you step by step.
-* [Image Processing](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/image_processing), which implements three common image processing plugins with `carefree-drawboard` 🎨.
-* [Stable Diffusion](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/stable_diffusion), which utilizes the famous `diffusers` library and implements two common Stable Diffusion plugins with `carefree-drawboard` 🎨.
+* [Image Processing](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/image_processing), which implements three common image processing plugins. It also shows how to use the `IPluginGroup` in `carefree-drawboard` 🎨 to group the plugins together and make the UI cleaner.
+* [Stable Diffusion](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/stable_diffusion), which utilizes the famous `diffusers` library and implements two common SD plugins.
 * [**Caption & Diffusion**](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/caption_and_diffusion), which shows how can we combine two different kinds of models (`Image Captioning` & `Stable Diffusion`) and make them work together.
-* [Stable Diffusion Inpainting](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/stable_diffusion_inpainting), which shows how can we implement complicated plugins like `StableDiffusionInpainting` very easily with `carefree-drawboard` 🎨.
-* [Stable Diffusion ControlNet](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/stable_diffusion_controlnet), which shows how can we decouple complicated workflows like `ControlNet` into separate, lightweight, and reusable plugins very easily with `carefree-drawboard` 🎨.
+* [Stable Diffusion Inpainting](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/stable_diffusion_inpainting), which shows how can we implement complicated plugins like `StableDiffusionInpainting` very easily.
+* [Stable Diffusion ControlNet](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/stable_diffusion_controlnet), which shows how can we decouple complicated workflows like `ControlNet` into separate, lightweight, and reusable plugins very easily.
 
 ## Documentation
 
 Check the [Wiki](https://github.com/carefree0910/carefree-drawboard/wiki) page for documentation!
 
 ## Status
```

### Comparing `carefree-drawboard-0.0.0a9/carefree_drawboard.egg-info/PKG-INFO` & `carefree-drawboard-0.0.1a0/carefree_drawboard.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,40 @@
 Metadata-Version: 2.1
 Name: carefree-drawboard
-Version: 0.0.0a9
+Version: 0.0.1a0
 Summary: 🎨 Infinite Drawboard in Python
 Author: carefree0910
 Author-email: syameimaru.saki@gmail.com
 Keywords: python carefree-learn drawboard
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # carefree-drawboard 🎨
 
 ![Stable Diffusion](examples/assets/stable-diffusion.png)
 
-> This is the screenshot I used for the [Stable Diffusion](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/stable_diffusion) example and I don't know what should be the proper banner, help!
-
 <div align="center">
 
+<br>
+
+**✨ Build performant, Infinite Drawboard based web apps in pure Python.**
+
+<br>
+
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/carefree0910/carefree-drawboard/blob/dev/examples/server.ipynb)
 [![PyPI version](https://badge.fury.io/py/carefree-drawboard.svg)](https://badge.fury.io/py/carefree-drawboard.svg)
 ![Checks](https://github.com/carefree0910/carefree-drawboard/actions/workflows/checks.yml/badge.svg)
 [![License](https://img.shields.io/badge/License-Apache_2.0-yellowgreen.svg)](https://opensource.org/licenses/Apache-2.0)
 
 ### [Wiki](https://github.com/carefree0910/carefree-drawboard/wiki) | [Examples](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples) | [Stable Diffusion](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/stable_diffusion) | [Caption & Diffusion](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/caption_and_diffusion) | [Inpainting](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/stable_diffusion_inpainting) | [ControlNet](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/stable_diffusion_controlnet)
 
 <div align="left">
 
+<br>
+
 ## Installation
 
 `carefree-drawboard` 🎨 requires the following to get started:
 
 * Python 3.8+
 * [Node.js 18+](https://nodejs.org/en/)
 
@@ -74,19 +80,19 @@
 > Notice that the generated template implements a `GaussianBlur` plugin, which requires an image to pop up. You can upload an image either by dragging it directly to the drawboard 🎨, or by clicking the `Plus` button at the top right corner and select `Upload Image`.
 
 [Demo Video](https://user-images.githubusercontent.com/15677328/234529497-8d7f5b61-9154-4211-8d99-ec09fca0dc2d.mp4)
 
 ## Examples
 
 * [**Getting Started**](https://github.com/carefree0910/carefree-drawboard/wiki/Getting-Started), which is a more detailed tutorial to guide you step by step.
-* [Image Processing](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/image_processing), which implements three common image processing plugins with `carefree-drawboard` 🎨.
-* [Stable Diffusion](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/stable_diffusion), which utilizes the famous `diffusers` library and implements two common Stable Diffusion plugins with `carefree-drawboard` 🎨.
+* [Image Processing](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/image_processing), which implements three common image processing plugins. It also shows how to use the `IPluginGroup` in `carefree-drawboard` 🎨 to group the plugins together and make the UI cleaner.
+* [Stable Diffusion](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/stable_diffusion), which utilizes the famous `diffusers` library and implements two common SD plugins.
 * [**Caption & Diffusion**](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/caption_and_diffusion), which shows how can we combine two different kinds of models (`Image Captioning` & `Stable Diffusion`) and make them work together.
-* [Stable Diffusion Inpainting](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/stable_diffusion_inpainting), which shows how can we implement complicated plugins like `StableDiffusionInpainting` very easily with `carefree-drawboard` 🎨.
-* [Stable Diffusion ControlNet](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/stable_diffusion_controlnet), which shows how can we decouple complicated workflows like `ControlNet` into separate, lightweight, and reusable plugins very easily with `carefree-drawboard` 🎨.
+* [Stable Diffusion Inpainting](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/stable_diffusion_inpainting), which shows how can we implement complicated plugins like `StableDiffusionInpainting` very easily.
+* [Stable Diffusion ControlNet](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/stable_diffusion_controlnet), which shows how can we decouple complicated workflows like `ControlNet` into separate, lightweight, and reusable plugins very easily.
 
 ## Documentation
 
 Check the [Wiki](https://github.com/carefree0910/carefree-drawboard/wiki) page for documentation!
 
 ## Status
```

### Comparing `carefree-drawboard-0.0.0a9/carefree_drawboard.egg-info/SOURCES.txt` & `carefree-drawboard-0.0.1a0/carefree_drawboard.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -31,53 +31,63 @@
 cfdraw/.web/src/reset.d.ts
 cfdraw/.web/src/vite-env.d.ts
 cfdraw/.web/src/actions/addImage.ts
 cfdraw/.web/src/actions/addText.ts
 cfdraw/.web/src/actions/arrange.ts
 cfdraw/.web/src/actions/download.ts
 cfdraw/.web/src/actions/export.ts
+cfdraw/.web/src/actions/i18n.ts
 cfdraw/.web/src/actions/importMeta.ts
 cfdraw/.web/src/actions/managePlugins.ts
 cfdraw/.web/src/actions/manageProjects.ts
 cfdraw/.web/src/actions/update.ts
 cfdraw/.web/src/actions/uploadImage.ts
+cfdraw/.web/src/assets/icon-loading.json
+cfdraw/.web/src/assets/loading-page.json
 cfdraw/.web/src/assets/icons/arrow-down.svg
+cfdraw/.web/src/assets/icons/delete.svg
 cfdraw/.web/src/components/CFButton.tsx
 cfdraw/.web/src/components/CFCircularProgress.tsx
 cfdraw/.web/src/components/CFDivider.tsx
 cfdraw/.web/src/components/CFHeading.tsx
 cfdraw/.web/src/components/CFImageUploader.tsx
 cfdraw/.web/src/components/CFInput.tsx
+cfdraw/.web/src/components/CFLoadingPage.tsx
+cfdraw/.web/src/components/CFLottie.tsx
 cfdraw/.web/src/components/CFSlider.tsx
 cfdraw/.web/src/components/CFSwitch.tsx
 cfdraw/.web/src/components/CFText.tsx
+cfdraw/.web/src/components/CFTextarea.tsx
 cfdraw/.web/src/components/CFTooltip.tsx
 cfdraw/.web/src/components/CFIcon/index.scss
 cfdraw/.web/src/components/CFIcon/index.tsx
 cfdraw/.web/src/components/CFSelect/index.scss
 cfdraw/.web/src/components/CFSelect/index.tsx
+cfdraw/.web/src/hooks/useAuth.ts
 cfdraw/.web/src/hooks/useFileDropper.ts
 cfdraw/.web/src/hooks/useGridLines.ts
 cfdraw/.web/src/hooks/useInitBoard.ts
 cfdraw/.web/src/hooks/usePreventDefaults.ts
 cfdraw/.web/src/hooks/usePython.ts
+cfdraw/.web/src/hooks/useSetup.ts
 cfdraw/.web/src/lang/add.ts
 cfdraw/.web/src/lang/brush.ts
 cfdraw/.web/src/lang/download.ts
 cfdraw/.web/src/lang/index.ts
 cfdraw/.web/src/lang/nodeEditor.ts
 cfdraw/.web/src/lang/plugins.ts
 cfdraw/.web/src/lang/projects.ts
 cfdraw/.web/src/lang/settings.ts
 cfdraw/.web/src/lang/toast.ts
 cfdraw/.web/src/lang/tooltip.ts
 cfdraw/.web/src/lang/ui.ts
 cfdraw/.web/src/plugins/index.tsx
-cfdraw/.web/src/plugins/_python/DefinitionFields.tsx
+cfdraw/.web/src/plugins/_python/ChatPlugin.tsx
 cfdraw/.web/src/plugins/_python/FieldsPlugin.tsx
+cfdraw/.web/src/plugins/_python/PluginGroup.tsx
 cfdraw/.web/src/plugins/_python/PluginWithSubmit.tsx
 cfdraw/.web/src/plugins/_python/QAPlugin.tsx
 cfdraw/.web/src/plugins/_python/TextAreaPlugin.tsx
 cfdraw/.web/src/plugins/_python/hooks.ts
 cfdraw/.web/src/plugins/_react/AddPlugin.tsx
 cfdraw/.web/src/plugins/_react/ArrangePlugin.tsx
 cfdraw/.web/src/plugins/_react/BrushPlugin.tsx
@@ -90,39 +100,38 @@
 cfdraw/.web/src/plugins/_react/SettingsPlugin.tsx
 cfdraw/.web/src/plugins/_react/TextEditorPlugin.tsx
 cfdraw/.web/src/plugins/_react/UndoRedoPlugin.tsx
 cfdraw/.web/src/plugins/components/Floating.tsx
 cfdraw/.web/src/plugins/components/Link.tsx
 cfdraw/.web/src/plugins/components/Render.tsx
 cfdraw/.web/src/plugins/components/hooks.ts
+cfdraw/.web/src/plugins/components/Fields/BooleanField.tsx
 cfdraw/.web/src/plugins/components/Fields/NumberField.tsx
 cfdraw/.web/src/plugins/components/Fields/SelectField.tsx
 cfdraw/.web/src/plugins/components/Fields/TextField.tsx
 cfdraw/.web/src/plugins/components/Fields/index.tsx
 cfdraw/.web/src/plugins/components/Fields/utils.ts
+cfdraw/.web/src/plugins/utils/cleanup.ts
 cfdraw/.web/src/plugins/utils/factory.ts
 cfdraw/.web/src/plugins/utils/renderFilters.ts
 cfdraw/.web/src/requests/actions.ts
 cfdraw/.web/src/requests/hooks.ts
 cfdraw/.web/src/requests/interceptors/_python.ts
 cfdraw/.web/src/requests/interceptors/index.ts
 cfdraw/.web/src/schema/_python.ts
 cfdraw/.web/src/schema/fields.ts
 cfdraw/.web/src/schema/meta.ts
 cfdraw/.web/src/schema/misc.ts
 cfdraw/.web/src/schema/plugins.ts
 cfdraw/.web/src/schema/requests.ts
-cfdraw/.web/src/stores/_python.ts
 cfdraw/.web/src/stores/debug.ts
 cfdraw/.web/src/stores/gridLines.ts
 cfdraw/.web/src/stores/hooks.ts
-cfdraw/.web/src/stores/init.ts
 cfdraw/.web/src/stores/meta.ts
-cfdraw/.web/src/stores/pluginVisible.ts
-cfdraw/.web/src/stores/plugins.ts
+cfdraw/.web/src/stores/pluginsInfo.ts
 cfdraw/.web/src/stores/pointerEvents.ts
 cfdraw/.web/src/stores/projects.ts
 cfdraw/.web/src/stores/settings.ts
 cfdraw/.web/src/stores/socket.ts
 cfdraw/.web/src/stores/theme.ts
 cfdraw/.web/src/stores/ui.ts
 cfdraw/.web/src/stores/user.ts
@@ -143,24 +152,25 @@
 cfdraw/app/endpoints/websocket.py
 cfdraw/parsers/__init__.py
 cfdraw/parsers/chakra.py
 cfdraw/parsers/noli.py
 cfdraw/plugins/__init__.py
 cfdraw/plugins/base.py
 cfdraw/plugins/factory.py
+cfdraw/plugins/node_validator.py
 cfdraw/plugins/sync.py
 cfdraw/plugins/community/__init__.py
 cfdraw/plugins/middlewares/__init__.py
-cfdraw/plugins/middlewares/fields.py
+cfdraw/plugins/middlewares/response.py
 cfdraw/plugins/middlewares/send_message.py
-cfdraw/plugins/middlewares/text_area.py
 cfdraw/plugins/middlewares/timer.py
 cfdraw/schema/__init__.py
 cfdraw/schema/fields.py
 cfdraw/schema/plugins.py
+cfdraw/schema/settings.py
 cfdraw/utils/__init__.py
 cfdraw/utils/cache.py
 cfdraw/utils/console.py
 cfdraw/utils/data_structures.py
 cfdraw/utils/exec.py
 cfdraw/utils/misc.py
 cfdraw/utils/prerequisites.py
```

### Comparing `carefree-drawboard-0.0.0a9/cfdraw/.web/package.json` & `carefree-drawboard-0.0.1a0/cfdraw/.web/package.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9892857142857142%*

 * *Differences: {"'dependencies'": "{'@carefree0910/business': '~0.5.1-alpha.3', '@carefree0910/core': "*

 * *                   "'~0.5.1-alpha.3', '@carefree0910/native': '~0.5.1-alpha.3', "*

 * *                   "'@carefree0910/svg': '~0.5.1-alpha.3', 'lottie-web': '^5.11.0', delete: "*

 * *                   "['opentype.js']}"}*

```diff
@@ -1,12 +1,13 @@
 {
     "dependencies": {
-        "@carefree0910/business": "~0.4.10-alpha.4",
-        "@carefree0910/core": "~0.4.10-alpha.1",
-        "@carefree0910/native": "~0.4.10-alpha.4",
+        "@carefree0910/business": "~0.5.1-alpha.3",
+        "@carefree0910/core": "~0.5.1-alpha.3",
+        "@carefree0910/native": "~0.5.1-alpha.3",
+        "@carefree0910/svg": "~0.5.1-alpha.3",
         "@chakra-ui/icons": "^2.0.4",
         "@chakra-ui/react": "^2.2.4",
         "@emotion/react": "^11.9.3",
         "@emotion/styled": "^11.9.3",
         "@svgdotjs/svg.filter.js": "^3.0.8",
         "@svgdotjs/svg.js": "^3.1.1",
         "@svgdotjs/svg.topath.js": "^2.0.3",
@@ -14,19 +15,19 @@
         "ahooks": "^3.7.6",
         "axios": "^1.3.4",
         "classnames": "^2.3.2",
         "eslint": "8.37.0",
         "eslint-config-next": "13.2.4",
         "framer-motion": "^10.10.0",
         "jszip": "^3.7.1",
+        "lottie-web": "^5.11.0",
         "ml-matrix": "^6.10.0",
         "mobx": "6.6.1",
         "mobx-react-lite": "^3.4.0",
         "next": "13.2.4",
-        "opentype.js": "^1.3.4",
         "platform": "^1.3.6",
         "rc-upload": "^4.3.4",
         "react": "18.2.0",
         "react-dom": "18.2.0",
         "uuid": "^9.0.0"
     },
     "devDependencies": {
```

### Comparing `carefree-drawboard-0.0.0a9/cfdraw/.web/src/App.tsx` & `carefree-drawboard-0.0.1a0/cfdraw/.web/src/App.tsx`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 import { Flex } from "@chakra-ui/react";
 import { observer } from "mobx-react-lite";
 
+import { useSetup } from "./hooks/useSetup";
 import { useWebSocket } from "./stores/socket";
 import { usePointerEvents } from "./stores/pointerEvents";
-import { useUserInitialization } from "./stores/user";
 import { useInitBoard } from "./hooks/useInitBoard";
 import { useFileDropper } from "./hooks/useFileDropper";
 import { useGridLines } from "./hooks/useGridLines";
 import { usePreventDefaults } from "./hooks/usePreventDefaults";
-import { useSyncPython } from "./hooks/usePython";
+import CFLoadingPage from "./components/CFLoadingPage";
 import BoardPanel from "./BoardPanel";
 
 function App() {
+  useSetup();
   useWebSocket();
-  useUserInitialization();
-  useSyncPython();
   useInitBoard();
   useFileDropper();
   useGridLines();
   usePreventDefaults();
   usePointerEvents();
 
   return (
     <Flex h="100vh" className="p-editor" direction="column" userSelect="none">
       <Flex w="100%" flex={1}>
-        <BoardPanel />
+        <CFLoadingPage>
+          <BoardPanel />
+        </CFLoadingPage>
       </Flex>
     </Flex>
   );
 }
 
 export default observer(App);
```

### Comparing `carefree-drawboard-0.0.0a9/cfdraw/.web/src/actions/addImage.ts` & `carefree-drawboard-0.0.1a0/cfdraw/.web/src/actions/addImage.ts`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import type { IImageUrls } from "@carefree0910/native";
 import {
   BBox,
   getCenteredBBox,
   ImageNode,
   IRectangleShapeNode,
   RectangleShapeNode,
 } from "@carefree0910/core";
@@ -29,46 +30,46 @@
     node.bboxFields = getCenteredBBox(w, h, BoardStore.board).fields;
   }
   return node;
 }
 
 export function rectangleToImage(
   rectangle: IRectangleShapeNode,
-  src: string,
+  urls: IImageUrls,
   alias?: string,
 ): ImageNode {
   return new ImageNode(
     alias ?? rectangle.alias,
     rectangle.params,
     rectangle.bboxFields,
     rectangle.layerParams,
     undefined,
     undefined,
-    { src },
+    urls,
   );
 }
 
-export function getNewImageNode(alias: string, src: string, info: NewImageInfo): ImageNode {
+export function getNewImageNode(alias: string, urls: IImageUrls, info: NewImageInfo): ImageNode {
   const newRectangle = info.type
     ? info
     : getNewRectangle(alias, info instanceof BBox ? info : { autoFit: true, wh: info });
-  return rectangleToImage(newRectangle, src);
+  return rectangleToImage(newRectangle, urls);
 }
 
 export function addNewImage(
   alias: string,
-  src: string,
+  urls: IImageUrls,
   opt: {
     info: NewImageInfo;
     meta: IMeta;
     callbacks?: BusinessOpCallbacks;
     noSelect?: boolean;
   },
 ): void {
-  const newImage = getNewImageNode(alias, src, opt.info);
+  const newImage = getNewImageNode(alias, urls, opt.info);
   newImage.meta = opt.meta;
   console.log("newImage: ", newImage.snapshot());
   useSafeExecute("addJson", null, true, opt.callbacks, {
     noSelect: opt.noSelect ?? true,
     safeOpt: {
       retry: 3,
       retryInterval: 500,
```

### Comparing `carefree-drawboard-0.0.0a9/cfdraw/.web/src/actions/addText.ts` & `carefree-drawboard-0.0.1a0/cfdraw/.web/src/actions/addText.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a9/cfdraw/.web/src/actions/arrange.ts` & `carefree-drawboard-0.0.1a0/cfdraw/.web/src/actions/arrange.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a9/cfdraw/.web/src/actions/download.ts` & `carefree-drawboard-0.0.1a0/cfdraw/.web/src/actions/download.ts`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import JSZip from "jszip";
 
 import { Graph, INode, download, toJsonBlob } from "@carefree0910/core";
 
 import type { DownloadFormat } from "@/schema/misc";
 import { toastWord } from "@/utils/toast";
 import { Toast_Words } from "@/lang/toast";
-import { useCurrentFullProject } from "./manageProjects";
+import { useCurrentProjectWithUserId } from "./manageProjects";
 import { Exporter } from "./export";
 
 export function downloadCurrentFullProject(): void {
-  const fullProject = useCurrentFullProject();
+  const projectWithUserId = useCurrentProjectWithUserId();
   toastWord("info", Toast_Words["downloading-project-message"]);
-  const blob = toJsonBlob(fullProject);
-  download(blob, `${fullProject.name}.cfdraw`);
+  const blob = toJsonBlob(projectWithUserId);
+  download(blob, `${projectWithUserId.name}.cfdraw`);
 }
 
 export async function downloadNodes(
   nodes: INode[],
   format: DownloadFormat,
   exportOriginalSize: boolean,
 ): Promise<void> {
```

### Comparing `carefree-drawboard-0.0.0a9/cfdraw/.web/src/actions/export.ts` & `carefree-drawboard-0.0.1a0/cfdraw/.web/src/actions/export.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a9/cfdraw/.web/src/actions/importMeta.ts` & `carefree-drawboard-0.0.1a0/cfdraw/.web/src/actions/importMeta.ts`

 * *Files 19% similar despite different names*

```diff
@@ -1,151 +1,225 @@
-import { RectangleShapeNode, getRandomHash, shallowCopy } from "@carefree0910/core";
-import { BoardStore, useAddNode } from "@carefree0910/business";
+import { RectangleShapeNode, getRandomHash, isUndefined, shallowCopy } from "@carefree0910/core";
+import {
+  BoardStore,
+  useAddNode,
+  useDefaultTextContent,
+  useSafeExecute,
+} from "@carefree0910/business";
 
-import type { IMetaData, IPythonFieldsMetaData, MetaType } from "@/schema/meta";
+import type { IPythonFieldsMetaData, IPythonResults, MetaType } from "@/schema/meta";
 import type { IImportMeta } from "@/schema/meta";
 import { toastWord } from "@/utils/toast";
+import { DEFAULT_FONT_SIZE, IMAGE_PLACEHOLDER, NSFW_IMAGE_PLACEHOLDER } from "@/utils/constants";
 import { Toast_Words } from "@/lang/toast";
 import { themeStore } from "@/stores/theme";
 import { updateMeta } from "./update";
 import { addNewText } from "./addText";
 import { addNewImage, getNewRectangle, INewRectangle, NewImageInfo } from "./addImage";
 import { getArrangements } from "./arrange";
 
-// consumers
+// helper functions
 
 function updateElapsedTimes(alias: string): void {
   const node = BoardStore.graph.getNode(alias);
   if (!node || node.type === "group" || !node.params.meta?.data) return;
   node.params.meta.data.elapsedTimes = { endTime: Date.now() };
   updateMeta(alias, node.params.meta);
 }
 
+function getWHFromContent(content: string, fontSize: number): { w: number; h: number } {
+  const numChars = content.length;
+  const ratio = Math.sqrt(0.75 * numChars);
+  const h = Math.ceil(fontSize * ratio);
+  const w = h * 2;
+  return { w, h };
+}
+
+// consumers
+
 const consumers: Record<MetaType, (input: IImportMeta<any>) => void> = {
   upload: consumeUpload,
   "add.text": consumeAddText,
+  "add.blank": consumeAddBlank,
   "add.sketch.path": consumeAddSketchPath,
   "python.fields": consumePythonFields,
 };
 function consumeUpload({ type, metaData }: IImportMeta<"upload">): void {
   const success = async () => {
-    toastWord("success", Toast_Words["upload-image-success-message"]);
+    if (safe) {
+      toastWord("success", Toast_Words["upload-image-success-message"]);
+    }
     updateElapsedTimes(newAlias);
   };
   const failed = async () => {
     toastWord("error", Toast_Words["upload-image-error-message"]);
   };
-  const { w, h, url, isDrag } = metaData;
+  let { w, h, url, safe, reason, isDrag } = metaData;
   const prefix = isDrag ? "drag-" : "";
   const newAlias = `${prefix}upload.${getRandomHash()}`;
   metaData.alias = newAlias;
   const bboxInfo: NewImageInfo = { w, h };
-  addNewImage(newAlias, url, {
-    info: bboxInfo,
-    meta: { type, data: metaData },
-    callbacks: { success, failed },
-    noSelect: false,
-  });
+  if (!safe) {
+    url = metaData.url = NSFW_IMAGE_PLACEHOLDER;
+    toastWord("warning", Toast_Words["nsfw-image-detected-warning-message"], {
+      appendix: ` (${reason})`,
+    });
+  }
+  addNewImage(
+    newAlias,
+    { src: url, placeholder: IMAGE_PLACEHOLDER },
+    {
+      info: bboxInfo,
+      meta: { type, data: metaData },
+      callbacks: { success, failed },
+      noSelect: false,
+    },
+  );
 }
 function consumeAddText({ lang, type, metaData }: IImportMeta<"add.text">): void {
   const newAlias = `add.text.${getRandomHash()}`;
   const { textColor } = themeStore.styles;
 
   const success = async () => {
     toastWord("success", Toast_Words["add-text-success-message"]);
     updateElapsedTimes(newAlias);
   };
   const failed = async () => {
     toastWord("error", Toast_Words["add-text-error-message"]);
   };
   const { addText } = useAddNode({ success, failed });
   metaData.alias = newAlias;
+  const content = useDefaultTextContent(lang);
+  const fontSize = DEFAULT_FONT_SIZE;
+  const { w, h } = getWHFromContent(content, fontSize);
   addText({ trace: true })({
     alias: newAlias,
     initColor: textColor,
     lang,
     autoFit: true,
     meta: { type, data: metaData },
+    content,
+    fontSize,
+    w,
+    h,
+  });
+}
+function consumeAddBlank({ type, metaData }: IImportMeta<"add.blank">): void {
+  const newAlias = `add.blank.${getRandomHash()}`;
+
+  const success = async () => {
+    toastWord("success", Toast_Words["add-blank-success-message"]);
+    updateElapsedTimes(newAlias);
+  };
+  const failed = async () => {
+    toastWord("error", Toast_Words["add-blank-error-message"]);
+  };
+  metaData.alias = newAlias;
+  const node = getNewRectangle(newAlias, { autoFit: true, wh: { w: 512, h: 512 } });
+  node.params.meta = { type, data: metaData };
+  useSafeExecute("addJson", null, true, { success, failed })({
+    alias: newAlias,
+    json: node.toJson(),
   });
 }
 function consumeAddSketchPath(): void {
   throw Error("Add sketch path by `importMeta` is not supported yet.");
 }
+interface IPack<R> {
+  res: R;
+  alias: string;
+  rectangle: RectangleShapeNode;
+  metaData: IPythonFieldsMetaData;
+}
 function consumePythonFields({ type, metaData }: IImportMeta<"python.fields">): void {
   const success = async () => {
     toastWord("success", Toast_Words["generate-image-success-message"]);
   };
   const failed = async (err: any) => {
     toastWord("error", Toast_Words["post-python-http-fields-plugin-error-message"], {
       appendix: ` (${err})`,
     });
   };
   const getNewAlias = () => `${type}.${metaData.identifier}.${getRandomHash()}`;
-  interface IPack<R> {
-    data: R;
-    alias: string;
-    rectangle: RectangleShapeNode;
-    metaData: IPythonFieldsMetaData;
-  }
-  function gatherPacks<T, R>(
-    responses: T[],
-    getRectangleInfo: (res: T) => INewRectangle,
-    getData: (res: T) => R,
-  ): IPack<R>[] {
-    const packs: IPack<R>[] = [];
-    responses.forEach((res, i) => {
+  function gatherPacks<T extends IPythonResults>(
+    results: T,
+    getRectangleInfo: (res: T["value"][number]) => INewRectangle,
+  ): IPack<T["value"][number]>[] {
+    const packs: IPack<T["value"][number]>[] = [];
+    results.value.forEach((res, i) => {
       const newAlias = getNewAlias();
-      const rectangle = getNewRectangle(`${i}.${getRandomHash()}`, getRectangleInfo(res));
-      const iMetaData = shallowCopy(metaData);
+      let iMetaData = shallowCopy(metaData);
       iMetaData.response.value = metaData.response.value[i] as any;
       iMetaData.alias = newAlias;
-      packs.push({ data: getData(res), alias: newAlias, rectangle, metaData: iMetaData });
+      if (!res.safe) {
+        if (results.type === "text") {
+          results.value[i].text = `NSFW 🙈 (${results.value[i].reason})`;
+        } else {
+          results.value[i].url = NSFW_IMAGE_PLACEHOLDER;
+          iMetaData.response.extra ??= {};
+          iMetaData.response.extra.reason = results.value[i].reason;
+          toastWord("warning", Toast_Words["nsfw-image-detected-warning-message"], {
+            appendix: ` (${results.value[i].reason})`,
+          });
+        }
+      } else if (results.type === "text") {
+        if (results.value[i].text.length === 0) {
+          toastWord("warning", Toast_Words["returned-empty-text-message"]);
+          return;
+        }
+      }
+      // rectangle should be calculated after the safety check,
+      // because the response might be changed
+      const rectangle = getNewRectangle(`${i}.${getRandomHash()}`, getRectangleInfo(res));
+      packs.push({
+        res,
+        alias: newAlias,
+        rectangle,
+        metaData: iMetaData,
+      });
     });
     return packs;
   }
   function getCallbacks(isLast: boolean) {
     return { success: isLast ? success : async () => void 0, failed };
   }
   if (metaData.response.type === "image") {
-    const packs = gatherPacks(
-      metaData.response.value,
-      ({ w, h }) => ({ autoFit: true, wh: { w, h } }),
-      ({ url }) => ({ url }),
-    );
-    const targets = getArrangements(packs.map(({ rectangle }) => rectangle)).targets;
-    packs.forEach(({ data: { url }, alias, metaData }, i) => {
+    const packs = gatherPacks(metaData.response, ({ w, h }) => ({ autoFit: true, wh: { w, h } }));
+    const targets =
+      metaData.from?.type === "add.blank" && !isUndefined(metaData.from.data.alias)
+        ? packs.map(() => BoardStore.graph.getExistingNode(metaData.from?.data.alias!))
+        : getArrangements(packs.map(({ rectangle }) => rectangle)).targets;
+    const anyUnsafe = metaData.response.value.some((res) => !res.safe);
+    packs.forEach(({ res: { url }, alias, metaData }, i) => {
       const isLast = i === packs.length - 1;
-      addNewImage(alias, url, {
-        info: targets[i].bbox,
-        meta: { type, data: metaData },
-        callbacks: getCallbacks(isLast),
-        noSelect: !isLast,
-      });
+      addNewImage(
+        alias,
+        { src: url, placeholder: IMAGE_PLACEHOLDER },
+        {
+          info: targets[i].bbox,
+          meta: { type, data: metaData },
+          callbacks: getCallbacks(isLast && !anyUnsafe),
+          noSelect: true,
+        },
+      );
     });
   } else if (metaData.response.type === "text") {
-    const fontSize = 48;
-    const packs = gatherPacks(
-      metaData.response.value,
-      (content) => {
-        const numChars = content.length;
-        const ratio = Math.sqrt(0.5 * numChars);
-        const h = Math.ceil(fontSize * ratio);
-        const w = h * 2;
-        return { autoFit: true, wh: { w, h } };
-      },
-      (content) => ({ content }),
-    );
+    const fontSize = DEFAULT_FONT_SIZE;
+    const packs = gatherPacks(metaData.response, ({ text }) => ({
+      autoFit: true,
+      wh: getWHFromContent(text, fontSize),
+    }));
     const targets = getArrangements(packs.map(({ rectangle }) => rectangle)).targets;
-    packs.forEach(({ data: { content }, alias, metaData }, i) => {
+    packs.forEach(({ res: { text }, alias, metaData }, i) => {
       const isLast = i === packs.length - 1;
-      addNewText(alias, content, fontSize, {
+      addNewText(alias, text, fontSize, {
         bbox: targets[i].bbox,
         meta: { type, data: metaData },
         callbacks: getCallbacks(isLast),
-        noSelect: !isLast,
+        noSelect: true,
       });
     });
   }
 }
 
 // import api
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `carefree-drawboard-0.0.0a9/cfdraw/.web/src/actions/managePlugins.ts` & `carefree-drawboard-0.0.1a0/cfdraw/.web/src/actions/managePlugins.ts`

 * *Files 15% similar despite different names*

```diff
@@ -1,31 +1,45 @@
 import { runInAction } from "mobx";
 
-import type { AvailablePluginsAndPythonPlugins } from "@/schema/plugins";
+import type { AllPlugins } from "@/schema/plugins";
 import { reactPluginSettings } from "@/_settings";
-import { usePythonPluginSettings } from "@/stores/_python";
-import { setPluginVisible, setPythonPluginVisible } from "@/stores/pluginVisible";
-import { floatingControlEvent } from "@/plugins/components/Floating";
+import { usePythonPluginSettings } from "@/stores/settings";
+import {
+  setPluginExpanded,
+  usePluginsExpanded,
+  setReactPluginVisible,
+  setPythonPluginVisible,
+} from "@/stores/pluginsInfo";
 
-function setAllPlugins(visible: boolean, except?: AvailablePluginsAndPythonPlugins[]) {
+function setAllPluginVisible(visible: boolean, except?: AllPlugins[]) {
   runInAction(() => {
     reactPluginSettings.forEach(({ type }) => {
       if (except?.includes(type)) return;
       if (!["settings", "undo", "redo"].includes(type)) {
-        setPluginVisible(type, visible);
+        setReactPluginVisible(type, visible);
       }
     });
     usePythonPluginSettings().forEach(({ props }) => {
       const identifier = props.pluginInfo.identifier;
       if (except?.includes(identifier)) return;
       setPythonPluginVisible(identifier, visible);
     });
   });
 }
 
-export function hideAllPlugins(opt?: { except?: AvailablePluginsAndPythonPlugins[] }) {
-  floatingControlEvent.emit({ expand: false, ignoreId: true, forceCheckIds: opt?.except });
-  setAllPlugins(false, opt?.except);
+export function collapseAllPlugins(opt?: { except?: AllPlugins[] }) {
+  runInAction(() => {
+    Object.keys(usePluginsExpanded()).forEach((id) => {
+      if (opt?.except && opt.except.some((e) => id.startsWith(e))) return;
+      setPluginExpanded(id, false);
+    });
+  });
+}
+export function hideAllPlugins(opt?: { except?: AllPlugins[] }) {
+  // collapse all plugins first
+  collapseAllPlugins(opt);
+  // then hide all plugins
+  setAllPluginVisible(false, opt?.except);
 }
-export function showAllPlugins(opt?: { except?: AvailablePluginsAndPythonPlugins[] }) {
-  setAllPlugins(true, opt?.except);
+export function showAllPlugins() {
+  setAllPluginVisible(true);
 }
```

### Comparing `carefree-drawboard-0.0.0a9/cfdraw/.web/src/actions/manageProjects.ts` & `carefree-drawboard-0.0.1a0/cfdraw/.web/src/actions/manageProjects.ts`

 * *Files 25% similar despite different names*

```diff
@@ -1,116 +1,162 @@
-import { INodePack, Matrix2D, Matrix2DFields, safeCall } from "@carefree0910/core";
+import {
+  INodePack,
+  Matrix2D,
+  Matrix2DFields,
+  identityMatrix2DFields,
+  safeCall,
+} from "@carefree0910/core";
 import {
   BoardStore,
   safeClearExecuterStack,
   useGlobalTransform,
   useSafeExecute,
 } from "@carefree0910/business";
 
 import { toastWord } from "@/utils/toast";
 import { Toast_Words } from "@/lang/toast";
 import { Requests } from "@/requests/actions";
+import { userStore } from "@/stores/user";
 import {
   IProjectsStore,
-  updateCurrentProject,
+  getNewProjectInfo,
+  updateCurrentProjectInfo,
   updateCurrentProjectUpdateTime,
-  useCurrentProject,
+  useCurrentProjectInfo,
 } from "@/stores/projects";
 
-interface IFullProject extends IProjectsStore {
+export interface IProject extends IProjectsStore {
   graphInfo: INodePack[];
   globalTransform: Matrix2DFields;
 }
+interface IProjectWithUserId extends IProject {
+  userId: string;
+}
+
+export function getNewProject(): IProject {
+  return { graphInfo: [], globalTransform: identityMatrix2DFields, ...getNewProjectInfo() };
+}
 
-export function useCurrentFullProject(): IFullProject {
-  const data = useCurrentProject();
+export function useCurrentProjectWithUserId(): IProjectWithUserId {
+  const info = useCurrentProjectInfo();
+  const userId = userStore.userId;
   const graphInfo = BoardStore.graph.toJsonInfo();
   const globalTransform = useGlobalTransform().globalTransform.fields;
-  return { ...data, graphInfo, globalTransform };
+  return { ...info, userId, graphInfo, globalTransform };
 }
 
-export async function saveProject(
+export function saveProject(
+  projectWithUserId: IProjectWithUserId,
   onSuccess: () => Promise<void>,
   noToast?: boolean,
 ): Promise<void> {
-  updateCurrentProjectUpdateTime();
-  const fullProject = useCurrentFullProject();
   if (!noToast) {
     toastWord("info", Toast_Words["uploading-project-message"]);
   }
 
   return safeCall(
     async () => {
       const res = await Requests.postJson<{
         success: boolean;
         message: string;
-      }>("_python", "/save_project", fullProject);
+      }>("_python", "/save_project", projectWithUserId);
       if (!res.success) {
         toastWord("warning", Toast_Words["save-project-error-message"], {
           appendix: ` - ${res.message}`,
         });
         throw Error;
       }
     },
     {
       success: onSuccess,
       failed: async () => void 0,
     },
   );
 }
-
-export interface ILoadedProject extends IProjectsStore {
-  graphInfo: INodePack[];
-  globalTransform: Matrix2DFields;
+export function saveCurrentProject(
+  onSuccess: () => Promise<void>,
+  noToast?: boolean,
+): Promise<void> {
+  updateCurrentProjectUpdateTime();
+  const projectWithUserId = useCurrentProjectWithUserId();
+  return saveProject(projectWithUserId, onSuccess, noToast);
 }
-function replaceProjectWith(
-  res: ILoadedProject,
-  onSuccess: (res: ILoadedProject) => Promise<void>,
+
+function replaceCurrentProjectWith(
+  project: IProject,
+  onSuccess: (project: IProject) => Promise<void>,
 ): void {
   useSafeExecute("replaceGraph", null, false, {
     success: async () => {
-      BoardStore.api.setGlobalTransform(new Matrix2D(res.globalTransform));
+      BoardStore.api.setGlobalTransform(new Matrix2D(project.globalTransform));
       safeClearExecuterStack();
-      updateCurrentProject(res);
-      onSuccess(res);
+      updateCurrentProjectInfo(project);
+      onSuccess(project);
     },
     failed: async () => void 0,
-  })({ json: JSON.stringify(res.graphInfo), apiInfos: {}, noFit: true });
+  })({ json: JSON.stringify(project.graphInfo), apiInfos: {}, noFit: true });
+}
+export function getProject(uid: string): Promise<IProject> {
+  return Requests.get<IProject>("_python", `/get_project/?userId=${userStore.userId}&uid=${uid}`);
 }
-export async function loadProject(
+export function loadProject(
   uid: string,
-  onSuccess: (res: ILoadedProject) => Promise<void>,
+  onSuccess: (project: IProject) => Promise<void>,
 ): Promise<void> {
   toastWord("info", Toast_Words["loading-project-message"]);
 
   return safeCall(
-    async () =>
-      Requests.get<ILoadedProject>("_python", `/get_project/${uid}`).then((res) =>
-        replaceProjectWith(res, onSuccess),
-      ),
+    async () => getProject(uid).then((res) => replaceCurrentProjectWith(res, onSuccess)),
     {
       success: async () => void 0,
       failed: async () => void 0,
     },
   );
 }
 export function loadLocalProject(
-  res: ILoadedProject,
-  onSuccess: (res: ILoadedProject) => Promise<void>,
+  project: IProject,
+  onSuccess: (project: IProject) => Promise<void>,
   noToast?: boolean,
 ): void {
   if (!noToast) {
     toastWord("info", Toast_Words["loading-project-message"]);
   }
-  replaceProjectWith(res, onSuccess);
+  replaceCurrentProjectWith(project, onSuccess);
 }
 
-interface IProjectItem {
-  uid: string;
-  name: string;
+export function getAllProjectInfo(): Promise<IProjectsStore[] | undefined> {
+  return safeCall(
+    async () =>
+      Requests.get<IProjectsStore[]>("_python", `/all_projects/?userId=${userStore.userId}`),
+    {
+      success: async () => void 0,
+      failed: async () => void 0,
+    },
+  );
 }
-export async function fetchAllProjects(): Promise<IProjectItem[] | undefined> {
-  return safeCall(async () => Requests.get<IProjectItem[]>("_python", "/all_projects"), {
-    success: async () => void 0,
-    failed: async () => void 0,
+
+export const AUTO_SAVE_PREFIX = "auto-save-";
+export function getAutoSaveProjectInfo(): Promise<IProjectsStore | undefined> {
+  if (!userStore.userId) {
+    throw Error("`userId` should be ready before calling `getAutoSaveProject`");
+  }
+  return getAllProjectInfo().then((projects) =>
+    (projects ?? []).find(({ uid }) => uid.startsWith(AUTO_SAVE_PREFIX)),
+  );
+}
+export function getAutoSaveProject(): Promise<IProject> {
+  const userId = userStore.userId;
+  if (!userId) {
+    throw Error("`userId` should be ready before calling `getAutoSaveProject`");
+  }
+  return getAutoSaveProjectInfo().then((info) => {
+    if (info) return getProject(info.uid);
+    const autoSaveProject = { userId, ...getNewProject() };
+    autoSaveProject.uid = `${AUTO_SAVE_PREFIX}${autoSaveProject.uid}`;
+    autoSaveProject.name = "Auto Save";
+    return saveProject(autoSaveProject, async () => void 0, true).then(() => autoSaveProject);
   });
 }
+
+export function deleteProject(uid: string): Promise<void> {
+  return Requests.delete("_python", `/projects/?userId=${userStore.userId}&uid=${uid}`);
+}
```

### Comparing `carefree-drawboard-0.0.0a9/cfdraw/.web/src/actions/uploadImage.ts` & `carefree-drawboard-0.0.1a0/cfdraw/.web/src/actions/uploadImage.ts`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 import { safeCall } from "@carefree0910/core";
 
 import { toastWord } from "@/utils/toast";
 import { Toast_Words } from "@/lang/toast";
 import { Requests } from "@/requests/actions";
+import { userStore } from "@/stores/user";
 
 type UploadImageOptions = {
   failed: (e: any) => Promise<void>;
 };
 
 interface IUploadImageResponseData {
   w: number;
   h: number;
   url: string;
+  safe: boolean;
+  reason: string;
 }
 
 export async function uploadImage(
   blob: Blob,
   { failed }: UploadImageOptions,
 ): Promise<IUploadImageResponseData | void> {
   return safeCall(
     async () => {
-      const res = await Requests.postBlob<{
+      const res = await Requests.postForm<{
         success: boolean;
         message: string;
         data: IUploadImageResponseData;
-      }>("_python", "/upload_image", { key: "image", blob });
+      }>("_python", "/upload_image", { image: blob, userId: userStore.userId });
       if (!res.success) {
         toastWord("warning", Toast_Words["upload-image-error-message"], {
           appendix: ` - ${res.message}`,
         });
         throw Error;
       }
       return res.data;
```

### Comparing `carefree-drawboard-0.0.0a9/cfdraw/.web/src/components/CFCircularProgress.tsx` & `carefree-drawboard-0.0.1a0/cfdraw/.web/src/components/CFCircularProgress.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a9/cfdraw/.web/src/components/CFIcon/index.scss` & `carefree-drawboard-0.0.1a0/cfdraw/.web/src/components/CFIcon/index.scss`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a9/cfdraw/.web/src/components/CFIcon/index.tsx` & `carefree-drawboard-0.0.1a0/cfdraw/.web/src/components/CFIcon/index.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a9/cfdraw/.web/src/components/CFImageUploader.tsx` & `carefree-drawboard-0.0.1a0/cfdraw/.web/src/components/CFImageUploader.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a9/cfdraw/.web/src/components/CFSelect/index.tsx` & `carefree-drawboard-0.0.1a0/cfdraw/.web/src/components/CFSelect/index.tsx`

 * *Files 9% similar despite different names*

```diff
@@ -13,15 +13,15 @@
   MenuListProps,
   Spacer,
 } from "@chakra-ui/react";
 
 import "./index.scss";
 import { ReactComponent as ArrowDownIcon } from "@/assets/icons/arrow-down.svg";
 import { genBlock } from "@/utils/bem";
-import { themeStore } from "@/stores/theme";
+import { themeStore, useScrollBarSx } from "@/stores/theme";
 import CFIcon from "../CFIcon";
 
 export interface ISelect<T extends string> extends MenuButtonProps {
   icon?: ReactElement;
   value: string;
   options: T[];
   iconProps?: BoxProps;
@@ -117,12 +117,12 @@
             );
           })}
         </MenuList>
       ) : null}
     </Menu>
   );
 }
+export const CFSrollableSelect = observer(<T extends string>(props: ISelect<T>) => {
+  return <CFSelect {...props} menuListProps={{ maxH: "116px", sx: useScrollBarSx() }} />;
+});
 
-export function CFSrollableSelect<T extends string>(props: ISelect<T>) {
-  return <CFSelect {...props} menuListProps={{ maxH: "116px", overflowY: "scroll" }} />;
-}
 export default observer(CFSelect);
```

### Comparing `carefree-drawboard-0.0.0a9/cfdraw/.web/src/components/CFSlider.tsx` & `carefree-drawboard-0.0.1a0/cfdraw/.web/src/components/CFSlider.tsx`

 * *Files 24% similar despite different names*

```diff
@@ -1,55 +1,61 @@
 import {
   Slider,
   SliderTrack,
   SliderFilledTrack,
   SliderThumb,
   Flex,
-  Text,
   FlexProps,
 } from "@chakra-ui/react";
 import { observer } from "mobx-react-lite";
 import { useUnmount } from "ahooks";
-import React, { ReactElement, useCallback, useEffect, useState } from "react";
+import React, { useCallback, useEffect, useState } from "react";
+
+import { BoardStore, useGlobalTransform, useIsReady } from "@carefree0910/business";
 
 import { themeStore } from "@/stores/theme";
+import { CFCaption } from "./CFText";
 import CFInput from "./CFInput";
+import CFTooltip from "./CFTooltip";
 
 export interface ICFSlider extends FlexProps {
   className?: string;
   min: number;
   max: number;
   value: number;
   step?: number;
   scale?: "linear" | "logarithmic";
-  label?: string | ReactElement;
+  label?: string;
+  tooltip?: string;
   onSliderChange(value: number): void;
   precision?: number;
 }
 
 const CFSlider: React.FC<ICFSlider> = ({
   className,
   min,
   max,
   value,
   step = 0.01,
   scale = "linear",
   label,
+  tooltip,
   onSliderChange,
   precision = 2,
   ...props
 }) => {
   const [val, setVal] = useState(value ?? 0);
   const [inputVal, setInputVal] = useState<string>(value?.toString() ?? "0");
   const [iptFocused, setIptFocused] = useState(false);
+  const offset = scale === "linear" || min > 0 ? 0 : -min + 1;
 
   const handleSliderChange = useCallback(
     (v: number) => {
       if (scale === "logarithmic") {
-        v = Math.pow(Math.E, v);
+        v = Math.pow(Math.E, v) - offset;
       }
       v = +v.toFixed(precision);
       setVal(v);
       onSliderChange(v);
     },
     [setVal, onSliderChange],
   );
@@ -123,27 +129,25 @@
   const {
     textColor,
     sliderColors: { sliderTrackColor, sliderThumbBorderColor, inputBgColor },
   } = themeStore.styles;
 
   return (
     <Flex className={className} align="center" color={textColor} {...props}>
-      {label && (
-        <Text minW="20%" align="center" fontSize="14px" flexShrink={0}>
-          {label}
-        </Text>
-      )}
+      <CFTooltip label={tooltip}>
+        <CFCaption label={label} />
+      </CFTooltip>
       <Slider
         focusThumbOnChange={!iptFocused}
         flex={1}
         h="32px"
         mx="1em"
-        value={scale === "linear" ? val : Math.log(val)}
-        min={scale === "linear" ? min : Math.log(min)}
-        max={scale === "linear" ? max : Math.log(max)}
+        value={scale === "linear" ? val : Math.log(val + offset)}
+        min={scale === "linear" ? min : Math.log(min + offset)}
+        max={scale === "linear" ? max : Math.log(max + offset)}
         color="#333"
         fontSize="12px"
         step={step}
         onChange={handleSliderChange}>
         <SliderTrack h="2px">
           <SliderFilledTrack bg={sliderTrackColor} />
         </SliderTrack>
@@ -170,9 +174,23 @@
         onBlur={(e) => handleInputBlur(+e.target.value)}
         onKeyDown={handleInputPress}
         onChange={handleInputChange}
       />
     </Flex>
   );
 };
+export const CFGlobalScaleSlider = observer(() => (
+  <>
+    {useIsReady() && (
+      <CFSlider
+        min={BoardStore.board.options.minScale}
+        max={BoardStore.board.options.maxScale}
+        step={0.001}
+        value={useGlobalTransform().globalScale}
+        scale="logarithmic"
+        onSliderChange={(value) => BoardStore.api.setGlobalScale(value)}
+      />
+    )}
+  </>
+));
 
 export default observer(CFSlider);
```

### Comparing `carefree-drawboard-0.0.0a9/cfdraw/.web/src/components/CFSwitch.tsx` & `carefree-drawboard-0.0.1a0/cfdraw/.web/src/components/CFSwitch.tsx`

 * *Files 8% similar despite different names*

```diff
@@ -8,14 +8,15 @@
   Spacer,
   Switch,
 } from "@chakra-ui/react";
 
 import { getRandomHash } from "@carefree0910/core";
 
 import { themeStore } from "@/stores/theme";
+import CFTooltip from "./CFTooltip";
 
 interface ICFSwitch extends FlexProps {
   label: string;
   value: boolean;
   setValue: (value: boolean) => void;
   tooltip?: ReactElement;
   disableSwitch?: boolean;
@@ -34,24 +35,25 @@
   const {
     textColor,
     switchColors: { checkedBgColor, uncheckedBgColor },
   } = themeStore.styles;
 
   return (
     <FormControl display="flex" alignItems="center" {...props}>
-      <FormLabel
-        mb="0"
-        color={textColor}
-        fontSize={props.fontSize ?? "14px"}
-        htmlFor={hashId}
-        userSelect="none"
-        {...formLabelProps}>
-        {label}
-      </FormLabel>
-      {tooltip}
+      <CFTooltip label={tooltip}>
+        <FormLabel
+          mb="0"
+          color={textColor}
+          fontSize={props.fontSize ?? "14px"}
+          htmlFor={hashId}
+          userSelect="none"
+          {...formLabelProps}>
+          {label}
+        </FormLabel>
+      </CFTooltip>
       <Spacer />
       <Switch
         id={hashId}
         sx={{
           "span.chakra-switch__track": { backgroundColor: checkedBgColor },
           "span.chakra-switch__track:not([data-checked])": { backgroundColor: uncheckedBgColor },
         }}
```

### Comparing `carefree-drawboard-0.0.0a9/cfdraw/.web/src/hooks/useFileDropper.ts` & `carefree-drawboard-0.0.1a0/cfdraw/.web/src/hooks/useFileDropper.ts`

 * *Files 8% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 import { toastWord } from "@/utils/toast";
 import { Toast_Words } from "@/lang/toast";
 import { BOARD_CONTAINER_ID } from "@/utils/constants";
 import { setDropping, hooksStore } from "@/stores/hooks";
 import { uploadImage } from "@/actions/uploadImage";
 import { importMeta } from "@/actions/importMeta";
+import { useIsSetup } from "./useSetup";
 
 export function useFileDropper(): void {
   function onDrop(): void {
     setDropping(true);
     setTimeout(() => {
       if (hooksStore.dropping) {
         toastWord("info", Toast_Words["dropping-message"]);
@@ -66,23 +67,27 @@
       if (res.reason) {
         toastWord("error", res.reason);
       }
     });
   }
 
   const dropPatience = 500;
+  const isReady = useIsReady();
+  const isSetup = useIsSetup();
 
   useEffect(() => {
+    if (!isReady || !isSetup) return;
+
     const dropper = new FileDropper({
       onDrop,
       onSuccess,
       onError,
       urlType: "dataUrl",
       listenTarget: document.getElementById(BOARD_CONTAINER_ID) as HTMLElement,
       bypassWHCheck: true,
     });
     dropper.init();
     return () => {
       dropper.destroy();
     };
-  }, [useIsReady()]);
+  }, [isReady, isSetup]);
 }
```

### Comparing `carefree-drawboard-0.0.0a9/cfdraw/.web/src/hooks/useGridLines.ts` & `carefree-drawboard-0.0.1a0/cfdraw/.web/src/hooks/useGridLines.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a9/cfdraw/.web/src/hooks/usePython.ts` & `carefree-drawboard-0.0.1a0/cfdraw/.web/src/plugins/utils/renderFilters.ts`

 * *Files 26% similar despite different names*

```diff
@@ -1,172 +1,146 @@
 import { useCallback } from "react";
 
-import type { ExportBlobOptions } from "@carefree0910/svg";
-import { BBox, INode, INodes, Logger } from "@carefree0910/core";
+import type { IResponse } from "@carefree0910/business";
+import { Dictionary, Logger, getHash, isUndefined, waitUntil } from "@carefree0910/core";
 
-import type { IMeta } from "@/schema/meta";
-import type {
-  INodeData,
-  IPythonSocketRequest,
-  IUsePythonInfo,
-  IUseSocketPython,
-  IPythonOnSocketMessage,
-} from "@/schema/_python";
-import { userStore } from "@/stores/user";
-import { debugStore } from "@/stores/debug";
-import { IPythonStore, updatePythonStore } from "@/stores/_python";
-import { useWebSocketHook } from "@/requests/hooks";
-import { uploadImage } from "@/actions/uploadImage";
-import { Exporter } from "@/actions/export";
-
-type IGetNodeData = ExportBlobOptions & { exportBox: BBox };
-async function getNodeData(node: INode | null, opt: IGetNodeData): Promise<INodeData> {
-  if (!node) return {};
-  const { x, y } = node.position;
-  const { w, h } = node.wh;
-  const transform = node.transform.fields;
-  const text = node.type === "text" ? node.params.content : undefined;
-  let src: string | undefined = undefined;
-  if (node.type === "image") {
-    src = node.renderParams.src;
-  } else if (node.type === "path") {
-    // should export the `PathNode` as an image based on the `exportBox`
-    opt.exportOptions ??= {};
-    opt.exportOptions.exportBox = opt.exportBox;
-    src = await Exporter.exportBlob([node], opt)
-      .then((blob) => {
-        if (!blob) throw Error("export blob for `PathNode` failed");
-        return uploadImage(blob, { failed: async () => void 0 });
-      })
-      .then((res) => {
-        if (!res) throw Error("upload image for `PathNode` failed");
-        return res.url;
-      });
+import type { IPythonSocketMessage, IPythonSocketRequest } from "@/schema/_python";
+import type { NodeConstraintSettings } from "@/schema/plugins";
+import { runOneTimeSocketHook } from "@/stores/socket";
+import { getPythonRequest } from "@/hooks/usePython";
+
+function checkConstraint(
+  constraint: NodeConstraintSettings["nodeConstraint"],
+  info?: IResponse,
+): boolean {
+  if (!constraint || constraint === "none") return true;
+  if (!info) return false;
+  if (constraint === "anyNode") return info.type !== "none";
+  if (constraint === "multiNode") return info.type === "multiple";
+  if (constraint === "singleNode") return !["group", "multiple", "none"].includes(info.type);
+  return info.type === constraint;
+}
+async function checkRules(
+  rules: NodeConstraintSettings["nodeConstraintRules"],
+  info?: IResponse,
+): Promise<boolean> {
+  if (rules?.some) {
+    for (const nodeConstraint of rules.some) {
+      if (await useNodeFilter({ nodeConstraint })(info)) return true;
+    }
+    return false;
   }
-  const meta = (node.type === "group" ? undefined : node.params.meta) as IMeta | undefined;
-  const children = node.type === "group" ? await getNodeDataList(node.nodes, opt) : undefined;
-  return { type: node.type, x, y, w, h, transform, text, src, meta, children };
-}
-async function getNodeDataList(nodes: INode[], opt: IGetNodeData): Promise<INodeData[]> {
-  return Promise.all(nodes.map((node) => getNodeData(node, opt)));
-}
-async function getPythonRequest({
-  node,
-  nodes,
-  identifier,
-  getExtraRequestData,
-  opt,
-}: Omit<IUsePythonInfo, "isInvisible"> & {
-  opt: ExportBlobOptions;
-}): Promise<Omit<IPythonSocketRequest, "hash">> {
-  const exportBox = new INodes(nodes).bbox;
-  const getNodeDataOpt: IGetNodeData = { exportBox, ...opt };
-  const nodeData = await getNodeData(node, getNodeDataOpt);
-  const nodeDataList = nodes.length <= 1 ? [] : await getNodeDataList(nodes, getNodeDataOpt);
-  return {
-    userId: userStore.userId,
-    identifier,
-    nodeData,
-    nodeDataList,
-    extraData: getExtraRequestData ? getExtraRequestData() : {},
-  };
+  if (rules?.every) {
+    for (const nodeConstraint of rules.every) {
+      if (!(await useNodeFilter({ nodeConstraint })(info))) return false;
+    }
+    return true;
+  }
+  if (rules?.exactly) {
+    if (!info) return false;
+    if (info.nodes.length !== rules.exactly.length) return false;
+    const selectedNodes = info.nodes.map((node) => node.type);
+    for (const nodeConstraint of rules.exactly) {
+      let searched = false;
+      for (let i = 0; i < selectedNodes.length; i++) {
+        if (selectedNodes[i] === nodeConstraint) {
+          selectedNodes.splice(i, 1);
+          searched = true;
+          break;
+        }
+      }
+      if (!searched) return false;
+    }
+  }
+  return true;
 }
-
-export function useSocketPython<R>({
-  hash,
-  node,
-  nodes,
-  identifier,
-  isInvisible,
-  retryInterval,
-  updateInterval,
-  getExtraRequestData,
-  onMessage,
-  onSocketError,
-}: IUseSocketPython<R>) {
-  const deps = [
-    hash,
-    node?.alias,
-    nodes.map((n) => n.alias).join("_"),
-    identifier,
-    retryInterval,
-    updateInterval,
-    isInvisible,
-    getExtraRequestData,
-  ];
-
-  const getMessage = useCallback(
-    () =>
-      getPythonRequest({
-        node,
-        nodes,
-        identifier,
-        getExtraRequestData,
-        opt: {},
-      }).then((req) => ({ hash: hash!, ...req })),
-    [deps],
-  );
-
-  const requestFn = useCallback(() => {
-    useWebSocketHook({
-      isInvisible,
-      hash,
-      getMessage,
-      onMessage,
-      onSocketError,
-      retryInterval,
-      updateInterval,
-    });
-  }, [getMessage, onMessage, onSocketError]);
-
-  requestFn();
+interface IValidatorResponse {
+  acceptable: boolean;
 }
-
-export function useSyncPython() {
-  const hash = "0";
-  const getMessage = useCallback(
-    (): Promise<IPythonSocketRequest> =>
-      Promise.resolve({
+export function hashInfo(info?: IResponse): string {
+  if (!info) return "";
+  const node = info.displayNode?.alias ?? "";
+  const nodes = info.nodes.map((node) => node.alias).join(",");
+  const transform = JSON.stringify(info.displayNode?.transform.fields ?? {});
+  const transforms = info.nodes.map((node) => JSON.stringify(node.transform.fields)).join(",");
+  return getHash(`${node}-${nodes}-${transform}-${transforms}`).toString();
+}
+const working: Dictionary<boolean> = {};
+const results: Dictionary<boolean> = {};
+const clear = (hash: string) => {
+  setTimeout(() => {
+    delete results[hash];
+  }, 1000);
+};
+function checkValidator(validator?: string, info?: IResponse): Promise<boolean> {
+  if (isUndefined(validator)) return Promise.resolve(true);
+  return new Promise((resolve) => {
+    const hash = hashInfo(info);
+    if (!isUndefined(results[hash])) return resolve(results[hash]);
+    if (working[hash]) {
+      return waitUntil(() => !isUndefined(results[hash])).then(() => resolve(results[hash]));
+    }
+    working[hash] = true;
+    const getMessage = (): Promise<IPythonSocketRequest> => {
+      return getPythonRequest({
+        node: info?.displayNode ?? null,
+        nodes: info?.nodes ?? [],
+        identifier: "node_validator",
+        opt: { noExport: true },
+      }).then((data) => ({
+        ...data,
         hash,
-        userId: userStore.userId,
-        identifier: "sync",
-        nodeData: {},
-        nodeDataList: [],
-        extraData: {},
+        extraData: { key: validator },
         isInternal: true,
-      }),
-    [],
-  );
-  const onMessage = useCallback<IPythonOnSocketMessage<IPythonStore>>(
-    async ({ status, total, pending, message, data: { progress, final } }) => {
-      if (status !== "finished") {
-        if (status === "pending") {
-          Logger.warn(`sync pending: ${pending} / ${total}`);
-        } else if (status === "working") {
-          // Logger.warn(`sync in progress: ${progress}`);
-        } else {
-          Logger.warn(`sync failed: ${message}`);
-          return { newMessage: getMessage };
-        }
-        return {};
-      } else {
-        if (!final) {
-          Logger.warn("sync data not found");
-          return { newMessage: getMessage };
-        }
-        if (updatePythonStore(final)) {
-          Logger.log(`sync successfully: ${JSON.stringify(final)}, rerendering`);
-        }
-        return debugStore.pollSync ? { newMessage: getMessage } : {};
+      }));
+    };
+    const onMessage = async ({
+      status,
+      message,
+      data: { final },
+    }: IPythonSocketMessage<IValidatorResponse>) => {
+      delete working[hash];
+      if (status === "finished" && final) {
+        results[hash] = final.acceptable;
+        clear(hash);
+        resolve(final.acceptable);
+      } else if (status === "exception") {
+        Logger.warn(`execute node validator ${validator} failed: ${message}`);
+        resolve(false);
       }
-    },
-    [],
-  );
+      return {};
+    };
 
-  useWebSocketHook<IPythonStore>({
-    isInvisible: false,
-    hash,
-    getMessage,
-    onMessage,
-    isInternal: true,
+    runOneTimeSocketHook({
+      key: hash,
+      getMessage,
+      onMessage,
+      isInternal: true,
+    });
   });
 }
+export function useConstraintDeps(settings: NodeConstraintSettings) {
+  return [settings.nodeConstraint, settings.nodeConstraintRules, settings.nodeConstraintValidator];
+}
+export function useNodeFilter(
+  settings: NodeConstraintSettings,
+): (info?: IResponse) => Promise<boolean> {
+  return useCallback(async (info) => {
+    if (!checkConstraint(settings.nodeConstraint, info)) return false;
+    if (!(await checkRules(settings.nodeConstraintRules, info))) return false;
+    if (!(await checkValidator(settings.nodeConstraintValidator, info))) return false;
+    return true;
+  }, useConstraintDeps(settings));
+}
+
+export function checkHasConstraint({
+  nodeConstraint,
+  nodeConstraintRules,
+  nodeConstraintValidator,
+}: NodeConstraintSettings): boolean {
+  if (nodeConstraint && nodeConstraint !== "none") return true;
+  if (nodeConstraintRules?.some) return true;
+  if (nodeConstraintRules?.every) return true;
+  if (nodeConstraintRules?.exactly) return true;
+  if (!isUndefined(nodeConstraintValidator)) return true;
+  return false;
+}
```

### Comparing `carefree-drawboard-0.0.0a9/cfdraw/.web/src/lang/add.ts` & `carefree-drawboard-0.0.1a0/cfdraw/.web/src/lang/add.ts`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 import { Lang } from "@carefree0910/core";
 
 export enum Add_Words {
   "add-plugin-header" = "add-plugin-header",
   "new-project-button" = "new-project-button",
   "upload-image-button" = "upload-image-button",
   "add-text-button" = "add-text-button",
+  "add-blank-button" = "add-blank-button",
 }
 
 export const addLangRecords: Record<Lang, Record<Add_Words, string>> = {
   zh: {
     [Add_Words["add-plugin-header"]]: "添加",
     [Add_Words["new-project-button"]]: "新建项目",
     [Add_Words["upload-image-button"]]: "上传图片",
     [Add_Words["add-text-button"]]: "添加文字",
+    [Add_Words["add-blank-button"]]: "添加空白画布",
   },
   en: {
     [Add_Words["add-plugin-header"]]: "Add",
     [Add_Words["new-project-button"]]: "New Project",
     [Add_Words["upload-image-button"]]: "Upload Image",
     [Add_Words["add-text-button"]]: "Add Text",
+    [Add_Words["add-blank-button"]]: "Add Blank Canvas",
   },
 };
```

### Comparing `carefree-drawboard-0.0.0a9/cfdraw/.web/src/lang/brush.ts` & `carefree-drawboard-0.0.1a0/cfdraw/.web/src/lang/brush.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a9/cfdraw/.web/src/lang/download.ts` & `carefree-drawboard-0.0.1a0/cfdraw/.web/src/lang/download.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a9/cfdraw/.web/src/lang/index.ts` & `carefree-drawboard-0.0.1a0/cfdraw/.web/src/lang/index.ts`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,14 @@
   addLangRecords,
   downloadLangRecords,
   nodeEditorLangRecords,
   brushLangRecords,
 ];
 
 export function initializeLang(): void {
-  langStore.updateProperty("tgt", "en");
   const collected = new Set();
   let anyDuplicate = false;
   for (const lang of Object.keys(langDescriptions) as Lang[]) {
     initLangDirs.forEach((d) => {
       updateDictionary(lang, d[lang]);
       Object.keys(d[lang]).forEach((k) => {
         const _k = `${lang}-${k}`;
```

### Comparing `carefree-drawboard-0.0.0a9/cfdraw/.web/src/lang/plugins.ts` & `carefree-drawboard-0.0.1a0/cfdraw/.web/src/lang/plugins.ts`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,12 @@
 import { Dictionary, Lang } from "@carefree0910/core";
 
-import {
-  allAvailablePlugins,
-  allAvailablePythonPlugins,
-  AvailablePluginsAndPythonPlugins,
-} from "@/schema/plugins";
+import { allReactPlugins, allPythonPlugins, AllPlugins } from "@/schema/plugins";
 
-const _pluginsLangRecords: Record<Lang, Record<AvailablePluginsAndPythonPlugins, string>> = {
+const _pluginsLangRecords: Record<Lang, Record<AllPlugins, string>> = {
   zh: {
     meta: "元数据",
     settings: "设置",
     project: "项目",
     add: "添加",
     arrange: "智能整理",
     undo: "撤销",
@@ -20,17 +16,19 @@
     wiki: "文档",
     github: "Github",
     email: "邮件",
     textEditor: "编辑文本",
     groupEditor: "编辑组",
     multiEditor: "编辑多节点",
     brush: "画笔",
+    "_python.fields": "Python 插件",
     "_python.textArea": "Python 文本框",
     "_python.QA": "Python 问答",
-    "_python.fields": "Python 插件",
+    "_python.chat": "Python 对话",
+    "_python.pluginGroup": "Python 插件组",
   },
   en: {
     meta: "Meta",
     settings: "Settings",
     project: "Project",
     add: "Add",
     arrange: "Auto Arrange",
@@ -41,36 +39,38 @@
     wiki: "Wiki",
     github: "Github",
     email: "Email",
     textEditor: "Edit Text",
     groupEditor: "Edit Group",
     multiEditor: "Edit Multi Nodes",
     brush: "Brush",
+    "_python.fields": "Python Plugin",
     "_python.textArea": "Python TextArea",
     "_python.QA": "Python Q & A",
-    "_python.fields": "Python Plugin",
+    "_python.chat": "Python Chat",
+    "_python.pluginGroup": "Python Plugin Group",
   },
 };
 
-export const Plugins_Words: Record<AvailablePluginsAndPythonPlugins, string> = {} as any;
+export const Plugins_Words: Record<AllPlugins, string> = {} as any;
 export const pluginsLangRecords: Dictionary<Dictionary<string>> = {};
 
 function injectScope(scope: string, data: Dictionary<string>) {
   Object.entries(data).forEach(([key, value]) => {
     data[key] = `${scope}.${value}`;
   });
 }
 function reverseMapping(data: Dictionary<string>) {
   return Object.fromEntries(Object.entries(data).map(([key, value]) => [value, key]));
 }
 
-allAvailablePlugins.forEach((plugin) => {
+allReactPlugins.forEach((plugin) => {
   (Plugins_Words as any)[plugin] = plugin;
 });
-allAvailablePythonPlugins.forEach((plugin) => {
+allPythonPlugins.forEach((plugin) => {
   (Plugins_Words as any)[plugin] = plugin;
 });
 const scope = "plugins";
 injectScope(scope, Plugins_Words);
 Object.entries(_pluginsLangRecords).forEach(([lang, record]) => {
   const reversedRecord = reverseMapping(record);
   injectScope(scope, reversedRecord);
```

### Comparing `carefree-drawboard-0.0.0a9/cfdraw/.web/src/lang/projects.ts` & `carefree-drawboard-0.0.1a0/cfdraw/.web/src/lang/projects.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a9/cfdraw/.web/src/lang/settings.ts` & `carefree-drawboard-0.0.1a0/cfdraw/.web/src/lang/settings.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a9/cfdraw/.web/src/lang/toast.ts` & `carefree-drawboard-0.0.1a0/cfdraw/.web/src/lang/toast.ts`

 * *Files 20% similar despite different names*

```diff
@@ -12,30 +12,42 @@
   "uploading-project-message" = "uploading-project-message",
   "adding-project-message" = "adding-project-message",
   "add-project-success-message" = "add-project-success-message",
   "save-project-success-message" = "save-project-success-message",
   "save-project-error-message" = "save-project-error-message",
   "loading-project-message" = "loading-project-message",
   "load-project-success-message" = "load-project-success-message",
+  "load-project-error-message" = "load-project-error-message",
   "please-select-project-message" = "please-select-project-message",
+  "please-select-project-to-delete-message" = "please-select-project-to-delete-message",
+  "already-selected-project-message" = "already-selected-project-message",
+  "cannot-delete-auto-save-project-message" = "cannot-delete-auto-save-project-message",
   "downloading-project-message" = "downloading-project-message",
   "importing-local-project-message" = "importing-local-project-message",
   "import-local-project-success-message" = "import-local-project-success-message",
   "import-local-project-error-message" = "import-local-project-error-message",
+  "delete-project-success-message" = "delete-project-success-message",
+  "delete-project-error-message" = "delete-project-error-message",
   "add-text-success-message" = "add-text-success-message",
   "add-text-error-message" = "add-text-error-message",
+  "add-blank-success-message" = "add-blank-success-message",
+  "add-blank-error-message" = "add-blank-error-message",
   "auto-arrange-no-need-message" = "auto-arrange-no-need-message",
   "submit-task-busy-message" = "submit-task-busy-message",
   "submit-task-success-message" = "submit-task-success-message",
   "submit-task-error-message" = "submit-task-error-message",
+  "submit-task-interrupted-message" = "submit-task-interrupted-message",
   "submit-task-finished-message" = "submit-task-finished-message",
   "downloading-nodes-message" = "downloading-nodes-message",
   "export-blob-error-message" = "export-blob-error-message",
   "enter-brush-mode-message" = "enter-brush-mode-message",
   "exit-brush-mode-message" = "exit-brush-mode-message",
+  "nsfw-image-detected-warning-message" = "nsfw-image-detected-warning-message",
+  "no-overlapped-node-message" = "no-overlapped-node-message",
+  "returned-empty-text-message" = "returned-empty-text-message",
 }
 
 export const toastLangRecords: Record<Lang, Record<Toast_Words, string>> = {
   zh: {
     [Toast_Words["dropping-message"]]: "识别中",
     [Toast_Words["uploading-image-message"]]: "上传中，请稍候",
     [Toast_Words["upload-image-success-message"]]: "上传图片成功",
@@ -47,30 +59,42 @@
     [Toast_Words["uploading-project-message"]]: "保存项目中",
     [Toast_Words["adding-project-message"]]: "新建项目中",
     [Toast_Words["add-project-success-message"]]: "新建项目成功",
     [Toast_Words["save-project-success-message"]]: "保存项目成功",
     [Toast_Words["save-project-error-message"]]: "保存项目失败",
     [Toast_Words["loading-project-message"]]: "加载项目中，请稍候",
     [Toast_Words["load-project-success-message"]]: "加载项目成功",
+    [Toast_Words["load-project-error-message"]]: "加载项目失败",
     [Toast_Words["please-select-project-message"]]: "请先选择想要加载的项目",
+    [Toast_Words["please-select-project-to-delete-message"]]: "请先选择想要删除的项目",
+    [Toast_Words["already-selected-project-message"]]: "要加载的项目是当前的项目，无需重复加载",
+    [Toast_Words["cannot-delete-auto-save-project-message"]]: "不能删除「自动保存」项目",
     [Toast_Words["downloading-project-message"]]: "下载项目中",
     [Toast_Words["importing-local-project-message"]]: "导入中",
     [Toast_Words["import-local-project-success-message"]]: "导入成功",
     [Toast_Words["import-local-project-error-message"]]: "导入失败",
+    [Toast_Words["delete-project-success-message"]]: "删除项目成功",
+    [Toast_Words["delete-project-error-message"]]: "删除项目失败",
     [Toast_Words["add-text-success-message"]]: "添加文字成功",
     [Toast_Words["add-text-error-message"]]: "添加文字时出了些问题",
+    [Toast_Words["add-blank-success-message"]]: "添加空白画布成功",
+    [Toast_Words["add-blank-error-message"]]: "添加空白画布时出了些问题",
     [Toast_Words["auto-arrange-no-need-message"]]: "当前节点无需整理",
     [Toast_Words["submit-task-busy-message"]]: "当前任务正在执行中，请稍候...",
     [Toast_Words["submit-task-success-message"]]: "任务提交成功",
     [Toast_Words["submit-task-error-message"]]: "执行任务时出了些问题",
+    [Toast_Words["submit-task-interrupted-message"]]: "任务执行被中断",
     [Toast_Words["submit-task-finished-message"]]: "任务已执行完成",
     [Toast_Words["downloading-nodes-message"]]: "下载中",
     [Toast_Words["export-blob-error-message"]]: "导出节点时出了些问题",
     [Toast_Words["enter-brush-mode-message"]]: "已进入涂鸦模式",
     [Toast_Words["exit-brush-mode-message"]]: "已退出涂鸦模式",
+    [Toast_Words["nsfw-image-detected-warning-message"]]: "检测到图片中可能包含敏感内容",
+    [Toast_Words["no-overlapped-node-message"]]: "当前空白画布上没有内容",
+    [Toast_Words["returned-empty-text-message"]]: "返回的文本内容为空",
   },
   en: {
     [Toast_Words["dropping-message"]]: "Detecting",
     [Toast_Words["uploading-image-message"]]: "Uploading, please wait for a while",
     [Toast_Words["upload-image-success-message"]]: "Image uploaded successfully!",
     [Toast_Words["upload-image-error-message"]]: "Upload image failed",
     [Toast_Words["strange-image-error-message"]]: "Only jpg/png images are supported",
@@ -80,26 +104,39 @@
     [Toast_Words["uploading-project-message"]]: "Saving",
     [Toast_Words["adding-project-message"]]: "Creating new project",
     [Toast_Words["add-project-success-message"]]: "Project created successfully!",
     [Toast_Words["save-project-success-message"]]: "Project saved successfully!",
     [Toast_Words["save-project-error-message"]]: "Save project failed",
     [Toast_Words["loading-project-message"]]: "Loading",
     [Toast_Words["load-project-success-message"]]: "Project loaded successfully!",
+    [Toast_Words["load-project-error-message"]]: "Load project failed",
     [Toast_Words["please-select-project-message"]]: "Please select a project first",
+    [Toast_Words["please-select-project-to-delete-message"]]: "Please select a project to delete",
+    [Toast_Words["already-selected-project-message"]]:
+      "The project you want to load is the current project, no need to load again",
+    [Toast_Words["cannot-delete-auto-save-project-message"]]: "Cannot delete 'Auto Save' project",
     [Toast_Words["downloading-project-message"]]: "Downloading",
     [Toast_Words["importing-local-project-message"]]: "Importing",
     [Toast_Words["import-local-project-success-message"]]: "Imported successfully!",
     [Toast_Words["import-local-project-error-message"]]: "Import failed",
+    [Toast_Words["delete-project-success-message"]]: "Project deleted successfully!",
+    [Toast_Words["delete-project-error-message"]]: "Delete project failed",
     [Toast_Words["add-text-success-message"]]: "Text added successfully",
     [Toast_Words["add-text-error-message"]]: "Something is wrong when adding Text Node",
+    [Toast_Words["add-blank-success-message"]]: "Blank Canvas added successfully",
+    [Toast_Words["add-blank-error-message"]]: "Something is wrong when adding Blank Canvas",
     [Toast_Words["auto-arrange-no-need-message"]]: "There is no need to arrange the Nodes",
     [Toast_Words["submit-task-busy-message"]]:
       "Current task is being executed, please wait for a while...",
     [Toast_Words["submit-task-success-message"]]: "Task submitted successfully!",
     [Toast_Words["submit-task-error-message"]]: "Something is wrong when executing the task",
+    [Toast_Words["submit-task-interrupted-message"]]: "Task submission is interrupted",
     [Toast_Words["submit-task-finished-message"]]: "Task has been executed successfully",
     [Toast_Words["downloading-nodes-message"]]: "Downloading",
     [Toast_Words["export-blob-error-message"]]: "Something is wrong when exporting Node",
     [Toast_Words["enter-brush-mode-message"]]: "Entered sketch mode",
     [Toast_Words["exit-brush-mode-message"]]: "Exited sketch mode",
+    [Toast_Words["nsfw-image-detected-warning-message"]]: "NSFW image detected",
+    [Toast_Words["no-overlapped-node-message"]]: "Cannot detect anything on current Blank Canvas",
+    [Toast_Words["returned-empty-text-message"]]: "Returned text is empty",
   },
 };
```

### Comparing `carefree-drawboard-0.0.0a9/cfdraw/.web/src/lang/tooltip.ts` & `carefree-drawboard-0.0.1a0/cfdraw/.web/src/lang/tooltip.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a9/cfdraw/.web/src/plugins/_python/PluginWithSubmit.tsx` & `carefree-drawboard-0.0.1a0/cfdraw/.web/src/plugins/_python/PluginWithSubmit.tsx`

 * *Files 16% similar despite different names*

```diff
@@ -1,63 +1,96 @@
 import { useCallback, useEffect, useState } from "react";
 import { observer } from "mobx-react-lite";
 
+import { isUndefined } from "@carefree0910/core";
 import { langStore, translate } from "@carefree0910/business";
 
 import type { IPythonSocketPluginWithSubmit } from "@/schema/_python";
 import { Event } from "@/utils/event";
 import { toast } from "@/utils/toast";
 import { Toast_Words } from "@/lang/toast";
-import { userStore } from "@/stores/user";
-import { getPluginHash } from "@/stores/plugins";
+import {
+  usePluginHash,
+  setPluginExpanded,
+  usePluginTaskCache,
+  setPluginTaskCache,
+} from "@/stores/pluginsInfo";
 import { useSocketPython } from "@/hooks/usePython";
+import { parseIStr } from "@/actions/i18n";
 import { CFButtonWithBusyTooltip } from "@/components/CFButton";
 import CFDivider from "@/components/CFDivider";
 import Render from "../components/Render";
-import { floatingControlEvent } from "../components/Floating";
+import { useCurrentMeta, useOnMessage } from "./hooks";
 
 export const socketFinishedEvent = new Event<{ id: string }>();
-function PythonPluginWithSubmit<R>({
+function PythonPluginWithSubmit({
   id,
-  pluginInfo: {
+  pluginInfo,
+  buttonText,
+  beforeSubmit,
+  afterSubmit,
+  onIntermediate,
+  onFinished,
+  onSocketError,
+  getExtraRequestData,
+  children,
+  ...props
+}: IPythonSocketPluginWithSubmit) {
+  const {
     node,
     nodes,
     identifier,
     retryInterval,
     updateInterval,
     closeOnSubmit = true,
     toastOnSubmit = true,
     toastMessageOnSubmit,
-  },
-  buttonText,
-  onMessage,
-  onSocketError,
-  getExtraRequestData,
-  children,
-  ...props
-}: IPythonSocketPluginWithSubmit<R>) {
+  } = pluginInfo;
   const lang = langStore.tgt;
   const [hash, setHash] = useState<string | undefined>(undefined);
   const [busy, setBusy] = useState(false);
+  const taskCache = usePluginTaskCache(id);
+  const currentMeta = useCurrentMeta(node, nodes);
   const onClick = useCallback(() => {
     if (busy) return;
-    if (!userStore.canAlwaysSubmit) {
-      setBusy(true);
+    beforeSubmit?.();
+    setBusy(true);
+    setHash(usePluginHash(id));
+    if (!taskCache) {
+      setPluginTaskCache(id, { currentMeta, parameters: getExtraRequestData?.() ?? {} });
     }
-    setHash(getPluginHash(id));
     if (closeOnSubmit) {
-      floatingControlEvent.emit({ id, expand: false });
+      if (isUndefined(props.groupId)) {
+        setPluginExpanded(id, false);
+      } else {
+        setPluginExpanded(props.groupId, true);
+      }
     }
     if (toastOnSubmit) {
-      toastMessageOnSubmit ??= translate(Toast_Words["submit-task-success-message"], lang);
-      toast("info", toastMessageOnSubmit);
+      toast(
+        "info",
+        parseIStr(
+          toastMessageOnSubmit ?? translate(Toast_Words["submit-task-success-message"], lang),
+        ),
+      );
     }
-  }, [id, lang, closeOnSubmit, toastOnSubmit, toastMessageOnSubmit, busy]);
+    afterSubmit?.();
+  }, [
+    id,
+    lang,
+    closeOnSubmit,
+    toastOnSubmit,
+    toastMessageOnSubmit,
+    busy,
+    currentMeta,
+    getExtraRequestData,
+  ]);
+  const onMessage = useOnMessage({ id, pluginInfo, onIntermediate, onFinished });
 
-  useSocketPython<R>({
+  useSocketPython({
     hash,
     node,
     nodes,
     identifier,
     isInvisible: props.renderInfo.isInvisible ?? false,
     retryInterval,
     updateInterval,
```

### Comparing `carefree-drawboard-0.0.0a9/cfdraw/.web/src/plugins/_python/QAPlugin.tsx` & `carefree-drawboard-0.0.1a0/cfdraw/.web/src/plugins/_python/ChatPlugin.tsx`

 * *Files 15% similar despite different names*

```diff
@@ -1,53 +1,60 @@
 import { useCallback, useState } from "react";
 import { observer } from "mobx-react-lite";
 import { Textarea } from "@chakra-ui/react";
 
 import { langStore, translate } from "@carefree0910/business";
 
-import type { IPythonOnSocketMessage, IPythonQAPlugin } from "@/schema/_python";
+import type { OnPythonPluginMessage, IPythonQAPlugin } from "@/schema/_python";
 import { UI_Words } from "@/lang/ui";
-import { getPluginIds } from "@/stores/plugins";
+import { usePluginIds } from "@/stores/pluginsInfo";
+import { parseIStr } from "@/actions/i18n";
 import CFInput from "@/components/CFInput";
 import { drawboardPluginFactory } from "@/plugins/utils/factory";
 import PythonPluginWithSubmit from "./PluginWithSubmit";
 
-const PythonQAPlugin = ({ pluginInfo, ...props }: IPythonQAPlugin) => {
-  const { id } = getPluginIds(`QA_${pluginInfo.identifier}`);
+const PythonChatPlugin = ({ pluginInfo, ...props }: IPythonQAPlugin) => {
+  const { id } = usePluginIds(`Chat_${pluginInfo.identifier}`);
+  const [context, setContext] = useState(parseIStr(pluginInfo.initialText));
   const [userInput, setUserInput] = useState("");
-  const [serverText, setServerText] = useState(pluginInfo.initialText);
   const lang = langStore.tgt;
-  const getExtraRequestData = useCallback(() => ({ text: userInput }), [userInput]);
-  const onMessage = useCallback<IPythonOnSocketMessage<{ text: string }>>(
-    async ({ status, data }) => {
-      if (status === "finished") {
-        setServerText(data.final?.text ?? "");
-      } else {
-        setServerText("Thinking...");
+  const getExtraRequestData = useCallback(() => ({ context, userInput }), [context, userInput]);
+  const onIntermediate = useCallback<OnPythonPluginMessage>(
+    async ({ data: { intermediate } }) => {
+      if (intermediate?.textList?.length) {
+        setContext(intermediate.textList[0]);
       }
-      return {};
     },
-    [setServerText],
+    [setContext],
+  );
+  const onFinished = useCallback<OnPythonPluginMessage>(
+    async ({ data: { final } }) => {
+      if (final?.type === "text") {
+        setContext(final.value[0].text);
+      }
+    },
+    [setContext],
   );
 
   return (
     <PythonPluginWithSubmit
       id={id}
       buttonText={translate(UI_Words["submit-task"], lang)}
       getExtraRequestData={getExtraRequestData}
-      onMessage={onMessage}
+      onIntermediate={onIntermediate}
+      onFinished={onFinished}
       pluginInfo={pluginInfo}
       {...props}>
-      <Textarea w="100%" h="40%" minH="0px" value={serverText} readOnly />
+      <Textarea w="100%" flex={1} minH="0px" value={context} readOnly />
       <CFInput
         w="100%"
-        h="30%"
+        h="42px"
         mt="16px"
         value={userInput}
         onChange={(event) => setUserInput(event.target.value)}
-        placeholder={translate(UI_Words["qa-field-placeholder"], lang)}
+        placeholder={translate(UI_Words["chat-field-placeholder"], lang)}
       />
     </PythonPluginWithSubmit>
   );
 };
 
-drawboardPluginFactory.registerPython("_python.QA", true)(observer(PythonQAPlugin));
+drawboardPluginFactory.registerPython("_python.chat", true)(observer(PythonChatPlugin));
```

### Comparing `carefree-drawboard-0.0.0a9/cfdraw/.web/src/plugins/_python/TextAreaPlugin.tsx` & `carefree-drawboard-0.0.1a0/cfdraw/.web/src/plugins/_python/TextAreaPlugin.tsx`

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,50 @@
-import { useCallback, useMemo, useState } from "react";
+import { useCallback, useEffect, useState } from "react";
 import { observer } from "mobx-react-lite";
 import { Textarea } from "@chakra-ui/react";
 
 import { getRandomHash } from "@carefree0910/core";
 
-import type { IPythonTextAreaPlugin, IPythonOnSocketMessage } from "@/schema/_python";
-import { getPluginIds } from "@/stores/plugins";
+import type { IPythonTextAreaPlugin, OnPythonPluginMessage } from "@/schema/_python";
+import { usePluginIds, usePluginNeedRender } from "@/stores/pluginsInfo";
 import { useSocketPython } from "@/hooks/usePython";
 import { drawboardPluginFactory } from "@/plugins/utils/factory";
 import Render from "@/plugins/components/Render";
+import { socketFinishedEvent } from "./PluginWithSubmit";
+import { useOnMessage } from "./hooks";
 
-const PythonTextAreaPlugin = ({
-  pluginInfo: { node, nodes, identifier, retryInterval, updateInterval, noLoading, textAlign },
-  ...props
-}: IPythonTextAreaPlugin) => {
-  const id = getPluginIds(`textArea_${identifier}`);
-  const hash = useMemo(() => getRandomHash().toString(), [id]);
+const PythonTextAreaPlugin = ({ pluginInfo, ...props }: IPythonTextAreaPlugin) => {
+  const { node, nodes, identifier, retryInterval, updateInterval, noLoading, textAlign } =
+    pluginInfo;
+  const { id } = usePluginIds(`textArea_${identifier}`);
+  const needRender = usePluginNeedRender(id);
+  const [hash, setHash] = useState<string | undefined>(undefined);
+  useEffect(() => {
+    if (needRender) {
+      setHash(getRandomHash().toString());
+    }
+  }, [needRender]);
+  useEffect(() => {
+    const { dispose } = socketFinishedEvent.on(({ id: incomingId }) => {
+      if (incomingId === id) {
+        setHash(undefined);
+      }
+    });
+    return dispose;
+  }, [id, setHash]);
   const [value, setValue] = useState("");
-  const onMessage = useCallback<IPythonOnSocketMessage<{ text: string }>>(
-    async ({ status, data }) => {
-      if (status === "finished") {
-        setValue(data.final?.text ?? "");
-      } else if (!noLoading) {
-        setValue("Loading...");
+  const onFinished = useCallback<OnPythonPluginMessage>(
+    async ({ data: { final } }) => {
+      if (final?.type === "text") {
+        setValue(final.value[0].text);
       }
-      return {};
     },
     [setValue],
   );
+  const onMessage = useOnMessage({ id, pluginInfo, onFinished });
 
   useSocketPython({
     hash,
     node,
     nodes,
     identifier,
     isInvisible: props.renderInfo.isInvisible ?? false,
```

### Comparing `carefree-drawboard-0.0.0a9/cfdraw/.web/src/plugins/_react/ArrangePlugin.tsx` & `carefree-drawboard-0.0.1a0/cfdraw/.web/src/plugins/_react/ArrangePlugin.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a9/cfdraw/.web/src/plugins/_react/BrushPlugin.tsx` & `carefree-drawboard-0.0.1a0/cfdraw/.web/src/plugins/_react/BrushPlugin.tsx`

 * *Files 6% similar despite different names*

```diff
@@ -14,22 +14,22 @@
 import type { ICommonMetaData, IMeta } from "@/schema/meta";
 import type { IPlugin } from "@/schema/plugins";
 import { toastWord } from "@/utils/toast";
 import { Brush_Words } from "@/lang/brush";
 import { Toast_Words } from "@/lang/toast";
 import { themeStore } from "@/stores/theme";
 import { VisibleManager, uiStore } from "@/stores/ui";
+import { setPluginExpanded } from "@/stores/pluginsInfo";
 import { hideAllPlugins } from "@/actions/managePlugins";
 import CFButton from "@/components/CFButton";
 import CFSlider from "@/components/CFSlider";
 import CFSwitch from "@/components/CFSwitch";
 import CFDivider from "@/components/CFDivider";
 import CFHeading from "@/components/CFHeading";
 import { drawboardPluginFactory } from "../utils/factory";
-import { floatingControlEvent } from "../components/Floating";
 import Render from "../components/Render";
 
 const useSwitchBrushMode = () => async (): Promise<void> => {
   const { defaultBrushStyles } = themeStore.styles;
   const previousInBrushMode = toolbarStore.inBrushMode;
   // handle drawboard
   if (!previousInBrushMode) {
@@ -105,30 +105,30 @@
   const options = toolbarStore.allBrushOptions;
   const inBrushMode = toolbarStore.inBrushMode;
   const switchBrushMode = useSwitchBrushMode();
   const optionsList = !options ? [] : Array.isArray(options) ? options : [options];
 
   useEffect(() => {
     if (inBrushMode) {
-      floatingControlEvent.emit({ id, expand: true });
+      setPluginExpanded(id, true);
     }
-  });
+  }, [inBrushMode]);
 
   return (
     <Render id={id} onFloatingButtonClick={switchBrushMode} {...props}>
       <CFHeading>{translate(Brush_Words["brush-plugin-header"], lang)}</CFHeading>
       <CFDivider />
       {optionsList.map((opt, i) => (
         <SingleBrushEditor key={`brush-${i}`} pathIndex={i} options={opt} />
       ))}
       <CFDivider my="16px" />
       <CFButton
         isDisabled={!inBrushMode}
         onClick={() => {
-          floatingControlEvent.emit({ id, expand: false });
+          setPluginExpanded(id, false);
           switchBrushMode();
         }}>
         {translate(Brush_Words["finish-brush-message"], lang)}
       </CFButton>
     </Render>
   );
 };
```

### Comparing `carefree-drawboard-0.0.0a9/cfdraw/.web/src/plugins/_react/DeletePlugin.tsx` & `carefree-drawboard-0.0.1a0/cfdraw/.web/src/plugins/_react/DeletePlugin.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a9/cfdraw/.web/src/plugins/_react/DownloadPlugin.tsx` & `carefree-drawboard-0.0.1a0/cfdraw/.web/src/plugins/_react/DownloadPlugin.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a9/cfdraw/.web/src/plugins/_react/GroupPlugin.tsx` & `carefree-drawboard-0.0.1a0/cfdraw/.web/src/plugins/_react/GroupPlugin.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a9/cfdraw/.web/src/plugins/_react/LinksPlugin.tsx` & `carefree-drawboard-0.0.1a0/cfdraw/.web/src/plugins/_react/LinksPlugin.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a9/cfdraw/.web/src/plugins/_react/MetaPlugin.tsx` & `carefree-drawboard-0.0.1a0/cfdraw/.web/src/plugins/_react/MetaPlugin.tsx`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import { observer } from "mobx-react-lite";
 import { Textarea } from "@chakra-ui/react";
 
 import { useSelecting } from "@carefree0910/business";
 
 import type { IPlugin } from "@/schema/plugins";
 import { IMeta, getMetaTrace } from "@/schema/meta";
-import { getPluginIds } from "@/stores/plugins";
+import { usePluginIds } from "@/stores/pluginsInfo";
 import { drawboardPluginFactory } from "../utils/factory";
 import Render from "../components/Render";
 
 function getMetaRepresentation(meta: IMeta): string {
   const { type, data } = meta;
   if (type.startsWith("python.")) {
     return data.identifier ?? "unknown";
   }
   return type;
 }
 
 const MetaPlugin = ({ pluginInfo, ...others }: IPlugin) => {
-  const { id } = getPluginIds("meta");
+  const { id } = usePluginIds("meta");
   const info = useSelecting("raw");
   if (!info || info.type === "group" || info.type === "multiple") return null;
   const _meta = info.displayNode?.params.meta;
   if (!_meta) return null;
   const meta = _meta as IMeta;
   const history = getMetaTrace(meta).reverse().map(getMetaRepresentation).join(" -> ");
```

### Comparing `carefree-drawboard-0.0.0a9/cfdraw/.web/src/plugins/_react/ProjectPlugin.tsx` & `carefree-drawboard-0.0.1a0/cfdraw/.web/src/plugins/_react/ProjectPlugin.tsx`

 * *Files 26% similar despite different names*

```diff
@@ -1,150 +1,221 @@
 import Upload from "rc-upload";
 import { observer } from "mobx-react-lite";
 import { useMemo, useState, useEffect, useCallback } from "react";
-import { Flex } from "@chakra-ui/react";
+import { Box, Flex, Image } from "@chakra-ui/react";
 
-import { Dictionary, Graph, INodePack, getRandomHash } from "@carefree0910/core";
+import { Dictionary, Graph, INodePack, Logger, getRandomHash } from "@carefree0910/core";
 import { langStore, translate, useSafeExecute } from "@carefree0910/business";
 
 import type { IPlugin } from "@/schema/plugins";
+import DeleteIcon from "@/assets/icons/delete.svg";
 import { toastWord } from "@/utils/toast";
+import { globalEvent } from "@/utils/event";
 import { Toast_Words } from "@/lang/toast";
 import { Projects_Words } from "@/lang/projects";
-import { setCurrentProjectName, useCurrentProject } from "@/stores/projects";
+import { userStore } from "@/stores/user";
 import {
-  ILoadedProject,
-  fetchAllProjects,
+  IProjectsStore,
+  getNewProjectInfo,
+  getTimeString,
+  setCurrentProjectName,
+  updateCurrentProjectInfo,
+  useCurrentProjectInfo,
+} from "@/stores/projects";
+import { usePluginIsExpanded } from "@/stores/pluginsInfo";
+import {
+  AUTO_SAVE_PREFIX,
+  IProject,
+  deleteProject,
+  getAllProjectInfo,
+  getProject,
   loadProject,
+  saveCurrentProject,
   saveProject,
 } from "@/actions/manageProjects";
 import { downloadCurrentFullProject } from "@/actions/download";
 import CFText from "@/components/CFText";
 import CFInput from "@/components/CFInput";
 import CFButton from "@/components/CFButton";
 import CFDivider from "@/components/CFDivider";
 import CFHeading from "@/components/CFHeading";
 import { CFSrollableSelect } from "@/components/CFSelect";
 import { drawboardPluginFactory } from "../utils/factory";
-import { floatingEvent, floatingRenderEvent } from "../components/Floating";
 import { useClosePanel } from "../components/hooks";
 import Render from "../components/Render";
 
-type IImportLocal = ILoadedProject | INodePack[];
+type IImportLocal = IProject | INodePack[];
+
 const ProjectPlugin = ({ pluginInfo, ...props }: IPlugin) => {
   const id = useMemo(() => `project_${getRandomHash()}`, []);
   const lang = langStore.tgt;
-  const { uid, name } = useCurrentProject();
+  const userId = userStore.userId;
+  const expand = usePluginIsExpanded(id);
+  const { uid, name } = useCurrentProjectInfo();
   const [selectedUid, setSelectedUid] = useState("");
   const [userInputName, setUserInputName] = useState(name);
-  const [allProjects, setAllProjects] = useState<Dictionary<string> | undefined>();
-  const allProjectUids = useMemo(() => Object.keys(allProjects ?? {}), [allProjects]);
+  const [allUid2Name, setAllUid2Name] = useState<Dictionary<string> | undefined>();
+  const allProjectUids = useMemo(() => Object.keys(allUid2Name ?? {}), [allUid2Name]);
+  const isSelectingAutoSave = useMemo(
+    () => selectedUid.startsWith(AUTO_SAVE_PREFIX),
+    [selectedUid],
+  );
+  const getLoadUid = useCallback(() => {
+    if (!isSelectingAutoSave) return Promise.resolve(selectedUid);
+    // should create a new project when loading auto save project
+    return getProject(selectedUid).then((autoSaveProject) => {
+      const newProject = getNewProjectInfo();
+      newProject.name = `From Auto Save ${getTimeString(Date.now())}`;
+      return saveProject(
+        { userId, ...autoSaveProject, ...newProject },
+        async () => void 0,
+        true,
+      ).then(() => {
+        updateCurrentProjectInfo(newProject);
+        updateProjectStates(newProject);
+        return newProject.uid;
+      });
+    });
+  }, [userId, selectedUid]);
 
   const updateUids = useCallback(() => {
-    fetchAllProjects().then((projects) => {
-      projects ??= [];
-      const uid2name = projects.reduce((acc, { uid, name }) => {
-        acc[uid] = name;
-        return acc;
-      }, {} as Dictionary<string>);
-      setAllProjects(uid2name);
-      if (!!uid2name[uid]) {
-        setSelectedUid(uid);
-      }
-    });
+    getAllProjectInfo()
+      .then((projects) => {
+        projects ??= [];
+        const uid2name = projects.reduce((acc, { uid, name }) => {
+          acc[uid] = name;
+          return acc;
+        }, {} as Dictionary<string>);
+        setAllUid2Name(uid2name);
+        if (!!uid2name[uid]) {
+          setSelectedUid(uid);
+        }
+      })
+      .catch((err) => {
+        Logger.warn(`[ProjectPlugin] updateUids failed: ${err}, retrying...`);
+        setTimeout(updateUids, 1000);
+      });
   }, []);
 
   useEffect(() => {
-    const { dispose: floatingDispose } = floatingEvent.on(({ type }) => {
+    const { dispose } = globalEvent.on(({ type }) => {
       if (type === "newProject") {
-        const { uid, name } = useCurrentProject();
-        updateProjectStates(uid, name);
+        updateProjectStates(useCurrentProjectInfo());
       }
     });
-    const { dispose: floatingRenderDispose } = floatingRenderEvent.on(
-      ({ id: incomingId, expand }) => {
-        if (id === incomingId && expand) updateUids();
-      },
-    );
-
-    return () => {
-      floatingDispose();
-      floatingRenderDispose();
-    };
+    return dispose;
   }, [id]);
 
+  useEffect(() => {
+    if (expand) {
+      updateUids();
+    }
+  }, [expand]);
+
   const closePanel = useClosePanel(id);
-  function updateProjectStates(uid: string, name: string) {
+  function updateProjectStates({ uid, name }: IProjectsStore) {
     setSelectedUid(uid);
     setUserInputName(name);
   }
 
   function onRenameProject() {
     setCurrentProjectName(userInputName);
     onSaveProject();
     closePanel();
   }
   function onSaveProject() {
-    saveProject(async () => {
+    saveCurrentProject(async () => {
       toastWord("success", Toast_Words["save-project-success-message"]);
       updateUids();
       closePanel();
     });
   }
-  async function onLoadProjectSuccess(res: ILoadedProject) {
-    updateProjectStates(res.uid, res.name);
+  async function onLoadProjectSuccess(project: IProject) {
+    updateProjectStates(project);
     toastWord("success", Toast_Words["load-project-success-message"]);
     closePanel();
   }
   function onLoadProject() {
     if (!selectedUid) {
       toastWord("warning", Toast_Words["please-select-project-message"]);
       return;
     }
-    loadProject(selectedUid, onLoadProjectSuccess);
+    if (selectedUid === uid) {
+      toastWord("info", Toast_Words["already-selected-project-message"]);
+      return;
+    }
+    getLoadUid()
+      .then((uid) => loadProject(uid, onLoadProjectSuccess))
+      .catch((err) =>
+        toastWord("error", Toast_Words["load-project-error-message"], { appendix: ` - ${err}` }),
+      );
   }
   function onDownloadProject(): void {
     downloadCurrentFullProject();
     closePanel();
   }
-  function onImportLocalProject(res: IImportLocal) {
+  function onImportLocalProject(data: IImportLocal) {
     toastWord("info", Toast_Words["importing-local-project-message"]);
-    if ((res as ILoadedProject).uid) {
-      res = (res as ILoadedProject).graphInfo;
+    if (!Array.isArray(data)) {
+      data = data.graphInfo;
     }
-    const json = Graph.fromJsonInfo(res as INodePack[])
+    const json = Graph.fromJsonInfo(data as INodePack[])
       .clone()
       .toJson();
     useSafeExecute("addGraph", null, true, {
       success: async () => {
         toastWord("success", Toast_Words["import-local-project-success-message"]);
         closePanel();
       },
       failed: async () => toastWord("error", Toast_Words["import-local-project-error-message"]),
     })({ json });
   }
+  function onDeleteProject() {
+    if (!selectedUid) {
+      toastWord("warning", Toast_Words["please-select-project-to-delete-message"]);
+      return;
+    }
+    if (isSelectingAutoSave) {
+      toastWord("warning", Toast_Words["cannot-delete-auto-save-project-message"]);
+      return;
+    }
+    deleteProject(selectedUid)
+      .then(() => {
+        toastWord("success", Toast_Words["delete-project-success-message"]);
+        updateUids();
+      })
+      .catch((err) =>
+        toastWord("error", Toast_Words["delete-project-error-message"], { appendix: ` - ${err}` }),
+      );
+  }
 
   return (
     <Render id={id} {...props}>
       <Flex w="100%" h="100%" direction="column">
         <CFHeading>{translate(Projects_Words["project-plugin-header"], lang)}</CFHeading>
         <CFDivider />
         <CFInput value={userInputName} onChange={(e) => setUserInputName(e.target.value)} />
         <CFButton mt="12px" onClick={onRenameProject}>
           {translate(Projects_Words["save-project"], lang)}
         </CFButton>
         <CFDivider />
-        {allProjects ? (
+        {allUid2Name ? (
           allProjectUids.length > 0 ? (
-            <CFSrollableSelect
-              value={selectedUid}
-              options={allProjectUids}
-              onOptionClick={(uid) => setSelectedUid(uid)}
-              optionConverter={(uid) => allProjects[uid]}
-            />
+            <Flex w="100%">
+              <CFSrollableSelect
+                flex={1}
+                value={selectedUid}
+                options={allProjectUids}
+                onOptionClick={(uid) => setSelectedUid(uid)}
+                optionConverter={(uid) => allUid2Name[uid]}
+              />
+              <Box as="button" w="32px" h="100%" p="4px" mx="4px" onClick={onDeleteProject}>
+                <Image src={DeleteIcon} />
+              </Box>
+            </Flex>
           ) : (
             <CFText>{translate(Projects_Words["no-projects-available"], lang)}</CFText>
           )
         ) : (
           <CFText>{translate(Projects_Words["loading-available-project"], lang)}</CFText>
         )}
         <CFButton mt="12px" onClick={onLoadProject}>
```

### Comparing `carefree-drawboard-0.0.0a9/cfdraw/.web/src/plugins/_react/SettingsPlugin.tsx` & `carefree-drawboard-0.0.1a0/cfdraw/.web/src/plugins/_react/SettingsPlugin.tsx`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,39 @@
 import { useMemo } from "react";
 import { observer } from "mobx-react-lite";
 import { Box, Checkbox, Flex } from "@chakra-ui/react";
 
 import { getRandomHash, Lang } from "@carefree0910/core";
 import {
-  BoardStore,
   langDescriptions,
   langStore,
   switchLangTo,
   translate,
-  useGlobalTransform,
   useIsReady,
 } from "@carefree0910/business";
 
-import { allAvailablePlugins, IPlugin } from "@/schema/plugins";
+import { allReactPlugins, IPlugin } from "@/schema/plugins";
 import { Plugins_Words } from "@/lang/plugins";
 import { Settings_Words } from "@/lang/settings";
 import { stripHashFromIdentifier } from "@/utils/misc";
 import { uiStore } from "@/stores/ui";
-import { usePythonPluginSettings } from "@/stores/_python";
+import { usePythonPluginSettings } from "@/stores/settings";
 import {
-  pluginIsVisible,
-  pythonPluginIsVisible,
+  useReactPluginIsVisible,
+  usePythonPluginIsVisible,
   setPythonPluginVisible,
-  setPluginVisible,
-} from "@/stores/pluginVisible";
+  setReactPluginVisible,
+} from "@/stores/pluginsInfo";
+import { parseIStr } from "@/actions/i18n";
 import { hideAllPlugins, showAllPlugins } from "@/actions/managePlugins";
 import CFButton from "@/components/CFButton";
 import CFSelect from "@/components/CFSelect";
-import CFSlider from "@/components/CFSlider";
 import CFDivider from "@/components/CFDivider";
 import CFHeading from "@/components/CFHeading";
+import { CFGlobalScaleSlider } from "@/components/CFSlider";
 import { drawboardPluginFactory } from "../utils/factory";
 import Render from "../components/Render";
 
 const SettingsPlugin = ({ pluginInfo, ...props }: IPlugin) => {
   const id = useMemo(() => `settings_${getRandomHash()}`, []);
   const lang = langStore.tgt;
   const commonProps = { fontWeight: 400, size: "md" };
@@ -56,58 +55,54 @@
           />
         </Box>
         {/* globalScale settings */}
         {useIsReady() && (
           <Box mt="24px">
             <CFHeading>{translate(Settings_Words["global-scale-header"], lang)}</CFHeading>
             <CFDivider />
-            <CFSlider
-              min={BoardStore.board.options.minScale}
-              max={BoardStore.board.options.maxScale}
-              step={0.001}
-              value={useGlobalTransform().globalScale}
-              scale="logarithmic"
-              onSliderChange={(value) => BoardStore.api.setGlobalScale(value)}
-            />
+            <CFGlobalScaleSlider />
           </Box>
         )}
-        {/* plugin settings */}
+        {/* plugin visible settings */}
         <Box mt="12px" pb="12px">
           <CFHeading>{translate(Settings_Words["plugins-header"], lang)}</CFHeading>
           <CFDivider />
           <Flex w="100%" gap="8px" direction="column" justifyContent="space-around">
-            {allAvailablePlugins
+            {allReactPlugins
               .filter((plugin) => !["settings", "undo", "redo"].includes(plugin))
               .map((plugin, i) => {
-                const pIsVisible = pluginIsVisible(plugin);
+                const pIsVisible = useReactPluginIsVisible(plugin);
                 return (
                   <Checkbox
                     key={`plugin-${i}`}
                     value={plugin}
                     isChecked={pIsVisible}
-                    onChange={() => setPluginVisible(plugin, !pIsVisible)}
+                    onChange={() => setReactPluginVisible(plugin, !pIsVisible)}
                     {...commonProps}
                     disabled={disablePluginSettings}>
                     {translate(Plugins_Words[plugin], lang)}
                   </Checkbox>
                 );
               })}
             {usePythonPluginSettings().map((settings, i) => {
               const identifierWithHash = settings.props.pluginInfo.identifier;
               const identifier = stripHashFromIdentifier(identifierWithHash);
-              const pIsVisible = pythonPluginIsVisible(identifierWithHash);
+              const pIsVisible = usePythonPluginIsVisible(identifierWithHash);
               return (
                 <Checkbox
                   key={`${identifierWithHash}-${i}`}
                   value={identifier}
                   isChecked={pIsVisible}
                   onChange={() => setPythonPluginVisible(identifierWithHash, !pIsVisible)}
                   {...commonProps}
                   disabled={disablePluginSettings}>
-                  {`${translate(Plugins_Words[settings.type], lang)} (${identifier})`}
+                  {parseIStr(
+                    settings.props.pluginInfo.name ??
+                      `${translate(Plugins_Words[settings.type], lang)} (${identifier})`,
+                  )}
                 </Checkbox>
               );
             })}
             <Flex w="100%" my="6px" justifyContent="space-around">
               <CFButton onClick={() => hideAllPlugins()} isDisabled={disablePluginSettings}>
                 {translate(Settings_Words["hide-all-plugins-message"], lang)}
               </CFButton>
```

### Comparing `carefree-drawboard-0.0.0a9/cfdraw/.web/src/plugins/_react/TextEditorPlugin.tsx` & `carefree-drawboard-0.0.1a0/cfdraw/.web/src/plugins/_react/TextEditorPlugin.tsx`

 * *Files 26% similar despite different names*

```diff
@@ -1,40 +1,36 @@
-import { useMemo, useState } from "react";
+import { useEffect, useMemo, useState } from "react";
 import { observer } from "mobx-react-lite";
 import { Flex, Textarea } from "@chakra-ui/react";
 
-import { getRandomHash, isUndefined } from "@carefree0910/core";
+import { getRandomHash } from "@carefree0910/core";
 import { langStore, translate, useEditText } from "@carefree0910/business";
 
 import type { IPlugin } from "@/schema/plugins";
 import { NodeEditor_Words } from "@/lang/nodeEditor";
 import CFSlider from "@/components/CFSlider";
 import CFDivider from "@/components/CFDivider";
 import CFHeading from "@/components/CFHeading";
 import { drawboardPluginFactory } from "../utils/factory";
 import Render from "../components/Render";
 
 const TextEditorPlugin = ({ pluginInfo: { node }, ...props }: IPlugin) => {
   const id = useMemo(() => `textEditor_${getRandomHash()}`, []);
   const lang = langStore.tgt;
-  const { nodeContent, nodeFontSize } = useMemo<{
-    nodeContent?: string;
-    nodeFontSize?: number;
-  }>(() => {
-    if (!node || node.type !== "text") return {};
-    return {
-      nodeContent: node.params.content,
-      nodeFontSize: node.params.fontSize,
-    };
-  }, [node]);
-  const [content, setContent] = useState(nodeContent ?? "");
-  const [fontSize, setFontSize] = useState(nodeFontSize ?? 16);
+  const [content, setContent] = useState("");
+  const [fontSize, setFontSize] = useState(0);
   const { editContent, editFontSize } = useEditText();
+  useEffect(() => {
+    if (node?.type === "text") {
+      setContent(node.params.content);
+      setFontSize(node.params.fontSize);
+    }
+  }, [node]);
 
-  if (isUndefined(nodeContent)) return null;
+  if (node?.type !== "text") return null;
 
   return (
     <Render id={id} {...props}>
       <CFHeading>{translate(NodeEditor_Words["text-editor-plugin-header"], lang)}</CFHeading>
       <CFDivider />
       <Flex direction="column" w="100%" h="100%">
         <CFSlider
```

### Comparing `carefree-drawboard-0.0.0a9/cfdraw/.web/src/plugins/_react/UndoRedoPlugin.tsx` & `carefree-drawboard-0.0.1a0/cfdraw/.web/src/plugins/_react/UndoRedoPlugin.tsx`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import { useEffect, useMemo } from "react";
 import { observer } from "mobx-react-lite";
 
 import { getRandomHash } from "@carefree0910/core";
 import { safeRedo, safeUndo, useUndoRedoSteps } from "@carefree0910/business";
 
 import type { IPlugin } from "@/schema/plugins";
-import { setPluginVisible } from "@/stores/pluginVisible";
+import { setReactPluginVisible } from "@/stores/pluginsInfo";
 import { drawboardPluginFactory } from "../utils/factory";
 import Render from "../components/Render";
 
 const UndoPlugin = ({ pluginInfo, ...props }: IPlugin) => {
   const id = useMemo(() => `undo_${getRandomHash()}`, []);
   const { undoSteps } = useUndoRedoSteps();
-  useEffect(() => setPluginVisible("undo", undoSteps > 0), [undoSteps]);
+  useEffect(() => setReactPluginVisible("undo", undoSteps > 0), [undoSteps]);
 
   return <Render id={id} onFloatingButtonClick={async () => safeUndo()} {...props} />;
 };
 const RedoPlugin = ({ pluginInfo, ...props }: IPlugin) => {
   const id = useMemo(() => `redo_${getRandomHash()}`, []);
   const { redoSteps } = useUndoRedoSteps();
-  useEffect(() => setPluginVisible("redo", redoSteps > 0), [redoSteps]);
+  useEffect(() => setReactPluginVisible("redo", redoSteps > 0), [redoSteps]);
 
   return <Render id={id} onFloatingButtonClick={async () => safeRedo()} {...props} />;
 };
 
 drawboardPluginFactory.register("undo", true)(observer(UndoPlugin));
 drawboardPluginFactory.register("redo", true)(observer(RedoPlugin));
```

### Comparing `carefree-drawboard-0.0.0a9/cfdraw/.web/src/plugins/utils/factory.ts` & `carefree-drawboard-0.0.1a0/cfdraw/.web/src/plugins/utils/factory.ts`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,12 @@
 import React from "react";
 
 import { Logger, checkNotExists } from "@carefree0910/core";
 
-import type {
-  AvailablePlugins,
-  AvailablePluginsAndPythonPlugins,
-  AvailablePythonPlugins,
-} from "@/schema/plugins";
+import type { ReactPlugins, AllPlugins, PythonPlugins } from "@/schema/plugins";
 
 function registerPlugin<T extends string>(
   d: Partial<Record<T, React.FC>>,
   name: T,
   overwrite: boolean = false,
 ): Function {
   return function (fn: React.FC) {
@@ -26,29 +22,29 @@
       }
     }
     d[name] = fn;
   };
 }
 
 class DrawboardPluginFactory {
-  d: Partial<Record<AvailablePlugins, React.FC>> = {};
-  python_d: Partial<Record<AvailablePythonPlugins, React.FC>> = {};
+  d: Partial<Record<ReactPlugins, React.FC>> = {};
+  python_d: Partial<Record<PythonPlugins, React.FC>> = {};
 
   constructor(public name: string) {}
 
-  register(name: AvailablePlugins, overwrite: boolean = false): Function {
+  register(name: ReactPlugins, overwrite: boolean = false): Function {
     return registerPlugin(this.d, name, overwrite);
   }
 
-  registerPython(name: AvailablePythonPlugins, overwrite: boolean = false): Function {
+  registerPython(name: PythonPlugins, overwrite: boolean = false): Function {
     return registerPlugin(this.python_d, name, overwrite);
   }
 
-  checkIsPython(name: AvailablePluginsAndPythonPlugins): name is AvailablePythonPlugins {
+  checkIsPython(name: AllPlugins): name is PythonPlugins {
     return !!(this.python_d as any)[name];
   }
 
-  get(name: AvailablePluginsAndPythonPlugins): React.FC | null {
+  get(name: AllPlugins): React.FC | null {
     return ((this.checkIsPython(name) ? this.python_d : this.d) as any)[name] ?? null;
   }
 }
 export const drawboardPluginFactory = new DrawboardPluginFactory("drawboard.plugin");
```

### Comparing `carefree-drawboard-0.0.0a9/cfdraw/.web/src/react-app-env.d.ts` & `carefree-drawboard-0.0.1a0/cfdraw/.web/src/react-app-env.d.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a9/cfdraw/.web/src/requests/actions.ts` & `carefree-drawboard-0.0.1a0/cfdraw/.web/src/requests/actions.ts`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import type { ResponseType } from "axios";
 
+import type { Dictionary } from "@carefree0910/core";
+
 import type { APISources } from "@/schema/requests";
 import { useAPI } from "./hooks";
 
 export class Requests {
   static get<R = unknown, T extends APISources = APISources>(
     source: T,
     endpoint: string,
@@ -20,19 +22,25 @@
     responseType: ResponseType = "json",
   ): Promise<R> {
     return useAPI(source)
       .post(endpoint, data, { responseType })
       .then((res) => res.data);
   }
 
-  static postBlob<R = unknown, T extends APISources = APISources>(
+  static postForm<R = unknown, T extends APISources = APISources>(
     source: T,
     endpoint: string,
-    { key, blob }: { key: string; blob: Blob },
+    data: Dictionary<string | Blob>,
   ): Promise<R> {
     const formData = new FormData();
-    formData.append(key, blob);
+    for (const [key, value] of Object.entries(data)) {
+      formData.append(key, value);
+    }
     return useAPI(source)
       .postForm(endpoint, formData)
       .then((res) => res.data);
   }
+
+  static delete<T extends APISources = APISources>(source: T, endpoint: string): Promise<void> {
+    return useAPI(source).delete(endpoint);
+  }
 }
```

### Comparing `carefree-drawboard-0.0.0a9/cfdraw/.web/src/requests/hooks.ts` & `carefree-drawboard-0.0.1a0/cfdraw/.web/src/requests/hooks.ts`

 * *Files 8% similar despite different names*

```diff
@@ -5,27 +5,27 @@
 
 import type { APISources, APIs } from "@/schema/requests";
 import type {
   IPythonOnSocketMessage,
   IPythonSocketRequest,
   IPythonSocketCallbacks,
 } from "@/schema/_python";
-import { pythonStore } from "@/stores/_python";
+import { settingsStore } from "@/stores/settings";
 import { useInceptors } from "./interceptors";
 import {
   checkSocketHookExists,
   getSocketHooks,
   pushSocketHook,
   runSocketHook,
   socketLog,
 } from "@/stores/socket";
 
 // cannot use `useMemo` here
 export function useAPI<T extends APISources>(source: T): APIs[T] {
-  const timeout = pythonStore.globalSettings?.timeout ?? 300000;
+  const timeout = settingsStore.internalSettings?.timeout ?? 300000;
   let baseURL = import.meta.env.VITE_CFDRAW_API_URL;
   if (!baseURL) {
     let backendPort = import.meta.env.VITE_CFDRAW_BE_PORT;
     if (!backendPort) {
       backendPort = 8123;
     }
     baseURL = `http://localhost:${backendPort}`;
@@ -66,22 +66,20 @@
 }
 export function useWebSocketHook<R>({
   isInvisible,
   hash: _hash,
   getMessage,
   onMessage,
   onSocketError,
-  dependencies,
   retryInterval,
   updateInterval,
   isInternal,
 }: IPythonSocketCallbacks<R> & {
   isInvisible: boolean;
   hash?: string;
-  dependencies?: any[];
   isInternal?: boolean;
 }) {
   const hash = useMemo(() => (isInvisible ? undefined : _hash), [isInvisible, _hash]);
   const onMessageWithRetry = useOnSocketMessageWithRetry(getMessage, onMessage, retryInterval);
 
   useEffect(() => {
     if (isUndefined(hash)) return;
@@ -98,9 +96,9 @@
       socketLog(
         `> current hooks: ${getSocketHooks()
           .map((h) => h.key)
           .join(", ")}`,
       );
       runSocketHook(hash);
     });
-  }, [hash, onMessageWithRetry, onSocketError, isInternal, ...(dependencies ?? [])]);
+  }, [hash, onMessageWithRetry, onSocketError, isInternal]);
 }
```

### Comparing `carefree-drawboard-0.0.0a9/cfdraw/.web/src/requests/interceptors/_python.ts` & `carefree-drawboard-0.0.1a0/cfdraw/.web/src/requests/interceptors/_python.ts`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import { Logger } from "@carefree0910/core";
 
 import type { Interceptors } from "@/schema/requests";
 
 export const _pythonInceptors: Interceptors = {
   beforeRequest: (config) => {
     if (Logger.isDebug) {
-      Logger.debug(`send to Python: ${JSON.stringify(config.data)} (${config.url})`);
+      Logger.debug(`[${config.url}] send to Python: ${JSON.stringify(config.data)}`);
     }
     config.headers["ngrok-skip-browser-warning"] = "";
     return config;
   },
   requestError(error) {
     if (Logger.isDebug) {
       Logger.debug(`send to Python error: ${error}`);
```

### Comparing `carefree-drawboard-0.0.0a9/cfdraw/.web/src/requests/interceptors/index.ts` & `carefree-drawboard-0.0.1a0/cfdraw/.web/src/requests/interceptors/index.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a9/cfdraw/.web/src/schema/_python.ts` & `carefree-drawboard-0.0.1a0/cfdraw/.web/src/schema/_python.ts`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 import type { TextareaProps } from "@chakra-ui/react";
 
 import type { Dictionary, INode, Matrix2DFields } from "@carefree0910/core";
 
-import type { IElapsedTimes, IMeta } from "./meta";
-import type { IPlugin, IPluginInfo } from "./plugins";
+import type { IElapsedTimes, IMeta, IPythonResults } from "./meta";
+import type { PythonPlugins, IMakePlugin, IPlugin, IPluginInfo } from "./plugins";
 import type { IDefinitions } from "./fields";
+import type { IStr } from "./misc";
 
 // general
 
 interface IPythonPluginInfo extends IPluginInfo, IPythonSocketIntervals {
+  name?: IStr;
   identifier: string;
+  noErrorToast?: boolean;
 }
 export interface IPythonPlugin extends IPlugin {
   pluginInfo: IPythonPluginInfo;
 }
 interface IPythonCallbacks {
   getExtraRequestData?: () => Dictionary<any>;
 }
@@ -23,14 +26,15 @@
 export interface INodeData {
   type?: INode["type"];
   // transform info
   x?: number;
   y?: number;
   w?: number;
   h?: number;
+  z?: number;
   transform?: Matrix2DFields;
   // text info
   text?: string;
   // image info
   src?: string;
   // meta
   meta?: IMeta;
@@ -39,44 +43,64 @@
 }
 
 // plugin
 
 interface IPythonPluginWithSubmitPluginInfo {
   closeOnSubmit?: boolean;
   toastOnSubmit?: boolean;
-  toastMessageOnSubmit?: string;
+  toastMessageOnSubmit?: IStr;
 }
 export interface IPythonFieldsPlugin extends IPythonPlugin {
   pluginInfo: IPythonPluginInfo &
     IPythonPluginWithSubmitPluginInfo & {
-      header?: string;
+      header?: IStr;
       definitions: IDefinitions;
       numColumns?: number;
-      noErrorToast?: boolean;
     };
 }
 
 export interface IPythonTextAreaPlugin extends IPythonPlugin {
   pluginInfo: IPythonPluginInfo & {
     noLoading?: boolean;
     textAlign?: TextareaProps["textAlign"];
   };
 }
 export interface IPythonQAPlugin extends IPythonPlugin {
   pluginInfo: IPythonPluginInfo & {
-    initialText: string;
+    initialText: IStr;
+  };
+}
+export interface IPythonChatPlugin extends IPythonPlugin {
+  pluginInfo: IPythonPluginInfo & {
+    initialText: IStr;
+  };
+}
+
+export interface IPythonPluginGroup extends IPythonPlugin {
+  pluginInfo: IPythonPluginInfo & {
+    header?: IStr;
+    plugins: IMakePlugin<PythonPlugins>[];
   };
 }
 
-export interface IPythonSocketPluginWithSubmit<R>
+export interface IUseOnPythonPluginMessage {
+  id: string;
+  pluginInfo: IPythonPluginInfo & IPythonPluginWithSubmitPluginInfo;
+  onIntermediate?: OnPythonPluginMessage;
+  onFinished: OnPythonPluginMessage;
+}
+export type OnPythonPluginMessage = (message: IPythonPluginMessage) => void;
+export interface IPythonSocketPluginWithSubmit
   extends Omit<IPythonPlugin, "id" | "pluginInfo">,
-    Omit<IPythonSocketCallbacks<R>, "getMessage"> {
+    Omit<IPythonSocketCallbacks<IPythonResults>, "getMessage" | "onMessage">,
+    IUseOnPythonPluginMessage {
   id: string;
   buttonText: string;
-  pluginInfo: IPythonPluginInfo & IPythonPluginWithSubmitPluginInfo;
+  beforeSubmit?: () => void;
+  afterSubmit?: () => void;
 }
 
 // web
 
 export interface IPythonSocketRequest {
   hash: string;
   userId: string;
@@ -96,27 +120,28 @@
        * will be used, which means the message will be sent after 1000ms by default.
        * > if you want to send the new message immediately, you can set it to 0.
        */
       newMessageInterval?: number;
     }
   | undefined
 >;
+export type IPythonOnPluginMessage = IPythonOnSocketMessage<IPythonResults>;
 export interface IPythonSocketIntervals {
   // if set, will retry in `retryInterval` ms when exception occurred
   retryInterval?: number;
   // if set, will re-send message every `updateInterval` ms
   updateInterval?: number;
 }
 export interface IPythonSocketCallbacks<R> extends IPythonCallbacks, IPythonSocketIntervals {
   getMessage: () => Promise<IPythonSocketRequest>;
   onMessage: IPythonOnSocketMessage<R>;
   onSocketError?: (err: any) => void;
 }
 
-export type PythonSocketStatus = "pending" | "working" | "finished" | "exception";
+export type PythonSocketStatus = "pending" | "working" | "finished" | "exception" | "interrupted";
 interface IPythonSocketIntermediate {
   imageList?: string[]; // intermediate images, if any
   textList?: string[]; // intermediate texts, if any
 }
 export interface IPythonSocketResponse<R> {
   progress?: number; // progress of current task, should be within [0, 1]
   intermediate?: IPythonSocketIntermediate;
@@ -127,12 +152,13 @@
   hash: string;
   status: PythonSocketStatus;
   total: number;
   pending: number;
   message: string;
   data: IPythonSocketResponse<R>;
 }
+export interface IPythonPluginMessage extends IPythonSocketMessage<IPythonResults> {}
 export interface IUseSocketPython<R>
   extends IUsePythonInfo,
     Omit<IPythonSocketCallbacks<R>, "getMessage"> {
   hash?: string;
 }
```

### Comparing `carefree-drawboard-0.0.0a9/cfdraw/.web/src/schema/meta.ts` & `carefree-drawboard-0.0.1a0/cfdraw/.web/src/schema/meta.ts`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,28 @@
 import type { Dictionary, Lang } from "@carefree0910/core";
 
 export interface IElapsedTimes {
   createTime?: number;
   startTime?: number;
   endTime?: number;
-  duration?: number;
+  pending?: number;
+  executing?: number;
+  upload?: number;
+  total?: number;
 }
 
 // general
 
-export const allMetaTypes = ["upload", "add.text", "add.sketch.path", "python.fields"] as const;
+export const allMetaTypes = [
+  "upload",
+  "add.text",
+  "add.blank",
+  "add.sketch.path",
+  "python.fields",
+] as const;
 export type MetaType = (typeof allMetaTypes)[number];
 export interface ICommonMetaData<T extends _IMetaData = _IMetaData> {
   lang?: Lang;
   alias?: string;
   elapsedTimes?: IElapsedTimes;
   from?: IMeta<T>;
 }
@@ -25,28 +34,32 @@
 
 // specific
 
 interface IUploadMetaData extends ICommonMetaData {
   w: number;
   h: number;
   url: string;
+  safe: boolean;
+  reason: string;
   isDrag: boolean;
 }
-export type IPythonResults =
-  | { type: "text"; value: string[] }
-  | { type: "image"; value: { w: number; h: number; url: string }[] };
+export type IPythonResults = (
+  | { type: "text"; value: { text: string; safe: boolean; reason: string }[] }
+  | { type: "image"; value: { w: number; h: number; url: string; safe: boolean; reason: string }[] }
+) & { extra?: Dictionary<any> };
 export type IPythonFieldsMetaData = ICommonMetaData & {
   identifier: string;
   parameters: Dictionary<any>;
   response: IPythonResults;
 };
 
 export interface IMetaData {
   upload: IUploadMetaData;
   "add.text": ICommonMetaData;
+  "add.blank": ICommonMetaData;
   "add.sketch.path": ICommonMetaData;
   "python.fields": IPythonFieldsMetaData;
 }
 
 export interface IImportMeta<T extends MetaType> {
   lang: Lang;
   type: T;
```

### Comparing `carefree-drawboard-0.0.0a9/cfdraw/.web/src/schema/plugins.ts` & `carefree-drawboard-0.0.1a0/cfdraw/.web/src/schema/plugins.ts`

 * *Files 21% similar despite different names*

```diff
@@ -1,71 +1,86 @@
 import type { RefObject } from "react";
-import type { FlexProps } from "@chakra-ui/react";
+import type { ButtonProps, FlexProps } from "@chakra-ui/react";
 
 import type { INode, NodeType, PivotType } from "@carefree0910/core";
-import type { IResponse } from "@carefree0910/business";
 
-import type { IFieldDefinition, _IFieldDefinition } from "./fields";
-import type { IPythonFieldsPlugin, IPythonQAPlugin, IPythonTextAreaPlugin } from "./_python";
+import type { IStr } from "./misc";
+import type { IFieldDefinition } from "./fields";
+import type {
+  IPythonChatPlugin,
+  IPythonFieldsPlugin,
+  IPythonPluginGroup,
+  IPythonQAPlugin,
+  IPythonTextAreaPlugin,
+} from "./_python";
 
 // general
 
-export type NodeConstraints = NodeType | "none" | "anyNode" | "singleNode" | "multiNode";
+type NodeConstraints = NodeType | "none" | "anyNode" | "singleNode" | "multiNode";
+interface NodeConstraintRules {
+  some?: NodeConstraints[];
+  every?: NodeConstraints[];
+  exactly?: NodeConstraints[];
+}
+export interface NodeConstraintSettings {
+  nodeConstraint?: NodeConstraints;
+  nodeConstraintRules?: NodeConstraintRules;
+  nodeConstraintValidator?: string;
+}
 export interface IExpandPositionInfo {
   w: number;
   h: number;
   iconW: number;
   iconH: number;
   pivot: PivotType;
   follow: boolean;
   expandOffsetX: number;
   expandOffsetY: number;
 }
 export interface IRenderInfo extends IExpandPositionInfo {
-  src?: string;
-  tooltip?: string;
+  src: IStr;
+  tooltip?: IStr;
   offsetX?: number;
   offsetY?: number;
   bgOpacity?: number;
-  renderFilter?: (info?: IResponse) => boolean;
   useModal?: boolean;
   modalOpacity?: number;
   expandProps?: FlexProps;
   isInvisible?: boolean;
 }
-export interface IFloating extends FlexProps {
+export interface IFloating extends ButtonProps {
   id: string;
+  groupId?: string; // the id of the group this floating belongs to
   renderInfo: IRenderInfo;
   noExpand?: boolean;
   onFloatingButtonClick?: () => Promise<void>;
 }
-export interface IRender extends Omit<IFloating, "id" | "renderInfo"> {
+export interface IRender extends Omit<IFloating, "id" | "renderInfo">, NodeConstraintSettings {
   id?: string;
-  nodeConstraint: NodeConstraints;
-  renderInfo: Partial<IRenderInfo> & { w: number; h: number };
+  renderInfo: Partial<Omit<IRenderInfo, "src">> & { w: number; h: number; src: string };
   containerRef?: RefObject<HTMLDivElement>;
 }
 export interface IPluginInfo {
   node: INode | null;
   nodes: INode[];
 }
 export interface IPlugin extends IRender {
   pluginInfo: IPluginInfo;
 }
 
 // specific
 
-export interface IField<T extends _IFieldDefinition> {
+export interface IField<T extends IFieldDefinition> {
   field: string;
-  definition: IFieldDefinition<T>;
+  definition: T;
 }
 
 // factory
 
-export const allAvailablePlugins = [
+export const allReactPlugins = [
   "meta",
   "settings",
   "project",
   "add",
   "arrange",
   "undo",
   "redo",
@@ -75,22 +90,24 @@
   "github",
   "email",
   "textEditor",
   "groupEditor",
   "multiEditor",
   "brush",
 ] as const;
-export const allAvailablePythonPlugins = [
+export const allPythonPlugins = [
+  "_python.fields",
   "_python.textArea",
   "_python.QA",
-  "_python.fields",
+  "_python.chat",
+  "_python.pluginGroup",
 ] as const;
-export type AvailablePlugins = (typeof allAvailablePlugins)[number];
-export type AvailablePythonPlugins = (typeof allAvailablePythonPlugins)[number];
-export type AvailablePluginsAndPythonPlugins = AvailablePlugins | AvailablePythonPlugins;
+export type ReactPlugins = (typeof allReactPlugins)[number];
+export type PythonPlugins = (typeof allPythonPlugins)[number];
+export type AllPlugins = ReactPlugins | PythonPlugins;
 
 export interface IPluginProps {
   // react plugins
   meta: IPlugin;
   settings: IPlugin;
   project: IPlugin;
   add: IPlugin;
@@ -103,19 +120,21 @@
   github: IPlugin;
   email: IPlugin;
   textEditor: IPlugin;
   groupEditor: IPlugin;
   multiEditor: IPlugin;
   brush: IPlugin;
   // python plugins
+  "_python.fields": IPythonFieldsPlugin;
   "_python.textArea": IPythonTextAreaPlugin;
   "_python.QA": IPythonQAPlugin;
-  "_python.fields": IPythonFieldsPlugin;
+  "_python.chat": IPythonChatPlugin;
+  "_python.pluginGroup": IPythonPluginGroup;
 }
 
-export interface IMakePlugin<T extends AvailablePluginsAndPythonPlugins> {
+export interface IMakePlugin<T extends AllPlugins> {
   type: T;
   props: Omit<IPluginProps[T], "containerRef" | "pluginInfo"> & {
     pluginInfo: Omit<IPluginProps[T]["pluginInfo"], "node" | "nodes">;
   };
   containerRef?: RefObject<HTMLDivElement>;
 }
```

### Comparing `carefree-drawboard-0.0.0a9/cfdraw/.web/src/schema/requests.ts` & `carefree-drawboard-0.0.1a0/cfdraw/.web/src/schema/requests.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a9/cfdraw/.web/src/stores/gridLines.ts` & `carefree-drawboard-0.0.1a0/cfdraw/.web/src/stores/gridLines.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a9/cfdraw/.web/src/stores/hooks.ts` & `carefree-drawboard-0.0.1a0/cfdraw/.web/src/stores/hooks.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a9/cfdraw/.web/src/stores/meta.ts` & `carefree-drawboard-0.0.1a0/cfdraw/.web/src/stores/meta.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a9/cfdraw/.web/src/stores/pointerEvents.ts` & `carefree-drawboard-0.0.1a0/cfdraw/.web/src/stores/pointerEvents.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a9/cfdraw/.web/src/stores/projects.ts` & `carefree-drawboard-0.0.1a0/cfdraw/.web/src/stores/projects.ts`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import { v4 as uuidv4 } from "uuid";
-import { makeObservable, observable, runInAction } from "mobx";
+import { makeObservable, observable } from "mobx";
 
 import { ABCStore } from "@carefree0910/business";
 
 import { formatTime } from "@/utils/misc";
 
 export interface IProjectsStore {
   uid: string;
@@ -28,31 +28,36 @@
 
   get info(): IPartialProjectsStore {
     return this;
   }
 }
 
 const projectsStore = new ProjectsStore();
-export const getNewProject = (): IProjectsStore => {
+export function getTimeString(time: number): string {
+  return formatTime(time, "YYYY-MM-DD HH:mm").slice(2);
+}
+export const getNewProjectInfo = (): IProjectsStore => {
   const time = new Date().getTime();
   return {
     uid: uuidv4(),
-    name: `Project ${formatTime(time, "YYYY-MM-DD HH:mm").slice(2)}`,
+    name: `Project ${getTimeString(time)}`,
     createTime: time / 1000,
     updateTime: time / 1000,
   };
 };
 export const setCurrentProjectName = (name: string) => projectsStore.updateProperty("name", name);
-export const useCurrentProject = (): IProjectsStore => {
+export const useCurrentProjectInfo = (): IProjectsStore => {
   if (!projectsStore.uid) {
-    projectsStore.updateProperty(getNewProject());
+    projectsStore.updateProperty(getNewProjectInfo());
   }
   return {
     uid: projectsStore.uid!,
     name: projectsStore.name!,
     createTime: projectsStore.createTime!,
     updateTime: projectsStore.updateTime!,
   };
 };
+export const getNewUpdateTime = () => new Date().getTime() / 1000;
 export const updateCurrentProjectUpdateTime = () =>
-  projectsStore.updateProperty("updateTime", new Date().getTime() / 1000);
-export const updateCurrentProject = (data: IProjectsStore) => projectsStore.updateProperty(data);
+  projectsStore.updateProperty("updateTime", getNewUpdateTime());
+export const updateCurrentProjectInfo = (data: IProjectsStore) =>
+  projectsStore.updateProperty(data);
```

### Comparing `carefree-drawboard-0.0.0a9/cfdraw/.web/src/stores/socket.ts` & `carefree-drawboard-0.0.1a0/cfdraw/.web/src/stores/socket.ts`

 * *Files 8% similar despite different names*

```diff
@@ -5,17 +5,16 @@
 import { ABCStore } from "@carefree0910/business";
 
 import type {
   IPythonSocketRequest,
   IPythonSocketMessage,
   IPythonOnSocketMessage,
 } from "@/schema/_python";
-import { pythonStore } from "@/stores/_python";
+import { settingsStore } from "@/stores/settings";
 import { useAPI } from "@/requests/hooks";
-import { removePluginMessageFromHash } from "./plugins";
 
 const DEBUG = false;
 
 interface SocketHook<R> {
   key: string;
   getMessage: () => Promise<IPythonSocketRequest>;
   onMessage: IPythonOnSocketMessage<R>;
@@ -46,49 +45,62 @@
   }
 
   get info(): ISocketStore {
     return this;
   }
 
   run(key: string) {
-    waitUntil(() => !!socketStore.socket).then(() => {
+    return waitUntil(() => !!socketStore.socket).then(() => {
       const hook = socketStore.hooks.get(key);
       if (!hook) {
         Logger.warn(`hook not found: ${key}`);
         return;
       }
       const hash = hook.key;
       socketLog(`>> send message (${hash})`);
 
       const send = () => {
-        hook.getMessage().then((data) => {
-          if (data.hash !== hash) {
-            Logger.warn("Internal error: hash mismatched.");
-            return;
-          }
-          if (this.shouldTerminate) {
-            Logger.warn("Should terminate socket connection in `send`.");
-            return;
-          }
-          socketStore.socket!.send(JSON.stringify(data));
-          socketLog(`>>> message sent (${hash})`);
-          if (hook.updateInterval && !hook.shouldTerminate) {
-            hook.timer = setTimeout(send, hook.updateInterval);
-          }
-        });
+        hook
+          .getMessage()
+          .then((data) => {
+            if (data.hash !== hash) {
+              Logger.warn("Internal error: hash mismatched.");
+              return;
+            }
+            if (this.shouldTerminate) {
+              Logger.warn("Should terminate socket connection in `send`.");
+              return;
+            }
+            socketStore.socket!.send(JSON.stringify(data));
+            socketLog(`>>> message sent (${hash})`);
+            if (hook.updateInterval && !hook.shouldTerminate) {
+              hook.timer = setTimeout(send, hook.updateInterval);
+            }
+          })
+          .catch((e) => {
+            hook.onMessage({
+              hash,
+              status: "interrupted",
+              message: e.message,
+              total: 0,
+              pending: 0,
+              data: {},
+            });
+          });
       };
 
       hook.shouldTerminate = false;
       send();
     });
   }
 }
 
 const socketStore = new SocketStore();
 export const socketLog = (...args: any[]) => DEBUG && console.log(...args);
+export const getSocketHook = (hash: string) => socketStore.hooks.get(hash);
 export const getSocketHooks = () => socketStore.hooks;
 export const runSocketHook = (key: string) => socketStore.run(key);
 export const pushSocketHook = <R>(hook: SocketHook<R>) => {
   return waitUntil(() => !!socketStore.socket).then(() => {
     // need to wait until socket is ready, to avoid hooks being pushed too early that
     // `runSocketHook` will be executed twice (one at `onopen`, other at `useWebSocketHook`)
     const hooks = socketStore.hooks.clone();
@@ -98,31 +110,42 @@
 };
 export const removeSocketHooks = (...hashes: string[]) => {
   const hooks = socketStore.hooks;
   hashes.forEach((hash) => {
     const hook = hooks.remove(hash);
     hook.shouldTerminate = true;
     clearTimeout(hook.timer);
-    removePluginMessageFromHash(hash);
   });
   socketStore.updateProperty("hooks", hooks);
 };
 export const checkSocketHookExists = (key: string) => {
   return socketStore.hooks.has(key);
 };
+export const runOneTimeSocketHook = <R>(hook: SocketHook<R>) => {
+  const onMessage: IPythonOnSocketMessage<R> = (data) => {
+    return hook.onMessage(data).then((res) => {
+      if (res && res.newMessage) {
+        Logger.warn("One-time socket hook should not return newMessage.");
+      }
+      removeSocketHooks(hook.key);
+      return {};
+    });
+  };
+  return pushSocketHook({ ...hook, onMessage }).then(() => runSocketHook(hook.key));
+};
 
 const log = socketLog;
 interface IUseWebSocket {
   interval?: number;
 }
 export function useWebSocket(opt?: IUseWebSocket) {
   const interval = opt?.interval ?? 1000;
   const baseURL = useAPI("_python").defaults.baseURL!;
   const socketURL = baseURL.replace("http", "ws").replace("https", "wss");
-  const socketEndpoint = pythonStore.globalSettings?.socketEndpoint ?? "/ws";
+  const socketEndpoint = settingsStore.internalSettings?.socketEndpoint ?? "/ws";
 
   useEffect(() => {
     function _connect() {
       log("connecting...");
       socket = new WebSocket(`${socketURL}${socketEndpoint}`);
       socket.onopen = () => {
         log("> onopen");
```

### Comparing `carefree-drawboard-0.0.0a9/cfdraw/.web/src/stores/ui.ts` & `carefree-drawboard-0.0.1a0/cfdraw/.web/src/stores/ui.ts`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import { makeObservable, observable, runInAction } from "mobx";
 
 import type { Dictionary } from "@carefree0910/core";
 import { ABCStore } from "@carefree0910/business";
 
-import type { AvailablePlugins } from "@/schema/plugins";
+import type { ReactPlugins } from "@/schema/plugins";
 import { reactPluginSettings } from "@/_settings";
 import {
-  pluginIsVisible,
-  pythonPluginIsVisible,
-  setPluginVisible,
+  useReactPluginIsVisible,
+  usePythonPluginIsVisible,
+  setReactPluginVisible,
   setPythonPluginVisible,
-} from "./pluginVisible";
-import { usePythonPluginSettings } from "./_python";
+} from "./pluginsInfo";
+import { usePythonPluginSettings } from "./settings";
 
 export interface IUIStore {
   disablePluginSettings: boolean;
 }
 class UIStore extends ABCStore<IUIStore> implements IUIStore {
   disablePluginSettings: boolean = false;
 
@@ -38,31 +38,31 @@
   static pythonVisibleBackup?: Dictionary<boolean>;
 
   static updateVisibleBackup() {
     this.visibleBackup = {};
     this.pythonVisibleBackup = {};
     for (const { type } of reactPluginSettings) {
       if (type !== "settings") {
-        this.visibleBackup[type] = pluginIsVisible(type);
+        this.visibleBackup[type] = useReactPluginIsVisible(type);
       }
     }
     for (const {
       props: {
         pluginInfo: { identifier },
       },
     } of usePythonPluginSettings()) {
-      this.pythonVisibleBackup[identifier] = pythonPluginIsVisible(identifier);
+      this.pythonVisibleBackup[identifier] = usePythonPluginIsVisible(identifier);
     }
   }
 
   static restoreVisibleBackup() {
     runInAction(() => {
       if (this.visibleBackup) {
         Object.entries(this.visibleBackup).forEach(([plugin, visible]) => {
-          setPluginVisible(plugin as AvailablePlugins, visible);
+          setReactPluginVisible(plugin as ReactPlugins, visible);
         });
       }
       if (this.pythonVisibleBackup) {
         Object.entries(this.pythonVisibleBackup).forEach(([identifier, visible]) => {
           setPythonPluginVisible(identifier, visible);
         });
       }
```

### Comparing `carefree-drawboard-0.0.0a9/cfdraw/.web/src/utils/event.ts` & `carefree-drawboard-0.0.1a0/cfdraw/.web/src/utils/event.ts`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import type { Dictionary } from "@carefree0910/core";
+
 export interface Listener<T> {
   (event: T): any;
 }
 
 export interface Disposable {
   dispose: () => void;
 }
@@ -31,7 +33,17 @@
     if (this.listenersOncer.length > 0) {
       const toCall = this.listenersOncer;
       this.listenersOncer = [];
       toCall.forEach((listener) => listener(event));
     }
   };
 }
+
+type GlobalEventType = "newProject";
+interface GlobalEventData {
+  newProject: undefined;
+}
+export interface IGlobalEvent<T extends GlobalEventType = GlobalEventType> {
+  type: T;
+  data: GlobalEventData[T];
+}
+export const globalEvent = new Event<IGlobalEvent>();
```

### Comparing `carefree-drawboard-0.0.0a9/cfdraw/.web/src/utils/misc.ts` & `carefree-drawboard-0.0.1a0/cfdraw/.web/src/utils/misc.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a9/cfdraw/.web/src/utils/toast.ts` & `carefree-drawboard-0.0.1a0/cfdraw/.web/src/utils/toast.ts`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import { ReactNode } from "react";
 import { makeObservable, observable } from "mobx";
 import { createStandaloneToast, UseToastOptions } from "@chakra-ui/toast";
 
 import { isUndefined } from "@carefree0910/core";
 import { ABCStore, langStore, translate } from "@carefree0910/business";
-
 import { settingsStore } from "@/stores/settings";
 
 export interface IToastStore {
   timer: any;
 }
 class ToastStore extends ABCStore<IToastStore> implements IToastStore {
   timer: any;
@@ -56,15 +55,15 @@
       },
       ...useToastOptions,
     });
   };
 
   let { duration, timeout, useToastOptions } = opt ?? {};
   if (status === "info" && isUndefined(timeout)) {
-    timeout = settingsStore.defaultInfoTimeout;
+    timeout = settingsStore.boardSettings?.globalSettings?.defaultInfoTimeout;
   }
   if (!isUndefined(timeout)) {
     toastStore.updateProperty("timer", setTimeout(_toast, timeout));
   } else {
     clearTimeout(toastStore.timer);
     _toast();
   }
```

### Comparing `carefree-drawboard-0.0.0a9/cfdraw/.web/tsconfig.json` & `carefree-drawboard-0.0.1a0/cfdraw/.web/tsconfig.json`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a9/cfdraw/.web/vite.config.ts` & `carefree-drawboard-0.0.1a0/cfdraw/.web/vite.config.ts`

 * *Files 7% similar despite different names*

```diff
@@ -46,15 +46,14 @@
   build: {
     rollupOptions: {
       output: {
         manualChunks: {
           axios: ["axios"],
           jszip: ["jszip"],
           react: ["react", "react-dom"],
-          opentype: ["opentype.js"],
           "chakra-ui": ["@chakra-ui/react", "@chakra-ui/icons"],
           svgdotjs: [
             "@svgdotjs/svg.js",
             "@svgdotjs/svg.filter.js",
             "@svgdotjs/svg.topath.js",
             "@svgdotjs/svg.topoly.js",
           ],
```

### Comparing `carefree-drawboard-0.0.0a9/cfdraw/.web/yarn.lock` & `carefree-drawboard-0.0.1a0/cfdraw/.web/yarn.lock`

 * *Files 0% similar despite different names*

```diff
@@ -213,41 +213,41 @@
   resolved "https://registry.yarnpkg.com/@babel/types/-/types-7.21.4.tgz#2d5d6bb7908699b3b416409ffd3b5daa25b030d4"
   integrity sha512-rU2oY501qDxE8Pyo7i/Orqma4ziCOrby0/9mvbDUGEfvZjb279Nk9k19e2fiCxHbRRpY2ZyrgW1eq22mvmOIzA==
   dependencies:
     "@babel/helper-string-parser" "^7.19.4"
     "@babel/helper-validator-identifier" "^7.19.1"
     to-fast-properties "^2.0.0"
 
-"@carefree0910/business@~0.4.10-alpha.4":
-  version "0.4.10-alpha.4"
-  resolved "https://registry.yarnpkg.com/@carefree0910/business/-/business-0.4.10-alpha.4.tgz#0f042da795388edbbab4de82b1d4e71c38e65594"
-  integrity sha512-B5plfUzIyuwB7N5w0jDpscZURsIgLPJgHsIyocBJcM7LPGMKrlmI8a6Em9Rel3gzjVGUu8TDLAtVkGuXy8uZEg==
-  dependencies:
-    "@carefree0910/core" "~0.4.10-alpha.1"
-    "@carefree0910/svg" "~0.4.10-alpha.3"
-
-"@carefree0910/core@~0.4.10-alpha.1":
-  version "0.4.10-alpha.1"
-  resolved "https://registry.yarnpkg.com/@carefree0910/core/-/core-0.4.10-alpha.1.tgz#8a1c579b7073a2119c8f30dae93bc1d1a21a3dbd"
-  integrity sha512-bjKvuFAHawgNW/avS/vOh/J70MCw/Lu+04cQvlVmqzYxlOGAZPKsRFNtYgTO2CNo6vgRt3sa+WpnBXibWssw2Q==
-
-"@carefree0910/native@~0.4.10-alpha.4":
-  version "0.4.10-alpha.4"
-  resolved "https://registry.yarnpkg.com/@carefree0910/native/-/native-0.4.10-alpha.4.tgz#b9eedf92119b072e90ff0244d1b5f4f4da71967f"
-  integrity sha512-feNfSuqVRt/inXpTK+WDTxKoCuDXiG3YQ9kFBH3YDw/uX1tn5HRWZGQpkfMiXBTNdi4rqk62zWR3IuXSAjKTfg==
-  dependencies:
-    "@carefree0910/core" "~0.4.10-alpha.1"
-    "@carefree0910/svg" "~0.4.10-alpha.3"
-
-"@carefree0910/svg@~0.4.10-alpha.3":
-  version "0.4.10-alpha.3"
-  resolved "https://registry.yarnpkg.com/@carefree0910/svg/-/svg-0.4.10-alpha.3.tgz#790a90eda3b9e4a30d96183450d1d1314ca53f68"
-  integrity sha512-QdeK8DQTPAp6JPb1xac0gMGEWN22H0boNSw76HlTmJ9x/ZdpRMNj24+nv5wKF+MOPu/xfNc+CKupBD76jWa6FQ==
+"@carefree0910/business@~0.5.1-alpha.3":
+  version "0.5.1-alpha.3"
+  resolved "https://registry.yarnpkg.com/@carefree0910/business/-/business-0.5.1-alpha.3.tgz#acd1d003402247d849f8dc8d91b7a1f3433cca19"
+  integrity sha512-f2VkJeBy+GXgc8DsWTG9QQ2/hk8F1iL7rX3EOR1fYLghljP5oP/d3qFfcuKxFUOnCMfte/UhIoqGzu2q6HlP4A==
+  dependencies:
+    "@carefree0910/core" "^0.5.1-alpha.3"
+    "@carefree0910/svg" "^0.5.1-alpha.3"
+
+"@carefree0910/core@^0.5.1-alpha.3", "@carefree0910/core@~0.5.1-alpha.3":
+  version "0.5.1-alpha.3"
+  resolved "https://registry.yarnpkg.com/@carefree0910/core/-/core-0.5.1-alpha.3.tgz#602e2331bdeb7d3bb7b364ba4059a18d11262fb9"
+  integrity sha512-FYXTZwlYCTwoW0KrnRe2QsaRGJCXU27dOdoC/3ASqjqi3075hGZ2welljRs5YMEIgNcpDu7dKX1ZCLbKsjTn7w==
+
+"@carefree0910/native@~0.5.1-alpha.3":
+  version "0.5.1-alpha.3"
+  resolved "https://registry.yarnpkg.com/@carefree0910/native/-/native-0.5.1-alpha.3.tgz#411a21a1b66508cede6a08bd732605db76c3d11b"
+  integrity sha512-vgoZ51dEEMCZEe4mHPTRKext0DY2ZZCQKBwqL7Fs0AxVAPA78V6nL6s9R8xZp5utxrqSyGJmOyCsH0Bqn52anw==
+  dependencies:
+    "@carefree0910/core" "^0.5.1-alpha.3"
+    "@carefree0910/svg" "^0.5.1-alpha.3"
+
+"@carefree0910/svg@^0.5.1-alpha.3", "@carefree0910/svg@~0.5.1-alpha.3":
+  version "0.5.1-alpha.3"
+  resolved "https://registry.yarnpkg.com/@carefree0910/svg/-/svg-0.5.1-alpha.3.tgz#76ce44e7893f256b2530a2b2773ddfd3ab764361"
+  integrity sha512-YfHTi2BI4GV5Zg7Kk9cxqEP0w9VwAm75kAfoieLY9YB7JNKR2wdG7jiVa8nIttnoXY38yf9YVbfwdxLhyBiqiQ==
   dependencies:
-    "@carefree0910/core" "~0.4.10-alpha.1"
+    "@carefree0910/core" "^0.5.1-alpha.3"
 
 "@chakra-ui/accordion@2.1.11":
   version "2.1.11"
   resolved "https://registry.yarnpkg.com/@chakra-ui/accordion/-/accordion-2.1.11.tgz#c6df0100c543645d0631df3aefde2ea2b8ed6313"
   integrity sha512-mfVPmqETp9pyRDHJ33AdF19oHv/LyxVzQJtlxUByuvs8Cj9QQZ2LQLg5kejm+b3mj03A7A6yfbuo3RNaI4Bhsg==
   dependencies:
     "@chakra-ui/descendant" "3.0.14"
@@ -3345,14 +3345,19 @@
 loose-envify@^1.0.0, loose-envify@^1.1.0, loose-envify@^1.4.0:
   version "1.4.0"
   resolved "https://registry.yarnpkg.com/loose-envify/-/loose-envify-1.4.0.tgz#71ee51fa7be4caec1a63839f7e682d8132d30caf"
   integrity sha512-lyuxPGr/Wfhrlem2CL/UcnUc1zcqKAImBDzukY7Y5F/yQiNdko6+fRLevlw1HgMySw7f611UIY408EtxRSoK3Q==
   dependencies:
     js-tokens "^3.0.0 || ^4.0.0"
 
+lottie-web@^5.11.0:
+  version "5.11.0"
+  resolved "https://registry.yarnpkg.com/lottie-web/-/lottie-web-5.11.0.tgz#04bb9fd6cdfbb10e586985dd666de6c727619d95"
+  integrity sha512-9vSt0AtdOH98GKDXwD5LPfFg9Pcmxt5+1BllAbudKM5iqPxpJnJUfuGaP45OyudDrESCOBgsjnntVUTygBNlzw==
+
 lru-cache@^5.1.1:
   version "5.1.1"
   resolved "https://registry.yarnpkg.com/lru-cache/-/lru-cache-5.1.1.tgz#1da27e6710271947695daf6848e847f01d84b920"
   integrity sha512-KpNARQA3Iwv+jTA0utUVVbrh+Jlrr1Fv0e56GGzAFOXN7dk/FviaDW8LHmK52DlcH4WP2n6gI8vN1aesBFgo9w==
   dependencies:
     yallist "^3.0.2"
 
@@ -3583,22 +3588,14 @@
   resolved "https://registry.yarnpkg.com/open/-/open-8.4.2.tgz#5b5ffe2a8f793dcd2aad73e550cb87b59cb084f9"
   integrity sha512-7x81NCL719oNbsq/3mh+hVrAWmFuEYUqrq/Iw3kUzH8ReypT9QQ0BLoJS7/G9k6N81XjW4qHWtjWwe/9eLy1EQ==
   dependencies:
     define-lazy-prop "^2.0.0"
     is-docker "^2.1.1"
     is-wsl "^2.2.0"
 
-opentype.js@^1.3.4:
-  version "1.3.4"
-  resolved "https://registry.yarnpkg.com/opentype.js/-/opentype.js-1.3.4.tgz#1c0e72e46288473cc4a4c6a2dc60fd7fe6020d77"
-  integrity sha512-d2JE9RP/6uagpQAVtJoF0pJJA/fgai89Cc50Yp0EJHk+eLp6QQ7gBoblsnubRULNY132I0J1QKMJ+JTbMqz4sw==
-  dependencies:
-    string.prototype.codepointat "^0.2.1"
-    tiny-inflate "^1.0.3"
-
 optionator@^0.9.1:
   version "0.9.1"
   resolved "https://registry.yarnpkg.com/optionator/-/optionator-0.9.1.tgz#4f236a6373dae0566a6d43e1326674f50c291499"
   integrity sha512-74RlY5FCnhq4jRxVUPKDaRwrVNXMqsGsiW6AJw4XK8hmtm10wC0ypZBLw5IIp85NZMr91+qd1RvvENwg7jjRFw==
   dependencies:
     deep-is "^0.1.3"
     fast-levenshtein "^2.0.6"
@@ -4042,19 +4039,14 @@
   resolved "https://registry.yarnpkg.com/string-width/-/string-width-4.2.3.tgz#269c7117d27b05ad2e536830a8ec895ef9c6d010"
   integrity sha512-wKyQRQpjJ0sIp62ErSZdGsjMJWsap5oRNihHhu6G7JVO/9jIB6UyevL+tXuOqrng8j/cxKTWyWUwvSTriiZz/g==
   dependencies:
     emoji-regex "^8.0.0"
     is-fullwidth-code-point "^3.0.0"
     strip-ansi "^6.0.1"
 
-string.prototype.codepointat@^0.2.1:
-  version "0.2.1"
-  resolved "https://registry.yarnpkg.com/string.prototype.codepointat/-/string.prototype.codepointat-0.2.1.tgz#004ad44c8afc727527b108cd462b4d971cd469bc"
-  integrity sha512-2cBVCj6I4IOvEnjgO/hWqXjqBGsY+zwPmHl12Srk9IXSZ56Jwwmy+66XO5Iut/oQVR7t5ihYdLB0GMa4alEUcg==
-
 string.prototype.matchall@^4.0.8:
   version "4.0.8"
   resolved "https://registry.yarnpkg.com/string.prototype.matchall/-/string.prototype.matchall-4.0.8.tgz#3bf85722021816dcd1bf38bb714915887ca79fd3"
   integrity sha512-6zOCOcJ+RJAQshcTvXPHoxoQGONa3e/Lqx90wUA+wEzX78sg5Bo+1tQo4N0pohS0erG9qtCqJDjNCQBjeWVxyg==
   dependencies:
     call-bind "^1.0.2"
     define-properties "^1.1.4"
@@ -4174,19 +4166,14 @@
   version "0.2.9"
   resolved "https://registry.yarnpkg.com/tiny-glob/-/tiny-glob-0.2.9.tgz#2212d441ac17928033b110f8b3640683129d31e2"
   integrity sha512-g/55ssRPUjShh+xkfx9UPDXqhckHEsHr4Vd9zX55oSdGZc/MD0m3sferOkwWtp98bv+kcVfEHtRJgBVJzelrzg==
   dependencies:
     globalyzer "0.1.0"
     globrex "^0.1.2"
 
-tiny-inflate@^1.0.3:
-  version "1.0.3"
-  resolved "https://registry.yarnpkg.com/tiny-inflate/-/tiny-inflate-1.0.3.tgz#122715494913a1805166aaf7c93467933eea26c4"
-  integrity sha512-pkY1fj1cKHb2seWDy0B16HeWyczlJA9/WW3u3c4z/NiWDsO3DOU5D7nhTLE9CF0yXv/QZFY7sEJmj24dK+Rrqw==
-
 tiny-invariant@^1.0.6:
   version "1.3.1"
   resolved "https://registry.yarnpkg.com/tiny-invariant/-/tiny-invariant-1.3.1.tgz#8560808c916ef02ecfd55e66090df23a4b7aa642"
   integrity sha512-AD5ih2NlSssTCwsMznbvwMZpJ1cbhkGd2uueNxzv2jDlEeZdU04JQfRnggJQ8DrcVBGjAsCKwFBbDlVNtEMlzw==
 
 to-fast-properties@^2.0.0:
   version "2.0.0"
```

### Comparing `carefree-drawboard-0.0.0a9/cfdraw/app/app.py` & `carefree-drawboard-0.0.1a0/cfdraw/app/app.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a9/cfdraw/app/endpoints/assets.py` & `carefree-drawboard-0.0.1a0/cfdraw/app/endpoints/assets.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a9/cfdraw/app/endpoints/project.py` & `carefree-drawboard-0.0.1a0/cfdraw/app/endpoints/project.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 from typing import List
 from pydantic import BaseModel
 from cftool.misc import print_warning
 
 from cfdraw import constants
 from cfdraw.parsers import noli
 from cfdraw.app.schema import IApp
+from cfdraw.utils.misc import get_err_msg
 from cfdraw.utils.server import raise_err
-from cfdraw.utils.server import get_err_msg
 from cfdraw.utils.server import get_responses
 from cfdraw.app.endpoints.base import IEndpoint
 
 
 suffix = ".cfdraw"
 
 
@@ -24,31 +24,32 @@
     uid: str
     name: str
     createTime: float
     updateTime: float
 
 
 class ProjectModel(ProjectMeta):
+    userId: str
     graphInfo: List[Any]
     globalTransform: noli.Matrix2D
 
 
 class SaveProjectResponse(BaseModel):
     success: bool
     message: str
 
 
-def maintain_meta(app: IApp) -> None:
-    upload_project_folder = app.config.upload_project_folder
+def maintain_meta(app: IApp, userId: str) -> None:
+    upload_project_folder = app.config.upload_project_folder / userId
     if not upload_project_folder.exists():
         upload_project_folder.mkdir(parents=True)
     existing_projects = [
-        file.absolute()
-        for file in upload_project_folder.iterdir()
-        if file.is_file() and file.suffix == suffix
+        path.absolute()
+        for path in upload_project_folder.iterdir()
+        if path.is_file() and path.suffix == suffix
     ]
     meta_path = upload_project_folder / constants.PROJECT_META_FILE
     checked = False
     if meta_path.is_file():
         try:
             with open(meta_path, "r") as f:
                 project_meta = json.load(f)
@@ -70,28 +71,34 @@
             createTime=d["createTime"],
             updateTime=d["updateTime"],
         )
     with open(meta_path, "w") as f:
         json.dump(project_meta, f)
 
 
+def maintain_all_meta(app: IApp) -> None:
+    for user_folder in app.config.upload_project_folder.iterdir():
+        if user_folder.is_dir():
+            maintain_meta(app, user_folder.name)
+
+
 def add_project_managements(app: IApp) -> None:
     @app.api.post("/save_project", responses=get_responses(SaveProjectResponse))
     def save_project(data: ProjectModel) -> SaveProjectResponse:
-        upload_project_folder = app.config.upload_project_folder
+        upload_project_folder = app.config.upload_project_folder / data.userId
         if not upload_project_folder.exists():
             upload_project_folder.mkdir(parents=True)
         try:
             file = f"{data.uid}{suffix}"
             with open(upload_project_folder / file, "w") as f:
                 json.dump(data.dict(), f)
             # maintain meta
             meta_path = upload_project_folder / constants.PROJECT_META_FILE
             if not meta_path.is_file():
-                maintain_meta(app)
+                maintain_meta(app, data.userId)
             else:
                 with open(meta_path, "r") as f:
                     meta = json.load(f)
                 meta[data.uid] = dict(
                     uid=data.uid,
                     name=data.name,
                     createTime=data.createTime,
@@ -100,60 +107,82 @@
                 with open(meta_path, "w") as f:
                     json.dump(meta, f)
         except Exception as err:
             err_msg = get_err_msg(err)
             return SaveProjectResponse(success=False, message=err_msg)
         return SaveProjectResponse(success=True, message="")
 
-    @app.api.get(
-        f"/get_project/{{uid:path}}",
-        responses=get_responses(ProjectModel),
-    )
-    async def fetch_project(uid: str) -> ProjectModel:  # type: ignore
+    @app.api.get("/get_project/", responses=get_responses(ProjectModel))
+    async def fetch_project(userId: str, uid: str) -> ProjectModel:  # type: ignore
         try:
+            upload_project_folder = app.config.upload_project_folder / userId
             file = f"{uid}{suffix}"
-            with open(app.config.upload_project_folder / file, "r") as f:
+            with open(upload_project_folder / file, "r") as f:
                 d = json.load(f)
-            # replace url if needed
-            graph = noli.parse_graph(d["graphInfo"])
-            for node in graph.all_single_nodes:
-                if node.type == noli.SingleNodeType.IMAGE:
-                    if node.renderParams is None:
-                        raise ValueError("`ImageNode` should have `renderParams`")
-                    src = node.renderParams.src
-                    # TODO: this kind of transformation should be included in the
-                    # migration stage, not runtime stage. Will be fixed in the future
-                    if src and isinstance(src, str) and src.startswith("http://"):
-                        pivot = constants.UPLOAD_IMAGE_FOLDER_NAME
-                        _, path = src.split(pivot)
-                        api_url = app.config.api_url
-                        node.renderParams.src = api_url + "/" + pivot + path
-            d["graphInfo"] = graph.dict()["root_nodes"]
+
+            # TODO: this kind of transformation should be included in the
+            # migration stage, not runtime stage. Will be fixed in the future
+
+            # # replace url if needed
+            # graph = noli.parse_graph(d["graphInfo"])
+            # for node in graph.all_single_nodes:
+            #     if node.type == noli.SingleNodeType.IMAGE:
+            #         if node.renderParams is None:
+            #             raise ValueError("`ImageNode` should have `renderParams`")
+            #         src = node.renderParams.src
+            #         if src and isinstance(src, str) and src.startswith("http://"):
+            #             pivot = constants.UPLOAD_IMAGE_FOLDER_NAME
+            #             _, path = src.split(pivot)
+            #             api_url = app.config.api_url
+            #             node.renderParams.src = api_url + "/" + pivot + path
+            # d["graphInfo"] = graph.dict()["root_nodes"]
+
             return ProjectModel(**d)
         except Exception as err:
             raise_err(err)
 
-    @app.api.get(f"/all_projects")
-    async def fetch_all_projects() -> List[ProjectMeta]:
-        upload_project_folder = app.config.upload_project_folder
+    @app.api.get("/all_projects/")
+    async def fetch_all_projects(userId: str) -> List[ProjectMeta]:
+        upload_project_folder = app.config.upload_project_folder / userId
         if not upload_project_folder.exists():
             return []
         meta_path = upload_project_folder / constants.PROJECT_META_FILE
         if not meta_path.is_file():
-            maintain_meta(app)
+            maintain_meta(app, userId)
         with open(meta_path, "r") as f:
             meta = json.load(f)
         s = sorted([(v["updateTime"], k) for k, v in meta.items()], reverse=True)
         return [ProjectMeta(**meta[k]) for _, k in s]
 
+    @app.api.delete("/projects/")
+    async def delete_project(userId: str, uid: str) -> None:
+        upload_project_folder = app.config.upload_project_folder / userId
+        if not upload_project_folder.exists():
+            return
+        file = f"{uid}{suffix}"
+        path = upload_project_folder / file
+        if path.is_file():
+            path.unlink()
+        # maintain meta
+        meta_path = upload_project_folder / constants.PROJECT_META_FILE
+        if not meta_path.is_file():
+            maintain_meta(app, userId)
+        else:
+            with open(meta_path, "r") as f:
+                meta = json.load(f)
+            if uid in meta:
+                meta.pop(uid)
+                with open(meta_path, "w") as f:
+                    json.dump(meta, f)
+
 
 class ProjectEndpoint(IEndpoint):
     def register(self) -> None:
         add_project_managements(self.app)
 
     async def on_startup(self) -> None:
-        maintain_meta(self.app)
+        maintain_all_meta(self.app)
 
 
 __all__ = [
     "ProjectEndpoint",
 ]
```

### Comparing `carefree-drawboard-0.0.0a9/cfdraw/app/endpoints/queue.py` & `carefree-drawboard-0.0.1a0/cfdraw/app/endpoints/queue.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from cftool.misc import print_error
 from cftool.misc import random_hash
 from cftool.misc import print_warning
 
 from cfdraw.app.schema import IRequestQueue
 from cfdraw.app.schema import IRequestQueueData
 from cfdraw.utils.misc import offload
-from cfdraw.utils.server import get_err_msg
+from cfdraw.utils.misc import get_err_msg
 from cfdraw.utils.data_structures import Item
 from cfdraw.utils.data_structures import QueuesInQueue
 from cfdraw.schema.plugins import ISend
 from cfdraw.schema.plugins import SocketStatus
 from cfdraw.schema.plugins import ISocketMessage
 
 
@@ -110,15 +110,15 @@
                                 ]
                             )
                             for queue_item in self._queues
                         ]
                     ),
                     "\n",
                 )
-            prefix = f"[broadcase_pending] [{hash}]"
+            prefix = f"[broadcast_pending] [{hash}]"
             success = True
             message = "null"
             try:
                 if pending is None:
                     message = (
                         f"{prefix} Internal error occurred: "
                         "cannot find pending request after submitted"
@@ -141,15 +141,15 @@
                 print_error(f"Failed to send following message: {message}")
 
     async def _broadcast_working(self, uid: str) -> bool:
         sender_pack = self._senders.get(uid)
         if sender_pack is None:
             return False
         hash, sender = sender_pack
-        prefix = f"[broadcase_working] [{hash}]"
+        prefix = f"[broadcast_working] [{hash}]"
         success = True
         try:
             message = f"{prefix} working..."
             success = await sender(
                 ISocketMessage(
                     hash=hash,
                     status=SocketStatus.WORKING,
@@ -165,15 +165,15 @@
         return success
 
     async def _broadcast_exception(self, uid: str, message: str) -> bool:
         sender_pack = self._senders.get(uid)
         if sender_pack is None:
             return False
         hash, sender = sender_pack
-        prefix = f"[broadcase_exception] [{hash}]"
+        prefix = f"[broadcast_exception] [{hash}]"
         success = True
         try:
             message = f"{prefix} {message}"
             success = await sender(ISocketMessage.make_exception(hash, message))
         except Exception as err:
             print_error(f"{prefix} {get_err_msg(err)}")
         if not success:
```

### Comparing `carefree-drawboard-0.0.0a9/cfdraw/app/endpoints/upload.py` & `carefree-drawboard-0.0.1a0/cfdraw/app/endpoints/upload.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,70 +1,106 @@
 from io import BytesIO
 from PIL import Image
+from typing import Union
 from typing import Optional
 from fastapi import File
+from fastapi import Form
 from fastapi import Response
 from fastapi import UploadFile
 from pydantic import BaseModel
+from PIL.PngImagePlugin import PngInfo
 
 from cfdraw import constants
-from cfdraw.utils import server
 from cfdraw.app.schema import IApp
-from cfdraw.utils.server import get_err_msg
+from cfdraw.utils.misc import get_err_msg
+from cfdraw.utils.server import save_image
 from cfdraw.utils.server import get_responses
+from cfdraw.utils.server import get_image_response
 from cfdraw.utils.server import get_image_response_kwargs
 from cfdraw.app.endpoints.base import IEndpoint
 
 
 class ImageDataModel(BaseModel):
     w: int
     h: int
     url: str
+    safe: bool = True
+    reason: str = ""
 
 
 class UploadImageResponse(BaseModel):
     success: bool
     message: str
     data: Optional[ImageDataModel]
 
 
 class FetchImageModel(BaseModel):
     url: str
     jpeg: bool
+    return_image: bool = False
+
+
+class ImageUploader:
+    """
+    Modify this class if you need to customize image handling processes.
+    * `upload_image`: save an image with given `contents`, will be better if `meta` can be stored.
+    * `fetch_image`: fetch an image based on `url` and `jpeg` flag.
+    """
+
+    @staticmethod
+    async def upload_image(
+        contents: Union[bytes, Image.Image],
+        meta: PngInfo,
+    ) -> ImageDataModel:
+        """
+        When this method is used in the:
+        * `upload_image` endpoint, `contents` will be a `bytes` object.
+        * `FieldsMiddleWare`, `contents` will be an `Image.Image` object.
+        """
+
+        if isinstance(contents, Image.Image):
+            image = contents
+        else:
+            image = Image.open(BytesIO(contents))
+        return ImageDataModel(**save_image(image, meta))
+
+    @staticmethod
+    async def fetch_image(data: FetchImageModel) -> Union[Response, Image.Image]:
+        file = data.url.split(constants.UPLOAD_IMAGE_FOLDER_NAME)[1][1:]  # remove '/'
+        return get_image_response(file, data.jpeg, data.return_image)
 
 
 def add_upload_image(app: IApp) -> None:
     @app.api.post("/upload_image", responses=get_responses(UploadImageResponse))
-    def upload_image(image: UploadFile = File(...)) -> UploadImageResponse:
+    async def upload_image(
+        image: UploadFile = File(),
+        userId: str = Form(),
+    ) -> UploadImageResponse:
         try:
             contents = image.file.read()
-            loaded_image = Image.open(BytesIO(contents))
-            res = server.upload_image(loaded_image)
+            meta = PngInfo()
+            meta.add_text("userId", userId)
+            data = await ImageUploader.upload_image(contents, meta)
         except Exception as err:
             err_msg = get_err_msg(err)
             return UploadImageResponse(success=False, message=err_msg, data=None)
         finally:
             image.file.close()
-        return UploadImageResponse(
-            success=True,
-            message="",
-            data=ImageDataModel(**res),
-        )
+        return UploadImageResponse(success=True, message="", data=data)
 
     @app.api.post("/fetch_image", **get_image_response_kwargs())
     async def fetch_image(data: FetchImageModel) -> Response:
-        file = data.url.split(constants.UPLOAD_IMAGE_FOLDER_NAME)[1][1:]  # remove '/'
-        return server.get_image_response(file, data.jpeg)
+        return await ImageUploader.fetch_image(data)
 
     @app.api.get(
         f"/{constants.UPLOAD_IMAGE_FOLDER_NAME}/{{file}}/",
         **get_image_response_kwargs(),
     )
     async def get_image(file: str, jpeg: bool = False) -> Response:
-        return server.get_image_response(file, jpeg)
+        return get_image_response(file, jpeg)
 
 
 class UploadEndpoint(IEndpoint):
     def register(self) -> None:
         add_upload_image(self.app)
```

### Comparing `carefree-drawboard-0.0.0a9/cfdraw/app/endpoints/websocket.py` & `carefree-drawboard-0.0.1a0/cfdraw/app/endpoints/websocket.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from cftool.misc import print_error
 from starlette.websockets import WebSocketState
 
 from cfdraw import constants
 from cfdraw.app.schema import IApp
 from cfdraw.app.schema import IRequestQueueData
 from cfdraw.utils.misc import offload
-from cfdraw.utils.server import get_err_msg
+from cfdraw.utils.misc import get_err_msg
 from cfdraw.schema.plugins import ElapsedTimes
 from cfdraw.schema.plugins import ISocketRequest
 from cfdraw.schema.plugins import ISocketMessage
 from cfdraw.app.endpoints.base import IEndpoint
 
 
 def add_websocket(app: IApp) -> None:
```

### Comparing `carefree-drawboard-0.0.0a9/cfdraw/app/schema.py` & `carefree-drawboard-0.0.1a0/cfdraw/app/schema.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a9/cfdraw/cli.py` & `carefree-drawboard-0.0.1a0/cfdraw/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,7 +90,15 @@
     folder = os.getcwd()
     set_init_codes(Path(folder), template)
 
 
 @cli.command()
 def install() -> None:
     prerequisites.install_frontend_packages(verbose=True)
+
+
+@cli.command()
+def build() -> None:
+    sys.path.insert(0, os.getcwd())
+    constants.set_env(constants.Env.PROD)
+    constants.set_unified(True)
+    exec.run_frontend_prod()
```

### Comparing `carefree-drawboard-0.0.0a9/cfdraw/config.py` & `carefree-drawboard-0.0.1a0/cfdraw/config.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,27 +3,30 @@
 from typing import Optional
 from pathlib import Path
 from importlib import import_module
 from dataclasses import dataclass
 
 from cfdraw import constants
 from cfdraw.utils.cache import cache_resource
+from cfdraw.schema.settings import BoardSettings
 
 
 @dataclass
 class Config:
     # app
     entry: str = constants.DEFAULT_ENTRY
     # frontend
     frontend_port: str = constants.FRONTEND_PORT
     # api
     backend_port: str = constants.BACKEND_PORT
     backend_hosting_url: Optional[str] = None  # this must be provided for hosting
     # upload
     upload_root: str = str(constants.UPLOAD_ROOT)
+    # board
+    board_settings: BoardSettings = BoardSettings()
     # misc
     use_react_strict_mode: bool = False
 
     @property
     def prod(self) -> bool:
         return constants.get_env() == constants.Env.PROD
```

### Comparing `carefree-drawboard-0.0.0a9/cfdraw/parsers/chakra.py` & `carefree-drawboard-0.0.1a0/cfdraw/parsers/chakra.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,15 +11,17 @@
     LEFT = "left"
     MATCH_PARENT = "match-parent"
     RIGHT = "right"
     START = "start"
 
 
 class IChakra(BaseModel):
-    p: Optional[str] = Field(None, description="Padding of the plugin")
+    w: Optional[str] = Field(None, description="Width")
+    h: Optional[str] = Field(None, description="Height")
+    p: Optional[str] = Field(None, description="Padding")
     bg: Optional[str] = Field(None, description="Background color")
     textAlign: Optional[TextAlign] = Field(None, description="Text align")
 
 
 __all__ = [
     "IChakra",
     "TextAlign",
```

### Comparing `carefree-drawboard-0.0.0a9/cfdraw/plugins/factory.py` & `carefree-drawboard-0.0.1a0/cfdraw/plugins/factory.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from typing import Type
 from typing import Callable
 from typing import NamedTuple
 
 from cfdraw.utils.data_structures import Types
 from cfdraw.schema.plugins import IPlugin
 from cfdraw.schema.plugins import IPluginSettings
+from cfdraw.schema.plugins import IPluginGroupInfo
 
 
 TPlugin = Type[IPlugin]
 
 
 class Plugins(Types[IPlugin]):
     pass
@@ -39,14 +40,19 @@
     @classmethod
     def _register(cls, d: Plugins, identifier: str) -> Callable[[TPlugin], TPlugin]:
         if identifier in d:
             raise ValueError(f"plugin {identifier} already exists")
 
         def _fn(plugin_type: TPlugin) -> TPlugin:
             plugin_type.identifier = identifier
+            pI = plugin_type().settings.pluginInfo
+            if isinstance(pI, IPluginGroupInfo):
+                for p_identifier, p_base in pI.plugins.items():
+                    p_base._in_group = True
+                    cls._register(d, p_identifier)(p_base)
             d[identifier] = plugin_type
             return plugin_type
 
         return _fn
 
     @classmethod
     def register(cls, identifier: str) -> Callable[[TPlugin], TPlugin]:
```

### Comparing `carefree-drawboard-0.0.0a9/cfdraw/plugins/middlewares/fields.py` & `carefree-drawboard-0.0.1a0/cfdraw/plugins/middlewares/response.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,30 +1,50 @@
+import time
+import asyncio
+
 from typing import List
 from typing import Union
 from PIL.Image import Image
+from PIL.PngImagePlugin import PngInfo
 
-from cfdraw.utils.server import upload_image
 from cfdraw.schema.plugins import PluginType
 from cfdraw.schema.plugins import IMiddleWare
+from cfdraw.schema.plugins import Subscription
 from cfdraw.schema.plugins import ISocketMessage
+from cfdraw.schema.plugins import ISocketRequest
+from cfdraw.app.endpoints.upload import ImageUploader
 
 
-class FieldsMiddleWare(IMiddleWare):
+class ResponseMiddleWare(IMiddleWare):
     @property
-    def subscriptions(self) -> List[PluginType]:
-        return [PluginType.FIELDS]
+    def subscriptions(self) -> Union[List[PluginType], Subscription]:
+        return Subscription.ALL
+
+    async def before(self, request: ISocketRequest) -> None:
+        await super().before(request)
+        self.request = request
 
     async def process(
         self,
         response: Union[str, List[str], Image, List[Image]],
     ) -> ISocketMessage:
         if not isinstance(response, list):
             response = [response]
         if isinstance(response[0], str):
-            return self.make_success(dict(type="text", value=response))
-        urls = [upload_image(image) for image in response]
+            return self.make_success(
+                dict(
+                    type="text",
+                    value=[dict(text=text, safe=True, reason="") for text in response],
+                )
+            )
+        meta = PngInfo()
+        meta.add_text("request", self.request.json())
+        t = time.time()
+        futures = [ImageUploader.upload_image(image, meta) for image in response]
+        urls = [data.dict() for data in await asyncio.gather(*futures)]
+        self.plugin.elapsed_times.upload = time.time() - t
         return self.make_success(dict(type="image", value=urls))
 
 
 __all__ = [
-    "FieldsMiddleWare",
+    "ResponseMiddleWare",
 ]
```

### Comparing `carefree-drawboard-0.0.0a9/cfdraw/plugins/middlewares/timer.py` & `carefree-drawboard-0.0.1a0/cfdraw/plugins/middlewares/timer.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a9/cfdraw/plugins/sync.py` & `carefree-drawboard-0.0.1a0/cfdraw/plugins/sync.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,20 +11,21 @@
         config = get_config()
         return ISocketMessage.make_success(
             data.hash,
             dict(
                 pluginSettings=[
                     plugin_type().to_plugin_settings()
                     for plugin_type in PluginFactory.plugins.values()
+                    if not plugin_type._in_group
                 ],
-                globalSettings=dict(
+                internalSettings=dict(
                     useStrictMode=config.use_react_strict_mode,
                     sockenEndpoint=str(constants.Endpoint.WEBSOCKET),
                 ),
-                boardSettings=dict(),
+                boardSettings=config.board_settings.to_filtered(),
             ),
         )
 
 
 __all__ = [
     "SyncSocketPlugin",
 ]
```

### Comparing `carefree-drawboard-0.0.0a9/cfdraw/schema/fields.py` & `carefree-drawboard-0.0.1a0/cfdraw/schema/fields.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,42 +4,53 @@
 from typing import List
 from typing import Union
 from typing import Optional
 from pydantic import Extra
 from pydantic import Field
 from pydantic import BaseModel
 
+from cfdraw.parsers.noli import IStr
+from cfdraw.parsers.chakra import IChakra
+
 
 """ This file should be identical to `src/schema/fields.ts` """
 
 
 class FieldType(str, Enum):
     TEXT = "text"
     IMAGE = "image"
     NUMBER = "number"
     SELECT = "select"
     BOOLEAN = "boolean"
+    COLOR = "color"
     LIST = "list"
     OBJECT = "object"
 
 
 class IBaseField(BaseModel):
-    props: Optional[Dict[str, Any]] = Field(None, description="Props for the component")
+    label: Optional[IStr] = Field(None, description="The label of the field")
+    tooltip: Optional[IStr] = Field(None, description="The tooltip of the field")
+    props: Optional[IChakra] = Field(None, description="Props for the component")
+    numRows: Optional[int] = Field(
+        None,
+        description="Number of rows that will be occupied by this field",
+    )
 
     class Config:
         extra = Extra.forbid
         smart_union = True
 
 
 class ITextField(IBaseField):
-    placeholder: Optional[str] = Field(None, description="Placeholder of the field")
-    type: FieldType = Field(FieldType.TEXT, description="Type of the field")
+    default: IStr = Field("", description="The default value of the field")
+    type: FieldType = Field(FieldType.TEXT, description="Type", const=True)
 
 
 class IImageField(IBaseField):
+    default: IStr = Field("", description="The default value of the field")
     type: FieldType = Field(FieldType.IMAGE, description="Type", const=True)
 
 
 class NumberScale(str, Enum):
     LINEAR = "linear"
     LOGARITHMIC = "logarithmic"
 
@@ -47,56 +58,73 @@
 class INumberField(IBaseField):
     default: float = Field(..., description="The default value of the field")
     min: Optional[float] = Field(None, description="The minimum value of the field")
     max: Optional[float] = Field(None, description="The maximum value of the field")
     step: Optional[float] = Field(None, description="The step of the field")
     isInt: Optional[bool] = Field(None, description="Whether the field is an integer")
     scale: Optional[NumberScale] = Field(None, description="The scale of the field")
-    label: Optional[str] = Field(None, description="The label of the field")
     precision: Optional[int] = Field(None, description="The precision of the field")
     type: FieldType = Field(FieldType.NUMBER, description="Type", const=True)
 
 
 class ISelectField(IBaseField):
-    values: List[str] = Field(..., description="The values of the field")
-    default: str = Field(..., description="The default value of the field")
+    values: List[IStr] = Field(..., description="The values of the field")
+    default: IStr = Field(..., description="The default value of the field")
+    isMulti: Optional[bool] = Field(None, description="Whether use multi-select")
     type: FieldType = Field(FieldType.SELECT, description="Type", const=True)
 
 
 class IBooleanField(IBaseField):
     default: bool = Field(..., description="The default value of the field")
     type: FieldType = Field(FieldType.BOOLEAN, description="Type", const=True)
 
 
+class IColorField(IBaseField):
+    default: IStr = Field("", description="The default value of the field")
+    type: FieldType = Field(FieldType.COLOR, description="Type", const=True)
+
+
 class IListField(IBaseField):
     item: "IFieldDefinition" = Field(..., description="The item of the field")
+    default: List[Any] = Field(
+        default_factory=lambda: [],
+        description="The default items of the field",
+    )
     type: FieldType = Field(FieldType.LIST, description="Type", const=True)
 
 
 class IObjectField(IBaseField):
     fields: Dict[str, "IFieldDefinition"] = Field(..., description="Sub fields")
+    default: Dict[str, Any] = Field(
+        default_factory=lambda: {},
+        description="The default object of the field",
+    )
     type: FieldType = Field(FieldType.OBJECT, description="Type", const=True)
 
 
 IFieldDefinition = Union[
     ITextField,
     IImageField,
     INumberField,
     ISelectField,
     IBooleanField,
+    IColorField,
     IListField,
     IObjectField,
 ]
 IListField.update_forward_refs()
 IObjectField.update_forward_refs()
 
 
 __all__ = [
     "FieldType",
     "ITextField",
     "IImageField",
+    "NumberScale",
     "INumberField",
     "ISelectField",
     "IBooleanField",
+    "IColorField",
     "IListField",
     "IObjectField",
+    "IFieldDefinition",
 ]
```

### Comparing `carefree-drawboard-0.0.0a9/cfdraw/schema/plugins.py` & `carefree-drawboard-0.0.1a0/cfdraw/schema/plugins.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,57 +3,93 @@
 from abc import abstractmethod
 from abc import ABC
 from PIL import Image
 from enum import Enum
 from typing import Any
 from typing import Dict
 from typing import List
+from typing import Type
+from typing import Union
 from typing import TypeVar
 from typing import Callable
 from typing import Optional
 from typing import Coroutine
 from aiohttp import ClientSession
 from pydantic import Field
 from pydantic import BaseModel
 
 from cfdraw.utils.misc import deprecated
 from cfdraw.schema.fields import IFieldDefinition
+from cfdraw.parsers.noli import IStr
 from cfdraw.parsers.noli import Matrix2D
 from cfdraw.parsers.noli import INodeType
 from cfdraw.parsers.noli import PivotType
+from cfdraw.parsers.noli import SingleNodeType
 from cfdraw.parsers.noli import NodeConstraints
+from cfdraw.parsers.noli import NodeConstraintRules
 from cfdraw.parsers.chakra import IChakra
 from cfdraw.parsers.chakra import TextAlign
 
 
 TPluginModel = TypeVar("TPluginModel")
 ISend = Callable[["ISocketMessage"], Coroutine[Any, Any, bool]]
 
 
 class PluginType(str, Enum):
-    # These types should align with the `allAvailablePythonPlugins` locates at
-    # `cfdraw/.web/src/schema/plugins.ts` (without the `_python.` prefix)
-    TEXT_AREA = "textArea"
-    QA = "QA"
-    FIELDS = "fields"
+    """
+    These types should align with the `allPythonPlugins` locates at
+    `cfdraw/.web/src/schema/plugins.ts`
+    """
+
+    FIELDS = "_python.fields"
+    TEXT_AREA = "_python.textArea"
+    QA = "_python.QA"
+    CHAT = "_python.chat"
+    PLUGIN_GROUP = "_python.pluginGroup"
+
     # this type of plugins will not be rendered on the drawboard 🎨
     _INTERNAL = "_internal"
 
 
+class ReactPluginType(str, Enum):
+    """
+    These types should align with the `allReactPlugins` locates at
+    `cfdraw/.web/src/schema/plugins.ts`
+    """
+
+    META = "meta"
+    SETTINGS = "settings"
+    PROJECT = "project"
+    ADD = "add"
+    ARRANGE = "arrange"
+    UNDO = "undo"
+    REDO = "redo"
+    DOWNLOAD = "download"
+    DELETE = "delete"
+    WIKI = "wiki"
+    GITHUB = "github"
+    EMAIL = "email"
+    TEXT_EDITOR = "textEditor"
+    GROUP_EDITOR = "groupEditor"
+    MULTI_EDITOR = "multiEditor"
+    BRUSH = "brush"
+
+
 # general
 
 
 class IPluginInfo(BaseModel):
     """
-    This should align with:
-    * `cfdraw/.web/src/schema/_python.ts`
+    This should align with the following interfaces locate at `cfdraw/.web/src/schema/_python.ts`:
+    * `IPythonPluginInfo`: `name`
     * `IPythonSocketIntervals`: `retryInterval`, `updateInterval`
     * `IPythonPluginWithSubmitPluginInfo`: `closeOnSubmit`, `toastOnSubmit`, `toastMessageOnSubmit`
     """
 
+    name: Optional[IStr] = Field(None, description="The name of the plugin")
     retryInterval: Optional[int] = Field(
         None,
         ge=0,
         description="If not None, the plugin will retry in `retryInterval` ms when exception occurred",
     )
     updateInterval: Optional[int] = Field(
         None,
@@ -64,44 +100,60 @@
         None,
         description="Whether close the expanded panel when the submit button is clicked",
     )
     toastOnSubmit: Optional[bool] = Field(
         None,
         description="Whether trigger a toast message when the submit button is clicked",
     )
-    toastMessageOnSubmit: Optional[str] = Field(
+    toastMessageOnSubmit: Optional[IStr] = Field(
         None,
         description="The message of the toast, only take effect when `toastOnSubmit` is `True`",
     )
 
 
 class IPluginSettings(IChakra):
     # required fields
-    w: int = Field(..., gt=0, description="Width of the expanded plugin")
-    h: int = Field(..., gt=0, description="Height of the expanded plugin")
-    nodeConstraint: NodeConstraints = Field(
-        ...,
+    w: int = Field(..., gt=0, description="Width of the expanded plugin")  # type: ignore
+    h: int = Field(..., gt=0, description="Height of the expanded plugin")  # type: ignore
+    # node constraints
+    nodeConstraint: Optional[NodeConstraints] = Field(
+        None,
         description="""
 Spcify when the plugin will be shown.
 > If set to 'none', the plugin will always be shown.
 > If set to 'anyNode', the plugin will be shown when any node is selected.
 > If set to 'singleNode', the plugin will be shown when only one node is selected.
 > If set to 'multiNode', the plugin will be shown when more than one node is selected.
 > Otherwise, the plugin will be shown when the selected node is of the specified type.
 """,
     )
+    nodeConstraintRules: Optional[NodeConstraintRules] = Field(
+        None,
+        description=(
+            "Specify the complex rule of the node constraint, "
+            "will work together with `nodeConstraint`, but it is often "
+            "not necessary to use `nodeConstraint` when this field is set."
+        ),
+    )
+    nodeConstraintValidator: Optional[str] = Field(
+        None,
+        description=(
+            "The universal fallback. "
+            "It specifies the name of the validator registered by `register_node_validator`."
+        ),
+    )
     # style fields
-    src: Optional[str] = Field(
+    src: Optional[IStr] = Field(
         None,
         description="""
 The image url that will be shown for the plugin.
 > If not specified, we will use a default plugin-ish image.
 """,
     )
-    tooltip: Optional[str] = Field(
+    tooltip: Optional[IStr] = Field(
         None,
         description="""
 The tooltip that will be shown for the plugin.
 > It is recommended to specify an informative tooltip, but it's also OK to leave it as `None`,
 in which case we will not show any tooltip for the plugin.
 """,
     )
@@ -137,19 +189,22 @@
         description="Extra (chakra) props of the plugin's expanded panel",
     )
     # React fields
     pluginInfo: IPluginInfo = Field(IPluginInfo(), description="Plugin info")
 
 
 class ElapsedTimes(BaseModel):
+    """This should align with `IElapsedTimes` at `cfdraw/.web/src/schema/meta.ts`"""
+
     createTime: Optional[float]
     startTime: Optional[float]
     endTime: Optional[float]
     pending: Optional[float]
     executing: Optional[float]
+    upload: Optional[float]
     total: Optional[float]
 
     def __init__(self, **data: Any):
         super().__init__(**data)
         self.createTime = time.time()
 
     def start(self) -> None:
@@ -159,14 +214,16 @@
             self.pending = start - self.createTime
 
     def end(self) -> None:
         end = time.time()
         self.endTime = end
         if self.startTime is not None:
             self.executing = end - self.startTime
+            if self.upload is not None:
+                self.executing -= self.upload
         if self.createTime is not None:
             self.total = end - self.createTime
 
 
 # web
 
 
@@ -174,27 +231,28 @@
     """This should align with `INodeData` at `src/schema/_python.ts`"""
 
     type: Optional[INodeType] = Field(None, description="Type of the node")
     x: Optional[float] = Field(None, description="X of the node")
     y: Optional[float] = Field(None, description="Y of the node")
     w: Optional[float] = Field(None, description="Width of the node")
     h: Optional[float] = Field(None, description="Height of the node")
+    z: Optional[float] = Field(None, description="Layer of the node")
     transform: Optional[Matrix2D] = Field(
         None,
         description="Transform matrix of the node",
     )
     text: Optional[str] = Field(
         None,
         description="Content of the (text) node, will be `None` if the node is not a text node",
     )
     src: Optional[str] = Field(
         None,
         description="""
 Image url of the node, will be `None` if the node is not intended to be converted to image.
-> Currently only `ImageNode` and `PathNode` will have this field defined.
+> Currently only `ImageNode` / `PathNode` / `BlankNode` will have this field defined.
 """,
     )
     meta: Optional[Dict[str, Any]] = Field(None, description="Meta of the node")
     children: Optional[List["INodeData"]] = Field(
         None,
         description=(
             "Will be a list of `INodeData` if and only if "
@@ -230,14 +288,15 @@
 class SocketStatus(str, Enum):
     """This should align with `PythonSocketStatus` at `src/schema/_python.ts`"""
 
     PENDING = "pending"
     WORKING = "working"
     FINISHED = "finished"
     EXCEPTION = "exception"
+    INTERRUPTED = "interrupted"
 
 
 class ISocketIntermediate(BaseModel):
     """This should align with `IPythonSocketIntermediate` at `src/schema/_python.ts`"""
 
     imageList: Optional[List[str]] = Field(
         None,
@@ -276,15 +335,15 @@
     message: str = Field(..., description="Message of the current status")
     data: ISocketResponse = Field(ISocketResponse(), description="Response data")
 
     @classmethod
     def make_progress(
         cls,
         hash: str,
-        progress: float,
+        progress: Optional[float] = None,
         intermediate: Optional[ISocketIntermediate] = None,
     ) -> "ISocketMessage":
         return cls(
             hash=hash,
             status=SocketStatus.WORKING,
             total=0,
             pending=0,
@@ -321,14 +380,17 @@
     hash: str
     identifier: str
     http_session: ClientSession
     # task specific
     task_hash: str
     send_message: ISend
     elapsed_times: ElapsedTimes
+    extra_responses: Dict[str, Any]
+    # internal
+    _in_group: bool = False
 
     @property
     @abstractmethod
     def type(self) -> PluginType:
         pass
 
     @property
@@ -341,27 +403,45 @@
         pass
 
     @abstractmethod
     def to_plugin_settings(self) -> Dict[str, Any]:
         pass
 
     @abstractmethod
+    def filter(self, nodes: List[INodeData], target: SingleNodeType) -> List[INodeData]:
+        pass
+
+    @abstractmethod
     async def load_image(self, src: str) -> Image.Image:
         pass
 
+    @abstractmethod
+    def send_progress(
+        self,
+        progress: float,
+        *,
+        textList: Optional[List[str]] = None,
+        imageList: Optional[List[str]] = None,
+    ) -> bool:
+        pass
+
+
+class Subscription(str, Enum):
+    ALL = "__all__"
+
 
 class IMiddleWare(ABC):
     hash: str
     plugin: IPlugin
 
     # abstract
 
     @property
     @abstractmethod
-    def subscriptions(self) -> List[PluginType]:
+    def subscriptions(self) -> Union[List[PluginType], Subscription]:
         pass
 
     @abstractmethod
     async def process(self, response: Any) -> ISocketMessage:
         """
         If `can_handle_message` is `False`, the `response` here could be anything except
         `ISocketMessage`, because in this case if `response` is already an `ISocketMessage`,
@@ -379,15 +459,18 @@
 
     # api
 
     def __init__(self, plugin: IPlugin) -> None:
         self.plugin = plugin
 
     async def __call__(self, response: Any) -> ISocketMessage:
-        if self.plugin.type not in self.subscriptions:
+        if (
+            self.subscriptions != Subscription.ALL
+            and self.plugin.type not in self.subscriptions
+        ):
             return response
         if isinstance(response, ISocketMessage) and not self.can_handle_message:
             return response
         return await self.process(response)
 
     def make_success(self, final: Dict[str, Any]) -> ISocketMessage:
         return ISocketMessage.make_success(self.hash, final)
@@ -395,15 +478,15 @@
 
 # (react) bindings
 
 
 class IFieldsPluginInfo(IPluginInfo):
     """This should align with `IPythonFieldsPlugin` at `cfdraw/.web/src/schema/_python.ts`"""
 
-    header: Optional[str] = Field(None, description="Header of the plugin")
+    header: Optional[IStr] = Field(None, description="Header of the plugin")
     definitions: Dict[str, IFieldDefinition] = Field(
         ...,
         description="Field definitions",
     )
     numColumns: Optional[int] = Field(None, description="Number of columns")
     noErrorToast: Optional[bool] = Field(None, description="Whether not to toast error")
 
@@ -416,20 +499,34 @@
     )
     textAlign: Optional[TextAlign] = Field(None, description="Text align")
 
 
 class IQAPluginInfo(IPluginInfo):
     """This should align with `IPythonQAPlugin` at `cfdraw/.web/src/schema/_python.ts`"""
 
-    initialText: str = Field(
+    initialText: IStr = Field(
         ...,
         description="The initial text to be displayed in the text area",
     )
 
 
+class IChatPluginInfo(IPluginInfo):
+    """This should align with `IPythonChatPlugin` at `cfdraw/.web/src/schema/_python.ts`"""
+
+    initialText: IStr = Field(
+        "",
+        description="The initial text to be displayed in the text area",
+    )
+
+
+class IPluginGroupInfo(IPluginInfo):
+    header: Optional[IStr] = Field(None, description="Header of the plugin group")
+    plugins: Dict[str, Type[IPlugin]] = Field(..., description="Plugins in the group")
+
+
 ## deprecated
 
 
 @deprecated("please use `ITextAreaPluginInfo` instead")
 class IHttpTextAreaPluginInfo(ITextAreaPluginInfo):
     pass
 
@@ -438,14 +535,15 @@
 class IHttpQAPluginInfo(IQAPluginInfo):
     pass
 
 
 __all__ = [
     "ISend",
     "PluginType",
+    "ReactPluginType",
     # general
     "IPluginInfo",
     "IPluginSettings",
     # web
     "INodeData",
     "ISocketRequest",
     "SocketStatus",
@@ -455,11 +553,13 @@
     # plugin interface
     "IPlugin",
     "IMiddleWare",
     "IFieldsPluginInfo",
     # bindings
     "ITextAreaPluginInfo",
     "IQAPluginInfo",
+    "IChatPluginInfo",
+    "IPluginGroupInfo",
     # deprecated
     "IHttpTextAreaPluginInfo",
     "IHttpQAPluginInfo",
 ]
```

### Comparing `carefree-drawboard-0.0.0a9/cfdraw/utils/cache.py` & `carefree-drawboard-0.0.1a0/cfdraw/utils/cache.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a9/cfdraw/utils/console.py` & `carefree-drawboard-0.0.1a0/cfdraw/utils/console.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a9/cfdraw/utils/data_structures.py` & `carefree-drawboard-0.0.1a0/cfdraw/utils/data_structures.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a9/cfdraw/utils/exec.py` & `carefree-drawboard-0.0.1a0/cfdraw/utils/exec.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a9/cfdraw/utils/misc.py` & `carefree-drawboard-0.0.1a0/cfdraw/utils/misc.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,27 @@
+import sys
 import asyncio
 import threading
 
 from typing import Any
 from typing import TypeVar
 from typing import Callable
 from typing import Coroutine
 from cftool.misc import print_error
 from cftool.misc import print_warning
 from concurrent.futures import ThreadPoolExecutor
 
-from cfdraw.utils.server import get_err_msg
-
 
 TFutureResponse = TypeVar("TFutureResponse")
 
 
+def get_err_msg(err: Exception) -> str:
+    return " | ".join(map(repr, sys.exc_info()[:2] + (str(err),)))
+
+
 def deprecated(message: str) -> Callable[[type], type]:
     def _deprecated(cls: type) -> type:
         def init(self: Any, *args: Any, **kwargs: Any) -> None:
             if not cls._warned_deprecation:  # type: ignore
                 print_warning(f"{cls.__name__} is deprecated, {message}")
                 cls._warned_deprecation = True  # type: ignore
             original_init(self, *args, **kwargs)
```

### Comparing `carefree-drawboard-0.0.0a9/cfdraw/utils/prerequisites.py` & `carefree-drawboard-0.0.1a0/cfdraw/utils/prerequisites.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a9/cfdraw/utils/processes.py` & `carefree-drawboard-0.0.1a0/cfdraw/utils/processes.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a9/cfdraw/utils/server.py` & `carefree-drawboard-0.0.1a0/cfdraw/utils/server.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,28 +1,30 @@
-import sys
 import socket
 import logging
 
 import numpy as np
 
 from io import BytesIO
 from PIL import Image
 from typing import Any
 from typing import Dict
 from typing import Type
+from typing import Union
 from typing import Optional
 from fastapi import Response
 from fastapi import HTTPException
 from pydantic import BaseModel
+from PIL.PngImagePlugin import PngInfo
 from cftool.cv import to_rgb
 from cftool.cv import np_to_bytes
 from cftool.misc import random_hash
 
 from cfdraw import constants
 from cfdraw.config import get_config
+from cfdraw.utils.misc import get_err_msg
 
 
 class RuntimeError(BaseModel):
     detail: str
 
     class Config:
         schema_extra = {
@@ -64,28 +66,24 @@
     return dict(
         responses=responses,
         response_class=Response(content=b""),
         response_description=description,
     )
 
 
-def get_err_msg(err: Exception) -> str:
-    return " | ".join(map(repr, sys.exc_info()[:2] + (str(err),)))
-
-
 def raise_err(err: Exception) -> None:
     logging.exception(err)
     raise HTTPException(status_code=constants.ERR_CODE, detail=get_err_msg(err))
 
 
-def upload_image(image: Image.Image) -> Dict[str, Any]:
+def save_image(image: Image.Image, meta: Optional[PngInfo] = None) -> Dict[str, Any]:
     w, h = image.size
     config = get_config()
     path = config.upload_image_folder / f"{random_hash()}.png"
-    image.save(path)
+    image.save(path, pnginfo=meta)
     url = f"{config.api_url}/{path.relative_to(config.upload_root_path).as_posix()}"
     return dict(w=w, h=h, url=url)
 
 
 def get_image(file: str, jpeg: bool = False) -> Image.Image:
     config = get_config()
     try:
@@ -98,21 +96,29 @@
             image = Image.open(f)
             image.load()
             return image
     except Exception as err:
         raise_err(err)
 
 
-def get_image_response(file: str, jpeg: bool = False) -> Response:
+def get_image_response(  # type: ignore
+    file: str,
+    jpeg: bool = False,
+    return_image: bool = False,
+) -> Union[Response, Image.Image]:
     config = get_config()
     try:
         image = Image.open(config.upload_image_folder / file)
         if not jpeg:
+            if return_image:
+                return image
             content = np_to_bytes(np.array(image))
         else:
             with BytesIO() as f:
                 to_rgb(image).save(f, format="JPEG", quality=95)
                 f.seek(0)
+                if return_image:
+                    return Image.open(f)
                 content = f.read()
         return Response(content=content, media_type="image/png")
     except Exception as err:
         raise_err(err)
```

### Comparing `carefree-drawboard-0.0.0a9/cfdraw/utils/template.py` & `carefree-drawboard-0.0.1a0/cfdraw/utils/template.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
 
 register_plugin("blur")(Plugin)
 {constants.DEFAULT_ENTRY} = App()
 """
 
 CONFIG_TEMPLATE = f"""
-from cfdraw.config import Config
+from cfdraw import *
 
 {constants.DEFAULT_CONFIG_ENTRY} = Config(
     # This tells us to use `cwd` to store stuffs (projects, creations, etc.)
     upload_root="./",
 )
 """
```

### Comparing `carefree-drawboard-0.0.0a9/setup.py` & `carefree-drawboard-0.0.1a0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "0.0.0-alpha.9"
+VERSION = "0.0.1-alpha.0"
 PACKAGE_NAME = "carefree-drawboard"
 
 DESCRIPTION = "🎨 Infinite Drawboard in Python"
 with open("README.md", encoding="utf-8") as f:
     LONG_DESCRIPTION = f.read()
 
 setup(
```

